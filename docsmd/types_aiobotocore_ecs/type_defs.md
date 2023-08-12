# Type definitions

> [Index](../README.md) > [ECS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ECS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
    type annotations stubs module [types-aiobotocore-ecs](https://pypi.org/project/types-aiobotocore-ecs/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AttachmentStateChangeTypeDef

```python
# AttachmentStateChangeTypeDef definition

class AttachmentStateChangeTypeDef(TypedDict):
    attachmentArn: str,
    status: str,
```

## KeyValuePairTypeDef

```python
# KeyValuePairTypeDef definition

class KeyValuePairTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
```

## AttributeTypeDef

```python
# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    name: str,
    value: NotRequired[str],
    targetType: NotRequired[TargetTypeType],  # (1)
    targetId: NotRequired[str],
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
## ManagedScalingTypeDef

```python
# ManagedScalingTypeDef definition

class ManagedScalingTypeDef(TypedDict):
    status: NotRequired[ManagedScalingStatusType],  # (1)
    targetCapacity: NotRequired[int],
    minimumScalingStepSize: NotRequired[int],
    maximumScalingStepSize: NotRequired[int],
    instanceWarmupPeriod: NotRequired[int],
```

1. See [:material-code-brackets: ManagedScalingStatusType](./literals.md#managedscalingstatustype) 
## AwsVpcConfigurationTypeDef

```python
# AwsVpcConfigurationTypeDef definition

class AwsVpcConfigurationTypeDef(TypedDict):
    subnets: Sequence[str],
    securityGroups: NotRequired[Sequence[str]],
    assignPublicIp: NotRequired[AssignPublicIpType],  # (1)
```

1. See [:material-code-brackets: AssignPublicIpType](./literals.md#assignpubliciptype) 
## CapacityProviderStrategyItemTypeDef

```python
# CapacityProviderStrategyItemTypeDef definition

class CapacityProviderStrategyItemTypeDef(TypedDict):
    capacityProvider: str,
    weight: NotRequired[int],
    base: NotRequired[int],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## ClusterServiceConnectDefaultsRequestTypeDef

```python
# ClusterServiceConnectDefaultsRequestTypeDef definition

class ClusterServiceConnectDefaultsRequestTypeDef(TypedDict):
    namespace: str,
```

## ClusterServiceConnectDefaultsTypeDef

```python
# ClusterServiceConnectDefaultsTypeDef definition

class ClusterServiceConnectDefaultsTypeDef(TypedDict):
    namespace: NotRequired[str],
```

## ClusterSettingTypeDef

```python
# ClusterSettingTypeDef definition

class ClusterSettingTypeDef(TypedDict):
    name: NotRequired[ClusterSettingNameType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: ClusterSettingNameType](./literals.md#clustersettingnametype) 
## ContainerDependencyTypeDef

```python
# ContainerDependencyTypeDef definition

class ContainerDependencyTypeDef(TypedDict):
    containerName: str,
    condition: ContainerConditionType,  # (1)
```

1. See [:material-code-brackets: ContainerConditionType](./literals.md#containerconditiontype) 
## EnvironmentFileTypeDef

```python
# EnvironmentFileTypeDef definition

class EnvironmentFileTypeDef(TypedDict):
    value: str,
    type: EnvironmentFileTypeType,  # (1)
```

1. See [:material-code-brackets: EnvironmentFileTypeType](./literals.md#environmentfiletypetype) 
## FirelensConfigurationTypeDef

```python
# FirelensConfigurationTypeDef definition

class FirelensConfigurationTypeDef(TypedDict):
    type: FirelensConfigurationTypeType,  # (1)
    options: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: FirelensConfigurationTypeType](./literals.md#firelensconfigurationtypetype) 
## HealthCheckTypeDef

```python
# HealthCheckTypeDef definition

class HealthCheckTypeDef(TypedDict):
    command: List[str],
    interval: NotRequired[int],
    timeout: NotRequired[int],
    retries: NotRequired[int],
    startPeriod: NotRequired[int],
```

## HostEntryTypeDef

```python
# HostEntryTypeDef definition

class HostEntryTypeDef(TypedDict):
    hostname: str,
    ipAddress: str,
```

## MountPointTypeDef

```python
# MountPointTypeDef definition

class MountPointTypeDef(TypedDict):
    sourceVolume: NotRequired[str],
    containerPath: NotRequired[str],
    readOnly: NotRequired[bool],
```

## PortMappingTypeDef

```python
# PortMappingTypeDef definition

class PortMappingTypeDef(TypedDict):
    containerPort: NotRequired[int],
    hostPort: NotRequired[int],
    protocol: NotRequired[TransportProtocolType],  # (1)
    name: NotRequired[str],
    appProtocol: NotRequired[ApplicationProtocolType],  # (2)
    containerPortRange: NotRequired[str],
```

1. See [:material-code-brackets: TransportProtocolType](./literals.md#transportprotocoltype) 
2. See [:material-code-brackets: ApplicationProtocolType](./literals.md#applicationprotocoltype) 
## RepositoryCredentialsTypeDef

```python
# RepositoryCredentialsTypeDef definition

class RepositoryCredentialsTypeDef(TypedDict):
    credentialsParameter: str,
```

## ResourceRequirementTypeDef

```python
# ResourceRequirementTypeDef definition

class ResourceRequirementTypeDef(TypedDict):
    value: str,
    type: ResourceTypeType,  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## SecretTypeDef

```python
# SecretTypeDef definition

class SecretTypeDef(TypedDict):
    name: str,
    valueFrom: str,
```

## SystemControlTypeDef

```python
# SystemControlTypeDef definition

class SystemControlTypeDef(TypedDict):
    namespace: NotRequired[str],
    value: NotRequired[str],
```

## UlimitTypeDef

```python
# UlimitTypeDef definition

class UlimitTypeDef(TypedDict):
    name: UlimitNameType,  # (1)
    softLimit: int,
    hardLimit: int,
```

1. See [:material-code-brackets: UlimitNameType](./literals.md#ulimitnametype) 
## VolumeFromTypeDef

```python
# VolumeFromTypeDef definition

class VolumeFromTypeDef(TypedDict):
    sourceContainer: NotRequired[str],
    readOnly: NotRequired[bool],
```

## InstanceHealthCheckResultTypeDef

```python
# InstanceHealthCheckResultTypeDef definition

class InstanceHealthCheckResultTypeDef(TypedDict):
    type: NotRequired[InstanceHealthCheckTypeType],  # (1)
    status: NotRequired[InstanceHealthCheckStateType],  # (2)
    lastUpdated: NotRequired[datetime],
    lastStatusChange: NotRequired[datetime],
```

1. See [:material-code-brackets: InstanceHealthCheckTypeType](./literals.md#instancehealthchecktypetype) 
2. See [:material-code-brackets: InstanceHealthCheckStateType](./literals.md#instancehealthcheckstatetype) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    doubleValue: NotRequired[float],
    longValue: NotRequired[int],
    integerValue: NotRequired[int],
    stringSetValue: NotRequired[List[str]],
```

## VersionInfoTypeDef

```python
# VersionInfoTypeDef definition

class VersionInfoTypeDef(TypedDict):
    agentVersion: NotRequired[str],
    agentHash: NotRequired[str],
    dockerVersion: NotRequired[str],
```

## NetworkBindingTypeDef

```python
# NetworkBindingTypeDef definition

class NetworkBindingTypeDef(TypedDict):
    bindIP: NotRequired[str],
    containerPort: NotRequired[int],
    hostPort: NotRequired[int],
    protocol: NotRequired[TransportProtocolType],  # (1)
    containerPortRange: NotRequired[str],
    hostPortRange: NotRequired[str],
```

1. See [:material-code-brackets: TransportProtocolType](./literals.md#transportprotocoltype) 
## ManagedAgentTypeDef

```python
# ManagedAgentTypeDef definition

class ManagedAgentTypeDef(TypedDict):
    lastStartedAt: NotRequired[datetime],
    name: NotRequired[ManagedAgentNameType],  # (1)
    reason: NotRequired[str],
    lastStatus: NotRequired[str],
```

1. See [:material-code-brackets: ManagedAgentNameType](./literals.md#managedagentnametype) 
## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    attachmentId: NotRequired[str],
    privateIpv4Address: NotRequired[str],
    ipv6Address: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## DeploymentControllerTypeDef

```python
# DeploymentControllerTypeDef definition

class DeploymentControllerTypeDef(TypedDict):
    type: DeploymentControllerTypeType,  # (1)
```

1. See [:material-code-brackets: DeploymentControllerTypeType](./literals.md#deploymentcontrollertypetype) 
## LoadBalancerTypeDef

```python
# LoadBalancerTypeDef definition

class LoadBalancerTypeDef(TypedDict):
    targetGroupArn: NotRequired[str],
    loadBalancerName: NotRequired[str],
    containerName: NotRequired[str],
    containerPort: NotRequired[int],
```

## PlacementConstraintTypeDef

```python
# PlacementConstraintTypeDef definition

class PlacementConstraintTypeDef(TypedDict):
    type: NotRequired[PlacementConstraintTypeType],  # (1)
    expression: NotRequired[str],
```

1. See [:material-code-brackets: PlacementConstraintTypeType](./literals.md#placementconstrainttypetype) 
## PlacementStrategyTypeDef

```python
# PlacementStrategyTypeDef definition

class PlacementStrategyTypeDef(TypedDict):
    type: NotRequired[PlacementStrategyTypeType],  # (1)
    field: NotRequired[str],
```

1. See [:material-code-brackets: PlacementStrategyTypeType](./literals.md#placementstrategytypetype) 
## ServiceRegistryTypeDef

```python
# ServiceRegistryTypeDef definition

class ServiceRegistryTypeDef(TypedDict):
    registryArn: NotRequired[str],
    port: NotRequired[int],
    containerName: NotRequired[str],
    containerPort: NotRequired[int],
```

## ScaleTypeDef

```python
# ScaleTypeDef definition

class ScaleTypeDef(TypedDict):
    value: NotRequired[float],
    unit: NotRequired[ScaleUnitType],  # (1)
```

1. See [:material-code-brackets: ScaleUnitType](./literals.md#scaleunittype) 
## DeleteAccountSettingRequestRequestTypeDef

```python
# DeleteAccountSettingRequestRequestTypeDef definition

class DeleteAccountSettingRequestRequestTypeDef(TypedDict):
    name: SettingNameType,  # (1)
    principalArn: NotRequired[str],
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
## SettingTypeDef

```python
# SettingTypeDef definition

class SettingTypeDef(TypedDict):
    name: NotRequired[SettingNameType],  # (1)
    value: NotRequired[str],
    principalArn: NotRequired[str],
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
## DeleteCapacityProviderRequestRequestTypeDef

```python
# DeleteCapacityProviderRequestRequestTypeDef definition

class DeleteCapacityProviderRequestRequestTypeDef(TypedDict):
    capacityProvider: str,
```

## DeleteClusterRequestRequestTypeDef

```python
# DeleteClusterRequestRequestTypeDef definition

class DeleteClusterRequestRequestTypeDef(TypedDict):
    cluster: str,
```

## DeleteServiceRequestRequestTypeDef

```python
# DeleteServiceRequestRequestTypeDef definition

class DeleteServiceRequestRequestTypeDef(TypedDict):
    service: str,
    cluster: NotRequired[str],
    force: NotRequired[bool],
```

## DeleteTaskDefinitionsRequestRequestTypeDef

```python
# DeleteTaskDefinitionsRequestRequestTypeDef definition

class DeleteTaskDefinitionsRequestRequestTypeDef(TypedDict):
    taskDefinitions: Sequence[str],
```

## FailureTypeDef

```python
# FailureTypeDef definition

class FailureTypeDef(TypedDict):
    arn: NotRequired[str],
    reason: NotRequired[str],
    detail: NotRequired[str],
```

## DeleteTaskSetRequestRequestTypeDef

```python
# DeleteTaskSetRequestRequestTypeDef definition

class DeleteTaskSetRequestRequestTypeDef(TypedDict):
    cluster: str,
    service: str,
    taskSet: str,
    force: NotRequired[bool],
```

## DeploymentAlarmsTypeDef

```python
# DeploymentAlarmsTypeDef definition

class DeploymentAlarmsTypeDef(TypedDict):
    alarmNames: Sequence[str],
    enable: bool,
    rollback: bool,
```

## DeploymentCircuitBreakerTypeDef

```python
# DeploymentCircuitBreakerTypeDef definition

class DeploymentCircuitBreakerTypeDef(TypedDict):
    enable: bool,
    rollback: bool,
```

## ServiceConnectServiceResourceTypeDef

```python
# ServiceConnectServiceResourceTypeDef definition

class ServiceConnectServiceResourceTypeDef(TypedDict):
    discoveryName: NotRequired[str],
    discoveryArn: NotRequired[str],
```

## DeregisterContainerInstanceRequestRequestTypeDef

```python
# DeregisterContainerInstanceRequestRequestTypeDef definition

class DeregisterContainerInstanceRequestRequestTypeDef(TypedDict):
    containerInstance: str,
    cluster: NotRequired[str],
    force: NotRequired[bool],
```

## DeregisterTaskDefinitionRequestRequestTypeDef

```python
# DeregisterTaskDefinitionRequestRequestTypeDef definition

class DeregisterTaskDefinitionRequestRequestTypeDef(TypedDict):
    taskDefinition: str,
```

## DescribeCapacityProvidersRequestRequestTypeDef

```python
# DescribeCapacityProvidersRequestRequestTypeDef definition

class DescribeCapacityProvidersRequestRequestTypeDef(TypedDict):
    capacityProviders: NotRequired[Sequence[str]],
    include: NotRequired[Sequence[CapacityProviderFieldType]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: CapacityProviderFieldType](./literals.md#capacityproviderfieldtype) 
## DescribeClustersRequestRequestTypeDef

```python
# DescribeClustersRequestRequestTypeDef definition

class DescribeClustersRequestRequestTypeDef(TypedDict):
    clusters: NotRequired[Sequence[str]],
    include: NotRequired[Sequence[ClusterFieldType]],  # (1)
```

1. See [:material-code-brackets: ClusterFieldType](./literals.md#clusterfieldtype) 
## DescribeContainerInstancesRequestRequestTypeDef

```python
# DescribeContainerInstancesRequestRequestTypeDef definition

class DescribeContainerInstancesRequestRequestTypeDef(TypedDict):
    containerInstances: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[ContainerInstanceFieldType]],  # (1)
```

1. See [:material-code-brackets: ContainerInstanceFieldType](./literals.md#containerinstancefieldtype) 
## DescribeServicesRequestRequestTypeDef

```python
# DescribeServicesRequestRequestTypeDef definition

class DescribeServicesRequestRequestTypeDef(TypedDict):
    services: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[ServiceFieldType]],  # (1)
```

1. See [:material-code-brackets: ServiceFieldType](./literals.md#servicefieldtype) 
## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeTaskDefinitionRequestRequestTypeDef

```python
# DescribeTaskDefinitionRequestRequestTypeDef definition

class DescribeTaskDefinitionRequestRequestTypeDef(TypedDict):
    taskDefinition: str,
    include: NotRequired[Sequence[TaskDefinitionFieldType]],  # (1)
```

1. See [:material-code-brackets: TaskDefinitionFieldType](./literals.md#taskdefinitionfieldtype) 
## DescribeTaskSetsRequestRequestTypeDef

```python
# DescribeTaskSetsRequestRequestTypeDef definition

class DescribeTaskSetsRequestRequestTypeDef(TypedDict):
    cluster: str,
    service: str,
    taskSets: NotRequired[Sequence[str]],
    include: NotRequired[Sequence[TaskSetFieldType]],  # (1)
```

1. See [:material-code-brackets: TaskSetFieldType](./literals.md#tasksetfieldtype) 
## DescribeTasksRequestRequestTypeDef

```python
# DescribeTasksRequestRequestTypeDef definition

class DescribeTasksRequestRequestTypeDef(TypedDict):
    tasks: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[TaskFieldType]],  # (1)
```

1. See [:material-code-brackets: TaskFieldType](./literals.md#taskfieldtype) 
## DeviceTypeDef

```python
# DeviceTypeDef definition

class DeviceTypeDef(TypedDict):
    hostPath: str,
    containerPath: NotRequired[str],
    permissions: NotRequired[List[DeviceCgroupPermissionType]],  # (1)
```

1. See [:material-code-brackets: DeviceCgroupPermissionType](./literals.md#devicecgrouppermissiontype) 
## DiscoverPollEndpointRequestRequestTypeDef

```python
# DiscoverPollEndpointRequestRequestTypeDef definition

class DiscoverPollEndpointRequestRequestTypeDef(TypedDict):
    containerInstance: NotRequired[str],
    cluster: NotRequired[str],
```

## DockerVolumeConfigurationTypeDef

```python
# DockerVolumeConfigurationTypeDef definition

class DockerVolumeConfigurationTypeDef(TypedDict):
    scope: NotRequired[ScopeType],  # (1)
    autoprovision: NotRequired[bool],
    driver: NotRequired[str],
    driverOpts: NotRequired[Dict[str, str]],
    labels: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## EFSAuthorizationConfigTypeDef

```python
# EFSAuthorizationConfigTypeDef definition

class EFSAuthorizationConfigTypeDef(TypedDict):
    accessPointId: NotRequired[str],
    iam: NotRequired[EFSAuthorizationConfigIAMType],  # (1)
```

1. See [:material-code-brackets: EFSAuthorizationConfigIAMType](./literals.md#efsauthorizationconfigiamtype) 
## EphemeralStorageTypeDef

```python
# EphemeralStorageTypeDef definition

class EphemeralStorageTypeDef(TypedDict):
    sizeInGiB: int,
```

## ExecuteCommandLogConfigurationTypeDef

```python
# ExecuteCommandLogConfigurationTypeDef definition

class ExecuteCommandLogConfigurationTypeDef(TypedDict):
    cloudWatchLogGroupName: NotRequired[str],
    cloudWatchEncryptionEnabled: NotRequired[bool],
    s3BucketName: NotRequired[str],
    s3EncryptionEnabled: NotRequired[bool],
    s3KeyPrefix: NotRequired[str],
```

## ExecuteCommandRequestRequestTypeDef

```python
# ExecuteCommandRequestRequestTypeDef definition

class ExecuteCommandRequestRequestTypeDef(TypedDict):
    command: str,
    interactive: bool,
    task: str,
    cluster: NotRequired[str],
    container: NotRequired[str],
```

## SessionTypeDef

```python
# SessionTypeDef definition

class SessionTypeDef(TypedDict):
    sessionId: NotRequired[str],
    streamUrl: NotRequired[str],
    tokenValue: NotRequired[str],
```

## FSxWindowsFileServerAuthorizationConfigTypeDef

```python
# FSxWindowsFileServerAuthorizationConfigTypeDef definition

class FSxWindowsFileServerAuthorizationConfigTypeDef(TypedDict):
    credentialsParameter: str,
    domain: str,
```

## GetTaskProtectionRequestRequestTypeDef

```python
# GetTaskProtectionRequestRequestTypeDef definition

class GetTaskProtectionRequestRequestTypeDef(TypedDict):
    cluster: str,
    tasks: NotRequired[Sequence[str]],
```

## ProtectedTaskTypeDef

```python
# ProtectedTaskTypeDef definition

class ProtectedTaskTypeDef(TypedDict):
    taskArn: NotRequired[str],
    protectionEnabled: NotRequired[bool],
    expirationDate: NotRequired[datetime],
```

## HostVolumePropertiesTypeDef

```python
# HostVolumePropertiesTypeDef definition

class HostVolumePropertiesTypeDef(TypedDict):
    sourcePath: NotRequired[str],
```

## InferenceAcceleratorOverrideTypeDef

```python
# InferenceAcceleratorOverrideTypeDef definition

class InferenceAcceleratorOverrideTypeDef(TypedDict):
    deviceName: NotRequired[str],
    deviceType: NotRequired[str],
```

## InferenceAcceleratorTypeDef

```python
# InferenceAcceleratorTypeDef definition

class InferenceAcceleratorTypeDef(TypedDict):
    deviceName: str,
    deviceType: str,
```

## KernelCapabilitiesTypeDef

```python
# KernelCapabilitiesTypeDef definition

class KernelCapabilitiesTypeDef(TypedDict):
    add: NotRequired[List[str]],
    drop: NotRequired[List[str]],
```

## TmpfsTypeDef

```python
# TmpfsTypeDef definition

class TmpfsTypeDef(TypedDict):
    containerPath: str,
    size: int,
    mountOptions: NotRequired[List[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAccountSettingsRequestRequestTypeDef

```python
# ListAccountSettingsRequestRequestTypeDef definition

class ListAccountSettingsRequestRequestTypeDef(TypedDict):
    name: NotRequired[SettingNameType],  # (1)
    value: NotRequired[str],
    principalArn: NotRequired[str],
    effectiveSettings: NotRequired[bool],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
## ListAttributesRequestRequestTypeDef

```python
# ListAttributesRequestRequestTypeDef definition

class ListAttributesRequestRequestTypeDef(TypedDict):
    targetType: TargetTypeType,  # (1)
    cluster: NotRequired[str],
    attributeName: NotRequired[str],
    attributeValue: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
## ListClustersRequestRequestTypeDef

```python
# ListClustersRequestRequestTypeDef definition

class ListClustersRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListContainerInstancesRequestRequestTypeDef

```python
# ListContainerInstancesRequestRequestTypeDef definition

class ListContainerInstancesRequestRequestTypeDef(TypedDict):
    cluster: NotRequired[str],
    filter: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    status: NotRequired[ContainerInstanceStatusType],  # (1)
```

1. See [:material-code-brackets: ContainerInstanceStatusType](./literals.md#containerinstancestatustype) 
## ListServicesByNamespaceRequestRequestTypeDef

```python
# ListServicesByNamespaceRequestRequestTypeDef definition

class ListServicesByNamespaceRequestRequestTypeDef(TypedDict):
    namespace: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListServicesRequestRequestTypeDef

```python
# ListServicesRequestRequestTypeDef definition

class ListServicesRequestRequestTypeDef(TypedDict):
    cluster: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    launchType: NotRequired[LaunchTypeType],  # (1)
    schedulingStrategy: NotRequired[SchedulingStrategyType],  # (2)
```

1. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
2. See [:material-code-brackets: SchedulingStrategyType](./literals.md#schedulingstrategytype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTaskDefinitionFamiliesRequestRequestTypeDef

```python
# ListTaskDefinitionFamiliesRequestRequestTypeDef definition

class ListTaskDefinitionFamiliesRequestRequestTypeDef(TypedDict):
    familyPrefix: NotRequired[str],
    status: NotRequired[TaskDefinitionFamilyStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TaskDefinitionFamilyStatusType](./literals.md#taskdefinitionfamilystatustype) 
## ListTaskDefinitionsRequestRequestTypeDef

```python
# ListTaskDefinitionsRequestRequestTypeDef definition

class ListTaskDefinitionsRequestRequestTypeDef(TypedDict):
    familyPrefix: NotRequired[str],
    status: NotRequired[TaskDefinitionStatusType],  # (1)
    sort: NotRequired[SortOrderType],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TaskDefinitionStatusType](./literals.md#taskdefinitionstatustype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListTasksRequestRequestTypeDef

```python
# ListTasksRequestRequestTypeDef definition

class ListTasksRequestRequestTypeDef(TypedDict):
    cluster: NotRequired[str],
    containerInstance: NotRequired[str],
    family: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    startedBy: NotRequired[str],
    serviceName: NotRequired[str],
    desiredStatus: NotRequired[DesiredStatusType],  # (1)
    launchType: NotRequired[LaunchTypeType],  # (2)
```

1. See [:material-code-brackets: DesiredStatusType](./literals.md#desiredstatustype) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
## ManagedAgentStateChangeTypeDef

```python
# ManagedAgentStateChangeTypeDef definition

class ManagedAgentStateChangeTypeDef(TypedDict):
    containerName: str,
    managedAgentName: ManagedAgentNameType,  # (1)
    status: str,
    reason: NotRequired[str],
```

1. See [:material-code-brackets: ManagedAgentNameType](./literals.md#managedagentnametype) 
## PlatformDeviceTypeDef

```python
# PlatformDeviceTypeDef definition

class PlatformDeviceTypeDef(TypedDict):
    id: str,
    type: PlatformDeviceTypeType,  # (1)
```

1. See [:material-code-brackets: PlatformDeviceTypeType](./literals.md#platformdevicetypetype) 
## PutAccountSettingDefaultRequestRequestTypeDef

```python
# PutAccountSettingDefaultRequestRequestTypeDef definition

class PutAccountSettingDefaultRequestRequestTypeDef(TypedDict):
    name: SettingNameType,  # (1)
    value: str,
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
## PutAccountSettingRequestRequestTypeDef

```python
# PutAccountSettingRequestRequestTypeDef definition

class PutAccountSettingRequestRequestTypeDef(TypedDict):
    name: SettingNameType,  # (1)
    value: str,
    principalArn: NotRequired[str],
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
## RuntimePlatformTypeDef

```python
# RuntimePlatformTypeDef definition

class RuntimePlatformTypeDef(TypedDict):
    cpuArchitecture: NotRequired[CPUArchitectureType],  # (1)
    operatingSystemFamily: NotRequired[OSFamilyType],  # (2)
```

1. See [:material-code-brackets: CPUArchitectureType](./literals.md#cpuarchitecturetype) 
2. See [:material-code-brackets: OSFamilyType](./literals.md#osfamilytype) 
## TaskDefinitionPlacementConstraintTypeDef

```python
# TaskDefinitionPlacementConstraintTypeDef definition

class TaskDefinitionPlacementConstraintTypeDef(TypedDict):
    type: NotRequired[TaskDefinitionPlacementConstraintTypeType],  # (1)
    expression: NotRequired[str],
```

1. See [:material-code-brackets: TaskDefinitionPlacementConstraintTypeType](./literals.md#taskdefinitionplacementconstrainttypetype) 
## ServiceConnectClientAliasTypeDef

```python
# ServiceConnectClientAliasTypeDef definition

class ServiceConnectClientAliasTypeDef(TypedDict):
    port: int,
    dnsName: NotRequired[str],
```

## ServiceEventTypeDef

```python
# ServiceEventTypeDef definition

class ServiceEventTypeDef(TypedDict):
    id: NotRequired[str],
    createdAt: NotRequired[datetime],
    message: NotRequired[str],
```

## StopTaskRequestRequestTypeDef

```python
# StopTaskRequestRequestTypeDef definition

class StopTaskRequestRequestTypeDef(TypedDict):
    task: str,
    cluster: NotRequired[str],
    reason: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateContainerAgentRequestRequestTypeDef

```python
# UpdateContainerAgentRequestRequestTypeDef definition

class UpdateContainerAgentRequestRequestTypeDef(TypedDict):
    containerInstance: str,
    cluster: NotRequired[str],
```

## UpdateContainerInstancesStateRequestRequestTypeDef

```python
# UpdateContainerInstancesStateRequestRequestTypeDef definition

class UpdateContainerInstancesStateRequestRequestTypeDef(TypedDict):
    containerInstances: Sequence[str],
    status: ContainerInstanceStatusType,  # (1)
    cluster: NotRequired[str],
```

1. See [:material-code-brackets: ContainerInstanceStatusType](./literals.md#containerinstancestatustype) 
## UpdateServicePrimaryTaskSetRequestRequestTypeDef

```python
# UpdateServicePrimaryTaskSetRequestRequestTypeDef definition

class UpdateServicePrimaryTaskSetRequestRequestTypeDef(TypedDict):
    cluster: str,
    service: str,
    primaryTaskSet: str,
```

## UpdateTaskProtectionRequestRequestTypeDef

```python
# UpdateTaskProtectionRequestRequestTypeDef definition

class UpdateTaskProtectionRequestRequestTypeDef(TypedDict):
    cluster: str,
    tasks: Sequence[str],
    protectionEnabled: bool,
    expiresInMinutes: NotRequired[int],
```

## SubmitAttachmentStateChangesRequestRequestTypeDef

```python
# SubmitAttachmentStateChangesRequestRequestTypeDef definition

class SubmitAttachmentStateChangesRequestRequestTypeDef(TypedDict):
    attachments: Sequence[AttachmentStateChangeTypeDef],  # (1)
    cluster: NotRequired[str],
```

1. See [:material-code-braces: AttachmentStateChangeTypeDef](./type_defs.md#attachmentstatechangetypedef) 
## AttachmentTypeDef

```python
# AttachmentTypeDef definition

class AttachmentTypeDef(TypedDict):
    id: NotRequired[str],
    type: NotRequired[str],
    status: NotRequired[str],
    details: NotRequired[List[KeyValuePairTypeDef]],  # (1)
```

1. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
## ProxyConfigurationTypeDef

```python
# ProxyConfigurationTypeDef definition

class ProxyConfigurationTypeDef(TypedDict):
    containerName: str,
    type: NotRequired[ProxyConfigurationTypeType],  # (1)
    properties: NotRequired[List[KeyValuePairTypeDef]],  # (2)
```

1. See [:material-code-brackets: ProxyConfigurationTypeType](./literals.md#proxyconfigurationtypetype) 
2. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
## DeleteAttributesRequestRequestTypeDef

```python
# DeleteAttributesRequestRequestTypeDef definition

class DeleteAttributesRequestRequestTypeDef(TypedDict):
    attributes: Sequence[AttributeTypeDef],  # (1)
    cluster: NotRequired[str],
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## PutAttributesRequestRequestTypeDef

```python
# PutAttributesRequestRequestTypeDef definition

class PutAttributesRequestRequestTypeDef(TypedDict):
    attributes: Sequence[AttributeTypeDef],  # (1)
    cluster: NotRequired[str],
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## AutoScalingGroupProviderTypeDef

```python
# AutoScalingGroupProviderTypeDef definition

class AutoScalingGroupProviderTypeDef(TypedDict):
    autoScalingGroupArn: str,
    managedScaling: NotRequired[ManagedScalingTypeDef],  # (1)
    managedTerminationProtection: NotRequired[ManagedTerminationProtectionType],  # (2)
```

1. See [:material-code-braces: ManagedScalingTypeDef](./type_defs.md#managedscalingtypedef) 
2. See [:material-code-brackets: ManagedTerminationProtectionType](./literals.md#managedterminationprotectiontype) 
## AutoScalingGroupProviderUpdateTypeDef

```python
# AutoScalingGroupProviderUpdateTypeDef definition

class AutoScalingGroupProviderUpdateTypeDef(TypedDict):
    managedScaling: NotRequired[ManagedScalingTypeDef],  # (1)
    managedTerminationProtection: NotRequired[ManagedTerminationProtectionType],  # (2)
```

1. See [:material-code-braces: ManagedScalingTypeDef](./type_defs.md#managedscalingtypedef) 
2. See [:material-code-brackets: ManagedTerminationProtectionType](./literals.md#managedterminationprotectiontype) 
## NetworkConfigurationTypeDef

```python
# NetworkConfigurationTypeDef definition

class NetworkConfigurationTypeDef(TypedDict):
    awsvpcConfiguration: NotRequired[AwsVpcConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AwsVpcConfigurationTypeDef](./type_defs.md#awsvpcconfigurationtypedef) 
## PutClusterCapacityProvidersRequestRequestTypeDef

```python
# PutClusterCapacityProvidersRequestRequestTypeDef definition

class PutClusterCapacityProvidersRequestRequestTypeDef(TypedDict):
    cluster: str,
    capacityProviders: Sequence[str],
    defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef],  # (1)
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateClusterSettingsRequestRequestTypeDef

```python
# UpdateClusterSettingsRequestRequestTypeDef definition

class UpdateClusterSettingsRequestRequestTypeDef(TypedDict):
    cluster: str,
    settings: Sequence[ClusterSettingTypeDef],  # (1)
```

1. See [:material-code-braces: ClusterSettingTypeDef](./type_defs.md#clustersettingtypedef) 
## ContainerOverrideTypeDef

```python
# ContainerOverrideTypeDef definition

class ContainerOverrideTypeDef(TypedDict):
    name: NotRequired[str],
    command: NotRequired[List[str]],
    environment: NotRequired[List[KeyValuePairTypeDef]],  # (1)
    environmentFiles: NotRequired[List[EnvironmentFileTypeDef]],  # (2)
    cpu: NotRequired[int],
    memory: NotRequired[int],
    memoryReservation: NotRequired[int],
    resourceRequirements: NotRequired[List[ResourceRequirementTypeDef]],  # (3)
```

1. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
2. See [:material-code-braces: EnvironmentFileTypeDef](./type_defs.md#environmentfiletypedef) 
3. See [:material-code-braces: ResourceRequirementTypeDef](./type_defs.md#resourcerequirementtypedef) 
## LogConfigurationTypeDef

```python
# LogConfigurationTypeDef definition

class LogConfigurationTypeDef(TypedDict):
    logDriver: LogDriverType,  # (1)
    options: NotRequired[Mapping[str, str]],
    secretOptions: NotRequired[Sequence[SecretTypeDef]],  # (2)
```

1. See [:material-code-brackets: LogDriverType](./literals.md#logdrivertype) 
2. See [:material-code-braces: SecretTypeDef](./type_defs.md#secrettypedef) 
## ContainerInstanceHealthStatusTypeDef

```python
# ContainerInstanceHealthStatusTypeDef definition

class ContainerInstanceHealthStatusTypeDef(TypedDict):
    overallStatus: NotRequired[InstanceHealthCheckStateType],  # (1)
    details: NotRequired[List[InstanceHealthCheckResultTypeDef]],  # (2)
```

1. See [:material-code-brackets: InstanceHealthCheckStateType](./literals.md#instancehealthcheckstatetype) 
2. See [:material-code-braces: InstanceHealthCheckResultTypeDef](./type_defs.md#instancehealthcheckresulttypedef) 
## ContainerStateChangeTypeDef

```python
# ContainerStateChangeTypeDef definition

class ContainerStateChangeTypeDef(TypedDict):
    containerName: NotRequired[str],
    imageDigest: NotRequired[str],
    runtimeId: NotRequired[str],
    exitCode: NotRequired[int],
    networkBindings: NotRequired[Sequence[NetworkBindingTypeDef]],  # (1)
    reason: NotRequired[str],
    status: NotRequired[str],
```

1. See [:material-code-braces: NetworkBindingTypeDef](./type_defs.md#networkbindingtypedef) 
## SubmitContainerStateChangeRequestRequestTypeDef

```python
# SubmitContainerStateChangeRequestRequestTypeDef definition

class SubmitContainerStateChangeRequestRequestTypeDef(TypedDict):
    cluster: NotRequired[str],
    task: NotRequired[str],
    containerName: NotRequired[str],
    runtimeId: NotRequired[str],
    status: NotRequired[str],
    exitCode: NotRequired[int],
    reason: NotRequired[str],
    networkBindings: NotRequired[Sequence[NetworkBindingTypeDef]],  # (1)
```

1. See [:material-code-braces: NetworkBindingTypeDef](./type_defs.md#networkbindingtypedef) 
## ContainerTypeDef

```python
# ContainerTypeDef definition

class ContainerTypeDef(TypedDict):
    containerArn: NotRequired[str],
    taskArn: NotRequired[str],
    name: NotRequired[str],
    image: NotRequired[str],
    imageDigest: NotRequired[str],
    runtimeId: NotRequired[str],
    lastStatus: NotRequired[str],
    exitCode: NotRequired[int],
    reason: NotRequired[str],
    networkBindings: NotRequired[List[NetworkBindingTypeDef]],  # (1)
    networkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (2)
    healthStatus: NotRequired[HealthStatusType],  # (3)
    managedAgents: NotRequired[List[ManagedAgentTypeDef]],  # (4)
    cpu: NotRequired[str],
    memory: NotRequired[str],
    memoryReservation: NotRequired[str],
    gpuIds: NotRequired[List[str]],
```

1. See [:material-code-braces: NetworkBindingTypeDef](./type_defs.md#networkbindingtypedef) 
2. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
3. See [:material-code-brackets: HealthStatusType](./literals.md#healthstatustype) 
4. See [:material-code-braces: ManagedAgentTypeDef](./type_defs.md#managedagenttypedef) 
## DeleteAttributesResponseTypeDef

```python
# DeleteAttributesResponseTypeDef definition

class DeleteAttributesResponseTypeDef(TypedDict):
    attributes: List[AttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DiscoverPollEndpointResponseTypeDef

```python
# DiscoverPollEndpointResponseTypeDef definition

class DiscoverPollEndpointResponseTypeDef(TypedDict):
    endpoint: str,
    telemetryEndpoint: str,
    serviceConnectEndpoint: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAttributesResponseTypeDef

```python
# ListAttributesResponseTypeDef definition

class ListAttributesResponseTypeDef(TypedDict):
    attributes: List[AttributeTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersResponseTypeDef

```python
# ListClustersResponseTypeDef definition

class ListClustersResponseTypeDef(TypedDict):
    clusterArns: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContainerInstancesResponseTypeDef

```python
# ListContainerInstancesResponseTypeDef definition

class ListContainerInstancesResponseTypeDef(TypedDict):
    containerInstanceArns: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServicesByNamespaceResponseTypeDef

```python
# ListServicesByNamespaceResponseTypeDef definition

class ListServicesByNamespaceResponseTypeDef(TypedDict):
    serviceArns: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServicesResponseTypeDef

```python
# ListServicesResponseTypeDef definition

class ListServicesResponseTypeDef(TypedDict):
    serviceArns: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTaskDefinitionFamiliesResponseTypeDef

```python
# ListTaskDefinitionFamiliesResponseTypeDef definition

class ListTaskDefinitionFamiliesResponseTypeDef(TypedDict):
    families: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTaskDefinitionsResponseTypeDef

```python
# ListTaskDefinitionsResponseTypeDef definition

class ListTaskDefinitionsResponseTypeDef(TypedDict):
    taskDefinitionArns: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTasksResponseTypeDef

```python
# ListTasksResponseTypeDef definition

class ListTasksResponseTypeDef(TypedDict):
    taskArns: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAttributesResponseTypeDef

```python
# PutAttributesResponseTypeDef definition

class PutAttributesResponseTypeDef(TypedDict):
    attributes: List[AttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubmitAttachmentStateChangesResponseTypeDef

```python
# SubmitAttachmentStateChangesResponseTypeDef definition

class SubmitAttachmentStateChangesResponseTypeDef(TypedDict):
    acknowledgment: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubmitContainerStateChangeResponseTypeDef

```python
# SubmitContainerStateChangeResponseTypeDef definition

class SubmitContainerStateChangeResponseTypeDef(TypedDict):
    acknowledgment: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubmitTaskStateChangeResponseTypeDef

```python
# SubmitTaskStateChangeResponseTypeDef definition

class SubmitTaskStateChangeResponseTypeDef(TypedDict):
    acknowledgment: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTaskSetRequestRequestTypeDef

```python
# UpdateTaskSetRequestRequestTypeDef definition

class UpdateTaskSetRequestRequestTypeDef(TypedDict):
    cluster: str,
    service: str,
    taskSet: str,
    scale: ScaleTypeDef,  # (1)
```

1. See [:material-code-braces: ScaleTypeDef](./type_defs.md#scaletypedef) 
## DeleteAccountSettingResponseTypeDef

```python
# DeleteAccountSettingResponseTypeDef definition

class DeleteAccountSettingResponseTypeDef(TypedDict):
    setting: SettingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SettingTypeDef](./type_defs.md#settingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountSettingsResponseTypeDef

```python
# ListAccountSettingsResponseTypeDef definition

class ListAccountSettingsResponseTypeDef(TypedDict):
    settings: List[SettingTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SettingTypeDef](./type_defs.md#settingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAccountSettingDefaultResponseTypeDef

```python
# PutAccountSettingDefaultResponseTypeDef definition

class PutAccountSettingDefaultResponseTypeDef(TypedDict):
    setting: SettingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SettingTypeDef](./type_defs.md#settingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAccountSettingResponseTypeDef

```python
# PutAccountSettingResponseTypeDef definition

class PutAccountSettingResponseTypeDef(TypedDict):
    setting: SettingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SettingTypeDef](./type_defs.md#settingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentConfigurationTypeDef

```python
# DeploymentConfigurationTypeDef definition

class DeploymentConfigurationTypeDef(TypedDict):
    deploymentCircuitBreaker: NotRequired[DeploymentCircuitBreakerTypeDef],  # (1)
    maximumPercent: NotRequired[int],
    minimumHealthyPercent: NotRequired[int],
    alarms: NotRequired[DeploymentAlarmsTypeDef],  # (2)
```

1. See [:material-code-braces: DeploymentCircuitBreakerTypeDef](./type_defs.md#deploymentcircuitbreakertypedef) 
2. See [:material-code-braces: DeploymentAlarmsTypeDef](./type_defs.md#deploymentalarmstypedef) 
## DescribeServicesRequestServicesInactiveWaitTypeDef

```python
# DescribeServicesRequestServicesInactiveWaitTypeDef definition

class DescribeServicesRequestServicesInactiveWaitTypeDef(TypedDict):
    services: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[ServiceFieldType]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceFieldType](./literals.md#servicefieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeServicesRequestServicesStableWaitTypeDef

```python
# DescribeServicesRequestServicesStableWaitTypeDef definition

class DescribeServicesRequestServicesStableWaitTypeDef(TypedDict):
    services: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[ServiceFieldType]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceFieldType](./literals.md#servicefieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTasksRequestTasksRunningWaitTypeDef

```python
# DescribeTasksRequestTasksRunningWaitTypeDef definition

class DescribeTasksRequestTasksRunningWaitTypeDef(TypedDict):
    tasks: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[TaskFieldType]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskFieldType](./literals.md#taskfieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTasksRequestTasksStoppedWaitTypeDef

```python
# DescribeTasksRequestTasksStoppedWaitTypeDef definition

class DescribeTasksRequestTasksStoppedWaitTypeDef(TypedDict):
    tasks: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[TaskFieldType]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskFieldType](./literals.md#taskfieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## EFSVolumeConfigurationTypeDef

```python
# EFSVolumeConfigurationTypeDef definition

class EFSVolumeConfigurationTypeDef(TypedDict):
    fileSystemId: str,
    rootDirectory: NotRequired[str],
    transitEncryption: NotRequired[EFSTransitEncryptionType],  # (1)
    transitEncryptionPort: NotRequired[int],
    authorizationConfig: NotRequired[EFSAuthorizationConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EFSTransitEncryptionType](./literals.md#efstransitencryptiontype) 
2. See [:material-code-braces: EFSAuthorizationConfigTypeDef](./type_defs.md#efsauthorizationconfigtypedef) 
## ExecuteCommandConfigurationTypeDef

```python
# ExecuteCommandConfigurationTypeDef definition

class ExecuteCommandConfigurationTypeDef(TypedDict):
    kmsKeyId: NotRequired[str],
    logging: NotRequired[ExecuteCommandLoggingType],  # (1)
    logConfiguration: NotRequired[ExecuteCommandLogConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: ExecuteCommandLoggingType](./literals.md#executecommandloggingtype) 
2. See [:material-code-braces: ExecuteCommandLogConfigurationTypeDef](./type_defs.md#executecommandlogconfigurationtypedef) 
## ExecuteCommandResponseTypeDef

```python
# ExecuteCommandResponseTypeDef definition

class ExecuteCommandResponseTypeDef(TypedDict):
    clusterArn: str,
    containerArn: str,
    containerName: str,
    interactive: bool,
    session: SessionTypeDef,  # (1)
    taskArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FSxWindowsFileServerVolumeConfigurationTypeDef

```python
# FSxWindowsFileServerVolumeConfigurationTypeDef definition

class FSxWindowsFileServerVolumeConfigurationTypeDef(TypedDict):
    fileSystemId: str,
    rootDirectory: str,
    authorizationConfig: FSxWindowsFileServerAuthorizationConfigTypeDef,  # (1)
```

1. See [:material-code-braces: FSxWindowsFileServerAuthorizationConfigTypeDef](./type_defs.md#fsxwindowsfileserverauthorizationconfigtypedef) 
## GetTaskProtectionResponseTypeDef

```python
# GetTaskProtectionResponseTypeDef definition

class GetTaskProtectionResponseTypeDef(TypedDict):
    protectedTasks: List[ProtectedTaskTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProtectedTaskTypeDef](./type_defs.md#protectedtasktypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTaskProtectionResponseTypeDef

```python
# UpdateTaskProtectionResponseTypeDef definition

class UpdateTaskProtectionResponseTypeDef(TypedDict):
    protectedTasks: List[ProtectedTaskTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProtectedTaskTypeDef](./type_defs.md#protectedtasktypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LinuxParametersTypeDef

```python
# LinuxParametersTypeDef definition

class LinuxParametersTypeDef(TypedDict):
    capabilities: NotRequired[KernelCapabilitiesTypeDef],  # (1)
    devices: NotRequired[List[DeviceTypeDef]],  # (2)
    initProcessEnabled: NotRequired[bool],
    sharedMemorySize: NotRequired[int],
    tmpfs: NotRequired[List[TmpfsTypeDef]],  # (3)
    maxSwap: NotRequired[int],
    swappiness: NotRequired[int],
```

1. See [:material-code-braces: KernelCapabilitiesTypeDef](./type_defs.md#kernelcapabilitiestypedef) 
2. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
3. See [:material-code-braces: TmpfsTypeDef](./type_defs.md#tmpfstypedef) 
## ListAccountSettingsRequestListAccountSettingsPaginateTypeDef

```python
# ListAccountSettingsRequestListAccountSettingsPaginateTypeDef definition

class ListAccountSettingsRequestListAccountSettingsPaginateTypeDef(TypedDict):
    name: NotRequired[SettingNameType],  # (1)
    value: NotRequired[str],
    principalArn: NotRequired[str],
    effectiveSettings: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttributesRequestListAttributesPaginateTypeDef

```python
# ListAttributesRequestListAttributesPaginateTypeDef definition

class ListAttributesRequestListAttributesPaginateTypeDef(TypedDict):
    targetType: TargetTypeType,  # (1)
    cluster: NotRequired[str],
    attributeName: NotRequired[str],
    attributeValue: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersRequestListClustersPaginateTypeDef

```python
# ListClustersRequestListClustersPaginateTypeDef definition

class ListClustersRequestListClustersPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContainerInstancesRequestListContainerInstancesPaginateTypeDef

```python
# ListContainerInstancesRequestListContainerInstancesPaginateTypeDef definition

class ListContainerInstancesRequestListContainerInstancesPaginateTypeDef(TypedDict):
    cluster: NotRequired[str],
    filter: NotRequired[str],
    status: NotRequired[ContainerInstanceStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ContainerInstanceStatusType](./literals.md#containerinstancestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef

```python
# ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef definition

class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(TypedDict):
    namespace: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesRequestListServicesPaginateTypeDef

```python
# ListServicesRequestListServicesPaginateTypeDef definition

class ListServicesRequestListServicesPaginateTypeDef(TypedDict):
    cluster: NotRequired[str],
    launchType: NotRequired[LaunchTypeType],  # (1)
    schedulingStrategy: NotRequired[SchedulingStrategyType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
2. See [:material-code-brackets: SchedulingStrategyType](./literals.md#schedulingstrategytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef

```python
# ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef definition

class ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef(TypedDict):
    familyPrefix: NotRequired[str],
    status: NotRequired[TaskDefinitionFamilyStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskDefinitionFamilyStatusType](./literals.md#taskdefinitionfamilystatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef

```python
# ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef definition

class ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef(TypedDict):
    familyPrefix: NotRequired[str],
    status: NotRequired[TaskDefinitionStatusType],  # (1)
    sort: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: TaskDefinitionStatusType](./literals.md#taskdefinitionstatustype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTasksRequestListTasksPaginateTypeDef

```python
# ListTasksRequestListTasksPaginateTypeDef definition

class ListTasksRequestListTasksPaginateTypeDef(TypedDict):
    cluster: NotRequired[str],
    containerInstance: NotRequired[str],
    family: NotRequired[str],
    startedBy: NotRequired[str],
    serviceName: NotRequired[str],
    desiredStatus: NotRequired[DesiredStatusType],  # (1)
    launchType: NotRequired[LaunchTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: DesiredStatusType](./literals.md#desiredstatustype) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## RegisterContainerInstanceRequestRequestTypeDef

```python
# RegisterContainerInstanceRequestRequestTypeDef definition

class RegisterContainerInstanceRequestRequestTypeDef(TypedDict):
    cluster: NotRequired[str],
    instanceIdentityDocument: NotRequired[str],
    instanceIdentityDocumentSignature: NotRequired[str],
    totalResources: NotRequired[Sequence[ResourceTypeDef]],  # (1)
    versionInfo: NotRequired[VersionInfoTypeDef],  # (2)
    containerInstanceArn: NotRequired[str],
    attributes: NotRequired[Sequence[AttributeTypeDef]],  # (3)
    platformDevices: NotRequired[Sequence[PlatformDeviceTypeDef]],  # (4)
    tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: VersionInfoTypeDef](./type_defs.md#versioninfotypedef) 
3. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
4. See [:material-code-braces: PlatformDeviceTypeDef](./type_defs.md#platformdevicetypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ServiceConnectServiceTypeDef

```python
# ServiceConnectServiceTypeDef definition

class ServiceConnectServiceTypeDef(TypedDict):
    portName: str,
    discoveryName: NotRequired[str],
    clientAliases: NotRequired[Sequence[ServiceConnectClientAliasTypeDef]],  # (1)
    ingressPortOverride: NotRequired[int],
```

1. See [:material-code-braces: ServiceConnectClientAliasTypeDef](./type_defs.md#serviceconnectclientaliastypedef) 
## CapacityProviderTypeDef

```python
# CapacityProviderTypeDef definition

class CapacityProviderTypeDef(TypedDict):
    capacityProviderArn: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[CapacityProviderStatusType],  # (1)
    autoScalingGroupProvider: NotRequired[AutoScalingGroupProviderTypeDef],  # (2)
    updateStatus: NotRequired[CapacityProviderUpdateStatusType],  # (3)
    updateStatusReason: NotRequired[str],
    tags: NotRequired[List[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: CapacityProviderStatusType](./literals.md#capacityproviderstatustype) 
2. See [:material-code-braces: AutoScalingGroupProviderTypeDef](./type_defs.md#autoscalinggroupprovidertypedef) 
3. See [:material-code-brackets: CapacityProviderUpdateStatusType](./literals.md#capacityproviderupdatestatustype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCapacityProviderRequestRequestTypeDef

```python
# CreateCapacityProviderRequestRequestTypeDef definition

class CreateCapacityProviderRequestRequestTypeDef(TypedDict):
    name: str,
    autoScalingGroupProvider: AutoScalingGroupProviderTypeDef,  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: AutoScalingGroupProviderTypeDef](./type_defs.md#autoscalinggroupprovidertypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateCapacityProviderRequestRequestTypeDef

```python
# UpdateCapacityProviderRequestRequestTypeDef definition

class UpdateCapacityProviderRequestRequestTypeDef(TypedDict):
    name: str,
    autoScalingGroupProvider: AutoScalingGroupProviderUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: AutoScalingGroupProviderUpdateTypeDef](./type_defs.md#autoscalinggroupproviderupdatetypedef) 
## CreateTaskSetRequestRequestTypeDef

```python
# CreateTaskSetRequestRequestTypeDef definition

class CreateTaskSetRequestRequestTypeDef(TypedDict):
    service: str,
    cluster: str,
    taskDefinition: str,
    externalId: NotRequired[str],
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (1)
    loadBalancers: NotRequired[Sequence[LoadBalancerTypeDef]],  # (2)
    serviceRegistries: NotRequired[Sequence[ServiceRegistryTypeDef]],  # (3)
    launchType: NotRequired[LaunchTypeType],  # (4)
    capacityProviderStrategy: NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],  # (5)
    platformVersion: NotRequired[str],
    scale: NotRequired[ScaleTypeDef],  # (6)
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (7)
```

1. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
2. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
3. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
4. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
5. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
6. See [:material-code-braces: ScaleTypeDef](./type_defs.md#scaletypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TaskSetTypeDef

```python
# TaskSetTypeDef definition

class TaskSetTypeDef(TypedDict):
    id: NotRequired[str],
    taskSetArn: NotRequired[str],
    serviceArn: NotRequired[str],
    clusterArn: NotRequired[str],
    startedBy: NotRequired[str],
    externalId: NotRequired[str],
    status: NotRequired[str],
    taskDefinition: NotRequired[str],
    computedDesiredCount: NotRequired[int],
    pendingCount: NotRequired[int],
    runningCount: NotRequired[int],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    launchType: NotRequired[LaunchTypeType],  # (1)
    capacityProviderStrategy: NotRequired[List[CapacityProviderStrategyItemTypeDef]],  # (2)
    platformVersion: NotRequired[str],
    platformFamily: NotRequired[str],
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (3)
    loadBalancers: NotRequired[List[LoadBalancerTypeDef]],  # (4)
    serviceRegistries: NotRequired[List[ServiceRegistryTypeDef]],  # (5)
    scale: NotRequired[ScaleTypeDef],  # (6)
    stabilityStatus: NotRequired[StabilityStatusType],  # (7)
    stabilityStatusAt: NotRequired[datetime],
    tags: NotRequired[List[TagTypeDef]],  # (8)
```

1. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
2. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
3. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
4. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
5. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
6. See [:material-code-braces: ScaleTypeDef](./type_defs.md#scaletypedef) 
7. See [:material-code-brackets: StabilityStatusType](./literals.md#stabilitystatustype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TaskOverrideTypeDef

```python
# TaskOverrideTypeDef definition

class TaskOverrideTypeDef(TypedDict):
    containerOverrides: NotRequired[List[ContainerOverrideTypeDef]],  # (1)
    cpu: NotRequired[str],
    inferenceAcceleratorOverrides: NotRequired[List[InferenceAcceleratorOverrideTypeDef]],  # (2)
    executionRoleArn: NotRequired[str],
    memory: NotRequired[str],
    taskRoleArn: NotRequired[str],
    ephemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (3)
```

1. See [:material-code-braces: ContainerOverrideTypeDef](./type_defs.md#containeroverridetypedef) 
2. See [:material-code-braces: InferenceAcceleratorOverrideTypeDef](./type_defs.md#inferenceacceleratoroverridetypedef) 
3. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
## ContainerInstanceTypeDef

```python
# ContainerInstanceTypeDef definition

class ContainerInstanceTypeDef(TypedDict):
    containerInstanceArn: NotRequired[str],
    ec2InstanceId: NotRequired[str],
    capacityProviderName: NotRequired[str],
    version: NotRequired[int],
    versionInfo: NotRequired[VersionInfoTypeDef],  # (1)
    remainingResources: NotRequired[List[ResourceTypeDef]],  # (2)
    registeredResources: NotRequired[List[ResourceTypeDef]],  # (2)
    status: NotRequired[str],
    statusReason: NotRequired[str],
    agentConnected: NotRequired[bool],
    runningTasksCount: NotRequired[int],
    pendingTasksCount: NotRequired[int],
    agentUpdateStatus: NotRequired[AgentUpdateStatusType],  # (4)
    attributes: NotRequired[List[AttributeTypeDef]],  # (5)
    registeredAt: NotRequired[datetime],
    attachments: NotRequired[List[AttachmentTypeDef]],  # (6)
    tags: NotRequired[List[TagTypeDef]],  # (7)
    healthStatus: NotRequired[ContainerInstanceHealthStatusTypeDef],  # (8)
```

1. See [:material-code-braces: VersionInfoTypeDef](./type_defs.md#versioninfotypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
4. See [:material-code-brackets: AgentUpdateStatusType](./literals.md#agentupdatestatustype) 
5. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
6. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: ContainerInstanceHealthStatusTypeDef](./type_defs.md#containerinstancehealthstatustypedef) 
## SubmitTaskStateChangeRequestRequestTypeDef

```python
# SubmitTaskStateChangeRequestRequestTypeDef definition

class SubmitTaskStateChangeRequestRequestTypeDef(TypedDict):
    cluster: NotRequired[str],
    task: NotRequired[str],
    status: NotRequired[str],
    reason: NotRequired[str],
    containers: NotRequired[Sequence[ContainerStateChangeTypeDef]],  # (1)
    attachments: NotRequired[Sequence[AttachmentStateChangeTypeDef]],  # (2)
    managedAgents: NotRequired[Sequence[ManagedAgentStateChangeTypeDef]],  # (3)
    pullStartedAt: NotRequired[Union[datetime, str]],
    pullStoppedAt: NotRequired[Union[datetime, str]],
    executionStoppedAt: NotRequired[Union[datetime, str]],
```

1. See [:material-code-braces: ContainerStateChangeTypeDef](./type_defs.md#containerstatechangetypedef) 
2. See [:material-code-braces: AttachmentStateChangeTypeDef](./type_defs.md#attachmentstatechangetypedef) 
3. See [:material-code-braces: ManagedAgentStateChangeTypeDef](./type_defs.md#managedagentstatechangetypedef) 
## ClusterConfigurationTypeDef

```python
# ClusterConfigurationTypeDef definition

class ClusterConfigurationTypeDef(TypedDict):
    executeCommandConfiguration: NotRequired[ExecuteCommandConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ExecuteCommandConfigurationTypeDef](./type_defs.md#executecommandconfigurationtypedef) 
## VolumeTypeDef

```python
# VolumeTypeDef definition

class VolumeTypeDef(TypedDict):
    name: NotRequired[str],
    host: NotRequired[HostVolumePropertiesTypeDef],  # (1)
    dockerVolumeConfiguration: NotRequired[DockerVolumeConfigurationTypeDef],  # (2)
    efsVolumeConfiguration: NotRequired[EFSVolumeConfigurationTypeDef],  # (3)
    fsxWindowsFileServerVolumeConfiguration: NotRequired[FSxWindowsFileServerVolumeConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: HostVolumePropertiesTypeDef](./type_defs.md#hostvolumepropertiestypedef) 
2. See [:material-code-braces: DockerVolumeConfigurationTypeDef](./type_defs.md#dockervolumeconfigurationtypedef) 
3. See [:material-code-braces: EFSVolumeConfigurationTypeDef](./type_defs.md#efsvolumeconfigurationtypedef) 
4. See [:material-code-braces: FSxWindowsFileServerVolumeConfigurationTypeDef](./type_defs.md#fsxwindowsfileservervolumeconfigurationtypedef) 
## ContainerDefinitionTypeDef

```python
# ContainerDefinitionTypeDef definition

class ContainerDefinitionTypeDef(TypedDict):
    name: NotRequired[str],
    image: NotRequired[str],
    repositoryCredentials: NotRequired[RepositoryCredentialsTypeDef],  # (1)
    cpu: NotRequired[int],
    memory: NotRequired[int],
    memoryReservation: NotRequired[int],
    links: NotRequired[List[str]],
    portMappings: NotRequired[List[PortMappingTypeDef]],  # (2)
    essential: NotRequired[bool],
    entryPoint: NotRequired[List[str]],
    command: NotRequired[List[str]],
    environment: NotRequired[List[KeyValuePairTypeDef]],  # (3)
    environmentFiles: NotRequired[List[EnvironmentFileTypeDef]],  # (4)
    mountPoints: NotRequired[List[MountPointTypeDef]],  # (5)
    volumesFrom: NotRequired[List[VolumeFromTypeDef]],  # (6)
    linuxParameters: NotRequired[LinuxParametersTypeDef],  # (7)
    secrets: NotRequired[List[SecretTypeDef]],  # (8)
    dependsOn: NotRequired[List[ContainerDependencyTypeDef]],  # (9)
    startTimeout: NotRequired[int],
    stopTimeout: NotRequired[int],
    hostname: NotRequired[str],
    user: NotRequired[str],
    workingDirectory: NotRequired[str],
    disableNetworking: NotRequired[bool],
    privileged: NotRequired[bool],
    readonlyRootFilesystem: NotRequired[bool],
    dnsServers: NotRequired[List[str]],
    dnsSearchDomains: NotRequired[List[str]],
    extraHosts: NotRequired[List[HostEntryTypeDef]],  # (10)
    dockerSecurityOptions: NotRequired[List[str]],
    interactive: NotRequired[bool],
    pseudoTerminal: NotRequired[bool],
    dockerLabels: NotRequired[Dict[str, str]],
    ulimits: NotRequired[List[UlimitTypeDef]],  # (11)
    logConfiguration: NotRequired[LogConfigurationTypeDef],  # (12)
    healthCheck: NotRequired[HealthCheckTypeDef],  # (13)
    systemControls: NotRequired[List[SystemControlTypeDef]],  # (14)
    resourceRequirements: NotRequired[List[ResourceRequirementTypeDef]],  # (15)
    firelensConfiguration: NotRequired[FirelensConfigurationTypeDef],  # (16)
    credentialSpecs: NotRequired[List[str]],
```

1. See [:material-code-braces: RepositoryCredentialsTypeDef](./type_defs.md#repositorycredentialstypedef) 
2. See [:material-code-braces: PortMappingTypeDef](./type_defs.md#portmappingtypedef) 
3. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
4. See [:material-code-braces: EnvironmentFileTypeDef](./type_defs.md#environmentfiletypedef) 
5. See [:material-code-braces: MountPointTypeDef](./type_defs.md#mountpointtypedef) 
6. See [:material-code-braces: VolumeFromTypeDef](./type_defs.md#volumefromtypedef) 
7. See [:material-code-braces: LinuxParametersTypeDef](./type_defs.md#linuxparameterstypedef) 
8. See [:material-code-braces: SecretTypeDef](./type_defs.md#secrettypedef) 
9. See [:material-code-braces: ContainerDependencyTypeDef](./type_defs.md#containerdependencytypedef) 
10. See [:material-code-braces: HostEntryTypeDef](./type_defs.md#hostentrytypedef) 
11. See [:material-code-braces: UlimitTypeDef](./type_defs.md#ulimittypedef) 
12. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
13. See [:material-code-braces: HealthCheckTypeDef](./type_defs.md#healthchecktypedef) 
14. See [:material-code-braces: SystemControlTypeDef](./type_defs.md#systemcontroltypedef) 
15. See [:material-code-braces: ResourceRequirementTypeDef](./type_defs.md#resourcerequirementtypedef) 
16. See [:material-code-braces: FirelensConfigurationTypeDef](./type_defs.md#firelensconfigurationtypedef) 
## ServiceConnectConfigurationTypeDef

```python
# ServiceConnectConfigurationTypeDef definition

class ServiceConnectConfigurationTypeDef(TypedDict):
    enabled: bool,
    namespace: NotRequired[str],
    services: NotRequired[Sequence[ServiceConnectServiceTypeDef]],  # (1)
    logConfiguration: NotRequired[LogConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ServiceConnectServiceTypeDef](./type_defs.md#serviceconnectservicetypedef) 
2. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
## CreateCapacityProviderResponseTypeDef

```python
# CreateCapacityProviderResponseTypeDef definition

class CreateCapacityProviderResponseTypeDef(TypedDict):
    capacityProvider: CapacityProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapacityProviderTypeDef](./type_defs.md#capacityprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCapacityProviderResponseTypeDef

```python
# DeleteCapacityProviderResponseTypeDef definition

class DeleteCapacityProviderResponseTypeDef(TypedDict):
    capacityProvider: CapacityProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapacityProviderTypeDef](./type_defs.md#capacityprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCapacityProvidersResponseTypeDef

```python
# DescribeCapacityProvidersResponseTypeDef definition

class DescribeCapacityProvidersResponseTypeDef(TypedDict):
    capacityProviders: List[CapacityProviderTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CapacityProviderTypeDef](./type_defs.md#capacityprovidertypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCapacityProviderResponseTypeDef

```python
# UpdateCapacityProviderResponseTypeDef definition

class UpdateCapacityProviderResponseTypeDef(TypedDict):
    capacityProvider: CapacityProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapacityProviderTypeDef](./type_defs.md#capacityprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTaskSetResponseTypeDef

```python
# CreateTaskSetResponseTypeDef definition

class CreateTaskSetResponseTypeDef(TypedDict):
    taskSet: TaskSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskSetTypeDef](./type_defs.md#tasksettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTaskSetResponseTypeDef

```python
# DeleteTaskSetResponseTypeDef definition

class DeleteTaskSetResponseTypeDef(TypedDict):
    taskSet: TaskSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskSetTypeDef](./type_defs.md#tasksettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTaskSetsResponseTypeDef

```python
# DescribeTaskSetsResponseTypeDef definition

class DescribeTaskSetsResponseTypeDef(TypedDict):
    taskSets: List[TaskSetTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TaskSetTypeDef](./type_defs.md#tasksettypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServicePrimaryTaskSetResponseTypeDef

```python
# UpdateServicePrimaryTaskSetResponseTypeDef definition

class UpdateServicePrimaryTaskSetResponseTypeDef(TypedDict):
    taskSet: TaskSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskSetTypeDef](./type_defs.md#tasksettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTaskSetResponseTypeDef

```python
# UpdateTaskSetResponseTypeDef definition

class UpdateTaskSetResponseTypeDef(TypedDict):
    taskSet: TaskSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskSetTypeDef](./type_defs.md#tasksettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunTaskRequestRequestTypeDef

```python
# RunTaskRequestRequestTypeDef definition

class RunTaskRequestRequestTypeDef(TypedDict):
    taskDefinition: str,
    capacityProviderStrategy: NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],  # (1)
    cluster: NotRequired[str],
    count: NotRequired[int],
    enableECSManagedTags: NotRequired[bool],
    enableExecuteCommand: NotRequired[bool],
    group: NotRequired[str],
    launchType: NotRequired[LaunchTypeType],  # (2)
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (3)
    overrides: NotRequired[TaskOverrideTypeDef],  # (4)
    placementConstraints: NotRequired[Sequence[PlacementConstraintTypeDef]],  # (5)
    placementStrategy: NotRequired[Sequence[PlacementStrategyTypeDef]],  # (6)
    platformVersion: NotRequired[str],
    propagateTags: NotRequired[PropagateTagsType],  # (7)
    referenceId: NotRequired[str],
    startedBy: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (8)
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
3. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
4. See [:material-code-braces: TaskOverrideTypeDef](./type_defs.md#taskoverridetypedef) 
5. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
6. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
7. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartTaskRequestRequestTypeDef

```python
# StartTaskRequestRequestTypeDef definition

class StartTaskRequestRequestTypeDef(TypedDict):
    containerInstances: Sequence[str],
    taskDefinition: str,
    cluster: NotRequired[str],
    enableECSManagedTags: NotRequired[bool],
    enableExecuteCommand: NotRequired[bool],
    group: NotRequired[str],
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (1)
    overrides: NotRequired[TaskOverrideTypeDef],  # (2)
    propagateTags: NotRequired[PropagateTagsType],  # (3)
    referenceId: NotRequired[str],
    startedBy: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
2. See [:material-code-braces: TaskOverrideTypeDef](./type_defs.md#taskoverridetypedef) 
3. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TaskTypeDef

```python
# TaskTypeDef definition

class TaskTypeDef(TypedDict):
    attachments: NotRequired[List[AttachmentTypeDef]],  # (1)
    attributes: NotRequired[List[AttributeTypeDef]],  # (2)
    availabilityZone: NotRequired[str],
    capacityProviderName: NotRequired[str],
    clusterArn: NotRequired[str],
    connectivity: NotRequired[ConnectivityType],  # (3)
    connectivityAt: NotRequired[datetime],
    containerInstanceArn: NotRequired[str],
    containers: NotRequired[List[ContainerTypeDef]],  # (4)
    cpu: NotRequired[str],
    createdAt: NotRequired[datetime],
    desiredStatus: NotRequired[str],
    enableExecuteCommand: NotRequired[bool],
    executionStoppedAt: NotRequired[datetime],
    group: NotRequired[str],
    healthStatus: NotRequired[HealthStatusType],  # (5)
    inferenceAccelerators: NotRequired[List[InferenceAcceleratorTypeDef]],  # (6)
    lastStatus: NotRequired[str],
    launchType: NotRequired[LaunchTypeType],  # (7)
    memory: NotRequired[str],
    overrides: NotRequired[TaskOverrideTypeDef],  # (8)
    platformVersion: NotRequired[str],
    platformFamily: NotRequired[str],
    pullStartedAt: NotRequired[datetime],
    pullStoppedAt: NotRequired[datetime],
    startedAt: NotRequired[datetime],
    startedBy: NotRequired[str],
    stopCode: NotRequired[TaskStopCodeType],  # (9)
    stoppedAt: NotRequired[datetime],
    stoppedReason: NotRequired[str],
    stoppingAt: NotRequired[datetime],
    tags: NotRequired[List[TagTypeDef]],  # (10)
    taskArn: NotRequired[str],
    taskDefinitionArn: NotRequired[str],
    version: NotRequired[int],
    ephemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (11)
```

1. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) 
2. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
3. See [:material-code-brackets: ConnectivityType](./literals.md#connectivitytype) 
4. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) 
5. See [:material-code-brackets: HealthStatusType](./literals.md#healthstatustype) 
6. See [:material-code-braces: InferenceAcceleratorTypeDef](./type_defs.md#inferenceacceleratortypedef) 
7. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
8. See [:material-code-braces: TaskOverrideTypeDef](./type_defs.md#taskoverridetypedef) 
9. See [:material-code-brackets: TaskStopCodeType](./literals.md#taskstopcodetype) 
10. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
11. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
## DeregisterContainerInstanceResponseTypeDef

```python
# DeregisterContainerInstanceResponseTypeDef definition

class DeregisterContainerInstanceResponseTypeDef(TypedDict):
    containerInstance: ContainerInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerInstanceTypeDef](./type_defs.md#containerinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContainerInstancesResponseTypeDef

```python
# DescribeContainerInstancesResponseTypeDef definition

class DescribeContainerInstancesResponseTypeDef(TypedDict):
    containerInstances: List[ContainerInstanceTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ContainerInstanceTypeDef](./type_defs.md#containerinstancetypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterContainerInstanceResponseTypeDef

```python
# RegisterContainerInstanceResponseTypeDef definition

class RegisterContainerInstanceResponseTypeDef(TypedDict):
    containerInstance: ContainerInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerInstanceTypeDef](./type_defs.md#containerinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContainerAgentResponseTypeDef

```python
# UpdateContainerAgentResponseTypeDef definition

class UpdateContainerAgentResponseTypeDef(TypedDict):
    containerInstance: ContainerInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerInstanceTypeDef](./type_defs.md#containerinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContainerInstancesStateResponseTypeDef

```python
# UpdateContainerInstancesStateResponseTypeDef definition

class UpdateContainerInstancesStateResponseTypeDef(TypedDict):
    containerInstances: List[ContainerInstanceTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ContainerInstanceTypeDef](./type_defs.md#containerinstancetypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterTypeDef

```python
# ClusterTypeDef definition

class ClusterTypeDef(TypedDict):
    clusterArn: NotRequired[str],
    clusterName: NotRequired[str],
    configuration: NotRequired[ClusterConfigurationTypeDef],  # (1)
    status: NotRequired[str],
    registeredContainerInstancesCount: NotRequired[int],
    runningTasksCount: NotRequired[int],
    pendingTasksCount: NotRequired[int],
    activeServicesCount: NotRequired[int],
    statistics: NotRequired[List[KeyValuePairTypeDef]],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    settings: NotRequired[List[ClusterSettingTypeDef]],  # (4)
    capacityProviders: NotRequired[List[str]],
    defaultCapacityProviderStrategy: NotRequired[List[CapacityProviderStrategyItemTypeDef]],  # (5)
    attachments: NotRequired[List[AttachmentTypeDef]],  # (6)
    attachmentsStatus: NotRequired[str],
    serviceConnectDefaults: NotRequired[ClusterServiceConnectDefaultsTypeDef],  # (7)
```

1. See [:material-code-braces: ClusterConfigurationTypeDef](./type_defs.md#clusterconfigurationtypedef) 
2. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ClusterSettingTypeDef](./type_defs.md#clustersettingtypedef) 
5. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
6. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) 
7. See [:material-code-braces: ClusterServiceConnectDefaultsTypeDef](./type_defs.md#clusterserviceconnectdefaultstypedef) 
## CreateClusterRequestRequestTypeDef

```python
# CreateClusterRequestRequestTypeDef definition

class CreateClusterRequestRequestTypeDef(TypedDict):
    clusterName: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    settings: NotRequired[Sequence[ClusterSettingTypeDef]],  # (2)
    configuration: NotRequired[ClusterConfigurationTypeDef],  # (3)
    capacityProviders: NotRequired[Sequence[str]],
    defaultCapacityProviderStrategy: NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],  # (4)
    serviceConnectDefaults: NotRequired[ClusterServiceConnectDefaultsRequestTypeDef],  # (5)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ClusterSettingTypeDef](./type_defs.md#clustersettingtypedef) 
3. See [:material-code-braces: ClusterConfigurationTypeDef](./type_defs.md#clusterconfigurationtypedef) 
4. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
5. See [:material-code-braces: ClusterServiceConnectDefaultsRequestTypeDef](./type_defs.md#clusterserviceconnectdefaultsrequesttypedef) 
## UpdateClusterRequestRequestTypeDef

```python
# UpdateClusterRequestRequestTypeDef definition

class UpdateClusterRequestRequestTypeDef(TypedDict):
    cluster: str,
    settings: NotRequired[Sequence[ClusterSettingTypeDef]],  # (1)
    configuration: NotRequired[ClusterConfigurationTypeDef],  # (2)
    serviceConnectDefaults: NotRequired[ClusterServiceConnectDefaultsRequestTypeDef],  # (3)
```

1. See [:material-code-braces: ClusterSettingTypeDef](./type_defs.md#clustersettingtypedef) 
2. See [:material-code-braces: ClusterConfigurationTypeDef](./type_defs.md#clusterconfigurationtypedef) 
3. See [:material-code-braces: ClusterServiceConnectDefaultsRequestTypeDef](./type_defs.md#clusterserviceconnectdefaultsrequesttypedef) 
## RegisterTaskDefinitionRequestRequestTypeDef

```python
# RegisterTaskDefinitionRequestRequestTypeDef definition

class RegisterTaskDefinitionRequestRequestTypeDef(TypedDict):
    family: str,
    containerDefinitions: Sequence[ContainerDefinitionTypeDef],  # (1)
    taskRoleArn: NotRequired[str],
    executionRoleArn: NotRequired[str],
    networkMode: NotRequired[NetworkModeType],  # (2)
    volumes: NotRequired[Sequence[VolumeTypeDef]],  # (3)
    placementConstraints: NotRequired[Sequence[TaskDefinitionPlacementConstraintTypeDef]],  # (4)
    requiresCompatibilities: NotRequired[Sequence[CompatibilityType]],  # (5)
    cpu: NotRequired[str],
    memory: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (6)
    pidMode: NotRequired[PidModeType],  # (7)
    ipcMode: NotRequired[IpcModeType],  # (8)
    proxyConfiguration: NotRequired[ProxyConfigurationTypeDef],  # (9)
    inferenceAccelerators: NotRequired[Sequence[InferenceAcceleratorTypeDef]],  # (10)
    ephemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (11)
    runtimePlatform: NotRequired[RuntimePlatformTypeDef],  # (12)
```

1. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) 
2. See [:material-code-brackets: NetworkModeType](./literals.md#networkmodetype) 
3. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
4. See [:material-code-braces: TaskDefinitionPlacementConstraintTypeDef](./type_defs.md#taskdefinitionplacementconstrainttypedef) 
5. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-brackets: PidModeType](./literals.md#pidmodetype) 
8. See [:material-code-brackets: IpcModeType](./literals.md#ipcmodetype) 
9. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
10. See [:material-code-braces: InferenceAcceleratorTypeDef](./type_defs.md#inferenceacceleratortypedef) 
11. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
12. See [:material-code-braces: RuntimePlatformTypeDef](./type_defs.md#runtimeplatformtypedef) 
## TaskDefinitionTypeDef

```python
# TaskDefinitionTypeDef definition

class TaskDefinitionTypeDef(TypedDict):
    taskDefinitionArn: NotRequired[str],
    containerDefinitions: NotRequired[List[ContainerDefinitionTypeDef]],  # (1)
    family: NotRequired[str],
    taskRoleArn: NotRequired[str],
    executionRoleArn: NotRequired[str],
    networkMode: NotRequired[NetworkModeType],  # (2)
    revision: NotRequired[int],
    volumes: NotRequired[List[VolumeTypeDef]],  # (3)
    status: NotRequired[TaskDefinitionStatusType],  # (4)
    requiresAttributes: NotRequired[List[AttributeTypeDef]],  # (5)
    placementConstraints: NotRequired[List[TaskDefinitionPlacementConstraintTypeDef]],  # (6)
    compatibilities: NotRequired[List[CompatibilityType]],  # (7)
    runtimePlatform: NotRequired[RuntimePlatformTypeDef],  # (8)
    requiresCompatibilities: NotRequired[List[CompatibilityType]],  # (7)
    cpu: NotRequired[str],
    memory: NotRequired[str],
    inferenceAccelerators: NotRequired[List[InferenceAcceleratorTypeDef]],  # (10)
    pidMode: NotRequired[PidModeType],  # (11)
    ipcMode: NotRequired[IpcModeType],  # (12)
    proxyConfiguration: NotRequired[ProxyConfigurationTypeDef],  # (13)
    registeredAt: NotRequired[datetime],
    deregisteredAt: NotRequired[datetime],
    registeredBy: NotRequired[str],
    ephemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (14)
```

1. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) 
2. See [:material-code-brackets: NetworkModeType](./literals.md#networkmodetype) 
3. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
4. See [:material-code-brackets: TaskDefinitionStatusType](./literals.md#taskdefinitionstatustype) 
5. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
6. See [:material-code-braces: TaskDefinitionPlacementConstraintTypeDef](./type_defs.md#taskdefinitionplacementconstrainttypedef) 
7. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
8. See [:material-code-braces: RuntimePlatformTypeDef](./type_defs.md#runtimeplatformtypedef) 
9. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
10. See [:material-code-braces: InferenceAcceleratorTypeDef](./type_defs.md#inferenceacceleratortypedef) 
11. See [:material-code-brackets: PidModeType](./literals.md#pidmodetype) 
12. See [:material-code-brackets: IpcModeType](./literals.md#ipcmodetype) 
13. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
14. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
## CreateServiceRequestRequestTypeDef

```python
# CreateServiceRequestRequestTypeDef definition

class CreateServiceRequestRequestTypeDef(TypedDict):
    serviceName: str,
    cluster: NotRequired[str],
    taskDefinition: NotRequired[str],
    loadBalancers: NotRequired[Sequence[LoadBalancerTypeDef]],  # (1)
    serviceRegistries: NotRequired[Sequence[ServiceRegistryTypeDef]],  # (2)
    desiredCount: NotRequired[int],
    clientToken: NotRequired[str],
    launchType: NotRequired[LaunchTypeType],  # (3)
    capacityProviderStrategy: NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],  # (4)
    platformVersion: NotRequired[str],
    role: NotRequired[str],
    deploymentConfiguration: NotRequired[DeploymentConfigurationTypeDef],  # (5)
    placementConstraints: NotRequired[Sequence[PlacementConstraintTypeDef]],  # (6)
    placementStrategy: NotRequired[Sequence[PlacementStrategyTypeDef]],  # (7)
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (8)
    healthCheckGracePeriodSeconds: NotRequired[int],
    schedulingStrategy: NotRequired[SchedulingStrategyType],  # (9)
    deploymentController: NotRequired[DeploymentControllerTypeDef],  # (10)
    tags: NotRequired[Sequence[TagTypeDef]],  # (11)
    enableECSManagedTags: NotRequired[bool],
    propagateTags: NotRequired[PropagateTagsType],  # (12)
    enableExecuteCommand: NotRequired[bool],
    serviceConnectConfiguration: NotRequired[ServiceConnectConfigurationTypeDef],  # (13)
```

1. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
2. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
3. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
4. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
5. See [:material-code-braces: DeploymentConfigurationTypeDef](./type_defs.md#deploymentconfigurationtypedef) 
6. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
7. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
8. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
9. See [:material-code-brackets: SchedulingStrategyType](./literals.md#schedulingstrategytype) 
10. See [:material-code-braces: DeploymentControllerTypeDef](./type_defs.md#deploymentcontrollertypedef) 
11. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
12. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
13. See [:material-code-braces: ServiceConnectConfigurationTypeDef](./type_defs.md#serviceconnectconfigurationtypedef) 
## DeploymentTypeDef

```python
# DeploymentTypeDef definition

class DeploymentTypeDef(TypedDict):
    id: NotRequired[str],
    status: NotRequired[str],
    taskDefinition: NotRequired[str],
    desiredCount: NotRequired[int],
    pendingCount: NotRequired[int],
    runningCount: NotRequired[int],
    failedTasks: NotRequired[int],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    capacityProviderStrategy: NotRequired[List[CapacityProviderStrategyItemTypeDef]],  # (1)
    launchType: NotRequired[LaunchTypeType],  # (2)
    platformVersion: NotRequired[str],
    platformFamily: NotRequired[str],
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (3)
    rolloutState: NotRequired[DeploymentRolloutStateType],  # (4)
    rolloutStateReason: NotRequired[str],
    serviceConnectConfiguration: NotRequired[ServiceConnectConfigurationTypeDef],  # (5)
    serviceConnectResources: NotRequired[List[ServiceConnectServiceResourceTypeDef]],  # (6)
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
3. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
4. See [:material-code-brackets: DeploymentRolloutStateType](./literals.md#deploymentrolloutstatetype) 
5. See [:material-code-braces: ServiceConnectConfigurationTypeDef](./type_defs.md#serviceconnectconfigurationtypedef) 
6. See [:material-code-braces: ServiceConnectServiceResourceTypeDef](./type_defs.md#serviceconnectserviceresourcetypedef) 
## UpdateServiceRequestRequestTypeDef

```python
# UpdateServiceRequestRequestTypeDef definition

class UpdateServiceRequestRequestTypeDef(TypedDict):
    service: str,
    cluster: NotRequired[str],
    desiredCount: NotRequired[int],
    taskDefinition: NotRequired[str],
    capacityProviderStrategy: NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],  # (1)
    deploymentConfiguration: NotRequired[DeploymentConfigurationTypeDef],  # (2)
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (3)
    placementConstraints: NotRequired[Sequence[PlacementConstraintTypeDef]],  # (4)
    placementStrategy: NotRequired[Sequence[PlacementStrategyTypeDef]],  # (5)
    platformVersion: NotRequired[str],
    forceNewDeployment: NotRequired[bool],
    healthCheckGracePeriodSeconds: NotRequired[int],
    enableExecuteCommand: NotRequired[bool],
    enableECSManagedTags: NotRequired[bool],
    loadBalancers: NotRequired[Sequence[LoadBalancerTypeDef]],  # (6)
    propagateTags: NotRequired[PropagateTagsType],  # (7)
    serviceRegistries: NotRequired[Sequence[ServiceRegistryTypeDef]],  # (8)
    serviceConnectConfiguration: NotRequired[ServiceConnectConfigurationTypeDef],  # (9)
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-braces: DeploymentConfigurationTypeDef](./type_defs.md#deploymentconfigurationtypedef) 
3. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
4. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
5. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
6. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
7. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
8. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
9. See [:material-code-braces: ServiceConnectConfigurationTypeDef](./type_defs.md#serviceconnectconfigurationtypedef) 
## DescribeTasksResponseTypeDef

```python
# DescribeTasksResponseTypeDef definition

class DescribeTasksResponseTypeDef(TypedDict):
    tasks: List[TaskTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunTaskResponseTypeDef

```python
# RunTaskResponseTypeDef definition

class RunTaskResponseTypeDef(TypedDict):
    tasks: List[TaskTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTaskResponseTypeDef

```python
# StartTaskResponseTypeDef definition

class StartTaskResponseTypeDef(TypedDict):
    tasks: List[TaskTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopTaskResponseTypeDef

```python
# StopTaskResponseTypeDef definition

class StopTaskResponseTypeDef(TypedDict):
    task: TaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterResponseTypeDef

```python
# CreateClusterResponseTypeDef definition

class CreateClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterResponseTypeDef

```python
# DeleteClusterResponseTypeDef definition

class DeleteClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeClustersResponseTypeDef

```python
# DescribeClustersResponseTypeDef definition

class DescribeClustersResponseTypeDef(TypedDict):
    clusters: List[ClusterTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutClusterCapacityProvidersResponseTypeDef

```python
# PutClusterCapacityProvidersResponseTypeDef definition

class PutClusterCapacityProvidersResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterResponseTypeDef

```python
# UpdateClusterResponseTypeDef definition

class UpdateClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterSettingsResponseTypeDef

```python
# UpdateClusterSettingsResponseTypeDef definition

class UpdateClusterSettingsResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTaskDefinitionsResponseTypeDef

```python
# DeleteTaskDefinitionsResponseTypeDef definition

class DeleteTaskDefinitionsResponseTypeDef(TypedDict):
    taskDefinitions: List[TaskDefinitionTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TaskDefinitionTypeDef](./type_defs.md#taskdefinitiontypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterTaskDefinitionResponseTypeDef

```python
# DeregisterTaskDefinitionResponseTypeDef definition

class DeregisterTaskDefinitionResponseTypeDef(TypedDict):
    taskDefinition: TaskDefinitionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskDefinitionTypeDef](./type_defs.md#taskdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTaskDefinitionResponseTypeDef

```python
# DescribeTaskDefinitionResponseTypeDef definition

class DescribeTaskDefinitionResponseTypeDef(TypedDict):
    taskDefinition: TaskDefinitionTypeDef,  # (1)
    tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TaskDefinitionTypeDef](./type_defs.md#taskdefinitiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterTaskDefinitionResponseTypeDef

```python
# RegisterTaskDefinitionResponseTypeDef definition

class RegisterTaskDefinitionResponseTypeDef(TypedDict):
    taskDefinition: TaskDefinitionTypeDef,  # (1)
    tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TaskDefinitionTypeDef](./type_defs.md#taskdefinitiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceTypeDef

```python
# ServiceTypeDef definition

class ServiceTypeDef(TypedDict):
    serviceArn: NotRequired[str],
    serviceName: NotRequired[str],
    clusterArn: NotRequired[str],
    loadBalancers: NotRequired[List[LoadBalancerTypeDef]],  # (1)
    serviceRegistries: NotRequired[List[ServiceRegistryTypeDef]],  # (2)
    status: NotRequired[str],
    desiredCount: NotRequired[int],
    runningCount: NotRequired[int],
    pendingCount: NotRequired[int],
    launchType: NotRequired[LaunchTypeType],  # (3)
    capacityProviderStrategy: NotRequired[List[CapacityProviderStrategyItemTypeDef]],  # (4)
    platformVersion: NotRequired[str],
    platformFamily: NotRequired[str],
    taskDefinition: NotRequired[str],
    deploymentConfiguration: NotRequired[DeploymentConfigurationTypeDef],  # (5)
    taskSets: NotRequired[List[TaskSetTypeDef]],  # (6)
    deployments: NotRequired[List[DeploymentTypeDef]],  # (7)
    roleArn: NotRequired[str],
    events: NotRequired[List[ServiceEventTypeDef]],  # (8)
    createdAt: NotRequired[datetime],
    placementConstraints: NotRequired[List[PlacementConstraintTypeDef]],  # (9)
    placementStrategy: NotRequired[List[PlacementStrategyTypeDef]],  # (10)
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (11)
    healthCheckGracePeriodSeconds: NotRequired[int],
    schedulingStrategy: NotRequired[SchedulingStrategyType],  # (12)
    deploymentController: NotRequired[DeploymentControllerTypeDef],  # (13)
    tags: NotRequired[List[TagTypeDef]],  # (14)
    createdBy: NotRequired[str],
    enableECSManagedTags: NotRequired[bool],
    propagateTags: NotRequired[PropagateTagsType],  # (15)
    enableExecuteCommand: NotRequired[bool],
```

1. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
2. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
3. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
4. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
5. See [:material-code-braces: DeploymentConfigurationTypeDef](./type_defs.md#deploymentconfigurationtypedef) 
6. See [:material-code-braces: TaskSetTypeDef](./type_defs.md#tasksettypedef) 
7. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
8. See [:material-code-braces: ServiceEventTypeDef](./type_defs.md#serviceeventtypedef) 
9. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
10. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
11. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
12. See [:material-code-brackets: SchedulingStrategyType](./literals.md#schedulingstrategytype) 
13. See [:material-code-braces: DeploymentControllerTypeDef](./type_defs.md#deploymentcontrollertypedef) 
14. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
15. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
## CreateServiceResponseTypeDef

```python
# CreateServiceResponseTypeDef definition

class CreateServiceResponseTypeDef(TypedDict):
    service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceResponseTypeDef

```python
# DeleteServiceResponseTypeDef definition

class DeleteServiceResponseTypeDef(TypedDict):
    service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeServicesResponseTypeDef

```python
# DescribeServicesResponseTypeDef definition

class DescribeServicesResponseTypeDef(TypedDict):
    services: List[ServiceTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceResponseTypeDef

```python
# UpdateServiceResponseTypeDef definition

class UpdateServiceResponseTypeDef(TypedDict):
    service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
