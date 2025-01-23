# Type definitions

> [Index](../README.md) > [CodeDeploy](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodeDeploy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#codedeploy)
    type annotations stubs module [types-aiobotocore-codedeploy](https://pypi.org/project/types-aiobotocore-codedeploy/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## TrafficRouteUnionTypeDef

```python
# TrafficRouteUnionTypeDef definition

TrafficRouteUnionTypeDef = Union[
    TrafficRouteTypeDef,  # (1)
    TrafficRouteOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TrafficRouteTypeDef](./type_defs.md#trafficroutetypedef) 
2. See [:material-code-braces: TrafficRouteOutputTypeDef](./type_defs.md#trafficrouteoutputtypedef) 

## TriggerConfigUnionTypeDef

```python
# TriggerConfigUnionTypeDef definition

TriggerConfigUnionTypeDef = Union[
    TriggerConfigTypeDef,  # (1)
    TriggerConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TriggerConfigTypeDef](./type_defs.md#triggerconfigtypedef) 
2. See [:material-code-braces: TriggerConfigOutputTypeDef](./type_defs.md#triggerconfigoutputtypedef) 

## EC2TagSetUnionTypeDef

```python
# EC2TagSetUnionTypeDef definition

EC2TagSetUnionTypeDef = Union[
    EC2TagSetTypeDef,  # (1)
    EC2TagSetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EC2TagSetTypeDef](./type_defs.md#ec2tagsettypedef) 
2. See [:material-code-braces: EC2TagSetOutputTypeDef](./type_defs.md#ec2tagsetoutputtypedef) 

## TargetGroupPairInfoUnionTypeDef

```python
# TargetGroupPairInfoUnionTypeDef definition

TargetGroupPairInfoUnionTypeDef = Union[
    TargetGroupPairInfoTypeDef,  # (1)
    TargetGroupPairInfoOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TargetGroupPairInfoTypeDef](./type_defs.md#targetgrouppairinfotypedef) 
2. See [:material-code-braces: TargetGroupPairInfoOutputTypeDef](./type_defs.md#targetgrouppairinfooutputtypedef) 



## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## AlarmTypeDef

```python
# AlarmTypeDef definition

class AlarmTypeDef(TypedDict):
    name: NotRequired[str],
```

## AppSpecContentTypeDef

```python
# AppSpecContentTypeDef definition

class AppSpecContentTypeDef(TypedDict):
    content: NotRequired[str],
    sha256: NotRequired[str],
```

## ApplicationInfoTypeDef

```python
# ApplicationInfoTypeDef definition

class ApplicationInfoTypeDef(TypedDict):
    applicationId: NotRequired[str],
    applicationName: NotRequired[str],
    createTime: NotRequired[datetime],
    linkedToGitHub: NotRequired[bool],
    gitHubAccountName: NotRequired[str],
    computePlatform: NotRequired[ComputePlatformType],  # (1)
```

1. See [:material-code-brackets: ComputePlatformType](./literals.md#computeplatformtype) 
## AutoRollbackConfigurationOutputTypeDef

```python
# AutoRollbackConfigurationOutputTypeDef definition

class AutoRollbackConfigurationOutputTypeDef(TypedDict):
    enabled: NotRequired[bool],
    events: NotRequired[List[AutoRollbackEventType]],  # (1)
```

1. See [:material-code-brackets: AutoRollbackEventType](./literals.md#autorollbackeventtype) 
## AutoRollbackConfigurationTypeDef

```python
# AutoRollbackConfigurationTypeDef definition

class AutoRollbackConfigurationTypeDef(TypedDict):
    enabled: NotRequired[bool],
    events: NotRequired[Sequence[AutoRollbackEventType]],  # (1)
```

1. See [:material-code-brackets: AutoRollbackEventType](./literals.md#autorollbackeventtype) 
## AutoScalingGroupTypeDef

```python
# AutoScalingGroupTypeDef definition

class AutoScalingGroupTypeDef(TypedDict):
    name: NotRequired[str],
    hook: NotRequired[str],
    terminationHook: NotRequired[str],
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

## BatchGetApplicationsInputRequestTypeDef

```python
# BatchGetApplicationsInputRequestTypeDef definition

class BatchGetApplicationsInputRequestTypeDef(TypedDict):
    applicationNames: Sequence[str],
```

## BatchGetDeploymentGroupsInputRequestTypeDef

```python
# BatchGetDeploymentGroupsInputRequestTypeDef definition

class BatchGetDeploymentGroupsInputRequestTypeDef(TypedDict):
    applicationName: str,
    deploymentGroupNames: Sequence[str],
```

## BatchGetDeploymentInstancesInputRequestTypeDef

```python
# BatchGetDeploymentInstancesInputRequestTypeDef definition

class BatchGetDeploymentInstancesInputRequestTypeDef(TypedDict):
    deploymentId: str,
    instanceIds: Sequence[str],
```

## BatchGetDeploymentTargetsInputRequestTypeDef

```python
# BatchGetDeploymentTargetsInputRequestTypeDef definition

class BatchGetDeploymentTargetsInputRequestTypeDef(TypedDict):
    deploymentId: str,
    targetIds: Sequence[str],
```

## BatchGetDeploymentsInputRequestTypeDef

```python
# BatchGetDeploymentsInputRequestTypeDef definition

class BatchGetDeploymentsInputRequestTypeDef(TypedDict):
    deploymentIds: Sequence[str],
```

## BatchGetOnPremisesInstancesInputRequestTypeDef

```python
# BatchGetOnPremisesInstancesInputRequestTypeDef definition

class BatchGetOnPremisesInstancesInputRequestTypeDef(TypedDict):
    instanceNames: Sequence[str],
```

## BlueInstanceTerminationOptionTypeDef

```python
# BlueInstanceTerminationOptionTypeDef definition

class BlueInstanceTerminationOptionTypeDef(TypedDict):
    action: NotRequired[InstanceActionType],  # (1)
    terminationWaitTimeInMinutes: NotRequired[int],
```

1. See [:material-code-brackets: InstanceActionType](./literals.md#instanceactiontype) 
## DeploymentReadyOptionTypeDef

```python
# DeploymentReadyOptionTypeDef definition

class DeploymentReadyOptionTypeDef(TypedDict):
    actionOnTimeout: NotRequired[DeploymentReadyActionType],  # (1)
    waitTimeInMinutes: NotRequired[int],
```

1. See [:material-code-brackets: DeploymentReadyActionType](./literals.md#deploymentreadyactiontype) 
## GreenFleetProvisioningOptionTypeDef

```python
# GreenFleetProvisioningOptionTypeDef definition

class GreenFleetProvisioningOptionTypeDef(TypedDict):
    action: NotRequired[GreenFleetProvisioningActionType],  # (1)
```

1. See [:material-code-brackets: GreenFleetProvisioningActionType](./literals.md#greenfleetprovisioningactiontype) 
## ContinueDeploymentInputRequestTypeDef

```python
# ContinueDeploymentInputRequestTypeDef definition

class ContinueDeploymentInputRequestTypeDef(TypedDict):
    deploymentId: NotRequired[str],
    deploymentWaitType: NotRequired[DeploymentWaitTypeType],  # (1)
```

1. See [:material-code-brackets: DeploymentWaitTypeType](./literals.md#deploymentwaittypetype) 
## MinimumHealthyHostsTypeDef

```python
# MinimumHealthyHostsTypeDef definition

class MinimumHealthyHostsTypeDef(TypedDict):
    type: NotRequired[MinimumHealthyHostsTypeType],  # (1)
    value: NotRequired[int],
```

1. See [:material-code-brackets: MinimumHealthyHostsTypeType](./literals.md#minimumhealthyhoststypetype) 
## DeploymentStyleTypeDef

```python
# DeploymentStyleTypeDef definition

class DeploymentStyleTypeDef(TypedDict):
    deploymentType: NotRequired[DeploymentTypeType],  # (1)
    deploymentOption: NotRequired[DeploymentOptionType],  # (2)
```

1. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
2. See [:material-code-brackets: DeploymentOptionType](./literals.md#deploymentoptiontype) 
## EC2TagFilterTypeDef

```python
# EC2TagFilterTypeDef definition

class EC2TagFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    Type: NotRequired[EC2TagFilterTypeType],  # (1)
```

1. See [:material-code-brackets: EC2TagFilterTypeType](./literals.md#ec2tagfiltertypetype) 
## ECSServiceTypeDef

```python
# ECSServiceTypeDef definition

class ECSServiceTypeDef(TypedDict):
    serviceName: NotRequired[str],
    clusterName: NotRequired[str],
```

## TagFilterTypeDef

```python
# TagFilterTypeDef definition

class TagFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    Type: NotRequired[TagFilterTypeType],  # (1)
```

1. See [:material-code-brackets: TagFilterTypeType](./literals.md#tagfiltertypetype) 
## DeleteApplicationInputRequestTypeDef

```python
# DeleteApplicationInputRequestTypeDef definition

class DeleteApplicationInputRequestTypeDef(TypedDict):
    applicationName: str,
```

## DeleteDeploymentConfigInputRequestTypeDef

```python
# DeleteDeploymentConfigInputRequestTypeDef definition

class DeleteDeploymentConfigInputRequestTypeDef(TypedDict):
    deploymentConfigName: str,
```

## DeleteDeploymentGroupInputRequestTypeDef

```python
# DeleteDeploymentGroupInputRequestTypeDef definition

class DeleteDeploymentGroupInputRequestTypeDef(TypedDict):
    applicationName: str,
    deploymentGroupName: str,
```

## DeleteGitHubAccountTokenInputRequestTypeDef

```python
# DeleteGitHubAccountTokenInputRequestTypeDef definition

class DeleteGitHubAccountTokenInputRequestTypeDef(TypedDict):
    tokenName: NotRequired[str],
```

## DeleteResourcesByExternalIdInputRequestTypeDef

```python
# DeleteResourcesByExternalIdInputRequestTypeDef definition

class DeleteResourcesByExternalIdInputRequestTypeDef(TypedDict):
    externalId: NotRequired[str],
```

## LastDeploymentInfoTypeDef

```python
# LastDeploymentInfoTypeDef definition

class LastDeploymentInfoTypeDef(TypedDict):
    deploymentId: NotRequired[str],
    status: NotRequired[DeploymentStatusType],  # (1)
    endTime: NotRequired[datetime],
    createTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
## TriggerConfigOutputTypeDef

```python
# TriggerConfigOutputTypeDef definition

class TriggerConfigOutputTypeDef(TypedDict):
    triggerName: NotRequired[str],
    triggerTargetArn: NotRequired[str],
    triggerEvents: NotRequired[List[TriggerEventTypeType]],  # (1)
```

1. See [:material-code-brackets: TriggerEventTypeType](./literals.md#triggereventtypetype) 
## DeploymentOverviewTypeDef

```python
# DeploymentOverviewTypeDef definition

class DeploymentOverviewTypeDef(TypedDict):
    Pending: NotRequired[int],
    InProgress: NotRequired[int],
    Succeeded: NotRequired[int],
    Failed: NotRequired[int],
    Skipped: NotRequired[int],
    Ready: NotRequired[int],
```

## ErrorInformationTypeDef

```python
# ErrorInformationTypeDef definition

class ErrorInformationTypeDef(TypedDict):
    code: NotRequired[ErrorCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## RelatedDeploymentsTypeDef

```python
# RelatedDeploymentsTypeDef definition

class RelatedDeploymentsTypeDef(TypedDict):
    autoUpdateOutdatedInstancesRootDeploymentId: NotRequired[str],
    autoUpdateOutdatedInstancesDeploymentIds: NotRequired[List[str]],
```

## RollbackInfoTypeDef

```python
# RollbackInfoTypeDef definition

class RollbackInfoTypeDef(TypedDict):
    rollbackDeploymentId: NotRequired[str],
    rollbackTriggeringDeploymentId: NotRequired[str],
    rollbackMessage: NotRequired[str],
```

## DeregisterOnPremisesInstanceInputRequestTypeDef

```python
# DeregisterOnPremisesInstanceInputRequestTypeDef definition

class DeregisterOnPremisesInstanceInputRequestTypeDef(TypedDict):
    instanceName: str,
```

## DiagnosticsTypeDef

```python
# DiagnosticsTypeDef definition

class DiagnosticsTypeDef(TypedDict):
    errorCode: NotRequired[LifecycleErrorCodeType],  # (1)
    scriptName: NotRequired[str],
    message: NotRequired[str],
    logTail: NotRequired[str],
```

1. See [:material-code-brackets: LifecycleErrorCodeType](./literals.md#lifecycleerrorcodetype) 
## TargetGroupInfoTypeDef

```python
# TargetGroupInfoTypeDef definition

class TargetGroupInfoTypeDef(TypedDict):
    name: NotRequired[str],
```

## ELBInfoTypeDef

```python
# ELBInfoTypeDef definition

class ELBInfoTypeDef(TypedDict):
    name: NotRequired[str],
```

## GenericRevisionInfoTypeDef

```python
# GenericRevisionInfoTypeDef definition

class GenericRevisionInfoTypeDef(TypedDict):
    description: NotRequired[str],
    deploymentGroups: NotRequired[List[str]],
    firstUsedTime: NotRequired[datetime],
    lastUsedTime: NotRequired[datetime],
    registerTime: NotRequired[datetime],
```

## GetApplicationInputRequestTypeDef

```python
# GetApplicationInputRequestTypeDef definition

class GetApplicationInputRequestTypeDef(TypedDict):
    applicationName: str,
```

## GetDeploymentConfigInputRequestTypeDef

```python
# GetDeploymentConfigInputRequestTypeDef definition

class GetDeploymentConfigInputRequestTypeDef(TypedDict):
    deploymentConfigName: str,
```

## GetDeploymentGroupInputRequestTypeDef

```python
# GetDeploymentGroupInputRequestTypeDef definition

class GetDeploymentGroupInputRequestTypeDef(TypedDict):
    applicationName: str,
    deploymentGroupName: str,
```

## GetDeploymentInputRequestTypeDef

```python
# GetDeploymentInputRequestTypeDef definition

class GetDeploymentInputRequestTypeDef(TypedDict):
    deploymentId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetDeploymentInstanceInputRequestTypeDef

```python
# GetDeploymentInstanceInputRequestTypeDef definition

class GetDeploymentInstanceInputRequestTypeDef(TypedDict):
    deploymentId: str,
    instanceId: str,
```

## GetDeploymentTargetInputRequestTypeDef

```python
# GetDeploymentTargetInputRequestTypeDef definition

class GetDeploymentTargetInputRequestTypeDef(TypedDict):
    deploymentId: str,
    targetId: str,
```

## GetOnPremisesInstanceInputRequestTypeDef

```python
# GetOnPremisesInstanceInputRequestTypeDef definition

class GetOnPremisesInstanceInputRequestTypeDef(TypedDict):
    instanceName: str,
```

## GitHubLocationTypeDef

```python
# GitHubLocationTypeDef definition

class GitHubLocationTypeDef(TypedDict):
    repository: NotRequired[str],
    commitId: NotRequired[str],
```

## LambdaFunctionInfoTypeDef

```python
# LambdaFunctionInfoTypeDef definition

class LambdaFunctionInfoTypeDef(TypedDict):
    functionName: NotRequired[str],
    functionAlias: NotRequired[str],
    currentVersion: NotRequired[str],
    targetVersion: NotRequired[str],
    targetVersionWeight: NotRequired[float],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListApplicationRevisionsInputRequestTypeDef

```python
# ListApplicationRevisionsInputRequestTypeDef definition

class ListApplicationRevisionsInputRequestTypeDef(TypedDict):
    applicationName: str,
    sortBy: NotRequired[ApplicationRevisionSortByType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    s3Bucket: NotRequired[str],
    s3KeyPrefix: NotRequired[str],
    deployed: NotRequired[ListStateFilterActionType],  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ApplicationRevisionSortByType](./literals.md#applicationrevisionsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ListStateFilterActionType](./literals.md#liststatefilteractiontype) 
## ListApplicationsInputRequestTypeDef

```python
# ListApplicationsInputRequestTypeDef definition

class ListApplicationsInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## ListDeploymentConfigsInputRequestTypeDef

```python
# ListDeploymentConfigsInputRequestTypeDef definition

class ListDeploymentConfigsInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## ListDeploymentGroupsInputRequestTypeDef

```python
# ListDeploymentGroupsInputRequestTypeDef definition

class ListDeploymentGroupsInputRequestTypeDef(TypedDict):
    applicationName: str,
    nextToken: NotRequired[str],
```

## ListDeploymentInstancesInputRequestTypeDef

```python
# ListDeploymentInstancesInputRequestTypeDef definition

class ListDeploymentInstancesInputRequestTypeDef(TypedDict):
    deploymentId: str,
    nextToken: NotRequired[str],
    instanceStatusFilter: NotRequired[Sequence[InstanceStatusType]],  # (1)
    instanceTypeFilter: NotRequired[Sequence[InstanceTypeType]],  # (2)
```

1. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
## ListDeploymentTargetsInputRequestTypeDef

```python
# ListDeploymentTargetsInputRequestTypeDef definition

class ListDeploymentTargetsInputRequestTypeDef(TypedDict):
    deploymentId: str,
    nextToken: NotRequired[str],
    targetFilters: NotRequired[Mapping[TargetFilterNameType, Sequence[str]]],  # (1)
```

1. See [:material-code-brackets: TargetFilterNameType](./literals.md#targetfilternametype) 
## ListGitHubAccountTokenNamesInputRequestTypeDef

```python
# ListGitHubAccountTokenNamesInputRequestTypeDef definition

class ListGitHubAccountTokenNamesInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
```

## MinimumHealthyHostsPerZoneTypeDef

```python
# MinimumHealthyHostsPerZoneTypeDef definition

class MinimumHealthyHostsPerZoneTypeDef(TypedDict):
    type: NotRequired[MinimumHealthyHostsPerZoneTypeType],  # (1)
    value: NotRequired[int],
```

1. See [:material-code-brackets: MinimumHealthyHostsPerZoneTypeType](./literals.md#minimumhealthyhostsperzonetypetype) 
## PutLifecycleEventHookExecutionStatusInputRequestTypeDef

```python
# PutLifecycleEventHookExecutionStatusInputRequestTypeDef definition

class PutLifecycleEventHookExecutionStatusInputRequestTypeDef(TypedDict):
    deploymentId: NotRequired[str],
    lifecycleEventHookExecutionId: NotRequired[str],
    status: NotRequired[LifecycleEventStatusType],  # (1)
```

1. See [:material-code-brackets: LifecycleEventStatusType](./literals.md#lifecycleeventstatustype) 
## RawStringTypeDef

```python
# RawStringTypeDef definition

class RawStringTypeDef(TypedDict):
    content: NotRequired[str],
    sha256: NotRequired[str],
```

## RegisterOnPremisesInstanceInputRequestTypeDef

```python
# RegisterOnPremisesInstanceInputRequestTypeDef definition

class RegisterOnPremisesInstanceInputRequestTypeDef(TypedDict):
    instanceName: str,
    iamSessionArn: NotRequired[str],
    iamUserArn: NotRequired[str],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucket: NotRequired[str],
    key: NotRequired[str],
    bundleType: NotRequired[BundleTypeType],  # (1)
    version: NotRequired[str],
    eTag: NotRequired[str],
```

1. See [:material-code-brackets: BundleTypeType](./literals.md#bundletypetype) 
## SkipWaitTimeForInstanceTerminationInputRequestTypeDef

```python
# SkipWaitTimeForInstanceTerminationInputRequestTypeDef definition

class SkipWaitTimeForInstanceTerminationInputRequestTypeDef(TypedDict):
    deploymentId: NotRequired[str],
```

## StopDeploymentInputRequestTypeDef

```python
# StopDeploymentInputRequestTypeDef definition

class StopDeploymentInputRequestTypeDef(TypedDict):
    deploymentId: str,
    autoRollbackEnabled: NotRequired[bool],
```

## TrafficRouteOutputTypeDef

```python
# TrafficRouteOutputTypeDef definition

class TrafficRouteOutputTypeDef(TypedDict):
    listenerArns: NotRequired[List[str]],
```

## TimeBasedCanaryTypeDef

```python
# TimeBasedCanaryTypeDef definition

class TimeBasedCanaryTypeDef(TypedDict):
    canaryPercentage: NotRequired[int],
    canaryInterval: NotRequired[int],
```

## TimeBasedLinearTypeDef

```python
# TimeBasedLinearTypeDef definition

class TimeBasedLinearTypeDef(TypedDict):
    linearPercentage: NotRequired[int],
    linearInterval: NotRequired[int],
```

## TrafficRouteTypeDef

```python
# TrafficRouteTypeDef definition

class TrafficRouteTypeDef(TypedDict):
    listenerArns: NotRequired[Sequence[str]],
```

## TriggerConfigTypeDef

```python
# TriggerConfigTypeDef definition

class TriggerConfigTypeDef(TypedDict):
    triggerName: NotRequired[str],
    triggerTargetArn: NotRequired[str],
    triggerEvents: NotRequired[Sequence[TriggerEventTypeType]],  # (1)
```

1. See [:material-code-brackets: TriggerEventTypeType](./literals.md#triggereventtypetype) 
## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateApplicationInputRequestTypeDef

```python
# UpdateApplicationInputRequestTypeDef definition

class UpdateApplicationInputRequestTypeDef(TypedDict):
    applicationName: NotRequired[str],
    newApplicationName: NotRequired[str],
```

## AddTagsToOnPremisesInstancesInputRequestTypeDef

```python
# AddTagsToOnPremisesInstancesInputRequestTypeDef definition

class AddTagsToOnPremisesInstancesInputRequestTypeDef(TypedDict):
    tags: Sequence[TagTypeDef],  # (1)
    instanceNames: Sequence[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateApplicationInputRequestTypeDef

```python
# CreateApplicationInputRequestTypeDef definition

class CreateApplicationInputRequestTypeDef(TypedDict):
    applicationName: str,
    computePlatform: NotRequired[ComputePlatformType],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: ComputePlatformType](./literals.md#computeplatformtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## InstanceInfoTypeDef

```python
# InstanceInfoTypeDef definition

class InstanceInfoTypeDef(TypedDict):
    instanceName: NotRequired[str],
    iamSessionArn: NotRequired[str],
    iamUserArn: NotRequired[str],
    instanceArn: NotRequired[str],
    registerTime: NotRequired[datetime],
    deregisterTime: NotRequired[datetime],
    tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RemoveTagsFromOnPremisesInstancesInputRequestTypeDef

```python
# RemoveTagsFromOnPremisesInstancesInputRequestTypeDef definition

class RemoveTagsFromOnPremisesInstancesInputRequestTypeDef(TypedDict):
    tags: Sequence[TagTypeDef],  # (1)
    instanceNames: Sequence[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AlarmConfigurationOutputTypeDef

```python
# AlarmConfigurationOutputTypeDef definition

class AlarmConfigurationOutputTypeDef(TypedDict):
    enabled: NotRequired[bool],
    ignorePollAlarmFailure: NotRequired[bool],
    alarms: NotRequired[List[AlarmTypeDef]],  # (1)
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
## AlarmConfigurationTypeDef

```python
# AlarmConfigurationTypeDef definition

class AlarmConfigurationTypeDef(TypedDict):
    enabled: NotRequired[bool],
    ignorePollAlarmFailure: NotRequired[bool],
    alarms: NotRequired[Sequence[AlarmTypeDef]],  # (1)
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
## BatchGetApplicationsOutputTypeDef

```python
# BatchGetApplicationsOutputTypeDef definition

class BatchGetApplicationsOutputTypeDef(TypedDict):
    applicationsInfo: List[ApplicationInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationInfoTypeDef](./type_defs.md#applicationinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationOutputTypeDef

```python
# CreateApplicationOutputTypeDef definition

class CreateApplicationOutputTypeDef(TypedDict):
    applicationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentConfigOutputTypeDef

```python
# CreateDeploymentConfigOutputTypeDef definition

class CreateDeploymentConfigOutputTypeDef(TypedDict):
    deploymentConfigId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentGroupOutputTypeDef

```python
# CreateDeploymentGroupOutputTypeDef definition

class CreateDeploymentGroupOutputTypeDef(TypedDict):
    deploymentGroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentOutputTypeDef

```python
# CreateDeploymentOutputTypeDef definition

class CreateDeploymentOutputTypeDef(TypedDict):
    deploymentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDeploymentGroupOutputTypeDef

```python
# DeleteDeploymentGroupOutputTypeDef definition

class DeleteDeploymentGroupOutputTypeDef(TypedDict):
    hooksNotCleanedUp: List[AutoScalingGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoScalingGroupTypeDef](./type_defs.md#autoscalinggrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGitHubAccountTokenOutputTypeDef

```python
# DeleteGitHubAccountTokenOutputTypeDef definition

class DeleteGitHubAccountTokenOutputTypeDef(TypedDict):
    tokenName: str,
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
## GetApplicationOutputTypeDef

```python
# GetApplicationOutputTypeDef definition

class GetApplicationOutputTypeDef(TypedDict):
    application: ApplicationInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationInfoTypeDef](./type_defs.md#applicationinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsOutputTypeDef

```python
# ListApplicationsOutputTypeDef definition

class ListApplicationsOutputTypeDef(TypedDict):
    applications: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentConfigsOutputTypeDef

```python
# ListDeploymentConfigsOutputTypeDef definition

class ListDeploymentConfigsOutputTypeDef(TypedDict):
    deploymentConfigsList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentGroupsOutputTypeDef

```python
# ListDeploymentGroupsOutputTypeDef definition

class ListDeploymentGroupsOutputTypeDef(TypedDict):
    applicationName: str,
    deploymentGroups: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentInstancesOutputTypeDef

```python
# ListDeploymentInstancesOutputTypeDef definition

class ListDeploymentInstancesOutputTypeDef(TypedDict):
    instancesList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentTargetsOutputTypeDef

```python
# ListDeploymentTargetsOutputTypeDef definition

class ListDeploymentTargetsOutputTypeDef(TypedDict):
    targetIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentsOutputTypeDef

```python
# ListDeploymentsOutputTypeDef definition

class ListDeploymentsOutputTypeDef(TypedDict):
    deployments: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGitHubAccountTokenNamesOutputTypeDef

```python
# ListGitHubAccountTokenNamesOutputTypeDef definition

class ListGitHubAccountTokenNamesOutputTypeDef(TypedDict):
    tokenNameList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOnPremisesInstancesOutputTypeDef

```python
# ListOnPremisesInstancesOutputTypeDef definition

class ListOnPremisesInstancesOutputTypeDef(TypedDict):
    instanceNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLifecycleEventHookExecutionStatusOutputTypeDef

```python
# PutLifecycleEventHookExecutionStatusOutputTypeDef definition

class PutLifecycleEventHookExecutionStatusOutputTypeDef(TypedDict):
    lifecycleEventHookExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopDeploymentOutputTypeDef

```python
# StopDeploymentOutputTypeDef definition

class StopDeploymentOutputTypeDef(TypedDict):
    status: StopStatusType,  # (1)
    statusMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StopStatusType](./literals.md#stopstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDeploymentGroupOutputTypeDef

```python
# UpdateDeploymentGroupOutputTypeDef definition

class UpdateDeploymentGroupOutputTypeDef(TypedDict):
    hooksNotCleanedUp: List[AutoScalingGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoScalingGroupTypeDef](./type_defs.md#autoscalinggrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BlueGreenDeploymentConfigurationTypeDef

```python
# BlueGreenDeploymentConfigurationTypeDef definition

class BlueGreenDeploymentConfigurationTypeDef(TypedDict):
    terminateBlueInstancesOnDeploymentSuccess: NotRequired[BlueInstanceTerminationOptionTypeDef],  # (1)
    deploymentReadyOption: NotRequired[DeploymentReadyOptionTypeDef],  # (2)
    greenFleetProvisioningOption: NotRequired[GreenFleetProvisioningOptionTypeDef],  # (3)
```

1. See [:material-code-braces: BlueInstanceTerminationOptionTypeDef](./type_defs.md#blueinstanceterminationoptiontypedef) 
2. See [:material-code-braces: DeploymentReadyOptionTypeDef](./type_defs.md#deploymentreadyoptiontypedef) 
3. See [:material-code-braces: GreenFleetProvisioningOptionTypeDef](./type_defs.md#greenfleetprovisioningoptiontypedef) 
## EC2TagSetOutputTypeDef

```python
# EC2TagSetOutputTypeDef definition

class EC2TagSetOutputTypeDef(TypedDict):
    ec2TagSetList: NotRequired[List[List[EC2TagFilterTypeDef]]],  # (1)
```

1. See [:material-code-braces: EC2TagFilterTypeDef](./type_defs.md#ec2tagfiltertypedef) 
## EC2TagSetTypeDef

```python
# EC2TagSetTypeDef definition

class EC2TagSetTypeDef(TypedDict):
    ec2TagSetList: NotRequired[Sequence[Sequence[EC2TagFilterTypeDef]]],  # (1)
```

1. See [:material-code-braces: EC2TagFilterTypeDef](./type_defs.md#ec2tagfiltertypedef) 
## ListOnPremisesInstancesInputRequestTypeDef

```python
# ListOnPremisesInstancesInputRequestTypeDef definition

class ListOnPremisesInstancesInputRequestTypeDef(TypedDict):
    registrationStatus: NotRequired[RegistrationStatusType],  # (1)
    tagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
## OnPremisesTagSetOutputTypeDef

```python
# OnPremisesTagSetOutputTypeDef definition

class OnPremisesTagSetOutputTypeDef(TypedDict):
    onPremisesTagSetList: NotRequired[List[List[TagFilterTypeDef]]],  # (1)
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
## OnPremisesTagSetTypeDef

```python
# OnPremisesTagSetTypeDef definition

class OnPremisesTagSetTypeDef(TypedDict):
    onPremisesTagSetList: NotRequired[Sequence[Sequence[TagFilterTypeDef]]],  # (1)
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
## LifecycleEventTypeDef

```python
# LifecycleEventTypeDef definition

class LifecycleEventTypeDef(TypedDict):
    lifecycleEventName: NotRequired[str],
    diagnostics: NotRequired[DiagnosticsTypeDef],  # (1)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    status: NotRequired[LifecycleEventStatusType],  # (2)
```

1. See [:material-code-braces: DiagnosticsTypeDef](./type_defs.md#diagnosticstypedef) 
2. See [:material-code-brackets: LifecycleEventStatusType](./literals.md#lifecycleeventstatustype) 
## ECSTaskSetTypeDef

```python
# ECSTaskSetTypeDef definition

class ECSTaskSetTypeDef(TypedDict):
    identifer: NotRequired[str],
    desiredCount: NotRequired[int],
    pendingCount: NotRequired[int],
    runningCount: NotRequired[int],
    status: NotRequired[str],
    trafficWeight: NotRequired[float],
    targetGroup: NotRequired[TargetGroupInfoTypeDef],  # (1)
    taskSetLabel: NotRequired[TargetLabelType],  # (2)
```

1. See [:material-code-braces: TargetGroupInfoTypeDef](./type_defs.md#targetgroupinfotypedef) 
2. See [:material-code-brackets: TargetLabelType](./literals.md#targetlabeltype) 
## GetDeploymentInputWaitTypeDef

```python
# GetDeploymentInputWaitTypeDef definition

class GetDeploymentInputWaitTypeDef(TypedDict):
    deploymentId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## ListApplicationRevisionsInputPaginateTypeDef

```python
# ListApplicationRevisionsInputPaginateTypeDef definition

class ListApplicationRevisionsInputPaginateTypeDef(TypedDict):
    applicationName: str,
    sortBy: NotRequired[ApplicationRevisionSortByType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    s3Bucket: NotRequired[str],
    s3KeyPrefix: NotRequired[str],
    deployed: NotRequired[ListStateFilterActionType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ApplicationRevisionSortByType](./literals.md#applicationrevisionsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ListStateFilterActionType](./literals.md#liststatefilteractiontype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationsInputPaginateTypeDef

```python
# ListApplicationsInputPaginateTypeDef definition

class ListApplicationsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentConfigsInputPaginateTypeDef

```python
# ListDeploymentConfigsInputPaginateTypeDef definition

class ListDeploymentConfigsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentGroupsInputPaginateTypeDef

```python
# ListDeploymentGroupsInputPaginateTypeDef definition

class ListDeploymentGroupsInputPaginateTypeDef(TypedDict):
    applicationName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentInstancesInputPaginateTypeDef

```python
# ListDeploymentInstancesInputPaginateTypeDef definition

class ListDeploymentInstancesInputPaginateTypeDef(TypedDict):
    deploymentId: str,
    instanceStatusFilter: NotRequired[Sequence[InstanceStatusType]],  # (1)
    instanceTypeFilter: NotRequired[Sequence[InstanceTypeType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentTargetsInputPaginateTypeDef

```python
# ListDeploymentTargetsInputPaginateTypeDef definition

class ListDeploymentTargetsInputPaginateTypeDef(TypedDict):
    deploymentId: str,
    targetFilters: NotRequired[Mapping[TargetFilterNameType, Sequence[str]]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TargetFilterNameType](./literals.md#targetfilternametype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGitHubAccountTokenNamesInputPaginateTypeDef

```python
# ListGitHubAccountTokenNamesInputPaginateTypeDef definition

class ListGitHubAccountTokenNamesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOnPremisesInstancesInputPaginateTypeDef

```python
# ListOnPremisesInstancesInputPaginateTypeDef definition

class ListOnPremisesInstancesInputPaginateTypeDef(TypedDict):
    registrationStatus: NotRequired[RegistrationStatusType],  # (1)
    tagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ZonalConfigTypeDef

```python
# ZonalConfigTypeDef definition

class ZonalConfigTypeDef(TypedDict):
    firstZoneMonitorDurationInSeconds: NotRequired[int],
    monitorDurationInSeconds: NotRequired[int],
    minimumHealthyHostsPerZone: NotRequired[MinimumHealthyHostsPerZoneTypeDef],  # (1)
```

1. See [:material-code-braces: MinimumHealthyHostsPerZoneTypeDef](./type_defs.md#minimumhealthyhostsperzonetypedef) 
## RevisionLocationTypeDef

```python
# RevisionLocationTypeDef definition

class RevisionLocationTypeDef(TypedDict):
    revisionType: NotRequired[RevisionLocationTypeType],  # (1)
    s3Location: NotRequired[S3LocationTypeDef],  # (2)
    gitHubLocation: NotRequired[GitHubLocationTypeDef],  # (3)
    string: NotRequired[RawStringTypeDef],  # (4)
    appSpecContent: NotRequired[AppSpecContentTypeDef],  # (5)
```

1. See [:material-code-brackets: RevisionLocationTypeType](./literals.md#revisionlocationtypetype) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
3. See [:material-code-braces: GitHubLocationTypeDef](./type_defs.md#githublocationtypedef) 
4. See [:material-code-braces: RawStringTypeDef](./type_defs.md#rawstringtypedef) 
5. See [:material-code-braces: AppSpecContentTypeDef](./type_defs.md#appspeccontenttypedef) 
## TargetGroupPairInfoOutputTypeDef

```python
# TargetGroupPairInfoOutputTypeDef definition

class TargetGroupPairInfoOutputTypeDef(TypedDict):
    targetGroups: NotRequired[List[TargetGroupInfoTypeDef]],  # (1)
    prodTrafficRoute: NotRequired[TrafficRouteOutputTypeDef],  # (2)
    testTrafficRoute: NotRequired[TrafficRouteOutputTypeDef],  # (2)
```

1. See [:material-code-braces: TargetGroupInfoTypeDef](./type_defs.md#targetgroupinfotypedef) 
2. See [:material-code-braces: TrafficRouteOutputTypeDef](./type_defs.md#trafficrouteoutputtypedef) 
3. See [:material-code-braces: TrafficRouteOutputTypeDef](./type_defs.md#trafficrouteoutputtypedef) 
## TrafficRoutingConfigTypeDef

```python
# TrafficRoutingConfigTypeDef definition

class TrafficRoutingConfigTypeDef(TypedDict):
    type: NotRequired[TrafficRoutingTypeType],  # (1)
    timeBasedCanary: NotRequired[TimeBasedCanaryTypeDef],  # (2)
    timeBasedLinear: NotRequired[TimeBasedLinearTypeDef],  # (3)
```

1. See [:material-code-brackets: TrafficRoutingTypeType](./literals.md#trafficroutingtypetype) 
2. See [:material-code-braces: TimeBasedCanaryTypeDef](./type_defs.md#timebasedcanarytypedef) 
3. See [:material-code-braces: TimeBasedLinearTypeDef](./type_defs.md#timebasedlineartypedef) 
## TimeRangeTypeDef

```python
# TimeRangeTypeDef definition

class TimeRangeTypeDef(TypedDict):
    start: NotRequired[TimestampTypeDef],
    end: NotRequired[TimestampTypeDef],
```

## BatchGetOnPremisesInstancesOutputTypeDef

```python
# BatchGetOnPremisesInstancesOutputTypeDef definition

class BatchGetOnPremisesInstancesOutputTypeDef(TypedDict):
    instanceInfos: List[InstanceInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceInfoTypeDef](./type_defs.md#instanceinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOnPremisesInstanceOutputTypeDef

```python
# GetOnPremisesInstanceOutputTypeDef definition

class GetOnPremisesInstanceOutputTypeDef(TypedDict):
    instanceInfo: InstanceInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceInfoTypeDef](./type_defs.md#instanceinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TargetInstancesOutputTypeDef

```python
# TargetInstancesOutputTypeDef definition

class TargetInstancesOutputTypeDef(TypedDict):
    tagFilters: NotRequired[List[EC2TagFilterTypeDef]],  # (1)
    autoScalingGroups: NotRequired[List[str]],
    ec2TagSet: NotRequired[EC2TagSetOutputTypeDef],  # (2)
```

1. See [:material-code-braces: EC2TagFilterTypeDef](./type_defs.md#ec2tagfiltertypedef) 
2. See [:material-code-braces: EC2TagSetOutputTypeDef](./type_defs.md#ec2tagsetoutputtypedef) 
## CloudFormationTargetTypeDef

```python
# CloudFormationTargetTypeDef definition

class CloudFormationTargetTypeDef(TypedDict):
    deploymentId: NotRequired[str],
    targetId: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    lifecycleEvents: NotRequired[List[LifecycleEventTypeDef]],  # (1)
    status: NotRequired[TargetStatusType],  # (2)
    resourceType: NotRequired[str],
    targetVersionWeight: NotRequired[float],
```

1. See [:material-code-braces: LifecycleEventTypeDef](./type_defs.md#lifecycleeventtypedef) 
2. See [:material-code-brackets: TargetStatusType](./literals.md#targetstatustype) 
## InstanceSummaryTypeDef

```python
# InstanceSummaryTypeDef definition

class InstanceSummaryTypeDef(TypedDict):
    deploymentId: NotRequired[str],
    instanceId: NotRequired[str],
    status: NotRequired[InstanceStatusType],  # (1)
    lastUpdatedAt: NotRequired[datetime],
    lifecycleEvents: NotRequired[List[LifecycleEventTypeDef]],  # (2)
    instanceType: NotRequired[InstanceTypeType],  # (3)
```

1. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
2. See [:material-code-braces: LifecycleEventTypeDef](./type_defs.md#lifecycleeventtypedef) 
3. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
## InstanceTargetTypeDef

```python
# InstanceTargetTypeDef definition

class InstanceTargetTypeDef(TypedDict):
    deploymentId: NotRequired[str],
    targetId: NotRequired[str],
    targetArn: NotRequired[str],
    status: NotRequired[TargetStatusType],  # (1)
    lastUpdatedAt: NotRequired[datetime],
    lifecycleEvents: NotRequired[List[LifecycleEventTypeDef]],  # (2)
    instanceLabel: NotRequired[TargetLabelType],  # (3)
```

1. See [:material-code-brackets: TargetStatusType](./literals.md#targetstatustype) 
2. See [:material-code-braces: LifecycleEventTypeDef](./type_defs.md#lifecycleeventtypedef) 
3. See [:material-code-brackets: TargetLabelType](./literals.md#targetlabeltype) 
## LambdaTargetTypeDef

```python
# LambdaTargetTypeDef definition

class LambdaTargetTypeDef(TypedDict):
    deploymentId: NotRequired[str],
    targetId: NotRequired[str],
    targetArn: NotRequired[str],
    status: NotRequired[TargetStatusType],  # (1)
    lastUpdatedAt: NotRequired[datetime],
    lifecycleEvents: NotRequired[List[LifecycleEventTypeDef]],  # (2)
    lambdaFunctionInfo: NotRequired[LambdaFunctionInfoTypeDef],  # (3)
```

1. See [:material-code-brackets: TargetStatusType](./literals.md#targetstatustype) 
2. See [:material-code-braces: LifecycleEventTypeDef](./type_defs.md#lifecycleeventtypedef) 
3. See [:material-code-braces: LambdaFunctionInfoTypeDef](./type_defs.md#lambdafunctioninfotypedef) 
## ECSTargetTypeDef

```python
# ECSTargetTypeDef definition

class ECSTargetTypeDef(TypedDict):
    deploymentId: NotRequired[str],
    targetId: NotRequired[str],
    targetArn: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    lifecycleEvents: NotRequired[List[LifecycleEventTypeDef]],  # (1)
    status: NotRequired[TargetStatusType],  # (2)
    taskSetsInfo: NotRequired[List[ECSTaskSetTypeDef]],  # (3)
```

1. See [:material-code-braces: LifecycleEventTypeDef](./type_defs.md#lifecycleeventtypedef) 
2. See [:material-code-brackets: TargetStatusType](./literals.md#targetstatustype) 
3. See [:material-code-braces: ECSTaskSetTypeDef](./type_defs.md#ecstasksettypedef) 
## BatchGetApplicationRevisionsInputRequestTypeDef

```python
# BatchGetApplicationRevisionsInputRequestTypeDef definition

class BatchGetApplicationRevisionsInputRequestTypeDef(TypedDict):
    applicationName: str,
    revisions: Sequence[RevisionLocationTypeDef],  # (1)
```

1. See [:material-code-braces: RevisionLocationTypeDef](./type_defs.md#revisionlocationtypedef) 
## GetApplicationRevisionInputRequestTypeDef

```python
# GetApplicationRevisionInputRequestTypeDef definition

class GetApplicationRevisionInputRequestTypeDef(TypedDict):
    applicationName: str,
    revision: RevisionLocationTypeDef,  # (1)
```

1. See [:material-code-braces: RevisionLocationTypeDef](./type_defs.md#revisionlocationtypedef) 
## GetApplicationRevisionOutputTypeDef

```python
# GetApplicationRevisionOutputTypeDef definition

class GetApplicationRevisionOutputTypeDef(TypedDict):
    applicationName: str,
    revision: RevisionLocationTypeDef,  # (1)
    revisionInfo: GenericRevisionInfoTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RevisionLocationTypeDef](./type_defs.md#revisionlocationtypedef) 
2. See [:material-code-braces: GenericRevisionInfoTypeDef](./type_defs.md#genericrevisioninfotypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationRevisionsOutputTypeDef

```python
# ListApplicationRevisionsOutputTypeDef definition

class ListApplicationRevisionsOutputTypeDef(TypedDict):
    revisions: List[RevisionLocationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RevisionLocationTypeDef](./type_defs.md#revisionlocationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterApplicationRevisionInputRequestTypeDef

```python
# RegisterApplicationRevisionInputRequestTypeDef definition

class RegisterApplicationRevisionInputRequestTypeDef(TypedDict):
    applicationName: str,
    revision: RevisionLocationTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: RevisionLocationTypeDef](./type_defs.md#revisionlocationtypedef) 
## RevisionInfoTypeDef

```python
# RevisionInfoTypeDef definition

class RevisionInfoTypeDef(TypedDict):
    revisionLocation: NotRequired[RevisionLocationTypeDef],  # (1)
    genericRevisionInfo: NotRequired[GenericRevisionInfoTypeDef],  # (2)
```

1. See [:material-code-braces: RevisionLocationTypeDef](./type_defs.md#revisionlocationtypedef) 
2. See [:material-code-braces: GenericRevisionInfoTypeDef](./type_defs.md#genericrevisioninfotypedef) 
## LoadBalancerInfoOutputTypeDef

```python
# LoadBalancerInfoOutputTypeDef definition

class LoadBalancerInfoOutputTypeDef(TypedDict):
    elbInfoList: NotRequired[List[ELBInfoTypeDef]],  # (1)
    targetGroupInfoList: NotRequired[List[TargetGroupInfoTypeDef]],  # (2)
    targetGroupPairInfoList: NotRequired[List[TargetGroupPairInfoOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: ELBInfoTypeDef](./type_defs.md#elbinfotypedef) 
2. See [:material-code-braces: TargetGroupInfoTypeDef](./type_defs.md#targetgroupinfotypedef) 
3. See [:material-code-braces: TargetGroupPairInfoOutputTypeDef](./type_defs.md#targetgrouppairinfooutputtypedef) 
## CreateDeploymentConfigInputRequestTypeDef

```python
# CreateDeploymentConfigInputRequestTypeDef definition

class CreateDeploymentConfigInputRequestTypeDef(TypedDict):
    deploymentConfigName: str,
    minimumHealthyHosts: NotRequired[MinimumHealthyHostsTypeDef],  # (1)
    trafficRoutingConfig: NotRequired[TrafficRoutingConfigTypeDef],  # (2)
    computePlatform: NotRequired[ComputePlatformType],  # (3)
    zonalConfig: NotRequired[ZonalConfigTypeDef],  # (4)
```

1. See [:material-code-braces: MinimumHealthyHostsTypeDef](./type_defs.md#minimumhealthyhoststypedef) 
2. See [:material-code-braces: TrafficRoutingConfigTypeDef](./type_defs.md#trafficroutingconfigtypedef) 
3. See [:material-code-brackets: ComputePlatformType](./literals.md#computeplatformtype) 
4. See [:material-code-braces: ZonalConfigTypeDef](./type_defs.md#zonalconfigtypedef) 
## DeploymentConfigInfoTypeDef

```python
# DeploymentConfigInfoTypeDef definition

class DeploymentConfigInfoTypeDef(TypedDict):
    deploymentConfigId: NotRequired[str],
    deploymentConfigName: NotRequired[str],
    minimumHealthyHosts: NotRequired[MinimumHealthyHostsTypeDef],  # (1)
    createTime: NotRequired[datetime],
    computePlatform: NotRequired[ComputePlatformType],  # (2)
    trafficRoutingConfig: NotRequired[TrafficRoutingConfigTypeDef],  # (3)
    zonalConfig: NotRequired[ZonalConfigTypeDef],  # (4)
```

1. See [:material-code-braces: MinimumHealthyHostsTypeDef](./type_defs.md#minimumhealthyhoststypedef) 
2. See [:material-code-brackets: ComputePlatformType](./literals.md#computeplatformtype) 
3. See [:material-code-braces: TrafficRoutingConfigTypeDef](./type_defs.md#trafficroutingconfigtypedef) 
4. See [:material-code-braces: ZonalConfigTypeDef](./type_defs.md#zonalconfigtypedef) 
## ListDeploymentsInputPaginateTypeDef

```python
# ListDeploymentsInputPaginateTypeDef definition

class ListDeploymentsInputPaginateTypeDef(TypedDict):
    applicationName: NotRequired[str],
    deploymentGroupName: NotRequired[str],
    externalId: NotRequired[str],
    includeOnlyStatuses: NotRequired[Sequence[DeploymentStatusType]],  # (1)
    createTimeRange: NotRequired[TimeRangeTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentsInputRequestTypeDef

```python
# ListDeploymentsInputRequestTypeDef definition

class ListDeploymentsInputRequestTypeDef(TypedDict):
    applicationName: NotRequired[str],
    deploymentGroupName: NotRequired[str],
    externalId: NotRequired[str],
    includeOnlyStatuses: NotRequired[Sequence[DeploymentStatusType]],  # (1)
    createTimeRange: NotRequired[TimeRangeTypeDef],  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
## TargetGroupPairInfoTypeDef

```python
# TargetGroupPairInfoTypeDef definition

class TargetGroupPairInfoTypeDef(TypedDict):
    targetGroups: NotRequired[Sequence[TargetGroupInfoTypeDef]],  # (1)
    prodTrafficRoute: NotRequired[TrafficRouteUnionTypeDef],  # (2)
    testTrafficRoute: NotRequired[TrafficRouteUnionTypeDef],  # (2)
```

1. See [:material-code-braces: TargetGroupInfoTypeDef](./type_defs.md#targetgroupinfotypedef) 
2. See [:material-code-braces: TrafficRouteTypeDef](./type_defs.md#trafficroutetypedef) [:material-code-braces: TrafficRouteOutputTypeDef](./type_defs.md#trafficrouteoutputtypedef) 
3. See [:material-code-braces: TrafficRouteTypeDef](./type_defs.md#trafficroutetypedef) [:material-code-braces: TrafficRouteOutputTypeDef](./type_defs.md#trafficrouteoutputtypedef) 
## TargetInstancesTypeDef

```python
# TargetInstancesTypeDef definition

class TargetInstancesTypeDef(TypedDict):
    tagFilters: NotRequired[Sequence[EC2TagFilterTypeDef]],  # (1)
    autoScalingGroups: NotRequired[Sequence[str]],
    ec2TagSet: NotRequired[EC2TagSetUnionTypeDef],  # (2)
```

1. See [:material-code-braces: EC2TagFilterTypeDef](./type_defs.md#ec2tagfiltertypedef) 
2. See [:material-code-braces: EC2TagSetTypeDef](./type_defs.md#ec2tagsettypedef) [:material-code-braces: EC2TagSetOutputTypeDef](./type_defs.md#ec2tagsetoutputtypedef) 
## BatchGetDeploymentInstancesOutputTypeDef

```python
# BatchGetDeploymentInstancesOutputTypeDef definition

class BatchGetDeploymentInstancesOutputTypeDef(TypedDict):
    instancesSummary: List[InstanceSummaryTypeDef],  # (1)
    errorMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeploymentInstanceOutputTypeDef

```python
# GetDeploymentInstanceOutputTypeDef definition

class GetDeploymentInstanceOutputTypeDef(TypedDict):
    instanceSummary: InstanceSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentTargetTypeDef

```python
# DeploymentTargetTypeDef definition

class DeploymentTargetTypeDef(TypedDict):
    deploymentTargetType: NotRequired[DeploymentTargetTypeType],  # (1)
    instanceTarget: NotRequired[InstanceTargetTypeDef],  # (2)
    lambdaTarget: NotRequired[LambdaTargetTypeDef],  # (3)
    ecsTarget: NotRequired[ECSTargetTypeDef],  # (4)
    cloudFormationTarget: NotRequired[CloudFormationTargetTypeDef],  # (5)
```

1. See [:material-code-brackets: DeploymentTargetTypeType](./literals.md#deploymenttargettypetype) 
2. See [:material-code-braces: InstanceTargetTypeDef](./type_defs.md#instancetargettypedef) 
3. See [:material-code-braces: LambdaTargetTypeDef](./type_defs.md#lambdatargettypedef) 
4. See [:material-code-braces: ECSTargetTypeDef](./type_defs.md#ecstargettypedef) 
5. See [:material-code-braces: CloudFormationTargetTypeDef](./type_defs.md#cloudformationtargettypedef) 
## BatchGetApplicationRevisionsOutputTypeDef

```python
# BatchGetApplicationRevisionsOutputTypeDef definition

class BatchGetApplicationRevisionsOutputTypeDef(TypedDict):
    applicationName: str,
    errorMessage: str,
    revisions: List[RevisionInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RevisionInfoTypeDef](./type_defs.md#revisioninfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentGroupInfoTypeDef

```python
# DeploymentGroupInfoTypeDef definition

class DeploymentGroupInfoTypeDef(TypedDict):
    applicationName: NotRequired[str],
    deploymentGroupId: NotRequired[str],
    deploymentGroupName: NotRequired[str],
    deploymentConfigName: NotRequired[str],
    ec2TagFilters: NotRequired[List[EC2TagFilterTypeDef]],  # (1)
    onPremisesInstanceTagFilters: NotRequired[List[TagFilterTypeDef]],  # (2)
    autoScalingGroups: NotRequired[List[AutoScalingGroupTypeDef]],  # (3)
    serviceRoleArn: NotRequired[str],
    targetRevision: NotRequired[RevisionLocationTypeDef],  # (4)
    triggerConfigurations: NotRequired[List[TriggerConfigOutputTypeDef]],  # (5)
    alarmConfiguration: NotRequired[AlarmConfigurationOutputTypeDef],  # (6)
    autoRollbackConfiguration: NotRequired[AutoRollbackConfigurationOutputTypeDef],  # (7)
    deploymentStyle: NotRequired[DeploymentStyleTypeDef],  # (8)
    outdatedInstancesStrategy: NotRequired[OutdatedInstancesStrategyType],  # (9)
    blueGreenDeploymentConfiguration: NotRequired[BlueGreenDeploymentConfigurationTypeDef],  # (10)
    loadBalancerInfo: NotRequired[LoadBalancerInfoOutputTypeDef],  # (11)
    lastSuccessfulDeployment: NotRequired[LastDeploymentInfoTypeDef],  # (12)
    lastAttemptedDeployment: NotRequired[LastDeploymentInfoTypeDef],  # (12)
    ec2TagSet: NotRequired[EC2TagSetOutputTypeDef],  # (14)
    onPremisesTagSet: NotRequired[OnPremisesTagSetOutputTypeDef],  # (15)
    computePlatform: NotRequired[ComputePlatformType],  # (16)
    ecsServices: NotRequired[List[ECSServiceTypeDef]],  # (17)
    terminationHookEnabled: NotRequired[bool],
```

1. See [:material-code-braces: EC2TagFilterTypeDef](./type_defs.md#ec2tagfiltertypedef) 
2. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
3. See [:material-code-braces: AutoScalingGroupTypeDef](./type_defs.md#autoscalinggrouptypedef) 
4. See [:material-code-braces: RevisionLocationTypeDef](./type_defs.md#revisionlocationtypedef) 
5. See [:material-code-braces: TriggerConfigOutputTypeDef](./type_defs.md#triggerconfigoutputtypedef) 
6. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
7. See [:material-code-braces: AutoRollbackConfigurationOutputTypeDef](./type_defs.md#autorollbackconfigurationoutputtypedef) 
8. See [:material-code-braces: DeploymentStyleTypeDef](./type_defs.md#deploymentstyletypedef) 
9. See [:material-code-brackets: OutdatedInstancesStrategyType](./literals.md#outdatedinstancesstrategytype) 
10. See [:material-code-braces: BlueGreenDeploymentConfigurationTypeDef](./type_defs.md#bluegreendeploymentconfigurationtypedef) 
11. See [:material-code-braces: LoadBalancerInfoOutputTypeDef](./type_defs.md#loadbalancerinfooutputtypedef) 
12. See [:material-code-braces: LastDeploymentInfoTypeDef](./type_defs.md#lastdeploymentinfotypedef) 
13. See [:material-code-braces: LastDeploymentInfoTypeDef](./type_defs.md#lastdeploymentinfotypedef) 
14. See [:material-code-braces: EC2TagSetOutputTypeDef](./type_defs.md#ec2tagsetoutputtypedef) 
15. See [:material-code-braces: OnPremisesTagSetOutputTypeDef](./type_defs.md#onpremisestagsetoutputtypedef) 
16. See [:material-code-brackets: ComputePlatformType](./literals.md#computeplatformtype) 
17. See [:material-code-braces: ECSServiceTypeDef](./type_defs.md#ecsservicetypedef) 
## DeploymentInfoTypeDef

```python
# DeploymentInfoTypeDef definition

class DeploymentInfoTypeDef(TypedDict):
    applicationName: NotRequired[str],
    deploymentGroupName: NotRequired[str],
    deploymentConfigName: NotRequired[str],
    deploymentId: NotRequired[str],
    previousRevision: NotRequired[RevisionLocationTypeDef],  # (1)
    revision: NotRequired[RevisionLocationTypeDef],  # (1)
    status: NotRequired[DeploymentStatusType],  # (3)
    errorInformation: NotRequired[ErrorInformationTypeDef],  # (4)
    createTime: NotRequired[datetime],
    startTime: NotRequired[datetime],
    completeTime: NotRequired[datetime],
    deploymentOverview: NotRequired[DeploymentOverviewTypeDef],  # (5)
    description: NotRequired[str],
    creator: NotRequired[DeploymentCreatorType],  # (6)
    ignoreApplicationStopFailures: NotRequired[bool],
    autoRollbackConfiguration: NotRequired[AutoRollbackConfigurationOutputTypeDef],  # (7)
    updateOutdatedInstancesOnly: NotRequired[bool],
    rollbackInfo: NotRequired[RollbackInfoTypeDef],  # (8)
    deploymentStyle: NotRequired[DeploymentStyleTypeDef],  # (9)
    targetInstances: NotRequired[TargetInstancesOutputTypeDef],  # (10)
    instanceTerminationWaitTimeStarted: NotRequired[bool],
    blueGreenDeploymentConfiguration: NotRequired[BlueGreenDeploymentConfigurationTypeDef],  # (11)
    loadBalancerInfo: NotRequired[LoadBalancerInfoOutputTypeDef],  # (12)
    additionalDeploymentStatusInfo: NotRequired[str],
    fileExistsBehavior: NotRequired[FileExistsBehaviorType],  # (13)
    deploymentStatusMessages: NotRequired[List[str]],
    computePlatform: NotRequired[ComputePlatformType],  # (14)
    externalId: NotRequired[str],
    relatedDeployments: NotRequired[RelatedDeploymentsTypeDef],  # (15)
    overrideAlarmConfiguration: NotRequired[AlarmConfigurationOutputTypeDef],  # (16)
```

1. See [:material-code-braces: RevisionLocationTypeDef](./type_defs.md#revisionlocationtypedef) 
2. See [:material-code-braces: RevisionLocationTypeDef](./type_defs.md#revisionlocationtypedef) 
3. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
4. See [:material-code-braces: ErrorInformationTypeDef](./type_defs.md#errorinformationtypedef) 
5. See [:material-code-braces: DeploymentOverviewTypeDef](./type_defs.md#deploymentoverviewtypedef) 
6. See [:material-code-brackets: DeploymentCreatorType](./literals.md#deploymentcreatortype) 
7. See [:material-code-braces: AutoRollbackConfigurationOutputTypeDef](./type_defs.md#autorollbackconfigurationoutputtypedef) 
8. See [:material-code-braces: RollbackInfoTypeDef](./type_defs.md#rollbackinfotypedef) 
9. See [:material-code-braces: DeploymentStyleTypeDef](./type_defs.md#deploymentstyletypedef) 
10. See [:material-code-braces: TargetInstancesOutputTypeDef](./type_defs.md#targetinstancesoutputtypedef) 
11. See [:material-code-braces: BlueGreenDeploymentConfigurationTypeDef](./type_defs.md#bluegreendeploymentconfigurationtypedef) 
12. See [:material-code-braces: LoadBalancerInfoOutputTypeDef](./type_defs.md#loadbalancerinfooutputtypedef) 
13. See [:material-code-brackets: FileExistsBehaviorType](./literals.md#fileexistsbehaviortype) 
14. See [:material-code-brackets: ComputePlatformType](./literals.md#computeplatformtype) 
15. See [:material-code-braces: RelatedDeploymentsTypeDef](./type_defs.md#relateddeploymentstypedef) 
16. See [:material-code-braces: AlarmConfigurationOutputTypeDef](./type_defs.md#alarmconfigurationoutputtypedef) 
## GetDeploymentConfigOutputTypeDef

```python
# GetDeploymentConfigOutputTypeDef definition

class GetDeploymentConfigOutputTypeDef(TypedDict):
    deploymentConfigInfo: DeploymentConfigInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentConfigInfoTypeDef](./type_defs.md#deploymentconfiginfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentInputRequestTypeDef

```python
# CreateDeploymentInputRequestTypeDef definition

class CreateDeploymentInputRequestTypeDef(TypedDict):
    applicationName: str,
    deploymentGroupName: NotRequired[str],
    revision: NotRequired[RevisionLocationTypeDef],  # (1)
    deploymentConfigName: NotRequired[str],
    description: NotRequired[str],
    ignoreApplicationStopFailures: NotRequired[bool],
    targetInstances: NotRequired[TargetInstancesTypeDef],  # (2)
    autoRollbackConfiguration: NotRequired[AutoRollbackConfigurationTypeDef],  # (3)
    updateOutdatedInstancesOnly: NotRequired[bool],
    fileExistsBehavior: NotRequired[FileExistsBehaviorType],  # (4)
    overrideAlarmConfiguration: NotRequired[AlarmConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: RevisionLocationTypeDef](./type_defs.md#revisionlocationtypedef) 
2. See [:material-code-braces: TargetInstancesTypeDef](./type_defs.md#targetinstancestypedef) 
3. See [:material-code-braces: AutoRollbackConfigurationTypeDef](./type_defs.md#autorollbackconfigurationtypedef) 
4. See [:material-code-brackets: FileExistsBehaviorType](./literals.md#fileexistsbehaviortype) 
5. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) 
## BatchGetDeploymentTargetsOutputTypeDef

```python
# BatchGetDeploymentTargetsOutputTypeDef definition

class BatchGetDeploymentTargetsOutputTypeDef(TypedDict):
    deploymentTargets: List[DeploymentTargetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentTargetTypeDef](./type_defs.md#deploymenttargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeploymentTargetOutputTypeDef

```python
# GetDeploymentTargetOutputTypeDef definition

class GetDeploymentTargetOutputTypeDef(TypedDict):
    deploymentTarget: DeploymentTargetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentTargetTypeDef](./type_defs.md#deploymenttargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetDeploymentGroupsOutputTypeDef

```python
# BatchGetDeploymentGroupsOutputTypeDef definition

class BatchGetDeploymentGroupsOutputTypeDef(TypedDict):
    deploymentGroupsInfo: List[DeploymentGroupInfoTypeDef],  # (1)
    errorMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentGroupInfoTypeDef](./type_defs.md#deploymentgroupinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeploymentGroupOutputTypeDef

```python
# GetDeploymentGroupOutputTypeDef definition

class GetDeploymentGroupOutputTypeDef(TypedDict):
    deploymentGroupInfo: DeploymentGroupInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentGroupInfoTypeDef](./type_defs.md#deploymentgroupinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetDeploymentsOutputTypeDef

```python
# BatchGetDeploymentsOutputTypeDef definition

class BatchGetDeploymentsOutputTypeDef(TypedDict):
    deploymentsInfo: List[DeploymentInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentInfoTypeDef](./type_defs.md#deploymentinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeploymentOutputTypeDef

```python
# GetDeploymentOutputTypeDef definition

class GetDeploymentOutputTypeDef(TypedDict):
    deploymentInfo: DeploymentInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentInfoTypeDef](./type_defs.md#deploymentinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoadBalancerInfoTypeDef

```python
# LoadBalancerInfoTypeDef definition

class LoadBalancerInfoTypeDef(TypedDict):
    elbInfoList: NotRequired[Sequence[ELBInfoTypeDef]],  # (1)
    targetGroupInfoList: NotRequired[Sequence[TargetGroupInfoTypeDef]],  # (2)
    targetGroupPairInfoList: NotRequired[Sequence[TargetGroupPairInfoUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: ELBInfoTypeDef](./type_defs.md#elbinfotypedef) 
2. See [:material-code-braces: TargetGroupInfoTypeDef](./type_defs.md#targetgroupinfotypedef) 
3. See [:material-code-braces: TargetGroupPairInfoTypeDef](./type_defs.md#targetgrouppairinfotypedef) [:material-code-braces: TargetGroupPairInfoOutputTypeDef](./type_defs.md#targetgrouppairinfooutputtypedef) 
## CreateDeploymentGroupInputRequestTypeDef

```python
# CreateDeploymentGroupInputRequestTypeDef definition

class CreateDeploymentGroupInputRequestTypeDef(TypedDict):
    applicationName: str,
    deploymentGroupName: str,
    serviceRoleArn: str,
    deploymentConfigName: NotRequired[str],
    ec2TagFilters: NotRequired[Sequence[EC2TagFilterTypeDef]],  # (1)
    onPremisesInstanceTagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (2)
    autoScalingGroups: NotRequired[Sequence[str]],
    triggerConfigurations: NotRequired[Sequence[TriggerConfigUnionTypeDef]],  # (3)
    alarmConfiguration: NotRequired[AlarmConfigurationTypeDef],  # (4)
    autoRollbackConfiguration: NotRequired[AutoRollbackConfigurationTypeDef],  # (5)
    outdatedInstancesStrategy: NotRequired[OutdatedInstancesStrategyType],  # (6)
    deploymentStyle: NotRequired[DeploymentStyleTypeDef],  # (7)
    blueGreenDeploymentConfiguration: NotRequired[BlueGreenDeploymentConfigurationTypeDef],  # (8)
    loadBalancerInfo: NotRequired[LoadBalancerInfoTypeDef],  # (9)
    ec2TagSet: NotRequired[EC2TagSetTypeDef],  # (10)
    ecsServices: NotRequired[Sequence[ECSServiceTypeDef]],  # (11)
    onPremisesTagSet: NotRequired[OnPremisesTagSetTypeDef],  # (12)
    tags: NotRequired[Sequence[TagTypeDef]],  # (13)
    terminationHookEnabled: NotRequired[bool],
```

1. See [:material-code-braces: EC2TagFilterTypeDef](./type_defs.md#ec2tagfiltertypedef) 
2. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
3. See [:material-code-braces: TriggerConfigTypeDef](./type_defs.md#triggerconfigtypedef) [:material-code-braces: TriggerConfigOutputTypeDef](./type_defs.md#triggerconfigoutputtypedef) 
4. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) 
5. See [:material-code-braces: AutoRollbackConfigurationTypeDef](./type_defs.md#autorollbackconfigurationtypedef) 
6. See [:material-code-brackets: OutdatedInstancesStrategyType](./literals.md#outdatedinstancesstrategytype) 
7. See [:material-code-braces: DeploymentStyleTypeDef](./type_defs.md#deploymentstyletypedef) 
8. See [:material-code-braces: BlueGreenDeploymentConfigurationTypeDef](./type_defs.md#bluegreendeploymentconfigurationtypedef) 
9. See [:material-code-braces: LoadBalancerInfoTypeDef](./type_defs.md#loadbalancerinfotypedef) 
10. See [:material-code-braces: EC2TagSetTypeDef](./type_defs.md#ec2tagsettypedef) 
11. See [:material-code-braces: ECSServiceTypeDef](./type_defs.md#ecsservicetypedef) 
12. See [:material-code-braces: OnPremisesTagSetTypeDef](./type_defs.md#onpremisestagsettypedef) 
13. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateDeploymentGroupInputRequestTypeDef

```python
# UpdateDeploymentGroupInputRequestTypeDef definition

class UpdateDeploymentGroupInputRequestTypeDef(TypedDict):
    applicationName: str,
    currentDeploymentGroupName: str,
    newDeploymentGroupName: NotRequired[str],
    deploymentConfigName: NotRequired[str],
    ec2TagFilters: NotRequired[Sequence[EC2TagFilterTypeDef]],  # (1)
    onPremisesInstanceTagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (2)
    autoScalingGroups: NotRequired[Sequence[str]],
    serviceRoleArn: NotRequired[str],
    triggerConfigurations: NotRequired[Sequence[TriggerConfigTypeDef]],  # (3)
    alarmConfiguration: NotRequired[AlarmConfigurationTypeDef],  # (4)
    autoRollbackConfiguration: NotRequired[AutoRollbackConfigurationTypeDef],  # (5)
    outdatedInstancesStrategy: NotRequired[OutdatedInstancesStrategyType],  # (6)
    deploymentStyle: NotRequired[DeploymentStyleTypeDef],  # (7)
    blueGreenDeploymentConfiguration: NotRequired[BlueGreenDeploymentConfigurationTypeDef],  # (8)
    loadBalancerInfo: NotRequired[LoadBalancerInfoTypeDef],  # (9)
    ec2TagSet: NotRequired[EC2TagSetTypeDef],  # (10)
    ecsServices: NotRequired[Sequence[ECSServiceTypeDef]],  # (11)
    onPremisesTagSet: NotRequired[OnPremisesTagSetTypeDef],  # (12)
    terminationHookEnabled: NotRequired[bool],
```

1. See [:material-code-braces: EC2TagFilterTypeDef](./type_defs.md#ec2tagfiltertypedef) 
2. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
3. See [:material-code-braces: TriggerConfigTypeDef](./type_defs.md#triggerconfigtypedef) 
4. See [:material-code-braces: AlarmConfigurationTypeDef](./type_defs.md#alarmconfigurationtypedef) 
5. See [:material-code-braces: AutoRollbackConfigurationTypeDef](./type_defs.md#autorollbackconfigurationtypedef) 
6. See [:material-code-brackets: OutdatedInstancesStrategyType](./literals.md#outdatedinstancesstrategytype) 
7. See [:material-code-braces: DeploymentStyleTypeDef](./type_defs.md#deploymentstyletypedef) 
8. See [:material-code-braces: BlueGreenDeploymentConfigurationTypeDef](./type_defs.md#bluegreendeploymentconfigurationtypedef) 
9. See [:material-code-braces: LoadBalancerInfoTypeDef](./type_defs.md#loadbalancerinfotypedef) 
10. See [:material-code-braces: EC2TagSetTypeDef](./type_defs.md#ec2tagsettypedef) 
11. See [:material-code-braces: ECSServiceTypeDef](./type_defs.md#ecsservicetypedef) 
12. See [:material-code-braces: OnPremisesTagSetTypeDef](./type_defs.md#onpremisestagsettypedef) 
