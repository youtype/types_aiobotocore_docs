# Type definitions

> [Index](../README.md) > [DeadlineCloud](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DeadlineCloud](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline.html#deadlinecloud)
    type annotations stubs module [types-aiobotocore-deadline](https://pypi.org/project/types-aiobotocore-deadline/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_deadline.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## IpAddressesUnionTypeDef

```python
# IpAddressesUnionTypeDef Union usage example

from types_aiobotocore_deadline.type_defs import IpAddressesUnionTypeDef


def get_value() -> IpAddressesUnionTypeDef:
    return ...


# IpAddressesUnionTypeDef definition

IpAddressesUnionTypeDef = Union[
    IpAddressesTypeDef,  # (1)
    IpAddressesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IpAddressesTypeDef](./type_defs.md#ipaddressestypedef) 
2. See [:material-code-braces: IpAddressesOutputTypeDef](./type_defs.md#ipaddressesoutputtypedef) 

## AttachmentsUnionTypeDef

```python
# AttachmentsUnionTypeDef Union usage example

from types_aiobotocore_deadline.type_defs import AttachmentsUnionTypeDef


def get_value() -> AttachmentsUnionTypeDef:
    return ...


# AttachmentsUnionTypeDef definition

AttachmentsUnionTypeDef = Union[
    AttachmentsTypeDef,  # (1)
    AttachmentsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttachmentsTypeDef](./type_defs.md#attachmentstypedef) 
2. See [:material-code-braces: AttachmentsOutputTypeDef](./type_defs.md#attachmentsoutputtypedef) 

## BudgetScheduleUnionTypeDef

```python
# BudgetScheduleUnionTypeDef Union usage example

from types_aiobotocore_deadline.type_defs import BudgetScheduleUnionTypeDef


def get_value() -> BudgetScheduleUnionTypeDef:
    return ...


# BudgetScheduleUnionTypeDef definition

BudgetScheduleUnionTypeDef = Union[
    BudgetScheduleTypeDef,  # (1)
    BudgetScheduleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BudgetScheduleTypeDef](./type_defs.md#budgetscheduletypedef) 
2. See [:material-code-braces: BudgetScheduleOutputTypeDef](./type_defs.md#budgetscheduleoutputtypedef) 

## FleetConfigurationUnionTypeDef

```python
# FleetConfigurationUnionTypeDef Union usage example

from types_aiobotocore_deadline.type_defs import FleetConfigurationUnionTypeDef


def get_value() -> FleetConfigurationUnionTypeDef:
    return ...


# FleetConfigurationUnionTypeDef definition

FleetConfigurationUnionTypeDef = Union[
    FleetConfigurationTypeDef,  # (1)
    FleetConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FleetConfigurationTypeDef](./type_defs.md#fleetconfigurationtypedef) 
2. See [:material-code-braces: FleetConfigurationOutputTypeDef](./type_defs.md#fleetconfigurationoutputtypedef) 



## AcceleratorCountRangeTypeDef

```python
# AcceleratorCountRangeTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AcceleratorCountRangeTypeDef


def get_value() -> AcceleratorCountRangeTypeDef:
    return {
        "min": ...,
    }


# AcceleratorCountRangeTypeDef definition

class AcceleratorCountRangeTypeDef(TypedDict):
    min: int,
    max: NotRequired[int],
```

## AcceleratorSelectionTypeDef

```python
# AcceleratorSelectionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AcceleratorSelectionTypeDef


def get_value() -> AcceleratorSelectionTypeDef:
    return {
        "name": ...,
    }


# AcceleratorSelectionTypeDef definition

class AcceleratorSelectionTypeDef(TypedDict):
    name: AcceleratorNameType,  # (1)
    runtime: NotRequired[str],
```

1. See [:material-code-brackets: AcceleratorNameType](./literals.md#acceleratornametype) 
## AcceleratorTotalMemoryMiBRangeTypeDef

```python
# AcceleratorTotalMemoryMiBRangeTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AcceleratorTotalMemoryMiBRangeTypeDef


def get_value() -> AcceleratorTotalMemoryMiBRangeTypeDef:
    return {
        "min": ...,
    }


# AcceleratorTotalMemoryMiBRangeTypeDef definition

class AcceleratorTotalMemoryMiBRangeTypeDef(TypedDict):
    min: int,
    max: NotRequired[int],
```

## AcquiredLimitTypeDef

```python
# AcquiredLimitTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AcquiredLimitTypeDef


def get_value() -> AcquiredLimitTypeDef:
    return {
        "limitId": ...,
    }


# AcquiredLimitTypeDef definition

class AcquiredLimitTypeDef(TypedDict):
    limitId: str,
    count: int,
```

## AssignedEnvironmentEnterSessionActionDefinitionTypeDef

```python
# AssignedEnvironmentEnterSessionActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssignedEnvironmentEnterSessionActionDefinitionTypeDef


def get_value() -> AssignedEnvironmentEnterSessionActionDefinitionTypeDef:
    return {
        "environmentId": ...,
    }


# AssignedEnvironmentEnterSessionActionDefinitionTypeDef definition

class AssignedEnvironmentEnterSessionActionDefinitionTypeDef(TypedDict):
    environmentId: str,
```

## AssignedEnvironmentExitSessionActionDefinitionTypeDef

```python
# AssignedEnvironmentExitSessionActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssignedEnvironmentExitSessionActionDefinitionTypeDef


def get_value() -> AssignedEnvironmentExitSessionActionDefinitionTypeDef:
    return {
        "environmentId": ...,
    }


# AssignedEnvironmentExitSessionActionDefinitionTypeDef definition

class AssignedEnvironmentExitSessionActionDefinitionTypeDef(TypedDict):
    environmentId: str,
```

## AssignedSyncInputJobAttachmentsSessionActionDefinitionTypeDef

```python
# AssignedSyncInputJobAttachmentsSessionActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssignedSyncInputJobAttachmentsSessionActionDefinitionTypeDef


def get_value() -> AssignedSyncInputJobAttachmentsSessionActionDefinitionTypeDef:
    return {
        "stepId": ...,
    }


# AssignedSyncInputJobAttachmentsSessionActionDefinitionTypeDef definition

class AssignedSyncInputJobAttachmentsSessionActionDefinitionTypeDef(TypedDict):
    stepId: NotRequired[str],
```

## LogConfigurationTypeDef

```python
# LogConfigurationTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import LogConfigurationTypeDef


def get_value() -> LogConfigurationTypeDef:
    return {
        "logDriver": ...,
    }


# LogConfigurationTypeDef definition

class LogConfigurationTypeDef(TypedDict):
    logDriver: str,
    options: NotRequired[Dict[str, str]],
    parameters: NotRequired[Dict[str, str]],
    error: NotRequired[str],
```

## TaskParameterValueTypeDef

```python
# TaskParameterValueTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import TaskParameterValueTypeDef


def get_value() -> TaskParameterValueTypeDef:
    return {
        "int": ...,
    }


# TaskParameterValueTypeDef definition

class TaskParameterValueTypeDef(TypedDict):
    int: NotRequired[str],
    float: NotRequired[str],
    string: NotRequired[str],
    path: NotRequired[str],
```

## AssociateMemberToFarmRequestTypeDef

```python
# AssociateMemberToFarmRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssociateMemberToFarmRequestTypeDef


def get_value() -> AssociateMemberToFarmRequestTypeDef:
    return {
        "farmId": ...,
    }


# AssociateMemberToFarmRequestTypeDef definition

class AssociateMemberToFarmRequestTypeDef(TypedDict):
    farmId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 
## AssociateMemberToFleetRequestTypeDef

```python
# AssociateMemberToFleetRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssociateMemberToFleetRequestTypeDef


def get_value() -> AssociateMemberToFleetRequestTypeDef:
    return {
        "farmId": ...,
    }


# AssociateMemberToFleetRequestTypeDef definition

class AssociateMemberToFleetRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 
## AssociateMemberToJobRequestTypeDef

```python
# AssociateMemberToJobRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssociateMemberToJobRequestTypeDef


def get_value() -> AssociateMemberToJobRequestTypeDef:
    return {
        "farmId": ...,
    }


# AssociateMemberToJobRequestTypeDef definition

class AssociateMemberToJobRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 
## AssociateMemberToQueueRequestTypeDef

```python
# AssociateMemberToQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssociateMemberToQueueRequestTypeDef


def get_value() -> AssociateMemberToQueueRequestTypeDef:
    return {
        "farmId": ...,
    }


# AssociateMemberToQueueRequestTypeDef definition

class AssociateMemberToQueueRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 
## AssumeFleetRoleForReadRequestTypeDef

```python
# AssumeFleetRoleForReadRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssumeFleetRoleForReadRequestTypeDef


def get_value() -> AssumeFleetRoleForReadRequestTypeDef:
    return {
        "farmId": ...,
    }


# AssumeFleetRoleForReadRequestTypeDef definition

class AssumeFleetRoleForReadRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
```

## AwsCredentialsTypeDef

```python
# AwsCredentialsTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AwsCredentialsTypeDef


def get_value() -> AwsCredentialsTypeDef:
    return {
        "accessKeyId": ...,
    }


# AwsCredentialsTypeDef definition

class AwsCredentialsTypeDef(TypedDict):
    accessKeyId: str,
    secretAccessKey: str,
    sessionToken: str,
    expiration: datetime,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ResponseMetadataTypeDef


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

## AssumeFleetRoleForWorkerRequestTypeDef

```python
# AssumeFleetRoleForWorkerRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssumeFleetRoleForWorkerRequestTypeDef


def get_value() -> AssumeFleetRoleForWorkerRequestTypeDef:
    return {
        "farmId": ...,
    }


# AssumeFleetRoleForWorkerRequestTypeDef definition

class AssumeFleetRoleForWorkerRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
```

## AssumeQueueRoleForReadRequestTypeDef

```python
# AssumeQueueRoleForReadRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssumeQueueRoleForReadRequestTypeDef


def get_value() -> AssumeQueueRoleForReadRequestTypeDef:
    return {
        "farmId": ...,
    }


# AssumeQueueRoleForReadRequestTypeDef definition

class AssumeQueueRoleForReadRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
```

## AssumeQueueRoleForUserRequestTypeDef

```python
# AssumeQueueRoleForUserRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssumeQueueRoleForUserRequestTypeDef


def get_value() -> AssumeQueueRoleForUserRequestTypeDef:
    return {
        "farmId": ...,
    }


# AssumeQueueRoleForUserRequestTypeDef definition

class AssumeQueueRoleForUserRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
```

## AssumeQueueRoleForWorkerRequestTypeDef

```python
# AssumeQueueRoleForWorkerRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssumeQueueRoleForWorkerRequestTypeDef


def get_value() -> AssumeQueueRoleForWorkerRequestTypeDef:
    return {
        "farmId": ...,
    }


# AssumeQueueRoleForWorkerRequestTypeDef definition

class AssumeQueueRoleForWorkerRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    queueId: str,
```

## ManifestPropertiesOutputTypeDef

```python
# ManifestPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ManifestPropertiesOutputTypeDef


def get_value() -> ManifestPropertiesOutputTypeDef:
    return {
        "fileSystemLocationName": ...,
    }


# ManifestPropertiesOutputTypeDef definition

class ManifestPropertiesOutputTypeDef(TypedDict):
    rootPath: str,
    rootPathFormat: PathFormatType,  # (1)
    fileSystemLocationName: NotRequired[str],
    outputRelativeDirectories: NotRequired[List[str]],
    inputManifestPath: NotRequired[str],
    inputManifestHash: NotRequired[str],
```

1. See [:material-code-brackets: PathFormatType](./literals.md#pathformattype) 
## ManifestPropertiesTypeDef

```python
# ManifestPropertiesTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ManifestPropertiesTypeDef


def get_value() -> ManifestPropertiesTypeDef:
    return {
        "fileSystemLocationName": ...,
    }


# ManifestPropertiesTypeDef definition

class ManifestPropertiesTypeDef(TypedDict):
    rootPath: str,
    rootPathFormat: PathFormatType,  # (1)
    fileSystemLocationName: NotRequired[str],
    outputRelativeDirectories: NotRequired[Sequence[str]],
    inputManifestPath: NotRequired[str],
    inputManifestHash: NotRequired[str],
```

1. See [:material-code-brackets: PathFormatType](./literals.md#pathformattype) 
## BudgetActionToAddTypeDef

```python
# BudgetActionToAddTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import BudgetActionToAddTypeDef


def get_value() -> BudgetActionToAddTypeDef:
    return {
        "type": ...,
    }


# BudgetActionToAddTypeDef definition

class BudgetActionToAddTypeDef(TypedDict):
    type: BudgetActionTypeType,  # (1)
    thresholdPercentage: float,
    description: NotRequired[str],
```

1. See [:material-code-brackets: BudgetActionTypeType](./literals.md#budgetactiontypetype) 
## BudgetActionToRemoveTypeDef

```python
# BudgetActionToRemoveTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import BudgetActionToRemoveTypeDef


def get_value() -> BudgetActionToRemoveTypeDef:
    return {
        "type": ...,
    }


# BudgetActionToRemoveTypeDef definition

class BudgetActionToRemoveTypeDef(TypedDict):
    type: BudgetActionTypeType,  # (1)
    thresholdPercentage: float,
```

1. See [:material-code-brackets: BudgetActionTypeType](./literals.md#budgetactiontypetype) 
## FixedBudgetScheduleOutputTypeDef

```python
# FixedBudgetScheduleOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FixedBudgetScheduleOutputTypeDef


def get_value() -> FixedBudgetScheduleOutputTypeDef:
    return {
        "startTime": ...,
    }


# FixedBudgetScheduleOutputTypeDef definition

class FixedBudgetScheduleOutputTypeDef(TypedDict):
    startTime: datetime,
    endTime: datetime,
```

## ConsumedUsagesTypeDef

```python
# ConsumedUsagesTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ConsumedUsagesTypeDef


def get_value() -> ConsumedUsagesTypeDef:
    return {
        "approximateDollarUsage": ...,
    }


# ConsumedUsagesTypeDef definition

class ConsumedUsagesTypeDef(TypedDict):
    approximateDollarUsage: float,
```

## UsageTrackingResourceTypeDef

```python
# UsageTrackingResourceTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UsageTrackingResourceTypeDef


def get_value() -> UsageTrackingResourceTypeDef:
    return {
        "queueId": ...,
    }


# UsageTrackingResourceTypeDef definition

class UsageTrackingResourceTypeDef(TypedDict):
    queueId: NotRequired[str],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import S3LocationTypeDef


def get_value() -> S3LocationTypeDef:
    return {
        "bucketName": ...,
    }


# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucketName: str,
    key: str,
```

## CreateFarmRequestTypeDef

```python
# CreateFarmRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateFarmRequestTypeDef


def get_value() -> CreateFarmRequestTypeDef:
    return {
        "displayName": ...,
    }


# CreateFarmRequestTypeDef definition

class CreateFarmRequestTypeDef(TypedDict):
    displayName: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## JobParameterTypeDef

```python
# JobParameterTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobParameterTypeDef


def get_value() -> JobParameterTypeDef:
    return {
        "int": ...,
    }


# JobParameterTypeDef definition

class JobParameterTypeDef(TypedDict):
    int: NotRequired[str],
    float: NotRequired[str],
    string: NotRequired[str],
    path: NotRequired[str],
```

## CreateLicenseEndpointRequestTypeDef

```python
# CreateLicenseEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateLicenseEndpointRequestTypeDef


def get_value() -> CreateLicenseEndpointRequestTypeDef:
    return {
        "vpcId": ...,
    }


# CreateLicenseEndpointRequestTypeDef definition

class CreateLicenseEndpointRequestTypeDef(TypedDict):
    vpcId: str,
    subnetIds: Sequence[str],
    securityGroupIds: Sequence[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateLimitRequestTypeDef

```python
# CreateLimitRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateLimitRequestTypeDef


def get_value() -> CreateLimitRequestTypeDef:
    return {
        "displayName": ...,
    }


# CreateLimitRequestTypeDef definition

class CreateLimitRequestTypeDef(TypedDict):
    displayName: str,
    amountRequirementName: str,
    maxCount: int,
    farmId: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## CreateMonitorRequestTypeDef

```python
# CreateMonitorRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateMonitorRequestTypeDef


def get_value() -> CreateMonitorRequestTypeDef:
    return {
        "displayName": ...,
    }


# CreateMonitorRequestTypeDef definition

class CreateMonitorRequestTypeDef(TypedDict):
    displayName: str,
    identityCenterInstanceArn: str,
    subdomain: str,
    roleArn: str,
    clientToken: NotRequired[str],
```

## CreateQueueEnvironmentRequestTypeDef

```python
# CreateQueueEnvironmentRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateQueueEnvironmentRequestTypeDef


def get_value() -> CreateQueueEnvironmentRequestTypeDef:
    return {
        "farmId": ...,
    }


# CreateQueueEnvironmentRequestTypeDef definition

class CreateQueueEnvironmentRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    priority: int,
    templateType: EnvironmentTemplateTypeType,  # (1)
    template: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentTemplateTypeType](./literals.md#environmenttemplatetypetype) 
## CreateQueueFleetAssociationRequestTypeDef

```python
# CreateQueueFleetAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateQueueFleetAssociationRequestTypeDef


def get_value() -> CreateQueueFleetAssociationRequestTypeDef:
    return {
        "farmId": ...,
    }


# CreateQueueFleetAssociationRequestTypeDef definition

class CreateQueueFleetAssociationRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    fleetId: str,
```

## CreateQueueLimitAssociationRequestTypeDef

```python
# CreateQueueLimitAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateQueueLimitAssociationRequestTypeDef


def get_value() -> CreateQueueLimitAssociationRequestTypeDef:
    return {
        "farmId": ...,
    }


# CreateQueueLimitAssociationRequestTypeDef definition

class CreateQueueLimitAssociationRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    limitId: str,
```

## JobAttachmentSettingsTypeDef

```python
# JobAttachmentSettingsTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobAttachmentSettingsTypeDef


def get_value() -> JobAttachmentSettingsTypeDef:
    return {
        "s3BucketName": ...,
    }


# JobAttachmentSettingsTypeDef definition

class JobAttachmentSettingsTypeDef(TypedDict):
    s3BucketName: str,
    rootPrefix: str,
```

## FileSystemLocationTypeDef

```python
# FileSystemLocationTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FileSystemLocationTypeDef


def get_value() -> FileSystemLocationTypeDef:
    return {
        "name": ...,
    }


# FileSystemLocationTypeDef definition

class FileSystemLocationTypeDef(TypedDict):
    name: str,
    path: str,
    type: FileSystemLocationTypeType,  # (1)
```

1. See [:material-code-brackets: FileSystemLocationTypeType](./literals.md#filesystemlocationtypetype) 
## FleetAmountCapabilityTypeDef

```python
# FleetAmountCapabilityTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FleetAmountCapabilityTypeDef


def get_value() -> FleetAmountCapabilityTypeDef:
    return {
        "name": ...,
    }


# FleetAmountCapabilityTypeDef definition

class FleetAmountCapabilityTypeDef(TypedDict):
    name: str,
    min: float,
    max: NotRequired[float],
```

## FleetAttributeCapabilityOutputTypeDef

```python
# FleetAttributeCapabilityOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FleetAttributeCapabilityOutputTypeDef


def get_value() -> FleetAttributeCapabilityOutputTypeDef:
    return {
        "name": ...,
    }


# FleetAttributeCapabilityOutputTypeDef definition

class FleetAttributeCapabilityOutputTypeDef(TypedDict):
    name: str,
    values: List[str],
```

## MemoryMiBRangeTypeDef

```python
# MemoryMiBRangeTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import MemoryMiBRangeTypeDef


def get_value() -> MemoryMiBRangeTypeDef:
    return {
        "min": ...,
    }


# MemoryMiBRangeTypeDef definition

class MemoryMiBRangeTypeDef(TypedDict):
    min: int,
    max: NotRequired[int],
```

## VCpuCountRangeTypeDef

```python
# VCpuCountRangeTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import VCpuCountRangeTypeDef


def get_value() -> VCpuCountRangeTypeDef:
    return {
        "min": ...,
    }


# VCpuCountRangeTypeDef definition

class VCpuCountRangeTypeDef(TypedDict):
    min: int,
    max: NotRequired[int],
```

## FleetAttributeCapabilityTypeDef

```python
# FleetAttributeCapabilityTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FleetAttributeCapabilityTypeDef


def get_value() -> FleetAttributeCapabilityTypeDef:
    return {
        "name": ...,
    }


# FleetAttributeCapabilityTypeDef definition

class FleetAttributeCapabilityTypeDef(TypedDict):
    name: str,
    values: Sequence[str],
```

## DeleteBudgetRequestTypeDef

```python
# DeleteBudgetRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteBudgetRequestTypeDef


def get_value() -> DeleteBudgetRequestTypeDef:
    return {
        "farmId": ...,
    }


# DeleteBudgetRequestTypeDef definition

class DeleteBudgetRequestTypeDef(TypedDict):
    farmId: str,
    budgetId: str,
```

## DeleteFarmRequestTypeDef

```python
# DeleteFarmRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteFarmRequestTypeDef


def get_value() -> DeleteFarmRequestTypeDef:
    return {
        "farmId": ...,
    }


# DeleteFarmRequestTypeDef definition

class DeleteFarmRequestTypeDef(TypedDict):
    farmId: str,
```

## DeleteFleetRequestTypeDef

```python
# DeleteFleetRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteFleetRequestTypeDef


def get_value() -> DeleteFleetRequestTypeDef:
    return {
        "farmId": ...,
    }


# DeleteFleetRequestTypeDef definition

class DeleteFleetRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    clientToken: NotRequired[str],
```

## DeleteLicenseEndpointRequestTypeDef

```python
# DeleteLicenseEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteLicenseEndpointRequestTypeDef


def get_value() -> DeleteLicenseEndpointRequestTypeDef:
    return {
        "licenseEndpointId": ...,
    }


# DeleteLicenseEndpointRequestTypeDef definition

class DeleteLicenseEndpointRequestTypeDef(TypedDict):
    licenseEndpointId: str,
```

## DeleteLimitRequestTypeDef

```python
# DeleteLimitRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteLimitRequestTypeDef


def get_value() -> DeleteLimitRequestTypeDef:
    return {
        "farmId": ...,
    }


# DeleteLimitRequestTypeDef definition

class DeleteLimitRequestTypeDef(TypedDict):
    farmId: str,
    limitId: str,
```

## DeleteMeteredProductRequestTypeDef

```python
# DeleteMeteredProductRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteMeteredProductRequestTypeDef


def get_value() -> DeleteMeteredProductRequestTypeDef:
    return {
        "licenseEndpointId": ...,
    }


# DeleteMeteredProductRequestTypeDef definition

class DeleteMeteredProductRequestTypeDef(TypedDict):
    licenseEndpointId: str,
    productId: str,
```

## DeleteMonitorRequestTypeDef

```python
# DeleteMonitorRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteMonitorRequestTypeDef


def get_value() -> DeleteMonitorRequestTypeDef:
    return {
        "monitorId": ...,
    }


# DeleteMonitorRequestTypeDef definition

class DeleteMonitorRequestTypeDef(TypedDict):
    monitorId: str,
```

## DeleteQueueEnvironmentRequestTypeDef

```python
# DeleteQueueEnvironmentRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteQueueEnvironmentRequestTypeDef


def get_value() -> DeleteQueueEnvironmentRequestTypeDef:
    return {
        "farmId": ...,
    }


# DeleteQueueEnvironmentRequestTypeDef definition

class DeleteQueueEnvironmentRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    queueEnvironmentId: str,
```

## DeleteQueueFleetAssociationRequestTypeDef

```python
# DeleteQueueFleetAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteQueueFleetAssociationRequestTypeDef


def get_value() -> DeleteQueueFleetAssociationRequestTypeDef:
    return {
        "farmId": ...,
    }


# DeleteQueueFleetAssociationRequestTypeDef definition

class DeleteQueueFleetAssociationRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    fleetId: str,
```

## DeleteQueueLimitAssociationRequestTypeDef

```python
# DeleteQueueLimitAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteQueueLimitAssociationRequestTypeDef


def get_value() -> DeleteQueueLimitAssociationRequestTypeDef:
    return {
        "farmId": ...,
    }


# DeleteQueueLimitAssociationRequestTypeDef definition

class DeleteQueueLimitAssociationRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    limitId: str,
```

## DeleteQueueRequestTypeDef

```python
# DeleteQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteQueueRequestTypeDef


def get_value() -> DeleteQueueRequestTypeDef:
    return {
        "farmId": ...,
    }


# DeleteQueueRequestTypeDef definition

class DeleteQueueRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
```

## DeleteStorageProfileRequestTypeDef

```python
# DeleteStorageProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteStorageProfileRequestTypeDef


def get_value() -> DeleteStorageProfileRequestTypeDef:
    return {
        "farmId": ...,
    }


# DeleteStorageProfileRequestTypeDef definition

class DeleteStorageProfileRequestTypeDef(TypedDict):
    farmId: str,
    storageProfileId: str,
```

## DeleteWorkerRequestTypeDef

```python
# DeleteWorkerRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DeleteWorkerRequestTypeDef


def get_value() -> DeleteWorkerRequestTypeDef:
    return {
        "farmId": ...,
    }


# DeleteWorkerRequestTypeDef definition

class DeleteWorkerRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
```

## DependencyCountsTypeDef

```python
# DependencyCountsTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DependencyCountsTypeDef


def get_value() -> DependencyCountsTypeDef:
    return {
        "dependenciesResolved": ...,
    }


# DependencyCountsTypeDef definition

class DependencyCountsTypeDef(TypedDict):
    dependenciesResolved: int,
    dependenciesUnresolved: int,
    consumersResolved: int,
    consumersUnresolved: int,
```

## DisassociateMemberFromFarmRequestTypeDef

```python
# DisassociateMemberFromFarmRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DisassociateMemberFromFarmRequestTypeDef


def get_value() -> DisassociateMemberFromFarmRequestTypeDef:
    return {
        "farmId": ...,
    }


# DisassociateMemberFromFarmRequestTypeDef definition

class DisassociateMemberFromFarmRequestTypeDef(TypedDict):
    farmId: str,
    principalId: str,
```

## DisassociateMemberFromFleetRequestTypeDef

```python
# DisassociateMemberFromFleetRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DisassociateMemberFromFleetRequestTypeDef


def get_value() -> DisassociateMemberFromFleetRequestTypeDef:
    return {
        "farmId": ...,
    }


# DisassociateMemberFromFleetRequestTypeDef definition

class DisassociateMemberFromFleetRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    principalId: str,
```

## DisassociateMemberFromJobRequestTypeDef

```python
# DisassociateMemberFromJobRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DisassociateMemberFromJobRequestTypeDef


def get_value() -> DisassociateMemberFromJobRequestTypeDef:
    return {
        "farmId": ...,
    }


# DisassociateMemberFromJobRequestTypeDef definition

class DisassociateMemberFromJobRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    principalId: str,
```

## DisassociateMemberFromQueueRequestTypeDef

```python
# DisassociateMemberFromQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DisassociateMemberFromQueueRequestTypeDef


def get_value() -> DisassociateMemberFromQueueRequestTypeDef:
    return {
        "farmId": ...,
    }


# DisassociateMemberFromQueueRequestTypeDef definition

class DisassociateMemberFromQueueRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    principalId: str,
```

## Ec2EbsVolumeTypeDef

```python
# Ec2EbsVolumeTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import Ec2EbsVolumeTypeDef


def get_value() -> Ec2EbsVolumeTypeDef:
    return {
        "sizeGiB": ...,
    }


# Ec2EbsVolumeTypeDef definition

class Ec2EbsVolumeTypeDef(TypedDict):
    sizeGiB: NotRequired[int],
    iops: NotRequired[int],
    throughputMiB: NotRequired[int],
```

## EnvironmentDetailsEntityTypeDef

```python
# EnvironmentDetailsEntityTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import EnvironmentDetailsEntityTypeDef


def get_value() -> EnvironmentDetailsEntityTypeDef:
    return {
        "jobId": ...,
    }


# EnvironmentDetailsEntityTypeDef definition

class EnvironmentDetailsEntityTypeDef(TypedDict):
    jobId: str,
    environmentId: str,
    schemaVersion: str,
    template: Dict[str, Any],
```

## EnvironmentDetailsErrorTypeDef

```python
# EnvironmentDetailsErrorTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import EnvironmentDetailsErrorTypeDef


def get_value() -> EnvironmentDetailsErrorTypeDef:
    return {
        "jobId": ...,
    }


# EnvironmentDetailsErrorTypeDef definition

class EnvironmentDetailsErrorTypeDef(TypedDict):
    jobId: str,
    environmentId: str,
    code: JobEntityErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: JobEntityErrorCodeType](./literals.md#jobentityerrorcodetype) 
## EnvironmentDetailsIdentifiersTypeDef

```python
# EnvironmentDetailsIdentifiersTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import EnvironmentDetailsIdentifiersTypeDef


def get_value() -> EnvironmentDetailsIdentifiersTypeDef:
    return {
        "jobId": ...,
    }


# EnvironmentDetailsIdentifiersTypeDef definition

class EnvironmentDetailsIdentifiersTypeDef(TypedDict):
    jobId: str,
    environmentId: str,
```

## EnvironmentEnterSessionActionDefinitionSummaryTypeDef

```python
# EnvironmentEnterSessionActionDefinitionSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import EnvironmentEnterSessionActionDefinitionSummaryTypeDef


def get_value() -> EnvironmentEnterSessionActionDefinitionSummaryTypeDef:
    return {
        "environmentId": ...,
    }


# EnvironmentEnterSessionActionDefinitionSummaryTypeDef definition

class EnvironmentEnterSessionActionDefinitionSummaryTypeDef(TypedDict):
    environmentId: str,
```

## EnvironmentEnterSessionActionDefinitionTypeDef

```python
# EnvironmentEnterSessionActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import EnvironmentEnterSessionActionDefinitionTypeDef


def get_value() -> EnvironmentEnterSessionActionDefinitionTypeDef:
    return {
        "environmentId": ...,
    }


# EnvironmentEnterSessionActionDefinitionTypeDef definition

class EnvironmentEnterSessionActionDefinitionTypeDef(TypedDict):
    environmentId: str,
```

## EnvironmentExitSessionActionDefinitionSummaryTypeDef

```python
# EnvironmentExitSessionActionDefinitionSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import EnvironmentExitSessionActionDefinitionSummaryTypeDef


def get_value() -> EnvironmentExitSessionActionDefinitionSummaryTypeDef:
    return {
        "environmentId": ...,
    }


# EnvironmentExitSessionActionDefinitionSummaryTypeDef definition

class EnvironmentExitSessionActionDefinitionSummaryTypeDef(TypedDict):
    environmentId: str,
```

## EnvironmentExitSessionActionDefinitionTypeDef

```python
# EnvironmentExitSessionActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import EnvironmentExitSessionActionDefinitionTypeDef


def get_value() -> EnvironmentExitSessionActionDefinitionTypeDef:
    return {
        "environmentId": ...,
    }


# EnvironmentExitSessionActionDefinitionTypeDef definition

class EnvironmentExitSessionActionDefinitionTypeDef(TypedDict):
    environmentId: str,
```

## FarmMemberTypeDef

```python
# FarmMemberTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FarmMemberTypeDef


def get_value() -> FarmMemberTypeDef:
    return {
        "farmId": ...,
    }


# FarmMemberTypeDef definition

class FarmMemberTypeDef(TypedDict):
    farmId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 
## FarmSummaryTypeDef

```python
# FarmSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FarmSummaryTypeDef


def get_value() -> FarmSummaryTypeDef:
    return {
        "farmId": ...,
    }


# FarmSummaryTypeDef definition

class FarmSummaryTypeDef(TypedDict):
    farmId: str,
    displayName: str,
    createdAt: datetime,
    createdBy: str,
    kmsKeyArn: NotRequired[str],
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

## FieldSortExpressionTypeDef

```python
# FieldSortExpressionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FieldSortExpressionTypeDef


def get_value() -> FieldSortExpressionTypeDef:
    return {
        "sortOrder": ...,
    }


# FieldSortExpressionTypeDef definition

class FieldSortExpressionTypeDef(TypedDict):
    sortOrder: SortOrderType,  # (1)
    name: str,
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## FleetMemberTypeDef

```python
# FleetMemberTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FleetMemberTypeDef


def get_value() -> FleetMemberTypeDef:
    return {
        "farmId": ...,
    }


# FleetMemberTypeDef definition

class FleetMemberTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 
## GetBudgetRequestTypeDef

```python
# GetBudgetRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetBudgetRequestTypeDef


def get_value() -> GetBudgetRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetBudgetRequestTypeDef definition

class GetBudgetRequestTypeDef(TypedDict):
    farmId: str,
    budgetId: str,
```

## ResponseBudgetActionTypeDef

```python
# ResponseBudgetActionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ResponseBudgetActionTypeDef


def get_value() -> ResponseBudgetActionTypeDef:
    return {
        "type": ...,
    }


# ResponseBudgetActionTypeDef definition

class ResponseBudgetActionTypeDef(TypedDict):
    type: BudgetActionTypeType,  # (1)
    thresholdPercentage: float,
    description: NotRequired[str],
```

1. See [:material-code-brackets: BudgetActionTypeType](./literals.md#budgetactiontypetype) 
## GetFarmRequestTypeDef

```python
# GetFarmRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetFarmRequestTypeDef


def get_value() -> GetFarmRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetFarmRequestTypeDef definition

class GetFarmRequestTypeDef(TypedDict):
    farmId: str,
```

## GetFleetRequestTypeDef

```python
# GetFleetRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetFleetRequestTypeDef


def get_value() -> GetFleetRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetFleetRequestTypeDef definition

class GetFleetRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## JobAttachmentDetailsErrorTypeDef

```python
# JobAttachmentDetailsErrorTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobAttachmentDetailsErrorTypeDef


def get_value() -> JobAttachmentDetailsErrorTypeDef:
    return {
        "jobId": ...,
    }


# JobAttachmentDetailsErrorTypeDef definition

class JobAttachmentDetailsErrorTypeDef(TypedDict):
    jobId: str,
    code: JobEntityErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: JobEntityErrorCodeType](./literals.md#jobentityerrorcodetype) 
## JobDetailsErrorTypeDef

```python
# JobDetailsErrorTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobDetailsErrorTypeDef


def get_value() -> JobDetailsErrorTypeDef:
    return {
        "jobId": ...,
    }


# JobDetailsErrorTypeDef definition

class JobDetailsErrorTypeDef(TypedDict):
    jobId: str,
    code: JobEntityErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: JobEntityErrorCodeType](./literals.md#jobentityerrorcodetype) 
## StepDetailsErrorTypeDef

```python
# StepDetailsErrorTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StepDetailsErrorTypeDef


def get_value() -> StepDetailsErrorTypeDef:
    return {
        "jobId": ...,
    }


# StepDetailsErrorTypeDef definition

class StepDetailsErrorTypeDef(TypedDict):
    jobId: str,
    stepId: str,
    code: JobEntityErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: JobEntityErrorCodeType](./literals.md#jobentityerrorcodetype) 
## GetJobRequestTypeDef

```python
# GetJobRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetJobRequestTypeDef


def get_value() -> GetJobRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetJobRequestTypeDef definition

class GetJobRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
```

## GetLicenseEndpointRequestTypeDef

```python
# GetLicenseEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetLicenseEndpointRequestTypeDef


def get_value() -> GetLicenseEndpointRequestTypeDef:
    return {
        "licenseEndpointId": ...,
    }


# GetLicenseEndpointRequestTypeDef definition

class GetLicenseEndpointRequestTypeDef(TypedDict):
    licenseEndpointId: str,
```

## GetLimitRequestTypeDef

```python
# GetLimitRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetLimitRequestTypeDef


def get_value() -> GetLimitRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetLimitRequestTypeDef definition

class GetLimitRequestTypeDef(TypedDict):
    farmId: str,
    limitId: str,
```

## GetMonitorRequestTypeDef

```python
# GetMonitorRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetMonitorRequestTypeDef


def get_value() -> GetMonitorRequestTypeDef:
    return {
        "monitorId": ...,
    }


# GetMonitorRequestTypeDef definition

class GetMonitorRequestTypeDef(TypedDict):
    monitorId: str,
```

## GetQueueEnvironmentRequestTypeDef

```python
# GetQueueEnvironmentRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueEnvironmentRequestTypeDef


def get_value() -> GetQueueEnvironmentRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetQueueEnvironmentRequestTypeDef definition

class GetQueueEnvironmentRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    queueEnvironmentId: str,
```

## GetQueueFleetAssociationRequestTypeDef

```python
# GetQueueFleetAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueFleetAssociationRequestTypeDef


def get_value() -> GetQueueFleetAssociationRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetQueueFleetAssociationRequestTypeDef definition

class GetQueueFleetAssociationRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    fleetId: str,
```

## GetQueueLimitAssociationRequestTypeDef

```python
# GetQueueLimitAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueLimitAssociationRequestTypeDef


def get_value() -> GetQueueLimitAssociationRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetQueueLimitAssociationRequestTypeDef definition

class GetQueueLimitAssociationRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    limitId: str,
```

## GetQueueRequestTypeDef

```python
# GetQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueRequestTypeDef


def get_value() -> GetQueueRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetQueueRequestTypeDef definition

class GetQueueRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
```

## GetSessionActionRequestTypeDef

```python
# GetSessionActionRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetSessionActionRequestTypeDef


def get_value() -> GetSessionActionRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetSessionActionRequestTypeDef definition

class GetSessionActionRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    sessionActionId: str,
```

## GetSessionRequestTypeDef

```python
# GetSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetSessionRequestTypeDef


def get_value() -> GetSessionRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetSessionRequestTypeDef definition

class GetSessionRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    sessionId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import PaginatorConfigTypeDef


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

## GetSessionsStatisticsAggregationRequestTypeDef

```python
# GetSessionsStatisticsAggregationRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetSessionsStatisticsAggregationRequestTypeDef


def get_value() -> GetSessionsStatisticsAggregationRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetSessionsStatisticsAggregationRequestTypeDef definition

class GetSessionsStatisticsAggregationRequestTypeDef(TypedDict):
    farmId: str,
    aggregationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetStepRequestTypeDef

```python
# GetStepRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetStepRequestTypeDef


def get_value() -> GetStepRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetStepRequestTypeDef definition

class GetStepRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
```

## GetStorageProfileForQueueRequestTypeDef

```python
# GetStorageProfileForQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetStorageProfileForQueueRequestTypeDef


def get_value() -> GetStorageProfileForQueueRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetStorageProfileForQueueRequestTypeDef definition

class GetStorageProfileForQueueRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    storageProfileId: str,
```

## GetStorageProfileRequestTypeDef

```python
# GetStorageProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetStorageProfileRequestTypeDef


def get_value() -> GetStorageProfileRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetStorageProfileRequestTypeDef definition

class GetStorageProfileRequestTypeDef(TypedDict):
    farmId: str,
    storageProfileId: str,
```

## GetTaskRequestTypeDef

```python
# GetTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetTaskRequestTypeDef


def get_value() -> GetTaskRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetTaskRequestTypeDef definition

class GetTaskRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    taskId: str,
```

## GetWorkerRequestTypeDef

```python
# GetWorkerRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetWorkerRequestTypeDef


def get_value() -> GetWorkerRequestTypeDef:
    return {
        "farmId": ...,
    }


# GetWorkerRequestTypeDef definition

class GetWorkerRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
```

## IpAddressesOutputTypeDef

```python
# IpAddressesOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import IpAddressesOutputTypeDef


def get_value() -> IpAddressesOutputTypeDef:
    return {
        "ipV4Addresses": ...,
    }


# IpAddressesOutputTypeDef definition

class IpAddressesOutputTypeDef(TypedDict):
    ipV4Addresses: NotRequired[List[str]],
    ipV6Addresses: NotRequired[List[str]],
```

## IpAddressesTypeDef

```python
# IpAddressesTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import IpAddressesTypeDef


def get_value() -> IpAddressesTypeDef:
    return {
        "ipV4Addresses": ...,
    }


# IpAddressesTypeDef definition

class IpAddressesTypeDef(TypedDict):
    ipV4Addresses: NotRequired[Sequence[str]],
    ipV6Addresses: NotRequired[Sequence[str]],
```

## JobAttachmentDetailsIdentifiersTypeDef

```python
# JobAttachmentDetailsIdentifiersTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobAttachmentDetailsIdentifiersTypeDef


def get_value() -> JobAttachmentDetailsIdentifiersTypeDef:
    return {
        "jobId": ...,
    }


# JobAttachmentDetailsIdentifiersTypeDef definition

class JobAttachmentDetailsIdentifiersTypeDef(TypedDict):
    jobId: str,
```

## PathMappingRuleTypeDef

```python
# PathMappingRuleTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import PathMappingRuleTypeDef


def get_value() -> PathMappingRuleTypeDef:
    return {
        "sourcePathFormat": ...,
    }


# PathMappingRuleTypeDef definition

class PathMappingRuleTypeDef(TypedDict):
    sourcePathFormat: PathFormatType,  # (1)
    sourcePath: str,
    destinationPath: str,
```

1. See [:material-code-brackets: PathFormatType](./literals.md#pathformattype) 
## JobDetailsIdentifiersTypeDef

```python
# JobDetailsIdentifiersTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobDetailsIdentifiersTypeDef


def get_value() -> JobDetailsIdentifiersTypeDef:
    return {
        "jobId": ...,
    }


# JobDetailsIdentifiersTypeDef definition

class JobDetailsIdentifiersTypeDef(TypedDict):
    jobId: str,
```

## StepDetailsIdentifiersTypeDef

```python
# StepDetailsIdentifiersTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StepDetailsIdentifiersTypeDef


def get_value() -> StepDetailsIdentifiersTypeDef:
    return {
        "jobId": ...,
    }


# StepDetailsIdentifiersTypeDef definition

class StepDetailsIdentifiersTypeDef(TypedDict):
    jobId: str,
    stepId: str,
```

## StepDetailsEntityTypeDef

```python
# StepDetailsEntityTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StepDetailsEntityTypeDef


def get_value() -> StepDetailsEntityTypeDef:
    return {
        "jobId": ...,
    }


# StepDetailsEntityTypeDef definition

class StepDetailsEntityTypeDef(TypedDict):
    jobId: str,
    stepId: str,
    schemaVersion: str,
    template: Dict[str, Any],
    dependencies: List[str],
```

## JobMemberTypeDef

```python
# JobMemberTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobMemberTypeDef


def get_value() -> JobMemberTypeDef:
    return {
        "farmId": ...,
    }


# JobMemberTypeDef definition

class JobMemberTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 
## PosixUserTypeDef

```python
# PosixUserTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import PosixUserTypeDef


def get_value() -> PosixUserTypeDef:
    return {
        "user": ...,
    }


# PosixUserTypeDef definition

class PosixUserTypeDef(TypedDict):
    user: str,
    group: str,
```

## WindowsUserTypeDef

```python
# WindowsUserTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import WindowsUserTypeDef


def get_value() -> WindowsUserTypeDef:
    return {
        "user": ...,
    }


# WindowsUserTypeDef definition

class WindowsUserTypeDef(TypedDict):
    user: str,
    passwordArn: str,
```

## JobSummaryTypeDef

```python
# JobSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobSummaryTypeDef


def get_value() -> JobSummaryTypeDef:
    return {
        "jobId": ...,
    }


# JobSummaryTypeDef definition

class JobSummaryTypeDef(TypedDict):
    jobId: str,
    name: str,
    lifecycleStatus: JobLifecycleStatusType,  # (1)
    lifecycleStatusMessage: str,
    priority: int,
    createdAt: datetime,
    createdBy: str,
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
    startedAt: NotRequired[datetime],
    endedAt: NotRequired[datetime],
    taskRunStatus: NotRequired[TaskRunStatusType],  # (2)
    targetTaskRunStatus: NotRequired[JobTargetTaskRunStatusType],  # (3)
    taskRunStatusCounts: NotRequired[Dict[TaskRunStatusType, int]],  # (4)
    maxFailedTasksCount: NotRequired[int],
    maxRetriesPerTask: NotRequired[int],
    maxWorkerCount: NotRequired[int],
    sourceJobId: NotRequired[str],
```

1. See [:material-code-brackets: JobLifecycleStatusType](./literals.md#joblifecyclestatustype) 
2. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
3. See [:material-code-brackets: JobTargetTaskRunStatusType](./literals.md#jobtargettaskrunstatustype) 
4. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
## LicenseEndpointSummaryTypeDef

```python
# LicenseEndpointSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import LicenseEndpointSummaryTypeDef


def get_value() -> LicenseEndpointSummaryTypeDef:
    return {
        "licenseEndpointId": ...,
    }


# LicenseEndpointSummaryTypeDef definition

class LicenseEndpointSummaryTypeDef(TypedDict):
    licenseEndpointId: NotRequired[str],
    status: NotRequired[LicenseEndpointStatusType],  # (1)
    statusMessage: NotRequired[str],
    vpcId: NotRequired[str],
```

1. See [:material-code-brackets: LicenseEndpointStatusType](./literals.md#licenseendpointstatustype) 
## LimitSummaryTypeDef

```python
# LimitSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import LimitSummaryTypeDef


def get_value() -> LimitSummaryTypeDef:
    return {
        "displayName": ...,
    }


# LimitSummaryTypeDef definition

class LimitSummaryTypeDef(TypedDict):
    displayName: str,
    amountRequirementName: str,
    maxCount: int,
    createdAt: datetime,
    createdBy: str,
    farmId: str,
    limitId: str,
    currentCount: int,
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

## ListAvailableMeteredProductsRequestTypeDef

```python
# ListAvailableMeteredProductsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListAvailableMeteredProductsRequestTypeDef


def get_value() -> ListAvailableMeteredProductsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListAvailableMeteredProductsRequestTypeDef definition

class ListAvailableMeteredProductsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## MeteredProductSummaryTypeDef

```python
# MeteredProductSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import MeteredProductSummaryTypeDef


def get_value() -> MeteredProductSummaryTypeDef:
    return {
        "productId": ...,
    }


# MeteredProductSummaryTypeDef definition

class MeteredProductSummaryTypeDef(TypedDict):
    productId: str,
    family: str,
    vendor: str,
    port: int,
```

## ListBudgetsRequestTypeDef

```python
# ListBudgetsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListBudgetsRequestTypeDef


def get_value() -> ListBudgetsRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListBudgetsRequestTypeDef definition

class ListBudgetsRequestTypeDef(TypedDict):
    farmId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    status: NotRequired[BudgetStatusType],  # (1)
```

1. See [:material-code-brackets: BudgetStatusType](./literals.md#budgetstatustype) 
## ListFarmMembersRequestTypeDef

```python
# ListFarmMembersRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFarmMembersRequestTypeDef


def get_value() -> ListFarmMembersRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListFarmMembersRequestTypeDef definition

class ListFarmMembersRequestTypeDef(TypedDict):
    farmId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListFarmsRequestTypeDef

```python
# ListFarmsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFarmsRequestTypeDef


def get_value() -> ListFarmsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListFarmsRequestTypeDef definition

class ListFarmsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    principalId: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListFleetMembersRequestTypeDef

```python
# ListFleetMembersRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFleetMembersRequestTypeDef


def get_value() -> ListFleetMembersRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListFleetMembersRequestTypeDef definition

class ListFleetMembersRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListFleetsRequestTypeDef

```python
# ListFleetsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFleetsRequestTypeDef


def get_value() -> ListFleetsRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListFleetsRequestTypeDef definition

class ListFleetsRequestTypeDef(TypedDict):
    farmId: str,
    principalId: NotRequired[str],
    displayName: NotRequired[str],
    status: NotRequired[FleetStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: FleetStatusType](./literals.md#fleetstatustype) 
## ListJobMembersRequestTypeDef

```python
# ListJobMembersRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListJobMembersRequestTypeDef


def get_value() -> ListJobMembersRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListJobMembersRequestTypeDef definition

class ListJobMembersRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListJobParameterDefinitionsRequestTypeDef

```python
# ListJobParameterDefinitionsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListJobParameterDefinitionsRequestTypeDef


def get_value() -> ListJobParameterDefinitionsRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListJobParameterDefinitionsRequestTypeDef definition

class ListJobParameterDefinitionsRequestTypeDef(TypedDict):
    farmId: str,
    jobId: str,
    queueId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListJobsRequestTypeDef

```python
# ListJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListJobsRequestTypeDef


def get_value() -> ListJobsRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListJobsRequestTypeDef definition

class ListJobsRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    principalId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListLicenseEndpointsRequestTypeDef

```python
# ListLicenseEndpointsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListLicenseEndpointsRequestTypeDef


def get_value() -> ListLicenseEndpointsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListLicenseEndpointsRequestTypeDef definition

class ListLicenseEndpointsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListLimitsRequestTypeDef

```python
# ListLimitsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListLimitsRequestTypeDef


def get_value() -> ListLimitsRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListLimitsRequestTypeDef definition

class ListLimitsRequestTypeDef(TypedDict):
    farmId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMeteredProductsRequestTypeDef

```python
# ListMeteredProductsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListMeteredProductsRequestTypeDef


def get_value() -> ListMeteredProductsRequestTypeDef:
    return {
        "licenseEndpointId": ...,
    }


# ListMeteredProductsRequestTypeDef definition

class ListMeteredProductsRequestTypeDef(TypedDict):
    licenseEndpointId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMonitorsRequestTypeDef

```python
# ListMonitorsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListMonitorsRequestTypeDef


def get_value() -> ListMonitorsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListMonitorsRequestTypeDef definition

class ListMonitorsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## MonitorSummaryTypeDef

```python
# MonitorSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import MonitorSummaryTypeDef


def get_value() -> MonitorSummaryTypeDef:
    return {
        "monitorId": ...,
    }


# MonitorSummaryTypeDef definition

class MonitorSummaryTypeDef(TypedDict):
    monitorId: str,
    displayName: str,
    subdomain: str,
    url: str,
    roleArn: str,
    identityCenterInstanceArn: str,
    identityCenterApplicationArn: str,
    createdAt: datetime,
    createdBy: str,
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

## ListQueueEnvironmentsRequestTypeDef

```python
# ListQueueEnvironmentsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueEnvironmentsRequestTypeDef


def get_value() -> ListQueueEnvironmentsRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListQueueEnvironmentsRequestTypeDef definition

class ListQueueEnvironmentsRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## QueueEnvironmentSummaryTypeDef

```python
# QueueEnvironmentSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import QueueEnvironmentSummaryTypeDef


def get_value() -> QueueEnvironmentSummaryTypeDef:
    return {
        "queueEnvironmentId": ...,
    }


# QueueEnvironmentSummaryTypeDef definition

class QueueEnvironmentSummaryTypeDef(TypedDict):
    queueEnvironmentId: str,
    name: str,
    priority: int,
```

## ListQueueFleetAssociationsRequestTypeDef

```python
# ListQueueFleetAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueFleetAssociationsRequestTypeDef


def get_value() -> ListQueueFleetAssociationsRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListQueueFleetAssociationsRequestTypeDef definition

class ListQueueFleetAssociationsRequestTypeDef(TypedDict):
    farmId: str,
    queueId: NotRequired[str],
    fleetId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## QueueFleetAssociationSummaryTypeDef

```python
# QueueFleetAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import QueueFleetAssociationSummaryTypeDef


def get_value() -> QueueFleetAssociationSummaryTypeDef:
    return {
        "queueId": ...,
    }


# QueueFleetAssociationSummaryTypeDef definition

class QueueFleetAssociationSummaryTypeDef(TypedDict):
    queueId: str,
    fleetId: str,
    status: QueueFleetAssociationStatusType,  # (1)
    createdAt: datetime,
    createdBy: str,
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-brackets: QueueFleetAssociationStatusType](./literals.md#queuefleetassociationstatustype) 
## ListQueueLimitAssociationsRequestTypeDef

```python
# ListQueueLimitAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueLimitAssociationsRequestTypeDef


def get_value() -> ListQueueLimitAssociationsRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListQueueLimitAssociationsRequestTypeDef definition

class ListQueueLimitAssociationsRequestTypeDef(TypedDict):
    farmId: str,
    queueId: NotRequired[str],
    limitId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## QueueLimitAssociationSummaryTypeDef

```python
# QueueLimitAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import QueueLimitAssociationSummaryTypeDef


def get_value() -> QueueLimitAssociationSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# QueueLimitAssociationSummaryTypeDef definition

class QueueLimitAssociationSummaryTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    queueId: str,
    limitId: str,
    status: QueueLimitAssociationStatusType,  # (1)
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-brackets: QueueLimitAssociationStatusType](./literals.md#queuelimitassociationstatustype) 
## ListQueueMembersRequestTypeDef

```python
# ListQueueMembersRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueMembersRequestTypeDef


def get_value() -> ListQueueMembersRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListQueueMembersRequestTypeDef definition

class ListQueueMembersRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## QueueMemberTypeDef

```python
# QueueMemberTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import QueueMemberTypeDef


def get_value() -> QueueMemberTypeDef:
    return {
        "farmId": ...,
    }


# QueueMemberTypeDef definition

class QueueMemberTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 
## ListQueuesRequestTypeDef

```python
# ListQueuesRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueuesRequestTypeDef


def get_value() -> ListQueuesRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListQueuesRequestTypeDef definition

class ListQueuesRequestTypeDef(TypedDict):
    farmId: str,
    principalId: NotRequired[str],
    status: NotRequired[QueueStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
## QueueSummaryTypeDef

```python
# QueueSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import QueueSummaryTypeDef


def get_value() -> QueueSummaryTypeDef:
    return {
        "farmId": ...,
    }


# QueueSummaryTypeDef definition

class QueueSummaryTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    displayName: str,
    status: QueueStatusType,  # (1)
    defaultBudgetAction: DefaultQueueBudgetActionType,  # (2)
    createdAt: datetime,
    createdBy: str,
    blockedReason: NotRequired[QueueBlockedReasonType],  # (3)
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
2. See [:material-code-brackets: DefaultQueueBudgetActionType](./literals.md#defaultqueuebudgetactiontype) 
3. See [:material-code-brackets: QueueBlockedReasonType](./literals.md#queueblockedreasontype) 
## ListSessionActionsRequestTypeDef

```python
# ListSessionActionsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListSessionActionsRequestTypeDef


def get_value() -> ListSessionActionsRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListSessionActionsRequestTypeDef definition

class ListSessionActionsRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    sessionId: NotRequired[str],
    taskId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListSessionsForWorkerRequestTypeDef

```python
# ListSessionsForWorkerRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListSessionsForWorkerRequestTypeDef


def get_value() -> ListSessionsForWorkerRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListSessionsForWorkerRequestTypeDef definition

class ListSessionsForWorkerRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## WorkerSessionSummaryTypeDef

```python
# WorkerSessionSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import WorkerSessionSummaryTypeDef


def get_value() -> WorkerSessionSummaryTypeDef:
    return {
        "sessionId": ...,
    }


# WorkerSessionSummaryTypeDef definition

class WorkerSessionSummaryTypeDef(TypedDict):
    sessionId: str,
    queueId: str,
    jobId: str,
    startedAt: datetime,
    lifecycleStatus: SessionLifecycleStatusType,  # (1)
    endedAt: NotRequired[datetime],
    targetLifecycleStatus: NotRequired[SessionLifecycleTargetStatusType],  # (2)
```

1. See [:material-code-brackets: SessionLifecycleStatusType](./literals.md#sessionlifecyclestatustype) 
2. See [:material-code-brackets: SessionLifecycleTargetStatusType](./literals.md#sessionlifecycletargetstatustype) 
## ListSessionsRequestTypeDef

```python
# ListSessionsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListSessionsRequestTypeDef


def get_value() -> ListSessionsRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListSessionsRequestTypeDef definition

class ListSessionsRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## SessionSummaryTypeDef

```python
# SessionSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SessionSummaryTypeDef


def get_value() -> SessionSummaryTypeDef:
    return {
        "sessionId": ...,
    }


# SessionSummaryTypeDef definition

class SessionSummaryTypeDef(TypedDict):
    sessionId: str,
    fleetId: str,
    workerId: str,
    startedAt: datetime,
    lifecycleStatus: SessionLifecycleStatusType,  # (1)
    endedAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
    targetLifecycleStatus: NotRequired[SessionLifecycleTargetStatusType],  # (2)
```

1. See [:material-code-brackets: SessionLifecycleStatusType](./literals.md#sessionlifecyclestatustype) 
2. See [:material-code-brackets: SessionLifecycleTargetStatusType](./literals.md#sessionlifecycletargetstatustype) 
## ListStepConsumersRequestTypeDef

```python
# ListStepConsumersRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStepConsumersRequestTypeDef


def get_value() -> ListStepConsumersRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListStepConsumersRequestTypeDef definition

class ListStepConsumersRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StepConsumerTypeDef

```python
# StepConsumerTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StepConsumerTypeDef


def get_value() -> StepConsumerTypeDef:
    return {
        "stepId": ...,
    }


# StepConsumerTypeDef definition

class StepConsumerTypeDef(TypedDict):
    stepId: str,
    status: DependencyConsumerResolutionStatusType,  # (1)
```

1. See [:material-code-brackets: DependencyConsumerResolutionStatusType](./literals.md#dependencyconsumerresolutionstatustype) 
## ListStepDependenciesRequestTypeDef

```python
# ListStepDependenciesRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStepDependenciesRequestTypeDef


def get_value() -> ListStepDependenciesRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListStepDependenciesRequestTypeDef definition

class ListStepDependenciesRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StepDependencyTypeDef

```python
# StepDependencyTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StepDependencyTypeDef


def get_value() -> StepDependencyTypeDef:
    return {
        "stepId": ...,
    }


# StepDependencyTypeDef definition

class StepDependencyTypeDef(TypedDict):
    stepId: str,
    status: DependencyConsumerResolutionStatusType,  # (1)
```

1. See [:material-code-brackets: DependencyConsumerResolutionStatusType](./literals.md#dependencyconsumerresolutionstatustype) 
## ListStepsRequestTypeDef

```python
# ListStepsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStepsRequestTypeDef


def get_value() -> ListStepsRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListStepsRequestTypeDef definition

class ListStepsRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListStorageProfilesForQueueRequestTypeDef

```python
# ListStorageProfilesForQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStorageProfilesForQueueRequestTypeDef


def get_value() -> ListStorageProfilesForQueueRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListStorageProfilesForQueueRequestTypeDef definition

class ListStorageProfilesForQueueRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StorageProfileSummaryTypeDef

```python
# StorageProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StorageProfileSummaryTypeDef


def get_value() -> StorageProfileSummaryTypeDef:
    return {
        "storageProfileId": ...,
    }


# StorageProfileSummaryTypeDef definition

class StorageProfileSummaryTypeDef(TypedDict):
    storageProfileId: str,
    displayName: str,
    osFamily: StorageProfileOperatingSystemFamilyType,  # (1)
```

1. See [:material-code-brackets: StorageProfileOperatingSystemFamilyType](./literals.md#storageprofileoperatingsystemfamilytype) 
## ListStorageProfilesRequestTypeDef

```python
# ListStorageProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStorageProfilesRequestTypeDef


def get_value() -> ListStorageProfilesRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListStorageProfilesRequestTypeDef definition

class ListStorageProfilesRequestTypeDef(TypedDict):
    farmId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTasksRequestTypeDef

```python
# ListTasksRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListTasksRequestTypeDef


def get_value() -> ListTasksRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListTasksRequestTypeDef definition

class ListTasksRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListWorkersRequestTypeDef

```python
# ListWorkersRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListWorkersRequestTypeDef


def get_value() -> ListWorkersRequestTypeDef:
    return {
        "farmId": ...,
    }


# ListWorkersRequestTypeDef definition

class ListWorkersRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ParameterFilterExpressionTypeDef

```python
# ParameterFilterExpressionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ParameterFilterExpressionTypeDef


def get_value() -> ParameterFilterExpressionTypeDef:
    return {
        "name": ...,
    }


# ParameterFilterExpressionTypeDef definition

class ParameterFilterExpressionTypeDef(TypedDict):
    name: str,
    operator: ComparisonOperatorType,  # (1)
    value: str,
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## ParameterSortExpressionTypeDef

```python
# ParameterSortExpressionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ParameterSortExpressionTypeDef


def get_value() -> ParameterSortExpressionTypeDef:
    return {
        "sortOrder": ...,
    }


# ParameterSortExpressionTypeDef definition

class ParameterSortExpressionTypeDef(TypedDict):
    sortOrder: SortOrderType,  # (1)
    name: str,
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## StepParameterTypeDef

```python
# StepParameterTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StepParameterTypeDef


def get_value() -> StepParameterTypeDef:
    return {
        "name": ...,
    }


# StepParameterTypeDef definition

class StepParameterTypeDef(TypedDict):
    name: str,
    type: StepParameterTypeType,  # (1)
```

1. See [:material-code-brackets: StepParameterTypeType](./literals.md#stepparametertypetype) 
## PutMeteredProductRequestTypeDef

```python
# PutMeteredProductRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import PutMeteredProductRequestTypeDef


def get_value() -> PutMeteredProductRequestTypeDef:
    return {
        "licenseEndpointId": ...,
    }


# PutMeteredProductRequestTypeDef definition

class PutMeteredProductRequestTypeDef(TypedDict):
    licenseEndpointId: str,
    productId: str,
```

## SearchTermFilterExpressionTypeDef

```python
# SearchTermFilterExpressionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchTermFilterExpressionTypeDef


def get_value() -> SearchTermFilterExpressionTypeDef:
    return {
        "searchTerm": ...,
    }


# SearchTermFilterExpressionTypeDef definition

class SearchTermFilterExpressionTypeDef(TypedDict):
    searchTerm: str,
```

## StringFilterExpressionTypeDef

```python
# StringFilterExpressionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StringFilterExpressionTypeDef


def get_value() -> StringFilterExpressionTypeDef:
    return {
        "name": ...,
    }


# StringFilterExpressionTypeDef definition

class StringFilterExpressionTypeDef(TypedDict):
    name: str,
    operator: ComparisonOperatorType,  # (1)
    value: str,
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## UserJobsFirstTypeDef

```python
# UserJobsFirstTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UserJobsFirstTypeDef


def get_value() -> UserJobsFirstTypeDef:
    return {
        "userIdentityId": ...,
    }


# UserJobsFirstTypeDef definition

class UserJobsFirstTypeDef(TypedDict):
    userIdentityId: str,
```

## ServiceManagedEc2InstanceMarketOptionsTypeDef

```python
# ServiceManagedEc2InstanceMarketOptionsTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ServiceManagedEc2InstanceMarketOptionsTypeDef


def get_value() -> ServiceManagedEc2InstanceMarketOptionsTypeDef:
    return {
        "type": ...,
    }


# ServiceManagedEc2InstanceMarketOptionsTypeDef definition

class ServiceManagedEc2InstanceMarketOptionsTypeDef(TypedDict):
    type: Ec2MarketTypeType,  # (1)
```

1. See [:material-code-brackets: Ec2MarketTypeType](./literals.md#ec2markettypetype) 
## SyncInputJobAttachmentsSessionActionDefinitionSummaryTypeDef

```python
# SyncInputJobAttachmentsSessionActionDefinitionSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SyncInputJobAttachmentsSessionActionDefinitionSummaryTypeDef


def get_value() -> SyncInputJobAttachmentsSessionActionDefinitionSummaryTypeDef:
    return {
        "stepId": ...,
    }


# SyncInputJobAttachmentsSessionActionDefinitionSummaryTypeDef definition

class SyncInputJobAttachmentsSessionActionDefinitionSummaryTypeDef(TypedDict):
    stepId: NotRequired[str],
```

## TaskRunSessionActionDefinitionSummaryTypeDef

```python
# TaskRunSessionActionDefinitionSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import TaskRunSessionActionDefinitionSummaryTypeDef


def get_value() -> TaskRunSessionActionDefinitionSummaryTypeDef:
    return {
        "taskId": ...,
    }


# TaskRunSessionActionDefinitionSummaryTypeDef definition

class TaskRunSessionActionDefinitionSummaryTypeDef(TypedDict):
    taskId: str,
    stepId: str,
```

## SyncInputJobAttachmentsSessionActionDefinitionTypeDef

```python
# SyncInputJobAttachmentsSessionActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SyncInputJobAttachmentsSessionActionDefinitionTypeDef


def get_value() -> SyncInputJobAttachmentsSessionActionDefinitionTypeDef:
    return {
        "stepId": ...,
    }


# SyncInputJobAttachmentsSessionActionDefinitionTypeDef definition

class SyncInputJobAttachmentsSessionActionDefinitionTypeDef(TypedDict):
    stepId: NotRequired[str],
```

## SessionsStatisticsResourcesTypeDef

```python
# SessionsStatisticsResourcesTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SessionsStatisticsResourcesTypeDef


def get_value() -> SessionsStatisticsResourcesTypeDef:
    return {
        "queueIds": ...,
    }


# SessionsStatisticsResourcesTypeDef definition

class SessionsStatisticsResourcesTypeDef(TypedDict):
    queueIds: NotRequired[Sequence[str]],
    fleetIds: NotRequired[Sequence[str]],
```

## StatsTypeDef

```python
# StatsTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StatsTypeDef


def get_value() -> StatsTypeDef:
    return {
        "min": ...,
    }


# StatsTypeDef definition

class StatsTypeDef(TypedDict):
    min: NotRequired[float],
    max: NotRequired[float],
    avg: NotRequired[float],
    sum: NotRequired[float],
```

## StepAmountCapabilityTypeDef

```python
# StepAmountCapabilityTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StepAmountCapabilityTypeDef


def get_value() -> StepAmountCapabilityTypeDef:
    return {
        "name": ...,
    }


# StepAmountCapabilityTypeDef definition

class StepAmountCapabilityTypeDef(TypedDict):
    name: str,
    min: NotRequired[float],
    max: NotRequired[float],
    value: NotRequired[float],
```

## StepAttributeCapabilityTypeDef

```python
# StepAttributeCapabilityTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StepAttributeCapabilityTypeDef


def get_value() -> StepAttributeCapabilityTypeDef:
    return {
        "name": ...,
    }


# StepAttributeCapabilityTypeDef definition

class StepAttributeCapabilityTypeDef(TypedDict):
    name: str,
    anyOf: NotRequired[List[str]],
    allOf: NotRequired[List[str]],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: NotRequired[Mapping[str, str]],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateFarmRequestTypeDef

```python
# UpdateFarmRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateFarmRequestTypeDef


def get_value() -> UpdateFarmRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateFarmRequestTypeDef definition

class UpdateFarmRequestTypeDef(TypedDict):
    farmId: str,
    displayName: NotRequired[str],
    description: NotRequired[str],
```

## UpdateJobRequestTypeDef

```python
# UpdateJobRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateJobRequestTypeDef


def get_value() -> UpdateJobRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateJobRequestTypeDef definition

class UpdateJobRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    clientToken: NotRequired[str],
    targetTaskRunStatus: NotRequired[JobTargetTaskRunStatusType],  # (1)
    priority: NotRequired[int],
    maxFailedTasksCount: NotRequired[int],
    maxRetriesPerTask: NotRequired[int],
    lifecycleStatus: NotRequired[UpdateJobLifecycleStatusType],  # (2)
    maxWorkerCount: NotRequired[int],
```

1. See [:material-code-brackets: JobTargetTaskRunStatusType](./literals.md#jobtargettaskrunstatustype) 
2. See [:material-code-brackets: UpdateJobLifecycleStatusType](./literals.md#updatejoblifecyclestatustype) 
## UpdateLimitRequestTypeDef

```python
# UpdateLimitRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateLimitRequestTypeDef


def get_value() -> UpdateLimitRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateLimitRequestTypeDef definition

class UpdateLimitRequestTypeDef(TypedDict):
    farmId: str,
    limitId: str,
    displayName: NotRequired[str],
    description: NotRequired[str],
    maxCount: NotRequired[int],
```

## UpdateMonitorRequestTypeDef

```python
# UpdateMonitorRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateMonitorRequestTypeDef


def get_value() -> UpdateMonitorRequestTypeDef:
    return {
        "monitorId": ...,
    }


# UpdateMonitorRequestTypeDef definition

class UpdateMonitorRequestTypeDef(TypedDict):
    monitorId: str,
    subdomain: NotRequired[str],
    displayName: NotRequired[str],
    roleArn: NotRequired[str],
```

## UpdateQueueEnvironmentRequestTypeDef

```python
# UpdateQueueEnvironmentRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateQueueEnvironmentRequestTypeDef


def get_value() -> UpdateQueueEnvironmentRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateQueueEnvironmentRequestTypeDef definition

class UpdateQueueEnvironmentRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    queueEnvironmentId: str,
    clientToken: NotRequired[str],
    priority: NotRequired[int],
    templateType: NotRequired[EnvironmentTemplateTypeType],  # (1)
    template: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentTemplateTypeType](./literals.md#environmenttemplatetypetype) 
## UpdateQueueFleetAssociationRequestTypeDef

```python
# UpdateQueueFleetAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateQueueFleetAssociationRequestTypeDef


def get_value() -> UpdateQueueFleetAssociationRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateQueueFleetAssociationRequestTypeDef definition

class UpdateQueueFleetAssociationRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    fleetId: str,
    status: UpdateQueueFleetAssociationStatusType,  # (1)
```

1. See [:material-code-brackets: UpdateQueueFleetAssociationStatusType](./literals.md#updatequeuefleetassociationstatustype) 
## UpdateQueueLimitAssociationRequestTypeDef

```python
# UpdateQueueLimitAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateQueueLimitAssociationRequestTypeDef


def get_value() -> UpdateQueueLimitAssociationRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateQueueLimitAssociationRequestTypeDef definition

class UpdateQueueLimitAssociationRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    limitId: str,
    status: UpdateQueueLimitAssociationStatusType,  # (1)
```

1. See [:material-code-brackets: UpdateQueueLimitAssociationStatusType](./literals.md#updatequeuelimitassociationstatustype) 
## UpdateSessionRequestTypeDef

```python
# UpdateSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateSessionRequestTypeDef


def get_value() -> UpdateSessionRequestTypeDef:
    return {
        "targetLifecycleStatus": ...,
    }


# UpdateSessionRequestTypeDef definition

class UpdateSessionRequestTypeDef(TypedDict):
    targetLifecycleStatus: SessionLifecycleTargetStatusType,  # (1)
    farmId: str,
    queueId: str,
    jobId: str,
    sessionId: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: SessionLifecycleTargetStatusType](./literals.md#sessionlifecycletargetstatustype) 
## UpdateStepRequestTypeDef

```python
# UpdateStepRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateStepRequestTypeDef


def get_value() -> UpdateStepRequestTypeDef:
    return {
        "targetTaskRunStatus": ...,
    }


# UpdateStepRequestTypeDef definition

class UpdateStepRequestTypeDef(TypedDict):
    targetTaskRunStatus: StepTargetTaskRunStatusType,  # (1)
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: StepTargetTaskRunStatusType](./literals.md#steptargettaskrunstatustype) 
## UpdateTaskRequestTypeDef

```python
# UpdateTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateTaskRequestTypeDef


def get_value() -> UpdateTaskRequestTypeDef:
    return {
        "targetRunStatus": ...,
    }


# UpdateTaskRequestTypeDef definition

class UpdateTaskRequestTypeDef(TypedDict):
    targetRunStatus: TaskTargetRunStatusType,  # (1)
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    taskId: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: TaskTargetRunStatusType](./literals.md#tasktargetrunstatustype) 
## WorkerAmountCapabilityTypeDef

```python
# WorkerAmountCapabilityTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import WorkerAmountCapabilityTypeDef


def get_value() -> WorkerAmountCapabilityTypeDef:
    return {
        "name": ...,
    }


# WorkerAmountCapabilityTypeDef definition

class WorkerAmountCapabilityTypeDef(TypedDict):
    name: str,
    value: float,
```

## WorkerAttributeCapabilityTypeDef

```python
# WorkerAttributeCapabilityTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import WorkerAttributeCapabilityTypeDef


def get_value() -> WorkerAttributeCapabilityTypeDef:
    return {
        "name": ...,
    }


# WorkerAttributeCapabilityTypeDef definition

class WorkerAttributeCapabilityTypeDef(TypedDict):
    name: str,
    values: Sequence[str],
```

## AcceleratorCapabilitiesOutputTypeDef

```python
# AcceleratorCapabilitiesOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AcceleratorCapabilitiesOutputTypeDef


def get_value() -> AcceleratorCapabilitiesOutputTypeDef:
    return {
        "selections": ...,
    }


# AcceleratorCapabilitiesOutputTypeDef definition

class AcceleratorCapabilitiesOutputTypeDef(TypedDict):
    selections: List[AcceleratorSelectionTypeDef],  # (1)
    count: NotRequired[AcceleratorCountRangeTypeDef],  # (2)
```

1. See [:material-code-braces: AcceleratorSelectionTypeDef](./type_defs.md#acceleratorselectiontypedef) 
2. See [:material-code-braces: AcceleratorCountRangeTypeDef](./type_defs.md#acceleratorcountrangetypedef) 
## AcceleratorCapabilitiesTypeDef

```python
# AcceleratorCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AcceleratorCapabilitiesTypeDef


def get_value() -> AcceleratorCapabilitiesTypeDef:
    return {
        "selections": ...,
    }


# AcceleratorCapabilitiesTypeDef definition

class AcceleratorCapabilitiesTypeDef(TypedDict):
    selections: Sequence[AcceleratorSelectionTypeDef],  # (1)
    count: NotRequired[AcceleratorCountRangeTypeDef],  # (2)
```

1. See [:material-code-braces: AcceleratorSelectionTypeDef](./type_defs.md#acceleratorselectiontypedef) 
2. See [:material-code-braces: AcceleratorCountRangeTypeDef](./type_defs.md#acceleratorcountrangetypedef) 
## AssignedTaskRunSessionActionDefinitionTypeDef

```python
# AssignedTaskRunSessionActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssignedTaskRunSessionActionDefinitionTypeDef


def get_value() -> AssignedTaskRunSessionActionDefinitionTypeDef:
    return {
        "taskId": ...,
    }


# AssignedTaskRunSessionActionDefinitionTypeDef definition

class AssignedTaskRunSessionActionDefinitionTypeDef(TypedDict):
    taskId: str,
    stepId: str,
    parameters: Dict[str, TaskParameterValueTypeDef],  # (1)
```

1. See [:material-code-braces: TaskParameterValueTypeDef](./type_defs.md#taskparametervaluetypedef) 
## TaskRunSessionActionDefinitionTypeDef

```python
# TaskRunSessionActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import TaskRunSessionActionDefinitionTypeDef


def get_value() -> TaskRunSessionActionDefinitionTypeDef:
    return {
        "taskId": ...,
    }


# TaskRunSessionActionDefinitionTypeDef definition

class TaskRunSessionActionDefinitionTypeDef(TypedDict):
    taskId: str,
    stepId: str,
    parameters: Dict[str, TaskParameterValueTypeDef],  # (1)
```

1. See [:material-code-braces: TaskParameterValueTypeDef](./type_defs.md#taskparametervaluetypedef) 
## TaskSearchSummaryTypeDef

```python
# TaskSearchSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import TaskSearchSummaryTypeDef


def get_value() -> TaskSearchSummaryTypeDef:
    return {
        "taskId": ...,
    }


# TaskSearchSummaryTypeDef definition

class TaskSearchSummaryTypeDef(TypedDict):
    taskId: NotRequired[str],
    stepId: NotRequired[str],
    jobId: NotRequired[str],
    queueId: NotRequired[str],
    runStatus: NotRequired[TaskRunStatusType],  # (1)
    targetRunStatus: NotRequired[TaskTargetRunStatusType],  # (2)
    parameters: NotRequired[Dict[str, TaskParameterValueTypeDef]],  # (3)
    failureRetryCount: NotRequired[int],
    startedAt: NotRequired[datetime],
    endedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
2. See [:material-code-brackets: TaskTargetRunStatusType](./literals.md#tasktargetrunstatustype) 
3. See [:material-code-braces: TaskParameterValueTypeDef](./type_defs.md#taskparametervaluetypedef) 
## TaskSummaryTypeDef

```python
# TaskSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import TaskSummaryTypeDef


def get_value() -> TaskSummaryTypeDef:
    return {
        "taskId": ...,
    }


# TaskSummaryTypeDef definition

class TaskSummaryTypeDef(TypedDict):
    taskId: str,
    createdAt: datetime,
    createdBy: str,
    runStatus: TaskRunStatusType,  # (1)
    targetRunStatus: NotRequired[TaskTargetRunStatusType],  # (2)
    failureRetryCount: NotRequired[int],
    parameters: NotRequired[Dict[str, TaskParameterValueTypeDef]],  # (3)
    startedAt: NotRequired[datetime],
    endedAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
    latestSessionActionId: NotRequired[str],
```

1. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
2. See [:material-code-brackets: TaskTargetRunStatusType](./literals.md#tasktargetrunstatustype) 
3. See [:material-code-braces: TaskParameterValueTypeDef](./type_defs.md#taskparametervaluetypedef) 
## AssumeFleetRoleForReadResponseTypeDef

```python
# AssumeFleetRoleForReadResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssumeFleetRoleForReadResponseTypeDef


def get_value() -> AssumeFleetRoleForReadResponseTypeDef:
    return {
        "credentials": ...,
    }


# AssumeFleetRoleForReadResponseTypeDef definition

class AssumeFleetRoleForReadResponseTypeDef(TypedDict):
    credentials: AwsCredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssumeFleetRoleForWorkerResponseTypeDef

```python
# AssumeFleetRoleForWorkerResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssumeFleetRoleForWorkerResponseTypeDef


def get_value() -> AssumeFleetRoleForWorkerResponseTypeDef:
    return {
        "credentials": ...,
    }


# AssumeFleetRoleForWorkerResponseTypeDef definition

class AssumeFleetRoleForWorkerResponseTypeDef(TypedDict):
    credentials: AwsCredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssumeQueueRoleForReadResponseTypeDef

```python
# AssumeQueueRoleForReadResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssumeQueueRoleForReadResponseTypeDef


def get_value() -> AssumeQueueRoleForReadResponseTypeDef:
    return {
        "credentials": ...,
    }


# AssumeQueueRoleForReadResponseTypeDef definition

class AssumeQueueRoleForReadResponseTypeDef(TypedDict):
    credentials: AwsCredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssumeQueueRoleForUserResponseTypeDef

```python
# AssumeQueueRoleForUserResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssumeQueueRoleForUserResponseTypeDef


def get_value() -> AssumeQueueRoleForUserResponseTypeDef:
    return {
        "credentials": ...,
    }


# AssumeQueueRoleForUserResponseTypeDef definition

class AssumeQueueRoleForUserResponseTypeDef(TypedDict):
    credentials: AwsCredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssumeQueueRoleForWorkerResponseTypeDef

```python
# AssumeQueueRoleForWorkerResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssumeQueueRoleForWorkerResponseTypeDef


def get_value() -> AssumeQueueRoleForWorkerResponseTypeDef:
    return {
        "credentials": ...,
    }


# AssumeQueueRoleForWorkerResponseTypeDef definition

class AssumeQueueRoleForWorkerResponseTypeDef(TypedDict):
    credentials: AwsCredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyJobTemplateResponseTypeDef

```python
# CopyJobTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CopyJobTemplateResponseTypeDef


def get_value() -> CopyJobTemplateResponseTypeDef:
    return {
        "templateType": ...,
    }


# CopyJobTemplateResponseTypeDef definition

class CopyJobTemplateResponseTypeDef(TypedDict):
    templateType: JobTemplateTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobTemplateTypeType](./literals.md#jobtemplatetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBudgetResponseTypeDef

```python
# CreateBudgetResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateBudgetResponseTypeDef


def get_value() -> CreateBudgetResponseTypeDef:
    return {
        "budgetId": ...,
    }


# CreateBudgetResponseTypeDef definition

class CreateBudgetResponseTypeDef(TypedDict):
    budgetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFarmResponseTypeDef

```python
# CreateFarmResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateFarmResponseTypeDef


def get_value() -> CreateFarmResponseTypeDef:
    return {
        "farmId": ...,
    }


# CreateFarmResponseTypeDef definition

class CreateFarmResponseTypeDef(TypedDict):
    farmId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetResponseTypeDef

```python
# CreateFleetResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateFleetResponseTypeDef


def get_value() -> CreateFleetResponseTypeDef:
    return {
        "fleetId": ...,
    }


# CreateFleetResponseTypeDef definition

class CreateFleetResponseTypeDef(TypedDict):
    fleetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobResponseTypeDef

```python
# CreateJobResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateJobResponseTypeDef


def get_value() -> CreateJobResponseTypeDef:
    return {
        "jobId": ...,
    }


# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLicenseEndpointResponseTypeDef

```python
# CreateLicenseEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateLicenseEndpointResponseTypeDef


def get_value() -> CreateLicenseEndpointResponseTypeDef:
    return {
        "licenseEndpointId": ...,
    }


# CreateLicenseEndpointResponseTypeDef definition

class CreateLicenseEndpointResponseTypeDef(TypedDict):
    licenseEndpointId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLimitResponseTypeDef

```python
# CreateLimitResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateLimitResponseTypeDef


def get_value() -> CreateLimitResponseTypeDef:
    return {
        "limitId": ...,
    }


# CreateLimitResponseTypeDef definition

class CreateLimitResponseTypeDef(TypedDict):
    limitId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMonitorResponseTypeDef

```python
# CreateMonitorResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateMonitorResponseTypeDef


def get_value() -> CreateMonitorResponseTypeDef:
    return {
        "monitorId": ...,
    }


# CreateMonitorResponseTypeDef definition

class CreateMonitorResponseTypeDef(TypedDict):
    monitorId: str,
    identityCenterApplicationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQueueEnvironmentResponseTypeDef

```python
# CreateQueueEnvironmentResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateQueueEnvironmentResponseTypeDef


def get_value() -> CreateQueueEnvironmentResponseTypeDef:
    return {
        "queueEnvironmentId": ...,
    }


# CreateQueueEnvironmentResponseTypeDef definition

class CreateQueueEnvironmentResponseTypeDef(TypedDict):
    queueEnvironmentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQueueResponseTypeDef

```python
# CreateQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateQueueResponseTypeDef


def get_value() -> CreateQueueResponseTypeDef:
    return {
        "queueId": ...,
    }


# CreateQueueResponseTypeDef definition

class CreateQueueResponseTypeDef(TypedDict):
    queueId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStorageProfileResponseTypeDef

```python
# CreateStorageProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateStorageProfileResponseTypeDef


def get_value() -> CreateStorageProfileResponseTypeDef:
    return {
        "storageProfileId": ...,
    }


# CreateStorageProfileResponseTypeDef definition

class CreateStorageProfileResponseTypeDef(TypedDict):
    storageProfileId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkerResponseTypeDef

```python
# CreateWorkerResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateWorkerResponseTypeDef


def get_value() -> CreateWorkerResponseTypeDef:
    return {
        "workerId": ...,
    }


# CreateWorkerResponseTypeDef definition

class CreateWorkerResponseTypeDef(TypedDict):
    workerId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFarmResponseTypeDef

```python
# GetFarmResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetFarmResponseTypeDef


def get_value() -> GetFarmResponseTypeDef:
    return {
        "farmId": ...,
    }


# GetFarmResponseTypeDef definition

class GetFarmResponseTypeDef(TypedDict):
    farmId: str,
    displayName: str,
    description: str,
    kmsKeyArn: str,
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLicenseEndpointResponseTypeDef

```python
# GetLicenseEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetLicenseEndpointResponseTypeDef


def get_value() -> GetLicenseEndpointResponseTypeDef:
    return {
        "licenseEndpointId": ...,
    }


# GetLicenseEndpointResponseTypeDef definition

class GetLicenseEndpointResponseTypeDef(TypedDict):
    licenseEndpointId: str,
    status: LicenseEndpointStatusType,  # (1)
    statusMessage: str,
    vpcId: str,
    dnsName: str,
    subnetIds: List[str],
    securityGroupIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LicenseEndpointStatusType](./literals.md#licenseendpointstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLimitResponseTypeDef

```python
# GetLimitResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetLimitResponseTypeDef


def get_value() -> GetLimitResponseTypeDef:
    return {
        "displayName": ...,
    }


# GetLimitResponseTypeDef definition

class GetLimitResponseTypeDef(TypedDict):
    displayName: str,
    amountRequirementName: str,
    maxCount: int,
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    farmId: str,
    limitId: str,
    currentCount: int,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMonitorResponseTypeDef

```python
# GetMonitorResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetMonitorResponseTypeDef


def get_value() -> GetMonitorResponseTypeDef:
    return {
        "monitorId": ...,
    }


# GetMonitorResponseTypeDef definition

class GetMonitorResponseTypeDef(TypedDict):
    monitorId: str,
    displayName: str,
    subdomain: str,
    url: str,
    roleArn: str,
    identityCenterInstanceArn: str,
    identityCenterApplicationArn: str,
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueueEnvironmentResponseTypeDef

```python
# GetQueueEnvironmentResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueEnvironmentResponseTypeDef


def get_value() -> GetQueueEnvironmentResponseTypeDef:
    return {
        "queueEnvironmentId": ...,
    }


# GetQueueEnvironmentResponseTypeDef definition

class GetQueueEnvironmentResponseTypeDef(TypedDict):
    queueEnvironmentId: str,
    name: str,
    priority: int,
    templateType: EnvironmentTemplateTypeType,  # (1)
    template: str,
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EnvironmentTemplateTypeType](./literals.md#environmenttemplatetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueueFleetAssociationResponseTypeDef

```python
# GetQueueFleetAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueFleetAssociationResponseTypeDef


def get_value() -> GetQueueFleetAssociationResponseTypeDef:
    return {
        "queueId": ...,
    }


# GetQueueFleetAssociationResponseTypeDef definition

class GetQueueFleetAssociationResponseTypeDef(TypedDict):
    queueId: str,
    fleetId: str,
    status: QueueFleetAssociationStatusType,  # (1)
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: QueueFleetAssociationStatusType](./literals.md#queuefleetassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueueLimitAssociationResponseTypeDef

```python
# GetQueueLimitAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueLimitAssociationResponseTypeDef


def get_value() -> GetQueueLimitAssociationResponseTypeDef:
    return {
        "createdAt": ...,
    }


# GetQueueLimitAssociationResponseTypeDef definition

class GetQueueLimitAssociationResponseTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    queueId: str,
    limitId: str,
    status: QueueLimitAssociationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: QueueLimitAssociationStatusType](./literals.md#queuelimitassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTaskResponseTypeDef

```python
# GetTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetTaskResponseTypeDef


def get_value() -> GetTaskResponseTypeDef:
    return {
        "taskId": ...,
    }


# GetTaskResponseTypeDef definition

class GetTaskResponseTypeDef(TypedDict):
    taskId: str,
    createdAt: datetime,
    createdBy: str,
    runStatus: TaskRunStatusType,  # (1)
    targetRunStatus: TaskTargetRunStatusType,  # (2)
    failureRetryCount: int,
    parameters: Dict[str, TaskParameterValueTypeDef],  # (3)
    startedAt: datetime,
    endedAt: datetime,
    updatedAt: datetime,
    updatedBy: str,
    latestSessionActionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
2. See [:material-code-brackets: TaskTargetRunStatusType](./literals.md#tasktargetrunstatustype) 
3. See [:material-code-braces: TaskParameterValueTypeDef](./type_defs.md#taskparametervaluetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobParameterDefinitionsResponseTypeDef

```python
# ListJobParameterDefinitionsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListJobParameterDefinitionsResponseTypeDef


def get_value() -> ListJobParameterDefinitionsResponseTypeDef:
    return {
        "jobParameterDefinitions": ...,
    }


# ListJobParameterDefinitionsResponseTypeDef definition

class ListJobParameterDefinitionsResponseTypeDef(TypedDict):
    jobParameterDefinitions: List[Dict[str, Any]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListTagsForResourceResponseTypeDef


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
## StartSessionsStatisticsAggregationResponseTypeDef

```python
# StartSessionsStatisticsAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StartSessionsStatisticsAggregationResponseTypeDef


def get_value() -> StartSessionsStatisticsAggregationResponseTypeDef:
    return {
        "aggregationId": ...,
    }


# StartSessionsStatisticsAggregationResponseTypeDef definition

class StartSessionsStatisticsAggregationResponseTypeDef(TypedDict):
    aggregationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkerResponseTypeDef

```python
# UpdateWorkerResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateWorkerResponseTypeDef


def get_value() -> UpdateWorkerResponseTypeDef:
    return {
        "log": ...,
    }


# UpdateWorkerResponseTypeDef definition

class UpdateWorkerResponseTypeDef(TypedDict):
    log: LogConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachmentsOutputTypeDef

```python
# AttachmentsOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AttachmentsOutputTypeDef


def get_value() -> AttachmentsOutputTypeDef:
    return {
        "manifests": ...,
    }


# AttachmentsOutputTypeDef definition

class AttachmentsOutputTypeDef(TypedDict):
    manifests: List[ManifestPropertiesOutputTypeDef],  # (1)
    fileSystem: NotRequired[JobAttachmentsFileSystemType],  # (2)
```

1. See [:material-code-braces: ManifestPropertiesOutputTypeDef](./type_defs.md#manifestpropertiesoutputtypedef) 
2. See [:material-code-brackets: JobAttachmentsFileSystemType](./literals.md#jobattachmentsfilesystemtype) 
## AttachmentsTypeDef

```python
# AttachmentsTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AttachmentsTypeDef


def get_value() -> AttachmentsTypeDef:
    return {
        "manifests": ...,
    }


# AttachmentsTypeDef definition

class AttachmentsTypeDef(TypedDict):
    manifests: Sequence[ManifestPropertiesTypeDef],  # (1)
    fileSystem: NotRequired[JobAttachmentsFileSystemType],  # (2)
```

1. See [:material-code-braces: ManifestPropertiesTypeDef](./type_defs.md#manifestpropertiestypedef) 
2. See [:material-code-brackets: JobAttachmentsFileSystemType](./literals.md#jobattachmentsfilesystemtype) 
## BudgetScheduleOutputTypeDef

```python
# BudgetScheduleOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import BudgetScheduleOutputTypeDef


def get_value() -> BudgetScheduleOutputTypeDef:
    return {
        "fixed": ...,
    }


# BudgetScheduleOutputTypeDef definition

class BudgetScheduleOutputTypeDef(TypedDict):
    fixed: NotRequired[FixedBudgetScheduleOutputTypeDef],  # (1)
```

1. See [:material-code-braces: FixedBudgetScheduleOutputTypeDef](./type_defs.md#fixedbudgetscheduleoutputtypedef) 
## BudgetSummaryTypeDef

```python
# BudgetSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import BudgetSummaryTypeDef


def get_value() -> BudgetSummaryTypeDef:
    return {
        "budgetId": ...,
    }


# BudgetSummaryTypeDef definition

class BudgetSummaryTypeDef(TypedDict):
    budgetId: str,
    usageTrackingResource: UsageTrackingResourceTypeDef,  # (1)
    status: BudgetStatusType,  # (2)
    displayName: str,
    approximateDollarLimit: float,
    usages: ConsumedUsagesTypeDef,  # (3)
    createdBy: str,
    createdAt: datetime,
    description: NotRequired[str],
    updatedBy: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: UsageTrackingResourceTypeDef](./type_defs.md#usagetrackingresourcetypedef) 
2. See [:material-code-brackets: BudgetStatusType](./literals.md#budgetstatustype) 
3. See [:material-code-braces: ConsumedUsagesTypeDef](./type_defs.md#consumedusagestypedef) 
## CopyJobTemplateRequestTypeDef

```python
# CopyJobTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CopyJobTemplateRequestTypeDef


def get_value() -> CopyJobTemplateRequestTypeDef:
    return {
        "farmId": ...,
    }


# CopyJobTemplateRequestTypeDef definition

class CopyJobTemplateRequestTypeDef(TypedDict):
    farmId: str,
    jobId: str,
    queueId: str,
    targetS3Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## JobSearchSummaryTypeDef

```python
# JobSearchSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobSearchSummaryTypeDef


def get_value() -> JobSearchSummaryTypeDef:
    return {
        "jobId": ...,
    }


# JobSearchSummaryTypeDef definition

class JobSearchSummaryTypeDef(TypedDict):
    jobId: NotRequired[str],
    queueId: NotRequired[str],
    name: NotRequired[str],
    lifecycleStatus: NotRequired[JobLifecycleStatusType],  # (1)
    lifecycleStatusMessage: NotRequired[str],
    taskRunStatus: NotRequired[TaskRunStatusType],  # (2)
    targetTaskRunStatus: NotRequired[JobTargetTaskRunStatusType],  # (3)
    taskRunStatusCounts: NotRequired[Dict[TaskRunStatusType, int]],  # (4)
    priority: NotRequired[int],
    maxFailedTasksCount: NotRequired[int],
    maxRetriesPerTask: NotRequired[int],
    createdBy: NotRequired[str],
    createdAt: NotRequired[datetime],
    endedAt: NotRequired[datetime],
    startedAt: NotRequired[datetime],
    jobParameters: NotRequired[Dict[str, JobParameterTypeDef]],  # (5)
    maxWorkerCount: NotRequired[int],
    sourceJobId: NotRequired[str],
```

1. See [:material-code-brackets: JobLifecycleStatusType](./literals.md#joblifecyclestatustype) 
2. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
3. See [:material-code-brackets: JobTargetTaskRunStatusType](./literals.md#jobtargettaskrunstatustype) 
4. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
5. See [:material-code-braces: JobParameterTypeDef](./type_defs.md#jobparametertypedef) 
## CreateStorageProfileRequestTypeDef

```python
# CreateStorageProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateStorageProfileRequestTypeDef


def get_value() -> CreateStorageProfileRequestTypeDef:
    return {
        "farmId": ...,
    }


# CreateStorageProfileRequestTypeDef definition

class CreateStorageProfileRequestTypeDef(TypedDict):
    farmId: str,
    displayName: str,
    osFamily: StorageProfileOperatingSystemFamilyType,  # (1)
    clientToken: NotRequired[str],
    fileSystemLocations: NotRequired[Sequence[FileSystemLocationTypeDef]],  # (2)
```

1. See [:material-code-brackets: StorageProfileOperatingSystemFamilyType](./literals.md#storageprofileoperatingsystemfamilytype) 
2. See [:material-code-braces: FileSystemLocationTypeDef](./type_defs.md#filesystemlocationtypedef) 
## GetStorageProfileForQueueResponseTypeDef

```python
# GetStorageProfileForQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetStorageProfileForQueueResponseTypeDef


def get_value() -> GetStorageProfileForQueueResponseTypeDef:
    return {
        "storageProfileId": ...,
    }


# GetStorageProfileForQueueResponseTypeDef definition

class GetStorageProfileForQueueResponseTypeDef(TypedDict):
    storageProfileId: str,
    displayName: str,
    osFamily: StorageProfileOperatingSystemFamilyType,  # (1)
    fileSystemLocations: List[FileSystemLocationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: StorageProfileOperatingSystemFamilyType](./literals.md#storageprofileoperatingsystemfamilytype) 
2. See [:material-code-braces: FileSystemLocationTypeDef](./type_defs.md#filesystemlocationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStorageProfileResponseTypeDef

```python
# GetStorageProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetStorageProfileResponseTypeDef


def get_value() -> GetStorageProfileResponseTypeDef:
    return {
        "storageProfileId": ...,
    }


# GetStorageProfileResponseTypeDef definition

class GetStorageProfileResponseTypeDef(TypedDict):
    storageProfileId: str,
    displayName: str,
    osFamily: StorageProfileOperatingSystemFamilyType,  # (1)
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    fileSystemLocations: List[FileSystemLocationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: StorageProfileOperatingSystemFamilyType](./literals.md#storageprofileoperatingsystemfamilytype) 
2. See [:material-code-braces: FileSystemLocationTypeDef](./type_defs.md#filesystemlocationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStorageProfileRequestTypeDef

```python
# UpdateStorageProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateStorageProfileRequestTypeDef


def get_value() -> UpdateStorageProfileRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateStorageProfileRequestTypeDef definition

class UpdateStorageProfileRequestTypeDef(TypedDict):
    farmId: str,
    storageProfileId: str,
    clientToken: NotRequired[str],
    displayName: NotRequired[str],
    osFamily: NotRequired[StorageProfileOperatingSystemFamilyType],  # (1)
    fileSystemLocationsToAdd: NotRequired[Sequence[FileSystemLocationTypeDef]],  # (2)
    fileSystemLocationsToRemove: NotRequired[Sequence[FileSystemLocationTypeDef]],  # (2)
```

1. See [:material-code-brackets: StorageProfileOperatingSystemFamilyType](./literals.md#storageprofileoperatingsystemfamilytype) 
2. See [:material-code-braces: FileSystemLocationTypeDef](./type_defs.md#filesystemlocationtypedef) 
3. See [:material-code-braces: FileSystemLocationTypeDef](./type_defs.md#filesystemlocationtypedef) 
## FleetCapabilitiesTypeDef

```python
# FleetCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FleetCapabilitiesTypeDef


def get_value() -> FleetCapabilitiesTypeDef:
    return {
        "amounts": ...,
    }


# FleetCapabilitiesTypeDef definition

class FleetCapabilitiesTypeDef(TypedDict):
    amounts: NotRequired[List[FleetAmountCapabilityTypeDef]],  # (1)
    attributes: NotRequired[List[FleetAttributeCapabilityOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: FleetAmountCapabilityTypeDef](./type_defs.md#fleetamountcapabilitytypedef) 
2. See [:material-code-braces: FleetAttributeCapabilityOutputTypeDef](./type_defs.md#fleetattributecapabilityoutputtypedef) 
## CustomerManagedWorkerCapabilitiesOutputTypeDef

```python
# CustomerManagedWorkerCapabilitiesOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CustomerManagedWorkerCapabilitiesOutputTypeDef


def get_value() -> CustomerManagedWorkerCapabilitiesOutputTypeDef:
    return {
        "vCpuCount": ...,
    }


# CustomerManagedWorkerCapabilitiesOutputTypeDef definition

class CustomerManagedWorkerCapabilitiesOutputTypeDef(TypedDict):
    vCpuCount: VCpuCountRangeTypeDef,  # (1)
    memoryMiB: MemoryMiBRangeTypeDef,  # (2)
    osFamily: CustomerManagedFleetOperatingSystemFamilyType,  # (6)
    cpuArchitectureType: CpuArchitectureTypeType,  # (7)
    acceleratorTypes: NotRequired[List[AcceleratorTypeType]],  # (3)
    acceleratorCount: NotRequired[AcceleratorCountRangeTypeDef],  # (4)
    acceleratorTotalMemoryMiB: NotRequired[AcceleratorTotalMemoryMiBRangeTypeDef],  # (5)
    customAmounts: NotRequired[List[FleetAmountCapabilityTypeDef]],  # (8)
    customAttributes: NotRequired[List[FleetAttributeCapabilityOutputTypeDef]],  # (9)
```

1. See [:material-code-braces: VCpuCountRangeTypeDef](./type_defs.md#vcpucountrangetypedef) 
2. See [:material-code-braces: MemoryMiBRangeTypeDef](./type_defs.md#memorymibrangetypedef) 
3. See [:material-code-brackets: AcceleratorTypeType](./literals.md#acceleratortypetype) 
4. See [:material-code-braces: AcceleratorCountRangeTypeDef](./type_defs.md#acceleratorcountrangetypedef) 
5. See [:material-code-braces: AcceleratorTotalMemoryMiBRangeTypeDef](./type_defs.md#acceleratortotalmemorymibrangetypedef) 
6. See [:material-code-brackets: CustomerManagedFleetOperatingSystemFamilyType](./literals.md#customermanagedfleetoperatingsystemfamilytype) 
7. See [:material-code-brackets: CpuArchitectureTypeType](./literals.md#cpuarchitecturetypetype) 
8. See [:material-code-braces: FleetAmountCapabilityTypeDef](./type_defs.md#fleetamountcapabilitytypedef) 
9. See [:material-code-braces: FleetAttributeCapabilityOutputTypeDef](./type_defs.md#fleetattributecapabilityoutputtypedef) 
## CustomerManagedWorkerCapabilitiesTypeDef

```python
# CustomerManagedWorkerCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CustomerManagedWorkerCapabilitiesTypeDef


def get_value() -> CustomerManagedWorkerCapabilitiesTypeDef:
    return {
        "vCpuCount": ...,
    }


# CustomerManagedWorkerCapabilitiesTypeDef definition

class CustomerManagedWorkerCapabilitiesTypeDef(TypedDict):
    vCpuCount: VCpuCountRangeTypeDef,  # (1)
    memoryMiB: MemoryMiBRangeTypeDef,  # (2)
    osFamily: CustomerManagedFleetOperatingSystemFamilyType,  # (6)
    cpuArchitectureType: CpuArchitectureTypeType,  # (7)
    acceleratorTypes: NotRequired[Sequence[AcceleratorTypeType]],  # (3)
    acceleratorCount: NotRequired[AcceleratorCountRangeTypeDef],  # (4)
    acceleratorTotalMemoryMiB: NotRequired[AcceleratorTotalMemoryMiBRangeTypeDef],  # (5)
    customAmounts: NotRequired[Sequence[FleetAmountCapabilityTypeDef]],  # (8)
    customAttributes: NotRequired[Sequence[FleetAttributeCapabilityTypeDef]],  # (9)
```

1. See [:material-code-braces: VCpuCountRangeTypeDef](./type_defs.md#vcpucountrangetypedef) 
2. See [:material-code-braces: MemoryMiBRangeTypeDef](./type_defs.md#memorymibrangetypedef) 
3. See [:material-code-brackets: AcceleratorTypeType](./literals.md#acceleratortypetype) 
4. See [:material-code-braces: AcceleratorCountRangeTypeDef](./type_defs.md#acceleratorcountrangetypedef) 
5. See [:material-code-braces: AcceleratorTotalMemoryMiBRangeTypeDef](./type_defs.md#acceleratortotalmemorymibrangetypedef) 
6. See [:material-code-brackets: CustomerManagedFleetOperatingSystemFamilyType](./literals.md#customermanagedfleetoperatingsystemfamilytype) 
7. See [:material-code-brackets: CpuArchitectureTypeType](./literals.md#cpuarchitecturetypetype) 
8. See [:material-code-braces: FleetAmountCapabilityTypeDef](./type_defs.md#fleetamountcapabilitytypedef) 
9. See [:material-code-braces: FleetAttributeCapabilityTypeDef](./type_defs.md#fleetattributecapabilitytypedef) 
## DateTimeFilterExpressionTypeDef

```python
# DateTimeFilterExpressionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import DateTimeFilterExpressionTypeDef


def get_value() -> DateTimeFilterExpressionTypeDef:
    return {
        "name": ...,
    }


# DateTimeFilterExpressionTypeDef definition

class DateTimeFilterExpressionTypeDef(TypedDict):
    name: str,
    operator: ComparisonOperatorType,  # (1)
    dateTime: TimestampTypeDef,
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## FixedBudgetScheduleTypeDef

```python
# FixedBudgetScheduleTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FixedBudgetScheduleTypeDef


def get_value() -> FixedBudgetScheduleTypeDef:
    return {
        "startTime": ...,
    }


# FixedBudgetScheduleTypeDef definition

class FixedBudgetScheduleTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
```

## UpdatedSessionActionInfoTypeDef

```python
# UpdatedSessionActionInfoTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdatedSessionActionInfoTypeDef


def get_value() -> UpdatedSessionActionInfoTypeDef:
    return {
        "completedStatus": ...,
    }


# UpdatedSessionActionInfoTypeDef definition

class UpdatedSessionActionInfoTypeDef(TypedDict):
    completedStatus: NotRequired[CompletedStatusType],  # (1)
    processExitCode: NotRequired[int],
    progressMessage: NotRequired[str],
    startedAt: NotRequired[TimestampTypeDef],
    endedAt: NotRequired[TimestampTypeDef],
    updatedAt: NotRequired[TimestampTypeDef],
    progressPercent: NotRequired[float],
```

1. See [:material-code-brackets: CompletedStatusType](./literals.md#completedstatustype) 
## StepSummaryTypeDef

```python
# StepSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StepSummaryTypeDef


def get_value() -> StepSummaryTypeDef:
    return {
        "stepId": ...,
    }


# StepSummaryTypeDef definition

class StepSummaryTypeDef(TypedDict):
    stepId: str,
    name: str,
    lifecycleStatus: StepLifecycleStatusType,  # (1)
    taskRunStatus: TaskRunStatusType,  # (2)
    taskRunStatusCounts: Dict[TaskRunStatusType, int],  # (3)
    createdAt: datetime,
    createdBy: str,
    lifecycleStatusMessage: NotRequired[str],
    targetTaskRunStatus: NotRequired[StepTargetTaskRunStatusType],  # (4)
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
    startedAt: NotRequired[datetime],
    endedAt: NotRequired[datetime],
    dependencyCounts: NotRequired[DependencyCountsTypeDef],  # (5)
```

1. See [:material-code-brackets: StepLifecycleStatusType](./literals.md#steplifecyclestatustype) 
2. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
3. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
4. See [:material-code-brackets: StepTargetTaskRunStatusType](./literals.md#steptargettaskrunstatustype) 
5. See [:material-code-braces: DependencyCountsTypeDef](./type_defs.md#dependencycountstypedef) 
## ListFarmMembersResponseTypeDef

```python
# ListFarmMembersResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFarmMembersResponseTypeDef


def get_value() -> ListFarmMembersResponseTypeDef:
    return {
        "members": ...,
    }


# ListFarmMembersResponseTypeDef definition

class ListFarmMembersResponseTypeDef(TypedDict):
    members: List[FarmMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FarmMemberTypeDef](./type_defs.md#farmmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFarmsResponseTypeDef

```python
# ListFarmsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFarmsResponseTypeDef


def get_value() -> ListFarmsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListFarmsResponseTypeDef definition

class ListFarmsResponseTypeDef(TypedDict):
    farms: List[FarmSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FarmSummaryTypeDef](./type_defs.md#farmsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFleetMembersResponseTypeDef

```python
# ListFleetMembersResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFleetMembersResponseTypeDef


def get_value() -> ListFleetMembersResponseTypeDef:
    return {
        "members": ...,
    }


# ListFleetMembersResponseTypeDef definition

class ListFleetMembersResponseTypeDef(TypedDict):
    members: List[FleetMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetMemberTypeDef](./type_defs.md#fleetmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFleetRequestWaitTypeDef

```python
# GetFleetRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetFleetRequestWaitTypeDef


def get_value() -> GetFleetRequestWaitTypeDef:
    return {
        "farmId": ...,
    }


# GetFleetRequestWaitTypeDef definition

class GetFleetRequestWaitTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetJobRequestWaitTypeDef

```python
# GetJobRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetJobRequestWaitTypeDef


def get_value() -> GetJobRequestWaitTypeDef:
    return {
        "farmId": ...,
    }


# GetJobRequestWaitTypeDef definition

class GetJobRequestWaitTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetLicenseEndpointRequestWaitExtraTypeDef

```python
# GetLicenseEndpointRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetLicenseEndpointRequestWaitExtraTypeDef


def get_value() -> GetLicenseEndpointRequestWaitExtraTypeDef:
    return {
        "licenseEndpointId": ...,
    }


# GetLicenseEndpointRequestWaitExtraTypeDef definition

class GetLicenseEndpointRequestWaitExtraTypeDef(TypedDict):
    licenseEndpointId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetLicenseEndpointRequestWaitTypeDef

```python
# GetLicenseEndpointRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetLicenseEndpointRequestWaitTypeDef


def get_value() -> GetLicenseEndpointRequestWaitTypeDef:
    return {
        "licenseEndpointId": ...,
    }


# GetLicenseEndpointRequestWaitTypeDef definition

class GetLicenseEndpointRequestWaitTypeDef(TypedDict):
    licenseEndpointId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetQueueFleetAssociationRequestWaitTypeDef

```python
# GetQueueFleetAssociationRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueFleetAssociationRequestWaitTypeDef


def get_value() -> GetQueueFleetAssociationRequestWaitTypeDef:
    return {
        "farmId": ...,
    }


# GetQueueFleetAssociationRequestWaitTypeDef definition

class GetQueueFleetAssociationRequestWaitTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    fleetId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetQueueLimitAssociationRequestWaitTypeDef

```python
# GetQueueLimitAssociationRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueLimitAssociationRequestWaitTypeDef


def get_value() -> GetQueueLimitAssociationRequestWaitTypeDef:
    return {
        "farmId": ...,
    }


# GetQueueLimitAssociationRequestWaitTypeDef definition

class GetQueueLimitAssociationRequestWaitTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    limitId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetQueueRequestWaitExtraTypeDef

```python
# GetQueueRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueRequestWaitExtraTypeDef


def get_value() -> GetQueueRequestWaitExtraTypeDef:
    return {
        "farmId": ...,
    }


# GetQueueRequestWaitExtraTypeDef definition

class GetQueueRequestWaitExtraTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetQueueRequestWaitTypeDef

```python
# GetQueueRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueRequestWaitTypeDef


def get_value() -> GetQueueRequestWaitTypeDef:
    return {
        "farmId": ...,
    }


# GetQueueRequestWaitTypeDef definition

class GetQueueRequestWaitTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetJobEntityErrorTypeDef

```python
# GetJobEntityErrorTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetJobEntityErrorTypeDef


def get_value() -> GetJobEntityErrorTypeDef:
    return {
        "jobDetails": ...,
    }


# GetJobEntityErrorTypeDef definition

class GetJobEntityErrorTypeDef(TypedDict):
    jobDetails: NotRequired[JobDetailsErrorTypeDef],  # (1)
    jobAttachmentDetails: NotRequired[JobAttachmentDetailsErrorTypeDef],  # (2)
    stepDetails: NotRequired[StepDetailsErrorTypeDef],  # (3)
    environmentDetails: NotRequired[EnvironmentDetailsErrorTypeDef],  # (4)
```

1. See [:material-code-braces: JobDetailsErrorTypeDef](./type_defs.md#jobdetailserrortypedef) 
2. See [:material-code-braces: JobAttachmentDetailsErrorTypeDef](./type_defs.md#jobattachmentdetailserrortypedef) 
3. See [:material-code-braces: StepDetailsErrorTypeDef](./type_defs.md#stepdetailserrortypedef) 
4. See [:material-code-braces: EnvironmentDetailsErrorTypeDef](./type_defs.md#environmentdetailserrortypedef) 
## GetSessionsStatisticsAggregationRequestPaginateTypeDef

```python
# GetSessionsStatisticsAggregationRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetSessionsStatisticsAggregationRequestPaginateTypeDef


def get_value() -> GetSessionsStatisticsAggregationRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# GetSessionsStatisticsAggregationRequestPaginateTypeDef definition

class GetSessionsStatisticsAggregationRequestPaginateTypeDef(TypedDict):
    farmId: str,
    aggregationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAvailableMeteredProductsRequestPaginateTypeDef

```python
# ListAvailableMeteredProductsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListAvailableMeteredProductsRequestPaginateTypeDef


def get_value() -> ListAvailableMeteredProductsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListAvailableMeteredProductsRequestPaginateTypeDef definition

class ListAvailableMeteredProductsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBudgetsRequestPaginateTypeDef

```python
# ListBudgetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListBudgetsRequestPaginateTypeDef


def get_value() -> ListBudgetsRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListBudgetsRequestPaginateTypeDef definition

class ListBudgetsRequestPaginateTypeDef(TypedDict):
    farmId: str,
    status: NotRequired[BudgetStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: BudgetStatusType](./literals.md#budgetstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFarmMembersRequestPaginateTypeDef

```python
# ListFarmMembersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFarmMembersRequestPaginateTypeDef


def get_value() -> ListFarmMembersRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListFarmMembersRequestPaginateTypeDef definition

class ListFarmMembersRequestPaginateTypeDef(TypedDict):
    farmId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFarmsRequestPaginateTypeDef

```python
# ListFarmsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFarmsRequestPaginateTypeDef


def get_value() -> ListFarmsRequestPaginateTypeDef:
    return {
        "principalId": ...,
    }


# ListFarmsRequestPaginateTypeDef definition

class ListFarmsRequestPaginateTypeDef(TypedDict):
    principalId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFleetMembersRequestPaginateTypeDef

```python
# ListFleetMembersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFleetMembersRequestPaginateTypeDef


def get_value() -> ListFleetMembersRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListFleetMembersRequestPaginateTypeDef definition

class ListFleetMembersRequestPaginateTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFleetsRequestPaginateTypeDef

```python
# ListFleetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFleetsRequestPaginateTypeDef


def get_value() -> ListFleetsRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListFleetsRequestPaginateTypeDef definition

class ListFleetsRequestPaginateTypeDef(TypedDict):
    farmId: str,
    principalId: NotRequired[str],
    displayName: NotRequired[str],
    status: NotRequired[FleetStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FleetStatusType](./literals.md#fleetstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobMembersRequestPaginateTypeDef

```python
# ListJobMembersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListJobMembersRequestPaginateTypeDef


def get_value() -> ListJobMembersRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListJobMembersRequestPaginateTypeDef definition

class ListJobMembersRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobParameterDefinitionsRequestPaginateTypeDef

```python
# ListJobParameterDefinitionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListJobParameterDefinitionsRequestPaginateTypeDef


def get_value() -> ListJobParameterDefinitionsRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListJobParameterDefinitionsRequestPaginateTypeDef definition

class ListJobParameterDefinitionsRequestPaginateTypeDef(TypedDict):
    farmId: str,
    jobId: str,
    queueId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestPaginateTypeDef

```python
# ListJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListJobsRequestPaginateTypeDef


def get_value() -> ListJobsRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListJobsRequestPaginateTypeDef definition

class ListJobsRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    principalId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLicenseEndpointsRequestPaginateTypeDef

```python
# ListLicenseEndpointsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListLicenseEndpointsRequestPaginateTypeDef


def get_value() -> ListLicenseEndpointsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListLicenseEndpointsRequestPaginateTypeDef definition

class ListLicenseEndpointsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLimitsRequestPaginateTypeDef

```python
# ListLimitsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListLimitsRequestPaginateTypeDef


def get_value() -> ListLimitsRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListLimitsRequestPaginateTypeDef definition

class ListLimitsRequestPaginateTypeDef(TypedDict):
    farmId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMeteredProductsRequestPaginateTypeDef

```python
# ListMeteredProductsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListMeteredProductsRequestPaginateTypeDef


def get_value() -> ListMeteredProductsRequestPaginateTypeDef:
    return {
        "licenseEndpointId": ...,
    }


# ListMeteredProductsRequestPaginateTypeDef definition

class ListMeteredProductsRequestPaginateTypeDef(TypedDict):
    licenseEndpointId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMonitorsRequestPaginateTypeDef

```python
# ListMonitorsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListMonitorsRequestPaginateTypeDef


def get_value() -> ListMonitorsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListMonitorsRequestPaginateTypeDef definition

class ListMonitorsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueueEnvironmentsRequestPaginateTypeDef

```python
# ListQueueEnvironmentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueEnvironmentsRequestPaginateTypeDef


def get_value() -> ListQueueEnvironmentsRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListQueueEnvironmentsRequestPaginateTypeDef definition

class ListQueueEnvironmentsRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueueFleetAssociationsRequestPaginateTypeDef

```python
# ListQueueFleetAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueFleetAssociationsRequestPaginateTypeDef


def get_value() -> ListQueueFleetAssociationsRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListQueueFleetAssociationsRequestPaginateTypeDef definition

class ListQueueFleetAssociationsRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: NotRequired[str],
    fleetId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueueLimitAssociationsRequestPaginateTypeDef

```python
# ListQueueLimitAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueLimitAssociationsRequestPaginateTypeDef


def get_value() -> ListQueueLimitAssociationsRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListQueueLimitAssociationsRequestPaginateTypeDef definition

class ListQueueLimitAssociationsRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: NotRequired[str],
    limitId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueueMembersRequestPaginateTypeDef

```python
# ListQueueMembersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueMembersRequestPaginateTypeDef


def get_value() -> ListQueueMembersRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListQueueMembersRequestPaginateTypeDef definition

class ListQueueMembersRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueuesRequestPaginateTypeDef

```python
# ListQueuesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueuesRequestPaginateTypeDef


def get_value() -> ListQueuesRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListQueuesRequestPaginateTypeDef definition

class ListQueuesRequestPaginateTypeDef(TypedDict):
    farmId: str,
    principalId: NotRequired[str],
    status: NotRequired[QueueStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSessionActionsRequestPaginateTypeDef

```python
# ListSessionActionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListSessionActionsRequestPaginateTypeDef


def get_value() -> ListSessionActionsRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListSessionActionsRequestPaginateTypeDef definition

class ListSessionActionsRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    sessionId: NotRequired[str],
    taskId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSessionsForWorkerRequestPaginateTypeDef

```python
# ListSessionsForWorkerRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListSessionsForWorkerRequestPaginateTypeDef


def get_value() -> ListSessionsForWorkerRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListSessionsForWorkerRequestPaginateTypeDef definition

class ListSessionsForWorkerRequestPaginateTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSessionsRequestPaginateTypeDef

```python
# ListSessionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListSessionsRequestPaginateTypeDef


def get_value() -> ListSessionsRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListSessionsRequestPaginateTypeDef definition

class ListSessionsRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStepConsumersRequestPaginateTypeDef

```python
# ListStepConsumersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStepConsumersRequestPaginateTypeDef


def get_value() -> ListStepConsumersRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListStepConsumersRequestPaginateTypeDef definition

class ListStepConsumersRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStepDependenciesRequestPaginateTypeDef

```python
# ListStepDependenciesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStepDependenciesRequestPaginateTypeDef


def get_value() -> ListStepDependenciesRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListStepDependenciesRequestPaginateTypeDef definition

class ListStepDependenciesRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStepsRequestPaginateTypeDef

```python
# ListStepsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStepsRequestPaginateTypeDef


def get_value() -> ListStepsRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListStepsRequestPaginateTypeDef definition

class ListStepsRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStorageProfilesForQueueRequestPaginateTypeDef

```python
# ListStorageProfilesForQueueRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStorageProfilesForQueueRequestPaginateTypeDef


def get_value() -> ListStorageProfilesForQueueRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListStorageProfilesForQueueRequestPaginateTypeDef definition

class ListStorageProfilesForQueueRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStorageProfilesRequestPaginateTypeDef

```python
# ListStorageProfilesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStorageProfilesRequestPaginateTypeDef


def get_value() -> ListStorageProfilesRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListStorageProfilesRequestPaginateTypeDef definition

class ListStorageProfilesRequestPaginateTypeDef(TypedDict):
    farmId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTasksRequestPaginateTypeDef

```python
# ListTasksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListTasksRequestPaginateTypeDef


def get_value() -> ListTasksRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListTasksRequestPaginateTypeDef definition

class ListTasksRequestPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkersRequestPaginateTypeDef

```python
# ListWorkersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListWorkersRequestPaginateTypeDef


def get_value() -> ListWorkersRequestPaginateTypeDef:
    return {
        "farmId": ...,
    }


# ListWorkersRequestPaginateTypeDef definition

class ListWorkersRequestPaginateTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## HostPropertiesResponseTypeDef

```python
# HostPropertiesResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import HostPropertiesResponseTypeDef


def get_value() -> HostPropertiesResponseTypeDef:
    return {
        "ipAddresses": ...,
    }


# HostPropertiesResponseTypeDef definition

class HostPropertiesResponseTypeDef(TypedDict):
    ipAddresses: NotRequired[IpAddressesOutputTypeDef],  # (1)
    hostName: NotRequired[str],
    ec2InstanceArn: NotRequired[str],
    ec2InstanceType: NotRequired[str],
```

1. See [:material-code-braces: IpAddressesOutputTypeDef](./type_defs.md#ipaddressesoutputtypedef) 
## JobEntityIdentifiersUnionTypeDef

```python
# JobEntityIdentifiersUnionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobEntityIdentifiersUnionTypeDef


def get_value() -> JobEntityIdentifiersUnionTypeDef:
    return {
        "jobDetails": ...,
    }


# JobEntityIdentifiersUnionTypeDef definition

class JobEntityIdentifiersUnionTypeDef(TypedDict):
    jobDetails: NotRequired[JobDetailsIdentifiersTypeDef],  # (1)
    jobAttachmentDetails: NotRequired[JobAttachmentDetailsIdentifiersTypeDef],  # (2)
    stepDetails: NotRequired[StepDetailsIdentifiersTypeDef],  # (3)
    environmentDetails: NotRequired[EnvironmentDetailsIdentifiersTypeDef],  # (4)
```

1. See [:material-code-braces: JobDetailsIdentifiersTypeDef](./type_defs.md#jobdetailsidentifierstypedef) 
2. See [:material-code-braces: JobAttachmentDetailsIdentifiersTypeDef](./type_defs.md#jobattachmentdetailsidentifierstypedef) 
3. See [:material-code-braces: StepDetailsIdentifiersTypeDef](./type_defs.md#stepdetailsidentifierstypedef) 
4. See [:material-code-braces: EnvironmentDetailsIdentifiersTypeDef](./type_defs.md#environmentdetailsidentifierstypedef) 
## ListJobMembersResponseTypeDef

```python
# ListJobMembersResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListJobMembersResponseTypeDef


def get_value() -> ListJobMembersResponseTypeDef:
    return {
        "members": ...,
    }


# ListJobMembersResponseTypeDef definition

class ListJobMembersResponseTypeDef(TypedDict):
    members: List[JobMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobMemberTypeDef](./type_defs.md#jobmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobRunAsUserTypeDef

```python
# JobRunAsUserTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobRunAsUserTypeDef


def get_value() -> JobRunAsUserTypeDef:
    return {
        "posix": ...,
    }


# JobRunAsUserTypeDef definition

class JobRunAsUserTypeDef(TypedDict):
    runAs: RunAsType,  # (3)
    posix: NotRequired[PosixUserTypeDef],  # (1)
    windows: NotRequired[WindowsUserTypeDef],  # (2)
```

1. See [:material-code-braces: PosixUserTypeDef](./type_defs.md#posixusertypedef) 
2. See [:material-code-braces: WindowsUserTypeDef](./type_defs.md#windowsusertypedef) 
3. See [:material-code-brackets: RunAsType](./literals.md#runastype) 
## ListJobsResponseTypeDef

```python
# ListJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListJobsResponseTypeDef


def get_value() -> ListJobsResponseTypeDef:
    return {
        "jobs": ...,
    }


# ListJobsResponseTypeDef definition

class ListJobsResponseTypeDef(TypedDict):
    jobs: List[JobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLicenseEndpointsResponseTypeDef

```python
# ListLicenseEndpointsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListLicenseEndpointsResponseTypeDef


def get_value() -> ListLicenseEndpointsResponseTypeDef:
    return {
        "licenseEndpoints": ...,
    }


# ListLicenseEndpointsResponseTypeDef definition

class ListLicenseEndpointsResponseTypeDef(TypedDict):
    licenseEndpoints: List[LicenseEndpointSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseEndpointSummaryTypeDef](./type_defs.md#licenseendpointsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLimitsResponseTypeDef

```python
# ListLimitsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListLimitsResponseTypeDef


def get_value() -> ListLimitsResponseTypeDef:
    return {
        "limits": ...,
    }


# ListLimitsResponseTypeDef definition

class ListLimitsResponseTypeDef(TypedDict):
    limits: List[LimitSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LimitSummaryTypeDef](./type_defs.md#limitsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAvailableMeteredProductsResponseTypeDef

```python
# ListAvailableMeteredProductsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListAvailableMeteredProductsResponseTypeDef


def get_value() -> ListAvailableMeteredProductsResponseTypeDef:
    return {
        "meteredProducts": ...,
    }


# ListAvailableMeteredProductsResponseTypeDef definition

class ListAvailableMeteredProductsResponseTypeDef(TypedDict):
    meteredProducts: List[MeteredProductSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MeteredProductSummaryTypeDef](./type_defs.md#meteredproductsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMeteredProductsResponseTypeDef

```python
# ListMeteredProductsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListMeteredProductsResponseTypeDef


def get_value() -> ListMeteredProductsResponseTypeDef:
    return {
        "meteredProducts": ...,
    }


# ListMeteredProductsResponseTypeDef definition

class ListMeteredProductsResponseTypeDef(TypedDict):
    meteredProducts: List[MeteredProductSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MeteredProductSummaryTypeDef](./type_defs.md#meteredproductsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMonitorsResponseTypeDef

```python
# ListMonitorsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListMonitorsResponseTypeDef


def get_value() -> ListMonitorsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListMonitorsResponseTypeDef definition

class ListMonitorsResponseTypeDef(TypedDict):
    monitors: List[MonitorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MonitorSummaryTypeDef](./type_defs.md#monitorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueueEnvironmentsResponseTypeDef

```python
# ListQueueEnvironmentsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueEnvironmentsResponseTypeDef


def get_value() -> ListQueueEnvironmentsResponseTypeDef:
    return {
        "environments": ...,
    }


# ListQueueEnvironmentsResponseTypeDef definition

class ListQueueEnvironmentsResponseTypeDef(TypedDict):
    environments: List[QueueEnvironmentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QueueEnvironmentSummaryTypeDef](./type_defs.md#queueenvironmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueueFleetAssociationsResponseTypeDef

```python
# ListQueueFleetAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueFleetAssociationsResponseTypeDef


def get_value() -> ListQueueFleetAssociationsResponseTypeDef:
    return {
        "queueFleetAssociations": ...,
    }


# ListQueueFleetAssociationsResponseTypeDef definition

class ListQueueFleetAssociationsResponseTypeDef(TypedDict):
    queueFleetAssociations: List[QueueFleetAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QueueFleetAssociationSummaryTypeDef](./type_defs.md#queuefleetassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueueLimitAssociationsResponseTypeDef

```python
# ListQueueLimitAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueLimitAssociationsResponseTypeDef


def get_value() -> ListQueueLimitAssociationsResponseTypeDef:
    return {
        "queueLimitAssociations": ...,
    }


# ListQueueLimitAssociationsResponseTypeDef definition

class ListQueueLimitAssociationsResponseTypeDef(TypedDict):
    queueLimitAssociations: List[QueueLimitAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QueueLimitAssociationSummaryTypeDef](./type_defs.md#queuelimitassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueueMembersResponseTypeDef

```python
# ListQueueMembersResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueueMembersResponseTypeDef


def get_value() -> ListQueueMembersResponseTypeDef:
    return {
        "members": ...,
    }


# ListQueueMembersResponseTypeDef definition

class ListQueueMembersResponseTypeDef(TypedDict):
    members: List[QueueMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QueueMemberTypeDef](./type_defs.md#queuemembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueuesResponseTypeDef

```python
# ListQueuesResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListQueuesResponseTypeDef


def get_value() -> ListQueuesResponseTypeDef:
    return {
        "queues": ...,
    }


# ListQueuesResponseTypeDef definition

class ListQueuesResponseTypeDef(TypedDict):
    queues: List[QueueSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QueueSummaryTypeDef](./type_defs.md#queuesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSessionsForWorkerResponseTypeDef

```python
# ListSessionsForWorkerResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListSessionsForWorkerResponseTypeDef


def get_value() -> ListSessionsForWorkerResponseTypeDef:
    return {
        "sessions": ...,
    }


# ListSessionsForWorkerResponseTypeDef definition

class ListSessionsForWorkerResponseTypeDef(TypedDict):
    sessions: List[WorkerSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkerSessionSummaryTypeDef](./type_defs.md#workersessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSessionsResponseTypeDef

```python
# ListSessionsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListSessionsResponseTypeDef


def get_value() -> ListSessionsResponseTypeDef:
    return {
        "sessions": ...,
    }


# ListSessionsResponseTypeDef definition

class ListSessionsResponseTypeDef(TypedDict):
    sessions: List[SessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SessionSummaryTypeDef](./type_defs.md#sessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStepConsumersResponseTypeDef

```python
# ListStepConsumersResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStepConsumersResponseTypeDef


def get_value() -> ListStepConsumersResponseTypeDef:
    return {
        "consumers": ...,
    }


# ListStepConsumersResponseTypeDef definition

class ListStepConsumersResponseTypeDef(TypedDict):
    consumers: List[StepConsumerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StepConsumerTypeDef](./type_defs.md#stepconsumertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStepDependenciesResponseTypeDef

```python
# ListStepDependenciesResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStepDependenciesResponseTypeDef


def get_value() -> ListStepDependenciesResponseTypeDef:
    return {
        "dependencies": ...,
    }


# ListStepDependenciesResponseTypeDef definition

class ListStepDependenciesResponseTypeDef(TypedDict):
    dependencies: List[StepDependencyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StepDependencyTypeDef](./type_defs.md#stepdependencytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStorageProfilesForQueueResponseTypeDef

```python
# ListStorageProfilesForQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStorageProfilesForQueueResponseTypeDef


def get_value() -> ListStorageProfilesForQueueResponseTypeDef:
    return {
        "storageProfiles": ...,
    }


# ListStorageProfilesForQueueResponseTypeDef definition

class ListStorageProfilesForQueueResponseTypeDef(TypedDict):
    storageProfiles: List[StorageProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StorageProfileSummaryTypeDef](./type_defs.md#storageprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStorageProfilesResponseTypeDef

```python
# ListStorageProfilesResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStorageProfilesResponseTypeDef


def get_value() -> ListStorageProfilesResponseTypeDef:
    return {
        "storageProfiles": ...,
    }


# ListStorageProfilesResponseTypeDef definition

class ListStorageProfilesResponseTypeDef(TypedDict):
    storageProfiles: List[StorageProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StorageProfileSummaryTypeDef](./type_defs.md#storageprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ParameterSpaceTypeDef

```python
# ParameterSpaceTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ParameterSpaceTypeDef


def get_value() -> ParameterSpaceTypeDef:
    return {
        "parameters": ...,
    }


# ParameterSpaceTypeDef definition

class ParameterSpaceTypeDef(TypedDict):
    parameters: List[StepParameterTypeDef],  # (1)
    combination: NotRequired[str],
```

1. See [:material-code-braces: StepParameterTypeDef](./type_defs.md#stepparametertypedef) 
## SearchSortExpressionTypeDef

```python
# SearchSortExpressionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchSortExpressionTypeDef


def get_value() -> SearchSortExpressionTypeDef:
    return {
        "userJobsFirst": ...,
    }


# SearchSortExpressionTypeDef definition

class SearchSortExpressionTypeDef(TypedDict):
    userJobsFirst: NotRequired[UserJobsFirstTypeDef],  # (1)
    fieldSort: NotRequired[FieldSortExpressionTypeDef],  # (2)
    parameterSort: NotRequired[ParameterSortExpressionTypeDef],  # (3)
```

1. See [:material-code-braces: UserJobsFirstTypeDef](./type_defs.md#userjobsfirsttypedef) 
2. See [:material-code-braces: FieldSortExpressionTypeDef](./type_defs.md#fieldsortexpressiontypedef) 
3. See [:material-code-braces: ParameterSortExpressionTypeDef](./type_defs.md#parametersortexpressiontypedef) 
## SessionActionDefinitionSummaryTypeDef

```python
# SessionActionDefinitionSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SessionActionDefinitionSummaryTypeDef


def get_value() -> SessionActionDefinitionSummaryTypeDef:
    return {
        "envEnter": ...,
    }


# SessionActionDefinitionSummaryTypeDef definition

class SessionActionDefinitionSummaryTypeDef(TypedDict):
    envEnter: NotRequired[EnvironmentEnterSessionActionDefinitionSummaryTypeDef],  # (1)
    envExit: NotRequired[EnvironmentExitSessionActionDefinitionSummaryTypeDef],  # (2)
    taskRun: NotRequired[TaskRunSessionActionDefinitionSummaryTypeDef],  # (3)
    syncInputJobAttachments: NotRequired[SyncInputJobAttachmentsSessionActionDefinitionSummaryTypeDef],  # (4)
```

1. See [:material-code-braces: EnvironmentEnterSessionActionDefinitionSummaryTypeDef](./type_defs.md#environmententersessionactiondefinitionsummarytypedef) 
2. See [:material-code-braces: EnvironmentExitSessionActionDefinitionSummaryTypeDef](./type_defs.md#environmentexitsessionactiondefinitionsummarytypedef) 
3. See [:material-code-braces: TaskRunSessionActionDefinitionSummaryTypeDef](./type_defs.md#taskrunsessionactiondefinitionsummarytypedef) 
4. See [:material-code-braces: SyncInputJobAttachmentsSessionActionDefinitionSummaryTypeDef](./type_defs.md#syncinputjobattachmentssessionactiondefinitionsummarytypedef) 
## StartSessionsStatisticsAggregationRequestTypeDef

```python
# StartSessionsStatisticsAggregationRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StartSessionsStatisticsAggregationRequestTypeDef


def get_value() -> StartSessionsStatisticsAggregationRequestTypeDef:
    return {
        "farmId": ...,
    }


# StartSessionsStatisticsAggregationRequestTypeDef definition

class StartSessionsStatisticsAggregationRequestTypeDef(TypedDict):
    farmId: str,
    resourceIds: SessionsStatisticsResourcesTypeDef,  # (1)
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    groupBy: Sequence[UsageGroupByFieldType],  # (2)
    statistics: Sequence[UsageStatisticType],  # (3)
    timezone: NotRequired[str],
    period: NotRequired[PeriodType],  # (4)
```

1. See [:material-code-braces: SessionsStatisticsResourcesTypeDef](./type_defs.md#sessionsstatisticsresourcestypedef) 
2. See [:material-code-brackets: UsageGroupByFieldType](./literals.md#usagegroupbyfieldtype) 
3. See [:material-code-brackets: UsageStatisticType](./literals.md#usagestatistictype) 
4. See [:material-code-brackets: PeriodType](./literals.md#periodtype) 
## StatisticsTypeDef

```python
# StatisticsTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StatisticsTypeDef


def get_value() -> StatisticsTypeDef:
    return {
        "queueId": ...,
    }


# StatisticsTypeDef definition

class StatisticsTypeDef(TypedDict):
    count: int,
    costInUsd: StatsTypeDef,  # (2)
    runtimeInSeconds: StatsTypeDef,  # (2)
    queueId: NotRequired[str],
    fleetId: NotRequired[str],
    jobId: NotRequired[str],
    jobName: NotRequired[str],
    userId: NotRequired[str],
    usageType: NotRequired[UsageTypeType],  # (1)
    licenseProduct: NotRequired[str],
    instanceType: NotRequired[str],
    aggregationStartTime: NotRequired[datetime],
    aggregationEndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: UsageTypeType](./literals.md#usagetypetype) 
2. See [:material-code-braces: StatsTypeDef](./type_defs.md#statstypedef) 
3. See [:material-code-braces: StatsTypeDef](./type_defs.md#statstypedef) 
## StepRequiredCapabilitiesTypeDef

```python
# StepRequiredCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StepRequiredCapabilitiesTypeDef


def get_value() -> StepRequiredCapabilitiesTypeDef:
    return {
        "attributes": ...,
    }


# StepRequiredCapabilitiesTypeDef definition

class StepRequiredCapabilitiesTypeDef(TypedDict):
    attributes: List[StepAttributeCapabilityTypeDef],  # (1)
    amounts: List[StepAmountCapabilityTypeDef],  # (2)
```

1. See [:material-code-braces: StepAttributeCapabilityTypeDef](./type_defs.md#stepattributecapabilitytypedef) 
2. See [:material-code-braces: StepAmountCapabilityTypeDef](./type_defs.md#stepamountcapabilitytypedef) 
## WorkerCapabilitiesTypeDef

```python
# WorkerCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import WorkerCapabilitiesTypeDef


def get_value() -> WorkerCapabilitiesTypeDef:
    return {
        "amounts": ...,
    }


# WorkerCapabilitiesTypeDef definition

class WorkerCapabilitiesTypeDef(TypedDict):
    amounts: Sequence[WorkerAmountCapabilityTypeDef],  # (1)
    attributes: Sequence[WorkerAttributeCapabilityTypeDef],  # (2)
```

1. See [:material-code-braces: WorkerAmountCapabilityTypeDef](./type_defs.md#workeramountcapabilitytypedef) 
2. See [:material-code-braces: WorkerAttributeCapabilityTypeDef](./type_defs.md#workerattributecapabilitytypedef) 
## ServiceManagedEc2InstanceCapabilitiesOutputTypeDef

```python
# ServiceManagedEc2InstanceCapabilitiesOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ServiceManagedEc2InstanceCapabilitiesOutputTypeDef


def get_value() -> ServiceManagedEc2InstanceCapabilitiesOutputTypeDef:
    return {
        "vCpuCount": ...,
    }


# ServiceManagedEc2InstanceCapabilitiesOutputTypeDef definition

class ServiceManagedEc2InstanceCapabilitiesOutputTypeDef(TypedDict):
    vCpuCount: VCpuCountRangeTypeDef,  # (1)
    memoryMiB: MemoryMiBRangeTypeDef,  # (2)
    osFamily: ServiceManagedFleetOperatingSystemFamilyType,  # (3)
    cpuArchitectureType: CpuArchitectureTypeType,  # (4)
    rootEbsVolume: NotRequired[Ec2EbsVolumeTypeDef],  # (5)
    acceleratorCapabilities: NotRequired[AcceleratorCapabilitiesOutputTypeDef],  # (6)
    allowedInstanceTypes: NotRequired[List[str]],
    excludedInstanceTypes: NotRequired[List[str]],
    customAmounts: NotRequired[List[FleetAmountCapabilityTypeDef]],  # (7)
    customAttributes: NotRequired[List[FleetAttributeCapabilityOutputTypeDef]],  # (8)
```

1. See [:material-code-braces: VCpuCountRangeTypeDef](./type_defs.md#vcpucountrangetypedef) 
2. See [:material-code-braces: MemoryMiBRangeTypeDef](./type_defs.md#memorymibrangetypedef) 
3. See [:material-code-brackets: ServiceManagedFleetOperatingSystemFamilyType](./literals.md#servicemanagedfleetoperatingsystemfamilytype) 
4. See [:material-code-brackets: CpuArchitectureTypeType](./literals.md#cpuarchitecturetypetype) 
5. See [:material-code-braces: Ec2EbsVolumeTypeDef](./type_defs.md#ec2ebsvolumetypedef) 
6. See [:material-code-braces: AcceleratorCapabilitiesOutputTypeDef](./type_defs.md#acceleratorcapabilitiesoutputtypedef) 
7. See [:material-code-braces: FleetAmountCapabilityTypeDef](./type_defs.md#fleetamountcapabilitytypedef) 
8. See [:material-code-braces: FleetAttributeCapabilityOutputTypeDef](./type_defs.md#fleetattributecapabilityoutputtypedef) 
## ServiceManagedEc2InstanceCapabilitiesTypeDef

```python
# ServiceManagedEc2InstanceCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ServiceManagedEc2InstanceCapabilitiesTypeDef


def get_value() -> ServiceManagedEc2InstanceCapabilitiesTypeDef:
    return {
        "vCpuCount": ...,
    }


# ServiceManagedEc2InstanceCapabilitiesTypeDef definition

class ServiceManagedEc2InstanceCapabilitiesTypeDef(TypedDict):
    vCpuCount: VCpuCountRangeTypeDef,  # (1)
    memoryMiB: MemoryMiBRangeTypeDef,  # (2)
    osFamily: ServiceManagedFleetOperatingSystemFamilyType,  # (3)
    cpuArchitectureType: CpuArchitectureTypeType,  # (4)
    rootEbsVolume: NotRequired[Ec2EbsVolumeTypeDef],  # (5)
    acceleratorCapabilities: NotRequired[AcceleratorCapabilitiesTypeDef],  # (6)
    allowedInstanceTypes: NotRequired[Sequence[str]],
    excludedInstanceTypes: NotRequired[Sequence[str]],
    customAmounts: NotRequired[Sequence[FleetAmountCapabilityTypeDef]],  # (7)
    customAttributes: NotRequired[Sequence[FleetAttributeCapabilityTypeDef]],  # (8)
```

1. See [:material-code-braces: VCpuCountRangeTypeDef](./type_defs.md#vcpucountrangetypedef) 
2. See [:material-code-braces: MemoryMiBRangeTypeDef](./type_defs.md#memorymibrangetypedef) 
3. See [:material-code-brackets: ServiceManagedFleetOperatingSystemFamilyType](./literals.md#servicemanagedfleetoperatingsystemfamilytype) 
4. See [:material-code-brackets: CpuArchitectureTypeType](./literals.md#cpuarchitecturetypetype) 
5. See [:material-code-braces: Ec2EbsVolumeTypeDef](./type_defs.md#ec2ebsvolumetypedef) 
6. See [:material-code-braces: AcceleratorCapabilitiesTypeDef](./type_defs.md#acceleratorcapabilitiestypedef) 
7. See [:material-code-braces: FleetAmountCapabilityTypeDef](./type_defs.md#fleetamountcapabilitytypedef) 
8. See [:material-code-braces: FleetAttributeCapabilityTypeDef](./type_defs.md#fleetattributecapabilitytypedef) 
## AssignedSessionActionDefinitionTypeDef

```python
# AssignedSessionActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssignedSessionActionDefinitionTypeDef


def get_value() -> AssignedSessionActionDefinitionTypeDef:
    return {
        "envEnter": ...,
    }


# AssignedSessionActionDefinitionTypeDef definition

class AssignedSessionActionDefinitionTypeDef(TypedDict):
    envEnter: NotRequired[AssignedEnvironmentEnterSessionActionDefinitionTypeDef],  # (1)
    envExit: NotRequired[AssignedEnvironmentExitSessionActionDefinitionTypeDef],  # (2)
    taskRun: NotRequired[AssignedTaskRunSessionActionDefinitionTypeDef],  # (3)
    syncInputJobAttachments: NotRequired[AssignedSyncInputJobAttachmentsSessionActionDefinitionTypeDef],  # (4)
```

1. See [:material-code-braces: AssignedEnvironmentEnterSessionActionDefinitionTypeDef](./type_defs.md#assignedenvironmententersessionactiondefinitiontypedef) 
2. See [:material-code-braces: AssignedEnvironmentExitSessionActionDefinitionTypeDef](./type_defs.md#assignedenvironmentexitsessionactiondefinitiontypedef) 
3. See [:material-code-braces: AssignedTaskRunSessionActionDefinitionTypeDef](./type_defs.md#assignedtaskrunsessionactiondefinitiontypedef) 
4. See [:material-code-braces: AssignedSyncInputJobAttachmentsSessionActionDefinitionTypeDef](./type_defs.md#assignedsyncinputjobattachmentssessionactiondefinitiontypedef) 
## SessionActionDefinitionTypeDef

```python
# SessionActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SessionActionDefinitionTypeDef


def get_value() -> SessionActionDefinitionTypeDef:
    return {
        "envEnter": ...,
    }


# SessionActionDefinitionTypeDef definition

class SessionActionDefinitionTypeDef(TypedDict):
    envEnter: NotRequired[EnvironmentEnterSessionActionDefinitionTypeDef],  # (1)
    envExit: NotRequired[EnvironmentExitSessionActionDefinitionTypeDef],  # (2)
    taskRun: NotRequired[TaskRunSessionActionDefinitionTypeDef],  # (3)
    syncInputJobAttachments: NotRequired[SyncInputJobAttachmentsSessionActionDefinitionTypeDef],  # (4)
```

1. See [:material-code-braces: EnvironmentEnterSessionActionDefinitionTypeDef](./type_defs.md#environmententersessionactiondefinitiontypedef) 
2. See [:material-code-braces: EnvironmentExitSessionActionDefinitionTypeDef](./type_defs.md#environmentexitsessionactiondefinitiontypedef) 
3. See [:material-code-braces: TaskRunSessionActionDefinitionTypeDef](./type_defs.md#taskrunsessionactiondefinitiontypedef) 
4. See [:material-code-braces: SyncInputJobAttachmentsSessionActionDefinitionTypeDef](./type_defs.md#syncinputjobattachmentssessionactiondefinitiontypedef) 
## SearchTasksResponseTypeDef

```python
# SearchTasksResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchTasksResponseTypeDef


def get_value() -> SearchTasksResponseTypeDef:
    return {
        "tasks": ...,
    }


# SearchTasksResponseTypeDef definition

class SearchTasksResponseTypeDef(TypedDict):
    tasks: List[TaskSearchSummaryTypeDef],  # (1)
    nextItemOffset: int,
    totalResults: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskSearchSummaryTypeDef](./type_defs.md#tasksearchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTasksResponseTypeDef

```python
# ListTasksResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListTasksResponseTypeDef


def get_value() -> ListTasksResponseTypeDef:
    return {
        "tasks": ...,
    }


# ListTasksResponseTypeDef definition

class ListTasksResponseTypeDef(TypedDict):
    tasks: List[TaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TaskSummaryTypeDef](./type_defs.md#tasksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobResponseTypeDef

```python
# GetJobResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetJobResponseTypeDef


def get_value() -> GetJobResponseTypeDef:
    return {
        "jobId": ...,
    }


# GetJobResponseTypeDef definition

class GetJobResponseTypeDef(TypedDict):
    jobId: str,
    name: str,
    lifecycleStatus: JobLifecycleStatusType,  # (1)
    lifecycleStatusMessage: str,
    priority: int,
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    startedAt: datetime,
    endedAt: datetime,
    taskRunStatus: TaskRunStatusType,  # (2)
    targetTaskRunStatus: JobTargetTaskRunStatusType,  # (3)
    taskRunStatusCounts: Dict[TaskRunStatusType, int],  # (4)
    storageProfileId: str,
    maxFailedTasksCount: int,
    maxRetriesPerTask: int,
    parameters: Dict[str, JobParameterTypeDef],  # (5)
    attachments: AttachmentsOutputTypeDef,  # (6)
    description: str,
    maxWorkerCount: int,
    sourceJobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: JobLifecycleStatusType](./literals.md#joblifecyclestatustype) 
2. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
3. See [:material-code-brackets: JobTargetTaskRunStatusType](./literals.md#jobtargettaskrunstatustype) 
4. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
5. See [:material-code-braces: JobParameterTypeDef](./type_defs.md#jobparametertypedef) 
6. See [:material-code-braces: AttachmentsOutputTypeDef](./type_defs.md#attachmentsoutputtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobAttachmentDetailsEntityTypeDef

```python
# JobAttachmentDetailsEntityTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobAttachmentDetailsEntityTypeDef


def get_value() -> JobAttachmentDetailsEntityTypeDef:
    return {
        "jobId": ...,
    }


# JobAttachmentDetailsEntityTypeDef definition

class JobAttachmentDetailsEntityTypeDef(TypedDict):
    jobId: str,
    attachments: AttachmentsOutputTypeDef,  # (1)
```

1. See [:material-code-braces: AttachmentsOutputTypeDef](./type_defs.md#attachmentsoutputtypedef) 
## GetBudgetResponseTypeDef

```python
# GetBudgetResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetBudgetResponseTypeDef


def get_value() -> GetBudgetResponseTypeDef:
    return {
        "budgetId": ...,
    }


# GetBudgetResponseTypeDef definition

class GetBudgetResponseTypeDef(TypedDict):
    budgetId: str,
    usageTrackingResource: UsageTrackingResourceTypeDef,  # (1)
    status: BudgetStatusType,  # (2)
    displayName: str,
    description: str,
    approximateDollarLimit: float,
    usages: ConsumedUsagesTypeDef,  # (3)
    actions: List[ResponseBudgetActionTypeDef],  # (4)
    schedule: BudgetScheduleOutputTypeDef,  # (5)
    createdBy: str,
    createdAt: datetime,
    updatedBy: str,
    updatedAt: datetime,
    queueStoppedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: UsageTrackingResourceTypeDef](./type_defs.md#usagetrackingresourcetypedef) 
2. See [:material-code-brackets: BudgetStatusType](./literals.md#budgetstatustype) 
3. See [:material-code-braces: ConsumedUsagesTypeDef](./type_defs.md#consumedusagestypedef) 
4. See [:material-code-braces: ResponseBudgetActionTypeDef](./type_defs.md#responsebudgetactiontypedef) 
5. See [:material-code-braces: BudgetScheduleOutputTypeDef](./type_defs.md#budgetscheduleoutputtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBudgetsResponseTypeDef

```python
# ListBudgetsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListBudgetsResponseTypeDef


def get_value() -> ListBudgetsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListBudgetsResponseTypeDef definition

class ListBudgetsResponseTypeDef(TypedDict):
    budgets: List[BudgetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BudgetSummaryTypeDef](./type_defs.md#budgetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchJobsResponseTypeDef

```python
# SearchJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchJobsResponseTypeDef


def get_value() -> SearchJobsResponseTypeDef:
    return {
        "jobs": ...,
    }


# SearchJobsResponseTypeDef definition

class SearchJobsResponseTypeDef(TypedDict):
    jobs: List[JobSearchSummaryTypeDef],  # (1)
    nextItemOffset: int,
    totalResults: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobSearchSummaryTypeDef](./type_defs.md#jobsearchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomerManagedFleetConfigurationOutputTypeDef

```python
# CustomerManagedFleetConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CustomerManagedFleetConfigurationOutputTypeDef


def get_value() -> CustomerManagedFleetConfigurationOutputTypeDef:
    return {
        "mode": ...,
    }


# CustomerManagedFleetConfigurationOutputTypeDef definition

class CustomerManagedFleetConfigurationOutputTypeDef(TypedDict):
    mode: AutoScalingModeType,  # (1)
    workerCapabilities: CustomerManagedWorkerCapabilitiesOutputTypeDef,  # (2)
    storageProfileId: NotRequired[str],
```

1. See [:material-code-brackets: AutoScalingModeType](./literals.md#autoscalingmodetype) 
2. See [:material-code-braces: CustomerManagedWorkerCapabilitiesOutputTypeDef](./type_defs.md#customermanagedworkercapabilitiesoutputtypedef) 
## CustomerManagedFleetConfigurationTypeDef

```python
# CustomerManagedFleetConfigurationTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CustomerManagedFleetConfigurationTypeDef


def get_value() -> CustomerManagedFleetConfigurationTypeDef:
    return {
        "mode": ...,
    }


# CustomerManagedFleetConfigurationTypeDef definition

class CustomerManagedFleetConfigurationTypeDef(TypedDict):
    mode: AutoScalingModeType,  # (1)
    workerCapabilities: CustomerManagedWorkerCapabilitiesTypeDef,  # (2)
    storageProfileId: NotRequired[str],
```

1. See [:material-code-brackets: AutoScalingModeType](./literals.md#autoscalingmodetype) 
2. See [:material-code-braces: CustomerManagedWorkerCapabilitiesTypeDef](./type_defs.md#customermanagedworkercapabilitiestypedef) 
## SearchFilterExpressionTypeDef

```python
# SearchFilterExpressionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchFilterExpressionTypeDef


def get_value() -> SearchFilterExpressionTypeDef:
    return {
        "dateTimeFilter": ...,
    }


# SearchFilterExpressionTypeDef definition

class SearchFilterExpressionTypeDef(TypedDict):
    dateTimeFilter: NotRequired[DateTimeFilterExpressionTypeDef],  # (1)
    parameterFilter: NotRequired[ParameterFilterExpressionTypeDef],  # (2)
    searchTermFilter: NotRequired[SearchTermFilterExpressionTypeDef],  # (3)
    stringFilter: NotRequired[StringFilterExpressionTypeDef],  # (4)
    groupFilter: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: DateTimeFilterExpressionTypeDef](./type_defs.md#datetimefilterexpressiontypedef) 
2. See [:material-code-braces: ParameterFilterExpressionTypeDef](./type_defs.md#parameterfilterexpressiontypedef) 
3. See [:material-code-braces: SearchTermFilterExpressionTypeDef](./type_defs.md#searchtermfilterexpressiontypedef) 
4. See [:material-code-braces: StringFilterExpressionTypeDef](./type_defs.md#stringfilterexpressiontypedef) 
## BudgetScheduleTypeDef

```python
# BudgetScheduleTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import BudgetScheduleTypeDef


def get_value() -> BudgetScheduleTypeDef:
    return {
        "fixed": ...,
    }


# BudgetScheduleTypeDef definition

class BudgetScheduleTypeDef(TypedDict):
    fixed: NotRequired[FixedBudgetScheduleTypeDef],  # (1)
```

1. See [:material-code-braces: FixedBudgetScheduleTypeDef](./type_defs.md#fixedbudgetscheduletypedef) 
## UpdateWorkerScheduleRequestTypeDef

```python
# UpdateWorkerScheduleRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateWorkerScheduleRequestTypeDef


def get_value() -> UpdateWorkerScheduleRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateWorkerScheduleRequestTypeDef definition

class UpdateWorkerScheduleRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    updatedSessionActions: NotRequired[Mapping[str, UpdatedSessionActionInfoTypeDef]],  # (1)
```

1. See [:material-code-braces: UpdatedSessionActionInfoTypeDef](./type_defs.md#updatedsessionactioninfotypedef) 
## ListStepsResponseTypeDef

```python
# ListStepsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListStepsResponseTypeDef


def get_value() -> ListStepsResponseTypeDef:
    return {
        "steps": ...,
    }


# ListStepsResponseTypeDef definition

class ListStepsResponseTypeDef(TypedDict):
    steps: List[StepSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StepSummaryTypeDef](./type_defs.md#stepsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSessionResponseTypeDef

```python
# GetSessionResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetSessionResponseTypeDef


def get_value() -> GetSessionResponseTypeDef:
    return {
        "sessionId": ...,
    }


# GetSessionResponseTypeDef definition

class GetSessionResponseTypeDef(TypedDict):
    sessionId: str,
    fleetId: str,
    workerId: str,
    startedAt: datetime,
    log: LogConfigurationTypeDef,  # (1)
    lifecycleStatus: SessionLifecycleStatusType,  # (2)
    endedAt: datetime,
    updatedAt: datetime,
    updatedBy: str,
    targetLifecycleStatus: SessionLifecycleTargetStatusType,  # (3)
    hostProperties: HostPropertiesResponseTypeDef,  # (4)
    workerLog: LogConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
2. See [:material-code-brackets: SessionLifecycleStatusType](./literals.md#sessionlifecyclestatustype) 
3. See [:material-code-brackets: SessionLifecycleTargetStatusType](./literals.md#sessionlifecycletargetstatustype) 
4. See [:material-code-braces: HostPropertiesResponseTypeDef](./type_defs.md#hostpropertiesresponsetypedef) 
5. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkerResponseTypeDef

```python
# GetWorkerResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetWorkerResponseTypeDef


def get_value() -> GetWorkerResponseTypeDef:
    return {
        "farmId": ...,
    }


# GetWorkerResponseTypeDef definition

class GetWorkerResponseTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    hostProperties: HostPropertiesResponseTypeDef,  # (1)
    status: WorkerStatusType,  # (2)
    log: LogConfigurationTypeDef,  # (3)
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: HostPropertiesResponseTypeDef](./type_defs.md#hostpropertiesresponsetypedef) 
2. See [:material-code-brackets: WorkerStatusType](./literals.md#workerstatustype) 
3. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkerSearchSummaryTypeDef

```python
# WorkerSearchSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import WorkerSearchSummaryTypeDef


def get_value() -> WorkerSearchSummaryTypeDef:
    return {
        "fleetId": ...,
    }


# WorkerSearchSummaryTypeDef definition

class WorkerSearchSummaryTypeDef(TypedDict):
    fleetId: NotRequired[str],
    workerId: NotRequired[str],
    status: NotRequired[WorkerStatusType],  # (1)
    hostProperties: NotRequired[HostPropertiesResponseTypeDef],  # (2)
    createdBy: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: WorkerStatusType](./literals.md#workerstatustype) 
2. See [:material-code-braces: HostPropertiesResponseTypeDef](./type_defs.md#hostpropertiesresponsetypedef) 
## WorkerSummaryTypeDef

```python
# WorkerSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import WorkerSummaryTypeDef


def get_value() -> WorkerSummaryTypeDef:
    return {
        "workerId": ...,
    }


# WorkerSummaryTypeDef definition

class WorkerSummaryTypeDef(TypedDict):
    workerId: str,
    farmId: str,
    fleetId: str,
    status: WorkerStatusType,  # (1)
    createdAt: datetime,
    createdBy: str,
    hostProperties: NotRequired[HostPropertiesResponseTypeDef],  # (2)
    log: NotRequired[LogConfigurationTypeDef],  # (3)
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-brackets: WorkerStatusType](./literals.md#workerstatustype) 
2. See [:material-code-braces: HostPropertiesResponseTypeDef](./type_defs.md#hostpropertiesresponsetypedef) 
3. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
## HostPropertiesRequestTypeDef

```python
# HostPropertiesRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import HostPropertiesRequestTypeDef


def get_value() -> HostPropertiesRequestTypeDef:
    return {
        "ipAddresses": ...,
    }


# HostPropertiesRequestTypeDef definition

class HostPropertiesRequestTypeDef(TypedDict):
    ipAddresses: NotRequired[IpAddressesUnionTypeDef],  # (1)
    hostName: NotRequired[str],
```

1. See [:material-code-braces: IpAddressesTypeDef](./type_defs.md#ipaddressestypedef) [:material-code-braces: IpAddressesOutputTypeDef](./type_defs.md#ipaddressesoutputtypedef) 
## BatchGetJobEntityRequestTypeDef

```python
# BatchGetJobEntityRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import BatchGetJobEntityRequestTypeDef


def get_value() -> BatchGetJobEntityRequestTypeDef:
    return {
        "farmId": ...,
    }


# BatchGetJobEntityRequestTypeDef definition

class BatchGetJobEntityRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    identifiers: Sequence[JobEntityIdentifiersUnionTypeDef],  # (1)
```

1. See [:material-code-braces: JobEntityIdentifiersUnionTypeDef](./type_defs.md#jobentityidentifiersuniontypedef) 
## CreateQueueRequestTypeDef

```python
# CreateQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateQueueRequestTypeDef


def get_value() -> CreateQueueRequestTypeDef:
    return {
        "farmId": ...,
    }


# CreateQueueRequestTypeDef definition

class CreateQueueRequestTypeDef(TypedDict):
    farmId: str,
    displayName: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    defaultBudgetAction: NotRequired[DefaultQueueBudgetActionType],  # (1)
    jobAttachmentSettings: NotRequired[JobAttachmentSettingsTypeDef],  # (2)
    roleArn: NotRequired[str],
    jobRunAsUser: NotRequired[JobRunAsUserTypeDef],  # (3)
    requiredFileSystemLocationNames: NotRequired[Sequence[str]],
    allowedStorageProfileIds: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DefaultQueueBudgetActionType](./literals.md#defaultqueuebudgetactiontype) 
2. See [:material-code-braces: JobAttachmentSettingsTypeDef](./type_defs.md#jobattachmentsettingstypedef) 
3. See [:material-code-braces: JobRunAsUserTypeDef](./type_defs.md#jobrunasusertypedef) 
## GetQueueResponseTypeDef

```python
# GetQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetQueueResponseTypeDef


def get_value() -> GetQueueResponseTypeDef:
    return {
        "queueId": ...,
    }


# GetQueueResponseTypeDef definition

class GetQueueResponseTypeDef(TypedDict):
    queueId: str,
    displayName: str,
    description: str,
    farmId: str,
    status: QueueStatusType,  # (1)
    defaultBudgetAction: DefaultQueueBudgetActionType,  # (2)
    blockedReason: QueueBlockedReasonType,  # (3)
    jobAttachmentSettings: JobAttachmentSettingsTypeDef,  # (4)
    roleArn: str,
    requiredFileSystemLocationNames: List[str],
    allowedStorageProfileIds: List[str],
    jobRunAsUser: JobRunAsUserTypeDef,  # (5)
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
2. See [:material-code-brackets: DefaultQueueBudgetActionType](./literals.md#defaultqueuebudgetactiontype) 
3. See [:material-code-brackets: QueueBlockedReasonType](./literals.md#queueblockedreasontype) 
4. See [:material-code-braces: JobAttachmentSettingsTypeDef](./type_defs.md#jobattachmentsettingstypedef) 
5. See [:material-code-braces: JobRunAsUserTypeDef](./type_defs.md#jobrunasusertypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobDetailsEntityTypeDef

```python
# JobDetailsEntityTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobDetailsEntityTypeDef


def get_value() -> JobDetailsEntityTypeDef:
    return {
        "jobId": ...,
    }


# JobDetailsEntityTypeDef definition

class JobDetailsEntityTypeDef(TypedDict):
    jobId: str,
    logGroupName: str,
    schemaVersion: str,
    jobAttachmentSettings: NotRequired[JobAttachmentSettingsTypeDef],  # (1)
    jobRunAsUser: NotRequired[JobRunAsUserTypeDef],  # (2)
    queueRoleArn: NotRequired[str],
    parameters: NotRequired[Dict[str, JobParameterTypeDef]],  # (3)
    pathMappingRules: NotRequired[List[PathMappingRuleTypeDef]],  # (4)
```

1. See [:material-code-braces: JobAttachmentSettingsTypeDef](./type_defs.md#jobattachmentsettingstypedef) 
2. See [:material-code-braces: JobRunAsUserTypeDef](./type_defs.md#jobrunasusertypedef) 
3. See [:material-code-braces: JobParameterTypeDef](./type_defs.md#jobparametertypedef) 
4. See [:material-code-braces: PathMappingRuleTypeDef](./type_defs.md#pathmappingruletypedef) 
## UpdateQueueRequestTypeDef

```python
# UpdateQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateQueueRequestTypeDef


def get_value() -> UpdateQueueRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateQueueRequestTypeDef definition

class UpdateQueueRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    clientToken: NotRequired[str],
    displayName: NotRequired[str],
    description: NotRequired[str],
    defaultBudgetAction: NotRequired[DefaultQueueBudgetActionType],  # (1)
    jobAttachmentSettings: NotRequired[JobAttachmentSettingsTypeDef],  # (2)
    roleArn: NotRequired[str],
    jobRunAsUser: NotRequired[JobRunAsUserTypeDef],  # (3)
    requiredFileSystemLocationNamesToAdd: NotRequired[Sequence[str]],
    requiredFileSystemLocationNamesToRemove: NotRequired[Sequence[str]],
    allowedStorageProfileIdsToAdd: NotRequired[Sequence[str]],
    allowedStorageProfileIdsToRemove: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: DefaultQueueBudgetActionType](./literals.md#defaultqueuebudgetactiontype) 
2. See [:material-code-braces: JobAttachmentSettingsTypeDef](./type_defs.md#jobattachmentsettingstypedef) 
3. See [:material-code-braces: JobRunAsUserTypeDef](./type_defs.md#jobrunasusertypedef) 
## StepSearchSummaryTypeDef

```python
# StepSearchSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import StepSearchSummaryTypeDef


def get_value() -> StepSearchSummaryTypeDef:
    return {
        "stepId": ...,
    }


# StepSearchSummaryTypeDef definition

class StepSearchSummaryTypeDef(TypedDict):
    stepId: NotRequired[str],
    jobId: NotRequired[str],
    queueId: NotRequired[str],
    name: NotRequired[str],
    lifecycleStatus: NotRequired[StepLifecycleStatusType],  # (1)
    lifecycleStatusMessage: NotRequired[str],
    taskRunStatus: NotRequired[TaskRunStatusType],  # (2)
    targetTaskRunStatus: NotRequired[StepTargetTaskRunStatusType],  # (3)
    taskRunStatusCounts: NotRequired[Dict[TaskRunStatusType, int]],  # (4)
    createdAt: NotRequired[datetime],
    startedAt: NotRequired[datetime],
    endedAt: NotRequired[datetime],
    parameterSpace: NotRequired[ParameterSpaceTypeDef],  # (5)
```

1. See [:material-code-brackets: StepLifecycleStatusType](./literals.md#steplifecyclestatustype) 
2. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
3. See [:material-code-brackets: StepTargetTaskRunStatusType](./literals.md#steptargettaskrunstatustype) 
4. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
5. See [:material-code-braces: ParameterSpaceTypeDef](./type_defs.md#parameterspacetypedef) 
## SessionActionSummaryTypeDef

```python
# SessionActionSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SessionActionSummaryTypeDef


def get_value() -> SessionActionSummaryTypeDef:
    return {
        "sessionActionId": ...,
    }


# SessionActionSummaryTypeDef definition

class SessionActionSummaryTypeDef(TypedDict):
    sessionActionId: str,
    status: SessionActionStatusType,  # (1)
    definition: SessionActionDefinitionSummaryTypeDef,  # (2)
    startedAt: NotRequired[datetime],
    endedAt: NotRequired[datetime],
    workerUpdatedAt: NotRequired[datetime],
    progressPercent: NotRequired[float],
```

1. See [:material-code-brackets: SessionActionStatusType](./literals.md#sessionactionstatustype) 
2. See [:material-code-braces: SessionActionDefinitionSummaryTypeDef](./type_defs.md#sessionactiondefinitionsummarytypedef) 
## GetSessionsStatisticsAggregationResponseTypeDef

```python
# GetSessionsStatisticsAggregationResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetSessionsStatisticsAggregationResponseTypeDef


def get_value() -> GetSessionsStatisticsAggregationResponseTypeDef:
    return {
        "statistics": ...,
    }


# GetSessionsStatisticsAggregationResponseTypeDef definition

class GetSessionsStatisticsAggregationResponseTypeDef(TypedDict):
    statistics: List[StatisticsTypeDef],  # (1)
    status: SessionsStatisticsAggregationStatusType,  # (2)
    statusMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StatisticsTypeDef](./type_defs.md#statisticstypedef) 
2. See [:material-code-brackets: SessionsStatisticsAggregationStatusType](./literals.md#sessionsstatisticsaggregationstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStepResponseTypeDef

```python
# GetStepResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetStepResponseTypeDef


def get_value() -> GetStepResponseTypeDef:
    return {
        "stepId": ...,
    }


# GetStepResponseTypeDef definition

class GetStepResponseTypeDef(TypedDict):
    stepId: str,
    name: str,
    lifecycleStatus: StepLifecycleStatusType,  # (1)
    lifecycleStatusMessage: str,
    taskRunStatus: TaskRunStatusType,  # (2)
    taskRunStatusCounts: Dict[TaskRunStatusType, int],  # (3)
    targetTaskRunStatus: StepTargetTaskRunStatusType,  # (4)
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    startedAt: datetime,
    endedAt: datetime,
    dependencyCounts: DependencyCountsTypeDef,  # (5)
    requiredCapabilities: StepRequiredCapabilitiesTypeDef,  # (6)
    parameterSpace: ParameterSpaceTypeDef,  # (7)
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: StepLifecycleStatusType](./literals.md#steplifecyclestatustype) 
2. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
3. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
4. See [:material-code-brackets: StepTargetTaskRunStatusType](./literals.md#steptargettaskrunstatustype) 
5. See [:material-code-braces: DependencyCountsTypeDef](./type_defs.md#dependencycountstypedef) 
6. See [:material-code-braces: StepRequiredCapabilitiesTypeDef](./type_defs.md#steprequiredcapabilitiestypedef) 
7. See [:material-code-braces: ParameterSpaceTypeDef](./type_defs.md#parameterspacetypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceManagedEc2FleetConfigurationOutputTypeDef

```python
# ServiceManagedEc2FleetConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ServiceManagedEc2FleetConfigurationOutputTypeDef


def get_value() -> ServiceManagedEc2FleetConfigurationOutputTypeDef:
    return {
        "instanceCapabilities": ...,
    }


# ServiceManagedEc2FleetConfigurationOutputTypeDef definition

class ServiceManagedEc2FleetConfigurationOutputTypeDef(TypedDict):
    instanceCapabilities: ServiceManagedEc2InstanceCapabilitiesOutputTypeDef,  # (1)
    instanceMarketOptions: ServiceManagedEc2InstanceMarketOptionsTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceManagedEc2InstanceCapabilitiesOutputTypeDef](./type_defs.md#servicemanagedec2instancecapabilitiesoutputtypedef) 
2. See [:material-code-braces: ServiceManagedEc2InstanceMarketOptionsTypeDef](./type_defs.md#servicemanagedec2instancemarketoptionstypedef) 
## ServiceManagedEc2FleetConfigurationTypeDef

```python
# ServiceManagedEc2FleetConfigurationTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ServiceManagedEc2FleetConfigurationTypeDef


def get_value() -> ServiceManagedEc2FleetConfigurationTypeDef:
    return {
        "instanceCapabilities": ...,
    }


# ServiceManagedEc2FleetConfigurationTypeDef definition

class ServiceManagedEc2FleetConfigurationTypeDef(TypedDict):
    instanceCapabilities: ServiceManagedEc2InstanceCapabilitiesTypeDef,  # (1)
    instanceMarketOptions: ServiceManagedEc2InstanceMarketOptionsTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceManagedEc2InstanceCapabilitiesTypeDef](./type_defs.md#servicemanagedec2instancecapabilitiestypedef) 
2. See [:material-code-braces: ServiceManagedEc2InstanceMarketOptionsTypeDef](./type_defs.md#servicemanagedec2instancemarketoptionstypedef) 
## AssignedSessionActionTypeDef

```python
# AssignedSessionActionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssignedSessionActionTypeDef


def get_value() -> AssignedSessionActionTypeDef:
    return {
        "sessionActionId": ...,
    }


# AssignedSessionActionTypeDef definition

class AssignedSessionActionTypeDef(TypedDict):
    sessionActionId: str,
    definition: AssignedSessionActionDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: AssignedSessionActionDefinitionTypeDef](./type_defs.md#assignedsessionactiondefinitiontypedef) 
## GetSessionActionResponseTypeDef

```python
# GetSessionActionResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetSessionActionResponseTypeDef


def get_value() -> GetSessionActionResponseTypeDef:
    return {
        "sessionActionId": ...,
    }


# GetSessionActionResponseTypeDef definition

class GetSessionActionResponseTypeDef(TypedDict):
    sessionActionId: str,
    status: SessionActionStatusType,  # (1)
    startedAt: datetime,
    endedAt: datetime,
    workerUpdatedAt: datetime,
    progressPercent: float,
    sessionId: str,
    processExitCode: int,
    progressMessage: str,
    definition: SessionActionDefinitionTypeDef,  # (2)
    acquiredLimits: List[AcquiredLimitTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: SessionActionStatusType](./literals.md#sessionactionstatustype) 
2. See [:material-code-braces: SessionActionDefinitionTypeDef](./type_defs.md#sessionactiondefinitiontypedef) 
3. See [:material-code-braces: AcquiredLimitTypeDef](./type_defs.md#acquiredlimittypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobRequestTypeDef

```python
# CreateJobRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateJobRequestTypeDef


def get_value() -> CreateJobRequestTypeDef:
    return {
        "farmId": ...,
    }


# CreateJobRequestTypeDef definition

class CreateJobRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    priority: int,
    clientToken: NotRequired[str],
    template: NotRequired[str],
    templateType: NotRequired[JobTemplateTypeType],  # (1)
    parameters: NotRequired[Mapping[str, JobParameterTypeDef]],  # (2)
    attachments: NotRequired[AttachmentsUnionTypeDef],  # (3)
    storageProfileId: NotRequired[str],
    targetTaskRunStatus: NotRequired[CreateJobTargetTaskRunStatusType],  # (4)
    maxFailedTasksCount: NotRequired[int],
    maxRetriesPerTask: NotRequired[int],
    maxWorkerCount: NotRequired[int],
    sourceJobId: NotRequired[str],
```

1. See [:material-code-brackets: JobTemplateTypeType](./literals.md#jobtemplatetypetype) 
2. See [:material-code-braces: JobParameterTypeDef](./type_defs.md#jobparametertypedef) 
3. See [:material-code-braces: AttachmentsTypeDef](./type_defs.md#attachmentstypedef) [:material-code-braces: AttachmentsOutputTypeDef](./type_defs.md#attachmentsoutputtypedef) 
4. See [:material-code-brackets: CreateJobTargetTaskRunStatusType](./literals.md#createjobtargettaskrunstatustype) 
## SearchGroupedFilterExpressionsTypeDef

```python
# SearchGroupedFilterExpressionsTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchGroupedFilterExpressionsTypeDef


def get_value() -> SearchGroupedFilterExpressionsTypeDef:
    return {
        "filters": ...,
    }


# SearchGroupedFilterExpressionsTypeDef definition

class SearchGroupedFilterExpressionsTypeDef(TypedDict):
    filters: Sequence[SearchFilterExpressionTypeDef],  # (1)
    operator: LogicalOperatorType,  # (2)
```

1. See [:material-code-braces: SearchFilterExpressionTypeDef](./type_defs.md#searchfilterexpressiontypedef) 
2. See [:material-code-brackets: LogicalOperatorType](./literals.md#logicaloperatortype) 
## SearchWorkersResponseTypeDef

```python
# SearchWorkersResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchWorkersResponseTypeDef


def get_value() -> SearchWorkersResponseTypeDef:
    return {
        "workers": ...,
    }


# SearchWorkersResponseTypeDef definition

class SearchWorkersResponseTypeDef(TypedDict):
    workers: List[WorkerSearchSummaryTypeDef],  # (1)
    nextItemOffset: int,
    totalResults: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkerSearchSummaryTypeDef](./type_defs.md#workersearchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkersResponseTypeDef

```python
# ListWorkersResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListWorkersResponseTypeDef


def get_value() -> ListWorkersResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListWorkersResponseTypeDef definition

class ListWorkersResponseTypeDef(TypedDict):
    workers: List[WorkerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkerSummaryTypeDef](./type_defs.md#workersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkerRequestTypeDef

```python
# CreateWorkerRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateWorkerRequestTypeDef


def get_value() -> CreateWorkerRequestTypeDef:
    return {
        "farmId": ...,
    }


# CreateWorkerRequestTypeDef definition

class CreateWorkerRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    hostProperties: NotRequired[HostPropertiesRequestTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: HostPropertiesRequestTypeDef](./type_defs.md#hostpropertiesrequesttypedef) 
## UpdateWorkerRequestTypeDef

```python
# UpdateWorkerRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateWorkerRequestTypeDef


def get_value() -> UpdateWorkerRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateWorkerRequestTypeDef definition

class UpdateWorkerRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    status: NotRequired[UpdatedWorkerStatusType],  # (1)
    capabilities: NotRequired[WorkerCapabilitiesTypeDef],  # (2)
    hostProperties: NotRequired[HostPropertiesRequestTypeDef],  # (3)
```

1. See [:material-code-brackets: UpdatedWorkerStatusType](./literals.md#updatedworkerstatustype) 
2. See [:material-code-braces: WorkerCapabilitiesTypeDef](./type_defs.md#workercapabilitiestypedef) 
3. See [:material-code-braces: HostPropertiesRequestTypeDef](./type_defs.md#hostpropertiesrequesttypedef) 
## JobEntityTypeDef

```python
# JobEntityTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import JobEntityTypeDef


def get_value() -> JobEntityTypeDef:
    return {
        "jobDetails": ...,
    }


# JobEntityTypeDef definition

class JobEntityTypeDef(TypedDict):
    jobDetails: NotRequired[JobDetailsEntityTypeDef],  # (1)
    jobAttachmentDetails: NotRequired[JobAttachmentDetailsEntityTypeDef],  # (2)
    stepDetails: NotRequired[StepDetailsEntityTypeDef],  # (3)
    environmentDetails: NotRequired[EnvironmentDetailsEntityTypeDef],  # (4)
```

1. See [:material-code-braces: JobDetailsEntityTypeDef](./type_defs.md#jobdetailsentitytypedef) 
2. See [:material-code-braces: JobAttachmentDetailsEntityTypeDef](./type_defs.md#jobattachmentdetailsentitytypedef) 
3. See [:material-code-braces: StepDetailsEntityTypeDef](./type_defs.md#stepdetailsentitytypedef) 
4. See [:material-code-braces: EnvironmentDetailsEntityTypeDef](./type_defs.md#environmentdetailsentitytypedef) 
## SearchStepsResponseTypeDef

```python
# SearchStepsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchStepsResponseTypeDef


def get_value() -> SearchStepsResponseTypeDef:
    return {
        "steps": ...,
    }


# SearchStepsResponseTypeDef definition

class SearchStepsResponseTypeDef(TypedDict):
    steps: List[StepSearchSummaryTypeDef],  # (1)
    nextItemOffset: int,
    totalResults: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StepSearchSummaryTypeDef](./type_defs.md#stepsearchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSessionActionsResponseTypeDef

```python
# ListSessionActionsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListSessionActionsResponseTypeDef


def get_value() -> ListSessionActionsResponseTypeDef:
    return {
        "sessionActions": ...,
    }


# ListSessionActionsResponseTypeDef definition

class ListSessionActionsResponseTypeDef(TypedDict):
    sessionActions: List[SessionActionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SessionActionSummaryTypeDef](./type_defs.md#sessionactionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FleetConfigurationOutputTypeDef

```python
# FleetConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FleetConfigurationOutputTypeDef


def get_value() -> FleetConfigurationOutputTypeDef:
    return {
        "customerManaged": ...,
    }


# FleetConfigurationOutputTypeDef definition

class FleetConfigurationOutputTypeDef(TypedDict):
    customerManaged: NotRequired[CustomerManagedFleetConfigurationOutputTypeDef],  # (1)
    serviceManagedEc2: NotRequired[ServiceManagedEc2FleetConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: CustomerManagedFleetConfigurationOutputTypeDef](./type_defs.md#customermanagedfleetconfigurationoutputtypedef) 
2. See [:material-code-braces: ServiceManagedEc2FleetConfigurationOutputTypeDef](./type_defs.md#servicemanagedec2fleetconfigurationoutputtypedef) 
## FleetConfigurationTypeDef

```python
# FleetConfigurationTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FleetConfigurationTypeDef


def get_value() -> FleetConfigurationTypeDef:
    return {
        "customerManaged": ...,
    }


# FleetConfigurationTypeDef definition

class FleetConfigurationTypeDef(TypedDict):
    customerManaged: NotRequired[CustomerManagedFleetConfigurationTypeDef],  # (1)
    serviceManagedEc2: NotRequired[ServiceManagedEc2FleetConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: CustomerManagedFleetConfigurationTypeDef](./type_defs.md#customermanagedfleetconfigurationtypedef) 
2. See [:material-code-braces: ServiceManagedEc2FleetConfigurationTypeDef](./type_defs.md#servicemanagedec2fleetconfigurationtypedef) 
## AssignedSessionTypeDef

```python
# AssignedSessionTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import AssignedSessionTypeDef


def get_value() -> AssignedSessionTypeDef:
    return {
        "queueId": ...,
    }


# AssignedSessionTypeDef definition

class AssignedSessionTypeDef(TypedDict):
    queueId: str,
    jobId: str,
    sessionActions: List[AssignedSessionActionTypeDef],  # (1)
    logConfiguration: LogConfigurationTypeDef,  # (2)
```

1. See [:material-code-braces: AssignedSessionActionTypeDef](./type_defs.md#assignedsessionactiontypedef) 
2. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
## SearchJobsRequestTypeDef

```python
# SearchJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchJobsRequestTypeDef


def get_value() -> SearchJobsRequestTypeDef:
    return {
        "farmId": ...,
    }


# SearchJobsRequestTypeDef definition

class SearchJobsRequestTypeDef(TypedDict):
    farmId: str,
    queueIds: Sequence[str],
    itemOffset: int,
    filterExpressions: NotRequired[SearchGroupedFilterExpressionsTypeDef],  # (1)
    sortExpressions: NotRequired[Sequence[SearchSortExpressionTypeDef]],  # (2)
    pageSize: NotRequired[int],
```

1. See [:material-code-braces: SearchGroupedFilterExpressionsTypeDef](./type_defs.md#searchgroupedfilterexpressionstypedef) 
2. See [:material-code-braces: SearchSortExpressionTypeDef](./type_defs.md#searchsortexpressiontypedef) 
## SearchStepsRequestTypeDef

```python
# SearchStepsRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchStepsRequestTypeDef


def get_value() -> SearchStepsRequestTypeDef:
    return {
        "farmId": ...,
    }


# SearchStepsRequestTypeDef definition

class SearchStepsRequestTypeDef(TypedDict):
    farmId: str,
    queueIds: Sequence[str],
    itemOffset: int,
    jobId: NotRequired[str],
    filterExpressions: NotRequired[SearchGroupedFilterExpressionsTypeDef],  # (1)
    sortExpressions: NotRequired[Sequence[SearchSortExpressionTypeDef]],  # (2)
    pageSize: NotRequired[int],
```

1. See [:material-code-braces: SearchGroupedFilterExpressionsTypeDef](./type_defs.md#searchgroupedfilterexpressionstypedef) 
2. See [:material-code-braces: SearchSortExpressionTypeDef](./type_defs.md#searchsortexpressiontypedef) 
## SearchTasksRequestTypeDef

```python
# SearchTasksRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchTasksRequestTypeDef


def get_value() -> SearchTasksRequestTypeDef:
    return {
        "farmId": ...,
    }


# SearchTasksRequestTypeDef definition

class SearchTasksRequestTypeDef(TypedDict):
    farmId: str,
    queueIds: Sequence[str],
    itemOffset: int,
    jobId: NotRequired[str],
    filterExpressions: NotRequired[SearchGroupedFilterExpressionsTypeDef],  # (1)
    sortExpressions: NotRequired[Sequence[SearchSortExpressionTypeDef]],  # (2)
    pageSize: NotRequired[int],
```

1. See [:material-code-braces: SearchGroupedFilterExpressionsTypeDef](./type_defs.md#searchgroupedfilterexpressionstypedef) 
2. See [:material-code-braces: SearchSortExpressionTypeDef](./type_defs.md#searchsortexpressiontypedef) 
## SearchWorkersRequestTypeDef

```python
# SearchWorkersRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import SearchWorkersRequestTypeDef


def get_value() -> SearchWorkersRequestTypeDef:
    return {
        "farmId": ...,
    }


# SearchWorkersRequestTypeDef definition

class SearchWorkersRequestTypeDef(TypedDict):
    farmId: str,
    fleetIds: Sequence[str],
    itemOffset: int,
    filterExpressions: NotRequired[SearchGroupedFilterExpressionsTypeDef],  # (1)
    sortExpressions: NotRequired[Sequence[SearchSortExpressionTypeDef]],  # (2)
    pageSize: NotRequired[int],
```

1. See [:material-code-braces: SearchGroupedFilterExpressionsTypeDef](./type_defs.md#searchgroupedfilterexpressionstypedef) 
2. See [:material-code-braces: SearchSortExpressionTypeDef](./type_defs.md#searchsortexpressiontypedef) 
## CreateBudgetRequestTypeDef

```python
# CreateBudgetRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateBudgetRequestTypeDef


def get_value() -> CreateBudgetRequestTypeDef:
    return {
        "farmId": ...,
    }


# CreateBudgetRequestTypeDef definition

class CreateBudgetRequestTypeDef(TypedDict):
    farmId: str,
    usageTrackingResource: UsageTrackingResourceTypeDef,  # (1)
    displayName: str,
    approximateDollarLimit: float,
    actions: Sequence[BudgetActionToAddTypeDef],  # (2)
    schedule: BudgetScheduleUnionTypeDef,  # (3)
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-braces: UsageTrackingResourceTypeDef](./type_defs.md#usagetrackingresourcetypedef) 
2. See [:material-code-braces: BudgetActionToAddTypeDef](./type_defs.md#budgetactiontoaddtypedef) 
3. See [:material-code-braces: BudgetScheduleTypeDef](./type_defs.md#budgetscheduletypedef) [:material-code-braces: BudgetScheduleOutputTypeDef](./type_defs.md#budgetscheduleoutputtypedef) 
## UpdateBudgetRequestTypeDef

```python
# UpdateBudgetRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateBudgetRequestTypeDef


def get_value() -> UpdateBudgetRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateBudgetRequestTypeDef definition

class UpdateBudgetRequestTypeDef(TypedDict):
    farmId: str,
    budgetId: str,
    clientToken: NotRequired[str],
    displayName: NotRequired[str],
    description: NotRequired[str],
    status: NotRequired[BudgetStatusType],  # (1)
    approximateDollarLimit: NotRequired[float],
    actionsToAdd: NotRequired[Sequence[BudgetActionToAddTypeDef]],  # (2)
    actionsToRemove: NotRequired[Sequence[BudgetActionToRemoveTypeDef]],  # (3)
    schedule: NotRequired[BudgetScheduleUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: BudgetStatusType](./literals.md#budgetstatustype) 
2. See [:material-code-braces: BudgetActionToAddTypeDef](./type_defs.md#budgetactiontoaddtypedef) 
3. See [:material-code-braces: BudgetActionToRemoveTypeDef](./type_defs.md#budgetactiontoremovetypedef) 
4. See [:material-code-braces: BudgetScheduleTypeDef](./type_defs.md#budgetscheduletypedef) [:material-code-braces: BudgetScheduleOutputTypeDef](./type_defs.md#budgetscheduleoutputtypedef) 
## BatchGetJobEntityResponseTypeDef

```python
# BatchGetJobEntityResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import BatchGetJobEntityResponseTypeDef


def get_value() -> BatchGetJobEntityResponseTypeDef:
    return {
        "entities": ...,
    }


# BatchGetJobEntityResponseTypeDef definition

class BatchGetJobEntityResponseTypeDef(TypedDict):
    entities: List[JobEntityTypeDef],  # (1)
    errors: List[GetJobEntityErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: JobEntityTypeDef](./type_defs.md#jobentitytypedef) 
2. See [:material-code-braces: GetJobEntityErrorTypeDef](./type_defs.md#getjobentityerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FleetSummaryTypeDef

```python
# FleetSummaryTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import FleetSummaryTypeDef


def get_value() -> FleetSummaryTypeDef:
    return {
        "fleetId": ...,
    }


# FleetSummaryTypeDef definition

class FleetSummaryTypeDef(TypedDict):
    fleetId: str,
    farmId: str,
    displayName: str,
    status: FleetStatusType,  # (1)
    workerCount: int,
    minWorkerCount: int,
    maxWorkerCount: int,
    configuration: FleetConfigurationOutputTypeDef,  # (3)
    createdAt: datetime,
    createdBy: str,
    autoScalingStatus: NotRequired[AutoScalingStatusType],  # (2)
    targetWorkerCount: NotRequired[int],
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-brackets: FleetStatusType](./literals.md#fleetstatustype) 
2. See [:material-code-brackets: AutoScalingStatusType](./literals.md#autoscalingstatustype) 
3. See [:material-code-braces: FleetConfigurationOutputTypeDef](./type_defs.md#fleetconfigurationoutputtypedef) 
## GetFleetResponseTypeDef

```python
# GetFleetResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import GetFleetResponseTypeDef


def get_value() -> GetFleetResponseTypeDef:
    return {
        "fleetId": ...,
    }


# GetFleetResponseTypeDef definition

class GetFleetResponseTypeDef(TypedDict):
    fleetId: str,
    farmId: str,
    displayName: str,
    description: str,
    status: FleetStatusType,  # (1)
    autoScalingStatus: AutoScalingStatusType,  # (2)
    targetWorkerCount: int,
    workerCount: int,
    minWorkerCount: int,
    maxWorkerCount: int,
    configuration: FleetConfigurationOutputTypeDef,  # (3)
    capabilities: FleetCapabilitiesTypeDef,  # (4)
    roleArn: str,
    createdAt: datetime,
    createdBy: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: FleetStatusType](./literals.md#fleetstatustype) 
2. See [:material-code-brackets: AutoScalingStatusType](./literals.md#autoscalingstatustype) 
3. See [:material-code-braces: FleetConfigurationOutputTypeDef](./type_defs.md#fleetconfigurationoutputtypedef) 
4. See [:material-code-braces: FleetCapabilitiesTypeDef](./type_defs.md#fleetcapabilitiestypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkerScheduleResponseTypeDef

```python
# UpdateWorkerScheduleResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateWorkerScheduleResponseTypeDef


def get_value() -> UpdateWorkerScheduleResponseTypeDef:
    return {
        "assignedSessions": ...,
    }


# UpdateWorkerScheduleResponseTypeDef definition

class UpdateWorkerScheduleResponseTypeDef(TypedDict):
    assignedSessions: Dict[str, AssignedSessionTypeDef],  # (1)
    cancelSessionActions: Dict[str, List[str]],
    desiredWorkerStatus: DesiredWorkerStatusType,  # (2)
    updateIntervalSeconds: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssignedSessionTypeDef](./type_defs.md#assignedsessiontypedef) 
2. See [:material-code-brackets: DesiredWorkerStatusType](./literals.md#desiredworkerstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFleetsResponseTypeDef

```python
# ListFleetsResponseTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import ListFleetsResponseTypeDef


def get_value() -> ListFleetsResponseTypeDef:
    return {
        "fleets": ...,
    }


# ListFleetsResponseTypeDef definition

class ListFleetsResponseTypeDef(TypedDict):
    fleets: List[FleetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetSummaryTypeDef](./type_defs.md#fleetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetRequestTypeDef

```python
# CreateFleetRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import CreateFleetRequestTypeDef


def get_value() -> CreateFleetRequestTypeDef:
    return {
        "farmId": ...,
    }


# CreateFleetRequestTypeDef definition

class CreateFleetRequestTypeDef(TypedDict):
    farmId: str,
    displayName: str,
    roleArn: str,
    maxWorkerCount: int,
    configuration: FleetConfigurationUnionTypeDef,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    minWorkerCount: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FleetConfigurationTypeDef](./type_defs.md#fleetconfigurationtypedef) [:material-code-braces: FleetConfigurationOutputTypeDef](./type_defs.md#fleetconfigurationoutputtypedef) 
## UpdateFleetRequestTypeDef

```python
# UpdateFleetRequestTypeDef TypedDict usage example

from types_aiobotocore_deadline.type_defs import UpdateFleetRequestTypeDef


def get_value() -> UpdateFleetRequestTypeDef:
    return {
        "farmId": ...,
    }


# UpdateFleetRequestTypeDef definition

class UpdateFleetRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    clientToken: NotRequired[str],
    displayName: NotRequired[str],
    description: NotRequired[str],
    roleArn: NotRequired[str],
    minWorkerCount: NotRequired[int],
    maxWorkerCount: NotRequired[int],
    configuration: NotRequired[FleetConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: FleetConfigurationTypeDef](./type_defs.md#fleetconfigurationtypedef) [:material-code-braces: FleetConfigurationOutputTypeDef](./type_defs.md#fleetconfigurationoutputtypedef) 
