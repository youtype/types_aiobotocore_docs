# Type definitions

> [Index](../README.md) > [OpsWorks](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).



## StackConfigurationManagerTypeDef

```python
# StackConfigurationManagerTypeDef definition

class StackConfigurationManagerTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    Type: NotRequired[str],
    Arn: NotRequired[str],
    DatabaseName: NotRequired[str],
```

## EnvironmentVariableTypeDef

```python
# EnvironmentVariableTypeDef definition

class EnvironmentVariableTypeDef(TypedDict):
    Key: str,
    Value: str,
    Secure: NotRequired[bool],
```

## SourceTypeDef

```python
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
# SslConfigurationTypeDef definition

class SslConfigurationTypeDef(TypedDict):
    Certificate: str,
    PrivateKey: str,
    Chain: NotRequired[str],
```

## AssignInstanceRequestRequestTypeDef

```python
# AssignInstanceRequestRequestTypeDef definition

class AssignInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    LayerIds: Sequence[str],
```

## AssignVolumeRequestRequestTypeDef

```python
# AssignVolumeRequestRequestTypeDef definition

class AssignVolumeRequestRequestTypeDef(TypedDict):
    VolumeId: str,
    InstanceId: NotRequired[str],
```

## AssociateElasticIpRequestRequestTypeDef

```python
# AssociateElasticIpRequestRequestTypeDef definition

class AssociateElasticIpRequestRequestTypeDef(TypedDict):
    ElasticIp: str,
    InstanceId: NotRequired[str],
```

## AttachElasticLoadBalancerRequestRequestTypeDef

```python
# AttachElasticLoadBalancerRequestRequestTypeDef definition

class AttachElasticLoadBalancerRequestRequestTypeDef(TypedDict):
    ElasticLoadBalancerName: str,
    LayerId: str,
```

## AutoScalingThresholdsOutputTypeDef

```python
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
# ChefConfigurationTypeDef definition

class ChefConfigurationTypeDef(TypedDict):
    ManageBerkshelf: NotRequired[bool],
    BerkshelfVersion: NotRequired[str],
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

## CloudWatchLogsLogStreamTypeDef

```python
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

## DeploymentCommandTypeDef

```python
# DeploymentCommandTypeDef definition

class DeploymentCommandTypeDef(TypedDict):
    Name: DeploymentCommandNameType,  # (1)
    Args: NotRequired[Mapping[str, Sequence[str]]],
```

1. See [:material-code-brackets: DeploymentCommandNameType](./literals.md#deploymentcommandnametype) 
## RecipesTypeDef

```python
# RecipesTypeDef definition

class RecipesTypeDef(TypedDict):
    Setup: NotRequired[Sequence[str]],
    Configure: NotRequired[Sequence[str]],
    Deploy: NotRequired[Sequence[str]],
    Undeploy: NotRequired[Sequence[str]],
    Shutdown: NotRequired[Sequence[str]],
```

## VolumeConfigurationTypeDef

```python
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

## CreateUserProfileRequestRequestTypeDef

```python
# CreateUserProfileRequestRequestTypeDef definition

class CreateUserProfileRequestRequestTypeDef(TypedDict):
    IamUserArn: str,
    SshUsername: NotRequired[str],
    SshPublicKey: NotRequired[str],
    AllowSelfManagement: NotRequired[bool],
```

## DeleteAppRequestRequestTypeDef

```python
# DeleteAppRequestRequestTypeDef definition

class DeleteAppRequestRequestTypeDef(TypedDict):
    AppId: str,
```

## DeleteInstanceRequestRequestTypeDef

```python
# DeleteInstanceRequestRequestTypeDef definition

class DeleteInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    DeleteElasticIp: NotRequired[bool],
    DeleteVolumes: NotRequired[bool],
```

## DeleteLayerRequestRequestTypeDef

```python
# DeleteLayerRequestRequestTypeDef definition

class DeleteLayerRequestRequestTypeDef(TypedDict):
    LayerId: str,
```

## DeleteStackRequestRequestTypeDef

```python
# DeleteStackRequestRequestTypeDef definition

class DeleteStackRequestRequestTypeDef(TypedDict):
    StackId: str,
```

## DeleteUserProfileRequestRequestTypeDef

```python
# DeleteUserProfileRequestRequestTypeDef definition

class DeleteUserProfileRequestRequestTypeDef(TypedDict):
    IamUserArn: str,
```

## DeploymentCommandOutputTypeDef

```python
# DeploymentCommandOutputTypeDef definition

class DeploymentCommandOutputTypeDef(TypedDict):
    Name: DeploymentCommandNameType,  # (1)
    Args: NotRequired[Dict[str, List[str]]],
```

1. See [:material-code-brackets: DeploymentCommandNameType](./literals.md#deploymentcommandnametype) 
## DeregisterEcsClusterRequestRequestTypeDef

```python
# DeregisterEcsClusterRequestRequestTypeDef definition

class DeregisterEcsClusterRequestRequestTypeDef(TypedDict):
    EcsClusterArn: str,
```

## DeregisterElasticIpRequestRequestTypeDef

```python
# DeregisterElasticIpRequestRequestTypeDef definition

class DeregisterElasticIpRequestRequestTypeDef(TypedDict):
    ElasticIp: str,
```

## DeregisterInstanceRequestRequestTypeDef

```python
# DeregisterInstanceRequestRequestTypeDef definition

class DeregisterInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
```

## DeregisterRdsDbInstanceRequestRequestTypeDef

```python
# DeregisterRdsDbInstanceRequestRequestTypeDef definition

class DeregisterRdsDbInstanceRequestRequestTypeDef(TypedDict):
    RdsDbInstanceArn: str,
```

## DeregisterVolumeRequestRequestTypeDef

```python
# DeregisterVolumeRequestRequestTypeDef definition

class DeregisterVolumeRequestRequestTypeDef(TypedDict):
    VolumeId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeAppsRequestRequestTypeDef

```python
# DescribeAppsRequestRequestTypeDef definition

class DescribeAppsRequestRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    AppIds: NotRequired[Sequence[str]],
```

## DescribeCommandsRequestRequestTypeDef

```python
# DescribeCommandsRequestRequestTypeDef definition

class DescribeCommandsRequestRequestTypeDef(TypedDict):
    DeploymentId: NotRequired[str],
    InstanceId: NotRequired[str],
    CommandIds: NotRequired[Sequence[str]],
```

## DescribeDeploymentsRequestRequestTypeDef

```python
# DescribeDeploymentsRequestRequestTypeDef definition

class DescribeDeploymentsRequestRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    AppId: NotRequired[str],
    DeploymentIds: NotRequired[Sequence[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeEcsClustersRequestRequestTypeDef

```python
# DescribeEcsClustersRequestRequestTypeDef definition

class DescribeEcsClustersRequestRequestTypeDef(TypedDict):
    EcsClusterArns: NotRequired[Sequence[str]],
    StackId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## EcsClusterTypeDef

```python
# EcsClusterTypeDef definition

class EcsClusterTypeDef(TypedDict):
    EcsClusterArn: NotRequired[str],
    EcsClusterName: NotRequired[str],
    StackId: NotRequired[str],
    RegisteredAt: NotRequired[str],
```

## DescribeElasticIpsRequestRequestTypeDef

```python
# DescribeElasticIpsRequestRequestTypeDef definition

class DescribeElasticIpsRequestRequestTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    StackId: NotRequired[str],
    Ips: NotRequired[Sequence[str]],
```

## ElasticIpTypeDef

```python
# ElasticIpTypeDef definition

class ElasticIpTypeDef(TypedDict):
    Ip: NotRequired[str],
    Name: NotRequired[str],
    Domain: NotRequired[str],
    Region: NotRequired[str],
    InstanceId: NotRequired[str],
```

## DescribeElasticLoadBalancersRequestRequestTypeDef

```python
# DescribeElasticLoadBalancersRequestRequestTypeDef definition

class DescribeElasticLoadBalancersRequestRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerIds: NotRequired[Sequence[str]],
```

## ElasticLoadBalancerTypeDef

```python
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

## DescribeInstancesRequestRequestTypeDef

```python
# DescribeInstancesRequestRequestTypeDef definition

class DescribeInstancesRequestRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
```

## DescribeLayersRequestRequestTypeDef

```python
# DescribeLayersRequestRequestTypeDef definition

class DescribeLayersRequestRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerIds: NotRequired[Sequence[str]],
```

## DescribeLoadBasedAutoScalingRequestRequestTypeDef

```python
# DescribeLoadBasedAutoScalingRequestRequestTypeDef definition

class DescribeLoadBasedAutoScalingRequestRequestTypeDef(TypedDict):
    LayerIds: Sequence[str],
```

## SelfUserProfileTypeDef

```python
# SelfUserProfileTypeDef definition

class SelfUserProfileTypeDef(TypedDict):
    IamUserArn: NotRequired[str],
    Name: NotRequired[str],
    SshUsername: NotRequired[str],
    SshPublicKey: NotRequired[str],
```

## DescribePermissionsRequestRequestTypeDef

```python
# DescribePermissionsRequestRequestTypeDef definition

class DescribePermissionsRequestRequestTypeDef(TypedDict):
    IamUserArn: NotRequired[str],
    StackId: NotRequired[str],
```

## PermissionTypeDef

```python
# PermissionTypeDef definition

class PermissionTypeDef(TypedDict):
    StackId: NotRequired[str],
    IamUserArn: NotRequired[str],
    AllowSsh: NotRequired[bool],
    AllowSudo: NotRequired[bool],
    Level: NotRequired[str],
```

## DescribeRaidArraysRequestRequestTypeDef

```python
# DescribeRaidArraysRequestRequestTypeDef definition

class DescribeRaidArraysRequestRequestTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    StackId: NotRequired[str],
    RaidArrayIds: NotRequired[Sequence[str]],
```

## RaidArrayTypeDef

```python
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

## DescribeRdsDbInstancesRequestRequestTypeDef

```python
# DescribeRdsDbInstancesRequestRequestTypeDef definition

class DescribeRdsDbInstancesRequestRequestTypeDef(TypedDict):
    StackId: str,
    RdsDbInstanceArns: NotRequired[Sequence[str]],
```

## RdsDbInstanceTypeDef

```python
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

## DescribeServiceErrorsRequestRequestTypeDef

```python
# DescribeServiceErrorsRequestRequestTypeDef definition

class DescribeServiceErrorsRequestRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    InstanceId: NotRequired[str],
    ServiceErrorIds: NotRequired[Sequence[str]],
```

## ServiceErrorTypeDef

```python
# ServiceErrorTypeDef definition

class ServiceErrorTypeDef(TypedDict):
    ServiceErrorId: NotRequired[str],
    StackId: NotRequired[str],
    InstanceId: NotRequired[str],
    Type: NotRequired[str],
    Message: NotRequired[str],
    CreatedAt: NotRequired[str],
```

## DescribeStackProvisioningParametersRequestRequestTypeDef

```python
# DescribeStackProvisioningParametersRequestRequestTypeDef definition

class DescribeStackProvisioningParametersRequestRequestTypeDef(TypedDict):
    StackId: str,
```

## DescribeStackSummaryRequestRequestTypeDef

```python
# DescribeStackSummaryRequestRequestTypeDef definition

class DescribeStackSummaryRequestRequestTypeDef(TypedDict):
    StackId: str,
```

## DescribeStacksRequestRequestTypeDef

```python
# DescribeStacksRequestRequestTypeDef definition

class DescribeStacksRequestRequestTypeDef(TypedDict):
    StackIds: NotRequired[Sequence[str]],
```

## DescribeTimeBasedAutoScalingRequestRequestTypeDef

```python
# DescribeTimeBasedAutoScalingRequestRequestTypeDef definition

class DescribeTimeBasedAutoScalingRequestRequestTypeDef(TypedDict):
    InstanceIds: Sequence[str],
```

## DescribeUserProfilesRequestRequestTypeDef

```python
# DescribeUserProfilesRequestRequestTypeDef definition

class DescribeUserProfilesRequestRequestTypeDef(TypedDict):
    IamUserArns: NotRequired[Sequence[str]],
```

## UserProfileTypeDef

```python
# UserProfileTypeDef definition

class UserProfileTypeDef(TypedDict):
    IamUserArn: NotRequired[str],
    Name: NotRequired[str],
    SshUsername: NotRequired[str],
    SshPublicKey: NotRequired[str],
    AllowSelfManagement: NotRequired[bool],
```

## DescribeVolumesRequestRequestTypeDef

```python
# DescribeVolumesRequestRequestTypeDef definition

class DescribeVolumesRequestRequestTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    StackId: NotRequired[str],
    RaidArrayId: NotRequired[str],
    VolumeIds: NotRequired[Sequence[str]],
```

## VolumeTypeDef

```python
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

## DetachElasticLoadBalancerRequestRequestTypeDef

```python
# DetachElasticLoadBalancerRequestRequestTypeDef definition

class DetachElasticLoadBalancerRequestRequestTypeDef(TypedDict):
    ElasticLoadBalancerName: str,
    LayerId: str,
```

## DisassociateElasticIpRequestRequestTypeDef

```python
# DisassociateElasticIpRequestRequestTypeDef definition

class DisassociateElasticIpRequestRequestTypeDef(TypedDict):
    ElasticIp: str,
```

## GetHostnameSuggestionRequestRequestTypeDef

```python
# GetHostnameSuggestionRequestRequestTypeDef definition

class GetHostnameSuggestionRequestRequestTypeDef(TypedDict):
    LayerId: str,
```

## GrantAccessRequestRequestTypeDef

```python
# GrantAccessRequestRequestTypeDef definition

class GrantAccessRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    ValidForInMinutes: NotRequired[int],
```

## TemporaryCredentialTypeDef

```python
# TemporaryCredentialTypeDef definition

class TemporaryCredentialTypeDef(TypedDict):
    Username: NotRequired[str],
    Password: NotRequired[str],
    ValidForInMinutes: NotRequired[int],
    InstanceId: NotRequired[str],
```

## InstanceIdentityTypeDef

```python
# InstanceIdentityTypeDef definition

class InstanceIdentityTypeDef(TypedDict):
    Document: NotRequired[str],
    Signature: NotRequired[str],
```

## ReportedOsTypeDef

```python
# ReportedOsTypeDef definition

class ReportedOsTypeDef(TypedDict):
    Family: NotRequired[str],
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## InstancesCountTypeDef

```python
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
# ShutdownEventConfigurationTypeDef definition

class ShutdownEventConfigurationTypeDef(TypedDict):
    ExecutionTimeout: NotRequired[int],
    DelayUntilElbConnectionsDrained: NotRequired[bool],
```

## ListTagsRequestRequestTypeDef

```python
# ListTagsRequestRequestTypeDef definition

class ListTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## OperatingSystemConfigurationManagerTypeDef

```python
# OperatingSystemConfigurationManagerTypeDef definition

class OperatingSystemConfigurationManagerTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## RebootInstanceRequestRequestTypeDef

```python
# RebootInstanceRequestRequestTypeDef definition

class RebootInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
```

## RegisterEcsClusterRequestRequestTypeDef

```python
# RegisterEcsClusterRequestRequestTypeDef definition

class RegisterEcsClusterRequestRequestTypeDef(TypedDict):
    EcsClusterArn: str,
    StackId: str,
```

## RegisterElasticIpRequestRequestTypeDef

```python
# RegisterElasticIpRequestRequestTypeDef definition

class RegisterElasticIpRequestRequestTypeDef(TypedDict):
    ElasticIp: str,
    StackId: str,
```

## RegisterRdsDbInstanceRequestRequestTypeDef

```python
# RegisterRdsDbInstanceRequestRequestTypeDef definition

class RegisterRdsDbInstanceRequestRequestTypeDef(TypedDict):
    StackId: str,
    RdsDbInstanceArn: str,
    DbUser: str,
    DbPassword: str,
```

## RegisterVolumeRequestRequestTypeDef

```python
# RegisterVolumeRequestRequestTypeDef definition

class RegisterVolumeRequestRequestTypeDef(TypedDict):
    StackId: str,
    Ec2VolumeId: NotRequired[str],
```

## SetPermissionRequestRequestTypeDef

```python
# SetPermissionRequestRequestTypeDef definition

class SetPermissionRequestRequestTypeDef(TypedDict):
    StackId: str,
    IamUserArn: str,
    AllowSsh: NotRequired[bool],
    AllowSudo: NotRequired[bool],
    Level: NotRequired[str],
```

## WeeklyAutoScalingScheduleTypeDef

```python
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

## StartInstanceRequestRequestTypeDef

```python
# StartInstanceRequestRequestTypeDef definition

class StartInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
```

## StartStackRequestRequestTypeDef

```python
# StartStackRequestRequestTypeDef definition

class StartStackRequestRequestTypeDef(TypedDict):
    StackId: str,
```

## StopInstanceRequestRequestTypeDef

```python
# StopInstanceRequestRequestTypeDef definition

class StopInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    Force: NotRequired[bool],
```

## StopStackRequestRequestTypeDef

```python
# StopStackRequestRequestTypeDef definition

class StopStackRequestRequestTypeDef(TypedDict):
    StackId: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## WeeklyAutoScalingScheduleOutputTypeDef

```python
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

## UnassignInstanceRequestRequestTypeDef

```python
# UnassignInstanceRequestRequestTypeDef definition

class UnassignInstanceRequestRequestTypeDef(TypedDict):
    InstanceId: str,
```

## UnassignVolumeRequestRequestTypeDef

```python
# UnassignVolumeRequestRequestTypeDef definition

class UnassignVolumeRequestRequestTypeDef(TypedDict):
    VolumeId: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateElasticIpRequestRequestTypeDef

```python
# UpdateElasticIpRequestRequestTypeDef definition

class UpdateElasticIpRequestRequestTypeDef(TypedDict):
    ElasticIp: str,
    Name: NotRequired[str],
```

## UpdateInstanceRequestRequestTypeDef

```python
# UpdateInstanceRequestRequestTypeDef definition

class UpdateInstanceRequestRequestTypeDef(TypedDict):
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
## UpdateMyUserProfileRequestRequestTypeDef

```python
# UpdateMyUserProfileRequestRequestTypeDef definition

class UpdateMyUserProfileRequestRequestTypeDef(TypedDict):
    SshPublicKey: NotRequired[str],
```

## UpdateRdsDbInstanceRequestRequestTypeDef

```python
# UpdateRdsDbInstanceRequestRequestTypeDef definition

class UpdateRdsDbInstanceRequestRequestTypeDef(TypedDict):
    RdsDbInstanceArn: str,
    DbUser: NotRequired[str],
    DbPassword: NotRequired[str],
```

## UpdateUserProfileRequestRequestTypeDef

```python
# UpdateUserProfileRequestRequestTypeDef definition

class UpdateUserProfileRequestRequestTypeDef(TypedDict):
    IamUserArn: str,
    SshUsername: NotRequired[str],
    SshPublicKey: NotRequired[str],
    AllowSelfManagement: NotRequired[bool],
```

## UpdateVolumeRequestRequestTypeDef

```python
# UpdateVolumeRequestRequestTypeDef definition

class UpdateVolumeRequestRequestTypeDef(TypedDict):
    VolumeId: str,
    Name: NotRequired[str],
    MountPoint: NotRequired[str],
```

## AgentVersionTypeDef

```python
# AgentVersionTypeDef definition

class AgentVersionTypeDef(TypedDict):
    Version: NotRequired[str],
    ConfigurationManager: NotRequired[StackConfigurationManagerTypeDef],  # (1)
```

1. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
## DescribeAgentVersionsRequestRequestTypeDef

```python
# DescribeAgentVersionsRequestRequestTypeDef definition

class DescribeAgentVersionsRequestRequestTypeDef(TypedDict):
    StackId: NotRequired[str],
    ConfigurationManager: NotRequired[StackConfigurationManagerTypeDef],  # (1)
```

1. See [:material-code-braces: StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef) 
## AppTypeDef

```python
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
## CreateAppRequestRequestTypeDef

```python
# CreateAppRequestRequestTypeDef definition

class CreateAppRequestRequestTypeDef(TypedDict):
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
## UpdateAppRequestRequestTypeDef

```python
# UpdateAppRequestRequestTypeDef definition

class UpdateAppRequestRequestTypeDef(TypedDict):
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
# LoadBasedAutoScalingConfigurationTypeDef definition

class LoadBasedAutoScalingConfigurationTypeDef(TypedDict):
    LayerId: NotRequired[str],
    Enable: NotRequired[bool],
    UpScaling: NotRequired[AutoScalingThresholdsOutputTypeDef],  # (1)
    DownScaling: NotRequired[AutoScalingThresholdsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingThresholdsOutputTypeDef](./type_defs.md#autoscalingthresholdsoutputtypedef) 
2. See [:material-code-braces: AutoScalingThresholdsOutputTypeDef](./type_defs.md#autoscalingthresholdsoutputtypedef) 
## SetLoadBasedAutoScalingRequestRequestTypeDef

```python
# SetLoadBasedAutoScalingRequestRequestTypeDef definition

class SetLoadBasedAutoScalingRequestRequestTypeDef(TypedDict):
    LayerId: str,
    Enable: NotRequired[bool],
    UpScaling: NotRequired[AutoScalingThresholdsTypeDef],  # (1)
    DownScaling: NotRequired[AutoScalingThresholdsTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingThresholdsTypeDef](./type_defs.md#autoscalingthresholdstypedef) 
2. See [:material-code-braces: AutoScalingThresholdsTypeDef](./type_defs.md#autoscalingthresholdstypedef) 
## BlockDeviceMappingTypeDef

```python
# BlockDeviceMappingTypeDef definition

class BlockDeviceMappingTypeDef(TypedDict):
    DeviceName: NotRequired[str],
    NoDevice: NotRequired[str],
    VirtualName: NotRequired[str],
    Ebs: NotRequired[EbsBlockDeviceTypeDef],  # (1)
```

1. See [:material-code-braces: EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef) 
## CloneStackRequestRequestTypeDef

```python
# CloneStackRequestRequestTypeDef definition

class CloneStackRequestRequestTypeDef(TypedDict):
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
## CreateStackRequestRequestTypeDef

```python
# CreateStackRequestRequestTypeDef definition

class CreateStackRequestRequestTypeDef(TypedDict):
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
## CreateStackRequestServiceResourceCreateStackTypeDef

```python
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
## StackTypeDef

```python
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
## UpdateStackRequestRequestTypeDef

```python
# UpdateStackRequestRequestTypeDef definition

class UpdateStackRequestRequestTypeDef(TypedDict):
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
# CloneStackResultTypeDef definition

class CloneStackResultTypeDef(TypedDict):
    StackId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppResultTypeDef

```python
# CreateAppResultTypeDef definition

class CreateAppResultTypeDef(TypedDict):
    AppId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentResultTypeDef

```python
# CreateDeploymentResultTypeDef definition

class CreateDeploymentResultTypeDef(TypedDict):
    DeploymentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceResultTypeDef

```python
# CreateInstanceResultTypeDef definition

class CreateInstanceResultTypeDef(TypedDict):
    InstanceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLayerResultTypeDef

```python
# CreateLayerResultTypeDef definition

class CreateLayerResultTypeDef(TypedDict):
    LayerId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStackResultTypeDef

```python
# CreateStackResultTypeDef definition

class CreateStackResultTypeDef(TypedDict):
    StackId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserProfileResultTypeDef

```python
# CreateUserProfileResultTypeDef definition

class CreateUserProfileResultTypeDef(TypedDict):
    IamUserArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStackProvisioningParametersResultTypeDef

```python
# DescribeStackProvisioningParametersResultTypeDef definition

class DescribeStackProvisioningParametersResultTypeDef(TypedDict):
    AgentInstallerUrl: str,
    Parameters: Dict[str, str],
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
## GetHostnameSuggestionResultTypeDef

```python
# GetHostnameSuggestionResultTypeDef definition

class GetHostnameSuggestionResultTypeDef(TypedDict):
    LayerId: str,
    Hostname: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsResultTypeDef

```python
# ListTagsResultTypeDef definition

class ListTagsResultTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterEcsClusterResultTypeDef

```python
# RegisterEcsClusterResultTypeDef definition

class RegisterEcsClusterResultTypeDef(TypedDict):
    EcsClusterArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterElasticIpResultTypeDef

```python
# RegisterElasticIpResultTypeDef definition

class RegisterElasticIpResultTypeDef(TypedDict):
    ElasticIp: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterInstanceResultTypeDef

```python
# RegisterInstanceResultTypeDef definition

class RegisterInstanceResultTypeDef(TypedDict):
    InstanceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterVolumeResultTypeDef

```python
# RegisterVolumeResultTypeDef definition

class RegisterVolumeResultTypeDef(TypedDict):
    VolumeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CloudWatchLogsConfigurationOutputTypeDef

```python
# CloudWatchLogsConfigurationOutputTypeDef definition

class CloudWatchLogsConfigurationOutputTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    LogStreams: NotRequired[List[CloudWatchLogsLogStreamTypeDef]],  # (1)
```

1. See [:material-code-braces: CloudWatchLogsLogStreamTypeDef](./type_defs.md#cloudwatchlogslogstreamtypedef) 
## CloudWatchLogsConfigurationTypeDef

```python
# CloudWatchLogsConfigurationTypeDef definition

class CloudWatchLogsConfigurationTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    LogStreams: NotRequired[Sequence[CloudWatchLogsLogStreamTypeDef]],  # (1)
```

1. See [:material-code-braces: CloudWatchLogsLogStreamTypeDef](./type_defs.md#cloudwatchlogslogstreamtypedef) 
## DescribeCommandsResultTypeDef

```python
# DescribeCommandsResultTypeDef definition

class DescribeCommandsResultTypeDef(TypedDict):
    Commands: List[CommandTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommandTypeDef](./type_defs.md#commandtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentRequestRequestTypeDef

```python
# CreateDeploymentRequestRequestTypeDef definition

class CreateDeploymentRequestRequestTypeDef(TypedDict):
    StackId: str,
    Command: DeploymentCommandTypeDef,  # (1)
    AppId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
    LayerIds: NotRequired[Sequence[str]],
    Comment: NotRequired[str],
    CustomJson: NotRequired[str],
```

1. See [:material-code-braces: DeploymentCommandTypeDef](./type_defs.md#deploymentcommandtypedef) 
## DeploymentTypeDef

```python
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
## DescribeAppsRequestAppExistsWaitTypeDef

```python
# DescribeAppsRequestAppExistsWaitTypeDef definition

class DescribeAppsRequestAppExistsWaitTypeDef(TypedDict):
    StackId: NotRequired[str],
    AppIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef

```python
# DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef definition

class DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef(TypedDict):
    StackId: NotRequired[str],
    AppId: NotRequired[str],
    DeploymentIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInstancesRequestInstanceOnlineWaitTypeDef

```python
# DescribeInstancesRequestInstanceOnlineWaitTypeDef definition

class DescribeInstancesRequestInstanceOnlineWaitTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInstancesRequestInstanceRegisteredWaitTypeDef

```python
# DescribeInstancesRequestInstanceRegisteredWaitTypeDef definition

class DescribeInstancesRequestInstanceRegisteredWaitTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInstancesRequestInstanceStoppedWaitTypeDef

```python
# DescribeInstancesRequestInstanceStoppedWaitTypeDef definition

class DescribeInstancesRequestInstanceStoppedWaitTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInstancesRequestInstanceTerminatedWaitTypeDef

```python
# DescribeInstancesRequestInstanceTerminatedWaitTypeDef definition

class DescribeInstancesRequestInstanceTerminatedWaitTypeDef(TypedDict):
    StackId: NotRequired[str],
    LayerId: NotRequired[str],
    InstanceIds: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef

```python
# DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef definition

class DescribeEcsClustersRequestDescribeEcsClustersPaginateTypeDef(TypedDict):
    EcsClusterArns: NotRequired[Sequence[str]],
    StackId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEcsClustersResultTypeDef

```python
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
# DescribeElasticIpsResultTypeDef definition

class DescribeElasticIpsResultTypeDef(TypedDict):
    ElasticIps: List[ElasticIpTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ElasticIpTypeDef](./type_defs.md#elasticiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeElasticLoadBalancersResultTypeDef

```python
# DescribeElasticLoadBalancersResultTypeDef definition

class DescribeElasticLoadBalancersResultTypeDef(TypedDict):
    ElasticLoadBalancers: List[ElasticLoadBalancerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ElasticLoadBalancerTypeDef](./type_defs.md#elasticloadbalancertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMyUserProfileResultTypeDef

```python
# DescribeMyUserProfileResultTypeDef definition

class DescribeMyUserProfileResultTypeDef(TypedDict):
    UserProfile: SelfUserProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SelfUserProfileTypeDef](./type_defs.md#selfuserprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePermissionsResultTypeDef

```python
# DescribePermissionsResultTypeDef definition

class DescribePermissionsResultTypeDef(TypedDict):
    Permissions: List[PermissionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionTypeDef](./type_defs.md#permissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRaidArraysResultTypeDef

```python
# DescribeRaidArraysResultTypeDef definition

class DescribeRaidArraysResultTypeDef(TypedDict):
    RaidArrays: List[RaidArrayTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RaidArrayTypeDef](./type_defs.md#raidarraytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRdsDbInstancesResultTypeDef

```python
# DescribeRdsDbInstancesResultTypeDef definition

class DescribeRdsDbInstancesResultTypeDef(TypedDict):
    RdsDbInstances: List[RdsDbInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RdsDbInstanceTypeDef](./type_defs.md#rdsdbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeServiceErrorsResultTypeDef

```python
# DescribeServiceErrorsResultTypeDef definition

class DescribeServiceErrorsResultTypeDef(TypedDict):
    ServiceErrors: List[ServiceErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceErrorTypeDef](./type_defs.md#serviceerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserProfilesResultTypeDef

```python
# DescribeUserProfilesResultTypeDef definition

class DescribeUserProfilesResultTypeDef(TypedDict):
    UserProfiles: List[UserProfileTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserProfileTypeDef](./type_defs.md#userprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVolumesResultTypeDef

```python
# DescribeVolumesResultTypeDef definition

class DescribeVolumesResultTypeDef(TypedDict):
    Volumes: List[VolumeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GrantAccessResultTypeDef

```python
# GrantAccessResultTypeDef definition

class GrantAccessResultTypeDef(TypedDict):
    TemporaryCredential: TemporaryCredentialTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemporaryCredentialTypeDef](./type_defs.md#temporarycredentialtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterInstanceRequestRequestTypeDef

```python
# RegisterInstanceRequestRequestTypeDef definition

class RegisterInstanceRequestRequestTypeDef(TypedDict):
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
# LifecycleEventConfigurationTypeDef definition

class LifecycleEventConfigurationTypeDef(TypedDict):
    Shutdown: NotRequired[ShutdownEventConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ShutdownEventConfigurationTypeDef](./type_defs.md#shutdowneventconfigurationtypedef) 
## OperatingSystemTypeDef

```python
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
## SetTimeBasedAutoScalingRequestRequestTypeDef

```python
# SetTimeBasedAutoScalingRequestRequestTypeDef definition

class SetTimeBasedAutoScalingRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    AutoScalingSchedule: NotRequired[WeeklyAutoScalingScheduleTypeDef],  # (1)
```

1. See [:material-code-braces: WeeklyAutoScalingScheduleTypeDef](./type_defs.md#weeklyautoscalingscheduletypedef) 
## TimeBasedAutoScalingConfigurationTypeDef

```python
# TimeBasedAutoScalingConfigurationTypeDef definition

class TimeBasedAutoScalingConfigurationTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    AutoScalingSchedule: NotRequired[WeeklyAutoScalingScheduleOutputTypeDef],  # (1)
```

1. See [:material-code-braces: WeeklyAutoScalingScheduleOutputTypeDef](./type_defs.md#weeklyautoscalingscheduleoutputtypedef) 
## DescribeAgentVersionsResultTypeDef

```python
# DescribeAgentVersionsResultTypeDef definition

class DescribeAgentVersionsResultTypeDef(TypedDict):
    AgentVersions: List[AgentVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentVersionTypeDef](./type_defs.md#agentversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppsResultTypeDef

```python
# DescribeAppsResultTypeDef definition

class DescribeAppsResultTypeDef(TypedDict):
    Apps: List[AppTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLoadBasedAutoScalingResultTypeDef

```python
# DescribeLoadBasedAutoScalingResultTypeDef definition

class DescribeLoadBasedAutoScalingResultTypeDef(TypedDict):
    LoadBasedAutoScalingConfigurations: List[LoadBasedAutoScalingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBasedAutoScalingConfigurationTypeDef](./type_defs.md#loadbasedautoscalingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceRequestRequestTypeDef

```python
# CreateInstanceRequestRequestTypeDef definition

class CreateInstanceRequestRequestTypeDef(TypedDict):
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
# DescribeStacksResultTypeDef definition

class DescribeStacksResultTypeDef(TypedDict):
    Stacks: List[StackTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StackTypeDef](./type_defs.md#stacktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDeploymentsResultTypeDef

```python
# DescribeDeploymentsResultTypeDef definition

class DescribeDeploymentsResultTypeDef(TypedDict):
    Deployments: List[DeploymentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStackSummaryResultTypeDef

```python
# DescribeStackSummaryResultTypeDef definition

class DescribeStackSummaryResultTypeDef(TypedDict):
    StackSummary: StackSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StackSummaryTypeDef](./type_defs.md#stacksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLayerRequestRequestTypeDef

```python
# CreateLayerRequestRequestTypeDef definition

class CreateLayerRequestRequestTypeDef(TypedDict):
    StackId: str,
    Type: LayerTypeType,  # (1)
    Name: str,
    Shortname: str,
    Attributes: NotRequired[Mapping[LayerAttributesKeysType, str]],  # (2)
    CloudWatchLogsConfiguration: NotRequired[CloudWatchLogsConfigurationTypeDef],  # (3)
    CustomInstanceProfileArn: NotRequired[str],
    CustomJson: NotRequired[str],
    CustomSecurityGroupIds: NotRequired[Sequence[str]],
    Packages: NotRequired[Sequence[str]],
    VolumeConfigurations: NotRequired[Sequence[VolumeConfigurationTypeDef]],  # (4)
    EnableAutoHealing: NotRequired[bool],
    AutoAssignElasticIps: NotRequired[bool],
    AutoAssignPublicIps: NotRequired[bool],
    CustomRecipes: NotRequired[RecipesTypeDef],  # (5)
    InstallUpdatesOnBoot: NotRequired[bool],
    UseEbsOptimizedInstances: NotRequired[bool],
    LifecycleEventConfiguration: NotRequired[LifecycleEventConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: LayerTypeType](./literals.md#layertypetype) 
2. See [:material-code-brackets: LayerAttributesKeysType](./literals.md#layerattributeskeystype) 
3. See [:material-code-braces: CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef) 
4. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
5. See [:material-code-braces: RecipesTypeDef](./type_defs.md#recipestypedef) 
6. See [:material-code-braces: LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef) 
## CreateLayerRequestStackCreateLayerTypeDef

```python
# CreateLayerRequestStackCreateLayerTypeDef definition

class CreateLayerRequestStackCreateLayerTypeDef(TypedDict):
    Type: LayerTypeType,  # (1)
    Name: str,
    Shortname: str,
    Attributes: NotRequired[Mapping[LayerAttributesKeysType, str]],  # (2)
    CloudWatchLogsConfiguration: NotRequired[CloudWatchLogsConfigurationTypeDef],  # (3)
    CustomInstanceProfileArn: NotRequired[str],
    CustomJson: NotRequired[str],
    CustomSecurityGroupIds: NotRequired[Sequence[str]],
    Packages: NotRequired[Sequence[str]],
    VolumeConfigurations: NotRequired[Sequence[VolumeConfigurationTypeDef]],  # (4)
    EnableAutoHealing: NotRequired[bool],
    AutoAssignElasticIps: NotRequired[bool],
    AutoAssignPublicIps: NotRequired[bool],
    CustomRecipes: NotRequired[RecipesTypeDef],  # (5)
    InstallUpdatesOnBoot: NotRequired[bool],
    UseEbsOptimizedInstances: NotRequired[bool],
    LifecycleEventConfiguration: NotRequired[LifecycleEventConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: LayerTypeType](./literals.md#layertypetype) 
2. See [:material-code-brackets: LayerAttributesKeysType](./literals.md#layerattributeskeystype) 
3. See [:material-code-braces: CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef) 
4. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
5. See [:material-code-braces: RecipesTypeDef](./type_defs.md#recipestypedef) 
6. See [:material-code-braces: LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef) 
## LayerTypeDef

```python
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
## UpdateLayerRequestRequestTypeDef

```python
# UpdateLayerRequestRequestTypeDef definition

class UpdateLayerRequestRequestTypeDef(TypedDict):
    LayerId: str,
    Name: NotRequired[str],
    Shortname: NotRequired[str],
    Attributes: NotRequired[Mapping[LayerAttributesKeysType, str]],  # (1)
    CloudWatchLogsConfiguration: NotRequired[CloudWatchLogsConfigurationTypeDef],  # (2)
    CustomInstanceProfileArn: NotRequired[str],
    CustomJson: NotRequired[str],
    CustomSecurityGroupIds: NotRequired[Sequence[str]],
    Packages: NotRequired[Sequence[str]],
    VolumeConfigurations: NotRequired[Sequence[VolumeConfigurationTypeDef]],  # (3)
    EnableAutoHealing: NotRequired[bool],
    AutoAssignElasticIps: NotRequired[bool],
    AutoAssignPublicIps: NotRequired[bool],
    CustomRecipes: NotRequired[RecipesTypeDef],  # (4)
    InstallUpdatesOnBoot: NotRequired[bool],
    UseEbsOptimizedInstances: NotRequired[bool],
    LifecycleEventConfiguration: NotRequired[LifecycleEventConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: LayerAttributesKeysType](./literals.md#layerattributeskeystype) 
2. See [:material-code-braces: CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef) 
3. See [:material-code-braces: VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef) 
4. See [:material-code-braces: RecipesTypeDef](./type_defs.md#recipestypedef) 
5. See [:material-code-braces: LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef) 
## DescribeOperatingSystemsResponseTypeDef

```python
# DescribeOperatingSystemsResponseTypeDef definition

class DescribeOperatingSystemsResponseTypeDef(TypedDict):
    OperatingSystems: List[OperatingSystemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperatingSystemTypeDef](./type_defs.md#operatingsystemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTimeBasedAutoScalingResultTypeDef

```python
# DescribeTimeBasedAutoScalingResultTypeDef definition

class DescribeTimeBasedAutoScalingResultTypeDef(TypedDict):
    TimeBasedAutoScalingConfigurations: List[TimeBasedAutoScalingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TimeBasedAutoScalingConfigurationTypeDef](./type_defs.md#timebasedautoscalingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstancesResultTypeDef

```python
# DescribeInstancesResultTypeDef definition

class DescribeInstancesResultTypeDef(TypedDict):
    Instances: List[InstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLayersResultTypeDef

```python
# DescribeLayersResultTypeDef definition

class DescribeLayersResultTypeDef(TypedDict):
    Layers: List[LayerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LayerTypeDef](./type_defs.md#layertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
