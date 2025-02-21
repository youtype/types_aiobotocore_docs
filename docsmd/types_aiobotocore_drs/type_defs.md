# Type definitions

> [Index](../README.md) > [Drs](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Drs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
    type annotations stubs module [types-aiobotocore-drs](https://pypi.org/project/types-aiobotocore-drs/).



## AccountTypeDef

```python
# AccountTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import AccountTypeDef


def get_value() -> AccountTypeDef:
    return {
        "accountID": ...,
    }


# AccountTypeDef definition

class AccountTypeDef(TypedDict):
    accountID: NotRequired[str],
```

## AssociateSourceNetworkStackRequestTypeDef

```python
# AssociateSourceNetworkStackRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import AssociateSourceNetworkStackRequestTypeDef


def get_value() -> AssociateSourceNetworkStackRequestTypeDef:
    return {
        "cfnStackName": ...,
    }


# AssociateSourceNetworkStackRequestTypeDef definition

class AssociateSourceNetworkStackRequestTypeDef(TypedDict):
    cfnStackName: str,
    sourceNetworkID: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ResponseMetadataTypeDef


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

## CPUTypeDef

```python
# CPUTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import CPUTypeDef


def get_value() -> CPUTypeDef:
    return {
        "cores": ...,
    }


# CPUTypeDef definition

class CPUTypeDef(TypedDict):
    cores: NotRequired[int],
    modelName: NotRequired[str],
```

## ProductCodeTypeDef

```python
# ProductCodeTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ProductCodeTypeDef


def get_value() -> ProductCodeTypeDef:
    return {
        "productCodeId": ...,
    }


# ProductCodeTypeDef definition

class ProductCodeTypeDef(TypedDict):
    productCodeId: NotRequired[str],
    productCodeMode: NotRequired[ProductCodeModeType],  # (1)
```

1. See [:material-code-brackets: ProductCodeModeType](./literals.md#productcodemodetype) 
## CreateExtendedSourceServerRequestTypeDef

```python
# CreateExtendedSourceServerRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import CreateExtendedSourceServerRequestTypeDef


def get_value() -> CreateExtendedSourceServerRequestTypeDef:
    return {
        "sourceServerArn": ...,
    }


# CreateExtendedSourceServerRequestTypeDef definition

class CreateExtendedSourceServerRequestTypeDef(TypedDict):
    sourceServerArn: str,
    tags: NotRequired[Mapping[str, str]],
```

## LicensingTypeDef

```python
# LicensingTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LicensingTypeDef


def get_value() -> LicensingTypeDef:
    return {
        "osByol": ...,
    }


# LicensingTypeDef definition

class LicensingTypeDef(TypedDict):
    osByol: NotRequired[bool],
```

## PITPolicyRuleTypeDef

```python
# PITPolicyRuleTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import PITPolicyRuleTypeDef


def get_value() -> PITPolicyRuleTypeDef:
    return {
        "enabled": ...,
    }


# PITPolicyRuleTypeDef definition

class PITPolicyRuleTypeDef(TypedDict):
    interval: int,
    retentionDuration: int,
    units: PITPolicyRuleUnitsType,  # (1)
    enabled: NotRequired[bool],
    ruleID: NotRequired[int],
```

1. See [:material-code-brackets: PITPolicyRuleUnitsType](./literals.md#pitpolicyruleunitstype) 
## CreateSourceNetworkRequestTypeDef

```python
# CreateSourceNetworkRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import CreateSourceNetworkRequestTypeDef


def get_value() -> CreateSourceNetworkRequestTypeDef:
    return {
        "originAccountID": ...,
    }


# CreateSourceNetworkRequestTypeDef definition

class CreateSourceNetworkRequestTypeDef(TypedDict):
    originAccountID: str,
    originRegion: str,
    vpcID: str,
    tags: NotRequired[Mapping[str, str]],
```

## DataReplicationErrorTypeDef

```python
# DataReplicationErrorTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DataReplicationErrorTypeDef


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

from types_aiobotocore_drs.type_defs import DataReplicationInfoReplicatedDiskTypeDef


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
    volumeStatus: NotRequired[VolumeStatusType],  # (1)
```

1. See [:material-code-brackets: VolumeStatusType](./literals.md#volumestatustype) 
## DataReplicationInitiationStepTypeDef

```python
# DataReplicationInitiationStepTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DataReplicationInitiationStepTypeDef


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
## DeleteJobRequestTypeDef

```python
# DeleteJobRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DeleteJobRequestTypeDef


def get_value() -> DeleteJobRequestTypeDef:
    return {
        "jobID": ...,
    }


# DeleteJobRequestTypeDef definition

class DeleteJobRequestTypeDef(TypedDict):
    jobID: str,
```

## DeleteLaunchActionRequestTypeDef

```python
# DeleteLaunchActionRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DeleteLaunchActionRequestTypeDef


def get_value() -> DeleteLaunchActionRequestTypeDef:
    return {
        "actionId": ...,
    }


# DeleteLaunchActionRequestTypeDef definition

class DeleteLaunchActionRequestTypeDef(TypedDict):
    actionId: str,
    resourceId: str,
```

## DeleteLaunchConfigurationTemplateRequestTypeDef

```python
# DeleteLaunchConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DeleteLaunchConfigurationTemplateRequestTypeDef


def get_value() -> DeleteLaunchConfigurationTemplateRequestTypeDef:
    return {
        "launchConfigurationTemplateID": ...,
    }


# DeleteLaunchConfigurationTemplateRequestTypeDef definition

class DeleteLaunchConfigurationTemplateRequestTypeDef(TypedDict):
    launchConfigurationTemplateID: str,
```

## DeleteRecoveryInstanceRequestTypeDef

```python
# DeleteRecoveryInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DeleteRecoveryInstanceRequestTypeDef


def get_value() -> DeleteRecoveryInstanceRequestTypeDef:
    return {
        "recoveryInstanceID": ...,
    }


# DeleteRecoveryInstanceRequestTypeDef definition

class DeleteRecoveryInstanceRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
```

## DeleteReplicationConfigurationTemplateRequestTypeDef

```python
# DeleteReplicationConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DeleteReplicationConfigurationTemplateRequestTypeDef


def get_value() -> DeleteReplicationConfigurationTemplateRequestTypeDef:
    return {
        "replicationConfigurationTemplateID": ...,
    }


# DeleteReplicationConfigurationTemplateRequestTypeDef definition

class DeleteReplicationConfigurationTemplateRequestTypeDef(TypedDict):
    replicationConfigurationTemplateID: str,
```

## DeleteSourceNetworkRequestTypeDef

```python
# DeleteSourceNetworkRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DeleteSourceNetworkRequestTypeDef


def get_value() -> DeleteSourceNetworkRequestTypeDef:
    return {
        "sourceNetworkID": ...,
    }


# DeleteSourceNetworkRequestTypeDef definition

class DeleteSourceNetworkRequestTypeDef(TypedDict):
    sourceNetworkID: str,
```

## DeleteSourceServerRequestTypeDef

```python
# DeleteSourceServerRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DeleteSourceServerRequestTypeDef


def get_value() -> DeleteSourceServerRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# DeleteSourceServerRequestTypeDef definition

class DeleteSourceServerRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import PaginatorConfigTypeDef


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

from types_aiobotocore_drs.type_defs import DescribeJobLogItemsRequestTypeDef


def get_value() -> DescribeJobLogItemsRequestTypeDef:
    return {
        "jobID": ...,
    }


# DescribeJobLogItemsRequestTypeDef definition

class DescribeJobLogItemsRequestTypeDef(TypedDict):
    jobID: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## DescribeJobsRequestFiltersTypeDef

```python
# DescribeJobsRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeJobsRequestFiltersTypeDef


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

from types_aiobotocore_drs.type_defs import DescribeLaunchConfigurationTemplatesRequestTypeDef


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

## DescribeRecoveryInstancesRequestFiltersTypeDef

```python
# DescribeRecoveryInstancesRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeRecoveryInstancesRequestFiltersTypeDef


def get_value() -> DescribeRecoveryInstancesRequestFiltersTypeDef:
    return {
        "recoveryInstanceIDs": ...,
    }


# DescribeRecoveryInstancesRequestFiltersTypeDef definition

class DescribeRecoveryInstancesRequestFiltersTypeDef(TypedDict):
    recoveryInstanceIDs: NotRequired[Sequence[str]],
    sourceServerIDs: NotRequired[Sequence[str]],
```

## DescribeRecoverySnapshotsRequestFiltersTypeDef

```python
# DescribeRecoverySnapshotsRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeRecoverySnapshotsRequestFiltersTypeDef


def get_value() -> DescribeRecoverySnapshotsRequestFiltersTypeDef:
    return {
        "fromDateTime": ...,
    }


# DescribeRecoverySnapshotsRequestFiltersTypeDef definition

class DescribeRecoverySnapshotsRequestFiltersTypeDef(TypedDict):
    fromDateTime: NotRequired[str],
    toDateTime: NotRequired[str],
```

## RecoverySnapshotTypeDef

```python
# RecoverySnapshotTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RecoverySnapshotTypeDef


def get_value() -> RecoverySnapshotTypeDef:
    return {
        "ebsSnapshots": ...,
    }


# RecoverySnapshotTypeDef definition

class RecoverySnapshotTypeDef(TypedDict):
    expectedTimestamp: str,
    snapshotID: str,
    sourceServerID: str,
    ebsSnapshots: NotRequired[List[str]],
    timestamp: NotRequired[str],
```

## DescribeReplicationConfigurationTemplatesRequestTypeDef

```python
# DescribeReplicationConfigurationTemplatesRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeReplicationConfigurationTemplatesRequestTypeDef


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

## DescribeSourceNetworksRequestFiltersTypeDef

```python
# DescribeSourceNetworksRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeSourceNetworksRequestFiltersTypeDef


def get_value() -> DescribeSourceNetworksRequestFiltersTypeDef:
    return {
        "originAccountID": ...,
    }


# DescribeSourceNetworksRequestFiltersTypeDef definition

class DescribeSourceNetworksRequestFiltersTypeDef(TypedDict):
    originAccountID: NotRequired[str],
    originRegion: NotRequired[str],
    sourceNetworkIDs: NotRequired[Sequence[str]],
```

## DescribeSourceServersRequestFiltersTypeDef

```python
# DescribeSourceServersRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeSourceServersRequestFiltersTypeDef


def get_value() -> DescribeSourceServersRequestFiltersTypeDef:
    return {
        "hardwareId": ...,
    }


# DescribeSourceServersRequestFiltersTypeDef definition

class DescribeSourceServersRequestFiltersTypeDef(TypedDict):
    hardwareId: NotRequired[str],
    sourceServerIDs: NotRequired[Sequence[str]],
    stagingAccountIDs: NotRequired[Sequence[str]],
```

## DisconnectRecoveryInstanceRequestTypeDef

```python
# DisconnectRecoveryInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DisconnectRecoveryInstanceRequestTypeDef


def get_value() -> DisconnectRecoveryInstanceRequestTypeDef:
    return {
        "recoveryInstanceID": ...,
    }


# DisconnectRecoveryInstanceRequestTypeDef definition

class DisconnectRecoveryInstanceRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
```

## DisconnectSourceServerRequestTypeDef

```python
# DisconnectSourceServerRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DisconnectSourceServerRequestTypeDef


def get_value() -> DisconnectSourceServerRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# DisconnectSourceServerRequestTypeDef definition

class DisconnectSourceServerRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## DiskTypeDef

```python
# DiskTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DiskTypeDef


def get_value() -> DiskTypeDef:
    return {
        "bytes": ...,
    }


# DiskTypeDef definition

class DiskTypeDef(TypedDict):
    bytes: NotRequired[int],
    deviceName: NotRequired[str],
```

## SourceNetworkDataTypeDef

```python
# SourceNetworkDataTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import SourceNetworkDataTypeDef


def get_value() -> SourceNetworkDataTypeDef:
    return {
        "sourceNetworkID": ...,
    }


# SourceNetworkDataTypeDef definition

class SourceNetworkDataTypeDef(TypedDict):
    sourceNetworkID: NotRequired[str],
    sourceVpc: NotRequired[str],
    stackName: NotRequired[str],
    targetVpc: NotRequired[str],
```

## ExportSourceNetworkCfnTemplateRequestTypeDef

```python
# ExportSourceNetworkCfnTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ExportSourceNetworkCfnTemplateRequestTypeDef


def get_value() -> ExportSourceNetworkCfnTemplateRequestTypeDef:
    return {
        "sourceNetworkID": ...,
    }


# ExportSourceNetworkCfnTemplateRequestTypeDef definition

class ExportSourceNetworkCfnTemplateRequestTypeDef(TypedDict):
    sourceNetworkID: str,
```

## GetFailbackReplicationConfigurationRequestTypeDef

```python
# GetFailbackReplicationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import GetFailbackReplicationConfigurationRequestTypeDef


def get_value() -> GetFailbackReplicationConfigurationRequestTypeDef:
    return {
        "recoveryInstanceID": ...,
    }


# GetFailbackReplicationConfigurationRequestTypeDef definition

class GetFailbackReplicationConfigurationRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
```

## GetLaunchConfigurationRequestTypeDef

```python
# GetLaunchConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import GetLaunchConfigurationRequestTypeDef


def get_value() -> GetLaunchConfigurationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# GetLaunchConfigurationRequestTypeDef definition

class GetLaunchConfigurationRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## GetReplicationConfigurationRequestTypeDef

```python
# GetReplicationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import GetReplicationConfigurationRequestTypeDef


def get_value() -> GetReplicationConfigurationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# GetReplicationConfigurationRequestTypeDef definition

class GetReplicationConfigurationRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## IdentificationHintsTypeDef

```python
# IdentificationHintsTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import IdentificationHintsTypeDef


def get_value() -> IdentificationHintsTypeDef:
    return {
        "awsInstanceID": ...,
    }


# IdentificationHintsTypeDef definition

class IdentificationHintsTypeDef(TypedDict):
    awsInstanceID: NotRequired[str],
    fqdn: NotRequired[str],
    hostname: NotRequired[str],
    vmWareUuid: NotRequired[str],
```

## LaunchActionParameterTypeDef

```python
# LaunchActionParameterTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LaunchActionParameterTypeDef


def get_value() -> LaunchActionParameterTypeDef:
    return {
        "type": ...,
    }


# LaunchActionParameterTypeDef definition

class LaunchActionParameterTypeDef(TypedDict):
    type: NotRequired[LaunchActionParameterTypeType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: LaunchActionParameterTypeType](./literals.md#launchactionparametertypetype) 
## LaunchActionsRequestFiltersTypeDef

```python
# LaunchActionsRequestFiltersTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LaunchActionsRequestFiltersTypeDef


def get_value() -> LaunchActionsRequestFiltersTypeDef:
    return {
        "actionIds": ...,
    }


# LaunchActionsRequestFiltersTypeDef definition

class LaunchActionsRequestFiltersTypeDef(TypedDict):
    actionIds: NotRequired[Sequence[str]],
```

## LaunchIntoInstancePropertiesTypeDef

```python
# LaunchIntoInstancePropertiesTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LaunchIntoInstancePropertiesTypeDef


def get_value() -> LaunchIntoInstancePropertiesTypeDef:
    return {
        "launchIntoEC2InstanceID": ...,
    }


# LaunchIntoInstancePropertiesTypeDef definition

class LaunchIntoInstancePropertiesTypeDef(TypedDict):
    launchIntoEC2InstanceID: NotRequired[str],
```

## LifeCycleLastLaunchInitiatedTypeDef

```python
# LifeCycleLastLaunchInitiatedTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LifeCycleLastLaunchInitiatedTypeDef


def get_value() -> LifeCycleLastLaunchInitiatedTypeDef:
    return {
        "apiCallDateTime": ...,
    }


# LifeCycleLastLaunchInitiatedTypeDef definition

class LifeCycleLastLaunchInitiatedTypeDef(TypedDict):
    apiCallDateTime: NotRequired[str],
    jobID: NotRequired[str],
    type: NotRequired[LastLaunchTypeType],  # (1)
```

1. See [:material-code-brackets: LastLaunchTypeType](./literals.md#lastlaunchtypetype) 
## ListExtensibleSourceServersRequestTypeDef

```python
# ListExtensibleSourceServersRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ListExtensibleSourceServersRequestTypeDef


def get_value() -> ListExtensibleSourceServersRequestTypeDef:
    return {
        "stagingAccountID": ...,
    }


# ListExtensibleSourceServersRequestTypeDef definition

class ListExtensibleSourceServersRequestTypeDef(TypedDict):
    stagingAccountID: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## StagingSourceServerTypeDef

```python
# StagingSourceServerTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StagingSourceServerTypeDef


def get_value() -> StagingSourceServerTypeDef:
    return {
        "arn": ...,
    }


# StagingSourceServerTypeDef definition

class StagingSourceServerTypeDef(TypedDict):
    arn: NotRequired[str],
    hostname: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## ListStagingAccountsRequestTypeDef

```python
# ListStagingAccountsRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ListStagingAccountsRequestTypeDef


def get_value() -> ListStagingAccountsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListStagingAccountsRequestTypeDef definition

class ListStagingAccountsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import NetworkInterfaceTypeDef


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

from types_aiobotocore_drs.type_defs import OSTypeDef


def get_value() -> OSTypeDef:
    return {
        "fullString": ...,
    }


# OSTypeDef definition

class OSTypeDef(TypedDict):
    fullString: NotRequired[str],
```

## ParticipatingResourceIDTypeDef

```python
# ParticipatingResourceIDTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ParticipatingResourceIDTypeDef


def get_value() -> ParticipatingResourceIDTypeDef:
    return {
        "sourceNetworkID": ...,
    }


# ParticipatingResourceIDTypeDef definition

class ParticipatingResourceIDTypeDef(TypedDict):
    sourceNetworkID: NotRequired[str],
```

## RecoveryInstanceDataReplicationErrorTypeDef

```python
# RecoveryInstanceDataReplicationErrorTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RecoveryInstanceDataReplicationErrorTypeDef


def get_value() -> RecoveryInstanceDataReplicationErrorTypeDef:
    return {
        "error": ...,
    }


# RecoveryInstanceDataReplicationErrorTypeDef definition

class RecoveryInstanceDataReplicationErrorTypeDef(TypedDict):
    error: NotRequired[FailbackReplicationErrorType],  # (1)
    rawError: NotRequired[str],
```

1. See [:material-code-brackets: FailbackReplicationErrorType](./literals.md#failbackreplicationerrortype) 
## RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef

```python
# RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef


def get_value() -> RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef:
    return {
        "backloggedStorageBytes": ...,
    }


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
# RecoveryInstanceDataReplicationInitiationStepTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RecoveryInstanceDataReplicationInitiationStepTypeDef


def get_value() -> RecoveryInstanceDataReplicationInitiationStepTypeDef:
    return {
        "name": ...,
    }


# RecoveryInstanceDataReplicationInitiationStepTypeDef definition

class RecoveryInstanceDataReplicationInitiationStepTypeDef(TypedDict):
    name: NotRequired[RecoveryInstanceDataReplicationInitiationStepNameType],  # (1)
    status: NotRequired[RecoveryInstanceDataReplicationInitiationStepStatusType],  # (2)
```

1. See [:material-code-brackets: RecoveryInstanceDataReplicationInitiationStepNameType](./literals.md#recoveryinstancedatareplicationinitiationstepnametype) 
2. See [:material-code-brackets: RecoveryInstanceDataReplicationInitiationStepStatusType](./literals.md#recoveryinstancedatareplicationinitiationstepstatustype) 
## RecoveryInstanceDiskTypeDef

```python
# RecoveryInstanceDiskTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RecoveryInstanceDiskTypeDef


def get_value() -> RecoveryInstanceDiskTypeDef:
    return {
        "bytes": ...,
    }


# RecoveryInstanceDiskTypeDef definition

class RecoveryInstanceDiskTypeDef(TypedDict):
    bytes: NotRequired[int],
    ebsVolumeID: NotRequired[str],
    internalDeviceName: NotRequired[str],
```

## RecoveryInstanceFailbackTypeDef

```python
# RecoveryInstanceFailbackTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RecoveryInstanceFailbackTypeDef


def get_value() -> RecoveryInstanceFailbackTypeDef:
    return {
        "agentLastSeenByServiceDateTime": ...,
    }


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
# RecoveryLifeCycleTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RecoveryLifeCycleTypeDef


def get_value() -> RecoveryLifeCycleTypeDef:
    return {
        "apiCallDateTime": ...,
    }


# RecoveryLifeCycleTypeDef definition

class RecoveryLifeCycleTypeDef(TypedDict):
    apiCallDateTime: NotRequired[datetime],
    jobID: NotRequired[str],
    lastRecoveryResult: NotRequired[RecoveryResultType],  # (1)
```

1. See [:material-code-brackets: RecoveryResultType](./literals.md#recoveryresulttype) 
## ReplicationConfigurationReplicatedDiskTypeDef

```python
# ReplicationConfigurationReplicatedDiskTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ReplicationConfigurationReplicatedDiskTypeDef


def get_value() -> ReplicationConfigurationReplicatedDiskTypeDef:
    return {
        "deviceName": ...,
    }


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
## RetryDataReplicationRequestTypeDef

```python
# RetryDataReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RetryDataReplicationRequestTypeDef


def get_value() -> RetryDataReplicationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# RetryDataReplicationRequestTypeDef definition

class RetryDataReplicationRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## ReverseReplicationRequestTypeDef

```python
# ReverseReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ReverseReplicationRequestTypeDef


def get_value() -> ReverseReplicationRequestTypeDef:
    return {
        "recoveryInstanceID": ...,
    }


# ReverseReplicationRequestTypeDef definition

class ReverseReplicationRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
```

## SourceCloudPropertiesTypeDef

```python
# SourceCloudPropertiesTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import SourceCloudPropertiesTypeDef


def get_value() -> SourceCloudPropertiesTypeDef:
    return {
        "originAccountID": ...,
    }


# SourceCloudPropertiesTypeDef definition

class SourceCloudPropertiesTypeDef(TypedDict):
    originAccountID: NotRequired[str],
    originAvailabilityZone: NotRequired[str],
    originRegion: NotRequired[str],
    sourceOutpostArn: NotRequired[str],
```

## StagingAreaTypeDef

```python
# StagingAreaTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StagingAreaTypeDef


def get_value() -> StagingAreaTypeDef:
    return {
        "errorMessage": ...,
    }


# StagingAreaTypeDef definition

class StagingAreaTypeDef(TypedDict):
    errorMessage: NotRequired[str],
    stagingAccountID: NotRequired[str],
    stagingSourceServerArn: NotRequired[str],
    status: NotRequired[ExtensionStatusType],  # (1)
```

1. See [:material-code-brackets: ExtensionStatusType](./literals.md#extensionstatustype) 
## StartFailbackLaunchRequestTypeDef

```python
# StartFailbackLaunchRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartFailbackLaunchRequestTypeDef


def get_value() -> StartFailbackLaunchRequestTypeDef:
    return {
        "recoveryInstanceIDs": ...,
    }


# StartFailbackLaunchRequestTypeDef definition

class StartFailbackLaunchRequestTypeDef(TypedDict):
    recoveryInstanceIDs: Sequence[str],
    tags: NotRequired[Mapping[str, str]],
```

## StartRecoveryRequestSourceServerTypeDef

```python
# StartRecoveryRequestSourceServerTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartRecoveryRequestSourceServerTypeDef


def get_value() -> StartRecoveryRequestSourceServerTypeDef:
    return {
        "recoverySnapshotID": ...,
    }


# StartRecoveryRequestSourceServerTypeDef definition

class StartRecoveryRequestSourceServerTypeDef(TypedDict):
    sourceServerID: str,
    recoverySnapshotID: NotRequired[str],
```

## StartReplicationRequestTypeDef

```python
# StartReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartReplicationRequestTypeDef


def get_value() -> StartReplicationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# StartReplicationRequestTypeDef definition

class StartReplicationRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## StartSourceNetworkRecoveryRequestNetworkEntryTypeDef

```python
# StartSourceNetworkRecoveryRequestNetworkEntryTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartSourceNetworkRecoveryRequestNetworkEntryTypeDef


def get_value() -> StartSourceNetworkRecoveryRequestNetworkEntryTypeDef:
    return {
        "cfnStackName": ...,
    }


# StartSourceNetworkRecoveryRequestNetworkEntryTypeDef definition

class StartSourceNetworkRecoveryRequestNetworkEntryTypeDef(TypedDict):
    sourceNetworkID: str,
    cfnStackName: NotRequired[str],
```

## StartSourceNetworkReplicationRequestTypeDef

```python
# StartSourceNetworkReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartSourceNetworkReplicationRequestTypeDef


def get_value() -> StartSourceNetworkReplicationRequestTypeDef:
    return {
        "sourceNetworkID": ...,
    }


# StartSourceNetworkReplicationRequestTypeDef definition

class StartSourceNetworkReplicationRequestTypeDef(TypedDict):
    sourceNetworkID: str,
```

## StopFailbackRequestTypeDef

```python
# StopFailbackRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StopFailbackRequestTypeDef


def get_value() -> StopFailbackRequestTypeDef:
    return {
        "recoveryInstanceID": ...,
    }


# StopFailbackRequestTypeDef definition

class StopFailbackRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
```

## StopReplicationRequestTypeDef

```python
# StopReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StopReplicationRequestTypeDef


def get_value() -> StopReplicationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# StopReplicationRequestTypeDef definition

class StopReplicationRequestTypeDef(TypedDict):
    sourceServerID: str,
```

## StopSourceNetworkReplicationRequestTypeDef

```python
# StopSourceNetworkReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StopSourceNetworkReplicationRequestTypeDef


def get_value() -> StopSourceNetworkReplicationRequestTypeDef:
    return {
        "sourceNetworkID": ...,
    }


# StopSourceNetworkReplicationRequestTypeDef definition

class StopSourceNetworkReplicationRequestTypeDef(TypedDict):
    sourceNetworkID: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TerminateRecoveryInstancesRequestTypeDef

```python
# TerminateRecoveryInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import TerminateRecoveryInstancesRequestTypeDef


def get_value() -> TerminateRecoveryInstancesRequestTypeDef:
    return {
        "recoveryInstanceIDs": ...,
    }


# TerminateRecoveryInstancesRequestTypeDef definition

class TerminateRecoveryInstancesRequestTypeDef(TypedDict):
    recoveryInstanceIDs: Sequence[str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateFailbackReplicationConfigurationRequestTypeDef

```python
# UpdateFailbackReplicationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import UpdateFailbackReplicationConfigurationRequestTypeDef


def get_value() -> UpdateFailbackReplicationConfigurationRequestTypeDef:
    return {
        "recoveryInstanceID": ...,
    }


# UpdateFailbackReplicationConfigurationRequestTypeDef definition

class UpdateFailbackReplicationConfigurationRequestTypeDef(TypedDict):
    recoveryInstanceID: str,
    bandwidthThrottling: NotRequired[int],
    name: NotRequired[str],
    usePrivateIP: NotRequired[bool],
```

## CreateSourceNetworkResponseTypeDef

```python
# CreateSourceNetworkResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import CreateSourceNetworkResponseTypeDef


def get_value() -> CreateSourceNetworkResponseTypeDef:
    return {
        "sourceNetworkID": ...,
    }


# CreateSourceNetworkResponseTypeDef definition

class CreateSourceNetworkResponseTypeDef(TypedDict):
    sourceNetworkID: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportSourceNetworkCfnTemplateResponseTypeDef

```python
# ExportSourceNetworkCfnTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ExportSourceNetworkCfnTemplateResponseTypeDef


def get_value() -> ExportSourceNetworkCfnTemplateResponseTypeDef:
    return {
        "s3DestinationUrl": ...,
    }


# ExportSourceNetworkCfnTemplateResponseTypeDef definition

class ExportSourceNetworkCfnTemplateResponseTypeDef(TypedDict):
    s3DestinationUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFailbackReplicationConfigurationResponseTypeDef

```python
# GetFailbackReplicationConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import GetFailbackReplicationConfigurationResponseTypeDef


def get_value() -> GetFailbackReplicationConfigurationResponseTypeDef:
    return {
        "bandwidthThrottling": ...,
    }


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
# ListStagingAccountsResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ListStagingAccountsResponseTypeDef


def get_value() -> ListStagingAccountsResponseTypeDef:
    return {
        "accounts": ...,
    }


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
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ListTagsForResourceResponseTypeDef


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
## ReverseReplicationResponseTypeDef

```python
# ReverseReplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ReverseReplicationResponseTypeDef


def get_value() -> ReverseReplicationResponseTypeDef:
    return {
        "reversedDirectionSourceServerArn": ...,
    }


# ReverseReplicationResponseTypeDef definition

class ReverseReplicationResponseTypeDef(TypedDict):
    reversedDirectionSourceServerArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConversionPropertiesTypeDef

```python
# ConversionPropertiesTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ConversionPropertiesTypeDef


def get_value() -> ConversionPropertiesTypeDef:
    return {
        "dataTimestamp": ...,
    }


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
## CreateLaunchConfigurationTemplateRequestTypeDef

```python
# CreateLaunchConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import CreateLaunchConfigurationTemplateRequestTypeDef


def get_value() -> CreateLaunchConfigurationTemplateRequestTypeDef:
    return {
        "copyPrivateIp": ...,
    }


# CreateLaunchConfigurationTemplateRequestTypeDef definition

class CreateLaunchConfigurationTemplateRequestTypeDef(TypedDict):
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
# LaunchConfigurationTemplateTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LaunchConfigurationTemplateTypeDef


def get_value() -> LaunchConfigurationTemplateTypeDef:
    return {
        "arn": ...,
    }


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
## UpdateLaunchConfigurationTemplateRequestTypeDef

```python
# UpdateLaunchConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import UpdateLaunchConfigurationTemplateRequestTypeDef


def get_value() -> UpdateLaunchConfigurationTemplateRequestTypeDef:
    return {
        "launchConfigurationTemplateID": ...,
    }


# UpdateLaunchConfigurationTemplateRequestTypeDef definition

class UpdateLaunchConfigurationTemplateRequestTypeDef(TypedDict):
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
## CreateReplicationConfigurationTemplateRequestTypeDef

```python
# CreateReplicationConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import CreateReplicationConfigurationTemplateRequestTypeDef


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
# ReplicationConfigurationTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ReplicationConfigurationTemplateResponseTypeDef


def get_value() -> ReplicationConfigurationTemplateResponseTypeDef:
    return {
        "arn": ...,
    }


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
# ReplicationConfigurationTemplateTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ReplicationConfigurationTemplateTypeDef


def get_value() -> ReplicationConfigurationTemplateTypeDef:
    return {
        "arn": ...,
    }


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
## UpdateReplicationConfigurationTemplateRequestTypeDef

```python
# UpdateReplicationConfigurationTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import UpdateReplicationConfigurationTemplateRequestTypeDef


def get_value() -> UpdateReplicationConfigurationTemplateRequestTypeDef:
    return {
        "replicationConfigurationTemplateID": ...,
    }


# UpdateReplicationConfigurationTemplateRequestTypeDef definition

class UpdateReplicationConfigurationTemplateRequestTypeDef(TypedDict):
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
# DataReplicationInitiationTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DataReplicationInitiationTypeDef


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

from types_aiobotocore_drs.type_defs import DescribeJobLogItemsRequestPaginateTypeDef


def get_value() -> DescribeJobLogItemsRequestPaginateTypeDef:
    return {
        "jobID": ...,
    }


# DescribeJobLogItemsRequestPaginateTypeDef definition

class DescribeJobLogItemsRequestPaginateTypeDef(TypedDict):
    jobID: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef

```python
# DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef


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

from types_aiobotocore_drs.type_defs import DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef


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
## ListExtensibleSourceServersRequestPaginateTypeDef

```python
# ListExtensibleSourceServersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ListExtensibleSourceServersRequestPaginateTypeDef


def get_value() -> ListExtensibleSourceServersRequestPaginateTypeDef:
    return {
        "stagingAccountID": ...,
    }


# ListExtensibleSourceServersRequestPaginateTypeDef definition

class ListExtensibleSourceServersRequestPaginateTypeDef(TypedDict):
    stagingAccountID: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStagingAccountsRequestPaginateTypeDef

```python
# ListStagingAccountsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ListStagingAccountsRequestPaginateTypeDef


def get_value() -> ListStagingAccountsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListStagingAccountsRequestPaginateTypeDef definition

class ListStagingAccountsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeJobsRequestPaginateTypeDef

```python
# DescribeJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeJobsRequestPaginateTypeDef


def get_value() -> DescribeJobsRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# DescribeJobsRequestPaginateTypeDef definition

class DescribeJobsRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[DescribeJobsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeJobsRequestTypeDef

```python
# DescribeJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeJobsRequestTypeDef


def get_value() -> DescribeJobsRequestTypeDef:
    return {
        "filters": ...,
    }


# DescribeJobsRequestTypeDef definition

class DescribeJobsRequestTypeDef(TypedDict):
    filters: NotRequired[DescribeJobsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
## DescribeRecoveryInstancesRequestPaginateTypeDef

```python
# DescribeRecoveryInstancesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeRecoveryInstancesRequestPaginateTypeDef


def get_value() -> DescribeRecoveryInstancesRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# DescribeRecoveryInstancesRequestPaginateTypeDef definition

class DescribeRecoveryInstancesRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[DescribeRecoveryInstancesRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeRecoveryInstancesRequestFiltersTypeDef](./type_defs.md#describerecoveryinstancesrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRecoveryInstancesRequestTypeDef

```python
# DescribeRecoveryInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeRecoveryInstancesRequestTypeDef


def get_value() -> DescribeRecoveryInstancesRequestTypeDef:
    return {
        "filters": ...,
    }


# DescribeRecoveryInstancesRequestTypeDef definition

class DescribeRecoveryInstancesRequestTypeDef(TypedDict):
    filters: NotRequired[DescribeRecoveryInstancesRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeRecoveryInstancesRequestFiltersTypeDef](./type_defs.md#describerecoveryinstancesrequestfilterstypedef) 
## DescribeRecoverySnapshotsRequestPaginateTypeDef

```python
# DescribeRecoverySnapshotsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeRecoverySnapshotsRequestPaginateTypeDef


def get_value() -> DescribeRecoverySnapshotsRequestPaginateTypeDef:
    return {
        "sourceServerID": ...,
    }


# DescribeRecoverySnapshotsRequestPaginateTypeDef definition

class DescribeRecoverySnapshotsRequestPaginateTypeDef(TypedDict):
    sourceServerID: str,
    filters: NotRequired[DescribeRecoverySnapshotsRequestFiltersTypeDef],  # (1)
    order: NotRequired[RecoverySnapshotsOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: DescribeRecoverySnapshotsRequestFiltersTypeDef](./type_defs.md#describerecoverysnapshotsrequestfilterstypedef) 
2. See [:material-code-brackets: RecoverySnapshotsOrderType](./literals.md#recoverysnapshotsordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRecoverySnapshotsRequestTypeDef

```python
# DescribeRecoverySnapshotsRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeRecoverySnapshotsRequestTypeDef


def get_value() -> DescribeRecoverySnapshotsRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# DescribeRecoverySnapshotsRequestTypeDef definition

class DescribeRecoverySnapshotsRequestTypeDef(TypedDict):
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
# DescribeRecoverySnapshotsResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeRecoverySnapshotsResponseTypeDef


def get_value() -> DescribeRecoverySnapshotsResponseTypeDef:
    return {
        "items": ...,
    }


# DescribeRecoverySnapshotsResponseTypeDef definition

class DescribeRecoverySnapshotsResponseTypeDef(TypedDict):
    items: List[RecoverySnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecoverySnapshotTypeDef](./type_defs.md#recoverysnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSourceNetworksRequestPaginateTypeDef

```python
# DescribeSourceNetworksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeSourceNetworksRequestPaginateTypeDef


def get_value() -> DescribeSourceNetworksRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# DescribeSourceNetworksRequestPaginateTypeDef definition

class DescribeSourceNetworksRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[DescribeSourceNetworksRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeSourceNetworksRequestFiltersTypeDef](./type_defs.md#describesourcenetworksrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSourceNetworksRequestTypeDef

```python
# DescribeSourceNetworksRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeSourceNetworksRequestTypeDef


def get_value() -> DescribeSourceNetworksRequestTypeDef:
    return {
        "filters": ...,
    }


# DescribeSourceNetworksRequestTypeDef definition

class DescribeSourceNetworksRequestTypeDef(TypedDict):
    filters: NotRequired[DescribeSourceNetworksRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeSourceNetworksRequestFiltersTypeDef](./type_defs.md#describesourcenetworksrequestfilterstypedef) 
## DescribeSourceServersRequestPaginateTypeDef

```python
# DescribeSourceServersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeSourceServersRequestPaginateTypeDef


def get_value() -> DescribeSourceServersRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# DescribeSourceServersRequestPaginateTypeDef definition

class DescribeSourceServersRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[DescribeSourceServersRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSourceServersRequestTypeDef

```python
# DescribeSourceServersRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeSourceServersRequestTypeDef


def get_value() -> DescribeSourceServersRequestTypeDef:
    return {
        "filters": ...,
    }


# DescribeSourceServersRequestTypeDef definition

class DescribeSourceServersRequestTypeDef(TypedDict):
    filters: NotRequired[DescribeSourceServersRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
## EventResourceDataTypeDef

```python
# EventResourceDataTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import EventResourceDataTypeDef


def get_value() -> EventResourceDataTypeDef:
    return {
        "sourceNetworkData": ...,
    }


# EventResourceDataTypeDef definition

class EventResourceDataTypeDef(TypedDict):
    sourceNetworkData: NotRequired[SourceNetworkDataTypeDef],  # (1)
```

1. See [:material-code-braces: SourceNetworkDataTypeDef](./type_defs.md#sourcenetworkdatatypedef) 
## LaunchActionTypeDef

```python
# LaunchActionTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LaunchActionTypeDef


def get_value() -> LaunchActionTypeDef:
    return {
        "actionCode": ...,
    }


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
## PutLaunchActionRequestTypeDef

```python
# PutLaunchActionRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import PutLaunchActionRequestTypeDef


def get_value() -> PutLaunchActionRequestTypeDef:
    return {
        "actionCode": ...,
    }


# PutLaunchActionRequestTypeDef definition

class PutLaunchActionRequestTypeDef(TypedDict):
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
# PutLaunchActionResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import PutLaunchActionResponseTypeDef


def get_value() -> PutLaunchActionResponseTypeDef:
    return {
        "actionCode": ...,
    }


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
## ListLaunchActionsRequestPaginateTypeDef

```python
# ListLaunchActionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ListLaunchActionsRequestPaginateTypeDef


def get_value() -> ListLaunchActionsRequestPaginateTypeDef:
    return {
        "resourceId": ...,
    }


# ListLaunchActionsRequestPaginateTypeDef definition

class ListLaunchActionsRequestPaginateTypeDef(TypedDict):
    resourceId: str,
    filters: NotRequired[LaunchActionsRequestFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: LaunchActionsRequestFiltersTypeDef](./type_defs.md#launchactionsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLaunchActionsRequestTypeDef

```python
# ListLaunchActionsRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ListLaunchActionsRequestTypeDef


def get_value() -> ListLaunchActionsRequestTypeDef:
    return {
        "resourceId": ...,
    }


# ListLaunchActionsRequestTypeDef definition

class ListLaunchActionsRequestTypeDef(TypedDict):
    resourceId: str,
    filters: NotRequired[LaunchActionsRequestFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LaunchActionsRequestFiltersTypeDef](./type_defs.md#launchactionsrequestfilterstypedef) 
## LaunchConfigurationTypeDef

```python
# LaunchConfigurationTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LaunchConfigurationTypeDef


def get_value() -> LaunchConfigurationTypeDef:
    return {
        "copyPrivateIp": ...,
    }


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
## UpdateLaunchConfigurationRequestTypeDef

```python
# UpdateLaunchConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import UpdateLaunchConfigurationRequestTypeDef


def get_value() -> UpdateLaunchConfigurationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# UpdateLaunchConfigurationRequestTypeDef definition

class UpdateLaunchConfigurationRequestTypeDef(TypedDict):
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
# LifeCycleLastLaunchTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LifeCycleLastLaunchTypeDef


def get_value() -> LifeCycleLastLaunchTypeDef:
    return {
        "initiated": ...,
    }


# LifeCycleLastLaunchTypeDef definition

class LifeCycleLastLaunchTypeDef(TypedDict):
    initiated: NotRequired[LifeCycleLastLaunchInitiatedTypeDef],  # (1)
    status: NotRequired[LaunchStatusType],  # (2)
```

1. See [:material-code-braces: LifeCycleLastLaunchInitiatedTypeDef](./type_defs.md#lifecyclelastlaunchinitiatedtypedef) 
2. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
## ListExtensibleSourceServersResponseTypeDef

```python
# ListExtensibleSourceServersResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ListExtensibleSourceServersResponseTypeDef


def get_value() -> ListExtensibleSourceServersResponseTypeDef:
    return {
        "items": ...,
    }


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
# SourcePropertiesTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import SourcePropertiesTypeDef


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
    supportsNitroInstances: NotRequired[bool],
```

1. See [:material-code-braces: CPUTypeDef](./type_defs.md#cputypedef) 
2. See [:material-code-braces: DiskTypeDef](./type_defs.md#disktypedef) 
3. See [:material-code-braces: IdentificationHintsTypeDef](./type_defs.md#identificationhintstypedef) 
4. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
5. See [:material-code-braces: OSTypeDef](./type_defs.md#ostypedef) 
## ParticipatingResourceTypeDef

```python
# ParticipatingResourceTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ParticipatingResourceTypeDef


def get_value() -> ParticipatingResourceTypeDef:
    return {
        "launchStatus": ...,
    }


# ParticipatingResourceTypeDef definition

class ParticipatingResourceTypeDef(TypedDict):
    launchStatus: NotRequired[LaunchStatusType],  # (1)
    participatingResourceID: NotRequired[ParticipatingResourceIDTypeDef],  # (2)
```

1. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
2. See [:material-code-braces: ParticipatingResourceIDTypeDef](./type_defs.md#participatingresourceidtypedef) 
## RecoveryInstanceDataReplicationInitiationTypeDef

```python
# RecoveryInstanceDataReplicationInitiationTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RecoveryInstanceDataReplicationInitiationTypeDef


def get_value() -> RecoveryInstanceDataReplicationInitiationTypeDef:
    return {
        "startDateTime": ...,
    }


# RecoveryInstanceDataReplicationInitiationTypeDef definition

class RecoveryInstanceDataReplicationInitiationTypeDef(TypedDict):
    startDateTime: NotRequired[str],
    steps: NotRequired[List[RecoveryInstanceDataReplicationInitiationStepTypeDef]],  # (1)
```

1. See [:material-code-braces: RecoveryInstanceDataReplicationInitiationStepTypeDef](./type_defs.md#recoveryinstancedatareplicationinitiationsteptypedef) 
## RecoveryInstancePropertiesTypeDef

```python
# RecoveryInstancePropertiesTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RecoveryInstancePropertiesTypeDef


def get_value() -> RecoveryInstancePropertiesTypeDef:
    return {
        "cpus": ...,
    }


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
# SourceNetworkTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import SourceNetworkTypeDef


def get_value() -> SourceNetworkTypeDef:
    return {
        "arn": ...,
    }


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
# ReplicationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ReplicationConfigurationTypeDef


def get_value() -> ReplicationConfigurationTypeDef:
    return {
        "associateDefaultSecurityGroup": ...,
    }


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
## UpdateReplicationConfigurationRequestTypeDef

```python
# UpdateReplicationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import UpdateReplicationConfigurationRequestTypeDef


def get_value() -> UpdateReplicationConfigurationRequestTypeDef:
    return {
        "sourceServerID": ...,
    }


# UpdateReplicationConfigurationRequestTypeDef definition

class UpdateReplicationConfigurationRequestTypeDef(TypedDict):
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
## StartRecoveryRequestTypeDef

```python
# StartRecoveryRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartRecoveryRequestTypeDef


def get_value() -> StartRecoveryRequestTypeDef:
    return {
        "sourceServers": ...,
    }


# StartRecoveryRequestTypeDef definition

class StartRecoveryRequestTypeDef(TypedDict):
    sourceServers: Sequence[StartRecoveryRequestSourceServerTypeDef],  # (1)
    isDrill: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: StartRecoveryRequestSourceServerTypeDef](./type_defs.md#startrecoveryrequestsourceservertypedef) 
## StartSourceNetworkRecoveryRequestTypeDef

```python
# StartSourceNetworkRecoveryRequestTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartSourceNetworkRecoveryRequestTypeDef


def get_value() -> StartSourceNetworkRecoveryRequestTypeDef:
    return {
        "sourceNetworks": ...,
    }


# StartSourceNetworkRecoveryRequestTypeDef definition

class StartSourceNetworkRecoveryRequestTypeDef(TypedDict):
    sourceNetworks: Sequence[StartSourceNetworkRecoveryRequestNetworkEntryTypeDef],  # (1)
    deployAsNew: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: StartSourceNetworkRecoveryRequestNetworkEntryTypeDef](./type_defs.md#startsourcenetworkrecoveryrequestnetworkentrytypedef) 
## CreateLaunchConfigurationTemplateResponseTypeDef

```python
# CreateLaunchConfigurationTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import CreateLaunchConfigurationTemplateResponseTypeDef


def get_value() -> CreateLaunchConfigurationTemplateResponseTypeDef:
    return {
        "launchConfigurationTemplate": ...,
    }


# CreateLaunchConfigurationTemplateResponseTypeDef definition

class CreateLaunchConfigurationTemplateResponseTypeDef(TypedDict):
    launchConfigurationTemplate: LaunchConfigurationTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchConfigurationTemplateTypeDef](./type_defs.md#launchconfigurationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLaunchConfigurationTemplatesResponseTypeDef

```python
# DescribeLaunchConfigurationTemplatesResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeLaunchConfigurationTemplatesResponseTypeDef


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
## UpdateLaunchConfigurationTemplateResponseTypeDef

```python
# UpdateLaunchConfigurationTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import UpdateLaunchConfigurationTemplateResponseTypeDef


def get_value() -> UpdateLaunchConfigurationTemplateResponseTypeDef:
    return {
        "launchConfigurationTemplate": ...,
    }


# UpdateLaunchConfigurationTemplateResponseTypeDef definition

class UpdateLaunchConfigurationTemplateResponseTypeDef(TypedDict):
    launchConfigurationTemplate: LaunchConfigurationTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchConfigurationTemplateTypeDef](./type_defs.md#launchconfigurationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReplicationConfigurationTemplatesResponseTypeDef

```python
# DescribeReplicationConfigurationTemplatesResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeReplicationConfigurationTemplatesResponseTypeDef


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
## DataReplicationInfoTypeDef

```python
# DataReplicationInfoTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DataReplicationInfoTypeDef


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
# JobLogEventDataTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import JobLogEventDataTypeDef


def get_value() -> JobLogEventDataTypeDef:
    return {
        "conversionProperties": ...,
    }


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
# LaunchActionRunTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LaunchActionRunTypeDef


def get_value() -> LaunchActionRunTypeDef:
    return {
        "action": ...,
    }


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
# ListLaunchActionsResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ListLaunchActionsResponseTypeDef


def get_value() -> ListLaunchActionsResponseTypeDef:
    return {
        "items": ...,
    }


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
# LifeCycleTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LifeCycleTypeDef


def get_value() -> LifeCycleTypeDef:
    return {
        "addedToServiceDateTime": ...,
    }


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
# RecoveryInstanceDataReplicationInfoTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RecoveryInstanceDataReplicationInfoTypeDef


def get_value() -> RecoveryInstanceDataReplicationInfoTypeDef:
    return {
        "dataReplicationError": ...,
    }


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
# DescribeSourceNetworksResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeSourceNetworksResponseTypeDef


def get_value() -> DescribeSourceNetworksResponseTypeDef:
    return {
        "items": ...,
    }


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
# StartSourceNetworkReplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartSourceNetworkReplicationResponseTypeDef


def get_value() -> StartSourceNetworkReplicationResponseTypeDef:
    return {
        "sourceNetwork": ...,
    }


# StartSourceNetworkReplicationResponseTypeDef definition

class StartSourceNetworkReplicationResponseTypeDef(TypedDict):
    sourceNetwork: SourceNetworkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceNetworkTypeDef](./type_defs.md#sourcenetworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopSourceNetworkReplicationResponseTypeDef

```python
# StopSourceNetworkReplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StopSourceNetworkReplicationResponseTypeDef


def get_value() -> StopSourceNetworkReplicationResponseTypeDef:
    return {
        "sourceNetwork": ...,
    }


# StopSourceNetworkReplicationResponseTypeDef definition

class StopSourceNetworkReplicationResponseTypeDef(TypedDict):
    sourceNetwork: SourceNetworkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceNetworkTypeDef](./type_defs.md#sourcenetworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobLogTypeDef

```python
# JobLogTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import JobLogTypeDef


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
## LaunchActionsStatusTypeDef

```python
# LaunchActionsStatusTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import LaunchActionsStatusTypeDef


def get_value() -> LaunchActionsStatusTypeDef:
    return {
        "runs": ...,
    }


# LaunchActionsStatusTypeDef definition

class LaunchActionsStatusTypeDef(TypedDict):
    runs: NotRequired[List[LaunchActionRunTypeDef]],  # (1)
    ssmAgentDiscoveryDatetime: NotRequired[str],
```

1. See [:material-code-braces: LaunchActionRunTypeDef](./type_defs.md#launchactionruntypedef) 
## SourceServerResponseTypeDef

```python
# SourceServerResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import SourceServerResponseTypeDef


def get_value() -> SourceServerResponseTypeDef:
    return {
        "agentVersion": ...,
    }


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
# SourceServerTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import SourceServerTypeDef


def get_value() -> SourceServerTypeDef:
    return {
        "agentVersion": ...,
    }


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
# RecoveryInstanceTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import RecoveryInstanceTypeDef


def get_value() -> RecoveryInstanceTypeDef:
    return {
        "agentVersion": ...,
    }


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
# DescribeJobLogItemsResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeJobLogItemsResponseTypeDef


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
## ParticipatingServerTypeDef

```python
# ParticipatingServerTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import ParticipatingServerTypeDef


def get_value() -> ParticipatingServerTypeDef:
    return {
        "launchActionsStatus": ...,
    }


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
# CreateExtendedSourceServerResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import CreateExtendedSourceServerResponseTypeDef


def get_value() -> CreateExtendedSourceServerResponseTypeDef:
    return {
        "sourceServer": ...,
    }


# CreateExtendedSourceServerResponseTypeDef definition

class CreateExtendedSourceServerResponseTypeDef(TypedDict):
    sourceServer: SourceServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceServerTypeDef](./type_defs.md#sourceservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSourceServersResponseTypeDef

```python
# DescribeSourceServersResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeSourceServersResponseTypeDef


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
## StartReplicationResponseTypeDef

```python
# StartReplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartReplicationResponseTypeDef


def get_value() -> StartReplicationResponseTypeDef:
    return {
        "sourceServer": ...,
    }


# StartReplicationResponseTypeDef definition

class StartReplicationResponseTypeDef(TypedDict):
    sourceServer: SourceServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceServerTypeDef](./type_defs.md#sourceservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopReplicationResponseTypeDef

```python
# StopReplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StopReplicationResponseTypeDef


def get_value() -> StopReplicationResponseTypeDef:
    return {
        "sourceServer": ...,
    }


# StopReplicationResponseTypeDef definition

class StopReplicationResponseTypeDef(TypedDict):
    sourceServer: SourceServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceServerTypeDef](./type_defs.md#sourceservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRecoveryInstancesResponseTypeDef

```python
# DescribeRecoveryInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeRecoveryInstancesResponseTypeDef


def get_value() -> DescribeRecoveryInstancesResponseTypeDef:
    return {
        "items": ...,
    }


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
# JobTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import JobTypeDef


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
# AssociateSourceNetworkStackResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import AssociateSourceNetworkStackResponseTypeDef


def get_value() -> AssociateSourceNetworkStackResponseTypeDef:
    return {
        "job": ...,
    }


# AssociateSourceNetworkStackResponseTypeDef definition

class AssociateSourceNetworkStackResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeJobsResponseTypeDef

```python
# DescribeJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import DescribeJobsResponseTypeDef


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
## StartFailbackLaunchResponseTypeDef

```python
# StartFailbackLaunchResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartFailbackLaunchResponseTypeDef


def get_value() -> StartFailbackLaunchResponseTypeDef:
    return {
        "job": ...,
    }


# StartFailbackLaunchResponseTypeDef definition

class StartFailbackLaunchResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartRecoveryResponseTypeDef

```python
# StartRecoveryResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartRecoveryResponseTypeDef


def get_value() -> StartRecoveryResponseTypeDef:
    return {
        "job": ...,
    }


# StartRecoveryResponseTypeDef definition

class StartRecoveryResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSourceNetworkRecoveryResponseTypeDef

```python
# StartSourceNetworkRecoveryResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import StartSourceNetworkRecoveryResponseTypeDef


def get_value() -> StartSourceNetworkRecoveryResponseTypeDef:
    return {
        "job": ...,
    }


# StartSourceNetworkRecoveryResponseTypeDef definition

class StartSourceNetworkRecoveryResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TerminateRecoveryInstancesResponseTypeDef

```python
# TerminateRecoveryInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_drs.type_defs import TerminateRecoveryInstancesResponseTypeDef


def get_value() -> TerminateRecoveryInstancesResponseTypeDef:
    return {
        "job": ...,
    }


# TerminateRecoveryInstancesResponseTypeDef definition

class TerminateRecoveryInstancesResponseTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
