# Type definitions

> [Index](../README.md) > [DeadlineCloud](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DeadlineCloud](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline.html#DeadlineCloud)
    type annotations stubs module [types-aiobotocore-deadline](https://pypi.org/project/types-aiobotocore-deadline/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## FleetAttributeCapabilityUnionTypeDef

```python
# FleetAttributeCapabilityUnionTypeDef definition

FleetAttributeCapabilityUnionTypeDef = Union[
    FleetAttributeCapabilityTypeDef,  # (1)
    FleetAttributeCapabilityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FleetAttributeCapabilityTypeDef](./type_defs.md#fleetattributecapabilitytypedef) 
2. See [:material-code-braces: FleetAttributeCapabilityOutputTypeDef](./type_defs.md#fleetattributecapabilityoutputtypedef) 

## IpAddressesUnionTypeDef

```python
# IpAddressesUnionTypeDef definition

IpAddressesUnionTypeDef = Union[
    IpAddressesTypeDef,  # (1)
    IpAddressesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IpAddressesTypeDef](./type_defs.md#ipaddressestypedef) 
2. See [:material-code-braces: IpAddressesOutputTypeDef](./type_defs.md#ipaddressesoutputtypedef) 

## ManifestPropertiesUnionTypeDef

```python
# ManifestPropertiesUnionTypeDef definition

ManifestPropertiesUnionTypeDef = Union[
    ManifestPropertiesTypeDef,  # (1)
    ManifestPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ManifestPropertiesTypeDef](./type_defs.md#manifestpropertiestypedef) 
2. See [:material-code-braces: ManifestPropertiesOutputTypeDef](./type_defs.md#manifestpropertiesoutputtypedef) 

## FixedBudgetScheduleUnionTypeDef

```python
# FixedBudgetScheduleUnionTypeDef definition

FixedBudgetScheduleUnionTypeDef = Union[
    FixedBudgetScheduleTypeDef,  # (1)
    FixedBudgetScheduleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FixedBudgetScheduleTypeDef](./type_defs.md#fixedbudgetscheduletypedef) 
2. See [:material-code-braces: FixedBudgetScheduleOutputTypeDef](./type_defs.md#fixedbudgetscheduleoutputtypedef) 

## ServiceManagedEc2InstanceCapabilitiesUnionTypeDef

```python
# ServiceManagedEc2InstanceCapabilitiesUnionTypeDef definition

ServiceManagedEc2InstanceCapabilitiesUnionTypeDef = Union[
    ServiceManagedEc2InstanceCapabilitiesTypeDef,  # (1)
    ServiceManagedEc2InstanceCapabilitiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServiceManagedEc2InstanceCapabilitiesTypeDef](./type_defs.md#servicemanagedec2instancecapabilitiestypedef) 
2. See [:material-code-braces: ServiceManagedEc2InstanceCapabilitiesOutputTypeDef](./type_defs.md#servicemanagedec2instancecapabilitiesoutputtypedef) 

## CustomerManagedWorkerCapabilitiesUnionTypeDef

```python
# CustomerManagedWorkerCapabilitiesUnionTypeDef definition

CustomerManagedWorkerCapabilitiesUnionTypeDef = Union[
    CustomerManagedWorkerCapabilitiesTypeDef,  # (1)
    CustomerManagedWorkerCapabilitiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomerManagedWorkerCapabilitiesTypeDef](./type_defs.md#customermanagedworkercapabilitiestypedef) 
2. See [:material-code-braces: CustomerManagedWorkerCapabilitiesOutputTypeDef](./type_defs.md#customermanagedworkercapabilitiesoutputtypedef) 

## ServiceManagedEc2FleetConfigurationUnionTypeDef

```python
# ServiceManagedEc2FleetConfigurationUnionTypeDef definition

ServiceManagedEc2FleetConfigurationUnionTypeDef = Union[
    ServiceManagedEc2FleetConfigurationTypeDef,  # (1)
    ServiceManagedEc2FleetConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServiceManagedEc2FleetConfigurationTypeDef](./type_defs.md#servicemanagedec2fleetconfigurationtypedef) 
2. See [:material-code-braces: ServiceManagedEc2FleetConfigurationOutputTypeDef](./type_defs.md#servicemanagedec2fleetconfigurationoutputtypedef) 

## CustomerManagedFleetConfigurationUnionTypeDef

```python
# CustomerManagedFleetConfigurationUnionTypeDef definition

CustomerManagedFleetConfigurationUnionTypeDef = Union[
    CustomerManagedFleetConfigurationTypeDef,  # (1)
    CustomerManagedFleetConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomerManagedFleetConfigurationTypeDef](./type_defs.md#customermanagedfleetconfigurationtypedef) 
2. See [:material-code-braces: CustomerManagedFleetConfigurationOutputTypeDef](./type_defs.md#customermanagedfleetconfigurationoutputtypedef) 



## AcceleratorCountRangeTypeDef

```python
# AcceleratorCountRangeTypeDef definition

class AcceleratorCountRangeTypeDef(TypedDict):
    min: int,
    max: NotRequired[int],
```

## AcceleratorTotalMemoryMiBRangeTypeDef

```python
# AcceleratorTotalMemoryMiBRangeTypeDef definition

class AcceleratorTotalMemoryMiBRangeTypeDef(TypedDict):
    min: int,
    max: NotRequired[int],
```

## AssignedEnvironmentEnterSessionActionDefinitionTypeDef

```python
# AssignedEnvironmentEnterSessionActionDefinitionTypeDef definition

class AssignedEnvironmentEnterSessionActionDefinitionTypeDef(TypedDict):
    environmentId: str,
```

## AssignedEnvironmentExitSessionActionDefinitionTypeDef

```python
# AssignedEnvironmentExitSessionActionDefinitionTypeDef definition

class AssignedEnvironmentExitSessionActionDefinitionTypeDef(TypedDict):
    environmentId: str,
```

## AssignedSyncInputJobAttachmentsSessionActionDefinitionTypeDef

```python
# AssignedSyncInputJobAttachmentsSessionActionDefinitionTypeDef definition

class AssignedSyncInputJobAttachmentsSessionActionDefinitionTypeDef(TypedDict):
    stepId: NotRequired[str],
```

## LogConfigurationTypeDef

```python
# LogConfigurationTypeDef definition

class LogConfigurationTypeDef(TypedDict):
    logDriver: str,
    options: NotRequired[Dict[str, str]],
    parameters: NotRequired[Dict[str, str]],
    error: NotRequired[str],
```

## TaskParameterValueTypeDef

```python
# TaskParameterValueTypeDef definition

class TaskParameterValueTypeDef(TypedDict):
    int: NotRequired[str],
    float: NotRequired[str],
    string: NotRequired[str],
    path: NotRequired[str],
```

## AssociateMemberToFarmRequestRequestTypeDef

```python
# AssociateMemberToFarmRequestRequestTypeDef definition

class AssociateMemberToFarmRequestRequestTypeDef(TypedDict):
    farmId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 
## AssociateMemberToFleetRequestRequestTypeDef

```python
# AssociateMemberToFleetRequestRequestTypeDef definition

class AssociateMemberToFleetRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 
## AssociateMemberToJobRequestRequestTypeDef

```python
# AssociateMemberToJobRequestRequestTypeDef definition

class AssociateMemberToJobRequestRequestTypeDef(TypedDict):
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
## AssociateMemberToQueueRequestRequestTypeDef

```python
# AssociateMemberToQueueRequestRequestTypeDef definition

class AssociateMemberToQueueRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    principalId: str,
    principalType: PrincipalTypeType,  # (1)
    identityStoreId: str,
    membershipLevel: MembershipLevelType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: MembershipLevelType](./literals.md#membershipleveltype) 
## AssumeFleetRoleForReadRequestRequestTypeDef

```python
# AssumeFleetRoleForReadRequestRequestTypeDef definition

class AssumeFleetRoleForReadRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
```

## AwsCredentialsTypeDef

```python
# AwsCredentialsTypeDef definition

class AwsCredentialsTypeDef(TypedDict):
    accessKeyId: str,
    secretAccessKey: str,
    sessionToken: str,
    expiration: datetime,
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

## AssumeFleetRoleForWorkerRequestRequestTypeDef

```python
# AssumeFleetRoleForWorkerRequestRequestTypeDef definition

class AssumeFleetRoleForWorkerRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
```

## AssumeQueueRoleForReadRequestRequestTypeDef

```python
# AssumeQueueRoleForReadRequestRequestTypeDef definition

class AssumeQueueRoleForReadRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
```

## AssumeQueueRoleForUserRequestRequestTypeDef

```python
# AssumeQueueRoleForUserRequestRequestTypeDef definition

class AssumeQueueRoleForUserRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
```

## AssumeQueueRoleForWorkerRequestRequestTypeDef

```python
# AssumeQueueRoleForWorkerRequestRequestTypeDef definition

class AssumeQueueRoleForWorkerRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    queueId: str,
```

## ManifestPropertiesOutputTypeDef

```python
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
## BudgetActionToAddTypeDef

```python
# BudgetActionToAddTypeDef definition

class BudgetActionToAddTypeDef(TypedDict):
    type: BudgetActionTypeType,  # (1)
    thresholdPercentage: float,
    description: NotRequired[str],
```

1. See [:material-code-brackets: BudgetActionTypeType](./literals.md#budgetactiontypetype) 
## BudgetActionToRemoveTypeDef

```python
# BudgetActionToRemoveTypeDef definition

class BudgetActionToRemoveTypeDef(TypedDict):
    type: BudgetActionTypeType,  # (1)
    thresholdPercentage: float,
```

1. See [:material-code-brackets: BudgetActionTypeType](./literals.md#budgetactiontypetype) 
## FixedBudgetScheduleOutputTypeDef

```python
# FixedBudgetScheduleOutputTypeDef definition

class FixedBudgetScheduleOutputTypeDef(TypedDict):
    startTime: datetime,
    endTime: datetime,
```

## ConsumedUsagesTypeDef

```python
# ConsumedUsagesTypeDef definition

class ConsumedUsagesTypeDef(TypedDict):
    approximateDollarUsage: float,
```

## UsageTrackingResourceTypeDef

```python
# UsageTrackingResourceTypeDef definition

class UsageTrackingResourceTypeDef(TypedDict):
    queueId: NotRequired[str],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucketName: str,
    key: str,
```

## CreateFarmRequestRequestTypeDef

```python
# CreateFarmRequestRequestTypeDef definition

class CreateFarmRequestRequestTypeDef(TypedDict):
    displayName: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## JobParameterTypeDef

```python
# JobParameterTypeDef definition

class JobParameterTypeDef(TypedDict):
    int: NotRequired[str],
    float: NotRequired[str],
    string: NotRequired[str],
    path: NotRequired[str],
```

## CreateLicenseEndpointRequestRequestTypeDef

```python
# CreateLicenseEndpointRequestRequestTypeDef definition

class CreateLicenseEndpointRequestRequestTypeDef(TypedDict):
    vpcId: str,
    subnetIds: Sequence[str],
    securityGroupIds: Sequence[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateMonitorRequestRequestTypeDef

```python
# CreateMonitorRequestRequestTypeDef definition

class CreateMonitorRequestRequestTypeDef(TypedDict):
    displayName: str,
    identityCenterInstanceArn: str,
    subdomain: str,
    roleArn: str,
    clientToken: NotRequired[str],
```

## CreateQueueEnvironmentRequestRequestTypeDef

```python
# CreateQueueEnvironmentRequestRequestTypeDef definition

class CreateQueueEnvironmentRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    priority: int,
    templateType: EnvironmentTemplateTypeType,  # (1)
    template: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentTemplateTypeType](./literals.md#environmenttemplatetypetype) 
## CreateQueueFleetAssociationRequestRequestTypeDef

```python
# CreateQueueFleetAssociationRequestRequestTypeDef definition

class CreateQueueFleetAssociationRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    fleetId: str,
```

## JobAttachmentSettingsTypeDef

```python
# JobAttachmentSettingsTypeDef definition

class JobAttachmentSettingsTypeDef(TypedDict):
    s3BucketName: str,
    rootPrefix: str,
```

## FileSystemLocationTypeDef

```python
# FileSystemLocationTypeDef definition

class FileSystemLocationTypeDef(TypedDict):
    name: str,
    path: str,
    type: FileSystemLocationTypeType,  # (1)
```

1. See [:material-code-brackets: FileSystemLocationTypeType](./literals.md#filesystemlocationtypetype) 
## FleetAmountCapabilityTypeDef

```python
# FleetAmountCapabilityTypeDef definition

class FleetAmountCapabilityTypeDef(TypedDict):
    name: str,
    min: float,
    max: NotRequired[float],
```

## FleetAttributeCapabilityOutputTypeDef

```python
# FleetAttributeCapabilityOutputTypeDef definition

class FleetAttributeCapabilityOutputTypeDef(TypedDict):
    name: str,
    values: List[str],
```

## MemoryMiBRangeTypeDef

```python
# MemoryMiBRangeTypeDef definition

class MemoryMiBRangeTypeDef(TypedDict):
    min: int,
    max: NotRequired[int],
```

## VCpuCountRangeTypeDef

```python
# VCpuCountRangeTypeDef definition

class VCpuCountRangeTypeDef(TypedDict):
    min: int,
    max: NotRequired[int],
```

## DeleteBudgetRequestRequestTypeDef

```python
# DeleteBudgetRequestRequestTypeDef definition

class DeleteBudgetRequestRequestTypeDef(TypedDict):
    farmId: str,
    budgetId: str,
```

## DeleteFarmRequestRequestTypeDef

```python
# DeleteFarmRequestRequestTypeDef definition

class DeleteFarmRequestRequestTypeDef(TypedDict):
    farmId: str,
```

## DeleteFleetRequestRequestTypeDef

```python
# DeleteFleetRequestRequestTypeDef definition

class DeleteFleetRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    clientToken: NotRequired[str],
```

## DeleteLicenseEndpointRequestRequestTypeDef

```python
# DeleteLicenseEndpointRequestRequestTypeDef definition

class DeleteLicenseEndpointRequestRequestTypeDef(TypedDict):
    licenseEndpointId: str,
```

## DeleteMeteredProductRequestRequestTypeDef

```python
# DeleteMeteredProductRequestRequestTypeDef definition

class DeleteMeteredProductRequestRequestTypeDef(TypedDict):
    licenseEndpointId: str,
    productId: str,
```

## DeleteMonitorRequestRequestTypeDef

```python
# DeleteMonitorRequestRequestTypeDef definition

class DeleteMonitorRequestRequestTypeDef(TypedDict):
    monitorId: str,
```

## DeleteQueueEnvironmentRequestRequestTypeDef

```python
# DeleteQueueEnvironmentRequestRequestTypeDef definition

class DeleteQueueEnvironmentRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    queueEnvironmentId: str,
```

## DeleteQueueFleetAssociationRequestRequestTypeDef

```python
# DeleteQueueFleetAssociationRequestRequestTypeDef definition

class DeleteQueueFleetAssociationRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    fleetId: str,
```

## DeleteQueueRequestRequestTypeDef

```python
# DeleteQueueRequestRequestTypeDef definition

class DeleteQueueRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
```

## DeleteStorageProfileRequestRequestTypeDef

```python
# DeleteStorageProfileRequestRequestTypeDef definition

class DeleteStorageProfileRequestRequestTypeDef(TypedDict):
    farmId: str,
    storageProfileId: str,
```

## DeleteWorkerRequestRequestTypeDef

```python
# DeleteWorkerRequestRequestTypeDef definition

class DeleteWorkerRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
```

## DependencyCountsTypeDef

```python
# DependencyCountsTypeDef definition

class DependencyCountsTypeDef(TypedDict):
    dependenciesResolved: int,
    dependenciesUnresolved: int,
    consumersResolved: int,
    consumersUnresolved: int,
```

## DisassociateMemberFromFarmRequestRequestTypeDef

```python
# DisassociateMemberFromFarmRequestRequestTypeDef definition

class DisassociateMemberFromFarmRequestRequestTypeDef(TypedDict):
    farmId: str,
    principalId: str,
```

## DisassociateMemberFromFleetRequestRequestTypeDef

```python
# DisassociateMemberFromFleetRequestRequestTypeDef definition

class DisassociateMemberFromFleetRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    principalId: str,
```

## DisassociateMemberFromJobRequestRequestTypeDef

```python
# DisassociateMemberFromJobRequestRequestTypeDef definition

class DisassociateMemberFromJobRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    principalId: str,
```

## DisassociateMemberFromQueueRequestRequestTypeDef

```python
# DisassociateMemberFromQueueRequestRequestTypeDef definition

class DisassociateMemberFromQueueRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    principalId: str,
```

## Ec2EbsVolumeTypeDef

```python
# Ec2EbsVolumeTypeDef definition

class Ec2EbsVolumeTypeDef(TypedDict):
    sizeGiB: NotRequired[int],
    iops: NotRequired[int],
    throughputMiB: NotRequired[int],
```

## EnvironmentDetailsEntityTypeDef

```python
# EnvironmentDetailsEntityTypeDef definition

class EnvironmentDetailsEntityTypeDef(TypedDict):
    jobId: str,
    environmentId: str,
    schemaVersion: str,
    template: Dict[str, Any],
```

## EnvironmentDetailsErrorTypeDef

```python
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
# EnvironmentDetailsIdentifiersTypeDef definition

class EnvironmentDetailsIdentifiersTypeDef(TypedDict):
    jobId: str,
    environmentId: str,
```

## EnvironmentEnterSessionActionDefinitionSummaryTypeDef

```python
# EnvironmentEnterSessionActionDefinitionSummaryTypeDef definition

class EnvironmentEnterSessionActionDefinitionSummaryTypeDef(TypedDict):
    environmentId: str,
```

## EnvironmentEnterSessionActionDefinitionTypeDef

```python
# EnvironmentEnterSessionActionDefinitionTypeDef definition

class EnvironmentEnterSessionActionDefinitionTypeDef(TypedDict):
    environmentId: str,
```

## EnvironmentExitSessionActionDefinitionSummaryTypeDef

```python
# EnvironmentExitSessionActionDefinitionSummaryTypeDef definition

class EnvironmentExitSessionActionDefinitionSummaryTypeDef(TypedDict):
    environmentId: str,
```

## EnvironmentExitSessionActionDefinitionTypeDef

```python
# EnvironmentExitSessionActionDefinitionTypeDef definition

class EnvironmentExitSessionActionDefinitionTypeDef(TypedDict):
    environmentId: str,
```

## FarmMemberTypeDef

```python
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
# FieldSortExpressionTypeDef definition

class FieldSortExpressionTypeDef(TypedDict):
    sortOrder: SortOrderType,  # (1)
    name: str,
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## FleetAttributeCapabilityTypeDef

```python
# FleetAttributeCapabilityTypeDef definition

class FleetAttributeCapabilityTypeDef(TypedDict):
    name: str,
    values: Sequence[str],
```

## FleetMemberTypeDef

```python
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
## GetBudgetRequestRequestTypeDef

```python
# GetBudgetRequestRequestTypeDef definition

class GetBudgetRequestRequestTypeDef(TypedDict):
    farmId: str,
    budgetId: str,
```

## ResponseBudgetActionTypeDef

```python
# ResponseBudgetActionTypeDef definition

class ResponseBudgetActionTypeDef(TypedDict):
    type: BudgetActionTypeType,  # (1)
    thresholdPercentage: float,
    description: NotRequired[str],
```

1. See [:material-code-brackets: BudgetActionTypeType](./literals.md#budgetactiontypetype) 
## GetFarmRequestRequestTypeDef

```python
# GetFarmRequestRequestTypeDef definition

class GetFarmRequestRequestTypeDef(TypedDict):
    farmId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetFleetRequestRequestTypeDef

```python
# GetFleetRequestRequestTypeDef definition

class GetFleetRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
```

## JobAttachmentDetailsErrorTypeDef

```python
# JobAttachmentDetailsErrorTypeDef definition

class JobAttachmentDetailsErrorTypeDef(TypedDict):
    jobId: str,
    code: JobEntityErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: JobEntityErrorCodeType](./literals.md#jobentityerrorcodetype) 
## JobDetailsErrorTypeDef

```python
# JobDetailsErrorTypeDef definition

class JobDetailsErrorTypeDef(TypedDict):
    jobId: str,
    code: JobEntityErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: JobEntityErrorCodeType](./literals.md#jobentityerrorcodetype) 
## StepDetailsErrorTypeDef

```python
# StepDetailsErrorTypeDef definition

class StepDetailsErrorTypeDef(TypedDict):
    jobId: str,
    stepId: str,
    code: JobEntityErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: JobEntityErrorCodeType](./literals.md#jobentityerrorcodetype) 
## GetJobRequestRequestTypeDef

```python
# GetJobRequestRequestTypeDef definition

class GetJobRequestRequestTypeDef(TypedDict):
    farmId: str,
    jobId: str,
    queueId: str,
```

## GetLicenseEndpointRequestRequestTypeDef

```python
# GetLicenseEndpointRequestRequestTypeDef definition

class GetLicenseEndpointRequestRequestTypeDef(TypedDict):
    licenseEndpointId: str,
```

## GetMonitorRequestRequestTypeDef

```python
# GetMonitorRequestRequestTypeDef definition

class GetMonitorRequestRequestTypeDef(TypedDict):
    monitorId: str,
```

## GetQueueEnvironmentRequestRequestTypeDef

```python
# GetQueueEnvironmentRequestRequestTypeDef definition

class GetQueueEnvironmentRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    queueEnvironmentId: str,
```

## GetQueueFleetAssociationRequestRequestTypeDef

```python
# GetQueueFleetAssociationRequestRequestTypeDef definition

class GetQueueFleetAssociationRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    fleetId: str,
```

## GetQueueRequestRequestTypeDef

```python
# GetQueueRequestRequestTypeDef definition

class GetQueueRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
```

## GetSessionActionRequestRequestTypeDef

```python
# GetSessionActionRequestRequestTypeDef definition

class GetSessionActionRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    sessionActionId: str,
```

## GetSessionRequestRequestTypeDef

```python
# GetSessionRequestRequestTypeDef definition

class GetSessionRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    sessionId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetSessionsStatisticsAggregationRequestRequestTypeDef

```python
# GetSessionsStatisticsAggregationRequestRequestTypeDef definition

class GetSessionsStatisticsAggregationRequestRequestTypeDef(TypedDict):
    farmId: str,
    aggregationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetStepRequestRequestTypeDef

```python
# GetStepRequestRequestTypeDef definition

class GetStepRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
```

## GetStorageProfileForQueueRequestRequestTypeDef

```python
# GetStorageProfileForQueueRequestRequestTypeDef definition

class GetStorageProfileForQueueRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    storageProfileId: str,
```

## GetStorageProfileRequestRequestTypeDef

```python
# GetStorageProfileRequestRequestTypeDef definition

class GetStorageProfileRequestRequestTypeDef(TypedDict):
    farmId: str,
    storageProfileId: str,
```

## GetTaskRequestRequestTypeDef

```python
# GetTaskRequestRequestTypeDef definition

class GetTaskRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    taskId: str,
```

## GetWorkerRequestRequestTypeDef

```python
# GetWorkerRequestRequestTypeDef definition

class GetWorkerRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
```

## IpAddressesOutputTypeDef

```python
# IpAddressesOutputTypeDef definition

class IpAddressesOutputTypeDef(TypedDict):
    ipV4Addresses: NotRequired[List[str]],
    ipV6Addresses: NotRequired[List[str]],
```

## IpAddressesTypeDef

```python
# IpAddressesTypeDef definition

class IpAddressesTypeDef(TypedDict):
    ipV4Addresses: NotRequired[Sequence[str]],
    ipV6Addresses: NotRequired[Sequence[str]],
```

## JobAttachmentDetailsIdentifiersTypeDef

```python
# JobAttachmentDetailsIdentifiersTypeDef definition

class JobAttachmentDetailsIdentifiersTypeDef(TypedDict):
    jobId: str,
```

## PathMappingRuleTypeDef

```python
# PathMappingRuleTypeDef definition

class PathMappingRuleTypeDef(TypedDict):
    sourcePathFormat: PathFormatType,  # (1)
    sourcePath: str,
    destinationPath: str,
```

1. See [:material-code-brackets: PathFormatType](./literals.md#pathformattype) 
## JobDetailsIdentifiersTypeDef

```python
# JobDetailsIdentifiersTypeDef definition

class JobDetailsIdentifiersTypeDef(TypedDict):
    jobId: str,
```

## StepDetailsIdentifiersTypeDef

```python
# StepDetailsIdentifiersTypeDef definition

class StepDetailsIdentifiersTypeDef(TypedDict):
    jobId: str,
    stepId: str,
```

## StepDetailsEntityTypeDef

```python
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
# PosixUserTypeDef definition

class PosixUserTypeDef(TypedDict):
    user: str,
    group: str,
```

## WindowsUserTypeDef

```python
# WindowsUserTypeDef definition

class WindowsUserTypeDef(TypedDict):
    user: str,
    passwordArn: str,
```

## JobSummaryTypeDef

```python
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
    sourceJobId: NotRequired[str],
```

1. See [:material-code-brackets: JobLifecycleStatusType](./literals.md#joblifecyclestatustype) 
2. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
3. See [:material-code-brackets: JobTargetTaskRunStatusType](./literals.md#jobtargettaskrunstatustype) 
4. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
## LicenseEndpointSummaryTypeDef

```python
# LicenseEndpointSummaryTypeDef definition

class LicenseEndpointSummaryTypeDef(TypedDict):
    licenseEndpointId: NotRequired[str],
    status: NotRequired[LicenseEndpointStatusType],  # (1)
    statusMessage: NotRequired[str],
    vpcId: NotRequired[str],
```

1. See [:material-code-brackets: LicenseEndpointStatusType](./literals.md#licenseendpointstatustype) 
## ListAvailableMeteredProductsRequestRequestTypeDef

```python
# ListAvailableMeteredProductsRequestRequestTypeDef definition

class ListAvailableMeteredProductsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## MeteredProductSummaryTypeDef

```python
# MeteredProductSummaryTypeDef definition

class MeteredProductSummaryTypeDef(TypedDict):
    productId: str,
    family: str,
    vendor: str,
    port: int,
```

## ListBudgetsRequestRequestTypeDef

```python
# ListBudgetsRequestRequestTypeDef definition

class ListBudgetsRequestRequestTypeDef(TypedDict):
    farmId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    status: NotRequired[BudgetStatusType],  # (1)
```

1. See [:material-code-brackets: BudgetStatusType](./literals.md#budgetstatustype) 
## ListFarmMembersRequestRequestTypeDef

```python
# ListFarmMembersRequestRequestTypeDef definition

class ListFarmMembersRequestRequestTypeDef(TypedDict):
    farmId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListFarmsRequestRequestTypeDef

```python
# ListFarmsRequestRequestTypeDef definition

class ListFarmsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    principalId: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListFleetMembersRequestRequestTypeDef

```python
# ListFleetMembersRequestRequestTypeDef definition

class ListFleetMembersRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListFleetsRequestRequestTypeDef

```python
# ListFleetsRequestRequestTypeDef definition

class ListFleetsRequestRequestTypeDef(TypedDict):
    farmId: str,
    principalId: NotRequired[str],
    displayName: NotRequired[str],
    status: NotRequired[FleetStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: FleetStatusType](./literals.md#fleetstatustype) 
## ListJobMembersRequestRequestTypeDef

```python
# ListJobMembersRequestRequestTypeDef definition

class ListJobMembersRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListJobParameterDefinitionsRequestRequestTypeDef

```python
# ListJobParameterDefinitionsRequestRequestTypeDef definition

class ListJobParameterDefinitionsRequestRequestTypeDef(TypedDict):
    farmId: str,
    jobId: str,
    queueId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListJobsRequestRequestTypeDef

```python
# ListJobsRequestRequestTypeDef definition

class ListJobsRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    principalId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListLicenseEndpointsRequestRequestTypeDef

```python
# ListLicenseEndpointsRequestRequestTypeDef definition

class ListLicenseEndpointsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMeteredProductsRequestRequestTypeDef

```python
# ListMeteredProductsRequestRequestTypeDef definition

class ListMeteredProductsRequestRequestTypeDef(TypedDict):
    licenseEndpointId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMonitorsRequestRequestTypeDef

```python
# ListMonitorsRequestRequestTypeDef definition

class ListMonitorsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## MonitorSummaryTypeDef

```python
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

## ListQueueEnvironmentsRequestRequestTypeDef

```python
# ListQueueEnvironmentsRequestRequestTypeDef definition

class ListQueueEnvironmentsRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## QueueEnvironmentSummaryTypeDef

```python
# QueueEnvironmentSummaryTypeDef definition

class QueueEnvironmentSummaryTypeDef(TypedDict):
    queueEnvironmentId: str,
    name: str,
    priority: int,
```

## ListQueueFleetAssociationsRequestRequestTypeDef

```python
# ListQueueFleetAssociationsRequestRequestTypeDef definition

class ListQueueFleetAssociationsRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: NotRequired[str],
    fleetId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## QueueFleetAssociationSummaryTypeDef

```python
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
## ListQueueMembersRequestRequestTypeDef

```python
# ListQueueMembersRequestRequestTypeDef definition

class ListQueueMembersRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## QueueMemberTypeDef

```python
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
## ListQueuesRequestRequestTypeDef

```python
# ListQueuesRequestRequestTypeDef definition

class ListQueuesRequestRequestTypeDef(TypedDict):
    farmId: str,
    principalId: NotRequired[str],
    status: NotRequired[QueueStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
## QueueSummaryTypeDef

```python
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
## ListSessionActionsRequestRequestTypeDef

```python
# ListSessionActionsRequestRequestTypeDef definition

class ListSessionActionsRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    sessionId: NotRequired[str],
    taskId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListSessionsForWorkerRequestRequestTypeDef

```python
# ListSessionsForWorkerRequestRequestTypeDef definition

class ListSessionsForWorkerRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## WorkerSessionSummaryTypeDef

```python
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
## ListSessionsRequestRequestTypeDef

```python
# ListSessionsRequestRequestTypeDef definition

class ListSessionsRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## SessionSummaryTypeDef

```python
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
## ListStepConsumersRequestRequestTypeDef

```python
# ListStepConsumersRequestRequestTypeDef definition

class ListStepConsumersRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StepConsumerTypeDef

```python
# StepConsumerTypeDef definition

class StepConsumerTypeDef(TypedDict):
    stepId: str,
    status: DependencyConsumerResolutionStatusType,  # (1)
```

1. See [:material-code-brackets: DependencyConsumerResolutionStatusType](./literals.md#dependencyconsumerresolutionstatustype) 
## ListStepDependenciesRequestRequestTypeDef

```python
# ListStepDependenciesRequestRequestTypeDef definition

class ListStepDependenciesRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StepDependencyTypeDef

```python
# StepDependencyTypeDef definition

class StepDependencyTypeDef(TypedDict):
    stepId: str,
    status: DependencyConsumerResolutionStatusType,  # (1)
```

1. See [:material-code-brackets: DependencyConsumerResolutionStatusType](./literals.md#dependencyconsumerresolutionstatustype) 
## ListStepsRequestRequestTypeDef

```python
# ListStepsRequestRequestTypeDef definition

class ListStepsRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListStorageProfilesForQueueRequestRequestTypeDef

```python
# ListStorageProfilesForQueueRequestRequestTypeDef definition

class ListStorageProfilesForQueueRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StorageProfileSummaryTypeDef

```python
# StorageProfileSummaryTypeDef definition

class StorageProfileSummaryTypeDef(TypedDict):
    storageProfileId: str,
    displayName: str,
    osFamily: StorageProfileOperatingSystemFamilyType,  # (1)
```

1. See [:material-code-brackets: StorageProfileOperatingSystemFamilyType](./literals.md#storageprofileoperatingsystemfamilytype) 
## ListStorageProfilesRequestRequestTypeDef

```python
# ListStorageProfilesRequestRequestTypeDef definition

class ListStorageProfilesRequestRequestTypeDef(TypedDict):
    farmId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTasksRequestRequestTypeDef

```python
# ListTasksRequestRequestTypeDef definition

class ListTasksRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListWorkersRequestRequestTypeDef

```python
# ListWorkersRequestRequestTypeDef definition

class ListWorkersRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ManifestPropertiesTypeDef

```python
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
## ParameterFilterExpressionTypeDef

```python
# ParameterFilterExpressionTypeDef definition

class ParameterFilterExpressionTypeDef(TypedDict):
    name: str,
    operator: ComparisonOperatorType,  # (1)
    value: str,
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## ParameterSortExpressionTypeDef

```python
# ParameterSortExpressionTypeDef definition

class ParameterSortExpressionTypeDef(TypedDict):
    sortOrder: SortOrderType,  # (1)
    name: str,
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## StepParameterTypeDef

```python
# StepParameterTypeDef definition

class StepParameterTypeDef(TypedDict):
    name: str,
    type: StepParameterTypeType,  # (1)
```

1. See [:material-code-brackets: StepParameterTypeType](./literals.md#stepparametertypetype) 
## PutMeteredProductRequestRequestTypeDef

```python
# PutMeteredProductRequestRequestTypeDef definition

class PutMeteredProductRequestRequestTypeDef(TypedDict):
    licenseEndpointId: str,
    productId: str,
```

## SearchTermFilterExpressionTypeDef

```python
# SearchTermFilterExpressionTypeDef definition

class SearchTermFilterExpressionTypeDef(TypedDict):
    searchTerm: str,
```

## StringFilterExpressionTypeDef

```python
# StringFilterExpressionTypeDef definition

class StringFilterExpressionTypeDef(TypedDict):
    name: str,
    operator: ComparisonOperatorType,  # (1)
    value: str,
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## UserJobsFirstTypeDef

```python
# UserJobsFirstTypeDef definition

class UserJobsFirstTypeDef(TypedDict):
    userIdentityId: str,
```

## ServiceManagedEc2InstanceMarketOptionsTypeDef

```python
# ServiceManagedEc2InstanceMarketOptionsTypeDef definition

class ServiceManagedEc2InstanceMarketOptionsTypeDef(TypedDict):
    type: Ec2MarketTypeType,  # (1)
```

1. See [:material-code-brackets: Ec2MarketTypeType](./literals.md#ec2markettypetype) 
## SyncInputJobAttachmentsSessionActionDefinitionSummaryTypeDef

```python
# SyncInputJobAttachmentsSessionActionDefinitionSummaryTypeDef definition

class SyncInputJobAttachmentsSessionActionDefinitionSummaryTypeDef(TypedDict):
    stepId: NotRequired[str],
```

## TaskRunSessionActionDefinitionSummaryTypeDef

```python
# TaskRunSessionActionDefinitionSummaryTypeDef definition

class TaskRunSessionActionDefinitionSummaryTypeDef(TypedDict):
    taskId: str,
    stepId: str,
```

## SyncInputJobAttachmentsSessionActionDefinitionTypeDef

```python
# SyncInputJobAttachmentsSessionActionDefinitionTypeDef definition

class SyncInputJobAttachmentsSessionActionDefinitionTypeDef(TypedDict):
    stepId: NotRequired[str],
```

## SessionsStatisticsResourcesTypeDef

```python
# SessionsStatisticsResourcesTypeDef definition

class SessionsStatisticsResourcesTypeDef(TypedDict):
    queueIds: NotRequired[Sequence[str]],
    fleetIds: NotRequired[Sequence[str]],
```

## StatsTypeDef

```python
# StatsTypeDef definition

class StatsTypeDef(TypedDict):
    min: NotRequired[float],
    max: NotRequired[float],
    avg: NotRequired[float],
    sum: NotRequired[float],
```

## StepAmountCapabilityTypeDef

```python
# StepAmountCapabilityTypeDef definition

class StepAmountCapabilityTypeDef(TypedDict):
    name: str,
    min: NotRequired[float],
    max: NotRequired[float],
    value: NotRequired[float],
```

## StepAttributeCapabilityTypeDef

```python
# StepAttributeCapabilityTypeDef definition

class StepAttributeCapabilityTypeDef(TypedDict):
    name: str,
    anyOf: NotRequired[List[str]],
    allOf: NotRequired[List[str]],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: NotRequired[Mapping[str, str]],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateFarmRequestRequestTypeDef

```python
# UpdateFarmRequestRequestTypeDef definition

class UpdateFarmRequestRequestTypeDef(TypedDict):
    farmId: str,
    displayName: NotRequired[str],
    description: NotRequired[str],
```

## UpdateJobRequestRequestTypeDef

```python
# UpdateJobRequestRequestTypeDef definition

class UpdateJobRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    clientToken: NotRequired[str],
    targetTaskRunStatus: NotRequired[JobTargetTaskRunStatusType],  # (1)
    priority: NotRequired[int],
    maxFailedTasksCount: NotRequired[int],
    maxRetriesPerTask: NotRequired[int],
    lifecycleStatus: NotRequired[UpdateJobLifecycleStatusType],  # (2)
```

1. See [:material-code-brackets: JobTargetTaskRunStatusType](./literals.md#jobtargettaskrunstatustype) 
2. See [:material-code-brackets: UpdateJobLifecycleStatusType](./literals.md#updatejoblifecyclestatustype) 
## UpdateMonitorRequestRequestTypeDef

```python
# UpdateMonitorRequestRequestTypeDef definition

class UpdateMonitorRequestRequestTypeDef(TypedDict):
    monitorId: str,
    subdomain: NotRequired[str],
    displayName: NotRequired[str],
    roleArn: NotRequired[str],
```

## UpdateQueueEnvironmentRequestRequestTypeDef

```python
# UpdateQueueEnvironmentRequestRequestTypeDef definition

class UpdateQueueEnvironmentRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    queueEnvironmentId: str,
    clientToken: NotRequired[str],
    priority: NotRequired[int],
    templateType: NotRequired[EnvironmentTemplateTypeType],  # (1)
    template: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentTemplateTypeType](./literals.md#environmenttemplatetypetype) 
## UpdateQueueFleetAssociationRequestRequestTypeDef

```python
# UpdateQueueFleetAssociationRequestRequestTypeDef definition

class UpdateQueueFleetAssociationRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    fleetId: str,
    status: UpdateQueueFleetAssociationStatusType,  # (1)
```

1. See [:material-code-brackets: UpdateQueueFleetAssociationStatusType](./literals.md#updatequeuefleetassociationstatustype) 
## UpdateSessionRequestRequestTypeDef

```python
# UpdateSessionRequestRequestTypeDef definition

class UpdateSessionRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    sessionId: str,
    targetLifecycleStatus: SessionLifecycleTargetStatusType,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: SessionLifecycleTargetStatusType](./literals.md#sessionlifecycletargetstatustype) 
## UpdateStepRequestRequestTypeDef

```python
# UpdateStepRequestRequestTypeDef definition

class UpdateStepRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    targetTaskRunStatus: StepTargetTaskRunStatusType,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: StepTargetTaskRunStatusType](./literals.md#steptargettaskrunstatustype) 
## UpdateTaskRequestRequestTypeDef

```python
# UpdateTaskRequestRequestTypeDef definition

class UpdateTaskRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    taskId: str,
    targetRunStatus: TaskTargetRunStatusType,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: TaskTargetRunStatusType](./literals.md#tasktargetrunstatustype) 
## WorkerAmountCapabilityTypeDef

```python
# WorkerAmountCapabilityTypeDef definition

class WorkerAmountCapabilityTypeDef(TypedDict):
    name: str,
    value: float,
```

## WorkerAttributeCapabilityTypeDef

```python
# WorkerAttributeCapabilityTypeDef definition

class WorkerAttributeCapabilityTypeDef(TypedDict):
    name: str,
    values: Sequence[str],
```

## AssignedTaskRunSessionActionDefinitionTypeDef

```python
# AssignedTaskRunSessionActionDefinitionTypeDef definition

class AssignedTaskRunSessionActionDefinitionTypeDef(TypedDict):
    taskId: str,
    stepId: str,
    parameters: Dict[str, TaskParameterValueTypeDef],  # (1)
```

1. See [:material-code-braces: TaskParameterValueTypeDef](./type_defs.md#taskparametervaluetypedef) 
## TaskRunSessionActionDefinitionTypeDef

```python
# TaskRunSessionActionDefinitionTypeDef definition

class TaskRunSessionActionDefinitionTypeDef(TypedDict):
    taskId: str,
    stepId: str,
    parameters: Dict[str, TaskParameterValueTypeDef],  # (1)
```

1. See [:material-code-braces: TaskParameterValueTypeDef](./type_defs.md#taskparametervaluetypedef) 
## TaskSearchSummaryTypeDef

```python
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
# AssumeFleetRoleForReadResponseTypeDef definition

class AssumeFleetRoleForReadResponseTypeDef(TypedDict):
    credentials: AwsCredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssumeFleetRoleForWorkerResponseTypeDef

```python
# AssumeFleetRoleForWorkerResponseTypeDef definition

class AssumeFleetRoleForWorkerResponseTypeDef(TypedDict):
    credentials: AwsCredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssumeQueueRoleForReadResponseTypeDef

```python
# AssumeQueueRoleForReadResponseTypeDef definition

class AssumeQueueRoleForReadResponseTypeDef(TypedDict):
    credentials: AwsCredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssumeQueueRoleForUserResponseTypeDef

```python
# AssumeQueueRoleForUserResponseTypeDef definition

class AssumeQueueRoleForUserResponseTypeDef(TypedDict):
    credentials: AwsCredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssumeQueueRoleForWorkerResponseTypeDef

```python
# AssumeQueueRoleForWorkerResponseTypeDef definition

class AssumeQueueRoleForWorkerResponseTypeDef(TypedDict):
    credentials: AwsCredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyJobTemplateResponseTypeDef

```python
# CopyJobTemplateResponseTypeDef definition

class CopyJobTemplateResponseTypeDef(TypedDict):
    templateType: JobTemplateTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobTemplateTypeType](./literals.md#jobtemplatetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBudgetResponseTypeDef

```python
# CreateBudgetResponseTypeDef definition

class CreateBudgetResponseTypeDef(TypedDict):
    budgetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFarmResponseTypeDef

```python
# CreateFarmResponseTypeDef definition

class CreateFarmResponseTypeDef(TypedDict):
    farmId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetResponseTypeDef

```python
# CreateFleetResponseTypeDef definition

class CreateFleetResponseTypeDef(TypedDict):
    fleetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobResponseTypeDef

```python
# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLicenseEndpointResponseTypeDef

```python
# CreateLicenseEndpointResponseTypeDef definition

class CreateLicenseEndpointResponseTypeDef(TypedDict):
    licenseEndpointId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMonitorResponseTypeDef

```python
# CreateMonitorResponseTypeDef definition

class CreateMonitorResponseTypeDef(TypedDict):
    monitorId: str,
    identityCenterApplicationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQueueEnvironmentResponseTypeDef

```python
# CreateQueueEnvironmentResponseTypeDef definition

class CreateQueueEnvironmentResponseTypeDef(TypedDict):
    queueEnvironmentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQueueResponseTypeDef

```python
# CreateQueueResponseTypeDef definition

class CreateQueueResponseTypeDef(TypedDict):
    queueId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStorageProfileResponseTypeDef

```python
# CreateStorageProfileResponseTypeDef definition

class CreateStorageProfileResponseTypeDef(TypedDict):
    storageProfileId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkerResponseTypeDef

```python
# CreateWorkerResponseTypeDef definition

class CreateWorkerResponseTypeDef(TypedDict):
    workerId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFarmResponseTypeDef

```python
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
## GetMonitorResponseTypeDef

```python
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
## GetTaskResponseTypeDef

```python
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
# ListJobParameterDefinitionsResponseTypeDef definition

class ListJobParameterDefinitionsResponseTypeDef(TypedDict):
    jobParameterDefinitions: List[Dict[str, Any]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
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
## StartSessionsStatisticsAggregationResponseTypeDef

```python
# StartSessionsStatisticsAggregationResponseTypeDef definition

class StartSessionsStatisticsAggregationResponseTypeDef(TypedDict):
    aggregationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkerResponseTypeDef

```python
# UpdateWorkerResponseTypeDef definition

class UpdateWorkerResponseTypeDef(TypedDict):
    log: LogConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachmentsOutputTypeDef

```python
# AttachmentsOutputTypeDef definition

class AttachmentsOutputTypeDef(TypedDict):
    manifests: List[ManifestPropertiesOutputTypeDef],  # (1)
    fileSystem: NotRequired[JobAttachmentsFileSystemType],  # (2)
```

1. See [:material-code-braces: ManifestPropertiesOutputTypeDef](./type_defs.md#manifestpropertiesoutputtypedef) 
2. See [:material-code-brackets: JobAttachmentsFileSystemType](./literals.md#jobattachmentsfilesystemtype) 
## BudgetScheduleOutputTypeDef

```python
# BudgetScheduleOutputTypeDef definition

class BudgetScheduleOutputTypeDef(TypedDict):
    fixed: NotRequired[FixedBudgetScheduleOutputTypeDef],  # (1)
```

1. See [:material-code-braces: FixedBudgetScheduleOutputTypeDef](./type_defs.md#fixedbudgetscheduleoutputtypedef) 
## BudgetSummaryTypeDef

```python
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
## CopyJobTemplateRequestRequestTypeDef

```python
# CopyJobTemplateRequestRequestTypeDef definition

class CopyJobTemplateRequestRequestTypeDef(TypedDict):
    farmId: str,
    jobId: str,
    queueId: str,
    targetS3Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## JobSearchSummaryTypeDef

```python
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
    sourceJobId: NotRequired[str],
```

1. See [:material-code-brackets: JobLifecycleStatusType](./literals.md#joblifecyclestatustype) 
2. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
3. See [:material-code-brackets: JobTargetTaskRunStatusType](./literals.md#jobtargettaskrunstatustype) 
4. See [:material-code-brackets: TaskRunStatusType](./literals.md#taskrunstatustype) 
5. See [:material-code-braces: JobParameterTypeDef](./type_defs.md#jobparametertypedef) 
## CreateStorageProfileRequestRequestTypeDef

```python
# CreateStorageProfileRequestRequestTypeDef definition

class CreateStorageProfileRequestRequestTypeDef(TypedDict):
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
## UpdateStorageProfileRequestRequestTypeDef

```python
# UpdateStorageProfileRequestRequestTypeDef definition

class UpdateStorageProfileRequestRequestTypeDef(TypedDict):
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
# FleetCapabilitiesTypeDef definition

class FleetCapabilitiesTypeDef(TypedDict):
    amounts: NotRequired[List[FleetAmountCapabilityTypeDef]],  # (1)
    attributes: NotRequired[List[FleetAttributeCapabilityOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: FleetAmountCapabilityTypeDef](./type_defs.md#fleetamountcapabilitytypedef) 
2. See [:material-code-braces: FleetAttributeCapabilityOutputTypeDef](./type_defs.md#fleetattributecapabilityoutputtypedef) 
## CustomerManagedWorkerCapabilitiesOutputTypeDef

```python
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
## DateTimeFilterExpressionTypeDef

```python
# DateTimeFilterExpressionTypeDef definition

class DateTimeFilterExpressionTypeDef(TypedDict):
    name: str,
    operator: ComparisonOperatorType,  # (1)
    dateTime: TimestampTypeDef,
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## FixedBudgetScheduleTypeDef

```python
# FixedBudgetScheduleTypeDef definition

class FixedBudgetScheduleTypeDef(TypedDict):
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
```

## UpdatedSessionActionInfoTypeDef

```python
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
## ServiceManagedEc2InstanceCapabilitiesOutputTypeDef

```python
# ServiceManagedEc2InstanceCapabilitiesOutputTypeDef definition

class ServiceManagedEc2InstanceCapabilitiesOutputTypeDef(TypedDict):
    vCpuCount: VCpuCountRangeTypeDef,  # (1)
    memoryMiB: MemoryMiBRangeTypeDef,  # (2)
    osFamily: ServiceManagedFleetOperatingSystemFamilyType,  # (3)
    cpuArchitectureType: CpuArchitectureTypeType,  # (4)
    rootEbsVolume: NotRequired[Ec2EbsVolumeTypeDef],  # (5)
    allowedInstanceTypes: NotRequired[List[str]],
    excludedInstanceTypes: NotRequired[List[str]],
    customAmounts: NotRequired[List[FleetAmountCapabilityTypeDef]],  # (6)
    customAttributes: NotRequired[List[FleetAttributeCapabilityOutputTypeDef]],  # (7)
```

1. See [:material-code-braces: VCpuCountRangeTypeDef](./type_defs.md#vcpucountrangetypedef) 
2. See [:material-code-braces: MemoryMiBRangeTypeDef](./type_defs.md#memorymibrangetypedef) 
3. See [:material-code-brackets: ServiceManagedFleetOperatingSystemFamilyType](./literals.md#servicemanagedfleetoperatingsystemfamilytype) 
4. See [:material-code-brackets: CpuArchitectureTypeType](./literals.md#cpuarchitecturetypetype) 
5. See [:material-code-braces: Ec2EbsVolumeTypeDef](./type_defs.md#ec2ebsvolumetypedef) 
6. See [:material-code-braces: FleetAmountCapabilityTypeDef](./type_defs.md#fleetamountcapabilitytypedef) 
7. See [:material-code-braces: FleetAttributeCapabilityOutputTypeDef](./type_defs.md#fleetattributecapabilityoutputtypedef) 
## ListFarmMembersResponseTypeDef

```python
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
# ListFarmsResponseTypeDef definition

class ListFarmsResponseTypeDef(TypedDict):
    farms: List[FarmSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FarmSummaryTypeDef](./type_defs.md#farmsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceManagedEc2InstanceCapabilitiesTypeDef

```python
# ServiceManagedEc2InstanceCapabilitiesTypeDef definition

class ServiceManagedEc2InstanceCapabilitiesTypeDef(TypedDict):
    vCpuCount: VCpuCountRangeTypeDef,  # (1)
    memoryMiB: MemoryMiBRangeTypeDef,  # (2)
    osFamily: ServiceManagedFleetOperatingSystemFamilyType,  # (3)
    cpuArchitectureType: CpuArchitectureTypeType,  # (4)
    rootEbsVolume: NotRequired[Ec2EbsVolumeTypeDef],  # (5)
    allowedInstanceTypes: NotRequired[Sequence[str]],
    excludedInstanceTypes: NotRequired[Sequence[str]],
    customAmounts: NotRequired[Sequence[FleetAmountCapabilityTypeDef]],  # (6)
    customAttributes: NotRequired[Sequence[FleetAttributeCapabilityTypeDef]],  # (7)
```

1. See [:material-code-braces: VCpuCountRangeTypeDef](./type_defs.md#vcpucountrangetypedef) 
2. See [:material-code-braces: MemoryMiBRangeTypeDef](./type_defs.md#memorymibrangetypedef) 
3. See [:material-code-brackets: ServiceManagedFleetOperatingSystemFamilyType](./literals.md#servicemanagedfleetoperatingsystemfamilytype) 
4. See [:material-code-brackets: CpuArchitectureTypeType](./literals.md#cpuarchitecturetypetype) 
5. See [:material-code-braces: Ec2EbsVolumeTypeDef](./type_defs.md#ec2ebsvolumetypedef) 
6. See [:material-code-braces: FleetAmountCapabilityTypeDef](./type_defs.md#fleetamountcapabilitytypedef) 
7. See [:material-code-braces: FleetAttributeCapabilityTypeDef](./type_defs.md#fleetattributecapabilitytypedef) 
## ListFleetMembersResponseTypeDef

```python
# ListFleetMembersResponseTypeDef definition

class ListFleetMembersResponseTypeDef(TypedDict):
    members: List[FleetMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetMemberTypeDef](./type_defs.md#fleetmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFleetRequestFleetActiveWaitTypeDef

```python
# GetFleetRequestFleetActiveWaitTypeDef definition

class GetFleetRequestFleetActiveWaitTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetJobRequestJobCreateCompleteWaitTypeDef

```python
# GetJobRequestJobCreateCompleteWaitTypeDef definition

class GetJobRequestJobCreateCompleteWaitTypeDef(TypedDict):
    farmId: str,
    jobId: str,
    queueId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetLicenseEndpointRequestLicenseEndpointDeletedWaitTypeDef

```python
# GetLicenseEndpointRequestLicenseEndpointDeletedWaitTypeDef definition

class GetLicenseEndpointRequestLicenseEndpointDeletedWaitTypeDef(TypedDict):
    licenseEndpointId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetLicenseEndpointRequestLicenseEndpointValidWaitTypeDef

```python
# GetLicenseEndpointRequestLicenseEndpointValidWaitTypeDef definition

class GetLicenseEndpointRequestLicenseEndpointValidWaitTypeDef(TypedDict):
    licenseEndpointId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetQueueFleetAssociationRequestQueueFleetAssociationStoppedWaitTypeDef

```python
# GetQueueFleetAssociationRequestQueueFleetAssociationStoppedWaitTypeDef definition

class GetQueueFleetAssociationRequestQueueFleetAssociationStoppedWaitTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    fleetId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetQueueRequestQueueSchedulingBlockedWaitTypeDef

```python
# GetQueueRequestQueueSchedulingBlockedWaitTypeDef definition

class GetQueueRequestQueueSchedulingBlockedWaitTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetQueueRequestQueueSchedulingWaitTypeDef

```python
# GetQueueRequestQueueSchedulingWaitTypeDef definition

class GetQueueRequestQueueSchedulingWaitTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetJobEntityErrorTypeDef

```python
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
## GetSessionsStatisticsAggregationRequestGetSessionsStatisticsAggregationPaginateTypeDef

```python
# GetSessionsStatisticsAggregationRequestGetSessionsStatisticsAggregationPaginateTypeDef definition

class GetSessionsStatisticsAggregationRequestGetSessionsStatisticsAggregationPaginateTypeDef(TypedDict):
    farmId: str,
    aggregationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAvailableMeteredProductsRequestListAvailableMeteredProductsPaginateTypeDef

```python
# ListAvailableMeteredProductsRequestListAvailableMeteredProductsPaginateTypeDef definition

class ListAvailableMeteredProductsRequestListAvailableMeteredProductsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBudgetsRequestListBudgetsPaginateTypeDef

```python
# ListBudgetsRequestListBudgetsPaginateTypeDef definition

class ListBudgetsRequestListBudgetsPaginateTypeDef(TypedDict):
    farmId: str,
    status: NotRequired[BudgetStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: BudgetStatusType](./literals.md#budgetstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFarmMembersRequestListFarmMembersPaginateTypeDef

```python
# ListFarmMembersRequestListFarmMembersPaginateTypeDef definition

class ListFarmMembersRequestListFarmMembersPaginateTypeDef(TypedDict):
    farmId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFarmsRequestListFarmsPaginateTypeDef

```python
# ListFarmsRequestListFarmsPaginateTypeDef definition

class ListFarmsRequestListFarmsPaginateTypeDef(TypedDict):
    principalId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFleetMembersRequestListFleetMembersPaginateTypeDef

```python
# ListFleetMembersRequestListFleetMembersPaginateTypeDef definition

class ListFleetMembersRequestListFleetMembersPaginateTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFleetsRequestListFleetsPaginateTypeDef

```python
# ListFleetsRequestListFleetsPaginateTypeDef definition

class ListFleetsRequestListFleetsPaginateTypeDef(TypedDict):
    farmId: str,
    principalId: NotRequired[str],
    displayName: NotRequired[str],
    status: NotRequired[FleetStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FleetStatusType](./literals.md#fleetstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobMembersRequestListJobMembersPaginateTypeDef

```python
# ListJobMembersRequestListJobMembersPaginateTypeDef definition

class ListJobMembersRequestListJobMembersPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobParameterDefinitionsRequestListJobParameterDefinitionsPaginateTypeDef

```python
# ListJobParameterDefinitionsRequestListJobParameterDefinitionsPaginateTypeDef definition

class ListJobParameterDefinitionsRequestListJobParameterDefinitionsPaginateTypeDef(TypedDict):
    farmId: str,
    jobId: str,
    queueId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestListJobsPaginateTypeDef

```python
# ListJobsRequestListJobsPaginateTypeDef definition

class ListJobsRequestListJobsPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    principalId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLicenseEndpointsRequestListLicenseEndpointsPaginateTypeDef

```python
# ListLicenseEndpointsRequestListLicenseEndpointsPaginateTypeDef definition

class ListLicenseEndpointsRequestListLicenseEndpointsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMeteredProductsRequestListMeteredProductsPaginateTypeDef

```python
# ListMeteredProductsRequestListMeteredProductsPaginateTypeDef definition

class ListMeteredProductsRequestListMeteredProductsPaginateTypeDef(TypedDict):
    licenseEndpointId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMonitorsRequestListMonitorsPaginateTypeDef

```python
# ListMonitorsRequestListMonitorsPaginateTypeDef definition

class ListMonitorsRequestListMonitorsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueueEnvironmentsRequestListQueueEnvironmentsPaginateTypeDef

```python
# ListQueueEnvironmentsRequestListQueueEnvironmentsPaginateTypeDef definition

class ListQueueEnvironmentsRequestListQueueEnvironmentsPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueueFleetAssociationsRequestListQueueFleetAssociationsPaginateTypeDef

```python
# ListQueueFleetAssociationsRequestListQueueFleetAssociationsPaginateTypeDef definition

class ListQueueFleetAssociationsRequestListQueueFleetAssociationsPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: NotRequired[str],
    fleetId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueueMembersRequestListQueueMembersPaginateTypeDef

```python
# ListQueueMembersRequestListQueueMembersPaginateTypeDef definition

class ListQueueMembersRequestListQueueMembersPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueuesRequestListQueuesPaginateTypeDef

```python
# ListQueuesRequestListQueuesPaginateTypeDef definition

class ListQueuesRequestListQueuesPaginateTypeDef(TypedDict):
    farmId: str,
    principalId: NotRequired[str],
    status: NotRequired[QueueStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSessionActionsRequestListSessionActionsPaginateTypeDef

```python
# ListSessionActionsRequestListSessionActionsPaginateTypeDef definition

class ListSessionActionsRequestListSessionActionsPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    sessionId: NotRequired[str],
    taskId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSessionsForWorkerRequestListSessionsForWorkerPaginateTypeDef

```python
# ListSessionsForWorkerRequestListSessionsForWorkerPaginateTypeDef definition

class ListSessionsForWorkerRequestListSessionsForWorkerPaginateTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSessionsRequestListSessionsPaginateTypeDef

```python
# ListSessionsRequestListSessionsPaginateTypeDef definition

class ListSessionsRequestListSessionsPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStepConsumersRequestListStepConsumersPaginateTypeDef

```python
# ListStepConsumersRequestListStepConsumersPaginateTypeDef definition

class ListStepConsumersRequestListStepConsumersPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStepDependenciesRequestListStepDependenciesPaginateTypeDef

```python
# ListStepDependenciesRequestListStepDependenciesPaginateTypeDef definition

class ListStepDependenciesRequestListStepDependenciesPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStepsRequestListStepsPaginateTypeDef

```python
# ListStepsRequestListStepsPaginateTypeDef definition

class ListStepsRequestListStepsPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStorageProfilesForQueueRequestListStorageProfilesForQueuePaginateTypeDef

```python
# ListStorageProfilesForQueueRequestListStorageProfilesForQueuePaginateTypeDef definition

class ListStorageProfilesForQueueRequestListStorageProfilesForQueuePaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStorageProfilesRequestListStorageProfilesPaginateTypeDef

```python
# ListStorageProfilesRequestListStorageProfilesPaginateTypeDef definition

class ListStorageProfilesRequestListStorageProfilesPaginateTypeDef(TypedDict):
    farmId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTasksRequestListTasksPaginateTypeDef

```python
# ListTasksRequestListTasksPaginateTypeDef definition

class ListTasksRequestListTasksPaginateTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    jobId: str,
    stepId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkersRequestListWorkersPaginateTypeDef

```python
# ListWorkersRequestListWorkersPaginateTypeDef definition

class ListWorkersRequestListWorkersPaginateTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## HostPropertiesResponseTypeDef

```python
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
# ListLicenseEndpointsResponseTypeDef definition

class ListLicenseEndpointsResponseTypeDef(TypedDict):
    licenseEndpoints: List[LicenseEndpointSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseEndpointSummaryTypeDef](./type_defs.md#licenseendpointsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAvailableMeteredProductsResponseTypeDef

```python
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
# ListQueueFleetAssociationsResponseTypeDef definition

class ListQueueFleetAssociationsResponseTypeDef(TypedDict):
    queueFleetAssociations: List[QueueFleetAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QueueFleetAssociationSummaryTypeDef](./type_defs.md#queuefleetassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueueMembersResponseTypeDef

```python
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
# ParameterSpaceTypeDef definition

class ParameterSpaceTypeDef(TypedDict):
    parameters: List[StepParameterTypeDef],  # (1)
    combination: NotRequired[str],
```

1. See [:material-code-braces: StepParameterTypeDef](./type_defs.md#stepparametertypedef) 
## SearchSortExpressionTypeDef

```python
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
## StartSessionsStatisticsAggregationRequestRequestTypeDef

```python
# StartSessionsStatisticsAggregationRequestRequestTypeDef definition

class StartSessionsStatisticsAggregationRequestRequestTypeDef(TypedDict):
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
# StepRequiredCapabilitiesTypeDef definition

class StepRequiredCapabilitiesTypeDef(TypedDict):
    attributes: List[StepAttributeCapabilityTypeDef],  # (1)
    amounts: List[StepAmountCapabilityTypeDef],  # (2)
```

1. See [:material-code-braces: StepAttributeCapabilityTypeDef](./type_defs.md#stepattributecapabilitytypedef) 
2. See [:material-code-braces: StepAmountCapabilityTypeDef](./type_defs.md#stepamountcapabilitytypedef) 
## WorkerCapabilitiesTypeDef

```python
# WorkerCapabilitiesTypeDef definition

class WorkerCapabilitiesTypeDef(TypedDict):
    amounts: Sequence[WorkerAmountCapabilityTypeDef],  # (1)
    attributes: Sequence[WorkerAttributeCapabilityTypeDef],  # (2)
```

1. See [:material-code-braces: WorkerAmountCapabilityTypeDef](./type_defs.md#workeramountcapabilitytypedef) 
2. See [:material-code-braces: WorkerAttributeCapabilityTypeDef](./type_defs.md#workerattributecapabilitytypedef) 
## AssignedSessionActionDefinitionTypeDef

```python
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
# JobAttachmentDetailsEntityTypeDef definition

class JobAttachmentDetailsEntityTypeDef(TypedDict):
    jobId: str,
    attachments: AttachmentsOutputTypeDef,  # (1)
```

1. See [:material-code-braces: AttachmentsOutputTypeDef](./type_defs.md#attachmentsoutputtypedef) 
## GetBudgetResponseTypeDef

```python
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
# CustomerManagedFleetConfigurationOutputTypeDef definition

class CustomerManagedFleetConfigurationOutputTypeDef(TypedDict):
    mode: AutoScalingModeType,  # (1)
    workerCapabilities: CustomerManagedWorkerCapabilitiesOutputTypeDef,  # (2)
    storageProfileId: NotRequired[str],
```

1. See [:material-code-brackets: AutoScalingModeType](./literals.md#autoscalingmodetype) 
2. See [:material-code-braces: CustomerManagedWorkerCapabilitiesOutputTypeDef](./type_defs.md#customermanagedworkercapabilitiesoutputtypedef) 
## SearchFilterExpressionTypeDef

```python
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
## UpdateWorkerScheduleRequestRequestTypeDef

```python
# UpdateWorkerScheduleRequestRequestTypeDef definition

class UpdateWorkerScheduleRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    updatedSessionActions: NotRequired[Mapping[str, UpdatedSessionActionInfoTypeDef]],  # (1)
```

1. See [:material-code-braces: UpdatedSessionActionInfoTypeDef](./type_defs.md#updatedsessionactioninfotypedef) 
## ListStepsResponseTypeDef

```python
# ListStepsResponseTypeDef definition

class ListStepsResponseTypeDef(TypedDict):
    steps: List[StepSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: StepSummaryTypeDef](./type_defs.md#stepsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceManagedEc2FleetConfigurationOutputTypeDef

```python
# ServiceManagedEc2FleetConfigurationOutputTypeDef definition

class ServiceManagedEc2FleetConfigurationOutputTypeDef(TypedDict):
    instanceCapabilities: ServiceManagedEc2InstanceCapabilitiesOutputTypeDef,  # (1)
    instanceMarketOptions: ServiceManagedEc2InstanceMarketOptionsTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceManagedEc2InstanceCapabilitiesOutputTypeDef](./type_defs.md#servicemanagedec2instancecapabilitiesoutputtypedef) 
2. See [:material-code-braces: ServiceManagedEc2InstanceMarketOptionsTypeDef](./type_defs.md#servicemanagedec2instancemarketoptionstypedef) 
## CustomerManagedWorkerCapabilitiesTypeDef

```python
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
    customAttributes: NotRequired[Sequence[FleetAttributeCapabilityUnionTypeDef]],  # (9)
```

1. See [:material-code-braces: VCpuCountRangeTypeDef](./type_defs.md#vcpucountrangetypedef) 
2. See [:material-code-braces: MemoryMiBRangeTypeDef](./type_defs.md#memorymibrangetypedef) 
3. See [:material-code-brackets: AcceleratorTypeType](./literals.md#acceleratortypetype) 
4. See [:material-code-braces: AcceleratorCountRangeTypeDef](./type_defs.md#acceleratorcountrangetypedef) 
5. See [:material-code-braces: AcceleratorTotalMemoryMiBRangeTypeDef](./type_defs.md#acceleratortotalmemorymibrangetypedef) 
6. See [:material-code-brackets: CustomerManagedFleetOperatingSystemFamilyType](./literals.md#customermanagedfleetoperatingsystemfamilytype) 
7. See [:material-code-brackets: CpuArchitectureTypeType](./literals.md#cpuarchitecturetypetype) 
8. See [:material-code-braces: FleetAmountCapabilityTypeDef](./type_defs.md#fleetamountcapabilitytypedef) 
9. See [:material-code-braces: FleetAttributeCapabilityTypeDef](./type_defs.md#fleetattributecapabilitytypedef) [:material-code-braces: FleetAttributeCapabilityOutputTypeDef](./type_defs.md#fleetattributecapabilityoutputtypedef) 
## GetSessionResponseTypeDef

```python
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
# GetWorkerResponseTypeDef definition

class GetWorkerResponseTypeDef(TypedDict):
    workerId: str,
    farmId: str,
    fleetId: str,
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
# HostPropertiesRequestTypeDef definition

class HostPropertiesRequestTypeDef(TypedDict):
    ipAddresses: NotRequired[IpAddressesUnionTypeDef],  # (1)
    hostName: NotRequired[str],
```

1. See [:material-code-braces: IpAddressesTypeDef](./type_defs.md#ipaddressestypedef) [:material-code-braces: IpAddressesOutputTypeDef](./type_defs.md#ipaddressesoutputtypedef) 
## BatchGetJobEntityRequestRequestTypeDef

```python
# BatchGetJobEntityRequestRequestTypeDef definition

class BatchGetJobEntityRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    workerId: str,
    identifiers: Sequence[JobEntityIdentifiersUnionTypeDef],  # (1)
```

1. See [:material-code-braces: JobEntityIdentifiersUnionTypeDef](./type_defs.md#jobentityidentifiersuniontypedef) 
## CreateQueueRequestRequestTypeDef

```python
# CreateQueueRequestRequestTypeDef definition

class CreateQueueRequestRequestTypeDef(TypedDict):
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
## UpdateQueueRequestRequestTypeDef

```python
# UpdateQueueRequestRequestTypeDef definition

class UpdateQueueRequestRequestTypeDef(TypedDict):
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
## AttachmentsTypeDef

```python
# AttachmentsTypeDef definition

class AttachmentsTypeDef(TypedDict):
    manifests: Sequence[ManifestPropertiesUnionTypeDef],  # (1)
    fileSystem: NotRequired[JobAttachmentsFileSystemType],  # (2)
```

1. See [:material-code-braces: ManifestPropertiesTypeDef](./type_defs.md#manifestpropertiestypedef) [:material-code-braces: ManifestPropertiesOutputTypeDef](./type_defs.md#manifestpropertiesoutputtypedef) 
2. See [:material-code-brackets: JobAttachmentsFileSystemType](./literals.md#jobattachmentsfilesystemtype) 
## StepSearchSummaryTypeDef

```python
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
## AssignedSessionActionTypeDef

```python
# AssignedSessionActionTypeDef definition

class AssignedSessionActionTypeDef(TypedDict):
    sessionActionId: str,
    definition: AssignedSessionActionDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: AssignedSessionActionDefinitionTypeDef](./type_defs.md#assignedsessionactiondefinitiontypedef) 
## GetSessionActionResponseTypeDef

```python
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: SessionActionStatusType](./literals.md#sessionactionstatustype) 
2. See [:material-code-braces: SessionActionDefinitionTypeDef](./type_defs.md#sessionactiondefinitiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchGroupedFilterExpressionsTypeDef

```python
# SearchGroupedFilterExpressionsTypeDef definition

class SearchGroupedFilterExpressionsTypeDef(TypedDict):
    filters: Sequence[SearchFilterExpressionTypeDef],  # (1)
    operator: LogicalOperatorType,  # (2)
```

1. See [:material-code-braces: SearchFilterExpressionTypeDef](./type_defs.md#searchfilterexpressiontypedef) 
2. See [:material-code-brackets: LogicalOperatorType](./literals.md#logicaloperatortype) 
## BudgetScheduleTypeDef

```python
# BudgetScheduleTypeDef definition

class BudgetScheduleTypeDef(TypedDict):
    fixed: NotRequired[FixedBudgetScheduleUnionTypeDef],  # (1)
```

1. See [:material-code-braces: FixedBudgetScheduleTypeDef](./type_defs.md#fixedbudgetscheduletypedef) [:material-code-braces: FixedBudgetScheduleOutputTypeDef](./type_defs.md#fixedbudgetscheduleoutputtypedef) 
## FleetConfigurationOutputTypeDef

```python
# FleetConfigurationOutputTypeDef definition

class FleetConfigurationOutputTypeDef(TypedDict):
    customerManaged: NotRequired[CustomerManagedFleetConfigurationOutputTypeDef],  # (1)
    serviceManagedEc2: NotRequired[ServiceManagedEc2FleetConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: CustomerManagedFleetConfigurationOutputTypeDef](./type_defs.md#customermanagedfleetconfigurationoutputtypedef) 
2. See [:material-code-braces: ServiceManagedEc2FleetConfigurationOutputTypeDef](./type_defs.md#servicemanagedec2fleetconfigurationoutputtypedef) 
## ServiceManagedEc2FleetConfigurationTypeDef

```python
# ServiceManagedEc2FleetConfigurationTypeDef definition

class ServiceManagedEc2FleetConfigurationTypeDef(TypedDict):
    instanceCapabilities: ServiceManagedEc2InstanceCapabilitiesUnionTypeDef,  # (1)
    instanceMarketOptions: ServiceManagedEc2InstanceMarketOptionsTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceManagedEc2InstanceCapabilitiesTypeDef](./type_defs.md#servicemanagedec2instancecapabilitiestypedef) [:material-code-braces: ServiceManagedEc2InstanceCapabilitiesOutputTypeDef](./type_defs.md#servicemanagedec2instancecapabilitiesoutputtypedef) 
2. See [:material-code-braces: ServiceManagedEc2InstanceMarketOptionsTypeDef](./type_defs.md#servicemanagedec2instancemarketoptionstypedef) 
## SearchWorkersResponseTypeDef

```python
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
# ListWorkersResponseTypeDef definition

class ListWorkersResponseTypeDef(TypedDict):
    workers: List[WorkerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkerSummaryTypeDef](./type_defs.md#workersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkerRequestRequestTypeDef

```python
# CreateWorkerRequestRequestTypeDef definition

class CreateWorkerRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    hostProperties: NotRequired[HostPropertiesRequestTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: HostPropertiesRequestTypeDef](./type_defs.md#hostpropertiesrequesttypedef) 
## UpdateWorkerRequestRequestTypeDef

```python
# UpdateWorkerRequestRequestTypeDef definition

class UpdateWorkerRequestRequestTypeDef(TypedDict):
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
## CreateJobRequestRequestTypeDef

```python
# CreateJobRequestRequestTypeDef definition

class CreateJobRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueId: str,
    priority: int,
    clientToken: NotRequired[str],
    template: NotRequired[str],
    templateType: NotRequired[JobTemplateTypeType],  # (1)
    parameters: NotRequired[Mapping[str, JobParameterTypeDef]],  # (2)
    attachments: NotRequired[AttachmentsTypeDef],  # (3)
    storageProfileId: NotRequired[str],
    targetTaskRunStatus: NotRequired[CreateJobTargetTaskRunStatusType],  # (4)
    maxFailedTasksCount: NotRequired[int],
    maxRetriesPerTask: NotRequired[int],
    sourceJobId: NotRequired[str],
```

1. See [:material-code-brackets: JobTemplateTypeType](./literals.md#jobtemplatetypetype) 
2. See [:material-code-braces: JobParameterTypeDef](./type_defs.md#jobparametertypedef) 
3. See [:material-code-braces: AttachmentsTypeDef](./type_defs.md#attachmentstypedef) 
4. See [:material-code-brackets: CreateJobTargetTaskRunStatusType](./literals.md#createjobtargettaskrunstatustype) 
## SearchStepsResponseTypeDef

```python
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
# ListSessionActionsResponseTypeDef definition

class ListSessionActionsResponseTypeDef(TypedDict):
    sessionActions: List[SessionActionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SessionActionSummaryTypeDef](./type_defs.md#sessionactionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssignedSessionTypeDef

```python
# AssignedSessionTypeDef definition

class AssignedSessionTypeDef(TypedDict):
    queueId: str,
    jobId: str,
    sessionActions: List[AssignedSessionActionTypeDef],  # (1)
    logConfiguration: LogConfigurationTypeDef,  # (2)
```

1. See [:material-code-braces: AssignedSessionActionTypeDef](./type_defs.md#assignedsessionactiontypedef) 
2. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
## SearchJobsRequestRequestTypeDef

```python
# SearchJobsRequestRequestTypeDef definition

class SearchJobsRequestRequestTypeDef(TypedDict):
    farmId: str,
    queueIds: Sequence[str],
    itemOffset: int,
    filterExpressions: NotRequired[SearchGroupedFilterExpressionsTypeDef],  # (1)
    sortExpressions: NotRequired[Sequence[SearchSortExpressionTypeDef]],  # (2)
    pageSize: NotRequired[int],
```

1. See [:material-code-braces: SearchGroupedFilterExpressionsTypeDef](./type_defs.md#searchgroupedfilterexpressionstypedef) 
2. See [:material-code-braces: SearchSortExpressionTypeDef](./type_defs.md#searchsortexpressiontypedef) 
## SearchStepsRequestRequestTypeDef

```python
# SearchStepsRequestRequestTypeDef definition

class SearchStepsRequestRequestTypeDef(TypedDict):
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
## SearchTasksRequestRequestTypeDef

```python
# SearchTasksRequestRequestTypeDef definition

class SearchTasksRequestRequestTypeDef(TypedDict):
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
## SearchWorkersRequestRequestTypeDef

```python
# SearchWorkersRequestRequestTypeDef definition

class SearchWorkersRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetIds: Sequence[str],
    itemOffset: int,
    filterExpressions: NotRequired[SearchGroupedFilterExpressionsTypeDef],  # (1)
    sortExpressions: NotRequired[Sequence[SearchSortExpressionTypeDef]],  # (2)
    pageSize: NotRequired[int],
```

1. See [:material-code-braces: SearchGroupedFilterExpressionsTypeDef](./type_defs.md#searchgroupedfilterexpressionstypedef) 
2. See [:material-code-braces: SearchSortExpressionTypeDef](./type_defs.md#searchsortexpressiontypedef) 
## CreateBudgetRequestRequestTypeDef

```python
# CreateBudgetRequestRequestTypeDef definition

class CreateBudgetRequestRequestTypeDef(TypedDict):
    farmId: str,
    usageTrackingResource: UsageTrackingResourceTypeDef,  # (1)
    displayName: str,
    approximateDollarLimit: float,
    actions: Sequence[BudgetActionToAddTypeDef],  # (2)
    schedule: BudgetScheduleTypeDef,  # (3)
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-braces: UsageTrackingResourceTypeDef](./type_defs.md#usagetrackingresourcetypedef) 
2. See [:material-code-braces: BudgetActionToAddTypeDef](./type_defs.md#budgetactiontoaddtypedef) 
3. See [:material-code-braces: BudgetScheduleTypeDef](./type_defs.md#budgetscheduletypedef) 
## UpdateBudgetRequestRequestTypeDef

```python
# UpdateBudgetRequestRequestTypeDef definition

class UpdateBudgetRequestRequestTypeDef(TypedDict):
    farmId: str,
    budgetId: str,
    clientToken: NotRequired[str],
    displayName: NotRequired[str],
    description: NotRequired[str],
    status: NotRequired[BudgetStatusType],  # (1)
    approximateDollarLimit: NotRequired[float],
    actionsToAdd: NotRequired[Sequence[BudgetActionToAddTypeDef]],  # (2)
    actionsToRemove: NotRequired[Sequence[BudgetActionToRemoveTypeDef]],  # (3)
    schedule: NotRequired[BudgetScheduleTypeDef],  # (4)
```

1. See [:material-code-brackets: BudgetStatusType](./literals.md#budgetstatustype) 
2. See [:material-code-braces: BudgetActionToAddTypeDef](./type_defs.md#budgetactiontoaddtypedef) 
3. See [:material-code-braces: BudgetActionToRemoveTypeDef](./type_defs.md#budgetactiontoremovetypedef) 
4. See [:material-code-braces: BudgetScheduleTypeDef](./type_defs.md#budgetscheduletypedef) 
## FleetSummaryTypeDef

```python
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
## CustomerManagedFleetConfigurationTypeDef

```python
# CustomerManagedFleetConfigurationTypeDef definition

class CustomerManagedFleetConfigurationTypeDef(TypedDict):
    mode: AutoScalingModeType,  # (1)
    workerCapabilities: CustomerManagedWorkerCapabilitiesUnionTypeDef,  # (2)
    storageProfileId: NotRequired[str],
```

1. See [:material-code-brackets: AutoScalingModeType](./literals.md#autoscalingmodetype) 
2. See [:material-code-braces: CustomerManagedWorkerCapabilitiesTypeDef](./type_defs.md#customermanagedworkercapabilitiestypedef) [:material-code-braces: CustomerManagedWorkerCapabilitiesOutputTypeDef](./type_defs.md#customermanagedworkercapabilitiesoutputtypedef) 
## BatchGetJobEntityResponseTypeDef

```python
# BatchGetJobEntityResponseTypeDef definition

class BatchGetJobEntityResponseTypeDef(TypedDict):
    entities: List[JobEntityTypeDef],  # (1)
    errors: List[GetJobEntityErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: JobEntityTypeDef](./type_defs.md#jobentitytypedef) 
2. See [:material-code-braces: GetJobEntityErrorTypeDef](./type_defs.md#getjobentityerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkerScheduleResponseTypeDef

```python
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
# ListFleetsResponseTypeDef definition

class ListFleetsResponseTypeDef(TypedDict):
    fleets: List[FleetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetSummaryTypeDef](./type_defs.md#fleetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FleetConfigurationTypeDef

```python
# FleetConfigurationTypeDef definition

class FleetConfigurationTypeDef(TypedDict):
    customerManaged: NotRequired[CustomerManagedFleetConfigurationUnionTypeDef],  # (1)
    serviceManagedEc2: NotRequired[ServiceManagedEc2FleetConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: CustomerManagedFleetConfigurationTypeDef](./type_defs.md#customermanagedfleetconfigurationtypedef) [:material-code-braces: CustomerManagedFleetConfigurationOutputTypeDef](./type_defs.md#customermanagedfleetconfigurationoutputtypedef) 
2. See [:material-code-braces: ServiceManagedEc2FleetConfigurationTypeDef](./type_defs.md#servicemanagedec2fleetconfigurationtypedef) [:material-code-braces: ServiceManagedEc2FleetConfigurationOutputTypeDef](./type_defs.md#servicemanagedec2fleetconfigurationoutputtypedef) 
## CreateFleetRequestRequestTypeDef

```python
# CreateFleetRequestRequestTypeDef definition

class CreateFleetRequestRequestTypeDef(TypedDict):
    farmId: str,
    displayName: str,
    roleArn: str,
    maxWorkerCount: int,
    configuration: FleetConfigurationTypeDef,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    minWorkerCount: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FleetConfigurationTypeDef](./type_defs.md#fleetconfigurationtypedef) 
## UpdateFleetRequestRequestTypeDef

```python
# UpdateFleetRequestRequestTypeDef definition

class UpdateFleetRequestRequestTypeDef(TypedDict):
    farmId: str,
    fleetId: str,
    clientToken: NotRequired[str],
    displayName: NotRequired[str],
    description: NotRequired[str],
    roleArn: NotRequired[str],
    minWorkerCount: NotRequired[int],
    maxWorkerCount: NotRequired[int],
    configuration: NotRequired[FleetConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: FleetConfigurationTypeDef](./type_defs.md#fleetconfigurationtypedef) 
