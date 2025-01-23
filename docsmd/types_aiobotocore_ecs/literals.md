# Literals

> [Index](../README.md) > [ECS](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [ECS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ecs)
    type annotations stubs module [types-aiobotocore-ecs](https://pypi.org/project/types-aiobotocore-ecs/).

## AgentUpdateStatusType

```python
# AgentUpdateStatusType usage example

from types_aiobotocore_ecs.literals import AgentUpdateStatusType

def get_value() -> AgentUpdateStatusType:
    return "FAILED"
```

```python
# AgentUpdateStatusType definition

AgentUpdateStatusType = Literal[
    "FAILED",
    "PENDING",
    "STAGED",
    "STAGING",
    "UPDATED",
    "UPDATING",
]
```
## ApplicationProtocolType

```python
# ApplicationProtocolType usage example

from types_aiobotocore_ecs.literals import ApplicationProtocolType

def get_value() -> ApplicationProtocolType:
    return "grpc"
```

```python
# ApplicationProtocolType definition

ApplicationProtocolType = Literal[
    "grpc",
    "http",
    "http2",
]
```
## AssignPublicIpType

```python
# AssignPublicIpType usage example

from types_aiobotocore_ecs.literals import AssignPublicIpType

def get_value() -> AssignPublicIpType:
    return "DISABLED"
```

```python
# AssignPublicIpType definition

AssignPublicIpType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## AvailabilityZoneRebalancingType

```python
# AvailabilityZoneRebalancingType usage example

from types_aiobotocore_ecs.literals import AvailabilityZoneRebalancingType

def get_value() -> AvailabilityZoneRebalancingType:
    return "DISABLED"
```

```python
# AvailabilityZoneRebalancingType definition

AvailabilityZoneRebalancingType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## CPUArchitectureType

```python
# CPUArchitectureType usage example

from types_aiobotocore_ecs.literals import CPUArchitectureType

def get_value() -> CPUArchitectureType:
    return "ARM64"
```

```python
# CPUArchitectureType definition

CPUArchitectureType = Literal[
    "ARM64",
    "X86_64",
]
```
## CapacityProviderFieldType

```python
# CapacityProviderFieldType usage example

from types_aiobotocore_ecs.literals import CapacityProviderFieldType

def get_value() -> CapacityProviderFieldType:
    return "TAGS"
```

```python
# CapacityProviderFieldType definition

CapacityProviderFieldType = Literal[
    "TAGS",
]
```
## CapacityProviderStatusType

```python
# CapacityProviderStatusType usage example

from types_aiobotocore_ecs.literals import CapacityProviderStatusType

def get_value() -> CapacityProviderStatusType:
    return "ACTIVE"
```

```python
# CapacityProviderStatusType definition

CapacityProviderStatusType = Literal[
    "ACTIVE",
    "INACTIVE",
]
```
## CapacityProviderUpdateStatusType

```python
# CapacityProviderUpdateStatusType usage example

from types_aiobotocore_ecs.literals import CapacityProviderUpdateStatusType

def get_value() -> CapacityProviderUpdateStatusType:
    return "DELETE_COMPLETE"
```

```python
# CapacityProviderUpdateStatusType definition

CapacityProviderUpdateStatusType = Literal[
    "DELETE_COMPLETE",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "UPDATE_COMPLETE",
    "UPDATE_FAILED",
    "UPDATE_IN_PROGRESS",
]
```
## ClusterFieldType

```python
# ClusterFieldType usage example

from types_aiobotocore_ecs.literals import ClusterFieldType

def get_value() -> ClusterFieldType:
    return "ATTACHMENTS"
```

```python
# ClusterFieldType definition

ClusterFieldType = Literal[
    "ATTACHMENTS",
    "CONFIGURATIONS",
    "SETTINGS",
    "STATISTICS",
    "TAGS",
]
```
## ClusterSettingNameType

```python
# ClusterSettingNameType usage example

from types_aiobotocore_ecs.literals import ClusterSettingNameType

def get_value() -> ClusterSettingNameType:
    return "containerInsights"
```

```python
# ClusterSettingNameType definition

ClusterSettingNameType = Literal[
    "containerInsights",
]
```
## CompatibilityType

```python
# CompatibilityType usage example

from types_aiobotocore_ecs.literals import CompatibilityType

def get_value() -> CompatibilityType:
    return "EC2"
```

```python
# CompatibilityType definition

CompatibilityType = Literal[
    "EC2",
    "EXTERNAL",
    "FARGATE",
]
```
## ConnectivityType

```python
# ConnectivityType usage example

from types_aiobotocore_ecs.literals import ConnectivityType

def get_value() -> ConnectivityType:
    return "CONNECTED"
```

```python
# ConnectivityType definition

ConnectivityType = Literal[
    "CONNECTED",
    "DISCONNECTED",
]
```
## ContainerConditionType

```python
# ContainerConditionType usage example

from types_aiobotocore_ecs.literals import ContainerConditionType

def get_value() -> ContainerConditionType:
    return "COMPLETE"
```

```python
# ContainerConditionType definition

ContainerConditionType = Literal[
    "COMPLETE",
    "HEALTHY",
    "START",
    "SUCCESS",
]
```
## ContainerInstanceFieldType

```python
# ContainerInstanceFieldType usage example

from types_aiobotocore_ecs.literals import ContainerInstanceFieldType

def get_value() -> ContainerInstanceFieldType:
    return "CONTAINER_INSTANCE_HEALTH"
```

```python
# ContainerInstanceFieldType definition

ContainerInstanceFieldType = Literal[
    "CONTAINER_INSTANCE_HEALTH",
    "TAGS",
]
```
## ContainerInstanceStatusType

```python
# ContainerInstanceStatusType usage example

from types_aiobotocore_ecs.literals import ContainerInstanceStatusType

def get_value() -> ContainerInstanceStatusType:
    return "ACTIVE"
```

```python
# ContainerInstanceStatusType definition

ContainerInstanceStatusType = Literal[
    "ACTIVE",
    "DEREGISTERING",
    "DRAINING",
    "REGISTERING",
    "REGISTRATION_FAILED",
]
```
## DeploymentControllerTypeType

```python
# DeploymentControllerTypeType usage example

from types_aiobotocore_ecs.literals import DeploymentControllerTypeType

def get_value() -> DeploymentControllerTypeType:
    return "CODE_DEPLOY"
```

```python
# DeploymentControllerTypeType definition

DeploymentControllerTypeType = Literal[
    "CODE_DEPLOY",
    "ECS",
    "EXTERNAL",
]
```
## DeploymentRolloutStateType

```python
# DeploymentRolloutStateType usage example

from types_aiobotocore_ecs.literals import DeploymentRolloutStateType

def get_value() -> DeploymentRolloutStateType:
    return "COMPLETED"
```

```python
# DeploymentRolloutStateType definition

DeploymentRolloutStateType = Literal[
    "COMPLETED",
    "FAILED",
    "IN_PROGRESS",
]
```
## DesiredStatusType

```python
# DesiredStatusType usage example

from types_aiobotocore_ecs.literals import DesiredStatusType

def get_value() -> DesiredStatusType:
    return "PENDING"
```

```python
# DesiredStatusType definition

DesiredStatusType = Literal[
    "PENDING",
    "RUNNING",
    "STOPPED",
]
```
## DeviceCgroupPermissionType

```python
# DeviceCgroupPermissionType usage example

from types_aiobotocore_ecs.literals import DeviceCgroupPermissionType

def get_value() -> DeviceCgroupPermissionType:
    return "mknod"
```

```python
# DeviceCgroupPermissionType definition

DeviceCgroupPermissionType = Literal[
    "mknod",
    "read",
    "write",
]
```
## EBSResourceTypeType

```python
# EBSResourceTypeType usage example

from types_aiobotocore_ecs.literals import EBSResourceTypeType

def get_value() -> EBSResourceTypeType:
    return "volume"
```

```python
# EBSResourceTypeType definition

EBSResourceTypeType = Literal[
    "volume",
]
```
## EFSAuthorizationConfigIAMType

```python
# EFSAuthorizationConfigIAMType usage example

from types_aiobotocore_ecs.literals import EFSAuthorizationConfigIAMType

def get_value() -> EFSAuthorizationConfigIAMType:
    return "DISABLED"
```

```python
# EFSAuthorizationConfigIAMType definition

EFSAuthorizationConfigIAMType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## EFSTransitEncryptionType

```python
# EFSTransitEncryptionType usage example

from types_aiobotocore_ecs.literals import EFSTransitEncryptionType

def get_value() -> EFSTransitEncryptionType:
    return "DISABLED"
```

```python
# EFSTransitEncryptionType definition

EFSTransitEncryptionType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## EnvironmentFileTypeType

```python
# EnvironmentFileTypeType usage example

from types_aiobotocore_ecs.literals import EnvironmentFileTypeType

def get_value() -> EnvironmentFileTypeType:
    return "s3"
```

```python
# EnvironmentFileTypeType definition

EnvironmentFileTypeType = Literal[
    "s3",
]
```
## ExecuteCommandLoggingType

```python
# ExecuteCommandLoggingType usage example

from types_aiobotocore_ecs.literals import ExecuteCommandLoggingType

def get_value() -> ExecuteCommandLoggingType:
    return "DEFAULT"
```

```python
# ExecuteCommandLoggingType definition

ExecuteCommandLoggingType = Literal[
    "DEFAULT",
    "NONE",
    "OVERRIDE",
]
```
## FirelensConfigurationTypeType

```python
# FirelensConfigurationTypeType usage example

from types_aiobotocore_ecs.literals import FirelensConfigurationTypeType

def get_value() -> FirelensConfigurationTypeType:
    return "fluentbit"
```

```python
# FirelensConfigurationTypeType definition

FirelensConfigurationTypeType = Literal[
    "fluentbit",
    "fluentd",
]
```
## HealthStatusType

```python
# HealthStatusType usage example

from types_aiobotocore_ecs.literals import HealthStatusType

def get_value() -> HealthStatusType:
    return "HEALTHY"
```

```python
# HealthStatusType definition

HealthStatusType = Literal[
    "HEALTHY",
    "UNHEALTHY",
    "UNKNOWN",
]
```
## InstanceHealthCheckStateType

```python
# InstanceHealthCheckStateType usage example

from types_aiobotocore_ecs.literals import InstanceHealthCheckStateType

def get_value() -> InstanceHealthCheckStateType:
    return "IMPAIRED"
```

```python
# InstanceHealthCheckStateType definition

InstanceHealthCheckStateType = Literal[
    "IMPAIRED",
    "INITIALIZING",
    "INSUFFICIENT_DATA",
    "OK",
]
```
## InstanceHealthCheckTypeType

```python
# InstanceHealthCheckTypeType usage example

from types_aiobotocore_ecs.literals import InstanceHealthCheckTypeType

def get_value() -> InstanceHealthCheckTypeType:
    return "CONTAINER_RUNTIME"
```

```python
# InstanceHealthCheckTypeType definition

InstanceHealthCheckTypeType = Literal[
    "CONTAINER_RUNTIME",
]
```
## IpcModeType

```python
# IpcModeType usage example

from types_aiobotocore_ecs.literals import IpcModeType

def get_value() -> IpcModeType:
    return "host"
```

```python
# IpcModeType definition

IpcModeType = Literal[
    "host",
    "none",
    "task",
]
```
## LaunchTypeType

```python
# LaunchTypeType usage example

from types_aiobotocore_ecs.literals import LaunchTypeType

def get_value() -> LaunchTypeType:
    return "EC2"
```

```python
# LaunchTypeType definition

LaunchTypeType = Literal[
    "EC2",
    "EXTERNAL",
    "FARGATE",
]
```
## ListAccountSettingsPaginatorName

```python
# ListAccountSettingsPaginatorName usage example

from types_aiobotocore_ecs.literals import ListAccountSettingsPaginatorName

def get_value() -> ListAccountSettingsPaginatorName:
    return "list_account_settings"
```

```python
# ListAccountSettingsPaginatorName definition

ListAccountSettingsPaginatorName = Literal[
    "list_account_settings",
]
```
## ListAttributesPaginatorName

```python
# ListAttributesPaginatorName usage example

from types_aiobotocore_ecs.literals import ListAttributesPaginatorName

def get_value() -> ListAttributesPaginatorName:
    return "list_attributes"
```

```python
# ListAttributesPaginatorName definition

ListAttributesPaginatorName = Literal[
    "list_attributes",
]
```
## ListClustersPaginatorName

```python
# ListClustersPaginatorName usage example

from types_aiobotocore_ecs.literals import ListClustersPaginatorName

def get_value() -> ListClustersPaginatorName:
    return "list_clusters"
```

```python
# ListClustersPaginatorName definition

ListClustersPaginatorName = Literal[
    "list_clusters",
]
```
## ListContainerInstancesPaginatorName

```python
# ListContainerInstancesPaginatorName usage example

from types_aiobotocore_ecs.literals import ListContainerInstancesPaginatorName

def get_value() -> ListContainerInstancesPaginatorName:
    return "list_container_instances"
```

```python
# ListContainerInstancesPaginatorName definition

ListContainerInstancesPaginatorName = Literal[
    "list_container_instances",
]
```
## ListServicesByNamespacePaginatorName

```python
# ListServicesByNamespacePaginatorName usage example

from types_aiobotocore_ecs.literals import ListServicesByNamespacePaginatorName

def get_value() -> ListServicesByNamespacePaginatorName:
    return "list_services_by_namespace"
```

```python
# ListServicesByNamespacePaginatorName definition

ListServicesByNamespacePaginatorName = Literal[
    "list_services_by_namespace",
]
```
## ListServicesPaginatorName

```python
# ListServicesPaginatorName usage example

from types_aiobotocore_ecs.literals import ListServicesPaginatorName

def get_value() -> ListServicesPaginatorName:
    return "list_services"
```

```python
# ListServicesPaginatorName definition

ListServicesPaginatorName = Literal[
    "list_services",
]
```
## ListTaskDefinitionFamiliesPaginatorName

```python
# ListTaskDefinitionFamiliesPaginatorName usage example

from types_aiobotocore_ecs.literals import ListTaskDefinitionFamiliesPaginatorName

def get_value() -> ListTaskDefinitionFamiliesPaginatorName:
    return "list_task_definition_families"
```

```python
# ListTaskDefinitionFamiliesPaginatorName definition

ListTaskDefinitionFamiliesPaginatorName = Literal[
    "list_task_definition_families",
]
```
## ListTaskDefinitionsPaginatorName

```python
# ListTaskDefinitionsPaginatorName usage example

from types_aiobotocore_ecs.literals import ListTaskDefinitionsPaginatorName

def get_value() -> ListTaskDefinitionsPaginatorName:
    return "list_task_definitions"
```

```python
# ListTaskDefinitionsPaginatorName definition

ListTaskDefinitionsPaginatorName = Literal[
    "list_task_definitions",
]
```
## ListTasksPaginatorName

```python
# ListTasksPaginatorName usage example

from types_aiobotocore_ecs.literals import ListTasksPaginatorName

def get_value() -> ListTasksPaginatorName:
    return "list_tasks"
```

```python
# ListTasksPaginatorName definition

ListTasksPaginatorName = Literal[
    "list_tasks",
]
```
## LogDriverType

```python
# LogDriverType usage example

from types_aiobotocore_ecs.literals import LogDriverType

def get_value() -> LogDriverType:
    return "awsfirelens"
```

```python
# LogDriverType definition

LogDriverType = Literal[
    "awsfirelens",
    "awslogs",
    "fluentd",
    "gelf",
    "journald",
    "json-file",
    "splunk",
    "syslog",
]
```
## ManagedAgentNameType

```python
# ManagedAgentNameType usage example

from types_aiobotocore_ecs.literals import ManagedAgentNameType

def get_value() -> ManagedAgentNameType:
    return "ExecuteCommandAgent"
```

```python
# ManagedAgentNameType definition

ManagedAgentNameType = Literal[
    "ExecuteCommandAgent",
]
```
## ManagedDrainingType

```python
# ManagedDrainingType usage example

from types_aiobotocore_ecs.literals import ManagedDrainingType

def get_value() -> ManagedDrainingType:
    return "DISABLED"
```

```python
# ManagedDrainingType definition

ManagedDrainingType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## ManagedScalingStatusType

```python
# ManagedScalingStatusType usage example

from types_aiobotocore_ecs.literals import ManagedScalingStatusType

def get_value() -> ManagedScalingStatusType:
    return "DISABLED"
```

```python
# ManagedScalingStatusType definition

ManagedScalingStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## ManagedTerminationProtectionType

```python
# ManagedTerminationProtectionType usage example

from types_aiobotocore_ecs.literals import ManagedTerminationProtectionType

def get_value() -> ManagedTerminationProtectionType:
    return "DISABLED"
```

```python
# ManagedTerminationProtectionType definition

ManagedTerminationProtectionType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## NetworkModeType

```python
# NetworkModeType usage example

from types_aiobotocore_ecs.literals import NetworkModeType

def get_value() -> NetworkModeType:
    return "awsvpc"
```

```python
# NetworkModeType definition

NetworkModeType = Literal[
    "awsvpc",
    "bridge",
    "host",
    "none",
]
```
## OSFamilyType

```python
# OSFamilyType usage example

from types_aiobotocore_ecs.literals import OSFamilyType

def get_value() -> OSFamilyType:
    return "LINUX"
```

```python
# OSFamilyType definition

OSFamilyType = Literal[
    "LINUX",
    "WINDOWS_SERVER_2004_CORE",
    "WINDOWS_SERVER_2016_FULL",
    "WINDOWS_SERVER_2019_CORE",
    "WINDOWS_SERVER_2019_FULL",
    "WINDOWS_SERVER_2022_CORE",
    "WINDOWS_SERVER_2022_FULL",
    "WINDOWS_SERVER_20H2_CORE",
]
```
## PidModeType

```python
# PidModeType usage example

from types_aiobotocore_ecs.literals import PidModeType

def get_value() -> PidModeType:
    return "host"
```

```python
# PidModeType definition

PidModeType = Literal[
    "host",
    "task",
]
```
## PlacementConstraintTypeType

```python
# PlacementConstraintTypeType usage example

from types_aiobotocore_ecs.literals import PlacementConstraintTypeType

def get_value() -> PlacementConstraintTypeType:
    return "distinctInstance"
```

```python
# PlacementConstraintTypeType definition

PlacementConstraintTypeType = Literal[
    "distinctInstance",
    "memberOf",
]
```
## PlacementStrategyTypeType

```python
# PlacementStrategyTypeType usage example

from types_aiobotocore_ecs.literals import PlacementStrategyTypeType

def get_value() -> PlacementStrategyTypeType:
    return "binpack"
```

```python
# PlacementStrategyTypeType definition

PlacementStrategyTypeType = Literal[
    "binpack",
    "random",
    "spread",
]
```
## PlatformDeviceTypeType

```python
# PlatformDeviceTypeType usage example

from types_aiobotocore_ecs.literals import PlatformDeviceTypeType

def get_value() -> PlatformDeviceTypeType:
    return "GPU"
```

```python
# PlatformDeviceTypeType definition

PlatformDeviceTypeType = Literal[
    "GPU",
]
```
## PropagateTagsType

```python
# PropagateTagsType usage example

from types_aiobotocore_ecs.literals import PropagateTagsType

def get_value() -> PropagateTagsType:
    return "NONE"
```

```python
# PropagateTagsType definition

PropagateTagsType = Literal[
    "NONE",
    "SERVICE",
    "TASK_DEFINITION",
]
```
## ProxyConfigurationTypeType

```python
# ProxyConfigurationTypeType usage example

from types_aiobotocore_ecs.literals import ProxyConfigurationTypeType

def get_value() -> ProxyConfigurationTypeType:
    return "APPMESH"
```

```python
# ProxyConfigurationTypeType definition

ProxyConfigurationTypeType = Literal[
    "APPMESH",
]
```
## ResourceTypeType

```python
# ResourceTypeType usage example

from types_aiobotocore_ecs.literals import ResourceTypeType

def get_value() -> ResourceTypeType:
    return "GPU"
```

```python
# ResourceTypeType definition

ResourceTypeType = Literal[
    "GPU",
    "InferenceAccelerator",
]
```
## ScaleUnitType

```python
# ScaleUnitType usage example

from types_aiobotocore_ecs.literals import ScaleUnitType

def get_value() -> ScaleUnitType:
    return "PERCENT"
```

```python
# ScaleUnitType definition

ScaleUnitType = Literal[
    "PERCENT",
]
```
## SchedulingStrategyType

```python
# SchedulingStrategyType usage example

from types_aiobotocore_ecs.literals import SchedulingStrategyType

def get_value() -> SchedulingStrategyType:
    return "DAEMON"
```

```python
# SchedulingStrategyType definition

SchedulingStrategyType = Literal[
    "DAEMON",
    "REPLICA",
]
```
## ScopeType

```python
# ScopeType usage example

from types_aiobotocore_ecs.literals import ScopeType

def get_value() -> ScopeType:
    return "shared"
```

```python
# ScopeType definition

ScopeType = Literal[
    "shared",
    "task",
]
```
## ServiceDeploymentRollbackMonitorsStatusType

```python
# ServiceDeploymentRollbackMonitorsStatusType usage example

from types_aiobotocore_ecs.literals import ServiceDeploymentRollbackMonitorsStatusType

def get_value() -> ServiceDeploymentRollbackMonitorsStatusType:
    return "DISABLED"
```

```python
# ServiceDeploymentRollbackMonitorsStatusType definition

ServiceDeploymentRollbackMonitorsStatusType = Literal[
    "DISABLED",
    "MONITORING",
    "MONITORING_COMPLETE",
    "TRIGGERED",
]
```
## ServiceDeploymentStatusType

```python
# ServiceDeploymentStatusType usage example

from types_aiobotocore_ecs.literals import ServiceDeploymentStatusType

def get_value() -> ServiceDeploymentStatusType:
    return "IN_PROGRESS"
```

```python
# ServiceDeploymentStatusType definition

ServiceDeploymentStatusType = Literal[
    "IN_PROGRESS",
    "PENDING",
    "ROLLBACK_FAILED",
    "ROLLBACK_IN_PROGRESS",
    "ROLLBACK_SUCCESSFUL",
    "STOP_REQUESTED",
    "STOPPED",
    "SUCCESSFUL",
]
```
## ServiceFieldType

```python
# ServiceFieldType usage example

from types_aiobotocore_ecs.literals import ServiceFieldType

def get_value() -> ServiceFieldType:
    return "TAGS"
```

```python
# ServiceFieldType definition

ServiceFieldType = Literal[
    "TAGS",
]
```
## ServicesInactiveWaiterName

```python
# ServicesInactiveWaiterName usage example

from types_aiobotocore_ecs.literals import ServicesInactiveWaiterName

def get_value() -> ServicesInactiveWaiterName:
    return "services_inactive"
```

```python
# ServicesInactiveWaiterName definition

ServicesInactiveWaiterName = Literal[
    "services_inactive",
]
```
## ServicesStableWaiterName

```python
# ServicesStableWaiterName usage example

from types_aiobotocore_ecs.literals import ServicesStableWaiterName

def get_value() -> ServicesStableWaiterName:
    return "services_stable"
```

```python
# ServicesStableWaiterName definition

ServicesStableWaiterName = Literal[
    "services_stable",
]
```
## SettingNameType

```python
# SettingNameType usage example

from types_aiobotocore_ecs.literals import SettingNameType

def get_value() -> SettingNameType:
    return "awsvpcTrunking"
```

```python
# SettingNameType definition

SettingNameType = Literal[
    "awsvpcTrunking",
    "containerInsights",
    "containerInstanceLongArnFormat",
    "fargateFIPSMode",
    "fargateTaskRetirementWaitPeriod",
    "guardDutyActivate",
    "serviceLongArnFormat",
    "tagResourceAuthorization",
    "taskLongArnFormat",
]
```
## SettingTypeType

```python
# SettingTypeType usage example

from types_aiobotocore_ecs.literals import SettingTypeType

def get_value() -> SettingTypeType:
    return "aws_managed"
```

```python
# SettingTypeType definition

SettingTypeType = Literal[
    "aws_managed",
    "user",
]
```
## SortOrderType

```python
# SortOrderType usage example

from types_aiobotocore_ecs.literals import SortOrderType

def get_value() -> SortOrderType:
    return "ASC"
```

```python
# SortOrderType definition

SortOrderType = Literal[
    "ASC",
    "DESC",
]
```
## StabilityStatusType

```python
# StabilityStatusType usage example

from types_aiobotocore_ecs.literals import StabilityStatusType

def get_value() -> StabilityStatusType:
    return "STABILIZING"
```

```python
# StabilityStatusType definition

StabilityStatusType = Literal[
    "STABILIZING",
    "STEADY_STATE",
]
```
## TargetTypeType

```python
# TargetTypeType usage example

from types_aiobotocore_ecs.literals import TargetTypeType

def get_value() -> TargetTypeType:
    return "container-instance"
```

```python
# TargetTypeType definition

TargetTypeType = Literal[
    "container-instance",
]
```
## TaskDefinitionFamilyStatusType

```python
# TaskDefinitionFamilyStatusType usage example

from types_aiobotocore_ecs.literals import TaskDefinitionFamilyStatusType

def get_value() -> TaskDefinitionFamilyStatusType:
    return "ACTIVE"
```

```python
# TaskDefinitionFamilyStatusType definition

TaskDefinitionFamilyStatusType = Literal[
    "ACTIVE",
    "ALL",
    "INACTIVE",
]
```
## TaskDefinitionFieldType

```python
# TaskDefinitionFieldType usage example

from types_aiobotocore_ecs.literals import TaskDefinitionFieldType

def get_value() -> TaskDefinitionFieldType:
    return "TAGS"
```

```python
# TaskDefinitionFieldType definition

TaskDefinitionFieldType = Literal[
    "TAGS",
]
```
## TaskDefinitionPlacementConstraintTypeType

```python
# TaskDefinitionPlacementConstraintTypeType usage example

from types_aiobotocore_ecs.literals import TaskDefinitionPlacementConstraintTypeType

def get_value() -> TaskDefinitionPlacementConstraintTypeType:
    return "memberOf"
```

```python
# TaskDefinitionPlacementConstraintTypeType definition

TaskDefinitionPlacementConstraintTypeType = Literal[
    "memberOf",
]
```
## TaskDefinitionStatusType

```python
# TaskDefinitionStatusType usage example

from types_aiobotocore_ecs.literals import TaskDefinitionStatusType

def get_value() -> TaskDefinitionStatusType:
    return "ACTIVE"
```

```python
# TaskDefinitionStatusType definition

TaskDefinitionStatusType = Literal[
    "ACTIVE",
    "DELETE_IN_PROGRESS",
    "INACTIVE",
]
```
## TaskFieldType

```python
# TaskFieldType usage example

from types_aiobotocore_ecs.literals import TaskFieldType

def get_value() -> TaskFieldType:
    return "TAGS"
```

```python
# TaskFieldType definition

TaskFieldType = Literal[
    "TAGS",
]
```
## TaskFilesystemTypeType

```python
# TaskFilesystemTypeType usage example

from types_aiobotocore_ecs.literals import TaskFilesystemTypeType

def get_value() -> TaskFilesystemTypeType:
    return "ext3"
```

```python
# TaskFilesystemTypeType definition

TaskFilesystemTypeType = Literal[
    "ext3",
    "ext4",
    "ntfs",
    "xfs",
]
```
## TaskSetFieldType

```python
# TaskSetFieldType usage example

from types_aiobotocore_ecs.literals import TaskSetFieldType

def get_value() -> TaskSetFieldType:
    return "TAGS"
```

```python
# TaskSetFieldType definition

TaskSetFieldType = Literal[
    "TAGS",
]
```
## TaskStopCodeType

```python
# TaskStopCodeType usage example

from types_aiobotocore_ecs.literals import TaskStopCodeType

def get_value() -> TaskStopCodeType:
    return "EssentialContainerExited"
```

```python
# TaskStopCodeType definition

TaskStopCodeType = Literal[
    "EssentialContainerExited",
    "ServiceSchedulerInitiated",
    "SpotInterruption",
    "TaskFailedToStart",
    "TerminationNotice",
    "UserInitiated",
]
```
## TasksRunningWaiterName

```python
# TasksRunningWaiterName usage example

from types_aiobotocore_ecs.literals import TasksRunningWaiterName

def get_value() -> TasksRunningWaiterName:
    return "tasks_running"
```

```python
# TasksRunningWaiterName definition

TasksRunningWaiterName = Literal[
    "tasks_running",
]
```
## TasksStoppedWaiterName

```python
# TasksStoppedWaiterName usage example

from types_aiobotocore_ecs.literals import TasksStoppedWaiterName

def get_value() -> TasksStoppedWaiterName:
    return "tasks_stopped"
```

```python
# TasksStoppedWaiterName definition

TasksStoppedWaiterName = Literal[
    "tasks_stopped",
]
```
## TransportProtocolType

```python
# TransportProtocolType usage example

from types_aiobotocore_ecs.literals import TransportProtocolType

def get_value() -> TransportProtocolType:
    return "tcp"
```

```python
# TransportProtocolType definition

TransportProtocolType = Literal[
    "tcp",
    "udp",
]
```
## UlimitNameType

```python
# UlimitNameType usage example

from types_aiobotocore_ecs.literals import UlimitNameType

def get_value() -> UlimitNameType:
    return "core"
```

```python
# UlimitNameType definition

UlimitNameType = Literal[
    "core",
    "cpu",
    "data",
    "fsize",
    "locks",
    "memlock",
    "msgqueue",
    "nice",
    "nofile",
    "nproc",
    "rss",
    "rtprio",
    "rttime",
    "sigpending",
    "stack",
]
```
## VersionConsistencyType

```python
# VersionConsistencyType usage example

from types_aiobotocore_ecs.literals import VersionConsistencyType

def get_value() -> VersionConsistencyType:
    return "disabled"
```

```python
# VersionConsistencyType definition

VersionConsistencyType = Literal[
    "disabled",
    "enabled",
]
```
## ECSServiceName

```python
# ECSServiceName usage example

from types_aiobotocore_ecs.literals import ECSServiceName

def get_value() -> ECSServiceName:
    return "ecs"
```

```python
# ECSServiceName definition

ECSServiceName = Literal[
    "ecs",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_ecs.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition

ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "application-signals",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "apptest",
    "arc-zonal-shift",
    "artifact",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "b2bi",
    "backup",
    "backup-gateway",
    "backupsearch",
    "batch",
    "bcm-data-exports",
    "bcm-pricing-calculator",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
    "bedrock-data-automation",
    "bedrock-data-automation-runtime",
    "bedrock-runtime",
    "billing",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chatbot",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cleanroomsml",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudfront-keyvaluestore",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codeconnections",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcampaignsv2",
    "connectcases",
    "connectparticipant",
    "controlcatalog",
    "controltower",
    "cost-optimization-hub",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "datazone",
    "dax",
    "deadline",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "ds-data",
    "dsql",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "eks-auth",
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "freetier",
    "fsx",
    "gamelift",
    "geo-maps",
    "geo-places",
    "geo-routes",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector-scan",
    "inspector2",
    "internetmonitor",
    "invoicing",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "launch-wizard",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "m2",
    "machinelearning",
    "macie2",
    "mailmanager",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-agreement",
    "marketplace-catalog",
    "marketplace-deployment",
    "marketplace-entitlement",
    "marketplace-reporting",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "neptune-graph",
    "neptunedata",
    "network-firewall",
    "networkflowmonitor",
    "networkmanager",
    "networkmonitor",
    "notifications",
    "notificationscontacts",
    "oam",
    "observabilityadmin",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "partnercentral-selling",
    "payment-cryptography",
    "payment-cryptography-data",
    "pca-connector-ad",
    "pca-connector-scep",
    "pcs",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "privatenetworks",
    "proton",
    "qapps",
    "qbusiness",
    "qconnect",
    "qldb",
    "qldb-session",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "repostspace",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53profiles",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "s3tables",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "security-ir",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "socialmessaging",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-quicksetup",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "supplychain",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "taxsettings",
    "textract",
    "timestream-influxdb",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "trustedadvisor",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-thin-client",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_ecs.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition

ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example

from types_aiobotocore_ecs.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_account_settings"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_account_settings",
    "list_attributes",
    "list_clusters",
    "list_container_instances",
    "list_services",
    "list_services_by_namespace",
    "list_task_definition_families",
    "list_task_definitions",
    "list_tasks",
]
```
## WaiterName

```python
# WaiterName usage example

from types_aiobotocore_ecs.literals import WaiterName

def get_value() -> WaiterName:
    return "services_inactive"
```

```python
# WaiterName definition

WaiterName = Literal[
    "services_inactive",
    "services_stable",
    "tasks_running",
    "tasks_stopped",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_ecs.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition

RegionName = Literal[
    "af-south-1",
    "ap-east-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-northeast-3",
    "ap-south-1",
    "ap-south-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "ap-southeast-3",
    "ap-southeast-4",
    "ap-southeast-5",
    "ap-southeast-7",
    "ca-central-1",
    "ca-west-1",
    "eu-central-1",
    "eu-central-2",
    "eu-north-1",
    "eu-south-1",
    "eu-south-2",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "il-central-1",
    "me-central-1",
    "me-south-1",
    "mx-central-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
