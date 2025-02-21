# Type definitions

> [Index](../README.md) > [OpsWorks](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#opsworks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

## AutoScalingThresholdsUnionTypeDef

```python
# AutoScalingThresholdsUnionTypeDef Union usage example

from types_aiobotocore_opsworks.type_defs import AutoScalingThresholdsUnionTypeDef


def get_value() -> AutoScalingThresholdsUnionTypeDef:
    return ...


# AutoScalingThresholdsUnionTypeDef definition

AutoScalingThresholdsUnionTypeDef = Union[
    AutoScalingThresholdsTypeDef,  # (1)
    AutoScalingThresholdsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AutoScalingThresholdsTypeDef](./type_defs.md#autoscalingthresholdstypedef) 
2. See [:material-code-braces: AutoScalingThresholdsOutputTypeDef](./type_defs.md#autoscalingthresholdsoutputtypedef) 

## DeploymentCommandUnionTypeDef

```python
# DeploymentCommandUnionTypeDef Union usage example

from types_aiobotocore_opsworks.type_defs import DeploymentCommandUnionTypeDef


def get_value() -> DeploymentCommandUnionTypeDef:
    return ...


# DeploymentCommandUnionTypeDef definition

DeploymentCommandUnionTypeDef = Union[
    DeploymentCommandTypeDef,  # (1)
    DeploymentCommandOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeploymentCommandTypeDef](./type_defs.md#deploymentcommandtypedef) 
2. See [:material-code-braces: DeploymentCommandOutputTypeDef](./type_defs.md#deploymentcommandoutputtypedef) 

## RecipesUnionTypeDef

```python
# RecipesUnionTypeDef Union usage example

from types_aiobotocore_opsworks.type_defs import RecipesUnionTypeDef


def get_value() -> RecipesUnionTypeDef:
    return ...


# RecipesUnionTypeDef definition

RecipesUnionTypeDef = Union[
    RecipesTypeDef,  # (1)
    RecipesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RecipesTypeDef](./type_defs.md#recipestypedef) 
2. See [:material-code-braces: RecipesOutputTypeDef](./type_defs.md#recipesoutputtypedef) 

## WeeklyAutoScalingScheduleUnionTypeDef

```python
# WeeklyAutoScalingScheduleUnionTypeDef Union usage example

from types_aiobotocore_opsworks.type_defs import WeeklyAutoScalingScheduleUnionTypeDef


def get_value() -> WeeklyAutoScalingScheduleUnionTypeDef:
    return ...


# WeeklyAutoScalingScheduleUnionTypeDef definition

WeeklyAutoScalingScheduleUnionTypeDef = Union[
    WeeklyAutoScalingScheduleTypeDef,  # (1)
    WeeklyAutoScalingScheduleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WeeklyAutoScalingScheduleTypeDef](./type_defs.md#weeklyautoscalingscheduletypedef) 
2. See [:material-code-braces: WeeklyAutoScalingScheduleOutputTypeDef](./type_defs.md#weeklyautoscalingscheduleoutputtypedef) 

## CloudWatchLogsConfigurationUnionTypeDef

```python
# CloudWatchLogsConfigurationUnionTypeDef Union usage example

from types_aiobotocore_opsworks.type_defs import CloudWatchLogsConfigurationUnionTypeDef


def get_value() -> CloudWatchLogsConfigurationUnionTypeDef:
    return ...


# CloudWatchLogsConfigurationUnionTypeDef definition

CloudWatchLogsConfigurationUnionTypeDef = Union[
    CloudWatchLogsConfigurationTypeDef,  # (1)
    CloudWatchLogsConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef) 
2. See [:material-code-braces: CloudWatchLogsConfigurationOutputTypeDef](./type_defs.md#cloudwatchlogsconfigurationoutputtypedef) 



## StackConfigurationManagerTypeDef

```python
# StackConfigurationManagerTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import StackConfigurationManagerTypeDef


def get_value() -> StackConfigurationManagerTypeDef:
    return {
        "Name": ...,
    }


# StackConfigurationManagerTypeDef definition

class StackConfigurationManagerTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## DataSourceTypeDef

```python
# DataSourceTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DataSourceTypeDef


def get_value() -> DataSourceTypeDef:
    return {
        "Type": ...,
    }


# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    Type: NotRequired[str],
    Arn: NotRequired[str],
    DatabaseName: NotRequired[str],
```

## EnvironmentVariableTypeDef

```python
# EnvironmentVariableTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import EnvironmentVariableTypeDef


def get_value() -> EnvironmentVariableTypeDef:
    return {
        "Key": ...,
    }


# EnvironmentVariableTypeDef definition

class EnvironmentVariableTypeDef(TypedDict):
    Key: str,
    Value: str,
    Secure: NotRequired[bool],
```

## SourceTypeDef

```python
# SourceTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import SourceTypeDef


def get_value() -> SourceTypeDef:
    return {
        "Type": ...,
    }


# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    Type: NotRequired[SourceTypeType],  # (1)
    Url: NotRequired[str],
    Username: NotRequired[str],
    Password: NotRequired[str],
    SshKey: NotRequired[str],
    Revision: NotRequired[str],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## SslConfigurationTypeDef

```python
# SslConfigurationTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import SslConfigurationTypeDef


def get_value() -> SslConfigurationTypeDef:
    return {
        "Certificate": ...,
    }


# SslConfigurationTypeDef definition

class SslConfigurationTypeDef(TypedDict):
    Certificate: str,
    PrivateKey: str,
    Chain: NotRequired[str],
```

## AssignInstanceRequestTypeDef

```python
# AssignInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import AssignInstanceRequestTypeDef


def get_value() -> AssignInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# AssignInstanceRequestTypeDef definition

class AssignInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
    LayerIds: Sequence[str],
```

## AssignVolumeRequestTypeDef

```python
# AssignVolumeRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import AssignVolumeRequestTypeDef


def get_value() -> AssignVolumeRequestTypeDef:
    return {
        "VolumeId": ...,
    }


# AssignVolumeRequestTypeDef definition

class AssignVolumeRequestTypeDef(TypedDict):
    VolumeId: str,
    InstanceId: NotRequired[str],
```

## AssociateElasticIpRequestTypeDef

```python
# AssociateElasticIpRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import AssociateElasticIpRequestTypeDef


def get_value() -> AssociateElasticIpRequestTypeDef:
    return {
        "ElasticIp": ...,
    }


# AssociateElasticIpRequestTypeDef definition

class AssociateElasticIpRequestTypeDef(TypedDict):
    ElasticIp: str,
    InstanceId: NotRequired[str],
```

## AttachElasticLoadBalancerRequestTypeDef

```python
# AttachElasticLoadBalancerRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import AttachElasticLoadBalancerRequestTypeDef


def get_value() -> AttachElasticLoadBalancerRequestTypeDef:
    return {
        "ElasticLoadBalancerName": ...,
    }


# AttachElasticLoadBalancerRequestTypeDef definition

class AttachElasticLoadBalancerRequestTypeDef(TypedDict):
    ElasticLoadBalancerName: str,
    LayerId: str,
```

## AutoScalingThresholdsOutputTypeDef

```python
# AutoScalingThresholdsOutputTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import AutoScalingThresholdsOutputTypeDef


def get_value() -> AutoScalingThresholdsOutputTypeDef:
    return {
        "InstanceCount": ...,
    }


# AutoScalingThresholdsOutputTypeDef definition

class AutoScalingThresholdsOutputTypeDef(TypedDict):
    InstanceCount: NotRequired[int],
    ThresholdsWaitTime: NotRequired[int],
    IgnoreMetricsTime: NotRequired[int],
    CpuThreshold: NotRequired[float],
    MemoryThreshold: NotRequired[float],
    LoadThreshold: NotRequired[float],
    Alarms: NotRequired[List[str]],
```

## AutoScalingThresholdsTypeDef

```python
# AutoScalingThresholdsTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import AutoScalingThresholdsTypeDef


def get_value() -> AutoScalingThresholdsTypeDef:
    return {
        "InstanceCount": ...,
    }


# AutoScalingThresholdsTypeDef definition

class AutoScalingThresholdsTypeDef(TypedDict):
    InstanceCount: NotRequired[int],
    ThresholdsWaitTime: NotRequired[int],
    IgnoreMetricsTime: NotRequired[int],
    CpuThreshold: NotRequired[float],
    MemoryThreshold: NotRequired[float],
    LoadThreshold: NotRequired[float],
    Alarms: NotRequired[Sequence[str]],
```

## EbsBlockDeviceTypeDef

```python
# EbsBlockDeviceTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import EbsBlockDeviceTypeDef


def get_value() -> EbsBlockDeviceTypeDef:
    return {
        "SnapshotId": ...,
    }


# EbsBlockDeviceTypeDef definition

class EbsBlockDeviceTypeDef(TypedDict):
    SnapshotId: NotRequired[str],
    Iops: NotRequired[int],
    VolumeSize: NotRequired[int],
    VolumeType: NotRequired[VolumeTypeType],  # (1)
    DeleteOnTermination: NotRequired[bool],
```

1. See [:material-code-brackets: VolumeTypeType](./literals.md#volumetypetype) 
## ChefConfigurationTypeDef

```python
# ChefConfigurationTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import ChefConfigurationTypeDef


def get_value() -> ChefConfigurationTypeDef:
    return {
        "ManageBerkshelf": ...,
    }


# ChefConfigurationTypeDef definition

class ChefConfigurationTypeDef(TypedDict):
    ManageBerkshelf: NotRequired[bool],
    BerkshelfVersion: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import ResponseMetadataTypeDef


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

## CloudWatchLogsLogStreamTypeDef

```python
# CloudWatchLogsLogStreamTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CloudWatchLogsLogStreamTypeDef


def get_value() -> CloudWatchLogsLogStreamTypeDef:
    return {
        "LogGroupName": ...,
    }


# CloudWatchLogsLogStreamTypeDef definition

class CloudWatchLogsLogStreamTypeDef(TypedDict):
    LogGroupName: NotRequired[str],
    DatetimeFormat: NotRequired[str],
    TimeZone: NotRequired[CloudWatchLogsTimeZoneType],  # (1)
    File: NotRequired[str],
    FileFingerprintLines: NotRequired[str],
    MultiLineStartPattern: NotRequired[str],
    InitialPosition: NotRequired[CloudWatchLogsInitialPositionType],  # (2)
    Encoding: NotRequired[CloudWatchLogsEncodingType],  # (3)
    BufferDuration: NotRequired[int],
    BatchCount: NotRequired[int],
    BatchSize: NotRequired[int],
```

1. See [:material-code-brackets: CloudWatchLogsTimeZoneType](./literals.md#cloudwatchlogstimezonetype) 
2. See [:material-code-brackets: CloudWatchLogsInitialPositionType](./literals.md#cloudwatchlogsinitialpositiontype) 
3. See [:material-code-brackets: CloudWatchLogsEncodingType](./literals.md#cloudwatchlogsencodingtype) 
## CommandTypeDef

```python
# CommandTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CommandTypeDef


def get_value() -> CommandTypeDef:
    return {
        "CommandId": ...,
    }


# CommandTypeDef definition

class CommandTypeDef(TypedDict):
    CommandId: NotRequired[str],
    InstanceId: NotRequired[str],
    DeploymentId: NotRequired[str],
    CreatedAt: NotRequired[str],
    AcknowledgedAt: NotRequired[str],
    CompletedAt: NotRequired[str],
    Status: NotRequired[str],
    ExitCode: NotRequired[int],
    LogUrl: NotRequired[str],
    Type: NotRequired[str],
```

## VolumeConfigurationTypeDef

```python
# VolumeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import VolumeConfigurationTypeDef


def get_value() -> VolumeConfigurationTypeDef:
    return {
        "MountPoint": ...,
    }


# VolumeConfigurationTypeDef definition

class VolumeConfigurationTypeDef(TypedDict):
    MountPoint: str,
    NumberOfDisks: int,
    Size: int,
    RaidLevel: NotRequired[int],
    VolumeType: NotRequired[str],
    Iops: NotRequired[int],
    Encrypted: NotRequired[bool],
```

## CreateUserProfileRequestTypeDef

```python
# CreateUserProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateUserProfileRequestTypeDef


def get_value() -> CreateUserProfileRequestTypeDef:
    return {
        "IamUserArn": ...,
    }


# CreateUserProfileRequestTypeDef definition

class CreateUserProfileRequestTypeDef(TypedDict):
    IamUserArn: str,
    SshUsername: NotRequired[str],
    SshPublicKey: NotRequired[str],
    AllowSelfManagement: NotRequired[bool],
```

## DeleteAppRequestTypeDef

```python
# DeleteAppRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeleteAppRequestTypeDef


def get_value() -> DeleteAppRequestTypeDef:
    return {
        "AppId": ...,
    }


# DeleteAppRequestTypeDef definition

class DeleteAppRequestTypeDef(TypedDict):
    AppId: str,
```

## DeleteInstanceRequestTypeDef

```python
# DeleteInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeleteInstanceRequestTypeDef


def get_value() -> DeleteInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeleteInstanceRequestTypeDef definition

class DeleteInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
    DeleteElasticIp: NotRequired[bool],
    DeleteVolumes: NotRequired[bool],
```

## DeleteLayerRequestTypeDef

```python
# DeleteLayerRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeleteLayerRequestTypeDef


def get_value() -> DeleteLayerRequestTypeDef:
    return {
        "LayerId": ...,
    }


# DeleteLayerRequestTypeDef definition

class DeleteLayerRequestTypeDef(TypedDict):
    LayerId: str,
```

## DeleteStackRequestTypeDef

```python
# DeleteStackRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeleteStackRequestTypeDef


def get_value() -> DeleteStackRequestTypeDef:
    return {
        "StackId": ...,
    }


# DeleteStackRequestTypeDef definition

class DeleteStackRequestTypeDef(TypedDict):
    StackId: str,
```

## DeleteUserProfileRequestTypeDef

```python
# DeleteUserProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeleteUserProfileRequestTypeDef


def get_value() -> DeleteUserProfileRequestTypeDef:
    return {
        "IamUserArn": ...,
    }


# DeleteUserProfileRequestTypeDef definition

class DeleteUserProfileRequestTypeDef(TypedDict):
    IamUserArn: str,
```

## DeploymentCommandOutputTypeDef

```python
# DeploymentCommandOutputTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeploymentCommandOutputTypeDef


def get_value() -> DeploymentCommandOutputTypeDef:
    return {
        "Name": ...,
    }


# DeploymentCommandOutputTypeDef definition

class DeploymentCommandOutputTypeDef(TypedDict):
    Name: DeploymentCommandNameType,  # (1)
    Args: NotRequired[Dict[str, List[str]]],
```

1. See [:material-code-brackets: DeploymentCommandNameType](./literals.md#deploymentcommandnametype) 
## DeploymentCommandTypeDef

```python
# DeploymentCommandTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeploymentCommandTypeDef


def get_value() -> DeploymentCommandTypeDef:
    return {
        "Name": ...,
    }


# DeploymentCommandTypeDef definition

class DeploymentCommandTypeDef(TypedDict):
    Name: DeploymentCommandNameType,  # (1)
    Args: NotRequired[Mapping[str, Sequence[str]]],
```

1. See [:material-code-brackets: DeploymentCommandNameType](./literals.md#deploymentcommandnametype) 
## DeregisterEcsClusterRequestTypeDef

```python
# DeregisterEcsClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeregisterEcsClusterRequestTypeDef


def get_value() -> DeregisterEcsClusterRequestTypeDef:
    return {
        "EcsClusterArn": ...,
    }


# DeregisterEcsClusterRequestTypeDef definition

class DeregisterEcsClusterRequestTypeDef(TypedDict):
    EcsClusterArn: str,
```

## DeregisterElasticIpRequestTypeDef

```python
# DeregisterElasticIpRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeregisterElasticIpRequestTypeDef


def get_value() -> DeregisterElasticIpRequestTypeDef:
    return {
        "ElasticIp": ...,
    }


# DeregisterElasticIpRequestTypeDef definition

class DeregisterElasticIpRequestTypeDef(TypedDict):
    ElasticIp: str,
```

## DeregisterInstanceRequestTypeDef

```python
# DeregisterInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeregisterInstanceRequestTypeDef


def get_value() -> DeregisterInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DeregisterInstanceRequestTypeDef definition

class DeregisterInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
```

## DeregisterRdsDbInstanceRequestTypeDef

```python
# DeregisterRdsDbInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeregisterRdsDbInstanceRequestTypeDef


def get_value() -> DeregisterRdsDbInstanceRequestTypeDef:
    return {
        "RdsDbInstanceArn": ...,
    }


# DeregisterRdsDbInstanceRequestTypeDef definition

class DeregisterRdsDbInstanceRequestTypeDef(TypedDict):
    RdsDbInstanceArn: str,
```

## DeregisterVolumeRequestTypeDef

```python
# DeregisterVolumeRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeregisterVolumeRequestTypeDef


def get_value() -> DeregisterVolumeRequestTypeDef:
    return {
        "VolumeId": ...,
    }


# DeregisterVolumeRequestTypeDef definition

class DeregisterVolumeRequestTypeDef(TypedDict):
    VolumeId: str,
```

## DescribeAppsRequestTypeDef

```python
# DescribeAppsRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeAppsRequestTypeDef


def get_value() -> DescribeAppsRequestTypeDef:
    return {
        "StackId": ...,
    }


# DescribeAppsRequestTypeDef definition

class DescribeAppsRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    AppIds: NotRequired[Sequence[str]],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeCommandsRequestTypeDef

```python
# DescribeCommandsRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeCommandsRequestTypeDef


def get_value() -> DescribeCommandsRequestTypeDef:
    return {
        "DeploymentId": ...,
    }


# DescribeCommandsRequestTypeDef definition

class DescribeCommandsRequestTypeDef(TypedDict):
    DeploymentId: NotRequired[str],
    InstanceId: NotRequired[str],
    CommandIds: NotRequired[Sequence[str]],
```

## DescribeDeploymentsRequestTypeDef

```python
# DescribeDeploymentsRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeDeploymentsRequestTypeDef


def get_value() -> DescribeDeploymentsRequestTypeDef:
    return {
        "StackId": ...,
    }


# DescribeDeploymentsRequestTypeDef definition

class DescribeDeploymentsRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    AppId: NotRequired[str],
    DeploymentIds: NotRequired[Sequence[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import PaginatorConfigTypeDef


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

## DescribeEcsClustersRequestTypeDef

```python
# DescribeEcsClustersRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeEcsClustersRequestTypeDef


def get_value() -> DescribeEcsClustersRequestTypeDef:
    return {
        "EcsClusterArns": ...,
    }


# DescribeEcsClustersRequestTypeDef definition

class DescribeEcsClustersRequestTypeDef(TypedDict):
    EcsClusterArns: NotRequired[Sequence[str]],
    StackId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## EcsClusterTypeDef

```python
# EcsClusterTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import EcsClusterTypeDef


def get_value() -> EcsClusterTypeDef:
    return {
        "EcsClusterArn": ...,
    }


# EcsClusterTypeDef definition

class EcsClusterTypeDef(TypedDict):
    EcsClusterArn: NotRequired[str],
    EcsClusterName: NotRequired[str],
    StackId: NotRequired[str],
    RegisteredAt: NotRequired[str],
```

## DescribeElasticIpsRequestTypeDef

```python
# DescribeElasticIpsRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeElasticIpsRequestTypeDef


def get_value() -> DescribeElasticIpsRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeElasticIpsRequestTypeDef definition

class DescribeElasticIpsRequestTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    StackId: NotRequired[str],
    Ips: NotRequired[Sequence[str]],
```

## ElasticIpTypeDef

```python
# ElasticIpTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import ElasticIpTypeDef


def get_value() -> ElasticIpTypeDef:
    return {
        "Ip": ...,
    }


# ElasticIpTypeDef definition

class ElasticIpTypeDef(TypedDict):
    Ip: NotRequired[str],
    Name: NotRequired[str],
    Domain: NotRequired[str],
    Region: NotRequired[str],
    InstanceId: NotRequired[str],
```

## DescribeElasticLoadBalancersRequestTypeDef

```python
# DescribeElasticLoadBalancersRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeElasticLoadBalancersRequestTypeDef


def get_value() -> DescribeElasticLoadBalancersRequestTypeDef:
    return {
        "StackId": ...,
    }


# DescribeElasticLoadBalancersRequestTypeDef definition

class DescribeElasticLoadBalancersRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerIds: NotRequired[Sequence[str]],
```

## ElasticLoadBalancerTypeDef

```python
# ElasticLoadBalancerTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import ElasticLoadBalancerTypeDef


def get_value() -> ElasticLoadBalancerTypeDef:
    return {
        "ElasticLoadBalancerName": ...,
    }


# ElasticLoadBalancerTypeDef definition

class ElasticLoadBalancerTypeDef(TypedDict):
    ElasticLoadBalancerName: NotRequired[str],
    Region: NotRequired[str],
    DnsName: NotRequired[str],
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    VpcId: NotRequired[str],
    AvailabilityZones: NotRequired[List[str]],
    SubnetIds: NotRequired[List[str]],
    Ec2InstanceIds: NotRequired[List[str]],
```

## DescribeInstancesRequestTypeDef

```python
# DescribeInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeInstancesRequestTypeDef


def get_value() -> DescribeInstancesRequestTypeDef:
    return {
        "StackId": ...,
    }


# DescribeInstancesRequestTypeDef definition

class DescribeInstancesRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
```

## DescribeLayersRequestTypeDef

```python
# DescribeLayersRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeLayersRequestTypeDef


def get_value() -> DescribeLayersRequestTypeDef:
    return {
        "StackId": ...,
    }


# DescribeLayersRequestTypeDef definition

class DescribeLayersRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerIds: NotRequired[Sequence[str]],
```

## DescribeLoadBasedAutoScalingRequestTypeDef

```python
# DescribeLoadBasedAutoScalingRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeLoadBasedAutoScalingRequestTypeDef


def get_value() -> DescribeLoadBasedAutoScalingRequestTypeDef:
    return {
        "LayerIds": ...,
    }


# DescribeLoadBasedAutoScalingRequestTypeDef definition

class DescribeLoadBasedAutoScalingRequestTypeDef(TypedDict):
    LayerIds: Sequence[str],
```

## SelfUserProfileTypeDef

```python
# SelfUserProfileTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import SelfUserProfileTypeDef


def get_value() -> SelfUserProfileTypeDef:
    return {
        "IamUserArn": ...,
    }


# SelfUserProfileTypeDef definition

class SelfUserProfileTypeDef(TypedDict):
    IamUserArn: NotRequired[str],
    Name: NotRequired[str],
    SshUsername: NotRequired[str],
    SshPublicKey: NotRequired[str],
```

## DescribePermissionsRequestTypeDef

```python
# DescribePermissionsRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribePermissionsRequestTypeDef


def get_value() -> DescribePermissionsRequestTypeDef:
    return {
        "IamUserArn": ...,
    }


# DescribePermissionsRequestTypeDef definition

class DescribePermissionsRequestTypeDef(TypedDict):
    IamUserArn: NotRequired[str],
    StackId: NotRequired[str],
```

## PermissionTypeDef

```python
# PermissionTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import PermissionTypeDef


def get_value() -> PermissionTypeDef:
    return {
        "StackId": ...,
    }


# PermissionTypeDef definition

class PermissionTypeDef(TypedDict):
    StackId: NotRequired[str],
    IamUserArn: NotRequired[str],
    AllowSsh: NotRequired[bool],
    AllowSudo: NotRequired[bool],
    Level: NotRequired[str],
```

## DescribeRaidArraysRequestTypeDef

```python
# DescribeRaidArraysRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeRaidArraysRequestTypeDef


def get_value() -> DescribeRaidArraysRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeRaidArraysRequestTypeDef definition

class DescribeRaidArraysRequestTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    StackId: NotRequired[str],
    RaidArrayIds: NotRequired[Sequence[str]],
```

## RaidArrayTypeDef

```python
# RaidArrayTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RaidArrayTypeDef


def get_value() -> RaidArrayTypeDef:
    return {
        "RaidArrayId": ...,
    }


# RaidArrayTypeDef definition

class RaidArrayTypeDef(TypedDict):
    RaidArrayId: NotRequired[str],
    InstanceId: NotRequired[str],
    Name: NotRequired[str],
    RaidLevel: NotRequired[int],
    NumberOfDisks: NotRequired[int],
    Size: NotRequired[int],
    Device: NotRequired[str],
    MountPoint: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    CreatedAt: NotRequired[str],
    StackId: NotRequired[str],
    VolumeType: NotRequired[str],
    Iops: NotRequired[int],
```

## DescribeRdsDbInstancesRequestTypeDef

```python
# DescribeRdsDbInstancesRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeRdsDbInstancesRequestTypeDef


def get_value() -> DescribeRdsDbInstancesRequestTypeDef:
    return {
        "StackId": ...,
    }


# DescribeRdsDbInstancesRequestTypeDef definition

class DescribeRdsDbInstancesRequestTypeDef(TypedDict):
    StackId: str,
    RdsDbInstanceArns: NotRequired[Sequence[str]],
```

## RdsDbInstanceTypeDef

```python
# RdsDbInstanceTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RdsDbInstanceTypeDef


def get_value() -> RdsDbInstanceTypeDef:
    return {
        "RdsDbInstanceArn": ...,
    }


# RdsDbInstanceTypeDef definition

class RdsDbInstanceTypeDef(TypedDict):
    RdsDbInstanceArn: NotRequired[str],
    DbInstanceIdentifier: NotRequired[str],
    DbUser: NotRequired[str],
    DbPassword: NotRequired[str],
    Region: NotRequired[str],
    Address: NotRequired[str],
    Engine: NotRequired[str],
    StackId: NotRequired[str],
    MissingOnRds: NotRequired[bool],
```

## DescribeServiceErrorsRequestTypeDef

```python
# DescribeServiceErrorsRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeServiceErrorsRequestTypeDef


def get_value() -> DescribeServiceErrorsRequestTypeDef:
    return {
        "StackId": ...,
    }


# DescribeServiceErrorsRequestTypeDef definition

class DescribeServiceErrorsRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    InstanceId: NotRequired[str],
    ServiceErrorIds: NotRequired[Sequence[str]],
```

## ServiceErrorTypeDef

```python
# ServiceErrorTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import ServiceErrorTypeDef


def get_value() -> ServiceErrorTypeDef:
    return {
        "ServiceErrorId": ...,
    }


# ServiceErrorTypeDef definition

class ServiceErrorTypeDef(TypedDict):
    ServiceErrorId: NotRequired[str],
    StackId: NotRequired[str],
    InstanceId: NotRequired[str],
    Type: NotRequired[str],
    Message: NotRequired[str],
    CreatedAt: NotRequired[str],
```

## DescribeStackProvisioningParametersRequestTypeDef

```python
# DescribeStackProvisioningParametersRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeStackProvisioningParametersRequestTypeDef


def get_value() -> DescribeStackProvisioningParametersRequestTypeDef:
    return {
        "StackId": ...,
    }


# DescribeStackProvisioningParametersRequestTypeDef definition

class DescribeStackProvisioningParametersRequestTypeDef(TypedDict):
    StackId: str,
```

## DescribeStackSummaryRequestTypeDef

```python
# DescribeStackSummaryRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeStackSummaryRequestTypeDef


def get_value() -> DescribeStackSummaryRequestTypeDef:
    return {
        "StackId": ...,
    }


# DescribeStackSummaryRequestTypeDef definition

class DescribeStackSummaryRequestTypeDef(TypedDict):
    StackId: str,
```

## DescribeStacksRequestTypeDef

```python
# DescribeStacksRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeStacksRequestTypeDef


def get_value() -> DescribeStacksRequestTypeDef:
    return {
        "StackIds": ...,
    }


# DescribeStacksRequestTypeDef definition

class DescribeStacksRequestTypeDef(TypedDict):
    StackIds: NotRequired[Sequence[str]],
```

## DescribeTimeBasedAutoScalingRequestTypeDef

```python
# DescribeTimeBasedAutoScalingRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeTimeBasedAutoScalingRequestTypeDef


def get_value() -> DescribeTimeBasedAutoScalingRequestTypeDef:
    return {
        "InstanceIds": ...,
    }


# DescribeTimeBasedAutoScalingRequestTypeDef definition

class DescribeTimeBasedAutoScalingRequestTypeDef(TypedDict):
    InstanceIds: Sequence[str],
```

## DescribeUserProfilesRequestTypeDef

```python
# DescribeUserProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeUserProfilesRequestTypeDef


def get_value() -> DescribeUserProfilesRequestTypeDef:
    return {
        "IamUserArns": ...,
    }


# DescribeUserProfilesRequestTypeDef definition

class DescribeUserProfilesRequestTypeDef(TypedDict):
    IamUserArns: NotRequired[Sequence[str]],
```

## UserProfileTypeDef

```python
# UserProfileTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UserProfileTypeDef


def get_value() -> UserProfileTypeDef:
    return {
        "IamUserArn": ...,
    }


# UserProfileTypeDef definition

class UserProfileTypeDef(TypedDict):
    IamUserArn: NotRequired[str],
    Name: NotRequired[str],
    SshUsername: NotRequired[str],
    SshPublicKey: NotRequired[str],
    AllowSelfManagement: NotRequired[bool],
```

## DescribeVolumesRequestTypeDef

```python
# DescribeVolumesRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeVolumesRequestTypeDef


def get_value() -> DescribeVolumesRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# DescribeVolumesRequestTypeDef definition

class DescribeVolumesRequestTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    StackId: NotRequired[str],
    RaidArrayId: NotRequired[str],
    VolumeIds: NotRequired[Sequence[str]],
```

## VolumeTypeDef

```python
# VolumeTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import VolumeTypeDef


def get_value() -> VolumeTypeDef:
    return {
        "VolumeId": ...,
    }


# VolumeTypeDef definition

class VolumeTypeDef(TypedDict):
    VolumeId: NotRequired[str],
    Ec2VolumeId: NotRequired[str],
    Name: NotRequired[str],
    RaidArrayId: NotRequired[str],
    InstanceId: NotRequired[str],
    Status: NotRequired[str],
    Size: NotRequired[int],
    Device: NotRequired[str],
    MountPoint: NotRequired[str],
    Region: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    VolumeType: NotRequired[str],
    Iops: NotRequired[int],
    Encrypted: NotRequired[bool],
```

## DetachElasticLoadBalancerRequestTypeDef

```python
# DetachElasticLoadBalancerRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DetachElasticLoadBalancerRequestTypeDef


def get_value() -> DetachElasticLoadBalancerRequestTypeDef:
    return {
        "ElasticLoadBalancerName": ...,
    }


# DetachElasticLoadBalancerRequestTypeDef definition

class DetachElasticLoadBalancerRequestTypeDef(TypedDict):
    ElasticLoadBalancerName: str,
    LayerId: str,
```

## DisassociateElasticIpRequestTypeDef

```python
# DisassociateElasticIpRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DisassociateElasticIpRequestTypeDef


def get_value() -> DisassociateElasticIpRequestTypeDef:
    return {
        "ElasticIp": ...,
    }


# DisassociateElasticIpRequestTypeDef definition

class DisassociateElasticIpRequestTypeDef(TypedDict):
    ElasticIp: str,
```

## GetHostnameSuggestionRequestTypeDef

```python
# GetHostnameSuggestionRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import GetHostnameSuggestionRequestTypeDef


def get_value() -> GetHostnameSuggestionRequestTypeDef:
    return {
        "LayerId": ...,
    }


# GetHostnameSuggestionRequestTypeDef definition

class GetHostnameSuggestionRequestTypeDef(TypedDict):
    LayerId: str,
```

## GrantAccessRequestTypeDef

```python
# GrantAccessRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import GrantAccessRequestTypeDef


def get_value() -> GrantAccessRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# GrantAccessRequestTypeDef definition

class GrantAccessRequestTypeDef(TypedDict):
    InstanceId: str,
    ValidForInMinutes: NotRequired[int],
```

## TemporaryCredentialTypeDef

```python
# TemporaryCredentialTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import TemporaryCredentialTypeDef


def get_value() -> TemporaryCredentialTypeDef:
    return {
        "Username": ...,
    }


# TemporaryCredentialTypeDef definition

class TemporaryCredentialTypeDef(TypedDict):
    Username: NotRequired[str],
    Password: NotRequired[str],
    ValidForInMinutes: NotRequired[int],
    InstanceId: NotRequired[str],
```

## InstanceIdentityTypeDef

```python
# InstanceIdentityTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import InstanceIdentityTypeDef


def get_value() -> InstanceIdentityTypeDef:
    return {
        "Document": ...,
    }


# InstanceIdentityTypeDef definition

class InstanceIdentityTypeDef(TypedDict):
    Document: NotRequired[str],
    Signature: NotRequired[str],
```

## ReportedOsTypeDef

```python
# ReportedOsTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import ReportedOsTypeDef


def get_value() -> ReportedOsTypeDef:
    return {
        "Family": ...,
    }


# ReportedOsTypeDef definition

class ReportedOsTypeDef(TypedDict):
    Family: NotRequired[str],
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## InstancesCountTypeDef

```python
# InstancesCountTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import InstancesCountTypeDef


def get_value() -> InstancesCountTypeDef:
    return {
        "Assigning": ...,
    }


# InstancesCountTypeDef definition

class InstancesCountTypeDef(TypedDict):
    Assigning: NotRequired[int],
    Booting: NotRequired[int],
    ConnectionLost: NotRequired[int],
    Deregistering: NotRequired[int],
    Online: NotRequired[int],
    Pending: NotRequired[int],
    Rebooting: NotRequired[int],
    Registered: NotRequired[int],
    Registering: NotRequired[int],
    Requested: NotRequired[int],
    RunningSetup: NotRequired[int],
    SetupFailed: NotRequired[int],
    ShuttingDown: NotRequired[int],
    StartFailed: NotRequired[int],
    StopFailed: NotRequired[int],
    Stopped: NotRequired[int],
    Stopping: NotRequired[int],
    Terminated: NotRequired[int],
    Terminating: NotRequired[int],
    Unassigning: NotRequired[int],
```

## RecipesOutputTypeDef

```python
# RecipesOutputTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RecipesOutputTypeDef


def get_value() -> RecipesOutputTypeDef:
    return {
        "Setup": ...,
    }


# RecipesOutputTypeDef definition

class RecipesOutputTypeDef(TypedDict):
    Setup: NotRequired[List[str]],
    Configure: NotRequired[List[str]],
    Deploy: NotRequired[List[str]],
    Undeploy: NotRequired[List[str]],
    Shutdown: NotRequired[List[str]],
```

## ShutdownEventConfigurationTypeDef

```python
# ShutdownEventConfigurationTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import ShutdownEventConfigurationTypeDef


def get_value() -> ShutdownEventConfigurationTypeDef:
    return {
        "ExecutionTimeout": ...,
    }


# ShutdownEventConfigurationTypeDef definition

class ShutdownEventConfigurationTypeDef(TypedDict):
    ExecutionTimeout: NotRequired[int],
    DelayUntilElbConnectionsDrained: NotRequired[bool],
```

## ListTagsRequestTypeDef

```python
# ListTagsRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import ListTagsRequestTypeDef


def get_value() -> ListTagsRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsRequestTypeDef definition

class ListTagsRequestTypeDef(TypedDict):
    ResourceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## OperatingSystemConfigurationManagerTypeDef

```python
# OperatingSystemConfigurationManagerTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import OperatingSystemConfigurationManagerTypeDef


def get_value() -> OperatingSystemConfigurationManagerTypeDef:
    return {
        "Name": ...,
    }


# OperatingSystemConfigurationManagerTypeDef definition

class OperatingSystemConfigurationManagerTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## RebootInstanceRequestTypeDef

```python
# RebootInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RebootInstanceRequestTypeDef


def get_value() -> RebootInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# RebootInstanceRequestTypeDef definition

class RebootInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
```

## RecipesTypeDef

```python
# RecipesTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RecipesTypeDef


def get_value() -> RecipesTypeDef:
    return {
        "Setup": ...,
    }


# RecipesTypeDef definition

class RecipesTypeDef(TypedDict):
    Setup: NotRequired[Sequence[str]],
    Configure: NotRequired[Sequence[str]],
    Deploy: NotRequired[Sequence[str]],
    Undeploy: NotRequired[Sequence[str]],
    Shutdown: NotRequired[Sequence[str]],
```

## RegisterEcsClusterRequestTypeDef

```python
# RegisterEcsClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RegisterEcsClusterRequestTypeDef


def get_value() -> RegisterEcsClusterRequestTypeDef:
    return {
        "EcsClusterArn": ...,
    }


# RegisterEcsClusterRequestTypeDef definition

class RegisterEcsClusterRequestTypeDef(TypedDict):
    EcsClusterArn: str,
    StackId: str,
```

## RegisterElasticIpRequestTypeDef

```python
# RegisterElasticIpRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RegisterElasticIpRequestTypeDef


def get_value() -> RegisterElasticIpRequestTypeDef:
    return {
        "ElasticIp": ...,
    }


# RegisterElasticIpRequestTypeDef definition

class RegisterElasticIpRequestTypeDef(TypedDict):
    ElasticIp: str,
    StackId: str,
```

## RegisterRdsDbInstanceRequestTypeDef

```python
# RegisterRdsDbInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RegisterRdsDbInstanceRequestTypeDef


def get_value() -> RegisterRdsDbInstanceRequestTypeDef:
    return {
        "StackId": ...,
    }


# RegisterRdsDbInstanceRequestTypeDef definition

class RegisterRdsDbInstanceRequestTypeDef(TypedDict):
    StackId: str,
    RdsDbInstanceArn: str,
    DbUser: str,
    DbPassword: str,
```

## RegisterVolumeRequestTypeDef

```python
# RegisterVolumeRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RegisterVolumeRequestTypeDef


def get_value() -> RegisterVolumeRequestTypeDef:
    return {
        "StackId": ...,
    }


# RegisterVolumeRequestTypeDef definition

class RegisterVolumeRequestTypeDef(TypedDict):
    StackId: str,
    Ec2VolumeId: NotRequired[str],
```

## SetPermissionRequestTypeDef

```python
# SetPermissionRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import SetPermissionRequestTypeDef


def get_value() -> SetPermissionRequestTypeDef:
    return {
        "StackId": ...,
    }


# SetPermissionRequestTypeDef definition

class SetPermissionRequestTypeDef(TypedDict):
    StackId: str,
    IamUserArn: str,
    AllowSsh: NotRequired[bool],
    AllowSudo: NotRequired[bool],
    Level: NotRequired[str],
```

## StartInstanceRequestTypeDef

```python
# StartInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import StartInstanceRequestTypeDef


def get_value() -> StartInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StartInstanceRequestTypeDef definition

class StartInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
```

## StartStackRequestTypeDef

```python
# StartStackRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import StartStackRequestTypeDef


def get_value() -> StartStackRequestTypeDef:
    return {
        "StackId": ...,
    }


# StartStackRequestTypeDef definition

class StartStackRequestTypeDef(TypedDict):
    StackId: str,
```

## StopInstanceRequestTypeDef

```python
# StopInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import StopInstanceRequestTypeDef


def get_value() -> StopInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# StopInstanceRequestTypeDef definition

class StopInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
    Force: NotRequired[bool],
```

## StopStackRequestTypeDef

```python
# StopStackRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import StopStackRequestTypeDef


def get_value() -> StopStackRequestTypeDef:
    return {
        "StackId": ...,
    }


# StopStackRequestTypeDef definition

class StopStackRequestTypeDef(TypedDict):
    StackId: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## WeeklyAutoScalingScheduleOutputTypeDef

```python
# WeeklyAutoScalingScheduleOutputTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import WeeklyAutoScalingScheduleOutputTypeDef


def get_value() -> WeeklyAutoScalingScheduleOutputTypeDef:
    return {
        "Monday": ...,
    }


# WeeklyAutoScalingScheduleOutputTypeDef definition

class WeeklyAutoScalingScheduleOutputTypeDef(TypedDict):
    Monday: NotRequired[Dict[str, str]],
    Tuesday: NotRequired[Dict[str, str]],
    Wednesday: NotRequired[Dict[str, str]],
    Thursday: NotRequired[Dict[str, str]],
    Friday: NotRequired[Dict[str, str]],
    Saturday: NotRequired[Dict[str, str]],
    Sunday: NotRequired[Dict[str, str]],
```

## UnassignInstanceRequestTypeDef

```python
# UnassignInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UnassignInstanceRequestTypeDef


def get_value() -> UnassignInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UnassignInstanceRequestTypeDef definition

class UnassignInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
```

## UnassignVolumeRequestTypeDef

```python
# UnassignVolumeRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UnassignVolumeRequestTypeDef


def get_value() -> UnassignVolumeRequestTypeDef:
    return {
        "VolumeId": ...,
    }


# UnassignVolumeRequestTypeDef definition

class UnassignVolumeRequestTypeDef(TypedDict):
    VolumeId: str,
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateElasticIpRequestTypeDef

```python
# UpdateElasticIpRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UpdateElasticIpRequestTypeDef


def get_value() -> UpdateElasticIpRequestTypeDef:
    return {
        "ElasticIp": ...,
    }


# UpdateElasticIpRequestTypeDef definition

class UpdateElasticIpRequestTypeDef(TypedDict):
    ElasticIp: str,
    Name: NotRequired[str],
```

## UpdateInstanceRequestTypeDef

```python
# UpdateInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UpdateInstanceRequestTypeDef


def get_value() -> UpdateInstanceRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# UpdateInstanceRequestTypeDef definition

class UpdateInstanceRequestTypeDef(TypedDict):
    InstanceId: str,
    LayerIds: NotRequired[Sequence[str]],
    InstanceType: NotRequired[str],
    AutoScalingType: NotRequired[AutoScalingTypeType],  # (1)
    Hostname: NotRequired[str],
    Os: NotRequired[str],
    AmiId: NotRequired[str],
    SshKeyName: NotRequired[str],
    Architecture: NotRequired[ArchitectureType],  # (2)
    InstallUpdatesOnBoot: NotRequired[bool],
    EbsOptimized: NotRequired[bool],
    AgentVersion: NotRequired[str],
```

1. See [:material-code-brackets: AutoScalingTypeType](./literals.md#autoscalingtypetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## UpdateMyUserProfileRequestTypeDef

```python
# UpdateMyUserProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UpdateMyUserProfileRequestTypeDef


def get_value() -> UpdateMyUserProfileRequestTypeDef:
    return {
        "SshPublicKey": ...,
    }


# UpdateMyUserProfileRequestTypeDef definition

class UpdateMyUserProfileRequestTypeDef(TypedDict):
    SshPublicKey: NotRequired[str],
```

## UpdateRdsDbInstanceRequestTypeDef

```python
# UpdateRdsDbInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UpdateRdsDbInstanceRequestTypeDef


def get_value() -> UpdateRdsDbInstanceRequestTypeDef:
    return {
        "RdsDbInstanceArn": ...,
    }


# UpdateRdsDbInstanceRequestTypeDef definition

class UpdateRdsDbInstanceRequestTypeDef(TypedDict):
    RdsDbInstanceArn: str,
    DbUser: NotRequired[str],
    DbPassword: NotRequired[str],
```

## UpdateUserProfileRequestTypeDef

```python
# UpdateUserProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UpdateUserProfileRequestTypeDef


def get_value() -> UpdateUserProfileRequestTypeDef:
    return {
        "IamUserArn": ...,
    }


# UpdateUserProfileRequestTypeDef definition

class UpdateUserProfileRequestTypeDef(TypedDict):
    IamUserArn: str,
    SshUsername: NotRequired[str],
    SshPublicKey: NotRequired[str],
    AllowSelfManagement: NotRequired[bool],
```

## UpdateVolumeRequestTypeDef

```python
# UpdateVolumeRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UpdateVolumeRequestTypeDef


def get_value() -> UpdateVolumeRequestTypeDef:
    return {
        "VolumeId": ...,
    }


# UpdateVolumeRequestTypeDef definition

class UpdateVolumeRequestTypeDef(TypedDict):
    VolumeId: str,
    Name: NotRequired[str],
    MountPoint: NotRequired[str],
```

## WeeklyAutoScalingScheduleTypeDef

```python
# WeeklyAutoScalingScheduleTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import WeeklyAutoScalingScheduleTypeDef


def get_value() -> WeeklyAutoScalingScheduleTypeDef:
    return {
        "Monday": ...,
    }


# WeeklyAutoScalingScheduleTypeDef definition

class WeeklyAutoScalingScheduleTypeDef(TypedDict):
    Monday: NotRequired[Mapping[str, str]],
    Tuesday: NotRequired[Mapping[str, str]],
    Wednesday: NotRequired[Mapping[str, str]],
    Thursday: NotRequired[Mapping[str, str]],
    Friday: NotRequired[Mapping[str, str]],
    Saturday: NotRequired[Mapping[str, str]],
    Sunday: NotRequired[Mapping[str, str]],
```

## AgentVersionTypeDef

```python
# AgentVersionTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import AgentVersionTypeDef


def get_value() -> AgentVersionTypeDef:
    return {
        "Version": ...,
    }


# AgentVersionTypeDef definition

class AgentVersionTypeDef(TypedDict):
    Version: NotRequired[str],
    ConfigurationManager: NotRequired[StackConfigurationManagerTypeDef],  # (1)
```

1. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
## DescribeAgentVersionsRequestTypeDef

```python
# DescribeAgentVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeAgentVersionsRequestTypeDef


def get_value() -> DescribeAgentVersionsRequestTypeDef:
    return {
        "StackId": ...,
    }


# DescribeAgentVersionsRequestTypeDef definition

class DescribeAgentVersionsRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    ConfigurationManager: NotRequired[StackConfigurationManagerTypeDef],  # (1)
```

1. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
## AppTypeDef

```python
# AppTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import AppTypeDef


def get_value() -> AppTypeDef:
    return {
        "AppId": ...,
    }


# AppTypeDef definition

class AppTypeDef(TypedDict):
    AppId: NotRequired[str],
    StackId: NotRequired[str],
    Shortname: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    DataSources: NotRequired[List[DataSourceTypeDef]],  # (1)
    Type: NotRequired[AppTypeType],  # (2)
    AppSource: NotRequired[SourceTypeDef],  # (3)
    Domains: NotRequired[List[str]],
    EnableSsl: NotRequired[bool],
    SslConfiguration: NotRequired[SslConfigurationTypeDef],  # (4)
    Attributes: NotRequired[Dict[AppAttributesKeysType, str]],  # (5)
    CreatedAt: NotRequired[str],
    Environment: NotRequired[List[EnvironmentVariableTypeDef]],  # (6)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
3. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
4. See [:material-code-braces: SslConfigurationTypeDef](./type_defs.md#sslconfigurationtypedef) 
5. See [:material-code-brackets: AppAttributesKeysType](./literals.md#appattributeskeystype) 
6. See [:material-code-braces: EnvironmentVariableTypeDef](./type_defs.md#environmentvariabletypedef) 
## CreateAppRequestTypeDef

```python
# CreateAppRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateAppRequestTypeDef


def get_value() -> CreateAppRequestTypeDef:
    return {
        "StackId": ...,
    }


# CreateAppRequestTypeDef definition

class CreateAppRequestTypeDef(TypedDict):
    StackId: str,
    Name: str,
    Type: AppTypeType,  # (1)
    Shortname: NotRequired[str],
    Description: NotRequired[str],
    DataSources: NotRequired[Sequence[DataSourceTypeDef]],  # (2)
    AppSource: NotRequired[SourceTypeDef],  # (3)
    Domains: NotRequired[Sequence[str]],
    EnableSsl: NotRequired[bool],
    SslConfiguration: NotRequired[SslConfigurationTypeDef],  # (4)
    Attributes: NotRequired[Mapping[AppAttributesKeysType, str]],  # (5)
    Environment: NotRequired[Sequence[EnvironmentVariableTypeDef]],  # (6)
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
2. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
3. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
4. See [:material-code-braces: SslConfigurationTypeDef](./type_defs.md#sslconfigurationtypedef) 
5. See [:material-code-brackets: AppAttributesKeysType](./literals.md#appattributeskeystype) 
6. See [:material-code-braces: EnvironmentVariableTypeDef](./type_defs.md#environmentvariabletypedef) 
## UpdateAppRequestTypeDef

```python
# UpdateAppRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UpdateAppRequestTypeDef


def get_value() -> UpdateAppRequestTypeDef:
    return {
        "AppId": ...,
    }


# UpdateAppRequestTypeDef definition

class UpdateAppRequestTypeDef(TypedDict):
    AppId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    DataSources: NotRequired[Sequence[DataSourceTypeDef]],  # (1)
    Type: NotRequired[AppTypeType],  # (2)
    AppSource: NotRequired[SourceTypeDef],  # (3)
    Domains: NotRequired[Sequence[str]],
    EnableSsl: NotRequired[bool],
    SslConfiguration: NotRequired[SslConfigurationTypeDef],  # (4)
    Attributes: NotRequired[Mapping[AppAttributesKeysType, str]],  # (5)
    Environment: NotRequired[Sequence[EnvironmentVariableTypeDef]],  # (6)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
3. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
4. See [:material-code-braces: SslConfigurationTypeDef](./type_defs.md#sslconfigurationtypedef) 
5. See [:material-code-brackets: AppAttributesKeysType](./literals.md#appattributeskeystype) 
6. See [:material-code-braces: EnvironmentVariableTypeDef](./type_defs.md#environmentvariabletypedef) 
## LoadBasedAutoScalingConfigurationTypeDef

```python
# LoadBasedAutoScalingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import LoadBasedAutoScalingConfigurationTypeDef


def get_value() -> LoadBasedAutoScalingConfigurationTypeDef:
    return {
        "LayerId": ...,
    }


# LoadBasedAutoScalingConfigurationTypeDef definition

class LoadBasedAutoScalingConfigurationTypeDef(TypedDict):
    LayerId: NotRequired[str],
    Enable: NotRequired[bool],
    UpScaling: NotRequired[AutoScalingThresholdsOutputTypeDef],  # (1)
    DownScaling: NotRequired[AutoScalingThresholdsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingThresholdsOutputTypeDef](./type_defs.md#autoscalingthresholdsoutputtypedef) 
2. See [:material-code-braces: AutoScalingThresholdsOutputTypeDef](./type_defs.md#autoscalingthresholdsoutputtypedef) 
## BlockDeviceMappingTypeDef

```python
# BlockDeviceMappingTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import BlockDeviceMappingTypeDef


def get_value() -> BlockDeviceMappingTypeDef:
    return {
        "DeviceName": ...,
    }


# BlockDeviceMappingTypeDef definition

class BlockDeviceMappingTypeDef(TypedDict):
    DeviceName: NotRequired[str],
    NoDevice: NotRequired[str],
    VirtualName: NotRequired[str],
    Ebs: NotRequired[EbsBlockDeviceTypeDef],  # (1)
```

1. See [:material-code-braces: EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef) 
## CloneStackRequestTypeDef

```python
# CloneStackRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CloneStackRequestTypeDef


def get_value() -> CloneStackRequestTypeDef:
    return {
        "SourceStackId": ...,
    }


# CloneStackRequestTypeDef definition

class CloneStackRequestTypeDef(TypedDict):
    SourceStackId: str,
    ServiceRoleArn: str,
    Name: NotRequired[str],
    Region: NotRequired[str],
    VpcId: NotRequired[str],
    Attributes: NotRequired[Mapping[StackAttributesKeysType, str]],  # (1)
    DefaultInstanceProfileArn: NotRequired[str],
    DefaultOs: NotRequired[str],
    HostnameTheme: NotRequired[str],
    DefaultAvailabilityZone: NotRequired[str],
    DefaultSubnetId: NotRequired[str],
    CustomJson: NotRequired[str],
    ConfigurationManager: NotRequired[StackConfigurationManagerTypeDef],  # (2)
    ChefConfiguration: NotRequired[ChefConfigurationTypeDef],  # (3)
    UseCustomCookbooks: NotRequired[bool],
    UseOpsworksSecurityGroups: NotRequired[bool],
    CustomCookbooksSource: NotRequired[SourceTypeDef],  # (4)
    DefaultSshKeyName: NotRequired[str],
    ClonePermissions: NotRequired[bool],
    CloneAppIds: NotRequired[Sequence[str]],
    DefaultRootDeviceType: NotRequired[RootDeviceTypeType],  # (5)
    AgentVersion: NotRequired[str],
```

1. See [:material-code-brackets: StackAttributesKeysType](./literals.md#stackattributeskeystype) 
2. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
3. See [:material-code-braces: ChefConfigurationTypeDef](./type_defs.md#chefconfigurationtypedef) 
4. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
5. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 
## CreateStackRequestServiceResourceCreateStackTypeDef

```python
# CreateStackRequestServiceResourceCreateStackTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateStackRequestServiceResourceCreateStackTypeDef


def get_value() -> CreateStackRequestServiceResourceCreateStackTypeDef:
    return {
        "Name": ...,
    }


# CreateStackRequestServiceResourceCreateStackTypeDef definition

class CreateStackRequestServiceResourceCreateStackTypeDef(TypedDict):
    Name: str,
    Region: str,
    ServiceRoleArn: str,
    DefaultInstanceProfileArn: str,
    VpcId: NotRequired[str],
    Attributes: NotRequired[Mapping[StackAttributesKeysType, str]],  # (1)
    DefaultOs: NotRequired[str],
    HostnameTheme: NotRequired[str],
    DefaultAvailabilityZone: NotRequired[str],
    DefaultSubnetId: NotRequired[str],
    CustomJson: NotRequired[str],
    ConfigurationManager: NotRequired[StackConfigurationManagerTypeDef],  # (2)
    ChefConfiguration: NotRequired[ChefConfigurationTypeDef],  # (3)
    UseCustomCookbooks: NotRequired[bool],
    UseOpsworksSecurityGroups: NotRequired[bool],
    CustomCookbooksSource: NotRequired[SourceTypeDef],  # (4)
    DefaultSshKeyName: NotRequired[str],
    DefaultRootDeviceType: NotRequired[RootDeviceTypeType],  # (5)
    AgentVersion: NotRequired[str],
```

1. See [:material-code-brackets: StackAttributesKeysType](./literals.md#stackattributeskeystype) 
2. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
3. See [:material-code-braces: ChefConfigurationTypeDef](./type_defs.md#chefconfigurationtypedef) 
4. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
5. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 
## CreateStackRequestTypeDef

```python
# CreateStackRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateStackRequestTypeDef


def get_value() -> CreateStackRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateStackRequestTypeDef definition

class CreateStackRequestTypeDef(TypedDict):
    Name: str,
    Region: str,
    ServiceRoleArn: str,
    DefaultInstanceProfileArn: str,
    VpcId: NotRequired[str],
    Attributes: NotRequired[Mapping[StackAttributesKeysType, str]],  # (1)
    DefaultOs: NotRequired[str],
    HostnameTheme: NotRequired[str],
    DefaultAvailabilityZone: NotRequired[str],
    DefaultSubnetId: NotRequired[str],
    CustomJson: NotRequired[str],
    ConfigurationManager: NotRequired[StackConfigurationManagerTypeDef],  # (2)
    ChefConfiguration: NotRequired[ChefConfigurationTypeDef],  # (3)
    UseCustomCookbooks: NotRequired[bool],
    UseOpsworksSecurityGroups: NotRequired[bool],
    CustomCookbooksSource: NotRequired[SourceTypeDef],  # (4)
    DefaultSshKeyName: NotRequired[str],
    DefaultRootDeviceType: NotRequired[RootDeviceTypeType],  # (5)
    AgentVersion: NotRequired[str],
```

1. See [:material-code-brackets: StackAttributesKeysType](./literals.md#stackattributeskeystype) 
2. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
3. See [:material-code-braces: ChefConfigurationTypeDef](./type_defs.md#chefconfigurationtypedef) 
4. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
5. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 
## StackTypeDef

```python
# StackTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import StackTypeDef


def get_value() -> StackTypeDef:
    return {
        "StackId": ...,
    }


# StackTypeDef definition

class StackTypeDef(TypedDict):
    StackId: NotRequired[str],
    Name: NotRequired[str],
    Arn: NotRequired[str],
    Region: NotRequired[str],
    VpcId: NotRequired[str],
    Attributes: NotRequired[Dict[StackAttributesKeysType, str]],  # (1)
    ServiceRoleArn: NotRequired[str],
    DefaultInstanceProfileArn: NotRequired[str],
    DefaultOs: NotRequired[str],
    HostnameTheme: NotRequired[str],
    DefaultAvailabilityZone: NotRequired[str],
    DefaultSubnetId: NotRequired[str],
    CustomJson: NotRequired[str],
    ConfigurationManager: NotRequired[StackConfigurationManagerTypeDef],  # (2)
    ChefConfiguration: NotRequired[ChefConfigurationTypeDef],  # (3)
    UseCustomCookbooks: NotRequired[bool],
    UseOpsworksSecurityGroups: NotRequired[bool],
    CustomCookbooksSource: NotRequired[SourceTypeDef],  # (4)
    DefaultSshKeyName: NotRequired[str],
    CreatedAt: NotRequired[str],
    DefaultRootDeviceType: NotRequired[RootDeviceTypeType],  # (5)
    AgentVersion: NotRequired[str],
```

1. See [:material-code-brackets: StackAttributesKeysType](./literals.md#stackattributeskeystype) 
2. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
3. See [:material-code-braces: ChefConfigurationTypeDef](./type_defs.md#chefconfigurationtypedef) 
4. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
5. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 
## UpdateStackRequestTypeDef

```python
# UpdateStackRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UpdateStackRequestTypeDef


def get_value() -> UpdateStackRequestTypeDef:
    return {
        "StackId": ...,
    }


# UpdateStackRequestTypeDef definition

class UpdateStackRequestTypeDef(TypedDict):
    StackId: str,
    Name: NotRequired[str],
    Attributes: NotRequired[Mapping[StackAttributesKeysType, str]],  # (1)
    ServiceRoleArn: NotRequired[str],
    DefaultInstanceProfileArn: NotRequired[str],
    DefaultOs: NotRequired[str],
    HostnameTheme: NotRequired[str],
    DefaultAvailabilityZone: NotRequired[str],
    DefaultSubnetId: NotRequired[str],
    CustomJson: NotRequired[str],
    ConfigurationManager: NotRequired[StackConfigurationManagerTypeDef],  # (2)
    ChefConfiguration: NotRequired[ChefConfigurationTypeDef],  # (3)
    UseCustomCookbooks: NotRequired[bool],
    CustomCookbooksSource: NotRequired[SourceTypeDef],  # (4)
    DefaultSshKeyName: NotRequired[str],
    DefaultRootDeviceType: NotRequired[RootDeviceTypeType],  # (5)
    UseOpsworksSecurityGroups: NotRequired[bool],
    AgentVersion: NotRequired[str],
```

1. See [:material-code-brackets: StackAttributesKeysType](./literals.md#stackattributeskeystype) 
2. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
3. See [:material-code-braces: ChefConfigurationTypeDef](./type_defs.md#chefconfigurationtypedef) 
4. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
5. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 
## CloneStackResultTypeDef

```python
# CloneStackResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CloneStackResultTypeDef


def get_value() -> CloneStackResultTypeDef:
    return {
        "StackId": ...,
    }


# CloneStackResultTypeDef definition

class CloneStackResultTypeDef(TypedDict):
    StackId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppResultTypeDef

```python
# CreateAppResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateAppResultTypeDef


def get_value() -> CreateAppResultTypeDef:
    return {
        "AppId": ...,
    }


# CreateAppResultTypeDef definition

class CreateAppResultTypeDef(TypedDict):
    AppId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentResultTypeDef

```python
# CreateDeploymentResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateDeploymentResultTypeDef


def get_value() -> CreateDeploymentResultTypeDef:
    return {
        "DeploymentId": ...,
    }


# CreateDeploymentResultTypeDef definition

class CreateDeploymentResultTypeDef(TypedDict):
    DeploymentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceResultTypeDef

```python
# CreateInstanceResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateInstanceResultTypeDef


def get_value() -> CreateInstanceResultTypeDef:
    return {
        "InstanceId": ...,
    }


# CreateInstanceResultTypeDef definition

class CreateInstanceResultTypeDef(TypedDict):
    InstanceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLayerResultTypeDef

```python
# CreateLayerResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateLayerResultTypeDef


def get_value() -> CreateLayerResultTypeDef:
    return {
        "LayerId": ...,
    }


# CreateLayerResultTypeDef definition

class CreateLayerResultTypeDef(TypedDict):
    LayerId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStackResultTypeDef

```python
# CreateStackResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateStackResultTypeDef


def get_value() -> CreateStackResultTypeDef:
    return {
        "StackId": ...,
    }


# CreateStackResultTypeDef definition

class CreateStackResultTypeDef(TypedDict):
    StackId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserProfileResultTypeDef

```python
# CreateUserProfileResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateUserProfileResultTypeDef


def get_value() -> CreateUserProfileResultTypeDef:
    return {
        "IamUserArn": ...,
    }


# CreateUserProfileResultTypeDef definition

class CreateUserProfileResultTypeDef(TypedDict):
    IamUserArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStackProvisioningParametersResultTypeDef

```python
# DescribeStackProvisioningParametersResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeStackProvisioningParametersResultTypeDef


def get_value() -> DescribeStackProvisioningParametersResultTypeDef:
    return {
        "AgentInstallerUrl": ...,
    }


# DescribeStackProvisioningParametersResultTypeDef definition

class DescribeStackProvisioningParametersResultTypeDef(TypedDict):
    AgentInstallerUrl: str,
    Parameters: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetHostnameSuggestionResultTypeDef

```python
# GetHostnameSuggestionResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import GetHostnameSuggestionResultTypeDef


def get_value() -> GetHostnameSuggestionResultTypeDef:
    return {
        "LayerId": ...,
    }


# GetHostnameSuggestionResultTypeDef definition

class GetHostnameSuggestionResultTypeDef(TypedDict):
    LayerId: str,
    Hostname: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsResultTypeDef

```python
# ListTagsResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import ListTagsResultTypeDef


def get_value() -> ListTagsResultTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsResultTypeDef definition

class ListTagsResultTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterEcsClusterResultTypeDef

```python
# RegisterEcsClusterResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RegisterEcsClusterResultTypeDef


def get_value() -> RegisterEcsClusterResultTypeDef:
    return {
        "EcsClusterArn": ...,
    }


# RegisterEcsClusterResultTypeDef definition

class RegisterEcsClusterResultTypeDef(TypedDict):
    EcsClusterArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterElasticIpResultTypeDef

```python
# RegisterElasticIpResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RegisterElasticIpResultTypeDef


def get_value() -> RegisterElasticIpResultTypeDef:
    return {
        "ElasticIp": ...,
    }


# RegisterElasticIpResultTypeDef definition

class RegisterElasticIpResultTypeDef(TypedDict):
    ElasticIp: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterInstanceResultTypeDef

```python
# RegisterInstanceResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RegisterInstanceResultTypeDef


def get_value() -> RegisterInstanceResultTypeDef:
    return {
        "InstanceId": ...,
    }


# RegisterInstanceResultTypeDef definition

class RegisterInstanceResultTypeDef(TypedDict):
    InstanceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterVolumeResultTypeDef

```python
# RegisterVolumeResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RegisterVolumeResultTypeDef


def get_value() -> RegisterVolumeResultTypeDef:
    return {
        "VolumeId": ...,
    }


# RegisterVolumeResultTypeDef definition

class RegisterVolumeResultTypeDef(TypedDict):
    VolumeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CloudWatchLogsConfigurationOutputTypeDef

```python
# CloudWatchLogsConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CloudWatchLogsConfigurationOutputTypeDef


def get_value() -> CloudWatchLogsConfigurationOutputTypeDef:
    return {
        "Enabled": ...,
    }


# CloudWatchLogsConfigurationOutputTypeDef definition

class CloudWatchLogsConfigurationOutputTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    LogStreams: NotRequired[List[CloudWatchLogsLogStreamTypeDef]],  # (1)
```

1. See [:material-code-braces: CloudWatchLogsLogStreamTypeDef](./type_defs.md#cloudwatchlogslogstreamtypedef) 
## CloudWatchLogsConfigurationTypeDef

```python
# CloudWatchLogsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CloudWatchLogsConfigurationTypeDef


def get_value() -> CloudWatchLogsConfigurationTypeDef:
    return {
        "Enabled": ...,
    }


# CloudWatchLogsConfigurationTypeDef definition

class CloudWatchLogsConfigurationTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    LogStreams: NotRequired[Sequence[CloudWatchLogsLogStreamTypeDef]],  # (1)
```

1. See [:material-code-braces: CloudWatchLogsLogStreamTypeDef](./type_defs.md#cloudwatchlogslogstreamtypedef) 
## DescribeCommandsResultTypeDef

```python
# DescribeCommandsResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeCommandsResultTypeDef


def get_value() -> DescribeCommandsResultTypeDef:
    return {
        "Commands": ...,
    }


# DescribeCommandsResultTypeDef definition

class DescribeCommandsResultTypeDef(TypedDict):
    Commands: List[CommandTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommandTypeDef](./type_defs.md#commandtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentTypeDef

```python
# DeploymentTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DeploymentTypeDef


def get_value() -> DeploymentTypeDef:
    return {
        "DeploymentId": ...,
    }


# DeploymentTypeDef definition

class DeploymentTypeDef(TypedDict):
    DeploymentId: NotRequired[str],
    StackId: NotRequired[str],
    AppId: NotRequired[str],
    CreatedAt: NotRequired[str],
    CompletedAt: NotRequired[str],
    Duration: NotRequired[int],
    IamUserArn: NotRequired[str],
    Comment: NotRequired[str],
    Command: NotRequired[DeploymentCommandOutputTypeDef],  # (1)
    Status: NotRequired[str],
    CustomJson: NotRequired[str],
    InstanceIds: NotRequired[List[str]],
```

1. See [:material-code-braces: DeploymentCommandOutputTypeDef](./type_defs.md#deploymentcommandoutputtypedef) 
## DescribeAppsRequestWaitTypeDef

```python
# DescribeAppsRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeAppsRequestWaitTypeDef


def get_value() -> DescribeAppsRequestWaitTypeDef:
    return {
        "StackId": ...,
    }


# DescribeAppsRequestWaitTypeDef definition

class DescribeAppsRequestWaitTypeDef(TypedDict):
    StackId: NotRequired[str],
    AppIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeDeploymentsRequestWaitTypeDef

```python
# DescribeDeploymentsRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeDeploymentsRequestWaitTypeDef


def get_value() -> DescribeDeploymentsRequestWaitTypeDef:
    return {
        "StackId": ...,
    }


# DescribeDeploymentsRequestWaitTypeDef definition

class DescribeDeploymentsRequestWaitTypeDef(TypedDict):
    StackId: NotRequired[str],
    AppId: NotRequired[str],
    DeploymentIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInstancesRequestWaitExtraExtraExtraTypeDef

```python
# DescribeInstancesRequestWaitExtraExtraExtraTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeInstancesRequestWaitExtraExtraExtraTypeDef


def get_value() -> DescribeInstancesRequestWaitExtraExtraExtraTypeDef:
    return {
        "StackId": ...,
    }


# DescribeInstancesRequestWaitExtraExtraExtraTypeDef definition

class DescribeInstancesRequestWaitExtraExtraExtraTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInstancesRequestWaitExtraExtraTypeDef

```python
# DescribeInstancesRequestWaitExtraExtraTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeInstancesRequestWaitExtraExtraTypeDef


def get_value() -> DescribeInstancesRequestWaitExtraExtraTypeDef:
    return {
        "StackId": ...,
    }


# DescribeInstancesRequestWaitExtraExtraTypeDef definition

class DescribeInstancesRequestWaitExtraExtraTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInstancesRequestWaitExtraTypeDef

```python
# DescribeInstancesRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeInstancesRequestWaitExtraTypeDef


def get_value() -> DescribeInstancesRequestWaitExtraTypeDef:
    return {
        "StackId": ...,
    }


# DescribeInstancesRequestWaitExtraTypeDef definition

class DescribeInstancesRequestWaitExtraTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInstancesRequestWaitTypeDef

```python
# DescribeInstancesRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeInstancesRequestWaitTypeDef


def get_value() -> DescribeInstancesRequestWaitTypeDef:
    return {
        "StackId": ...,
    }


# DescribeInstancesRequestWaitTypeDef definition

class DescribeInstancesRequestWaitTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEcsClustersRequestPaginateTypeDef

```python
# DescribeEcsClustersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeEcsClustersRequestPaginateTypeDef


def get_value() -> DescribeEcsClustersRequestPaginateTypeDef:
    return {
        "EcsClusterArns": ...,
    }


# DescribeEcsClustersRequestPaginateTypeDef definition

class DescribeEcsClustersRequestPaginateTypeDef(TypedDict):
    EcsClusterArns: NotRequired[Sequence[str]],
    StackId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEcsClustersResultTypeDef

```python
# DescribeEcsClustersResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeEcsClustersResultTypeDef


def get_value() -> DescribeEcsClustersResultTypeDef:
    return {
        "EcsClusters": ...,
    }


# DescribeEcsClustersResultTypeDef definition

class DescribeEcsClustersResultTypeDef(TypedDict):
    EcsClusters: List[EcsClusterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EcsClusterTypeDef](./type_defs.md#ecsclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeElasticIpsResultTypeDef

```python
# DescribeElasticIpsResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeElasticIpsResultTypeDef


def get_value() -> DescribeElasticIpsResultTypeDef:
    return {
        "ElasticIps": ...,
    }


# DescribeElasticIpsResultTypeDef definition

class DescribeElasticIpsResultTypeDef(TypedDict):
    ElasticIps: List[ElasticIpTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ElasticIpTypeDef](./type_defs.md#elasticiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeElasticLoadBalancersResultTypeDef

```python
# DescribeElasticLoadBalancersResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeElasticLoadBalancersResultTypeDef


def get_value() -> DescribeElasticLoadBalancersResultTypeDef:
    return {
        "ElasticLoadBalancers": ...,
    }


# DescribeElasticLoadBalancersResultTypeDef definition

class DescribeElasticLoadBalancersResultTypeDef(TypedDict):
    ElasticLoadBalancers: List[ElasticLoadBalancerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ElasticLoadBalancerTypeDef](./type_defs.md#elasticloadbalancertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMyUserProfileResultTypeDef

```python
# DescribeMyUserProfileResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeMyUserProfileResultTypeDef


def get_value() -> DescribeMyUserProfileResultTypeDef:
    return {
        "UserProfile": ...,
    }


# DescribeMyUserProfileResultTypeDef definition

class DescribeMyUserProfileResultTypeDef(TypedDict):
    UserProfile: SelfUserProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SelfUserProfileTypeDef](./type_defs.md#selfuserprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePermissionsResultTypeDef

```python
# DescribePermissionsResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribePermissionsResultTypeDef


def get_value() -> DescribePermissionsResultTypeDef:
    return {
        "Permissions": ...,
    }


# DescribePermissionsResultTypeDef definition

class DescribePermissionsResultTypeDef(TypedDict):
    Permissions: List[PermissionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionTypeDef](./type_defs.md#permissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRaidArraysResultTypeDef

```python
# DescribeRaidArraysResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeRaidArraysResultTypeDef


def get_value() -> DescribeRaidArraysResultTypeDef:
    return {
        "RaidArrays": ...,
    }


# DescribeRaidArraysResultTypeDef definition

class DescribeRaidArraysResultTypeDef(TypedDict):
    RaidArrays: List[RaidArrayTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RaidArrayTypeDef](./type_defs.md#raidarraytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRdsDbInstancesResultTypeDef

```python
# DescribeRdsDbInstancesResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeRdsDbInstancesResultTypeDef


def get_value() -> DescribeRdsDbInstancesResultTypeDef:
    return {
        "RdsDbInstances": ...,
    }


# DescribeRdsDbInstancesResultTypeDef definition

class DescribeRdsDbInstancesResultTypeDef(TypedDict):
    RdsDbInstances: List[RdsDbInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RdsDbInstanceTypeDef](./type_defs.md#rdsdbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeServiceErrorsResultTypeDef

```python
# DescribeServiceErrorsResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeServiceErrorsResultTypeDef


def get_value() -> DescribeServiceErrorsResultTypeDef:
    return {
        "ServiceErrors": ...,
    }


# DescribeServiceErrorsResultTypeDef definition

class DescribeServiceErrorsResultTypeDef(TypedDict):
    ServiceErrors: List[ServiceErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceErrorTypeDef](./type_defs.md#serviceerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserProfilesResultTypeDef

```python
# DescribeUserProfilesResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeUserProfilesResultTypeDef


def get_value() -> DescribeUserProfilesResultTypeDef:
    return {
        "UserProfiles": ...,
    }


# DescribeUserProfilesResultTypeDef definition

class DescribeUserProfilesResultTypeDef(TypedDict):
    UserProfiles: List[UserProfileTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserProfileTypeDef](./type_defs.md#userprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVolumesResultTypeDef

```python
# DescribeVolumesResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeVolumesResultTypeDef


def get_value() -> DescribeVolumesResultTypeDef:
    return {
        "Volumes": ...,
    }


# DescribeVolumesResultTypeDef definition

class DescribeVolumesResultTypeDef(TypedDict):
    Volumes: List[VolumeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GrantAccessResultTypeDef

```python
# GrantAccessResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import GrantAccessResultTypeDef


def get_value() -> GrantAccessResultTypeDef:
    return {
        "TemporaryCredential": ...,
    }


# GrantAccessResultTypeDef definition

class GrantAccessResultTypeDef(TypedDict):
    TemporaryCredential: TemporaryCredentialTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemporaryCredentialTypeDef](./type_defs.md#temporarycredentialtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterInstanceRequestTypeDef

```python
# RegisterInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import RegisterInstanceRequestTypeDef


def get_value() -> RegisterInstanceRequestTypeDef:
    return {
        "StackId": ...,
    }


# RegisterInstanceRequestTypeDef definition

class RegisterInstanceRequestTypeDef(TypedDict):
    StackId: str,
    Hostname: NotRequired[str],
    PublicIp: NotRequired[str],
    PrivateIp: NotRequired[str],
    RsaPublicKey: NotRequired[str],
    RsaPublicKeyFingerprint: NotRequired[str],
    InstanceIdentity: NotRequired[InstanceIdentityTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceIdentityTypeDef](./type_defs.md#instanceidentitytypedef) 
## StackSummaryTypeDef

```python
# StackSummaryTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import StackSummaryTypeDef


def get_value() -> StackSummaryTypeDef:
    return {
        "StackId": ...,
    }


# StackSummaryTypeDef definition

class StackSummaryTypeDef(TypedDict):
    StackId: NotRequired[str],
    Name: NotRequired[str],
    Arn: NotRequired[str],
    LayersCount: NotRequired[int],
    AppsCount: NotRequired[int],
    InstancesCount: NotRequired[InstancesCountTypeDef],  # (1)
```

1. See [:material-code-braces: InstancesCountTypeDef](./type_defs.md#instancescounttypedef) 
## LifecycleEventConfigurationTypeDef

```python
# LifecycleEventConfigurationTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import LifecycleEventConfigurationTypeDef


def get_value() -> LifecycleEventConfigurationTypeDef:
    return {
        "Shutdown": ...,
    }


# LifecycleEventConfigurationTypeDef definition

class LifecycleEventConfigurationTypeDef(TypedDict):
    Shutdown: NotRequired[ShutdownEventConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ShutdownEventConfigurationTypeDef](./type_defs.md#shutdowneventconfigurationtypedef) 
## OperatingSystemTypeDef

```python
# OperatingSystemTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import OperatingSystemTypeDef


def get_value() -> OperatingSystemTypeDef:
    return {
        "Name": ...,
    }


# OperatingSystemTypeDef definition

class OperatingSystemTypeDef(TypedDict):
    Name: NotRequired[str],
    Id: NotRequired[str],
    Type: NotRequired[str],
    ConfigurationManagers: NotRequired[List[OperatingSystemConfigurationManagerTypeDef]],  # (1)
    ReportedName: NotRequired[str],
    ReportedVersion: NotRequired[str],
    Supported: NotRequired[bool],
```

1. See [:material-code-braces: OperatingSystemConfigurationManagerTypeDef](./type_defs.md#operatingsystemconfigurationmanagertypedef) 
## TimeBasedAutoScalingConfigurationTypeDef

```python
# TimeBasedAutoScalingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import TimeBasedAutoScalingConfigurationTypeDef


def get_value() -> TimeBasedAutoScalingConfigurationTypeDef:
    return {
        "InstanceId": ...,
    }


# TimeBasedAutoScalingConfigurationTypeDef definition

class TimeBasedAutoScalingConfigurationTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    AutoScalingSchedule: NotRequired[WeeklyAutoScalingScheduleOutputTypeDef],  # (1)
```

1. See [:material-code-braces: WeeklyAutoScalingScheduleOutputTypeDef](./type_defs.md#weeklyautoscalingscheduleoutputtypedef) 
## DescribeAgentVersionsResultTypeDef

```python
# DescribeAgentVersionsResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeAgentVersionsResultTypeDef


def get_value() -> DescribeAgentVersionsResultTypeDef:
    return {
        "AgentVersions": ...,
    }


# DescribeAgentVersionsResultTypeDef definition

class DescribeAgentVersionsResultTypeDef(TypedDict):
    AgentVersions: List[AgentVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentVersionTypeDef](./type_defs.md#agentversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppsResultTypeDef

```python
# DescribeAppsResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeAppsResultTypeDef


def get_value() -> DescribeAppsResultTypeDef:
    return {
        "Apps": ...,
    }


# DescribeAppsResultTypeDef definition

class DescribeAppsResultTypeDef(TypedDict):
    Apps: List[AppTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLoadBasedAutoScalingResultTypeDef

```python
# DescribeLoadBasedAutoScalingResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeLoadBasedAutoScalingResultTypeDef


def get_value() -> DescribeLoadBasedAutoScalingResultTypeDef:
    return {
        "LoadBasedAutoScalingConfigurations": ...,
    }


# DescribeLoadBasedAutoScalingResultTypeDef definition

class DescribeLoadBasedAutoScalingResultTypeDef(TypedDict):
    LoadBasedAutoScalingConfigurations: List[LoadBasedAutoScalingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBasedAutoScalingConfigurationTypeDef](./type_defs.md#loadbasedautoscalingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetLoadBasedAutoScalingRequestTypeDef

```python
# SetLoadBasedAutoScalingRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import SetLoadBasedAutoScalingRequestTypeDef


def get_value() -> SetLoadBasedAutoScalingRequestTypeDef:
    return {
        "LayerId": ...,
    }


# SetLoadBasedAutoScalingRequestTypeDef definition

class SetLoadBasedAutoScalingRequestTypeDef(TypedDict):
    LayerId: str,
    Enable: NotRequired[bool],
    UpScaling: NotRequired[AutoScalingThresholdsUnionTypeDef],  # (1)
    DownScaling: NotRequired[AutoScalingThresholdsUnionTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingThresholdsTypeDef](./type_defs.md#autoscalingthresholdstypedef) [:material-code-braces: AutoScalingThresholdsOutputTypeDef](./type_defs.md#autoscalingthresholdsoutputtypedef) 
2. See [:material-code-braces: AutoScalingThresholdsTypeDef](./type_defs.md#autoscalingthresholdstypedef) [:material-code-braces: AutoScalingThresholdsOutputTypeDef](./type_defs.md#autoscalingthresholdsoutputtypedef) 
## CreateInstanceRequestTypeDef

```python
# CreateInstanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateInstanceRequestTypeDef


def get_value() -> CreateInstanceRequestTypeDef:
    return {
        "StackId": ...,
    }


# CreateInstanceRequestTypeDef definition

class CreateInstanceRequestTypeDef(TypedDict):
    StackId: str,
    LayerIds: Sequence[str],
    InstanceType: str,
    AutoScalingType: NotRequired[AutoScalingTypeType],  # (1)
    Hostname: NotRequired[str],
    Os: NotRequired[str],
    AmiId: NotRequired[str],
    SshKeyName: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    VirtualizationType: NotRequired[str],
    SubnetId: NotRequired[str],
    Architecture: NotRequired[ArchitectureType],  # (2)
    RootDeviceType: NotRequired[RootDeviceTypeType],  # (3)
    BlockDeviceMappings: NotRequired[Sequence[BlockDeviceMappingTypeDef]],  # (4)
    InstallUpdatesOnBoot: NotRequired[bool],
    EbsOptimized: NotRequired[bool],
    AgentVersion: NotRequired[str],
    Tenancy: NotRequired[str],
```

1. See [:material-code-brackets: AutoScalingTypeType](./literals.md#autoscalingtypetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 
4. See [:material-code-braces: BlockDeviceMappingTypeDef](./type_defs.md#blockdevicemappingtypedef) 
## InstanceTypeDef

```python
# InstanceTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import InstanceTypeDef


def get_value() -> InstanceTypeDef:
    return {
        "AgentVersion": ...,
    }


# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    AgentVersion: NotRequired[str],
    AmiId: NotRequired[str],
    Architecture: NotRequired[ArchitectureType],  # (1)
    Arn: NotRequired[str],
    AutoScalingType: NotRequired[AutoScalingTypeType],  # (2)
    AvailabilityZone: NotRequired[str],
    BlockDeviceMappings: NotRequired[List[BlockDeviceMappingTypeDef]],  # (3)
    CreatedAt: NotRequired[str],
    EbsOptimized: NotRequired[bool],
    Ec2InstanceId: NotRequired[str],
    EcsClusterArn: NotRequired[str],
    EcsContainerInstanceArn: NotRequired[str],
    ElasticIp: NotRequired[str],
    Hostname: NotRequired[str],
    InfrastructureClass: NotRequired[str],
    InstallUpdatesOnBoot: NotRequired[bool],
    InstanceId: NotRequired[str],
    InstanceProfileArn: NotRequired[str],
    InstanceType: NotRequired[str],
    LastServiceErrorId: NotRequired[str],
    LayerIds: NotRequired[List[str]],
    Os: NotRequired[str],
    Platform: NotRequired[str],
    PrivateDns: NotRequired[str],
    PrivateIp: NotRequired[str],
    PublicDns: NotRequired[str],
    PublicIp: NotRequired[str],
    RegisteredBy: NotRequired[str],
    ReportedAgentVersion: NotRequired[str],
    ReportedOs: NotRequired[ReportedOsTypeDef],  # (4)
    RootDeviceType: NotRequired[RootDeviceTypeType],  # (5)
    RootDeviceVolumeId: NotRequired[str],
    SecurityGroupIds: NotRequired[List[str]],
    SshHostDsaKeyFingerprint: NotRequired[str],
    SshHostRsaKeyFingerprint: NotRequired[str],
    SshKeyName: NotRequired[str],
    StackId: NotRequired[str],
    Status: NotRequired[str],
    SubnetId: NotRequired[str],
    Tenancy: NotRequired[str],
    VirtualizationType: NotRequired[VirtualizationTypeType],  # (6)
```

1. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
2. See [:material-code-brackets: AutoScalingTypeType](./literals.md#autoscalingtypetype) 
3. See [:material-code-braces: BlockDeviceMappingTypeDef](./type_defs.md#blockdevicemappingtypedef) 
4. See [:material-code-braces: ReportedOsTypeDef](./type_defs.md#reportedostypedef) 
5. See [:material-code-brackets: RootDeviceTypeType](./literals.md#rootdevicetypetype) 
6. See [:material-code-brackets: VirtualizationTypeType](./literals.md#virtualizationtypetype) 
## DescribeStacksResultTypeDef

```python
# DescribeStacksResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeStacksResultTypeDef


def get_value() -> DescribeStacksResultTypeDef:
    return {
        "Stacks": ...,
    }


# DescribeStacksResultTypeDef definition

class DescribeStacksResultTypeDef(TypedDict):
    Stacks: List[StackTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StackTypeDef](./type_defs.md#stacktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDeploymentsResultTypeDef

```python
# DescribeDeploymentsResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeDeploymentsResultTypeDef


def get_value() -> DescribeDeploymentsResultTypeDef:
    return {
        "Deployments": ...,
    }


# DescribeDeploymentsResultTypeDef definition

class DescribeDeploymentsResultTypeDef(TypedDict):
    Deployments: List[DeploymentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentRequestTypeDef

```python
# CreateDeploymentRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateDeploymentRequestTypeDef


def get_value() -> CreateDeploymentRequestTypeDef:
    return {
        "StackId": ...,
    }


# CreateDeploymentRequestTypeDef definition

class CreateDeploymentRequestTypeDef(TypedDict):
    StackId: str,
    Command: DeploymentCommandUnionTypeDef,  # (1)
    AppId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
    LayerIds: NotRequired[Sequence[str]],
    Comment: NotRequired[str],
    CustomJson: NotRequired[str],
```

1. See [:material-code-braces: DeploymentCommandTypeDef](./type_defs.md#deploymentcommandtypedef) [:material-code-braces: DeploymentCommandOutputTypeDef](./type_defs.md#deploymentcommandoutputtypedef) 
## DescribeStackSummaryResultTypeDef

```python
# DescribeStackSummaryResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeStackSummaryResultTypeDef


def get_value() -> DescribeStackSummaryResultTypeDef:
    return {
        "StackSummary": ...,
    }


# DescribeStackSummaryResultTypeDef definition

class DescribeStackSummaryResultTypeDef(TypedDict):
    StackSummary: StackSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StackSummaryTypeDef](./type_defs.md#stacksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LayerTypeDef

```python
# LayerTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import LayerTypeDef


def get_value() -> LayerTypeDef:
    return {
        "Arn": ...,
    }


# LayerTypeDef definition

class LayerTypeDef(TypedDict):
    Arn: NotRequired[str],
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    Type: NotRequired[LayerTypeType],  # (1)
    Name: NotRequired[str],
    Shortname: NotRequired[str],
    Attributes: NotRequired[Dict[LayerAttributesKeysType, str]],  # (2)
    CloudWatchLogsConfiguration: NotRequired[CloudWatchLogsConfigurationOutputTypeDef],  # (3)
    CustomInstanceProfileArn: NotRequired[str],
    CustomJson: NotRequired[str],
    CustomSecurityGroupIds: NotRequired[List[str]],
    DefaultSecurityGroupNames: NotRequired[List[str]],
    Packages: NotRequired[List[str]],
    VolumeConfigurations: NotRequired[List[VolumeConfigurationTypeDef]],  # (4)
    EnableAutoHealing: NotRequired[bool],
    AutoAssignElasticIps: NotRequired[bool],
    AutoAssignPublicIps: NotRequired[bool],
    DefaultRecipes: NotRequired[RecipesOutputTypeDef],  # (5)
    CustomRecipes: NotRequired[RecipesOutputTypeDef],  # (5)
    CreatedAt: NotRequired[str],
    InstallUpdatesOnBoot: NotRequired[bool],
    UseEbsOptimizedInstances: NotRequired[bool],
    LifecycleEventConfiguration: NotRequired[LifecycleEventConfigurationTypeDef],  # (7)
```

1. See [:material-code-brackets: LayerTypeType](./literals.md#layertypetype) 
2. See [:material-code-brackets: LayerAttributesKeysType](./literals.md#layerattributeskeystype) 
3. See [:material-code-braces: CloudWatchLogsConfigurationOutputTypeDef](./type_defs.md#cloudwatchlogsconfigurationoutputtypedef) 
4. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
5. See [:material-code-braces: RecipesOutputTypeDef](./type_defs.md#recipesoutputtypedef) 
6. See [:material-code-braces: RecipesOutputTypeDef](./type_defs.md#recipesoutputtypedef) 
7. See [:material-code-braces: LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef) 
## DescribeOperatingSystemsResponseTypeDef

```python
# DescribeOperatingSystemsResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeOperatingSystemsResponseTypeDef


def get_value() -> DescribeOperatingSystemsResponseTypeDef:
    return {
        "OperatingSystems": ...,
    }


# DescribeOperatingSystemsResponseTypeDef definition

class DescribeOperatingSystemsResponseTypeDef(TypedDict):
    OperatingSystems: List[OperatingSystemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperatingSystemTypeDef](./type_defs.md#operatingsystemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTimeBasedAutoScalingResultTypeDef

```python
# DescribeTimeBasedAutoScalingResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeTimeBasedAutoScalingResultTypeDef


def get_value() -> DescribeTimeBasedAutoScalingResultTypeDef:
    return {
        "TimeBasedAutoScalingConfigurations": ...,
    }


# DescribeTimeBasedAutoScalingResultTypeDef definition

class DescribeTimeBasedAutoScalingResultTypeDef(TypedDict):
    TimeBasedAutoScalingConfigurations: List[TimeBasedAutoScalingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TimeBasedAutoScalingConfigurationTypeDef](./type_defs.md#timebasedautoscalingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetTimeBasedAutoScalingRequestTypeDef

```python
# SetTimeBasedAutoScalingRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import SetTimeBasedAutoScalingRequestTypeDef


def get_value() -> SetTimeBasedAutoScalingRequestTypeDef:
    return {
        "InstanceId": ...,
    }


# SetTimeBasedAutoScalingRequestTypeDef definition

class SetTimeBasedAutoScalingRequestTypeDef(TypedDict):
    InstanceId: str,
    AutoScalingSchedule: NotRequired[WeeklyAutoScalingScheduleUnionTypeDef],  # (1)
```

1. See [:material-code-braces: WeeklyAutoScalingScheduleTypeDef](./type_defs.md#weeklyautoscalingscheduletypedef) [:material-code-braces: WeeklyAutoScalingScheduleOutputTypeDef](./type_defs.md#weeklyautoscalingscheduleoutputtypedef) 
## DescribeInstancesResultTypeDef

```python
# DescribeInstancesResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeInstancesResultTypeDef


def get_value() -> DescribeInstancesResultTypeDef:
    return {
        "Instances": ...,
    }


# DescribeInstancesResultTypeDef definition

class DescribeInstancesResultTypeDef(TypedDict):
    Instances: List[InstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLayerRequestStackCreateLayerTypeDef

```python
# CreateLayerRequestStackCreateLayerTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateLayerRequestStackCreateLayerTypeDef


def get_value() -> CreateLayerRequestStackCreateLayerTypeDef:
    return {
        "Type": ...,
    }


# CreateLayerRequestStackCreateLayerTypeDef definition

class CreateLayerRequestStackCreateLayerTypeDef(TypedDict):
    Type: LayerTypeType,  # (1)
    Name: str,
    Shortname: str,
    Attributes: NotRequired[Mapping[LayerAttributesKeysType, str]],  # (2)
    CloudWatchLogsConfiguration: NotRequired[CloudWatchLogsConfigurationUnionTypeDef],  # (3)
    CustomInstanceProfileArn: NotRequired[str],
    CustomJson: NotRequired[str],
    CustomSecurityGroupIds: NotRequired[Sequence[str]],
    Packages: NotRequired[Sequence[str]],
    VolumeConfigurations: NotRequired[Sequence[VolumeConfigurationTypeDef]],  # (4)
    EnableAutoHealing: NotRequired[bool],
    AutoAssignElasticIps: NotRequired[bool],
    AutoAssignPublicIps: NotRequired[bool],
    CustomRecipes: NotRequired[RecipesUnionTypeDef],  # (5)
    InstallUpdatesOnBoot: NotRequired[bool],
    UseEbsOptimizedInstances: NotRequired[bool],
    LifecycleEventConfiguration: NotRequired[LifecycleEventConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: LayerTypeType](./literals.md#layertypetype) 
2. See [:material-code-brackets: LayerAttributesKeysType](./literals.md#layerattributeskeystype) 
3. See [:material-code-braces: CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef) [:material-code-braces: CloudWatchLogsConfigurationOutputTypeDef](./type_defs.md#cloudwatchlogsconfigurationoutputtypedef) 
4. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
5. See [:material-code-braces: RecipesTypeDef](./type_defs.md#recipestypedef) [:material-code-braces: RecipesOutputTypeDef](./type_defs.md#recipesoutputtypedef) 
6. See [:material-code-braces: LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef) 
## CreateLayerRequestTypeDef

```python
# CreateLayerRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import CreateLayerRequestTypeDef


def get_value() -> CreateLayerRequestTypeDef:
    return {
        "StackId": ...,
    }


# CreateLayerRequestTypeDef definition

class CreateLayerRequestTypeDef(TypedDict):
    StackId: str,
    Type: LayerTypeType,  # (1)
    Name: str,
    Shortname: str,
    Attributes: NotRequired[Mapping[LayerAttributesKeysType, str]],  # (2)
    CloudWatchLogsConfiguration: NotRequired[CloudWatchLogsConfigurationUnionTypeDef],  # (3)
    CustomInstanceProfileArn: NotRequired[str],
    CustomJson: NotRequired[str],
    CustomSecurityGroupIds: NotRequired[Sequence[str]],
    Packages: NotRequired[Sequence[str]],
    VolumeConfigurations: NotRequired[Sequence[VolumeConfigurationTypeDef]],  # (4)
    EnableAutoHealing: NotRequired[bool],
    AutoAssignElasticIps: NotRequired[bool],
    AutoAssignPublicIps: NotRequired[bool],
    CustomRecipes: NotRequired[RecipesUnionTypeDef],  # (5)
    InstallUpdatesOnBoot: NotRequired[bool],
    UseEbsOptimizedInstances: NotRequired[bool],
    LifecycleEventConfiguration: NotRequired[LifecycleEventConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: LayerTypeType](./literals.md#layertypetype) 
2. See [:material-code-brackets: LayerAttributesKeysType](./literals.md#layerattributeskeystype) 
3. See [:material-code-braces: CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef) [:material-code-braces: CloudWatchLogsConfigurationOutputTypeDef](./type_defs.md#cloudwatchlogsconfigurationoutputtypedef) 
4. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
5. See [:material-code-braces: RecipesTypeDef](./type_defs.md#recipestypedef) [:material-code-braces: RecipesOutputTypeDef](./type_defs.md#recipesoutputtypedef) 
6. See [:material-code-braces: LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef) 
## UpdateLayerRequestTypeDef

```python
# UpdateLayerRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import UpdateLayerRequestTypeDef


def get_value() -> UpdateLayerRequestTypeDef:
    return {
        "LayerId": ...,
    }


# UpdateLayerRequestTypeDef definition

class UpdateLayerRequestTypeDef(TypedDict):
    LayerId: str,
    Name: NotRequired[str],
    Shortname: NotRequired[str],
    Attributes: NotRequired[Mapping[LayerAttributesKeysType, str]],  # (1)
    CloudWatchLogsConfiguration: NotRequired[CloudWatchLogsConfigurationUnionTypeDef],  # (2)
    CustomInstanceProfileArn: NotRequired[str],
    CustomJson: NotRequired[str],
    CustomSecurityGroupIds: NotRequired[Sequence[str]],
    Packages: NotRequired[Sequence[str]],
    VolumeConfigurations: NotRequired[Sequence[VolumeConfigurationTypeDef]],  # (3)
    EnableAutoHealing: NotRequired[bool],
    AutoAssignElasticIps: NotRequired[bool],
    AutoAssignPublicIps: NotRequired[bool],
    CustomRecipes: NotRequired[RecipesUnionTypeDef],  # (4)
    InstallUpdatesOnBoot: NotRequired[bool],
    UseEbsOptimizedInstances: NotRequired[bool],
    LifecycleEventConfiguration: NotRequired[LifecycleEventConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: LayerAttributesKeysType](./literals.md#layerattributeskeystype) 
2. See [:material-code-braces: CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef) [:material-code-braces: CloudWatchLogsConfigurationOutputTypeDef](./type_defs.md#cloudwatchlogsconfigurationoutputtypedef) 
3. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
4. See [:material-code-braces: RecipesTypeDef](./type_defs.md#recipestypedef) [:material-code-braces: RecipesOutputTypeDef](./type_defs.md#recipesoutputtypedef) 
5. See [:material-code-braces: LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef) 
## DescribeLayersResultTypeDef

```python
# DescribeLayersResultTypeDef TypedDict usage example

from types_aiobotocore_opsworks.type_defs import DescribeLayersResultTypeDef


def get_value() -> DescribeLayersResultTypeDef:
    return {
        "Layers": ...,
    }


# DescribeLayersResultTypeDef definition

class DescribeLayersResultTypeDef(TypedDict):
    Layers: List[LayerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LayerTypeDef](./type_defs.md#layertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
