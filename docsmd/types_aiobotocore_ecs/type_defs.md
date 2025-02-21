# Type definitions

> [Index](../README.md) > [ECS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ECS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ecs)
    type annotations stubs module [types-aiobotocore-ecs](https://pypi.org/project/types-aiobotocore-ecs/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ContainerRestartPolicyUnionTypeDef

```python
# ContainerRestartPolicyUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import ContainerRestartPolicyUnionTypeDef


def get_value() -> ContainerRestartPolicyUnionTypeDef:
    return ...


# ContainerRestartPolicyUnionTypeDef definition

ContainerRestartPolicyUnionTypeDef = Union[
    ContainerRestartPolicyTypeDef,  # (1)
    ContainerRestartPolicyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ContainerRestartPolicyTypeDef](./type_defs.md#containerrestartpolicytypedef) 
2. See [:material-code-braces: ContainerRestartPolicyOutputTypeDef](./type_defs.md#containerrestartpolicyoutputtypedef) 

## DeviceUnionTypeDef

```python
# DeviceUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import DeviceUnionTypeDef


def get_value() -> DeviceUnionTypeDef:
    return ...


# DeviceUnionTypeDef definition

DeviceUnionTypeDef = Union[
    DeviceTypeDef,  # (1)
    DeviceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: DeviceOutputTypeDef](./type_defs.md#deviceoutputtypedef) 

## DockerVolumeConfigurationUnionTypeDef

```python
# DockerVolumeConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import DockerVolumeConfigurationUnionTypeDef


def get_value() -> DockerVolumeConfigurationUnionTypeDef:
    return ...


# DockerVolumeConfigurationUnionTypeDef definition

DockerVolumeConfigurationUnionTypeDef = Union[
    DockerVolumeConfigurationTypeDef,  # (1)
    DockerVolumeConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DockerVolumeConfigurationTypeDef](./type_defs.md#dockervolumeconfigurationtypedef) 
2. See [:material-code-braces: DockerVolumeConfigurationOutputTypeDef](./type_defs.md#dockervolumeconfigurationoutputtypedef) 

## FirelensConfigurationUnionTypeDef

```python
# FirelensConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import FirelensConfigurationUnionTypeDef


def get_value() -> FirelensConfigurationUnionTypeDef:
    return ...


# FirelensConfigurationUnionTypeDef definition

FirelensConfigurationUnionTypeDef = Union[
    FirelensConfigurationTypeDef,  # (1)
    FirelensConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FirelensConfigurationTypeDef](./type_defs.md#firelensconfigurationtypedef) 
2. See [:material-code-braces: FirelensConfigurationOutputTypeDef](./type_defs.md#firelensconfigurationoutputtypedef) 

## HealthCheckUnionTypeDef

```python
# HealthCheckUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import HealthCheckUnionTypeDef


def get_value() -> HealthCheckUnionTypeDef:
    return ...


# HealthCheckUnionTypeDef definition

HealthCheckUnionTypeDef = Union[
    HealthCheckTypeDef,  # (1)
    HealthCheckOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HealthCheckTypeDef](./type_defs.md#healthchecktypedef) 
2. See [:material-code-braces: HealthCheckOutputTypeDef](./type_defs.md#healthcheckoutputtypedef) 

## KernelCapabilitiesUnionTypeDef

```python
# KernelCapabilitiesUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import KernelCapabilitiesUnionTypeDef


def get_value() -> KernelCapabilitiesUnionTypeDef:
    return ...


# KernelCapabilitiesUnionTypeDef definition

KernelCapabilitiesUnionTypeDef = Union[
    KernelCapabilitiesTypeDef,  # (1)
    KernelCapabilitiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KernelCapabilitiesTypeDef](./type_defs.md#kernelcapabilitiestypedef) 
2. See [:material-code-braces: KernelCapabilitiesOutputTypeDef](./type_defs.md#kernelcapabilitiesoutputtypedef) 

## ResourceUnionTypeDef

```python
# ResourceUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import ResourceUnionTypeDef


def get_value() -> ResourceUnionTypeDef:
    return ...


# ResourceUnionTypeDef definition

ResourceUnionTypeDef = Union[
    ResourceTypeDef,  # (1)
    ResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 

## TmpfsUnionTypeDef

```python
# TmpfsUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import TmpfsUnionTypeDef


def get_value() -> TmpfsUnionTypeDef:
    return ...


# TmpfsUnionTypeDef definition

TmpfsUnionTypeDef = Union[
    TmpfsTypeDef,  # (1)
    TmpfsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TmpfsTypeDef](./type_defs.md#tmpfstypedef) 
2. See [:material-code-braces: TmpfsOutputTypeDef](./type_defs.md#tmpfsoutputtypedef) 

## ProxyConfigurationUnionTypeDef

```python
# ProxyConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import ProxyConfigurationUnionTypeDef


def get_value() -> ProxyConfigurationUnionTypeDef:
    return ...


# ProxyConfigurationUnionTypeDef definition

ProxyConfigurationUnionTypeDef = Union[
    ProxyConfigurationTypeDef,  # (1)
    ProxyConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
2. See [:material-code-braces: ProxyConfigurationOutputTypeDef](./type_defs.md#proxyconfigurationoutputtypedef) 

## NetworkConfigurationUnionTypeDef

```python
# NetworkConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import NetworkConfigurationUnionTypeDef


def get_value() -> NetworkConfigurationUnionTypeDef:
    return ...


# NetworkConfigurationUnionTypeDef definition

NetworkConfigurationUnionTypeDef = Union[
    NetworkConfigurationTypeDef,  # (1)
    NetworkConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
2. See [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 

## EBSTagSpecificationUnionTypeDef

```python
# EBSTagSpecificationUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import EBSTagSpecificationUnionTypeDef


def get_value() -> EBSTagSpecificationUnionTypeDef:
    return ...


# EBSTagSpecificationUnionTypeDef definition

EBSTagSpecificationUnionTypeDef = Union[
    EBSTagSpecificationTypeDef,  # (1)
    EBSTagSpecificationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EBSTagSpecificationTypeDef](./type_defs.md#ebstagspecificationtypedef) 
2. See [:material-code-braces: EBSTagSpecificationOutputTypeDef](./type_defs.md#ebstagspecificationoutputtypedef) 

## LogConfigurationUnionTypeDef

```python
# LogConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import LogConfigurationUnionTypeDef


def get_value() -> LogConfigurationUnionTypeDef:
    return ...


# LogConfigurationUnionTypeDef definition

LogConfigurationUnionTypeDef = Union[
    LogConfigurationTypeDef,  # (1)
    LogConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
2. See [:material-code-braces: LogConfigurationOutputTypeDef](./type_defs.md#logconfigurationoutputtypedef) 

## DeploymentConfigurationUnionTypeDef

```python
# DeploymentConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import DeploymentConfigurationUnionTypeDef


def get_value() -> DeploymentConfigurationUnionTypeDef:
    return ...


# DeploymentConfigurationUnionTypeDef definition

DeploymentConfigurationUnionTypeDef = Union[
    DeploymentConfigurationTypeDef,  # (1)
    DeploymentConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeploymentConfigurationTypeDef](./type_defs.md#deploymentconfigurationtypedef) 
2. See [:material-code-braces: DeploymentConfigurationOutputTypeDef](./type_defs.md#deploymentconfigurationoutputtypedef) 

## TaskOverrideUnionTypeDef

```python
# TaskOverrideUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import TaskOverrideUnionTypeDef


def get_value() -> TaskOverrideUnionTypeDef:
    return ...


# TaskOverrideUnionTypeDef definition

TaskOverrideUnionTypeDef = Union[
    TaskOverrideTypeDef,  # (1)
    TaskOverrideOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TaskOverrideTypeDef](./type_defs.md#taskoverridetypedef) 
2. See [:material-code-braces: TaskOverrideOutputTypeDef](./type_defs.md#taskoverrideoutputtypedef) 

## VolumeUnionTypeDef

```python
# VolumeUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import VolumeUnionTypeDef


def get_value() -> VolumeUnionTypeDef:
    return ...


# VolumeUnionTypeDef definition

VolumeUnionTypeDef = Union[
    VolumeTypeDef,  # (1)
    VolumeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
2. See [:material-code-braces: VolumeOutputTypeDef](./type_defs.md#volumeoutputtypedef) 

## LinuxParametersUnionTypeDef

```python
# LinuxParametersUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import LinuxParametersUnionTypeDef


def get_value() -> LinuxParametersUnionTypeDef:
    return ...


# LinuxParametersUnionTypeDef definition

LinuxParametersUnionTypeDef = Union[
    LinuxParametersTypeDef,  # (1)
    LinuxParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LinuxParametersTypeDef](./type_defs.md#linuxparameterstypedef) 
2. See [:material-code-braces: LinuxParametersOutputTypeDef](./type_defs.md#linuxparametersoutputtypedef) 

## ServiceManagedEBSVolumeConfigurationUnionTypeDef

```python
# ServiceManagedEBSVolumeConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import ServiceManagedEBSVolumeConfigurationUnionTypeDef


def get_value() -> ServiceManagedEBSVolumeConfigurationUnionTypeDef:
    return ...


# ServiceManagedEBSVolumeConfigurationUnionTypeDef definition

ServiceManagedEBSVolumeConfigurationUnionTypeDef = Union[
    ServiceManagedEBSVolumeConfigurationTypeDef,  # (1)
    ServiceManagedEBSVolumeConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServiceManagedEBSVolumeConfigurationTypeDef](./type_defs.md#servicemanagedebsvolumeconfigurationtypedef) 
2. See [:material-code-braces: ServiceManagedEBSVolumeConfigurationOutputTypeDef](./type_defs.md#servicemanagedebsvolumeconfigurationoutputtypedef) 

## ServiceConnectConfigurationUnionTypeDef

```python
# ServiceConnectConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import ServiceConnectConfigurationUnionTypeDef


def get_value() -> ServiceConnectConfigurationUnionTypeDef:
    return ...


# ServiceConnectConfigurationUnionTypeDef definition

ServiceConnectConfigurationUnionTypeDef = Union[
    ServiceConnectConfigurationTypeDef,  # (1)
    ServiceConnectConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServiceConnectConfigurationTypeDef](./type_defs.md#serviceconnectconfigurationtypedef) 
2. See [:material-code-braces: ServiceConnectConfigurationOutputTypeDef](./type_defs.md#serviceconnectconfigurationoutputtypedef) 

## ContainerDefinitionUnionTypeDef

```python
# ContainerDefinitionUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import ContainerDefinitionUnionTypeDef


def get_value() -> ContainerDefinitionUnionTypeDef:
    return ...


# ContainerDefinitionUnionTypeDef definition

ContainerDefinitionUnionTypeDef = Union[
    ContainerDefinitionTypeDef,  # (1)
    ContainerDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) 
2. See [:material-code-braces: ContainerDefinitionOutputTypeDef](./type_defs.md#containerdefinitionoutputtypedef) 

## ServiceVolumeConfigurationUnionTypeDef

```python
# ServiceVolumeConfigurationUnionTypeDef Union usage example

from types_aiobotocore_ecs.type_defs import ServiceVolumeConfigurationUnionTypeDef


def get_value() -> ServiceVolumeConfigurationUnionTypeDef:
    return ...


# ServiceVolumeConfigurationUnionTypeDef definition

ServiceVolumeConfigurationUnionTypeDef = Union[
    ServiceVolumeConfigurationTypeDef,  # (1)
    ServiceVolumeConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServiceVolumeConfigurationTypeDef](./type_defs.md#servicevolumeconfigurationtypedef) 
2. See [:material-code-braces: ServiceVolumeConfigurationOutputTypeDef](./type_defs.md#servicevolumeconfigurationoutputtypedef) 



## AttachmentStateChangeTypeDef

```python
# AttachmentStateChangeTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import AttachmentStateChangeTypeDef


def get_value() -> AttachmentStateChangeTypeDef:
    return {
        "attachmentArn": ...,
    }


# AttachmentStateChangeTypeDef definition

class AttachmentStateChangeTypeDef(TypedDict):
    attachmentArn: str,
    status: str,
```

## KeyValuePairTypeDef

```python
# KeyValuePairTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import KeyValuePairTypeDef


def get_value() -> KeyValuePairTypeDef:
    return {
        "name": ...,
    }


# KeyValuePairTypeDef definition

class KeyValuePairTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
```

## AttributeTypeDef

```python
# AttributeTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import AttributeTypeDef


def get_value() -> AttributeTypeDef:
    return {
        "name": ...,
    }


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
# ManagedScalingTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ManagedScalingTypeDef


def get_value() -> ManagedScalingTypeDef:
    return {
        "status": ...,
    }


# ManagedScalingTypeDef definition

class ManagedScalingTypeDef(TypedDict):
    status: NotRequired[ManagedScalingStatusType],  # (1)
    targetCapacity: NotRequired[int],
    minimumScalingStepSize: NotRequired[int],
    maximumScalingStepSize: NotRequired[int],
    instanceWarmupPeriod: NotRequired[int],
```

1. See [:material-code-brackets: ManagedScalingStatusType](./literals.md#managedscalingstatustype) 
## AwsVpcConfigurationOutputTypeDef

```python
# AwsVpcConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import AwsVpcConfigurationOutputTypeDef


def get_value() -> AwsVpcConfigurationOutputTypeDef:
    return {
        "subnets": ...,
    }


# AwsVpcConfigurationOutputTypeDef definition

class AwsVpcConfigurationOutputTypeDef(TypedDict):
    subnets: List[str],
    securityGroups: NotRequired[List[str]],
    assignPublicIp: NotRequired[AssignPublicIpType],  # (1)
```

1. See [:material-code-brackets: AssignPublicIpType](./literals.md#assignpubliciptype) 
## AwsVpcConfigurationTypeDef

```python
# AwsVpcConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import AwsVpcConfigurationTypeDef


def get_value() -> AwsVpcConfigurationTypeDef:
    return {
        "subnets": ...,
    }


# AwsVpcConfigurationTypeDef definition

class AwsVpcConfigurationTypeDef(TypedDict):
    subnets: Sequence[str],
    securityGroups: NotRequired[Sequence[str]],
    assignPublicIp: NotRequired[AssignPublicIpType],  # (1)
```

1. See [:material-code-brackets: AssignPublicIpType](./literals.md#assignpubliciptype) 
## CapacityProviderStrategyItemTypeDef

```python
# CapacityProviderStrategyItemTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import CapacityProviderStrategyItemTypeDef


def get_value() -> CapacityProviderStrategyItemTypeDef:
    return {
        "capacityProvider": ...,
    }


# CapacityProviderStrategyItemTypeDef definition

class CapacityProviderStrategyItemTypeDef(TypedDict):
    capacityProvider: str,
    weight: NotRequired[int],
    base: NotRequired[int],
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## ManagedStorageConfigurationTypeDef

```python
# ManagedStorageConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ManagedStorageConfigurationTypeDef


def get_value() -> ManagedStorageConfigurationTypeDef:
    return {
        "kmsKeyId": ...,
    }


# ManagedStorageConfigurationTypeDef definition

class ManagedStorageConfigurationTypeDef(TypedDict):
    kmsKeyId: NotRequired[str],
    fargateEphemeralStorageKmsKeyId: NotRequired[str],
```

## ClusterServiceConnectDefaultsRequestTypeDef

```python
# ClusterServiceConnectDefaultsRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ClusterServiceConnectDefaultsRequestTypeDef


def get_value() -> ClusterServiceConnectDefaultsRequestTypeDef:
    return {
        "namespace": ...,
    }


# ClusterServiceConnectDefaultsRequestTypeDef definition

class ClusterServiceConnectDefaultsRequestTypeDef(TypedDict):
    namespace: str,
```

## ClusterServiceConnectDefaultsTypeDef

```python
# ClusterServiceConnectDefaultsTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ClusterServiceConnectDefaultsTypeDef


def get_value() -> ClusterServiceConnectDefaultsTypeDef:
    return {
        "namespace": ...,
    }


# ClusterServiceConnectDefaultsTypeDef definition

class ClusterServiceConnectDefaultsTypeDef(TypedDict):
    namespace: NotRequired[str],
```

## ClusterSettingTypeDef

```python
# ClusterSettingTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ClusterSettingTypeDef


def get_value() -> ClusterSettingTypeDef:
    return {
        "name": ...,
    }


# ClusterSettingTypeDef definition

class ClusterSettingTypeDef(TypedDict):
    name: NotRequired[ClusterSettingNameType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: ClusterSettingNameType](./literals.md#clustersettingnametype) 
## ContainerDependencyTypeDef

```python
# ContainerDependencyTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerDependencyTypeDef


def get_value() -> ContainerDependencyTypeDef:
    return {
        "containerName": ...,
    }


# ContainerDependencyTypeDef definition

class ContainerDependencyTypeDef(TypedDict):
    containerName: str,
    condition: ContainerConditionType,  # (1)
```

1. See [:material-code-brackets: ContainerConditionType](./literals.md#containerconditiontype) 
## ContainerRestartPolicyOutputTypeDef

```python
# ContainerRestartPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerRestartPolicyOutputTypeDef


def get_value() -> ContainerRestartPolicyOutputTypeDef:
    return {
        "enabled": ...,
    }


# ContainerRestartPolicyOutputTypeDef definition

class ContainerRestartPolicyOutputTypeDef(TypedDict):
    enabled: bool,
    ignoredExitCodes: NotRequired[List[int]],
    restartAttemptPeriod: NotRequired[int],
```

## EnvironmentFileTypeDef

```python
# EnvironmentFileTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import EnvironmentFileTypeDef


def get_value() -> EnvironmentFileTypeDef:
    return {
        "value": ...,
    }


# EnvironmentFileTypeDef definition

class EnvironmentFileTypeDef(TypedDict):
    value: str,
    type: EnvironmentFileTypeType,  # (1)
```

1. See [:material-code-brackets: EnvironmentFileTypeType](./literals.md#environmentfiletypetype) 
## FirelensConfigurationOutputTypeDef

```python
# FirelensConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import FirelensConfigurationOutputTypeDef


def get_value() -> FirelensConfigurationOutputTypeDef:
    return {
        "type": ...,
    }


# FirelensConfigurationOutputTypeDef definition

class FirelensConfigurationOutputTypeDef(TypedDict):
    type: FirelensConfigurationTypeType,  # (1)
    options: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: FirelensConfigurationTypeType](./literals.md#firelensconfigurationtypetype) 
## HealthCheckOutputTypeDef

```python
# HealthCheckOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import HealthCheckOutputTypeDef


def get_value() -> HealthCheckOutputTypeDef:
    return {
        "command": ...,
    }


# HealthCheckOutputTypeDef definition

class HealthCheckOutputTypeDef(TypedDict):
    command: List[str],
    interval: NotRequired[int],
    timeout: NotRequired[int],
    retries: NotRequired[int],
    startPeriod: NotRequired[int],
```

## HostEntryTypeDef

```python
# HostEntryTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import HostEntryTypeDef


def get_value() -> HostEntryTypeDef:
    return {
        "hostname": ...,
    }


# HostEntryTypeDef definition

class HostEntryTypeDef(TypedDict):
    hostname: str,
    ipAddress: str,
```

## MountPointTypeDef

```python
# MountPointTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import MountPointTypeDef


def get_value() -> MountPointTypeDef:
    return {
        "sourceVolume": ...,
    }


# MountPointTypeDef definition

class MountPointTypeDef(TypedDict):
    sourceVolume: NotRequired[str],
    containerPath: NotRequired[str],
    readOnly: NotRequired[bool],
```

## PortMappingTypeDef

```python
# PortMappingTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PortMappingTypeDef


def get_value() -> PortMappingTypeDef:
    return {
        "containerPort": ...,
    }


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
# RepositoryCredentialsTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import RepositoryCredentialsTypeDef


def get_value() -> RepositoryCredentialsTypeDef:
    return {
        "credentialsParameter": ...,
    }


# RepositoryCredentialsTypeDef definition

class RepositoryCredentialsTypeDef(TypedDict):
    credentialsParameter: str,
```

## ResourceRequirementTypeDef

```python
# ResourceRequirementTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ResourceRequirementTypeDef


def get_value() -> ResourceRequirementTypeDef:
    return {
        "value": ...,
    }


# ResourceRequirementTypeDef definition

class ResourceRequirementTypeDef(TypedDict):
    value: str,
    type: ResourceTypeType,  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## SecretTypeDef

```python
# SecretTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import SecretTypeDef


def get_value() -> SecretTypeDef:
    return {
        "name": ...,
    }


# SecretTypeDef definition

class SecretTypeDef(TypedDict):
    name: str,
    valueFrom: str,
```

## SystemControlTypeDef

```python
# SystemControlTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import SystemControlTypeDef


def get_value() -> SystemControlTypeDef:
    return {
        "namespace": ...,
    }


# SystemControlTypeDef definition

class SystemControlTypeDef(TypedDict):
    namespace: NotRequired[str],
    value: NotRequired[str],
```

## UlimitTypeDef

```python
# UlimitTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UlimitTypeDef


def get_value() -> UlimitTypeDef:
    return {
        "name": ...,
    }


# UlimitTypeDef definition

class UlimitTypeDef(TypedDict):
    name: UlimitNameType,  # (1)
    softLimit: int,
    hardLimit: int,
```

1. See [:material-code-brackets: UlimitNameType](./literals.md#ulimitnametype) 
## VolumeFromTypeDef

```python
# VolumeFromTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import VolumeFromTypeDef


def get_value() -> VolumeFromTypeDef:
    return {
        "sourceContainer": ...,
    }


# VolumeFromTypeDef definition

class VolumeFromTypeDef(TypedDict):
    sourceContainer: NotRequired[str],
    readOnly: NotRequired[bool],
```

## ContainerImageTypeDef

```python
# ContainerImageTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerImageTypeDef


def get_value() -> ContainerImageTypeDef:
    return {
        "containerName": ...,
    }


# ContainerImageTypeDef definition

class ContainerImageTypeDef(TypedDict):
    containerName: NotRequired[str],
    imageDigest: NotRequired[str],
    image: NotRequired[str],
```

## InstanceHealthCheckResultTypeDef

```python
# InstanceHealthCheckResultTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import InstanceHealthCheckResultTypeDef


def get_value() -> InstanceHealthCheckResultTypeDef:
    return {
        "type": ...,
    }


# InstanceHealthCheckResultTypeDef definition

class InstanceHealthCheckResultTypeDef(TypedDict):
    type: NotRequired[InstanceHealthCheckTypeType],  # (1)
    status: NotRequired[InstanceHealthCheckStateType],  # (2)
    lastUpdated: NotRequired[datetime],
    lastStatusChange: NotRequired[datetime],
```

1. See [:material-code-brackets: InstanceHealthCheckTypeType](./literals.md#instancehealthchecktypetype) 
2. See [:material-code-brackets: InstanceHealthCheckStateType](./literals.md#instancehealthcheckstatetype) 
## ResourceOutputTypeDef

```python
# ResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ResourceOutputTypeDef


def get_value() -> ResourceOutputTypeDef:
    return {
        "name": ...,
    }


# ResourceOutputTypeDef definition

class ResourceOutputTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    doubleValue: NotRequired[float],
    longValue: NotRequired[int],
    integerValue: NotRequired[int],
    stringSetValue: NotRequired[List[str]],
```

## VersionInfoTypeDef

```python
# VersionInfoTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import VersionInfoTypeDef


def get_value() -> VersionInfoTypeDef:
    return {
        "agentVersion": ...,
    }


# VersionInfoTypeDef definition

class VersionInfoTypeDef(TypedDict):
    agentVersion: NotRequired[str],
    agentHash: NotRequired[str],
    dockerVersion: NotRequired[str],
```

## ContainerRestartPolicyTypeDef

```python
# ContainerRestartPolicyTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerRestartPolicyTypeDef


def get_value() -> ContainerRestartPolicyTypeDef:
    return {
        "enabled": ...,
    }


# ContainerRestartPolicyTypeDef definition

class ContainerRestartPolicyTypeDef(TypedDict):
    enabled: bool,
    ignoredExitCodes: NotRequired[Sequence[int]],
    restartAttemptPeriod: NotRequired[int],
```

## NetworkBindingTypeDef

```python
# NetworkBindingTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import NetworkBindingTypeDef


def get_value() -> NetworkBindingTypeDef:
    return {
        "bindIP": ...,
    }


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
# ManagedAgentTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ManagedAgentTypeDef


def get_value() -> ManagedAgentTypeDef:
    return {
        "lastStartedAt": ...,
    }


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
# NetworkInterfaceTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import NetworkInterfaceTypeDef


def get_value() -> NetworkInterfaceTypeDef:
    return {
        "attachmentId": ...,
    }


# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    attachmentId: NotRequired[str],
    privateIpv4Address: NotRequired[str],
    ipv6Address: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ResponseMetadataTypeDef


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

## DeploymentControllerTypeDef

```python
# DeploymentControllerTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeploymentControllerTypeDef


def get_value() -> DeploymentControllerTypeDef:
    return {
        "type": ...,
    }


# DeploymentControllerTypeDef definition

class DeploymentControllerTypeDef(TypedDict):
    type: DeploymentControllerTypeType,  # (1)
```

1. See [:material-code-brackets: DeploymentControllerTypeType](./literals.md#deploymentcontrollertypetype) 
## LoadBalancerTypeDef

```python
# LoadBalancerTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import LoadBalancerTypeDef


def get_value() -> LoadBalancerTypeDef:
    return {
        "targetGroupArn": ...,
    }


# LoadBalancerTypeDef definition

class LoadBalancerTypeDef(TypedDict):
    targetGroupArn: NotRequired[str],
    loadBalancerName: NotRequired[str],
    containerName: NotRequired[str],
    containerPort: NotRequired[int],
```

## PlacementConstraintTypeDef

```python
# PlacementConstraintTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PlacementConstraintTypeDef


def get_value() -> PlacementConstraintTypeDef:
    return {
        "type": ...,
    }


# PlacementConstraintTypeDef definition

class PlacementConstraintTypeDef(TypedDict):
    type: NotRequired[PlacementConstraintTypeType],  # (1)
    expression: NotRequired[str],
```

1. See [:material-code-brackets: PlacementConstraintTypeType](./literals.md#placementconstrainttypetype) 
## PlacementStrategyTypeDef

```python
# PlacementStrategyTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PlacementStrategyTypeDef


def get_value() -> PlacementStrategyTypeDef:
    return {
        "type": ...,
    }


# PlacementStrategyTypeDef definition

class PlacementStrategyTypeDef(TypedDict):
    type: NotRequired[PlacementStrategyTypeType],  # (1)
    field: NotRequired[str],
```

1. See [:material-code-brackets: PlacementStrategyTypeType](./literals.md#placementstrategytypetype) 
## ServiceRegistryTypeDef

```python
# ServiceRegistryTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceRegistryTypeDef


def get_value() -> ServiceRegistryTypeDef:
    return {
        "registryArn": ...,
    }


# ServiceRegistryTypeDef definition

class ServiceRegistryTypeDef(TypedDict):
    registryArn: NotRequired[str],
    port: NotRequired[int],
    containerName: NotRequired[str],
    containerPort: NotRequired[int],
```

## VpcLatticeConfigurationTypeDef

```python
# VpcLatticeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import VpcLatticeConfigurationTypeDef


def get_value() -> VpcLatticeConfigurationTypeDef:
    return {
        "roleArn": ...,
    }


# VpcLatticeConfigurationTypeDef definition

class VpcLatticeConfigurationTypeDef(TypedDict):
    roleArn: str,
    targetGroupArn: str,
    portName: str,
```

## ScaleTypeDef

```python
# ScaleTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ScaleTypeDef


def get_value() -> ScaleTypeDef:
    return {
        "value": ...,
    }


# ScaleTypeDef definition

class ScaleTypeDef(TypedDict):
    value: NotRequired[float],
    unit: NotRequired[ScaleUnitType],  # (1)
```

1. See [:material-code-brackets: ScaleUnitType](./literals.md#scaleunittype) 
## DeleteAccountSettingRequestTypeDef

```python
# DeleteAccountSettingRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteAccountSettingRequestTypeDef


def get_value() -> DeleteAccountSettingRequestTypeDef:
    return {
        "name": ...,
    }


# DeleteAccountSettingRequestTypeDef definition

class DeleteAccountSettingRequestTypeDef(TypedDict):
    name: SettingNameType,  # (1)
    principalArn: NotRequired[str],
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
## SettingTypeDef

```python
# SettingTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import SettingTypeDef


def get_value() -> SettingTypeDef:
    return {
        "name": ...,
    }


# SettingTypeDef definition

class SettingTypeDef(TypedDict):
    name: NotRequired[SettingNameType],  # (1)
    value: NotRequired[str],
    principalArn: NotRequired[str],
    type: NotRequired[SettingTypeType],  # (2)
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
2. See [:material-code-brackets: SettingTypeType](./literals.md#settingtypetype) 
## DeleteCapacityProviderRequestTypeDef

```python
# DeleteCapacityProviderRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteCapacityProviderRequestTypeDef


def get_value() -> DeleteCapacityProviderRequestTypeDef:
    return {
        "capacityProvider": ...,
    }


# DeleteCapacityProviderRequestTypeDef definition

class DeleteCapacityProviderRequestTypeDef(TypedDict):
    capacityProvider: str,
```

## DeleteClusterRequestTypeDef

```python
# DeleteClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteClusterRequestTypeDef


def get_value() -> DeleteClusterRequestTypeDef:
    return {
        "cluster": ...,
    }


# DeleteClusterRequestTypeDef definition

class DeleteClusterRequestTypeDef(TypedDict):
    cluster: str,
```

## DeleteServiceRequestTypeDef

```python
# DeleteServiceRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteServiceRequestTypeDef


def get_value() -> DeleteServiceRequestTypeDef:
    return {
        "service": ...,
    }


# DeleteServiceRequestTypeDef definition

class DeleteServiceRequestTypeDef(TypedDict):
    service: str,
    cluster: NotRequired[str],
    force: NotRequired[bool],
```

## DeleteTaskDefinitionsRequestTypeDef

```python
# DeleteTaskDefinitionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteTaskDefinitionsRequestTypeDef


def get_value() -> DeleteTaskDefinitionsRequestTypeDef:
    return {
        "taskDefinitions": ...,
    }


# DeleteTaskDefinitionsRequestTypeDef definition

class DeleteTaskDefinitionsRequestTypeDef(TypedDict):
    taskDefinitions: Sequence[str],
```

## FailureTypeDef

```python
# FailureTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import FailureTypeDef


def get_value() -> FailureTypeDef:
    return {
        "arn": ...,
    }


# FailureTypeDef definition

class FailureTypeDef(TypedDict):
    arn: NotRequired[str],
    reason: NotRequired[str],
    detail: NotRequired[str],
```

## DeleteTaskSetRequestTypeDef

```python
# DeleteTaskSetRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteTaskSetRequestTypeDef


def get_value() -> DeleteTaskSetRequestTypeDef:
    return {
        "cluster": ...,
    }


# DeleteTaskSetRequestTypeDef definition

class DeleteTaskSetRequestTypeDef(TypedDict):
    cluster: str,
    service: str,
    taskSet: str,
    force: NotRequired[bool],
```

## DeploymentAlarmsOutputTypeDef

```python
# DeploymentAlarmsOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeploymentAlarmsOutputTypeDef


def get_value() -> DeploymentAlarmsOutputTypeDef:
    return {
        "alarmNames": ...,
    }


# DeploymentAlarmsOutputTypeDef definition

class DeploymentAlarmsOutputTypeDef(TypedDict):
    alarmNames: List[str],
    rollback: bool,
    enable: bool,
```

## DeploymentAlarmsTypeDef

```python
# DeploymentAlarmsTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeploymentAlarmsTypeDef


def get_value() -> DeploymentAlarmsTypeDef:
    return {
        "alarmNames": ...,
    }


# DeploymentAlarmsTypeDef definition

class DeploymentAlarmsTypeDef(TypedDict):
    alarmNames: Sequence[str],
    rollback: bool,
    enable: bool,
```

## DeploymentCircuitBreakerTypeDef

```python
# DeploymentCircuitBreakerTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeploymentCircuitBreakerTypeDef


def get_value() -> DeploymentCircuitBreakerTypeDef:
    return {
        "enable": ...,
    }


# DeploymentCircuitBreakerTypeDef definition

class DeploymentCircuitBreakerTypeDef(TypedDict):
    enable: bool,
    rollback: bool,
```

## DeploymentEphemeralStorageTypeDef

```python
# DeploymentEphemeralStorageTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeploymentEphemeralStorageTypeDef


def get_value() -> DeploymentEphemeralStorageTypeDef:
    return {
        "kmsKeyId": ...,
    }


# DeploymentEphemeralStorageTypeDef definition

class DeploymentEphemeralStorageTypeDef(TypedDict):
    kmsKeyId: NotRequired[str],
```

## ServiceConnectServiceResourceTypeDef

```python
# ServiceConnectServiceResourceTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceConnectServiceResourceTypeDef


def get_value() -> ServiceConnectServiceResourceTypeDef:
    return {
        "discoveryName": ...,
    }


# ServiceConnectServiceResourceTypeDef definition

class ServiceConnectServiceResourceTypeDef(TypedDict):
    discoveryName: NotRequired[str],
    discoveryArn: NotRequired[str],
```

## DeregisterContainerInstanceRequestTypeDef

```python
# DeregisterContainerInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeregisterContainerInstanceRequestTypeDef


def get_value() -> DeregisterContainerInstanceRequestTypeDef:
    return {
        "containerInstance": ...,
    }


# DeregisterContainerInstanceRequestTypeDef definition

class DeregisterContainerInstanceRequestTypeDef(TypedDict):
    containerInstance: str,
    cluster: NotRequired[str],
    force: NotRequired[bool],
```

## DeregisterTaskDefinitionRequestTypeDef

```python
# DeregisterTaskDefinitionRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeregisterTaskDefinitionRequestTypeDef


def get_value() -> DeregisterTaskDefinitionRequestTypeDef:
    return {
        "taskDefinition": ...,
    }


# DeregisterTaskDefinitionRequestTypeDef definition

class DeregisterTaskDefinitionRequestTypeDef(TypedDict):
    taskDefinition: str,
```

## DescribeCapacityProvidersRequestTypeDef

```python
# DescribeCapacityProvidersRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeCapacityProvidersRequestTypeDef


def get_value() -> DescribeCapacityProvidersRequestTypeDef:
    return {
        "capacityProviders": ...,
    }


# DescribeCapacityProvidersRequestTypeDef definition

class DescribeCapacityProvidersRequestTypeDef(TypedDict):
    capacityProviders: NotRequired[Sequence[str]],
    include: NotRequired[Sequence[CapacityProviderFieldType]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: CapacityProviderFieldType](./literals.md#capacityproviderfieldtype) 
## DescribeClustersRequestTypeDef

```python
# DescribeClustersRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeClustersRequestTypeDef


def get_value() -> DescribeClustersRequestTypeDef:
    return {
        "clusters": ...,
    }


# DescribeClustersRequestTypeDef definition

class DescribeClustersRequestTypeDef(TypedDict):
    clusters: NotRequired[Sequence[str]],
    include: NotRequired[Sequence[ClusterFieldType]],  # (1)
```

1. See [:material-code-brackets: ClusterFieldType](./literals.md#clusterfieldtype) 
## DescribeContainerInstancesRequestTypeDef

```python
# DescribeContainerInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeContainerInstancesRequestTypeDef


def get_value() -> DescribeContainerInstancesRequestTypeDef:
    return {
        "containerInstances": ...,
    }


# DescribeContainerInstancesRequestTypeDef definition

class DescribeContainerInstancesRequestTypeDef(TypedDict):
    containerInstances: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[ContainerInstanceFieldType]],  # (1)
```

1. See [:material-code-brackets: ContainerInstanceFieldType](./literals.md#containerinstancefieldtype) 
## DescribeServiceDeploymentsRequestTypeDef

```python
# DescribeServiceDeploymentsRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeServiceDeploymentsRequestTypeDef


def get_value() -> DescribeServiceDeploymentsRequestTypeDef:
    return {
        "serviceDeploymentArns": ...,
    }


# DescribeServiceDeploymentsRequestTypeDef definition

class DescribeServiceDeploymentsRequestTypeDef(TypedDict):
    serviceDeploymentArns: Sequence[str],
```

## DescribeServiceRevisionsRequestTypeDef

```python
# DescribeServiceRevisionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeServiceRevisionsRequestTypeDef


def get_value() -> DescribeServiceRevisionsRequestTypeDef:
    return {
        "serviceRevisionArns": ...,
    }


# DescribeServiceRevisionsRequestTypeDef definition

class DescribeServiceRevisionsRequestTypeDef(TypedDict):
    serviceRevisionArns: Sequence[str],
```

## DescribeServicesRequestTypeDef

```python
# DescribeServicesRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeServicesRequestTypeDef


def get_value() -> DescribeServicesRequestTypeDef:
    return {
        "services": ...,
    }


# DescribeServicesRequestTypeDef definition

class DescribeServicesRequestTypeDef(TypedDict):
    services: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[ServiceFieldType]],  # (1)
```

1. See [:material-code-brackets: ServiceFieldType](./literals.md#servicefieldtype) 
## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeTaskDefinitionRequestTypeDef

```python
# DescribeTaskDefinitionRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeTaskDefinitionRequestTypeDef


def get_value() -> DescribeTaskDefinitionRequestTypeDef:
    return {
        "taskDefinition": ...,
    }


# DescribeTaskDefinitionRequestTypeDef definition

class DescribeTaskDefinitionRequestTypeDef(TypedDict):
    taskDefinition: str,
    include: NotRequired[Sequence[TaskDefinitionFieldType]],  # (1)
```

1. See [:material-code-brackets: TaskDefinitionFieldType](./literals.md#taskdefinitionfieldtype) 
## DescribeTaskSetsRequestTypeDef

```python
# DescribeTaskSetsRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeTaskSetsRequestTypeDef


def get_value() -> DescribeTaskSetsRequestTypeDef:
    return {
        "cluster": ...,
    }


# DescribeTaskSetsRequestTypeDef definition

class DescribeTaskSetsRequestTypeDef(TypedDict):
    cluster: str,
    service: str,
    taskSets: NotRequired[Sequence[str]],
    include: NotRequired[Sequence[TaskSetFieldType]],  # (1)
```

1. See [:material-code-brackets: TaskSetFieldType](./literals.md#tasksetfieldtype) 
## DescribeTasksRequestTypeDef

```python
# DescribeTasksRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeTasksRequestTypeDef


def get_value() -> DescribeTasksRequestTypeDef:
    return {
        "tasks": ...,
    }


# DescribeTasksRequestTypeDef definition

class DescribeTasksRequestTypeDef(TypedDict):
    tasks: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[TaskFieldType]],  # (1)
```

1. See [:material-code-brackets: TaskFieldType](./literals.md#taskfieldtype) 
## DeviceOutputTypeDef

```python
# DeviceOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeviceOutputTypeDef


def get_value() -> DeviceOutputTypeDef:
    return {
        "hostPath": ...,
    }


# DeviceOutputTypeDef definition

class DeviceOutputTypeDef(TypedDict):
    hostPath: str,
    containerPath: NotRequired[str],
    permissions: NotRequired[List[DeviceCgroupPermissionType]],  # (1)
```

1. See [:material-code-brackets: DeviceCgroupPermissionType](./literals.md#devicecgrouppermissiontype) 
## DeviceTypeDef

```python
# DeviceTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeviceTypeDef


def get_value() -> DeviceTypeDef:
    return {
        "hostPath": ...,
    }


# DeviceTypeDef definition

class DeviceTypeDef(TypedDict):
    hostPath: str,
    containerPath: NotRequired[str],
    permissions: NotRequired[Sequence[DeviceCgroupPermissionType]],  # (1)
```

1. See [:material-code-brackets: DeviceCgroupPermissionType](./literals.md#devicecgrouppermissiontype) 
## DiscoverPollEndpointRequestTypeDef

```python
# DiscoverPollEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DiscoverPollEndpointRequestTypeDef


def get_value() -> DiscoverPollEndpointRequestTypeDef:
    return {
        "containerInstance": ...,
    }


# DiscoverPollEndpointRequestTypeDef definition

class DiscoverPollEndpointRequestTypeDef(TypedDict):
    containerInstance: NotRequired[str],
    cluster: NotRequired[str],
```

## DockerVolumeConfigurationOutputTypeDef

```python
# DockerVolumeConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DockerVolumeConfigurationOutputTypeDef


def get_value() -> DockerVolumeConfigurationOutputTypeDef:
    return {
        "scope": ...,
    }


# DockerVolumeConfigurationOutputTypeDef definition

class DockerVolumeConfigurationOutputTypeDef(TypedDict):
    scope: NotRequired[ScopeType],  # (1)
    autoprovision: NotRequired[bool],
    driver: NotRequired[str],
    driverOpts: NotRequired[Dict[str, str]],
    labels: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## DockerVolumeConfigurationTypeDef

```python
# DockerVolumeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DockerVolumeConfigurationTypeDef


def get_value() -> DockerVolumeConfigurationTypeDef:
    return {
        "scope": ...,
    }


# DockerVolumeConfigurationTypeDef definition

class DockerVolumeConfigurationTypeDef(TypedDict):
    scope: NotRequired[ScopeType],  # (1)
    autoprovision: NotRequired[bool],
    driver: NotRequired[str],
    driverOpts: NotRequired[Mapping[str, str]],
    labels: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## EFSAuthorizationConfigTypeDef

```python
# EFSAuthorizationConfigTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import EFSAuthorizationConfigTypeDef


def get_value() -> EFSAuthorizationConfigTypeDef:
    return {
        "accessPointId": ...,
    }


# EFSAuthorizationConfigTypeDef definition

class EFSAuthorizationConfigTypeDef(TypedDict):
    accessPointId: NotRequired[str],
    iam: NotRequired[EFSAuthorizationConfigIAMType],  # (1)
```

1. See [:material-code-brackets: EFSAuthorizationConfigIAMType](./literals.md#efsauthorizationconfigiamtype) 
## EphemeralStorageTypeDef

```python
# EphemeralStorageTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import EphemeralStorageTypeDef


def get_value() -> EphemeralStorageTypeDef:
    return {
        "sizeInGiB": ...,
    }


# EphemeralStorageTypeDef definition

class EphemeralStorageTypeDef(TypedDict):
    sizeInGiB: int,
```

## ExecuteCommandLogConfigurationTypeDef

```python
# ExecuteCommandLogConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ExecuteCommandLogConfigurationTypeDef


def get_value() -> ExecuteCommandLogConfigurationTypeDef:
    return {
        "cloudWatchLogGroupName": ...,
    }


# ExecuteCommandLogConfigurationTypeDef definition

class ExecuteCommandLogConfigurationTypeDef(TypedDict):
    cloudWatchLogGroupName: NotRequired[str],
    cloudWatchEncryptionEnabled: NotRequired[bool],
    s3BucketName: NotRequired[str],
    s3EncryptionEnabled: NotRequired[bool],
    s3KeyPrefix: NotRequired[str],
```

## ExecuteCommandRequestTypeDef

```python
# ExecuteCommandRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ExecuteCommandRequestTypeDef


def get_value() -> ExecuteCommandRequestTypeDef:
    return {
        "command": ...,
    }


# ExecuteCommandRequestTypeDef definition

class ExecuteCommandRequestTypeDef(TypedDict):
    command: str,
    interactive: bool,
    task: str,
    cluster: NotRequired[str],
    container: NotRequired[str],
```

## SessionTypeDef

```python
# SessionTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import SessionTypeDef


def get_value() -> SessionTypeDef:
    return {
        "sessionId": ...,
    }


# SessionTypeDef definition

class SessionTypeDef(TypedDict):
    sessionId: NotRequired[str],
    streamUrl: NotRequired[str],
    tokenValue: NotRequired[str],
```

## FSxWindowsFileServerAuthorizationConfigTypeDef

```python
# FSxWindowsFileServerAuthorizationConfigTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import FSxWindowsFileServerAuthorizationConfigTypeDef


def get_value() -> FSxWindowsFileServerAuthorizationConfigTypeDef:
    return {
        "credentialsParameter": ...,
    }


# FSxWindowsFileServerAuthorizationConfigTypeDef definition

class FSxWindowsFileServerAuthorizationConfigTypeDef(TypedDict):
    credentialsParameter: str,
    domain: str,
```

## FirelensConfigurationTypeDef

```python
# FirelensConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import FirelensConfigurationTypeDef


def get_value() -> FirelensConfigurationTypeDef:
    return {
        "type": ...,
    }


# FirelensConfigurationTypeDef definition

class FirelensConfigurationTypeDef(TypedDict):
    type: FirelensConfigurationTypeType,  # (1)
    options: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: FirelensConfigurationTypeType](./literals.md#firelensconfigurationtypetype) 
## GetTaskProtectionRequestTypeDef

```python
# GetTaskProtectionRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import GetTaskProtectionRequestTypeDef


def get_value() -> GetTaskProtectionRequestTypeDef:
    return {
        "cluster": ...,
    }


# GetTaskProtectionRequestTypeDef definition

class GetTaskProtectionRequestTypeDef(TypedDict):
    cluster: str,
    tasks: NotRequired[Sequence[str]],
```

## ProtectedTaskTypeDef

```python
# ProtectedTaskTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ProtectedTaskTypeDef


def get_value() -> ProtectedTaskTypeDef:
    return {
        "taskArn": ...,
    }


# ProtectedTaskTypeDef definition

class ProtectedTaskTypeDef(TypedDict):
    taskArn: NotRequired[str],
    protectionEnabled: NotRequired[bool],
    expirationDate: NotRequired[datetime],
```

## HealthCheckTypeDef

```python
# HealthCheckTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import HealthCheckTypeDef


def get_value() -> HealthCheckTypeDef:
    return {
        "command": ...,
    }


# HealthCheckTypeDef definition

class HealthCheckTypeDef(TypedDict):
    command: Sequence[str],
    interval: NotRequired[int],
    timeout: NotRequired[int],
    retries: NotRequired[int],
    startPeriod: NotRequired[int],
```

## HostVolumePropertiesTypeDef

```python
# HostVolumePropertiesTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import HostVolumePropertiesTypeDef


def get_value() -> HostVolumePropertiesTypeDef:
    return {
        "sourcePath": ...,
    }


# HostVolumePropertiesTypeDef definition

class HostVolumePropertiesTypeDef(TypedDict):
    sourcePath: NotRequired[str],
```

## InferenceAcceleratorOverrideTypeDef

```python
# InferenceAcceleratorOverrideTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import InferenceAcceleratorOverrideTypeDef


def get_value() -> InferenceAcceleratorOverrideTypeDef:
    return {
        "deviceName": ...,
    }


# InferenceAcceleratorOverrideTypeDef definition

class InferenceAcceleratorOverrideTypeDef(TypedDict):
    deviceName: NotRequired[str],
    deviceType: NotRequired[str],
```

## InferenceAcceleratorTypeDef

```python
# InferenceAcceleratorTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import InferenceAcceleratorTypeDef


def get_value() -> InferenceAcceleratorTypeDef:
    return {
        "deviceName": ...,
    }


# InferenceAcceleratorTypeDef definition

class InferenceAcceleratorTypeDef(TypedDict):
    deviceName: str,
    deviceType: str,
```

## KernelCapabilitiesOutputTypeDef

```python
# KernelCapabilitiesOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import KernelCapabilitiesOutputTypeDef


def get_value() -> KernelCapabilitiesOutputTypeDef:
    return {
        "add": ...,
    }


# KernelCapabilitiesOutputTypeDef definition

class KernelCapabilitiesOutputTypeDef(TypedDict):
    add: NotRequired[List[str]],
    drop: NotRequired[List[str]],
```

## KernelCapabilitiesTypeDef

```python
# KernelCapabilitiesTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import KernelCapabilitiesTypeDef


def get_value() -> KernelCapabilitiesTypeDef:
    return {
        "add": ...,
    }


# KernelCapabilitiesTypeDef definition

class KernelCapabilitiesTypeDef(TypedDict):
    add: NotRequired[Sequence[str]],
    drop: NotRequired[Sequence[str]],
```

## TmpfsOutputTypeDef

```python
# TmpfsOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TmpfsOutputTypeDef


def get_value() -> TmpfsOutputTypeDef:
    return {
        "containerPath": ...,
    }


# TmpfsOutputTypeDef definition

class TmpfsOutputTypeDef(TypedDict):
    containerPath: str,
    size: int,
    mountOptions: NotRequired[List[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PaginatorConfigTypeDef


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

## ListAccountSettingsRequestTypeDef

```python
# ListAccountSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListAccountSettingsRequestTypeDef


def get_value() -> ListAccountSettingsRequestTypeDef:
    return {
        "name": ...,
    }


# ListAccountSettingsRequestTypeDef definition

class ListAccountSettingsRequestTypeDef(TypedDict):
    name: NotRequired[SettingNameType],  # (1)
    value: NotRequired[str],
    principalArn: NotRequired[str],
    effectiveSettings: NotRequired[bool],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
## ListAttributesRequestTypeDef

```python
# ListAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListAttributesRequestTypeDef


def get_value() -> ListAttributesRequestTypeDef:
    return {
        "targetType": ...,
    }


# ListAttributesRequestTypeDef definition

class ListAttributesRequestTypeDef(TypedDict):
    targetType: TargetTypeType,  # (1)
    cluster: NotRequired[str],
    attributeName: NotRequired[str],
    attributeValue: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
## ListClustersRequestTypeDef

```python
# ListClustersRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListClustersRequestTypeDef


def get_value() -> ListClustersRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListClustersRequestTypeDef definition

class ListClustersRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListContainerInstancesRequestTypeDef

```python
# ListContainerInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListContainerInstancesRequestTypeDef


def get_value() -> ListContainerInstancesRequestTypeDef:
    return {
        "cluster": ...,
    }


# ListContainerInstancesRequestTypeDef definition

class ListContainerInstancesRequestTypeDef(TypedDict):
    cluster: NotRequired[str],
    filter: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    status: NotRequired[ContainerInstanceStatusType],  # (1)
```

1. See [:material-code-brackets: ContainerInstanceStatusType](./literals.md#containerinstancestatustype) 
## ServiceDeploymentBriefTypeDef

```python
# ServiceDeploymentBriefTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceDeploymentBriefTypeDef


def get_value() -> ServiceDeploymentBriefTypeDef:
    return {
        "serviceDeploymentArn": ...,
    }


# ServiceDeploymentBriefTypeDef definition

class ServiceDeploymentBriefTypeDef(TypedDict):
    serviceDeploymentArn: NotRequired[str],
    serviceArn: NotRequired[str],
    clusterArn: NotRequired[str],
    startedAt: NotRequired[datetime],
    createdAt: NotRequired[datetime],
    finishedAt: NotRequired[datetime],
    targetServiceRevisionArn: NotRequired[str],
    status: NotRequired[ServiceDeploymentStatusType],  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: ServiceDeploymentStatusType](./literals.md#servicedeploymentstatustype) 
## ListServicesByNamespaceRequestTypeDef

```python
# ListServicesByNamespaceRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListServicesByNamespaceRequestTypeDef


def get_value() -> ListServicesByNamespaceRequestTypeDef:
    return {
        "namespace": ...,
    }


# ListServicesByNamespaceRequestTypeDef definition

class ListServicesByNamespaceRequestTypeDef(TypedDict):
    namespace: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListServicesRequestTypeDef

```python
# ListServicesRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListServicesRequestTypeDef


def get_value() -> ListServicesRequestTypeDef:
    return {
        "cluster": ...,
    }


# ListServicesRequestTypeDef definition

class ListServicesRequestTypeDef(TypedDict):
    cluster: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    launchType: NotRequired[LaunchTypeType],  # (1)
    schedulingStrategy: NotRequired[SchedulingStrategyType],  # (2)
```

1. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
2. See [:material-code-brackets: SchedulingStrategyType](./literals.md#schedulingstrategytype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTaskDefinitionFamiliesRequestTypeDef

```python
# ListTaskDefinitionFamiliesRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListTaskDefinitionFamiliesRequestTypeDef


def get_value() -> ListTaskDefinitionFamiliesRequestTypeDef:
    return {
        "familyPrefix": ...,
    }


# ListTaskDefinitionFamiliesRequestTypeDef definition

class ListTaskDefinitionFamiliesRequestTypeDef(TypedDict):
    familyPrefix: NotRequired[str],
    status: NotRequired[TaskDefinitionFamilyStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TaskDefinitionFamilyStatusType](./literals.md#taskdefinitionfamilystatustype) 
## ListTaskDefinitionsRequestTypeDef

```python
# ListTaskDefinitionsRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListTaskDefinitionsRequestTypeDef


def get_value() -> ListTaskDefinitionsRequestTypeDef:
    return {
        "familyPrefix": ...,
    }


# ListTaskDefinitionsRequestTypeDef definition

class ListTaskDefinitionsRequestTypeDef(TypedDict):
    familyPrefix: NotRequired[str],
    status: NotRequired[TaskDefinitionStatusType],  # (1)
    sort: NotRequired[SortOrderType],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TaskDefinitionStatusType](./literals.md#taskdefinitionstatustype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListTasksRequestTypeDef

```python
# ListTasksRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListTasksRequestTypeDef


def get_value() -> ListTasksRequestTypeDef:
    return {
        "cluster": ...,
    }


# ListTasksRequestTypeDef definition

class ListTasksRequestTypeDef(TypedDict):
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
# ManagedAgentStateChangeTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ManagedAgentStateChangeTypeDef


def get_value() -> ManagedAgentStateChangeTypeDef:
    return {
        "containerName": ...,
    }


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
# PlatformDeviceTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PlatformDeviceTypeDef


def get_value() -> PlatformDeviceTypeDef:
    return {
        "id": ...,
    }


# PlatformDeviceTypeDef definition

class PlatformDeviceTypeDef(TypedDict):
    id: str,
    type: PlatformDeviceTypeType,  # (1)
```

1. See [:material-code-brackets: PlatformDeviceTypeType](./literals.md#platformdevicetypetype) 
## PutAccountSettingDefaultRequestTypeDef

```python
# PutAccountSettingDefaultRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PutAccountSettingDefaultRequestTypeDef


def get_value() -> PutAccountSettingDefaultRequestTypeDef:
    return {
        "name": ...,
    }


# PutAccountSettingDefaultRequestTypeDef definition

class PutAccountSettingDefaultRequestTypeDef(TypedDict):
    name: SettingNameType,  # (1)
    value: str,
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
## PutAccountSettingRequestTypeDef

```python
# PutAccountSettingRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PutAccountSettingRequestTypeDef


def get_value() -> PutAccountSettingRequestTypeDef:
    return {
        "name": ...,
    }


# PutAccountSettingRequestTypeDef definition

class PutAccountSettingRequestTypeDef(TypedDict):
    name: SettingNameType,  # (1)
    value: str,
    principalArn: NotRequired[str],
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
## RuntimePlatformTypeDef

```python
# RuntimePlatformTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import RuntimePlatformTypeDef


def get_value() -> RuntimePlatformTypeDef:
    return {
        "cpuArchitecture": ...,
    }


# RuntimePlatformTypeDef definition

class RuntimePlatformTypeDef(TypedDict):
    cpuArchitecture: NotRequired[CPUArchitectureType],  # (1)
    operatingSystemFamily: NotRequired[OSFamilyType],  # (2)
```

1. See [:material-code-brackets: CPUArchitectureType](./literals.md#cpuarchitecturetype) 
2. See [:material-code-brackets: OSFamilyType](./literals.md#osfamilytype) 
## TaskDefinitionPlacementConstraintTypeDef

```python
# TaskDefinitionPlacementConstraintTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TaskDefinitionPlacementConstraintTypeDef


def get_value() -> TaskDefinitionPlacementConstraintTypeDef:
    return {
        "type": ...,
    }


# TaskDefinitionPlacementConstraintTypeDef definition

class TaskDefinitionPlacementConstraintTypeDef(TypedDict):
    type: NotRequired[TaskDefinitionPlacementConstraintTypeType],  # (1)
    expression: NotRequired[str],
```

1. See [:material-code-brackets: TaskDefinitionPlacementConstraintTypeType](./literals.md#taskdefinitionplacementconstrainttypetype) 
## ResourceTypeDef

```python
# ResourceTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ResourceTypeDef


def get_value() -> ResourceTypeDef:
    return {
        "name": ...,
    }


# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    doubleValue: NotRequired[float],
    longValue: NotRequired[int],
    integerValue: NotRequired[int],
    stringSetValue: NotRequired[Sequence[str]],
```

## RollbackTypeDef

```python
# RollbackTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import RollbackTypeDef


def get_value() -> RollbackTypeDef:
    return {
        "reason": ...,
    }


# RollbackTypeDef definition

class RollbackTypeDef(TypedDict):
    reason: NotRequired[str],
    startedAt: NotRequired[datetime],
    serviceRevisionArn: NotRequired[str],
```

## ServiceConnectClientAliasTypeDef

```python
# ServiceConnectClientAliasTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceConnectClientAliasTypeDef


def get_value() -> ServiceConnectClientAliasTypeDef:
    return {
        "port": ...,
    }


# ServiceConnectClientAliasTypeDef definition

class ServiceConnectClientAliasTypeDef(TypedDict):
    port: int,
    dnsName: NotRequired[str],
```

## TimeoutConfigurationTypeDef

```python
# TimeoutConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TimeoutConfigurationTypeDef


def get_value() -> TimeoutConfigurationTypeDef:
    return {
        "idleTimeoutSeconds": ...,
    }


# TimeoutConfigurationTypeDef definition

class TimeoutConfigurationTypeDef(TypedDict):
    idleTimeoutSeconds: NotRequired[int],
    perRequestTimeoutSeconds: NotRequired[int],
```

## ServiceConnectTlsCertificateAuthorityTypeDef

```python
# ServiceConnectTlsCertificateAuthorityTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceConnectTlsCertificateAuthorityTypeDef


def get_value() -> ServiceConnectTlsCertificateAuthorityTypeDef:
    return {
        "awsPcaAuthorityArn": ...,
    }


# ServiceConnectTlsCertificateAuthorityTypeDef definition

class ServiceConnectTlsCertificateAuthorityTypeDef(TypedDict):
    awsPcaAuthorityArn: NotRequired[str],
```

## ServiceDeploymentAlarmsTypeDef

```python
# ServiceDeploymentAlarmsTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceDeploymentAlarmsTypeDef


def get_value() -> ServiceDeploymentAlarmsTypeDef:
    return {
        "status": ...,
    }


# ServiceDeploymentAlarmsTypeDef definition

class ServiceDeploymentAlarmsTypeDef(TypedDict):
    status: NotRequired[ServiceDeploymentRollbackMonitorsStatusType],  # (1)
    alarmNames: NotRequired[List[str]],
    triggeredAlarmNames: NotRequired[List[str]],
```

1. See [:material-code-brackets: ServiceDeploymentRollbackMonitorsStatusType](./literals.md#servicedeploymentrollbackmonitorsstatustype) 
## ServiceDeploymentCircuitBreakerTypeDef

```python
# ServiceDeploymentCircuitBreakerTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceDeploymentCircuitBreakerTypeDef


def get_value() -> ServiceDeploymentCircuitBreakerTypeDef:
    return {
        "status": ...,
    }


# ServiceDeploymentCircuitBreakerTypeDef definition

class ServiceDeploymentCircuitBreakerTypeDef(TypedDict):
    status: NotRequired[ServiceDeploymentRollbackMonitorsStatusType],  # (1)
    failureCount: NotRequired[int],
    threshold: NotRequired[int],
```

1. See [:material-code-brackets: ServiceDeploymentRollbackMonitorsStatusType](./literals.md#servicedeploymentrollbackmonitorsstatustype) 
## ServiceRevisionSummaryTypeDef

```python
# ServiceRevisionSummaryTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceRevisionSummaryTypeDef


def get_value() -> ServiceRevisionSummaryTypeDef:
    return {
        "arn": ...,
    }


# ServiceRevisionSummaryTypeDef definition

class ServiceRevisionSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    requestedTaskCount: NotRequired[int],
    runningTaskCount: NotRequired[int],
    pendingTaskCount: NotRequired[int],
```

## ServiceEventTypeDef

```python
# ServiceEventTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceEventTypeDef


def get_value() -> ServiceEventTypeDef:
    return {
        "id": ...,
    }


# ServiceEventTypeDef definition

class ServiceEventTypeDef(TypedDict):
    id: NotRequired[str],
    createdAt: NotRequired[datetime],
    message: NotRequired[str],
```

## StopTaskRequestTypeDef

```python
# StopTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import StopTaskRequestTypeDef


def get_value() -> StopTaskRequestTypeDef:
    return {
        "task": ...,
    }


# StopTaskRequestTypeDef definition

class StopTaskRequestTypeDef(TypedDict):
    task: str,
    cluster: NotRequired[str],
    reason: NotRequired[str],
```

## TaskEphemeralStorageTypeDef

```python
# TaskEphemeralStorageTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TaskEphemeralStorageTypeDef


def get_value() -> TaskEphemeralStorageTypeDef:
    return {
        "sizeInGiB": ...,
    }


# TaskEphemeralStorageTypeDef definition

class TaskEphemeralStorageTypeDef(TypedDict):
    sizeInGiB: NotRequired[int],
    kmsKeyId: NotRequired[str],
```

## TaskManagedEBSVolumeTerminationPolicyTypeDef

```python
# TaskManagedEBSVolumeTerminationPolicyTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TaskManagedEBSVolumeTerminationPolicyTypeDef


def get_value() -> TaskManagedEBSVolumeTerminationPolicyTypeDef:
    return {
        "deleteOnTermination": ...,
    }


# TaskManagedEBSVolumeTerminationPolicyTypeDef definition

class TaskManagedEBSVolumeTerminationPolicyTypeDef(TypedDict):
    deleteOnTermination: bool,
```

## TmpfsTypeDef

```python
# TmpfsTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TmpfsTypeDef


def get_value() -> TmpfsTypeDef:
    return {
        "containerPath": ...,
    }


# TmpfsTypeDef definition

class TmpfsTypeDef(TypedDict):
    containerPath: str,
    size: int,
    mountOptions: NotRequired[Sequence[str]],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateContainerAgentRequestTypeDef

```python
# UpdateContainerAgentRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateContainerAgentRequestTypeDef


def get_value() -> UpdateContainerAgentRequestTypeDef:
    return {
        "containerInstance": ...,
    }


# UpdateContainerAgentRequestTypeDef definition

class UpdateContainerAgentRequestTypeDef(TypedDict):
    containerInstance: str,
    cluster: NotRequired[str],
```

## UpdateContainerInstancesStateRequestTypeDef

```python
# UpdateContainerInstancesStateRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateContainerInstancesStateRequestTypeDef


def get_value() -> UpdateContainerInstancesStateRequestTypeDef:
    return {
        "containerInstances": ...,
    }


# UpdateContainerInstancesStateRequestTypeDef definition

class UpdateContainerInstancesStateRequestTypeDef(TypedDict):
    containerInstances: Sequence[str],
    status: ContainerInstanceStatusType,  # (1)
    cluster: NotRequired[str],
```

1. See [:material-code-brackets: ContainerInstanceStatusType](./literals.md#containerinstancestatustype) 
## UpdateServicePrimaryTaskSetRequestTypeDef

```python
# UpdateServicePrimaryTaskSetRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateServicePrimaryTaskSetRequestTypeDef


def get_value() -> UpdateServicePrimaryTaskSetRequestTypeDef:
    return {
        "cluster": ...,
    }


# UpdateServicePrimaryTaskSetRequestTypeDef definition

class UpdateServicePrimaryTaskSetRequestTypeDef(TypedDict):
    cluster: str,
    service: str,
    primaryTaskSet: str,
```

## UpdateTaskProtectionRequestTypeDef

```python
# UpdateTaskProtectionRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateTaskProtectionRequestTypeDef


def get_value() -> UpdateTaskProtectionRequestTypeDef:
    return {
        "cluster": ...,
    }


# UpdateTaskProtectionRequestTypeDef definition

class UpdateTaskProtectionRequestTypeDef(TypedDict):
    cluster: str,
    tasks: Sequence[str],
    protectionEnabled: bool,
    expiresInMinutes: NotRequired[int],
```

## SubmitAttachmentStateChangesRequestTypeDef

```python
# SubmitAttachmentStateChangesRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import SubmitAttachmentStateChangesRequestTypeDef


def get_value() -> SubmitAttachmentStateChangesRequestTypeDef:
    return {
        "attachments": ...,
    }


# SubmitAttachmentStateChangesRequestTypeDef definition

class SubmitAttachmentStateChangesRequestTypeDef(TypedDict):
    attachments: Sequence[AttachmentStateChangeTypeDef],  # (1)
    cluster: NotRequired[str],
```

1. See [:material-code-braces: AttachmentStateChangeTypeDef](./type_defs.md#attachmentstatechangetypedef) 
## AttachmentTypeDef

```python
# AttachmentTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import AttachmentTypeDef


def get_value() -> AttachmentTypeDef:
    return {
        "id": ...,
    }


# AttachmentTypeDef definition

class AttachmentTypeDef(TypedDict):
    id: NotRequired[str],
    type: NotRequired[str],
    status: NotRequired[str],
    details: NotRequired[List[KeyValuePairTypeDef]],  # (1)
```

1. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
## ProxyConfigurationOutputTypeDef

```python
# ProxyConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ProxyConfigurationOutputTypeDef


def get_value() -> ProxyConfigurationOutputTypeDef:
    return {
        "type": ...,
    }


# ProxyConfigurationOutputTypeDef definition

class ProxyConfigurationOutputTypeDef(TypedDict):
    containerName: str,
    type: NotRequired[ProxyConfigurationTypeType],  # (1)
    properties: NotRequired[List[KeyValuePairTypeDef]],  # (2)
```

1. See [:material-code-brackets: ProxyConfigurationTypeType](./literals.md#proxyconfigurationtypetype) 
2. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
## ProxyConfigurationTypeDef

```python
# ProxyConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ProxyConfigurationTypeDef


def get_value() -> ProxyConfigurationTypeDef:
    return {
        "type": ...,
    }


# ProxyConfigurationTypeDef definition

class ProxyConfigurationTypeDef(TypedDict):
    containerName: str,
    type: NotRequired[ProxyConfigurationTypeType],  # (1)
    properties: NotRequired[Sequence[KeyValuePairTypeDef]],  # (2)
```

1. See [:material-code-brackets: ProxyConfigurationTypeType](./literals.md#proxyconfigurationtypetype) 
2. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
## DeleteAttributesRequestTypeDef

```python
# DeleteAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteAttributesRequestTypeDef


def get_value() -> DeleteAttributesRequestTypeDef:
    return {
        "attributes": ...,
    }


# DeleteAttributesRequestTypeDef definition

class DeleteAttributesRequestTypeDef(TypedDict):
    attributes: Sequence[AttributeTypeDef],  # (1)
    cluster: NotRequired[str],
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## PutAttributesRequestTypeDef

```python
# PutAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PutAttributesRequestTypeDef


def get_value() -> PutAttributesRequestTypeDef:
    return {
        "attributes": ...,
    }


# PutAttributesRequestTypeDef definition

class PutAttributesRequestTypeDef(TypedDict):
    attributes: Sequence[AttributeTypeDef],  # (1)
    cluster: NotRequired[str],
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## AutoScalingGroupProviderTypeDef

```python
# AutoScalingGroupProviderTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import AutoScalingGroupProviderTypeDef


def get_value() -> AutoScalingGroupProviderTypeDef:
    return {
        "autoScalingGroupArn": ...,
    }


# AutoScalingGroupProviderTypeDef definition

class AutoScalingGroupProviderTypeDef(TypedDict):
    autoScalingGroupArn: str,
    managedScaling: NotRequired[ManagedScalingTypeDef],  # (1)
    managedTerminationProtection: NotRequired[ManagedTerminationProtectionType],  # (2)
    managedDraining: NotRequired[ManagedDrainingType],  # (3)
```

1. See [:material-code-braces: ManagedScalingTypeDef](./type_defs.md#managedscalingtypedef) 
2. See [:material-code-brackets: ManagedTerminationProtectionType](./literals.md#managedterminationprotectiontype) 
3. See [:material-code-brackets: ManagedDrainingType](./literals.md#manageddrainingtype) 
## AutoScalingGroupProviderUpdateTypeDef

```python
# AutoScalingGroupProviderUpdateTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import AutoScalingGroupProviderUpdateTypeDef


def get_value() -> AutoScalingGroupProviderUpdateTypeDef:
    return {
        "managedScaling": ...,
    }


# AutoScalingGroupProviderUpdateTypeDef definition

class AutoScalingGroupProviderUpdateTypeDef(TypedDict):
    managedScaling: NotRequired[ManagedScalingTypeDef],  # (1)
    managedTerminationProtection: NotRequired[ManagedTerminationProtectionType],  # (2)
    managedDraining: NotRequired[ManagedDrainingType],  # (3)
```

1. See [:material-code-braces: ManagedScalingTypeDef](./type_defs.md#managedscalingtypedef) 
2. See [:material-code-brackets: ManagedTerminationProtectionType](./literals.md#managedterminationprotectiontype) 
3. See [:material-code-brackets: ManagedDrainingType](./literals.md#manageddrainingtype) 
## NetworkConfigurationOutputTypeDef

```python
# NetworkConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import NetworkConfigurationOutputTypeDef


def get_value() -> NetworkConfigurationOutputTypeDef:
    return {
        "awsvpcConfiguration": ...,
    }


# NetworkConfigurationOutputTypeDef definition

class NetworkConfigurationOutputTypeDef(TypedDict):
    awsvpcConfiguration: NotRequired[AwsVpcConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: AwsVpcConfigurationOutputTypeDef](./type_defs.md#awsvpcconfigurationoutputtypedef) 
## NetworkConfigurationTypeDef

```python
# NetworkConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import NetworkConfigurationTypeDef


def get_value() -> NetworkConfigurationTypeDef:
    return {
        "awsvpcConfiguration": ...,
    }


# NetworkConfigurationTypeDef definition

class NetworkConfigurationTypeDef(TypedDict):
    awsvpcConfiguration: NotRequired[AwsVpcConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AwsVpcConfigurationTypeDef](./type_defs.md#awsvpcconfigurationtypedef) 
## PutClusterCapacityProvidersRequestTypeDef

```python
# PutClusterCapacityProvidersRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PutClusterCapacityProvidersRequestTypeDef


def get_value() -> PutClusterCapacityProvidersRequestTypeDef:
    return {
        "cluster": ...,
    }


# PutClusterCapacityProvidersRequestTypeDef definition

class PutClusterCapacityProvidersRequestTypeDef(TypedDict):
    cluster: str,
    capacityProviders: Sequence[str],
    defaultCapacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef],  # (1)
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
## EBSTagSpecificationOutputTypeDef

```python
# EBSTagSpecificationOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import EBSTagSpecificationOutputTypeDef


def get_value() -> EBSTagSpecificationOutputTypeDef:
    return {
        "resourceType": ...,
    }


# EBSTagSpecificationOutputTypeDef definition

class EBSTagSpecificationOutputTypeDef(TypedDict):
    resourceType: EBSResourceTypeType,  # (1)
    tags: NotRequired[List[TagTypeDef]],  # (2)
    propagateTags: NotRequired[PropagateTagsType],  # (3)
```

1. See [:material-code-brackets: EBSResourceTypeType](./literals.md#ebsresourcetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
## EBSTagSpecificationTypeDef

```python
# EBSTagSpecificationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import EBSTagSpecificationTypeDef


def get_value() -> EBSTagSpecificationTypeDef:
    return {
        "resourceType": ...,
    }


# EBSTagSpecificationTypeDef definition

class EBSTagSpecificationTypeDef(TypedDict):
    resourceType: EBSResourceTypeType,  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    propagateTags: NotRequired[PropagateTagsType],  # (3)
```

1. See [:material-code-brackets: EBSResourceTypeType](./literals.md#ebsresourcetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateClusterSettingsRequestTypeDef

```python
# UpdateClusterSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateClusterSettingsRequestTypeDef


def get_value() -> UpdateClusterSettingsRequestTypeDef:
    return {
        "cluster": ...,
    }


# UpdateClusterSettingsRequestTypeDef definition

class UpdateClusterSettingsRequestTypeDef(TypedDict):
    cluster: str,
    settings: Sequence[ClusterSettingTypeDef],  # (1)
```

1. See [:material-code-braces: ClusterSettingTypeDef](./type_defs.md#clustersettingtypedef) 
## ContainerOverrideOutputTypeDef

```python
# ContainerOverrideOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerOverrideOutputTypeDef


def get_value() -> ContainerOverrideOutputTypeDef:
    return {
        "name": ...,
    }


# ContainerOverrideOutputTypeDef definition

class ContainerOverrideOutputTypeDef(TypedDict):
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
## ContainerOverrideTypeDef

```python
# ContainerOverrideTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerOverrideTypeDef


def get_value() -> ContainerOverrideTypeDef:
    return {
        "name": ...,
    }


# ContainerOverrideTypeDef definition

class ContainerOverrideTypeDef(TypedDict):
    name: NotRequired[str],
    command: NotRequired[Sequence[str]],
    environment: NotRequired[Sequence[KeyValuePairTypeDef]],  # (1)
    environmentFiles: NotRequired[Sequence[EnvironmentFileTypeDef]],  # (2)
    cpu: NotRequired[int],
    memory: NotRequired[int],
    memoryReservation: NotRequired[int],
    resourceRequirements: NotRequired[Sequence[ResourceRequirementTypeDef]],  # (3)
```

1. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
2. See [:material-code-braces: EnvironmentFileTypeDef](./type_defs.md#environmentfiletypedef) 
3. See [:material-code-braces: ResourceRequirementTypeDef](./type_defs.md#resourcerequirementtypedef) 
## LogConfigurationOutputTypeDef

```python
# LogConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import LogConfigurationOutputTypeDef


def get_value() -> LogConfigurationOutputTypeDef:
    return {
        "logDriver": ...,
    }


# LogConfigurationOutputTypeDef definition

class LogConfigurationOutputTypeDef(TypedDict):
    logDriver: LogDriverType,  # (1)
    options: NotRequired[Dict[str, str]],
    secretOptions: NotRequired[List[SecretTypeDef]],  # (2)
```

1. See [:material-code-brackets: LogDriverType](./literals.md#logdrivertype) 
2. See [:material-code-braces: SecretTypeDef](./type_defs.md#secrettypedef) 
## LogConfigurationTypeDef

```python
# LogConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import LogConfigurationTypeDef


def get_value() -> LogConfigurationTypeDef:
    return {
        "logDriver": ...,
    }


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
# ContainerInstanceHealthStatusTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerInstanceHealthStatusTypeDef


def get_value() -> ContainerInstanceHealthStatusTypeDef:
    return {
        "overallStatus": ...,
    }


# ContainerInstanceHealthStatusTypeDef definition

class ContainerInstanceHealthStatusTypeDef(TypedDict):
    overallStatus: NotRequired[InstanceHealthCheckStateType],  # (1)
    details: NotRequired[List[InstanceHealthCheckResultTypeDef]],  # (2)
```

1. See [:material-code-brackets: InstanceHealthCheckStateType](./literals.md#instancehealthcheckstatetype) 
2. See [:material-code-braces: InstanceHealthCheckResultTypeDef](./type_defs.md#instancehealthcheckresulttypedef) 
## ContainerStateChangeTypeDef

```python
# ContainerStateChangeTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerStateChangeTypeDef


def get_value() -> ContainerStateChangeTypeDef:
    return {
        "containerName": ...,
    }


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
## SubmitContainerStateChangeRequestTypeDef

```python
# SubmitContainerStateChangeRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import SubmitContainerStateChangeRequestTypeDef


def get_value() -> SubmitContainerStateChangeRequestTypeDef:
    return {
        "cluster": ...,
    }


# SubmitContainerStateChangeRequestTypeDef definition

class SubmitContainerStateChangeRequestTypeDef(TypedDict):
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
# ContainerTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerTypeDef


def get_value() -> ContainerTypeDef:
    return {
        "containerArn": ...,
    }


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
# DeleteAttributesResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteAttributesResponseTypeDef


def get_value() -> DeleteAttributesResponseTypeDef:
    return {
        "attributes": ...,
    }


# DeleteAttributesResponseTypeDef definition

class DeleteAttributesResponseTypeDef(TypedDict):
    attributes: List[AttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DiscoverPollEndpointResponseTypeDef

```python
# DiscoverPollEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DiscoverPollEndpointResponseTypeDef


def get_value() -> DiscoverPollEndpointResponseTypeDef:
    return {
        "endpoint": ...,
    }


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
# ListAttributesResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListAttributesResponseTypeDef


def get_value() -> ListAttributesResponseTypeDef:
    return {
        "attributes": ...,
    }


# ListAttributesResponseTypeDef definition

class ListAttributesResponseTypeDef(TypedDict):
    attributes: List[AttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersResponseTypeDef

```python
# ListClustersResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListClustersResponseTypeDef


def get_value() -> ListClustersResponseTypeDef:
    return {
        "clusterArns": ...,
    }


# ListClustersResponseTypeDef definition

class ListClustersResponseTypeDef(TypedDict):
    clusterArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContainerInstancesResponseTypeDef

```python
# ListContainerInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListContainerInstancesResponseTypeDef


def get_value() -> ListContainerInstancesResponseTypeDef:
    return {
        "containerInstanceArns": ...,
    }


# ListContainerInstancesResponseTypeDef definition

class ListContainerInstancesResponseTypeDef(TypedDict):
    containerInstanceArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServicesByNamespaceResponseTypeDef

```python
# ListServicesByNamespaceResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListServicesByNamespaceResponseTypeDef


def get_value() -> ListServicesByNamespaceResponseTypeDef:
    return {
        "serviceArns": ...,
    }


# ListServicesByNamespaceResponseTypeDef definition

class ListServicesByNamespaceResponseTypeDef(TypedDict):
    serviceArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServicesResponseTypeDef

```python
# ListServicesResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListServicesResponseTypeDef


def get_value() -> ListServicesResponseTypeDef:
    return {
        "serviceArns": ...,
    }


# ListServicesResponseTypeDef definition

class ListServicesResponseTypeDef(TypedDict):
    serviceArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTaskDefinitionFamiliesResponseTypeDef

```python
# ListTaskDefinitionFamiliesResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListTaskDefinitionFamiliesResponseTypeDef


def get_value() -> ListTaskDefinitionFamiliesResponseTypeDef:
    return {
        "families": ...,
    }


# ListTaskDefinitionFamiliesResponseTypeDef definition

class ListTaskDefinitionFamiliesResponseTypeDef(TypedDict):
    families: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTaskDefinitionsResponseTypeDef

```python
# ListTaskDefinitionsResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListTaskDefinitionsResponseTypeDef


def get_value() -> ListTaskDefinitionsResponseTypeDef:
    return {
        "taskDefinitionArns": ...,
    }


# ListTaskDefinitionsResponseTypeDef definition

class ListTaskDefinitionsResponseTypeDef(TypedDict):
    taskDefinitionArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTasksResponseTypeDef

```python
# ListTasksResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListTasksResponseTypeDef


def get_value() -> ListTasksResponseTypeDef:
    return {
        "taskArns": ...,
    }


# ListTasksResponseTypeDef definition

class ListTasksResponseTypeDef(TypedDict):
    taskArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAttributesResponseTypeDef

```python
# PutAttributesResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PutAttributesResponseTypeDef


def get_value() -> PutAttributesResponseTypeDef:
    return {
        "attributes": ...,
    }


# PutAttributesResponseTypeDef definition

class PutAttributesResponseTypeDef(TypedDict):
    attributes: List[AttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubmitAttachmentStateChangesResponseTypeDef

```python
# SubmitAttachmentStateChangesResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import SubmitAttachmentStateChangesResponseTypeDef


def get_value() -> SubmitAttachmentStateChangesResponseTypeDef:
    return {
        "acknowledgment": ...,
    }


# SubmitAttachmentStateChangesResponseTypeDef definition

class SubmitAttachmentStateChangesResponseTypeDef(TypedDict):
    acknowledgment: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubmitContainerStateChangeResponseTypeDef

```python
# SubmitContainerStateChangeResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import SubmitContainerStateChangeResponseTypeDef


def get_value() -> SubmitContainerStateChangeResponseTypeDef:
    return {
        "acknowledgment": ...,
    }


# SubmitContainerStateChangeResponseTypeDef definition

class SubmitContainerStateChangeResponseTypeDef(TypedDict):
    acknowledgment: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubmitTaskStateChangeResponseTypeDef

```python
# SubmitTaskStateChangeResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import SubmitTaskStateChangeResponseTypeDef


def get_value() -> SubmitTaskStateChangeResponseTypeDef:
    return {
        "acknowledgment": ...,
    }


# SubmitTaskStateChangeResponseTypeDef definition

class SubmitTaskStateChangeResponseTypeDef(TypedDict):
    acknowledgment: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTaskSetRequestTypeDef

```python
# UpdateTaskSetRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateTaskSetRequestTypeDef


def get_value() -> UpdateTaskSetRequestTypeDef:
    return {
        "cluster": ...,
    }


# UpdateTaskSetRequestTypeDef definition

class UpdateTaskSetRequestTypeDef(TypedDict):
    cluster: str,
    service: str,
    taskSet: str,
    scale: ScaleTypeDef,  # (1)
```

1. See [:material-code-braces: ScaleTypeDef](./type_defs.md#scaletypedef) 
## CreatedAtTypeDef

```python
# CreatedAtTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import CreatedAtTypeDef


def get_value() -> CreatedAtTypeDef:
    return {
        "before": ...,
    }


# CreatedAtTypeDef definition

class CreatedAtTypeDef(TypedDict):
    before: NotRequired[TimestampTypeDef],
    after: NotRequired[TimestampTypeDef],
```

## DeleteAccountSettingResponseTypeDef

```python
# DeleteAccountSettingResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteAccountSettingResponseTypeDef


def get_value() -> DeleteAccountSettingResponseTypeDef:
    return {
        "setting": ...,
    }


# DeleteAccountSettingResponseTypeDef definition

class DeleteAccountSettingResponseTypeDef(TypedDict):
    setting: SettingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SettingTypeDef](./type_defs.md#settingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountSettingsResponseTypeDef

```python
# ListAccountSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListAccountSettingsResponseTypeDef


def get_value() -> ListAccountSettingsResponseTypeDef:
    return {
        "settings": ...,
    }


# ListAccountSettingsResponseTypeDef definition

class ListAccountSettingsResponseTypeDef(TypedDict):
    settings: List[SettingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SettingTypeDef](./type_defs.md#settingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAccountSettingDefaultResponseTypeDef

```python
# PutAccountSettingDefaultResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PutAccountSettingDefaultResponseTypeDef


def get_value() -> PutAccountSettingDefaultResponseTypeDef:
    return {
        "setting": ...,
    }


# PutAccountSettingDefaultResponseTypeDef definition

class PutAccountSettingDefaultResponseTypeDef(TypedDict):
    setting: SettingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SettingTypeDef](./type_defs.md#settingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAccountSettingResponseTypeDef

```python
# PutAccountSettingResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PutAccountSettingResponseTypeDef


def get_value() -> PutAccountSettingResponseTypeDef:
    return {
        "setting": ...,
    }


# PutAccountSettingResponseTypeDef definition

class PutAccountSettingResponseTypeDef(TypedDict):
    setting: SettingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SettingTypeDef](./type_defs.md#settingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentConfigurationOutputTypeDef

```python
# DeploymentConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeploymentConfigurationOutputTypeDef


def get_value() -> DeploymentConfigurationOutputTypeDef:
    return {
        "deploymentCircuitBreaker": ...,
    }


# DeploymentConfigurationOutputTypeDef definition

class DeploymentConfigurationOutputTypeDef(TypedDict):
    deploymentCircuitBreaker: NotRequired[DeploymentCircuitBreakerTypeDef],  # (1)
    maximumPercent: NotRequired[int],
    minimumHealthyPercent: NotRequired[int],
    alarms: NotRequired[DeploymentAlarmsOutputTypeDef],  # (2)
```

1. See [:material-code-braces: DeploymentCircuitBreakerTypeDef](./type_defs.md#deploymentcircuitbreakertypedef) 
2. See [:material-code-braces: DeploymentAlarmsOutputTypeDef](./type_defs.md#deploymentalarmsoutputtypedef) 
## DeploymentConfigurationTypeDef

```python
# DeploymentConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeploymentConfigurationTypeDef


def get_value() -> DeploymentConfigurationTypeDef:
    return {
        "deploymentCircuitBreaker": ...,
    }


# DeploymentConfigurationTypeDef definition

class DeploymentConfigurationTypeDef(TypedDict):
    deploymentCircuitBreaker: NotRequired[DeploymentCircuitBreakerTypeDef],  # (1)
    maximumPercent: NotRequired[int],
    minimumHealthyPercent: NotRequired[int],
    alarms: NotRequired[DeploymentAlarmsTypeDef],  # (2)
```

1. See [:material-code-braces: DeploymentCircuitBreakerTypeDef](./type_defs.md#deploymentcircuitbreakertypedef) 
2. See [:material-code-braces: DeploymentAlarmsTypeDef](./type_defs.md#deploymentalarmstypedef) 
## DescribeServicesRequestWaitExtraTypeDef

```python
# DescribeServicesRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeServicesRequestWaitExtraTypeDef


def get_value() -> DescribeServicesRequestWaitExtraTypeDef:
    return {
        "services": ...,
    }


# DescribeServicesRequestWaitExtraTypeDef definition

class DescribeServicesRequestWaitExtraTypeDef(TypedDict):
    services: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[ServiceFieldType]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceFieldType](./literals.md#servicefieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeServicesRequestWaitTypeDef

```python
# DescribeServicesRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeServicesRequestWaitTypeDef


def get_value() -> DescribeServicesRequestWaitTypeDef:
    return {
        "services": ...,
    }


# DescribeServicesRequestWaitTypeDef definition

class DescribeServicesRequestWaitTypeDef(TypedDict):
    services: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[ServiceFieldType]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceFieldType](./literals.md#servicefieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTasksRequestWaitExtraTypeDef

```python
# DescribeTasksRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeTasksRequestWaitExtraTypeDef


def get_value() -> DescribeTasksRequestWaitExtraTypeDef:
    return {
        "tasks": ...,
    }


# DescribeTasksRequestWaitExtraTypeDef definition

class DescribeTasksRequestWaitExtraTypeDef(TypedDict):
    tasks: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[TaskFieldType]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskFieldType](./literals.md#taskfieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTasksRequestWaitTypeDef

```python
# DescribeTasksRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeTasksRequestWaitTypeDef


def get_value() -> DescribeTasksRequestWaitTypeDef:
    return {
        "tasks": ...,
    }


# DescribeTasksRequestWaitTypeDef definition

class DescribeTasksRequestWaitTypeDef(TypedDict):
    tasks: Sequence[str],
    cluster: NotRequired[str],
    include: NotRequired[Sequence[TaskFieldType]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskFieldType](./literals.md#taskfieldtype) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## EFSVolumeConfigurationTypeDef

```python
# EFSVolumeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import EFSVolumeConfigurationTypeDef


def get_value() -> EFSVolumeConfigurationTypeDef:
    return {
        "fileSystemId": ...,
    }


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
# ExecuteCommandConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ExecuteCommandConfigurationTypeDef


def get_value() -> ExecuteCommandConfigurationTypeDef:
    return {
        "kmsKeyId": ...,
    }


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
# ExecuteCommandResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ExecuteCommandResponseTypeDef


def get_value() -> ExecuteCommandResponseTypeDef:
    return {
        "clusterArn": ...,
    }


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
# FSxWindowsFileServerVolumeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import FSxWindowsFileServerVolumeConfigurationTypeDef


def get_value() -> FSxWindowsFileServerVolumeConfigurationTypeDef:
    return {
        "fileSystemId": ...,
    }


# FSxWindowsFileServerVolumeConfigurationTypeDef definition

class FSxWindowsFileServerVolumeConfigurationTypeDef(TypedDict):
    fileSystemId: str,
    rootDirectory: str,
    authorizationConfig: FSxWindowsFileServerAuthorizationConfigTypeDef,  # (1)
```

1. See [:material-code-braces: FSxWindowsFileServerAuthorizationConfigTypeDef](./type_defs.md#fsxwindowsfileserverauthorizationconfigtypedef) 
## GetTaskProtectionResponseTypeDef

```python
# GetTaskProtectionResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import GetTaskProtectionResponseTypeDef


def get_value() -> GetTaskProtectionResponseTypeDef:
    return {
        "protectedTasks": ...,
    }


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
# UpdateTaskProtectionResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateTaskProtectionResponseTypeDef


def get_value() -> UpdateTaskProtectionResponseTypeDef:
    return {
        "protectedTasks": ...,
    }


# UpdateTaskProtectionResponseTypeDef definition

class UpdateTaskProtectionResponseTypeDef(TypedDict):
    protectedTasks: List[ProtectedTaskTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProtectedTaskTypeDef](./type_defs.md#protectedtasktypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LinuxParametersOutputTypeDef

```python
# LinuxParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import LinuxParametersOutputTypeDef


def get_value() -> LinuxParametersOutputTypeDef:
    return {
        "capabilities": ...,
    }


# LinuxParametersOutputTypeDef definition

class LinuxParametersOutputTypeDef(TypedDict):
    capabilities: NotRequired[KernelCapabilitiesOutputTypeDef],  # (1)
    devices: NotRequired[List[DeviceOutputTypeDef]],  # (2)
    initProcessEnabled: NotRequired[bool],
    sharedMemorySize: NotRequired[int],
    tmpfs: NotRequired[List[TmpfsOutputTypeDef]],  # (3)
    maxSwap: NotRequired[int],
    swappiness: NotRequired[int],
```

1. See [:material-code-braces: KernelCapabilitiesOutputTypeDef](./type_defs.md#kernelcapabilitiesoutputtypedef) 
2. See [:material-code-braces: DeviceOutputTypeDef](./type_defs.md#deviceoutputtypedef) 
3. See [:material-code-braces: TmpfsOutputTypeDef](./type_defs.md#tmpfsoutputtypedef) 
## ListAccountSettingsRequestPaginateTypeDef

```python
# ListAccountSettingsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListAccountSettingsRequestPaginateTypeDef


def get_value() -> ListAccountSettingsRequestPaginateTypeDef:
    return {
        "name": ...,
    }


# ListAccountSettingsRequestPaginateTypeDef definition

class ListAccountSettingsRequestPaginateTypeDef(TypedDict):
    name: NotRequired[SettingNameType],  # (1)
    value: NotRequired[str],
    principalArn: NotRequired[str],
    effectiveSettings: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SettingNameType](./literals.md#settingnametype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttributesRequestPaginateTypeDef

```python
# ListAttributesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListAttributesRequestPaginateTypeDef


def get_value() -> ListAttributesRequestPaginateTypeDef:
    return {
        "targetType": ...,
    }


# ListAttributesRequestPaginateTypeDef definition

class ListAttributesRequestPaginateTypeDef(TypedDict):
    targetType: TargetTypeType,  # (1)
    cluster: NotRequired[str],
    attributeName: NotRequired[str],
    attributeValue: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersRequestPaginateTypeDef

```python
# ListClustersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListClustersRequestPaginateTypeDef


def get_value() -> ListClustersRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListClustersRequestPaginateTypeDef definition

class ListClustersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContainerInstancesRequestPaginateTypeDef

```python
# ListContainerInstancesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListContainerInstancesRequestPaginateTypeDef


def get_value() -> ListContainerInstancesRequestPaginateTypeDef:
    return {
        "cluster": ...,
    }


# ListContainerInstancesRequestPaginateTypeDef definition

class ListContainerInstancesRequestPaginateTypeDef(TypedDict):
    cluster: NotRequired[str],
    filter: NotRequired[str],
    status: NotRequired[ContainerInstanceStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ContainerInstanceStatusType](./literals.md#containerinstancestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesByNamespaceRequestPaginateTypeDef

```python
# ListServicesByNamespaceRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListServicesByNamespaceRequestPaginateTypeDef


def get_value() -> ListServicesByNamespaceRequestPaginateTypeDef:
    return {
        "namespace": ...,
    }


# ListServicesByNamespaceRequestPaginateTypeDef definition

class ListServicesByNamespaceRequestPaginateTypeDef(TypedDict):
    namespace: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesRequestPaginateTypeDef

```python
# ListServicesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListServicesRequestPaginateTypeDef


def get_value() -> ListServicesRequestPaginateTypeDef:
    return {
        "cluster": ...,
    }


# ListServicesRequestPaginateTypeDef definition

class ListServicesRequestPaginateTypeDef(TypedDict):
    cluster: NotRequired[str],
    launchType: NotRequired[LaunchTypeType],  # (1)
    schedulingStrategy: NotRequired[SchedulingStrategyType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
2. See [:material-code-brackets: SchedulingStrategyType](./literals.md#schedulingstrategytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTaskDefinitionFamiliesRequestPaginateTypeDef

```python
# ListTaskDefinitionFamiliesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListTaskDefinitionFamiliesRequestPaginateTypeDef


def get_value() -> ListTaskDefinitionFamiliesRequestPaginateTypeDef:
    return {
        "familyPrefix": ...,
    }


# ListTaskDefinitionFamiliesRequestPaginateTypeDef definition

class ListTaskDefinitionFamiliesRequestPaginateTypeDef(TypedDict):
    familyPrefix: NotRequired[str],
    status: NotRequired[TaskDefinitionFamilyStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskDefinitionFamilyStatusType](./literals.md#taskdefinitionfamilystatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTaskDefinitionsRequestPaginateTypeDef

```python
# ListTaskDefinitionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListTaskDefinitionsRequestPaginateTypeDef


def get_value() -> ListTaskDefinitionsRequestPaginateTypeDef:
    return {
        "familyPrefix": ...,
    }


# ListTaskDefinitionsRequestPaginateTypeDef definition

class ListTaskDefinitionsRequestPaginateTypeDef(TypedDict):
    familyPrefix: NotRequired[str],
    status: NotRequired[TaskDefinitionStatusType],  # (1)
    sort: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: TaskDefinitionStatusType](./literals.md#taskdefinitionstatustype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTasksRequestPaginateTypeDef

```python
# ListTasksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListTasksRequestPaginateTypeDef


def get_value() -> ListTasksRequestPaginateTypeDef:
    return {
        "cluster": ...,
    }


# ListTasksRequestPaginateTypeDef definition

class ListTasksRequestPaginateTypeDef(TypedDict):
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
## ListServiceDeploymentsResponseTypeDef

```python
# ListServiceDeploymentsResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListServiceDeploymentsResponseTypeDef


def get_value() -> ListServiceDeploymentsResponseTypeDef:
    return {
        "serviceDeployments": ...,
    }


# ListServiceDeploymentsResponseTypeDef definition

class ListServiceDeploymentsResponseTypeDef(TypedDict):
    serviceDeployments: List[ServiceDeploymentBriefTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceDeploymentBriefTypeDef](./type_defs.md#servicedeploymentbrieftypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceConnectTlsConfigurationTypeDef

```python
# ServiceConnectTlsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceConnectTlsConfigurationTypeDef


def get_value() -> ServiceConnectTlsConfigurationTypeDef:
    return {
        "issuerCertificateAuthority": ...,
    }


# ServiceConnectTlsConfigurationTypeDef definition

class ServiceConnectTlsConfigurationTypeDef(TypedDict):
    issuerCertificateAuthority: ServiceConnectTlsCertificateAuthorityTypeDef,  # (1)
    kmsKey: NotRequired[str],
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: ServiceConnectTlsCertificateAuthorityTypeDef](./type_defs.md#serviceconnecttlscertificateauthoritytypedef) 
## CapacityProviderTypeDef

```python
# CapacityProviderTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import CapacityProviderTypeDef


def get_value() -> CapacityProviderTypeDef:
    return {
        "capacityProviderArn": ...,
    }


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
## CreateCapacityProviderRequestTypeDef

```python
# CreateCapacityProviderRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import CreateCapacityProviderRequestTypeDef


def get_value() -> CreateCapacityProviderRequestTypeDef:
    return {
        "name": ...,
    }


# CreateCapacityProviderRequestTypeDef definition

class CreateCapacityProviderRequestTypeDef(TypedDict):
    name: str,
    autoScalingGroupProvider: AutoScalingGroupProviderTypeDef,  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: AutoScalingGroupProviderTypeDef](./type_defs.md#autoscalinggroupprovidertypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateCapacityProviderRequestTypeDef

```python
# UpdateCapacityProviderRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateCapacityProviderRequestTypeDef


def get_value() -> UpdateCapacityProviderRequestTypeDef:
    return {
        "name": ...,
    }


# UpdateCapacityProviderRequestTypeDef definition

class UpdateCapacityProviderRequestTypeDef(TypedDict):
    name: str,
    autoScalingGroupProvider: AutoScalingGroupProviderUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: AutoScalingGroupProviderUpdateTypeDef](./type_defs.md#autoscalinggroupproviderupdatetypedef) 
## TaskSetTypeDef

```python
# TaskSetTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TaskSetTypeDef


def get_value() -> TaskSetTypeDef:
    return {
        "id": ...,
    }


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
    networkConfiguration: NotRequired[NetworkConfigurationOutputTypeDef],  # (3)
    loadBalancers: NotRequired[List[LoadBalancerTypeDef]],  # (4)
    serviceRegistries: NotRequired[List[ServiceRegistryTypeDef]],  # (5)
    scale: NotRequired[ScaleTypeDef],  # (6)
    stabilityStatus: NotRequired[StabilityStatusType],  # (7)
    stabilityStatusAt: NotRequired[datetime],
    tags: NotRequired[List[TagTypeDef]],  # (8)
    fargateEphemeralStorage: NotRequired[DeploymentEphemeralStorageTypeDef],  # (9)
```

1. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
2. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
3. See [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
4. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
5. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
6. See [:material-code-braces: ScaleTypeDef](./type_defs.md#scaletypedef) 
7. See [:material-code-brackets: StabilityStatusType](./literals.md#stabilitystatustype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: DeploymentEphemeralStorageTypeDef](./type_defs.md#deploymentephemeralstoragetypedef) 
## ServiceManagedEBSVolumeConfigurationOutputTypeDef

```python
# ServiceManagedEBSVolumeConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceManagedEBSVolumeConfigurationOutputTypeDef


def get_value() -> ServiceManagedEBSVolumeConfigurationOutputTypeDef:
    return {
        "encrypted": ...,
    }


# ServiceManagedEBSVolumeConfigurationOutputTypeDef definition

class ServiceManagedEBSVolumeConfigurationOutputTypeDef(TypedDict):
    roleArn: str,
    encrypted: NotRequired[bool],
    kmsKeyId: NotRequired[str],
    volumeType: NotRequired[str],
    sizeInGiB: NotRequired[int],
    snapshotId: NotRequired[str],
    iops: NotRequired[int],
    throughput: NotRequired[int],
    tagSpecifications: NotRequired[List[EBSTagSpecificationOutputTypeDef]],  # (1)
    filesystemType: NotRequired[TaskFilesystemTypeType],  # (2)
```

1. See [:material-code-braces: EBSTagSpecificationOutputTypeDef](./type_defs.md#ebstagspecificationoutputtypedef) 
2. See [:material-code-brackets: TaskFilesystemTypeType](./literals.md#taskfilesystemtypetype) 
## TaskOverrideOutputTypeDef

```python
# TaskOverrideOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TaskOverrideOutputTypeDef


def get_value() -> TaskOverrideOutputTypeDef:
    return {
        "containerOverrides": ...,
    }


# TaskOverrideOutputTypeDef definition

class TaskOverrideOutputTypeDef(TypedDict):
    containerOverrides: NotRequired[List[ContainerOverrideOutputTypeDef]],  # (1)
    cpu: NotRequired[str],
    inferenceAcceleratorOverrides: NotRequired[List[InferenceAcceleratorOverrideTypeDef]],  # (2)
    executionRoleArn: NotRequired[str],
    memory: NotRequired[str],
    taskRoleArn: NotRequired[str],
    ephemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (3)
```

1. See [:material-code-braces: ContainerOverrideOutputTypeDef](./type_defs.md#containeroverrideoutputtypedef) 
2. See [:material-code-braces: InferenceAcceleratorOverrideTypeDef](./type_defs.md#inferenceacceleratoroverridetypedef) 
3. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
## TaskOverrideTypeDef

```python
# TaskOverrideTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TaskOverrideTypeDef


def get_value() -> TaskOverrideTypeDef:
    return {
        "containerOverrides": ...,
    }


# TaskOverrideTypeDef definition

class TaskOverrideTypeDef(TypedDict):
    containerOverrides: NotRequired[Sequence[ContainerOverrideTypeDef]],  # (1)
    cpu: NotRequired[str],
    inferenceAcceleratorOverrides: NotRequired[Sequence[InferenceAcceleratorOverrideTypeDef]],  # (2)
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
# ContainerInstanceTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerInstanceTypeDef


def get_value() -> ContainerInstanceTypeDef:
    return {
        "containerInstanceArn": ...,
    }


# ContainerInstanceTypeDef definition

class ContainerInstanceTypeDef(TypedDict):
    containerInstanceArn: NotRequired[str],
    ec2InstanceId: NotRequired[str],
    capacityProviderName: NotRequired[str],
    version: NotRequired[int],
    versionInfo: NotRequired[VersionInfoTypeDef],  # (1)
    remainingResources: NotRequired[List[ResourceOutputTypeDef]],  # (2)
    registeredResources: NotRequired[List[ResourceOutputTypeDef]],  # (2)
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
2. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
3. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
4. See [:material-code-brackets: AgentUpdateStatusType](./literals.md#agentupdatestatustype) 
5. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
6. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: ContainerInstanceHealthStatusTypeDef](./type_defs.md#containerinstancehealthstatustypedef) 
## SubmitTaskStateChangeRequestTypeDef

```python
# SubmitTaskStateChangeRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import SubmitTaskStateChangeRequestTypeDef


def get_value() -> SubmitTaskStateChangeRequestTypeDef:
    return {
        "cluster": ...,
    }


# SubmitTaskStateChangeRequestTypeDef definition

class SubmitTaskStateChangeRequestTypeDef(TypedDict):
    cluster: NotRequired[str],
    task: NotRequired[str],
    status: NotRequired[str],
    reason: NotRequired[str],
    containers: NotRequired[Sequence[ContainerStateChangeTypeDef]],  # (1)
    attachments: NotRequired[Sequence[AttachmentStateChangeTypeDef]],  # (2)
    managedAgents: NotRequired[Sequence[ManagedAgentStateChangeTypeDef]],  # (3)
    pullStartedAt: NotRequired[TimestampTypeDef],
    pullStoppedAt: NotRequired[TimestampTypeDef],
    executionStoppedAt: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: ContainerStateChangeTypeDef](./type_defs.md#containerstatechangetypedef) 
2. See [:material-code-braces: AttachmentStateChangeTypeDef](./type_defs.md#attachmentstatechangetypedef) 
3. See [:material-code-braces: ManagedAgentStateChangeTypeDef](./type_defs.md#managedagentstatechangetypedef) 
## ListServiceDeploymentsRequestTypeDef

```python
# ListServiceDeploymentsRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ListServiceDeploymentsRequestTypeDef


def get_value() -> ListServiceDeploymentsRequestTypeDef:
    return {
        "service": ...,
    }


# ListServiceDeploymentsRequestTypeDef definition

class ListServiceDeploymentsRequestTypeDef(TypedDict):
    service: str,
    cluster: NotRequired[str],
    status: NotRequired[Sequence[ServiceDeploymentStatusType]],  # (1)
    createdAt: NotRequired[CreatedAtTypeDef],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ServiceDeploymentStatusType](./literals.md#servicedeploymentstatustype) 
2. See [:material-code-braces: CreatedAtTypeDef](./type_defs.md#createdattypedef) 
## ServiceDeploymentTypeDef

```python
# ServiceDeploymentTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceDeploymentTypeDef


def get_value() -> ServiceDeploymentTypeDef:
    return {
        "serviceDeploymentArn": ...,
    }


# ServiceDeploymentTypeDef definition

class ServiceDeploymentTypeDef(TypedDict):
    serviceDeploymentArn: NotRequired[str],
    serviceArn: NotRequired[str],
    clusterArn: NotRequired[str],
    createdAt: NotRequired[datetime],
    startedAt: NotRequired[datetime],
    finishedAt: NotRequired[datetime],
    stoppedAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    sourceServiceRevisions: NotRequired[List[ServiceRevisionSummaryTypeDef]],  # (1)
    targetServiceRevision: NotRequired[ServiceRevisionSummaryTypeDef],  # (2)
    status: NotRequired[ServiceDeploymentStatusType],  # (3)
    statusReason: NotRequired[str],
    deploymentConfiguration: NotRequired[DeploymentConfigurationOutputTypeDef],  # (4)
    rollback: NotRequired[RollbackTypeDef],  # (5)
    deploymentCircuitBreaker: NotRequired[ServiceDeploymentCircuitBreakerTypeDef],  # (6)
    alarms: NotRequired[ServiceDeploymentAlarmsTypeDef],  # (7)
```

1. See [:material-code-braces: ServiceRevisionSummaryTypeDef](./type_defs.md#servicerevisionsummarytypedef) 
2. See [:material-code-braces: ServiceRevisionSummaryTypeDef](./type_defs.md#servicerevisionsummarytypedef) 
3. See [:material-code-brackets: ServiceDeploymentStatusType](./literals.md#servicedeploymentstatustype) 
4. See [:material-code-braces: DeploymentConfigurationOutputTypeDef](./type_defs.md#deploymentconfigurationoutputtypedef) 
5. See [:material-code-braces: RollbackTypeDef](./type_defs.md#rollbacktypedef) 
6. See [:material-code-braces: ServiceDeploymentCircuitBreakerTypeDef](./type_defs.md#servicedeploymentcircuitbreakertypedef) 
7. See [:material-code-braces: ServiceDeploymentAlarmsTypeDef](./type_defs.md#servicedeploymentalarmstypedef) 
## ClusterConfigurationTypeDef

```python
# ClusterConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ClusterConfigurationTypeDef


def get_value() -> ClusterConfigurationTypeDef:
    return {
        "executeCommandConfiguration": ...,
    }


# ClusterConfigurationTypeDef definition

class ClusterConfigurationTypeDef(TypedDict):
    executeCommandConfiguration: NotRequired[ExecuteCommandConfigurationTypeDef],  # (1)
    managedStorageConfiguration: NotRequired[ManagedStorageConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ExecuteCommandConfigurationTypeDef](./type_defs.md#executecommandconfigurationtypedef) 
2. See [:material-code-braces: ManagedStorageConfigurationTypeDef](./type_defs.md#managedstorageconfigurationtypedef) 
## VolumeOutputTypeDef

```python
# VolumeOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import VolumeOutputTypeDef


def get_value() -> VolumeOutputTypeDef:
    return {
        "name": ...,
    }


# VolumeOutputTypeDef definition

class VolumeOutputTypeDef(TypedDict):
    name: NotRequired[str],
    host: NotRequired[HostVolumePropertiesTypeDef],  # (1)
    dockerVolumeConfiguration: NotRequired[DockerVolumeConfigurationOutputTypeDef],  # (2)
    efsVolumeConfiguration: NotRequired[EFSVolumeConfigurationTypeDef],  # (3)
    fsxWindowsFileServerVolumeConfiguration: NotRequired[FSxWindowsFileServerVolumeConfigurationTypeDef],  # (4)
    configuredAtLaunch: NotRequired[bool],
```

1. See [:material-code-braces: HostVolumePropertiesTypeDef](./type_defs.md#hostvolumepropertiestypedef) 
2. See [:material-code-braces: DockerVolumeConfigurationOutputTypeDef](./type_defs.md#dockervolumeconfigurationoutputtypedef) 
3. See [:material-code-braces: EFSVolumeConfigurationTypeDef](./type_defs.md#efsvolumeconfigurationtypedef) 
4. See [:material-code-braces: FSxWindowsFileServerVolumeConfigurationTypeDef](./type_defs.md#fsxwindowsfileservervolumeconfigurationtypedef) 
## VolumeTypeDef

```python
# VolumeTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import VolumeTypeDef


def get_value() -> VolumeTypeDef:
    return {
        "name": ...,
    }


# VolumeTypeDef definition

class VolumeTypeDef(TypedDict):
    name: NotRequired[str],
    host: NotRequired[HostVolumePropertiesTypeDef],  # (1)
    dockerVolumeConfiguration: NotRequired[DockerVolumeConfigurationUnionTypeDef],  # (2)
    efsVolumeConfiguration: NotRequired[EFSVolumeConfigurationTypeDef],  # (3)
    fsxWindowsFileServerVolumeConfiguration: NotRequired[FSxWindowsFileServerVolumeConfigurationTypeDef],  # (4)
    configuredAtLaunch: NotRequired[bool],
```

1. See [:material-code-braces: HostVolumePropertiesTypeDef](./type_defs.md#hostvolumepropertiestypedef) 
2. See [:material-code-braces: DockerVolumeConfigurationTypeDef](./type_defs.md#dockervolumeconfigurationtypedef) [:material-code-braces: DockerVolumeConfigurationOutputTypeDef](./type_defs.md#dockervolumeconfigurationoutputtypedef) 
3. See [:material-code-braces: EFSVolumeConfigurationTypeDef](./type_defs.md#efsvolumeconfigurationtypedef) 
4. See [:material-code-braces: FSxWindowsFileServerVolumeConfigurationTypeDef](./type_defs.md#fsxwindowsfileservervolumeconfigurationtypedef) 
## ContainerDefinitionOutputTypeDef

```python
# ContainerDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerDefinitionOutputTypeDef


def get_value() -> ContainerDefinitionOutputTypeDef:
    return {
        "name": ...,
    }


# ContainerDefinitionOutputTypeDef definition

class ContainerDefinitionOutputTypeDef(TypedDict):
    name: NotRequired[str],
    image: NotRequired[str],
    repositoryCredentials: NotRequired[RepositoryCredentialsTypeDef],  # (1)
    cpu: NotRequired[int],
    memory: NotRequired[int],
    memoryReservation: NotRequired[int],
    links: NotRequired[List[str]],
    portMappings: NotRequired[List[PortMappingTypeDef]],  # (2)
    essential: NotRequired[bool],
    restartPolicy: NotRequired[ContainerRestartPolicyOutputTypeDef],  # (3)
    entryPoint: NotRequired[List[str]],
    command: NotRequired[List[str]],
    environment: NotRequired[List[KeyValuePairTypeDef]],  # (4)
    environmentFiles: NotRequired[List[EnvironmentFileTypeDef]],  # (5)
    mountPoints: NotRequired[List[MountPointTypeDef]],  # (6)
    volumesFrom: NotRequired[List[VolumeFromTypeDef]],  # (7)
    linuxParameters: NotRequired[LinuxParametersOutputTypeDef],  # (8)
    secrets: NotRequired[List[SecretTypeDef]],  # (9)
    dependsOn: NotRequired[List[ContainerDependencyTypeDef]],  # (10)
    startTimeout: NotRequired[int],
    stopTimeout: NotRequired[int],
    versionConsistency: NotRequired[VersionConsistencyType],  # (11)
    hostname: NotRequired[str],
    user: NotRequired[str],
    workingDirectory: NotRequired[str],
    disableNetworking: NotRequired[bool],
    privileged: NotRequired[bool],
    readonlyRootFilesystem: NotRequired[bool],
    dnsServers: NotRequired[List[str]],
    dnsSearchDomains: NotRequired[List[str]],
    extraHosts: NotRequired[List[HostEntryTypeDef]],  # (12)
    dockerSecurityOptions: NotRequired[List[str]],
    interactive: NotRequired[bool],
    pseudoTerminal: NotRequired[bool],
    dockerLabels: NotRequired[Dict[str, str]],
    ulimits: NotRequired[List[UlimitTypeDef]],  # (13)
    logConfiguration: NotRequired[LogConfigurationOutputTypeDef],  # (14)
    healthCheck: NotRequired[HealthCheckOutputTypeDef],  # (15)
    systemControls: NotRequired[List[SystemControlTypeDef]],  # (16)
    resourceRequirements: NotRequired[List[ResourceRequirementTypeDef]],  # (17)
    firelensConfiguration: NotRequired[FirelensConfigurationOutputTypeDef],  # (18)
    credentialSpecs: NotRequired[List[str]],
```

1. See [:material-code-braces: RepositoryCredentialsTypeDef](./type_defs.md#repositorycredentialstypedef) 
2. See [:material-code-braces: PortMappingTypeDef](./type_defs.md#portmappingtypedef) 
3. See [:material-code-braces: ContainerRestartPolicyOutputTypeDef](./type_defs.md#containerrestartpolicyoutputtypedef) 
4. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
5. See [:material-code-braces: EnvironmentFileTypeDef](./type_defs.md#environmentfiletypedef) 
6. See [:material-code-braces: MountPointTypeDef](./type_defs.md#mountpointtypedef) 
7. See [:material-code-braces: VolumeFromTypeDef](./type_defs.md#volumefromtypedef) 
8. See [:material-code-braces: LinuxParametersOutputTypeDef](./type_defs.md#linuxparametersoutputtypedef) 
9. See [:material-code-braces: SecretTypeDef](./type_defs.md#secrettypedef) 
10. See [:material-code-braces: ContainerDependencyTypeDef](./type_defs.md#containerdependencytypedef) 
11. See [:material-code-brackets: VersionConsistencyType](./literals.md#versionconsistencytype) 
12. See [:material-code-braces: HostEntryTypeDef](./type_defs.md#hostentrytypedef) 
13. See [:material-code-braces: UlimitTypeDef](./type_defs.md#ulimittypedef) 
14. See [:material-code-braces: LogConfigurationOutputTypeDef](./type_defs.md#logconfigurationoutputtypedef) 
15. See [:material-code-braces: HealthCheckOutputTypeDef](./type_defs.md#healthcheckoutputtypedef) 
16. See [:material-code-braces: SystemControlTypeDef](./type_defs.md#systemcontroltypedef) 
17. See [:material-code-braces: ResourceRequirementTypeDef](./type_defs.md#resourcerequirementtypedef) 
18. See [:material-code-braces: FirelensConfigurationOutputTypeDef](./type_defs.md#firelensconfigurationoutputtypedef) 
## RegisterContainerInstanceRequestTypeDef

```python
# RegisterContainerInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import RegisterContainerInstanceRequestTypeDef


def get_value() -> RegisterContainerInstanceRequestTypeDef:
    return {
        "cluster": ...,
    }


# RegisterContainerInstanceRequestTypeDef definition

class RegisterContainerInstanceRequestTypeDef(TypedDict):
    cluster: NotRequired[str],
    instanceIdentityDocument: NotRequired[str],
    instanceIdentityDocumentSignature: NotRequired[str],
    totalResources: NotRequired[Sequence[ResourceUnionTypeDef]],  # (1)
    versionInfo: NotRequired[VersionInfoTypeDef],  # (2)
    containerInstanceArn: NotRequired[str],
    attributes: NotRequired[Sequence[AttributeTypeDef]],  # (3)
    platformDevices: NotRequired[Sequence[PlatformDeviceTypeDef]],  # (4)
    tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
2. See [:material-code-braces: VersionInfoTypeDef](./type_defs.md#versioninfotypedef) 
3. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
4. See [:material-code-braces: PlatformDeviceTypeDef](./type_defs.md#platformdevicetypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ServiceConnectServiceOutputTypeDef

```python
# ServiceConnectServiceOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceConnectServiceOutputTypeDef


def get_value() -> ServiceConnectServiceOutputTypeDef:
    return {
        "portName": ...,
    }


# ServiceConnectServiceOutputTypeDef definition

class ServiceConnectServiceOutputTypeDef(TypedDict):
    portName: str,
    discoveryName: NotRequired[str],
    clientAliases: NotRequired[List[ServiceConnectClientAliasTypeDef]],  # (1)
    ingressPortOverride: NotRequired[int],
    timeout: NotRequired[TimeoutConfigurationTypeDef],  # (2)
    tls: NotRequired[ServiceConnectTlsConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: ServiceConnectClientAliasTypeDef](./type_defs.md#serviceconnectclientaliastypedef) 
2. See [:material-code-braces: TimeoutConfigurationTypeDef](./type_defs.md#timeoutconfigurationtypedef) 
3. See [:material-code-braces: ServiceConnectTlsConfigurationTypeDef](./type_defs.md#serviceconnecttlsconfigurationtypedef) 
## ServiceConnectServiceTypeDef

```python
# ServiceConnectServiceTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceConnectServiceTypeDef


def get_value() -> ServiceConnectServiceTypeDef:
    return {
        "portName": ...,
    }


# ServiceConnectServiceTypeDef definition

class ServiceConnectServiceTypeDef(TypedDict):
    portName: str,
    discoveryName: NotRequired[str],
    clientAliases: NotRequired[Sequence[ServiceConnectClientAliasTypeDef]],  # (1)
    ingressPortOverride: NotRequired[int],
    timeout: NotRequired[TimeoutConfigurationTypeDef],  # (2)
    tls: NotRequired[ServiceConnectTlsConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: ServiceConnectClientAliasTypeDef](./type_defs.md#serviceconnectclientaliastypedef) 
2. See [:material-code-braces: TimeoutConfigurationTypeDef](./type_defs.md#timeoutconfigurationtypedef) 
3. See [:material-code-braces: ServiceConnectTlsConfigurationTypeDef](./type_defs.md#serviceconnecttlsconfigurationtypedef) 
## LinuxParametersTypeDef

```python
# LinuxParametersTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import LinuxParametersTypeDef


def get_value() -> LinuxParametersTypeDef:
    return {
        "capabilities": ...,
    }


# LinuxParametersTypeDef definition

class LinuxParametersTypeDef(TypedDict):
    capabilities: NotRequired[KernelCapabilitiesUnionTypeDef],  # (1)
    devices: NotRequired[Sequence[DeviceUnionTypeDef]],  # (2)
    initProcessEnabled: NotRequired[bool],
    sharedMemorySize: NotRequired[int],
    tmpfs: NotRequired[Sequence[TmpfsUnionTypeDef]],  # (3)
    maxSwap: NotRequired[int],
    swappiness: NotRequired[int],
```

1. See [:material-code-braces: KernelCapabilitiesTypeDef](./type_defs.md#kernelcapabilitiestypedef) [:material-code-braces: KernelCapabilitiesOutputTypeDef](./type_defs.md#kernelcapabilitiesoutputtypedef) 
2. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) [:material-code-braces: DeviceOutputTypeDef](./type_defs.md#deviceoutputtypedef) 
3. See [:material-code-braces: TmpfsTypeDef](./type_defs.md#tmpfstypedef) [:material-code-braces: TmpfsOutputTypeDef](./type_defs.md#tmpfsoutputtypedef) 
## CreateCapacityProviderResponseTypeDef

```python
# CreateCapacityProviderResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import CreateCapacityProviderResponseTypeDef


def get_value() -> CreateCapacityProviderResponseTypeDef:
    return {
        "capacityProvider": ...,
    }


# CreateCapacityProviderResponseTypeDef definition

class CreateCapacityProviderResponseTypeDef(TypedDict):
    capacityProvider: CapacityProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapacityProviderTypeDef](./type_defs.md#capacityprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCapacityProviderResponseTypeDef

```python
# DeleteCapacityProviderResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteCapacityProviderResponseTypeDef


def get_value() -> DeleteCapacityProviderResponseTypeDef:
    return {
        "capacityProvider": ...,
    }


# DeleteCapacityProviderResponseTypeDef definition

class DeleteCapacityProviderResponseTypeDef(TypedDict):
    capacityProvider: CapacityProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapacityProviderTypeDef](./type_defs.md#capacityprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCapacityProvidersResponseTypeDef

```python
# DescribeCapacityProvidersResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeCapacityProvidersResponseTypeDef


def get_value() -> DescribeCapacityProvidersResponseTypeDef:
    return {
        "capacityProviders": ...,
    }


# DescribeCapacityProvidersResponseTypeDef definition

class DescribeCapacityProvidersResponseTypeDef(TypedDict):
    capacityProviders: List[CapacityProviderTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CapacityProviderTypeDef](./type_defs.md#capacityprovidertypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCapacityProviderResponseTypeDef

```python
# UpdateCapacityProviderResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateCapacityProviderResponseTypeDef


def get_value() -> UpdateCapacityProviderResponseTypeDef:
    return {
        "capacityProvider": ...,
    }


# UpdateCapacityProviderResponseTypeDef definition

class UpdateCapacityProviderResponseTypeDef(TypedDict):
    capacityProvider: CapacityProviderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapacityProviderTypeDef](./type_defs.md#capacityprovidertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTaskSetResponseTypeDef

```python
# CreateTaskSetResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import CreateTaskSetResponseTypeDef


def get_value() -> CreateTaskSetResponseTypeDef:
    return {
        "taskSet": ...,
    }


# CreateTaskSetResponseTypeDef definition

class CreateTaskSetResponseTypeDef(TypedDict):
    taskSet: TaskSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskSetTypeDef](./type_defs.md#tasksettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTaskSetResponseTypeDef

```python
# DeleteTaskSetResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteTaskSetResponseTypeDef


def get_value() -> DeleteTaskSetResponseTypeDef:
    return {
        "taskSet": ...,
    }


# DeleteTaskSetResponseTypeDef definition

class DeleteTaskSetResponseTypeDef(TypedDict):
    taskSet: TaskSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskSetTypeDef](./type_defs.md#tasksettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTaskSetsResponseTypeDef

```python
# DescribeTaskSetsResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeTaskSetsResponseTypeDef


def get_value() -> DescribeTaskSetsResponseTypeDef:
    return {
        "taskSets": ...,
    }


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
# UpdateServicePrimaryTaskSetResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateServicePrimaryTaskSetResponseTypeDef


def get_value() -> UpdateServicePrimaryTaskSetResponseTypeDef:
    return {
        "taskSet": ...,
    }


# UpdateServicePrimaryTaskSetResponseTypeDef definition

class UpdateServicePrimaryTaskSetResponseTypeDef(TypedDict):
    taskSet: TaskSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskSetTypeDef](./type_defs.md#tasksettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTaskSetResponseTypeDef

```python
# UpdateTaskSetResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateTaskSetResponseTypeDef


def get_value() -> UpdateTaskSetResponseTypeDef:
    return {
        "taskSet": ...,
    }


# UpdateTaskSetResponseTypeDef definition

class UpdateTaskSetResponseTypeDef(TypedDict):
    taskSet: TaskSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskSetTypeDef](./type_defs.md#tasksettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTaskSetRequestTypeDef

```python
# CreateTaskSetRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import CreateTaskSetRequestTypeDef


def get_value() -> CreateTaskSetRequestTypeDef:
    return {
        "service": ...,
    }


# CreateTaskSetRequestTypeDef definition

class CreateTaskSetRequestTypeDef(TypedDict):
    service: str,
    cluster: str,
    taskDefinition: str,
    externalId: NotRequired[str],
    networkConfiguration: NotRequired[NetworkConfigurationUnionTypeDef],  # (1)
    loadBalancers: NotRequired[Sequence[LoadBalancerTypeDef]],  # (2)
    serviceRegistries: NotRequired[Sequence[ServiceRegistryTypeDef]],  # (3)
    launchType: NotRequired[LaunchTypeType],  # (4)
    capacityProviderStrategy: NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],  # (5)
    platformVersion: NotRequired[str],
    scale: NotRequired[ScaleTypeDef],  # (6)
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (7)
```

1. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
2. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
3. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
4. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
5. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
6. See [:material-code-braces: ScaleTypeDef](./type_defs.md#scaletypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ServiceVolumeConfigurationOutputTypeDef

```python
# ServiceVolumeConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceVolumeConfigurationOutputTypeDef


def get_value() -> ServiceVolumeConfigurationOutputTypeDef:
    return {
        "name": ...,
    }


# ServiceVolumeConfigurationOutputTypeDef definition

class ServiceVolumeConfigurationOutputTypeDef(TypedDict):
    name: str,
    managedEBSVolume: NotRequired[ServiceManagedEBSVolumeConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ServiceManagedEBSVolumeConfigurationOutputTypeDef](./type_defs.md#servicemanagedebsvolumeconfigurationoutputtypedef) 
## ServiceManagedEBSVolumeConfigurationTypeDef

```python
# ServiceManagedEBSVolumeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceManagedEBSVolumeConfigurationTypeDef


def get_value() -> ServiceManagedEBSVolumeConfigurationTypeDef:
    return {
        "encrypted": ...,
    }


# ServiceManagedEBSVolumeConfigurationTypeDef definition

class ServiceManagedEBSVolumeConfigurationTypeDef(TypedDict):
    roleArn: str,
    encrypted: NotRequired[bool],
    kmsKeyId: NotRequired[str],
    volumeType: NotRequired[str],
    sizeInGiB: NotRequired[int],
    snapshotId: NotRequired[str],
    iops: NotRequired[int],
    throughput: NotRequired[int],
    tagSpecifications: NotRequired[Sequence[EBSTagSpecificationUnionTypeDef]],  # (1)
    filesystemType: NotRequired[TaskFilesystemTypeType],  # (2)
```

1. See [:material-code-braces: EBSTagSpecificationTypeDef](./type_defs.md#ebstagspecificationtypedef) [:material-code-braces: EBSTagSpecificationOutputTypeDef](./type_defs.md#ebstagspecificationoutputtypedef) 
2. See [:material-code-brackets: TaskFilesystemTypeType](./literals.md#taskfilesystemtypetype) 
## TaskManagedEBSVolumeConfigurationTypeDef

```python
# TaskManagedEBSVolumeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TaskManagedEBSVolumeConfigurationTypeDef


def get_value() -> TaskManagedEBSVolumeConfigurationTypeDef:
    return {
        "encrypted": ...,
    }


# TaskManagedEBSVolumeConfigurationTypeDef definition

class TaskManagedEBSVolumeConfigurationTypeDef(TypedDict):
    roleArn: str,
    encrypted: NotRequired[bool],
    kmsKeyId: NotRequired[str],
    volumeType: NotRequired[str],
    sizeInGiB: NotRequired[int],
    snapshotId: NotRequired[str],
    iops: NotRequired[int],
    throughput: NotRequired[int],
    tagSpecifications: NotRequired[Sequence[EBSTagSpecificationUnionTypeDef]],  # (1)
    terminationPolicy: NotRequired[TaskManagedEBSVolumeTerminationPolicyTypeDef],  # (2)
    filesystemType: NotRequired[TaskFilesystemTypeType],  # (3)
```

1. See [:material-code-braces: EBSTagSpecificationTypeDef](./type_defs.md#ebstagspecificationtypedef) [:material-code-braces: EBSTagSpecificationOutputTypeDef](./type_defs.md#ebstagspecificationoutputtypedef) 
2. See [:material-code-braces: TaskManagedEBSVolumeTerminationPolicyTypeDef](./type_defs.md#taskmanagedebsvolumeterminationpolicytypedef) 
3. See [:material-code-brackets: TaskFilesystemTypeType](./literals.md#taskfilesystemtypetype) 
## TaskTypeDef

```python
# TaskTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TaskTypeDef


def get_value() -> TaskTypeDef:
    return {
        "attachments": ...,
    }


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
    overrides: NotRequired[TaskOverrideOutputTypeDef],  # (8)
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
    fargateEphemeralStorage: NotRequired[TaskEphemeralStorageTypeDef],  # (12)
```

1. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) 
2. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
3. See [:material-code-brackets: ConnectivityType](./literals.md#connectivitytype) 
4. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) 
5. See [:material-code-brackets: HealthStatusType](./literals.md#healthstatustype) 
6. See [:material-code-braces: InferenceAcceleratorTypeDef](./type_defs.md#inferenceacceleratortypedef) 
7. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
8. See [:material-code-braces: TaskOverrideOutputTypeDef](./type_defs.md#taskoverrideoutputtypedef) 
9. See [:material-code-brackets: TaskStopCodeType](./literals.md#taskstopcodetype) 
10. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
11. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
12. See [:material-code-braces: TaskEphemeralStorageTypeDef](./type_defs.md#taskephemeralstoragetypedef) 
## DeregisterContainerInstanceResponseTypeDef

```python
# DeregisterContainerInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeregisterContainerInstanceResponseTypeDef


def get_value() -> DeregisterContainerInstanceResponseTypeDef:
    return {
        "containerInstance": ...,
    }


# DeregisterContainerInstanceResponseTypeDef definition

class DeregisterContainerInstanceResponseTypeDef(TypedDict):
    containerInstance: ContainerInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerInstanceTypeDef](./type_defs.md#containerinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContainerInstancesResponseTypeDef

```python
# DescribeContainerInstancesResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeContainerInstancesResponseTypeDef


def get_value() -> DescribeContainerInstancesResponseTypeDef:
    return {
        "containerInstances": ...,
    }


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
# RegisterContainerInstanceResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import RegisterContainerInstanceResponseTypeDef


def get_value() -> RegisterContainerInstanceResponseTypeDef:
    return {
        "containerInstance": ...,
    }


# RegisterContainerInstanceResponseTypeDef definition

class RegisterContainerInstanceResponseTypeDef(TypedDict):
    containerInstance: ContainerInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerInstanceTypeDef](./type_defs.md#containerinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContainerAgentResponseTypeDef

```python
# UpdateContainerAgentResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateContainerAgentResponseTypeDef


def get_value() -> UpdateContainerAgentResponseTypeDef:
    return {
        "containerInstance": ...,
    }


# UpdateContainerAgentResponseTypeDef definition

class UpdateContainerAgentResponseTypeDef(TypedDict):
    containerInstance: ContainerInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerInstanceTypeDef](./type_defs.md#containerinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContainerInstancesStateResponseTypeDef

```python
# UpdateContainerInstancesStateResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateContainerInstancesStateResponseTypeDef


def get_value() -> UpdateContainerInstancesStateResponseTypeDef:
    return {
        "containerInstances": ...,
    }


# UpdateContainerInstancesStateResponseTypeDef definition

class UpdateContainerInstancesStateResponseTypeDef(TypedDict):
    containerInstances: List[ContainerInstanceTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ContainerInstanceTypeDef](./type_defs.md#containerinstancetypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeServiceDeploymentsResponseTypeDef

```python
# DescribeServiceDeploymentsResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeServiceDeploymentsResponseTypeDef


def get_value() -> DescribeServiceDeploymentsResponseTypeDef:
    return {
        "serviceDeployments": ...,
    }


# DescribeServiceDeploymentsResponseTypeDef definition

class DescribeServiceDeploymentsResponseTypeDef(TypedDict):
    serviceDeployments: List[ServiceDeploymentTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ServiceDeploymentTypeDef](./type_defs.md#servicedeploymenttypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterTypeDef

```python
# ClusterTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ClusterTypeDef


def get_value() -> ClusterTypeDef:
    return {
        "clusterArn": ...,
    }


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
## CreateClusterRequestTypeDef

```python
# CreateClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import CreateClusterRequestTypeDef


def get_value() -> CreateClusterRequestTypeDef:
    return {
        "clusterName": ...,
    }


# CreateClusterRequestTypeDef definition

class CreateClusterRequestTypeDef(TypedDict):
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
## UpdateClusterRequestTypeDef

```python
# UpdateClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateClusterRequestTypeDef


def get_value() -> UpdateClusterRequestTypeDef:
    return {
        "cluster": ...,
    }


# UpdateClusterRequestTypeDef definition

class UpdateClusterRequestTypeDef(TypedDict):
    cluster: str,
    settings: NotRequired[Sequence[ClusterSettingTypeDef]],  # (1)
    configuration: NotRequired[ClusterConfigurationTypeDef],  # (2)
    serviceConnectDefaults: NotRequired[ClusterServiceConnectDefaultsRequestTypeDef],  # (3)
```

1. See [:material-code-braces: ClusterSettingTypeDef](./type_defs.md#clustersettingtypedef) 
2. See [:material-code-braces: ClusterConfigurationTypeDef](./type_defs.md#clusterconfigurationtypedef) 
3. See [:material-code-braces: ClusterServiceConnectDefaultsRequestTypeDef](./type_defs.md#clusterserviceconnectdefaultsrequesttypedef) 
## TaskDefinitionTypeDef

```python
# TaskDefinitionTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TaskDefinitionTypeDef


def get_value() -> TaskDefinitionTypeDef:
    return {
        "taskDefinitionArn": ...,
    }


# TaskDefinitionTypeDef definition

class TaskDefinitionTypeDef(TypedDict):
    taskDefinitionArn: NotRequired[str],
    containerDefinitions: NotRequired[List[ContainerDefinitionOutputTypeDef]],  # (1)
    family: NotRequired[str],
    taskRoleArn: NotRequired[str],
    executionRoleArn: NotRequired[str],
    networkMode: NotRequired[NetworkModeType],  # (2)
    revision: NotRequired[int],
    volumes: NotRequired[List[VolumeOutputTypeDef]],  # (3)
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
    proxyConfiguration: NotRequired[ProxyConfigurationOutputTypeDef],  # (13)
    registeredAt: NotRequired[datetime],
    deregisteredAt: NotRequired[datetime],
    registeredBy: NotRequired[str],
    ephemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (14)
    enableFaultInjection: NotRequired[bool],
```

1. See [:material-code-braces: ContainerDefinitionOutputTypeDef](./type_defs.md#containerdefinitionoutputtypedef) 
2. See [:material-code-brackets: NetworkModeType](./literals.md#networkmodetype) 
3. See [:material-code-braces: VolumeOutputTypeDef](./type_defs.md#volumeoutputtypedef) 
4. See [:material-code-brackets: TaskDefinitionStatusType](./literals.md#taskdefinitionstatustype) 
5. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
6. See [:material-code-braces: TaskDefinitionPlacementConstraintTypeDef](./type_defs.md#taskdefinitionplacementconstrainttypedef) 
7. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
8. See [:material-code-braces: RuntimePlatformTypeDef](./type_defs.md#runtimeplatformtypedef) 
9. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
10. See [:material-code-braces: InferenceAcceleratorTypeDef](./type_defs.md#inferenceacceleratortypedef) 
11. See [:material-code-brackets: PidModeType](./literals.md#pidmodetype) 
12. See [:material-code-brackets: IpcModeType](./literals.md#ipcmodetype) 
13. See [:material-code-braces: ProxyConfigurationOutputTypeDef](./type_defs.md#proxyconfigurationoutputtypedef) 
14. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
## ServiceConnectConfigurationOutputTypeDef

```python
# ServiceConnectConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceConnectConfigurationOutputTypeDef


def get_value() -> ServiceConnectConfigurationOutputTypeDef:
    return {
        "enabled": ...,
    }


# ServiceConnectConfigurationOutputTypeDef definition

class ServiceConnectConfigurationOutputTypeDef(TypedDict):
    enabled: bool,
    namespace: NotRequired[str],
    services: NotRequired[List[ServiceConnectServiceOutputTypeDef]],  # (1)
    logConfiguration: NotRequired[LogConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ServiceConnectServiceOutputTypeDef](./type_defs.md#serviceconnectserviceoutputtypedef) 
2. See [:material-code-braces: LogConfigurationOutputTypeDef](./type_defs.md#logconfigurationoutputtypedef) 
## ServiceConnectConfigurationTypeDef

```python
# ServiceConnectConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceConnectConfigurationTypeDef


def get_value() -> ServiceConnectConfigurationTypeDef:
    return {
        "enabled": ...,
    }


# ServiceConnectConfigurationTypeDef definition

class ServiceConnectConfigurationTypeDef(TypedDict):
    enabled: bool,
    namespace: NotRequired[str],
    services: NotRequired[Sequence[ServiceConnectServiceTypeDef]],  # (1)
    logConfiguration: NotRequired[LogConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ServiceConnectServiceTypeDef](./type_defs.md#serviceconnectservicetypedef) 
2. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
## TaskVolumeConfigurationTypeDef

```python
# TaskVolumeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import TaskVolumeConfigurationTypeDef


def get_value() -> TaskVolumeConfigurationTypeDef:
    return {
        "name": ...,
    }


# TaskVolumeConfigurationTypeDef definition

class TaskVolumeConfigurationTypeDef(TypedDict):
    name: str,
    managedEBSVolume: NotRequired[TaskManagedEBSVolumeConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: TaskManagedEBSVolumeConfigurationTypeDef](./type_defs.md#taskmanagedebsvolumeconfigurationtypedef) 
## DescribeTasksResponseTypeDef

```python
# DescribeTasksResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeTasksResponseTypeDef


def get_value() -> DescribeTasksResponseTypeDef:
    return {
        "tasks": ...,
    }


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
# RunTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import RunTaskResponseTypeDef


def get_value() -> RunTaskResponseTypeDef:
    return {
        "tasks": ...,
    }


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
# StartTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import StartTaskResponseTypeDef


def get_value() -> StartTaskResponseTypeDef:
    return {
        "tasks": ...,
    }


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
# StopTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import StopTaskResponseTypeDef


def get_value() -> StopTaskResponseTypeDef:
    return {
        "task": ...,
    }


# StopTaskResponseTypeDef definition

class StopTaskResponseTypeDef(TypedDict):
    task: TaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterResponseTypeDef

```python
# CreateClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import CreateClusterResponseTypeDef


def get_value() -> CreateClusterResponseTypeDef:
    return {
        "cluster": ...,
    }


# CreateClusterResponseTypeDef definition

class CreateClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterResponseTypeDef

```python
# DeleteClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteClusterResponseTypeDef


def get_value() -> DeleteClusterResponseTypeDef:
    return {
        "cluster": ...,
    }


# DeleteClusterResponseTypeDef definition

class DeleteClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeClustersResponseTypeDef

```python
# DescribeClustersResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeClustersResponseTypeDef


def get_value() -> DescribeClustersResponseTypeDef:
    return {
        "clusters": ...,
    }


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
# PutClusterCapacityProvidersResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import PutClusterCapacityProvidersResponseTypeDef


def get_value() -> PutClusterCapacityProvidersResponseTypeDef:
    return {
        "cluster": ...,
    }


# PutClusterCapacityProvidersResponseTypeDef definition

class PutClusterCapacityProvidersResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterResponseTypeDef

```python
# UpdateClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateClusterResponseTypeDef


def get_value() -> UpdateClusterResponseTypeDef:
    return {
        "cluster": ...,
    }


# UpdateClusterResponseTypeDef definition

class UpdateClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterSettingsResponseTypeDef

```python
# UpdateClusterSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateClusterSettingsResponseTypeDef


def get_value() -> UpdateClusterSettingsResponseTypeDef:
    return {
        "cluster": ...,
    }


# UpdateClusterSettingsResponseTypeDef definition

class UpdateClusterSettingsResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTaskDefinitionsResponseTypeDef

```python
# DeleteTaskDefinitionsResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteTaskDefinitionsResponseTypeDef


def get_value() -> DeleteTaskDefinitionsResponseTypeDef:
    return {
        "taskDefinitions": ...,
    }


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
# DeregisterTaskDefinitionResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeregisterTaskDefinitionResponseTypeDef


def get_value() -> DeregisterTaskDefinitionResponseTypeDef:
    return {
        "taskDefinition": ...,
    }


# DeregisterTaskDefinitionResponseTypeDef definition

class DeregisterTaskDefinitionResponseTypeDef(TypedDict):
    taskDefinition: TaskDefinitionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskDefinitionTypeDef](./type_defs.md#taskdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTaskDefinitionResponseTypeDef

```python
# DescribeTaskDefinitionResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeTaskDefinitionResponseTypeDef


def get_value() -> DescribeTaskDefinitionResponseTypeDef:
    return {
        "taskDefinition": ...,
    }


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
# RegisterTaskDefinitionResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import RegisterTaskDefinitionResponseTypeDef


def get_value() -> RegisterTaskDefinitionResponseTypeDef:
    return {
        "taskDefinition": ...,
    }


# RegisterTaskDefinitionResponseTypeDef definition

class RegisterTaskDefinitionResponseTypeDef(TypedDict):
    taskDefinition: TaskDefinitionTypeDef,  # (1)
    tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TaskDefinitionTypeDef](./type_defs.md#taskdefinitiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentTypeDef

```python
# DeploymentTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeploymentTypeDef


def get_value() -> DeploymentTypeDef:
    return {
        "id": ...,
    }


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
    networkConfiguration: NotRequired[NetworkConfigurationOutputTypeDef],  # (3)
    rolloutState: NotRequired[DeploymentRolloutStateType],  # (4)
    rolloutStateReason: NotRequired[str],
    serviceConnectConfiguration: NotRequired[ServiceConnectConfigurationOutputTypeDef],  # (5)
    serviceConnectResources: NotRequired[List[ServiceConnectServiceResourceTypeDef]],  # (6)
    volumeConfigurations: NotRequired[List[ServiceVolumeConfigurationOutputTypeDef]],  # (7)
    fargateEphemeralStorage: NotRequired[DeploymentEphemeralStorageTypeDef],  # (8)
    vpcLatticeConfigurations: NotRequired[List[VpcLatticeConfigurationTypeDef]],  # (9)
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
3. See [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
4. See [:material-code-brackets: DeploymentRolloutStateType](./literals.md#deploymentrolloutstatetype) 
5. See [:material-code-braces: ServiceConnectConfigurationOutputTypeDef](./type_defs.md#serviceconnectconfigurationoutputtypedef) 
6. See [:material-code-braces: ServiceConnectServiceResourceTypeDef](./type_defs.md#serviceconnectserviceresourcetypedef) 
7. See [:material-code-braces: ServiceVolumeConfigurationOutputTypeDef](./type_defs.md#servicevolumeconfigurationoutputtypedef) 
8. See [:material-code-braces: DeploymentEphemeralStorageTypeDef](./type_defs.md#deploymentephemeralstoragetypedef) 
9. See [:material-code-braces: VpcLatticeConfigurationTypeDef](./type_defs.md#vpclatticeconfigurationtypedef) 
## ServiceRevisionTypeDef

```python
# ServiceRevisionTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceRevisionTypeDef


def get_value() -> ServiceRevisionTypeDef:
    return {
        "serviceRevisionArn": ...,
    }


# ServiceRevisionTypeDef definition

class ServiceRevisionTypeDef(TypedDict):
    serviceRevisionArn: NotRequired[str],
    serviceArn: NotRequired[str],
    clusterArn: NotRequired[str],
    taskDefinition: NotRequired[str],
    capacityProviderStrategy: NotRequired[List[CapacityProviderStrategyItemTypeDef]],  # (1)
    launchType: NotRequired[LaunchTypeType],  # (2)
    platformVersion: NotRequired[str],
    platformFamily: NotRequired[str],
    loadBalancers: NotRequired[List[LoadBalancerTypeDef]],  # (3)
    serviceRegistries: NotRequired[List[ServiceRegistryTypeDef]],  # (4)
    networkConfiguration: NotRequired[NetworkConfigurationOutputTypeDef],  # (5)
    containerImages: NotRequired[List[ContainerImageTypeDef]],  # (6)
    guardDutyEnabled: NotRequired[bool],
    serviceConnectConfiguration: NotRequired[ServiceConnectConfigurationOutputTypeDef],  # (7)
    volumeConfigurations: NotRequired[List[ServiceVolumeConfigurationOutputTypeDef]],  # (8)
    fargateEphemeralStorage: NotRequired[DeploymentEphemeralStorageTypeDef],  # (9)
    createdAt: NotRequired[datetime],
    vpcLatticeConfigurations: NotRequired[List[VpcLatticeConfigurationTypeDef]],  # (10)
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
3. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
4. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
5. See [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
6. See [:material-code-braces: ContainerImageTypeDef](./type_defs.md#containerimagetypedef) 
7. See [:material-code-braces: ServiceConnectConfigurationOutputTypeDef](./type_defs.md#serviceconnectconfigurationoutputtypedef) 
8. See [:material-code-braces: ServiceVolumeConfigurationOutputTypeDef](./type_defs.md#servicevolumeconfigurationoutputtypedef) 
9. See [:material-code-braces: DeploymentEphemeralStorageTypeDef](./type_defs.md#deploymentephemeralstoragetypedef) 
10. See [:material-code-braces: VpcLatticeConfigurationTypeDef](./type_defs.md#vpclatticeconfigurationtypedef) 
## ContainerDefinitionTypeDef

```python
# ContainerDefinitionTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ContainerDefinitionTypeDef


def get_value() -> ContainerDefinitionTypeDef:
    return {
        "name": ...,
    }


# ContainerDefinitionTypeDef definition

class ContainerDefinitionTypeDef(TypedDict):
    name: NotRequired[str],
    image: NotRequired[str],
    repositoryCredentials: NotRequired[RepositoryCredentialsTypeDef],  # (1)
    cpu: NotRequired[int],
    memory: NotRequired[int],
    memoryReservation: NotRequired[int],
    links: NotRequired[Sequence[str]],
    portMappings: NotRequired[Sequence[PortMappingTypeDef]],  # (2)
    essential: NotRequired[bool],
    restartPolicy: NotRequired[ContainerRestartPolicyUnionTypeDef],  # (3)
    entryPoint: NotRequired[Sequence[str]],
    command: NotRequired[Sequence[str]],
    environment: NotRequired[Sequence[KeyValuePairTypeDef]],  # (4)
    environmentFiles: NotRequired[Sequence[EnvironmentFileTypeDef]],  # (5)
    mountPoints: NotRequired[Sequence[MountPointTypeDef]],  # (6)
    volumesFrom: NotRequired[Sequence[VolumeFromTypeDef]],  # (7)
    linuxParameters: NotRequired[LinuxParametersUnionTypeDef],  # (8)
    secrets: NotRequired[Sequence[SecretTypeDef]],  # (9)
    dependsOn: NotRequired[Sequence[ContainerDependencyTypeDef]],  # (10)
    startTimeout: NotRequired[int],
    stopTimeout: NotRequired[int],
    versionConsistency: NotRequired[VersionConsistencyType],  # (11)
    hostname: NotRequired[str],
    user: NotRequired[str],
    workingDirectory: NotRequired[str],
    disableNetworking: NotRequired[bool],
    privileged: NotRequired[bool],
    readonlyRootFilesystem: NotRequired[bool],
    dnsServers: NotRequired[Sequence[str]],
    dnsSearchDomains: NotRequired[Sequence[str]],
    extraHosts: NotRequired[Sequence[HostEntryTypeDef]],  # (12)
    dockerSecurityOptions: NotRequired[Sequence[str]],
    interactive: NotRequired[bool],
    pseudoTerminal: NotRequired[bool],
    dockerLabels: NotRequired[Mapping[str, str]],
    ulimits: NotRequired[Sequence[UlimitTypeDef]],  # (13)
    logConfiguration: NotRequired[LogConfigurationUnionTypeDef],  # (14)
    healthCheck: NotRequired[HealthCheckUnionTypeDef],  # (15)
    systemControls: NotRequired[Sequence[SystemControlTypeDef]],  # (16)
    resourceRequirements: NotRequired[Sequence[ResourceRequirementTypeDef]],  # (17)
    firelensConfiguration: NotRequired[FirelensConfigurationUnionTypeDef],  # (18)
    credentialSpecs: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: RepositoryCredentialsTypeDef](./type_defs.md#repositorycredentialstypedef) 
2. See [:material-code-braces: PortMappingTypeDef](./type_defs.md#portmappingtypedef) 
3. See [:material-code-braces: ContainerRestartPolicyTypeDef](./type_defs.md#containerrestartpolicytypedef) [:material-code-braces: ContainerRestartPolicyOutputTypeDef](./type_defs.md#containerrestartpolicyoutputtypedef) 
4. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
5. See [:material-code-braces: EnvironmentFileTypeDef](./type_defs.md#environmentfiletypedef) 
6. See [:material-code-braces: MountPointTypeDef](./type_defs.md#mountpointtypedef) 
7. See [:material-code-braces: VolumeFromTypeDef](./type_defs.md#volumefromtypedef) 
8. See [:material-code-braces: LinuxParametersTypeDef](./type_defs.md#linuxparameterstypedef) [:material-code-braces: LinuxParametersOutputTypeDef](./type_defs.md#linuxparametersoutputtypedef) 
9. See [:material-code-braces: SecretTypeDef](./type_defs.md#secrettypedef) 
10. See [:material-code-braces: ContainerDependencyTypeDef](./type_defs.md#containerdependencytypedef) 
11. See [:material-code-brackets: VersionConsistencyType](./literals.md#versionconsistencytype) 
12. See [:material-code-braces: HostEntryTypeDef](./type_defs.md#hostentrytypedef) 
13. See [:material-code-braces: UlimitTypeDef](./type_defs.md#ulimittypedef) 
14. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) [:material-code-braces: LogConfigurationOutputTypeDef](./type_defs.md#logconfigurationoutputtypedef) 
15. See [:material-code-braces: HealthCheckTypeDef](./type_defs.md#healthchecktypedef) [:material-code-braces: HealthCheckOutputTypeDef](./type_defs.md#healthcheckoutputtypedef) 
16. See [:material-code-braces: SystemControlTypeDef](./type_defs.md#systemcontroltypedef) 
17. See [:material-code-braces: ResourceRequirementTypeDef](./type_defs.md#resourcerequirementtypedef) 
18. See [:material-code-braces: FirelensConfigurationTypeDef](./type_defs.md#firelensconfigurationtypedef) [:material-code-braces: FirelensConfigurationOutputTypeDef](./type_defs.md#firelensconfigurationoutputtypedef) 
## ServiceVolumeConfigurationTypeDef

```python
# ServiceVolumeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceVolumeConfigurationTypeDef


def get_value() -> ServiceVolumeConfigurationTypeDef:
    return {
        "name": ...,
    }


# ServiceVolumeConfigurationTypeDef definition

class ServiceVolumeConfigurationTypeDef(TypedDict):
    name: str,
    managedEBSVolume: NotRequired[ServiceManagedEBSVolumeConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ServiceManagedEBSVolumeConfigurationTypeDef](./type_defs.md#servicemanagedebsvolumeconfigurationtypedef) [:material-code-braces: ServiceManagedEBSVolumeConfigurationOutputTypeDef](./type_defs.md#servicemanagedebsvolumeconfigurationoutputtypedef) 
## RunTaskRequestTypeDef

```python
# RunTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import RunTaskRequestTypeDef


def get_value() -> RunTaskRequestTypeDef:
    return {
        "taskDefinition": ...,
    }


# RunTaskRequestTypeDef definition

class RunTaskRequestTypeDef(TypedDict):
    taskDefinition: str,
    capacityProviderStrategy: NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],  # (1)
    cluster: NotRequired[str],
    count: NotRequired[int],
    enableECSManagedTags: NotRequired[bool],
    enableExecuteCommand: NotRequired[bool],
    group: NotRequired[str],
    launchType: NotRequired[LaunchTypeType],  # (2)
    networkConfiguration: NotRequired[NetworkConfigurationUnionTypeDef],  # (3)
    overrides: NotRequired[TaskOverrideUnionTypeDef],  # (4)
    placementConstraints: NotRequired[Sequence[PlacementConstraintTypeDef]],  # (5)
    placementStrategy: NotRequired[Sequence[PlacementStrategyTypeDef]],  # (6)
    platformVersion: NotRequired[str],
    propagateTags: NotRequired[PropagateTagsType],  # (7)
    referenceId: NotRequired[str],
    startedBy: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (8)
    clientToken: NotRequired[str],
    volumeConfigurations: NotRequired[Sequence[TaskVolumeConfigurationTypeDef]],  # (9)
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
3. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
4. See [:material-code-braces: TaskOverrideTypeDef](./type_defs.md#taskoverridetypedef) [:material-code-braces: TaskOverrideOutputTypeDef](./type_defs.md#taskoverrideoutputtypedef) 
5. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
6. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
7. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: TaskVolumeConfigurationTypeDef](./type_defs.md#taskvolumeconfigurationtypedef) 
## StartTaskRequestTypeDef

```python
# StartTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import StartTaskRequestTypeDef


def get_value() -> StartTaskRequestTypeDef:
    return {
        "containerInstances": ...,
    }


# StartTaskRequestTypeDef definition

class StartTaskRequestTypeDef(TypedDict):
    containerInstances: Sequence[str],
    taskDefinition: str,
    cluster: NotRequired[str],
    enableECSManagedTags: NotRequired[bool],
    enableExecuteCommand: NotRequired[bool],
    group: NotRequired[str],
    networkConfiguration: NotRequired[NetworkConfigurationUnionTypeDef],  # (1)
    overrides: NotRequired[TaskOverrideUnionTypeDef],  # (2)
    propagateTags: NotRequired[PropagateTagsType],  # (3)
    referenceId: NotRequired[str],
    startedBy: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    volumeConfigurations: NotRequired[Sequence[TaskVolumeConfigurationTypeDef]],  # (5)
```

1. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
2. See [:material-code-braces: TaskOverrideTypeDef](./type_defs.md#taskoverridetypedef) [:material-code-braces: TaskOverrideOutputTypeDef](./type_defs.md#taskoverrideoutputtypedef) 
3. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: TaskVolumeConfigurationTypeDef](./type_defs.md#taskvolumeconfigurationtypedef) 
## ServiceTypeDef

```python
# ServiceTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import ServiceTypeDef


def get_value() -> ServiceTypeDef:
    return {
        "serviceArn": ...,
    }


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
    deploymentConfiguration: NotRequired[DeploymentConfigurationOutputTypeDef],  # (5)
    taskSets: NotRequired[List[TaskSetTypeDef]],  # (6)
    deployments: NotRequired[List[DeploymentTypeDef]],  # (7)
    roleArn: NotRequired[str],
    events: NotRequired[List[ServiceEventTypeDef]],  # (8)
    createdAt: NotRequired[datetime],
    placementConstraints: NotRequired[List[PlacementConstraintTypeDef]],  # (9)
    placementStrategy: NotRequired[List[PlacementStrategyTypeDef]],  # (10)
    networkConfiguration: NotRequired[NetworkConfigurationOutputTypeDef],  # (11)
    healthCheckGracePeriodSeconds: NotRequired[int],
    schedulingStrategy: NotRequired[SchedulingStrategyType],  # (12)
    deploymentController: NotRequired[DeploymentControllerTypeDef],  # (13)
    tags: NotRequired[List[TagTypeDef]],  # (14)
    createdBy: NotRequired[str],
    enableECSManagedTags: NotRequired[bool],
    propagateTags: NotRequired[PropagateTagsType],  # (15)
    enableExecuteCommand: NotRequired[bool],
    availabilityZoneRebalancing: NotRequired[AvailabilityZoneRebalancingType],  # (16)
```

1. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
2. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
3. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
4. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
5. See [:material-code-braces: DeploymentConfigurationOutputTypeDef](./type_defs.md#deploymentconfigurationoutputtypedef) 
6. See [:material-code-braces: TaskSetTypeDef](./type_defs.md#tasksettypedef) 
7. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
8. See [:material-code-braces: ServiceEventTypeDef](./type_defs.md#serviceeventtypedef) 
9. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
10. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
11. See [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
12. See [:material-code-brackets: SchedulingStrategyType](./literals.md#schedulingstrategytype) 
13. See [:material-code-braces: DeploymentControllerTypeDef](./type_defs.md#deploymentcontrollertypedef) 
14. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
15. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
16. See [:material-code-brackets: AvailabilityZoneRebalancingType](./literals.md#availabilityzonerebalancingtype) 
## DescribeServiceRevisionsResponseTypeDef

```python
# DescribeServiceRevisionsResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeServiceRevisionsResponseTypeDef


def get_value() -> DescribeServiceRevisionsResponseTypeDef:
    return {
        "serviceRevisions": ...,
    }


# DescribeServiceRevisionsResponseTypeDef definition

class DescribeServiceRevisionsResponseTypeDef(TypedDict):
    serviceRevisions: List[ServiceRevisionTypeDef],  # (1)
    failures: List[FailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ServiceRevisionTypeDef](./type_defs.md#servicerevisiontypedef) 
2. See [:material-code-braces: FailureTypeDef](./type_defs.md#failuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceResponseTypeDef

```python
# CreateServiceResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import CreateServiceResponseTypeDef


def get_value() -> CreateServiceResponseTypeDef:
    return {
        "service": ...,
    }


# CreateServiceResponseTypeDef definition

class CreateServiceResponseTypeDef(TypedDict):
    service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceResponseTypeDef

```python
# DeleteServiceResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DeleteServiceResponseTypeDef


def get_value() -> DeleteServiceResponseTypeDef:
    return {
        "service": ...,
    }


# DeleteServiceResponseTypeDef definition

class DeleteServiceResponseTypeDef(TypedDict):
    service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeServicesResponseTypeDef

```python
# DescribeServicesResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import DescribeServicesResponseTypeDef


def get_value() -> DescribeServicesResponseTypeDef:
    return {
        "services": ...,
    }


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
# UpdateServiceResponseTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateServiceResponseTypeDef


def get_value() -> UpdateServiceResponseTypeDef:
    return {
        "service": ...,
    }


# UpdateServiceResponseTypeDef definition

class UpdateServiceResponseTypeDef(TypedDict):
    service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterTaskDefinitionRequestTypeDef

```python
# RegisterTaskDefinitionRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import RegisterTaskDefinitionRequestTypeDef


def get_value() -> RegisterTaskDefinitionRequestTypeDef:
    return {
        "family": ...,
    }


# RegisterTaskDefinitionRequestTypeDef definition

class RegisterTaskDefinitionRequestTypeDef(TypedDict):
    family: str,
    containerDefinitions: Sequence[ContainerDefinitionUnionTypeDef],  # (1)
    taskRoleArn: NotRequired[str],
    executionRoleArn: NotRequired[str],
    networkMode: NotRequired[NetworkModeType],  # (2)
    volumes: NotRequired[Sequence[VolumeUnionTypeDef]],  # (3)
    placementConstraints: NotRequired[Sequence[TaskDefinitionPlacementConstraintTypeDef]],  # (4)
    requiresCompatibilities: NotRequired[Sequence[CompatibilityType]],  # (5)
    cpu: NotRequired[str],
    memory: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (6)
    pidMode: NotRequired[PidModeType],  # (7)
    ipcMode: NotRequired[IpcModeType],  # (8)
    proxyConfiguration: NotRequired[ProxyConfigurationUnionTypeDef],  # (9)
    inferenceAccelerators: NotRequired[Sequence[InferenceAcceleratorTypeDef]],  # (10)
    ephemeralStorage: NotRequired[EphemeralStorageTypeDef],  # (11)
    runtimePlatform: NotRequired[RuntimePlatformTypeDef],  # (12)
    enableFaultInjection: NotRequired[bool],
```

1. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) [:material-code-braces: ContainerDefinitionOutputTypeDef](./type_defs.md#containerdefinitionoutputtypedef) 
2. See [:material-code-brackets: NetworkModeType](./literals.md#networkmodetype) 
3. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) [:material-code-braces: VolumeOutputTypeDef](./type_defs.md#volumeoutputtypedef) 
4. See [:material-code-braces: TaskDefinitionPlacementConstraintTypeDef](./type_defs.md#taskdefinitionplacementconstrainttypedef) 
5. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-brackets: PidModeType](./literals.md#pidmodetype) 
8. See [:material-code-brackets: IpcModeType](./literals.md#ipcmodetype) 
9. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) [:material-code-braces: ProxyConfigurationOutputTypeDef](./type_defs.md#proxyconfigurationoutputtypedef) 
10. See [:material-code-braces: InferenceAcceleratorTypeDef](./type_defs.md#inferenceacceleratortypedef) 
11. See [:material-code-braces: EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef) 
12. See [:material-code-braces: RuntimePlatformTypeDef](./type_defs.md#runtimeplatformtypedef) 
## CreateServiceRequestTypeDef

```python
# CreateServiceRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import CreateServiceRequestTypeDef


def get_value() -> CreateServiceRequestTypeDef:
    return {
        "serviceName": ...,
    }


# CreateServiceRequestTypeDef definition

class CreateServiceRequestTypeDef(TypedDict):
    serviceName: str,
    cluster: NotRequired[str],
    taskDefinition: NotRequired[str],
    availabilityZoneRebalancing: NotRequired[AvailabilityZoneRebalancingType],  # (1)
    loadBalancers: NotRequired[Sequence[LoadBalancerTypeDef]],  # (2)
    serviceRegistries: NotRequired[Sequence[ServiceRegistryTypeDef]],  # (3)
    desiredCount: NotRequired[int],
    clientToken: NotRequired[str],
    launchType: NotRequired[LaunchTypeType],  # (4)
    capacityProviderStrategy: NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],  # (5)
    platformVersion: NotRequired[str],
    role: NotRequired[str],
    deploymentConfiguration: NotRequired[DeploymentConfigurationUnionTypeDef],  # (6)
    placementConstraints: NotRequired[Sequence[PlacementConstraintTypeDef]],  # (7)
    placementStrategy: NotRequired[Sequence[PlacementStrategyTypeDef]],  # (8)
    networkConfiguration: NotRequired[NetworkConfigurationUnionTypeDef],  # (9)
    healthCheckGracePeriodSeconds: NotRequired[int],
    schedulingStrategy: NotRequired[SchedulingStrategyType],  # (10)
    deploymentController: NotRequired[DeploymentControllerTypeDef],  # (11)
    tags: NotRequired[Sequence[TagTypeDef]],  # (12)
    enableECSManagedTags: NotRequired[bool],
    propagateTags: NotRequired[PropagateTagsType],  # (13)
    enableExecuteCommand: NotRequired[bool],
    serviceConnectConfiguration: NotRequired[ServiceConnectConfigurationUnionTypeDef],  # (14)
    volumeConfigurations: NotRequired[Sequence[ServiceVolumeConfigurationUnionTypeDef]],  # (15)
    vpcLatticeConfigurations: NotRequired[Sequence[VpcLatticeConfigurationTypeDef]],  # (16)
```

1. See [:material-code-brackets: AvailabilityZoneRebalancingType](./literals.md#availabilityzonerebalancingtype) 
2. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
3. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
4. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
5. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
6. See [:material-code-braces: DeploymentConfigurationTypeDef](./type_defs.md#deploymentconfigurationtypedef) [:material-code-braces: DeploymentConfigurationOutputTypeDef](./type_defs.md#deploymentconfigurationoutputtypedef) 
7. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
8. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
9. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
10. See [:material-code-brackets: SchedulingStrategyType](./literals.md#schedulingstrategytype) 
11. See [:material-code-braces: DeploymentControllerTypeDef](./type_defs.md#deploymentcontrollertypedef) 
12. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
13. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
14. See [:material-code-braces: ServiceConnectConfigurationTypeDef](./type_defs.md#serviceconnectconfigurationtypedef) [:material-code-braces: ServiceConnectConfigurationOutputTypeDef](./type_defs.md#serviceconnectconfigurationoutputtypedef) 
15. See [:material-code-braces: ServiceVolumeConfigurationTypeDef](./type_defs.md#servicevolumeconfigurationtypedef) [:material-code-braces: ServiceVolumeConfigurationOutputTypeDef](./type_defs.md#servicevolumeconfigurationoutputtypedef) 
16. See [:material-code-braces: VpcLatticeConfigurationTypeDef](./type_defs.md#vpclatticeconfigurationtypedef) 
## UpdateServiceRequestTypeDef

```python
# UpdateServiceRequestTypeDef TypedDict usage example

from types_aiobotocore_ecs.type_defs import UpdateServiceRequestTypeDef


def get_value() -> UpdateServiceRequestTypeDef:
    return {
        "service": ...,
    }


# UpdateServiceRequestTypeDef definition

class UpdateServiceRequestTypeDef(TypedDict):
    service: str,
    cluster: NotRequired[str],
    desiredCount: NotRequired[int],
    taskDefinition: NotRequired[str],
    capacityProviderStrategy: NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],  # (1)
    deploymentConfiguration: NotRequired[DeploymentConfigurationUnionTypeDef],  # (2)
    availabilityZoneRebalancing: NotRequired[AvailabilityZoneRebalancingType],  # (3)
    networkConfiguration: NotRequired[NetworkConfigurationUnionTypeDef],  # (4)
    placementConstraints: NotRequired[Sequence[PlacementConstraintTypeDef]],  # (5)
    placementStrategy: NotRequired[Sequence[PlacementStrategyTypeDef]],  # (6)
    platformVersion: NotRequired[str],
    forceNewDeployment: NotRequired[bool],
    healthCheckGracePeriodSeconds: NotRequired[int],
    enableExecuteCommand: NotRequired[bool],
    enableECSManagedTags: NotRequired[bool],
    loadBalancers: NotRequired[Sequence[LoadBalancerTypeDef]],  # (7)
    propagateTags: NotRequired[PropagateTagsType],  # (8)
    serviceRegistries: NotRequired[Sequence[ServiceRegistryTypeDef]],  # (9)
    serviceConnectConfiguration: NotRequired[ServiceConnectConfigurationUnionTypeDef],  # (10)
    volumeConfigurations: NotRequired[Sequence[ServiceVolumeConfigurationUnionTypeDef]],  # (11)
    vpcLatticeConfigurations: NotRequired[Sequence[VpcLatticeConfigurationTypeDef]],  # (12)
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-braces: DeploymentConfigurationTypeDef](./type_defs.md#deploymentconfigurationtypedef) [:material-code-braces: DeploymentConfigurationOutputTypeDef](./type_defs.md#deploymentconfigurationoutputtypedef) 
3. See [:material-code-brackets: AvailabilityZoneRebalancingType](./literals.md#availabilityzonerebalancingtype) 
4. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
5. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
6. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
7. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
8. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
9. See [:material-code-braces: ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef) 
10. See [:material-code-braces: ServiceConnectConfigurationTypeDef](./type_defs.md#serviceconnectconfigurationtypedef) [:material-code-braces: ServiceConnectConfigurationOutputTypeDef](./type_defs.md#serviceconnectconfigurationoutputtypedef) 
11. See [:material-code-braces: ServiceVolumeConfigurationTypeDef](./type_defs.md#servicevolumeconfigurationtypedef) [:material-code-braces: ServiceVolumeConfigurationOutputTypeDef](./type_defs.md#servicevolumeconfigurationoutputtypedef) 
12. See [:material-code-braces: VpcLatticeConfigurationTypeDef](./type_defs.md#vpclatticeconfigurationtypedef) 
