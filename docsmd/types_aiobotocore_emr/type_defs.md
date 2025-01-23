# Type definitions

> [Index](../README.md) > [EMR](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EMR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#emr)
    type annotations stubs module [types-aiobotocore-emr](https://pypi.org/project/types-aiobotocore-emr/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ApplicationUnionTypeDef

```python
# ApplicationUnionTypeDef definition

ApplicationUnionTypeDef = Union[
    ApplicationTypeDef,  # (1)
    ApplicationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef) 

## ConfigurationUnionTypeDef

```python
# ConfigurationUnionTypeDef definition

ConfigurationUnionTypeDef = Union[
    ConfigurationTypeDef,  # (1)
    ConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 

## InstanceResizePolicyUnionTypeDef

```python
# InstanceResizePolicyUnionTypeDef definition

InstanceResizePolicyUnionTypeDef = Union[
    InstanceResizePolicyTypeDef,  # (1)
    InstanceResizePolicyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InstanceResizePolicyTypeDef](./type_defs.md#instanceresizepolicytypedef) 
2. See [:material-code-braces: InstanceResizePolicyOutputTypeDef](./type_defs.md#instanceresizepolicyoutputtypedef) 

## PlacementTypeUnionTypeDef

```python
# PlacementTypeUnionTypeDef definition

PlacementTypeUnionTypeDef = Union[
    PlacementTypeTypeDef,  # (1)
    PlacementTypeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PlacementTypeTypeDef](./type_defs.md#placementtypetypedef) 
2. See [:material-code-braces: PlacementTypeOutputTypeDef](./type_defs.md#placementtypeoutputtypedef) 

## ScriptBootstrapActionConfigUnionTypeDef

```python
# ScriptBootstrapActionConfigUnionTypeDef definition

ScriptBootstrapActionConfigUnionTypeDef = Union[
    ScriptBootstrapActionConfigTypeDef,  # (1)
    ScriptBootstrapActionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScriptBootstrapActionConfigTypeDef](./type_defs.md#scriptbootstrapactionconfigtypedef) 
2. See [:material-code-braces: ScriptBootstrapActionConfigOutputTypeDef](./type_defs.md#scriptbootstrapactionconfigoutputtypedef) 

## CloudWatchAlarmDefinitionUnionTypeDef

```python
# CloudWatchAlarmDefinitionUnionTypeDef definition

CloudWatchAlarmDefinitionUnionTypeDef = Union[
    CloudWatchAlarmDefinitionTypeDef,  # (1)
    CloudWatchAlarmDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CloudWatchAlarmDefinitionTypeDef](./type_defs.md#cloudwatchalarmdefinitiontypedef) 
2. See [:material-code-braces: CloudWatchAlarmDefinitionOutputTypeDef](./type_defs.md#cloudwatchalarmdefinitionoutputtypedef) 

## HadoopJarStepConfigUnionTypeDef

```python
# HadoopJarStepConfigUnionTypeDef definition

HadoopJarStepConfigUnionTypeDef = Union[
    HadoopJarStepConfigTypeDef,  # (1)
    HadoopJarStepConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HadoopJarStepConfigTypeDef](./type_defs.md#hadoopjarstepconfigtypedef) 
2. See [:material-code-braces: HadoopJarStepConfigOutputTypeDef](./type_defs.md#hadoopjarstepconfigoutputtypedef) 

## ShrinkPolicyUnionTypeDef

```python
# ShrinkPolicyUnionTypeDef definition

ShrinkPolicyUnionTypeDef = Union[
    ShrinkPolicyTypeDef,  # (1)
    ShrinkPolicyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ShrinkPolicyTypeDef](./type_defs.md#shrinkpolicytypedef) 
2. See [:material-code-braces: ShrinkPolicyOutputTypeDef](./type_defs.md#shrinkpolicyoutputtypedef) 

## BootstrapActionConfigUnionTypeDef

```python
# BootstrapActionConfigUnionTypeDef definition

BootstrapActionConfigUnionTypeDef = Union[
    BootstrapActionConfigTypeDef,  # (1)
    BootstrapActionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BootstrapActionConfigTypeDef](./type_defs.md#bootstrapactionconfigtypedef) 
2. See [:material-code-braces: BootstrapActionConfigOutputTypeDef](./type_defs.md#bootstrapactionconfigoutputtypedef) 

## ScalingTriggerUnionTypeDef

```python
# ScalingTriggerUnionTypeDef definition

ScalingTriggerUnionTypeDef = Union[
    ScalingTriggerTypeDef,  # (1)
    ScalingTriggerOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScalingTriggerTypeDef](./type_defs.md#scalingtriggertypedef) 
2. See [:material-code-braces: ScalingTriggerOutputTypeDef](./type_defs.md#scalingtriggeroutputtypedef) 

## StepConfigUnionTypeDef

```python
# StepConfigUnionTypeDef definition

StepConfigUnionTypeDef = Union[
    StepConfigTypeDef,  # (1)
    StepConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StepConfigTypeDef](./type_defs.md#stepconfigtypedef) 
2. See [:material-code-braces: StepConfigOutputTypeDef](./type_defs.md#stepconfigoutputtypedef) 

## ScalingRuleUnionTypeDef

```python
# ScalingRuleUnionTypeDef definition

ScalingRuleUnionTypeDef = Union[
    ScalingRuleTypeDef,  # (1)
    ScalingRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScalingRuleTypeDef](./type_defs.md#scalingruletypedef) 
2. See [:material-code-braces: ScalingRuleOutputTypeDef](./type_defs.md#scalingruleoutputtypedef) 



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

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ApplicationOutputTypeDef

```python
# ApplicationOutputTypeDef definition

class ApplicationOutputTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
    Args: NotRequired[List[str]],
    AdditionalInfo: NotRequired[Dict[str, str]],
```

## ApplicationTypeDef

```python
# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
    Args: NotRequired[Sequence[str]],
    AdditionalInfo: NotRequired[Mapping[str, str]],
```

## ScalingConstraintsTypeDef

```python
# ScalingConstraintsTypeDef definition

class ScalingConstraintsTypeDef(TypedDict):
    MinCapacity: int,
    MaxCapacity: int,
```

## AutoScalingPolicyStateChangeReasonTypeDef

```python
# AutoScalingPolicyStateChangeReasonTypeDef definition

class AutoScalingPolicyStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[AutoScalingPolicyStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: AutoScalingPolicyStateChangeReasonCodeType](./literals.md#autoscalingpolicystatechangereasoncodetype) 
## AutoTerminationPolicyTypeDef

```python
# AutoTerminationPolicyTypeDef definition

class AutoTerminationPolicyTypeDef(TypedDict):
    IdleTimeout: NotRequired[int],
```

## BlockPublicAccessConfigurationMetadataTypeDef

```python
# BlockPublicAccessConfigurationMetadataTypeDef definition

class BlockPublicAccessConfigurationMetadataTypeDef(TypedDict):
    CreationDateTime: datetime,
    CreatedByArn: str,
```

## PortRangeTypeDef

```python
# PortRangeTypeDef definition

class PortRangeTypeDef(TypedDict):
    MinRange: int,
    MaxRange: NotRequired[int],
```

## ScriptBootstrapActionConfigOutputTypeDef

```python
# ScriptBootstrapActionConfigOutputTypeDef definition

class ScriptBootstrapActionConfigOutputTypeDef(TypedDict):
    Path: str,
    Args: NotRequired[List[str]],
```

## CancelStepsInfoTypeDef

```python
# CancelStepsInfoTypeDef definition

class CancelStepsInfoTypeDef(TypedDict):
    StepId: NotRequired[str],
    Status: NotRequired[CancelStepsRequestStatusType],  # (1)
    Reason: NotRequired[str],
```

1. See [:material-code-brackets: CancelStepsRequestStatusType](./literals.md#cancelstepsrequeststatustype) 
## CancelStepsInputRequestTypeDef

```python
# CancelStepsInputRequestTypeDef definition

class CancelStepsInputRequestTypeDef(TypedDict):
    ClusterId: str,
    StepIds: Sequence[str],
    StepCancellationOption: NotRequired[StepCancellationOptionType],  # (1)
```

1. See [:material-code-brackets: StepCancellationOptionType](./literals.md#stepcancellationoptiontype) 
## MetricDimensionTypeDef

```python
# MetricDimensionTypeDef definition

class MetricDimensionTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ClusterStateChangeReasonTypeDef

```python
# ClusterStateChangeReasonTypeDef definition

class ClusterStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[ClusterStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: ClusterStateChangeReasonCodeType](./literals.md#clusterstatechangereasoncodetype) 
## ClusterTimelineTypeDef

```python
# ClusterTimelineTypeDef definition

class ClusterTimelineTypeDef(TypedDict):
    CreationDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
```

## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorData: NotRequired[List[Dict[str, str]]],
    ErrorMessage: NotRequired[str],
```

## ConfigurationOutputTypeDef

```python
# ConfigurationOutputTypeDef definition

class ConfigurationOutputTypeDef(TypedDict):
    Classification: NotRequired[str],
    Configurations: NotRequired[List[Dict[str, Any]]],
    Properties: NotRequired[Dict[str, str]],
```

## Ec2InstanceAttributesTypeDef

```python
# Ec2InstanceAttributesTypeDef definition

class Ec2InstanceAttributesTypeDef(TypedDict):
    Ec2KeyName: NotRequired[str],
    Ec2SubnetId: NotRequired[str],
    RequestedEc2SubnetIds: NotRequired[List[str]],
    Ec2AvailabilityZone: NotRequired[str],
    RequestedEc2AvailabilityZones: NotRequired[List[str]],
    IamInstanceProfile: NotRequired[str],
    EmrManagedMasterSecurityGroup: NotRequired[str],
    EmrManagedSlaveSecurityGroup: NotRequired[str],
    ServiceAccessSecurityGroup: NotRequired[str],
    AdditionalMasterSecurityGroups: NotRequired[List[str]],
    AdditionalSlaveSecurityGroups: NotRequired[List[str]],
```

## KerberosAttributesTypeDef

```python
# KerberosAttributesTypeDef definition

class KerberosAttributesTypeDef(TypedDict):
    Realm: str,
    KdcAdminPassword: str,
    CrossRealmTrustPrincipalPassword: NotRequired[str],
    ADDomainJoinUser: NotRequired[str],
    ADDomainJoinPassword: NotRequired[str],
```

## PlacementGroupConfigTypeDef

```python
# PlacementGroupConfigTypeDef definition

class PlacementGroupConfigTypeDef(TypedDict):
    InstanceRole: InstanceRoleTypeType,  # (1)
    PlacementStrategy: NotRequired[PlacementGroupStrategyType],  # (2)
```

1. See [:material-code-brackets: InstanceRoleTypeType](./literals.md#instanceroletypetype) 
2. See [:material-code-brackets: PlacementGroupStrategyType](./literals.md#placementgroupstrategytype) 
## CommandTypeDef

```python
# CommandTypeDef definition

class CommandTypeDef(TypedDict):
    Name: NotRequired[str],
    ScriptPath: NotRequired[str],
    Args: NotRequired[List[str]],
```

## ComputeLimitsTypeDef

```python
# ComputeLimitsTypeDef definition

class ComputeLimitsTypeDef(TypedDict):
    UnitType: ComputeLimitsUnitTypeType,  # (1)
    MinimumCapacityUnits: int,
    MaximumCapacityUnits: int,
    MaximumOnDemandCapacityUnits: NotRequired[int],
    MaximumCoreCapacityUnits: NotRequired[int],
```

1. See [:material-code-brackets: ComputeLimitsUnitTypeType](./literals.md#computelimitsunittypetype) 
## ConfigurationPaginatorTypeDef

```python
# ConfigurationPaginatorTypeDef definition

class ConfigurationPaginatorTypeDef(TypedDict):
    Classification: NotRequired[str],
    Configurations: NotRequired[List[Dict[str, Any]]],
    Properties: NotRequired[Dict[str, str]],
```

## ConfigurationTypeDef

```python
# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    Classification: NotRequired[str],
    Configurations: NotRequired[Sequence[Mapping[str, Any]]],
    Properties: NotRequired[Mapping[str, str]],
```

## CreateSecurityConfigurationInputRequestTypeDef

```python
# CreateSecurityConfigurationInputRequestTypeDef definition

class CreateSecurityConfigurationInputRequestTypeDef(TypedDict):
    Name: str,
    SecurityConfiguration: str,
```

## CreateStudioSessionMappingInputRequestTypeDef

```python
# CreateStudioSessionMappingInputRequestTypeDef definition

class CreateStudioSessionMappingInputRequestTypeDef(TypedDict):
    StudioId: str,
    IdentityType: IdentityTypeType,  # (1)
    SessionPolicyArn: str,
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## UsernamePasswordTypeDef

```python
# UsernamePasswordTypeDef definition

class UsernamePasswordTypeDef(TypedDict):
    Username: NotRequired[str],
    Password: NotRequired[str],
```

## DeleteSecurityConfigurationInputRequestTypeDef

```python
# DeleteSecurityConfigurationInputRequestTypeDef definition

class DeleteSecurityConfigurationInputRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteStudioInputRequestTypeDef

```python
# DeleteStudioInputRequestTypeDef definition

class DeleteStudioInputRequestTypeDef(TypedDict):
    StudioId: str,
```

## DeleteStudioSessionMappingInputRequestTypeDef

```python
# DeleteStudioSessionMappingInputRequestTypeDef definition

class DeleteStudioSessionMappingInputRequestTypeDef(TypedDict):
    StudioId: str,
    IdentityType: IdentityTypeType,  # (1)
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## DescribeClusterInputRequestTypeDef

```python
# DescribeClusterInputRequestTypeDef definition

class DescribeClusterInputRequestTypeDef(TypedDict):
    ClusterId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeNotebookExecutionInputRequestTypeDef

```python
# DescribeNotebookExecutionInputRequestTypeDef definition

class DescribeNotebookExecutionInputRequestTypeDef(TypedDict):
    NotebookExecutionId: str,
```

## DescribeReleaseLabelInputRequestTypeDef

```python
# DescribeReleaseLabelInputRequestTypeDef definition

class DescribeReleaseLabelInputRequestTypeDef(TypedDict):
    ReleaseLabel: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## OSReleaseTypeDef

```python
# OSReleaseTypeDef definition

class OSReleaseTypeDef(TypedDict):
    Label: NotRequired[str],
```

## SimplifiedApplicationTypeDef

```python
# SimplifiedApplicationTypeDef definition

class SimplifiedApplicationTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## DescribeSecurityConfigurationInputRequestTypeDef

```python
# DescribeSecurityConfigurationInputRequestTypeDef definition

class DescribeSecurityConfigurationInputRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeStepInputRequestTypeDef

```python
# DescribeStepInputRequestTypeDef definition

class DescribeStepInputRequestTypeDef(TypedDict):
    ClusterId: str,
    StepId: str,
```

## DescribeStudioInputRequestTypeDef

```python
# DescribeStudioInputRequestTypeDef definition

class DescribeStudioInputRequestTypeDef(TypedDict):
    StudioId: str,
```

## VolumeSpecificationTypeDef

```python
# VolumeSpecificationTypeDef definition

class VolumeSpecificationTypeDef(TypedDict):
    VolumeType: str,
    SizeInGB: int,
    Iops: NotRequired[int],
    Throughput: NotRequired[int],
```

## EbsVolumeTypeDef

```python
# EbsVolumeTypeDef definition

class EbsVolumeTypeDef(TypedDict):
    Device: NotRequired[str],
    VolumeId: NotRequired[str],
```

## ExecutionEngineConfigTypeDef

```python
# ExecutionEngineConfigTypeDef definition

class ExecutionEngineConfigTypeDef(TypedDict):
    Id: str,
    Type: NotRequired[ExecutionEngineTypeType],  # (1)
    MasterInstanceSecurityGroupId: NotRequired[str],
    ExecutionRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: ExecutionEngineTypeType](./literals.md#executionenginetypetype) 
## FailureDetailsTypeDef

```python
# FailureDetailsTypeDef definition

class FailureDetailsTypeDef(TypedDict):
    Reason: NotRequired[str],
    Message: NotRequired[str],
    LogFile: NotRequired[str],
```

## GetAutoTerminationPolicyInputRequestTypeDef

```python
# GetAutoTerminationPolicyInputRequestTypeDef definition

class GetAutoTerminationPolicyInputRequestTypeDef(TypedDict):
    ClusterId: str,
```

## GetClusterSessionCredentialsInputRequestTypeDef

```python
# GetClusterSessionCredentialsInputRequestTypeDef definition

class GetClusterSessionCredentialsInputRequestTypeDef(TypedDict):
    ClusterId: str,
    ExecutionRoleArn: NotRequired[str],
```

## GetManagedScalingPolicyInputRequestTypeDef

```python
# GetManagedScalingPolicyInputRequestTypeDef definition

class GetManagedScalingPolicyInputRequestTypeDef(TypedDict):
    ClusterId: str,
```

## GetStudioSessionMappingInputRequestTypeDef

```python
# GetStudioSessionMappingInputRequestTypeDef definition

class GetStudioSessionMappingInputRequestTypeDef(TypedDict):
    StudioId: str,
    IdentityType: IdentityTypeType,  # (1)
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## SessionMappingDetailTypeDef

```python
# SessionMappingDetailTypeDef definition

class SessionMappingDetailTypeDef(TypedDict):
    StudioId: NotRequired[str],
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    SessionPolicyArn: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## KeyValueTypeDef

```python
# KeyValueTypeDef definition

class KeyValueTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## HadoopStepConfigTypeDef

```python
# HadoopStepConfigTypeDef definition

class HadoopStepConfigTypeDef(TypedDict):
    Jar: NotRequired[str],
    Properties: NotRequired[Dict[str, str]],
    MainClass: NotRequired[str],
    Args: NotRequired[List[str]],
```

## SpotProvisioningSpecificationTypeDef

```python
# SpotProvisioningSpecificationTypeDef definition

class SpotProvisioningSpecificationTypeDef(TypedDict):
    TimeoutDurationMinutes: int,
    TimeoutAction: SpotProvisioningTimeoutActionType,  # (1)
    BlockDurationMinutes: NotRequired[int],
    AllocationStrategy: NotRequired[SpotProvisioningAllocationStrategyType],  # (2)
```

1. See [:material-code-brackets: SpotProvisioningTimeoutActionType](./literals.md#spotprovisioningtimeoutactiontype) 
2. See [:material-code-brackets: SpotProvisioningAllocationStrategyType](./literals.md#spotprovisioningallocationstrategytype) 
## SpotResizingSpecificationTypeDef

```python
# SpotResizingSpecificationTypeDef definition

class SpotResizingSpecificationTypeDef(TypedDict):
    TimeoutDurationMinutes: NotRequired[int],
    AllocationStrategy: NotRequired[SpotProvisioningAllocationStrategyType],  # (1)
```

1. See [:material-code-brackets: SpotProvisioningAllocationStrategyType](./literals.md#spotprovisioningallocationstrategytype) 
## InstanceFleetStateChangeReasonTypeDef

```python
# InstanceFleetStateChangeReasonTypeDef definition

class InstanceFleetStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[InstanceFleetStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: InstanceFleetStateChangeReasonCodeType](./literals.md#instancefleetstatechangereasoncodetype) 
## InstanceFleetTimelineTypeDef

```python
# InstanceFleetTimelineTypeDef definition

class InstanceFleetTimelineTypeDef(TypedDict):
    CreationDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
```

## InstanceGroupDetailTypeDef

```python
# InstanceGroupDetailTypeDef definition

class InstanceGroupDetailTypeDef(TypedDict):
    Market: MarketTypeType,  # (1)
    InstanceRole: InstanceRoleTypeType,  # (2)
    InstanceType: str,
    InstanceRequestCount: int,
    InstanceRunningCount: int,
    State: InstanceGroupStateType,  # (3)
    CreationDateTime: datetime,
    InstanceGroupId: NotRequired[str],
    Name: NotRequired[str],
    BidPrice: NotRequired[str],
    LastStateChangeReason: NotRequired[str],
    StartDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
    CustomAmiId: NotRequired[str],
```

1. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
2. See [:material-code-brackets: InstanceRoleTypeType](./literals.md#instanceroletypetype) 
3. See [:material-code-brackets: InstanceGroupStateType](./literals.md#instancegroupstatetype) 
## InstanceGroupStateChangeReasonTypeDef

```python
# InstanceGroupStateChangeReasonTypeDef definition

class InstanceGroupStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[InstanceGroupStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: InstanceGroupStateChangeReasonCodeType](./literals.md#instancegroupstatechangereasoncodetype) 
## InstanceGroupTimelineTypeDef

```python
# InstanceGroupTimelineTypeDef definition

class InstanceGroupTimelineTypeDef(TypedDict):
    CreationDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
```

## InstanceResizePolicyOutputTypeDef

```python
# InstanceResizePolicyOutputTypeDef definition

class InstanceResizePolicyOutputTypeDef(TypedDict):
    InstancesToTerminate: NotRequired[List[str]],
    InstancesToProtect: NotRequired[List[str]],
    InstanceTerminationTimeout: NotRequired[int],
```

## InstanceResizePolicyTypeDef

```python
# InstanceResizePolicyTypeDef definition

class InstanceResizePolicyTypeDef(TypedDict):
    InstancesToTerminate: NotRequired[Sequence[str]],
    InstancesToProtect: NotRequired[Sequence[str]],
    InstanceTerminationTimeout: NotRequired[int],
```

## InstanceStateChangeReasonTypeDef

```python
# InstanceStateChangeReasonTypeDef definition

class InstanceStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[InstanceStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: InstanceStateChangeReasonCodeType](./literals.md#instancestatechangereasoncodetype) 
## InstanceTimelineTypeDef

```python
# InstanceTimelineTypeDef definition

class InstanceTimelineTypeDef(TypedDict):
    CreationDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
```

## JobFlowExecutionStatusDetailTypeDef

```python
# JobFlowExecutionStatusDetailTypeDef definition

class JobFlowExecutionStatusDetailTypeDef(TypedDict):
    State: JobFlowExecutionStateType,  # (1)
    CreationDateTime: datetime,
    StartDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
    LastStateChangeReason: NotRequired[str],
```

1. See [:material-code-brackets: JobFlowExecutionStateType](./literals.md#jobflowexecutionstatetype) 
## PlacementTypeOutputTypeDef

```python
# PlacementTypeOutputTypeDef definition

class PlacementTypeOutputTypeDef(TypedDict):
    AvailabilityZone: NotRequired[str],
    AvailabilityZones: NotRequired[List[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBootstrapActionsInputRequestTypeDef

```python
# ListBootstrapActionsInputRequestTypeDef definition

class ListBootstrapActionsInputRequestTypeDef(TypedDict):
    ClusterId: str,
    Marker: NotRequired[str],
```

## ListInstanceFleetsInputRequestTypeDef

```python
# ListInstanceFleetsInputRequestTypeDef definition

class ListInstanceFleetsInputRequestTypeDef(TypedDict):
    ClusterId: str,
    Marker: NotRequired[str],
```

## ListInstanceGroupsInputRequestTypeDef

```python
# ListInstanceGroupsInputRequestTypeDef definition

class ListInstanceGroupsInputRequestTypeDef(TypedDict):
    ClusterId: str,
    Marker: NotRequired[str],
```

## ListInstancesInputRequestTypeDef

```python
# ListInstancesInputRequestTypeDef definition

class ListInstancesInputRequestTypeDef(TypedDict):
    ClusterId: str,
    InstanceGroupId: NotRequired[str],
    InstanceGroupTypes: NotRequired[Sequence[InstanceGroupTypeType]],  # (1)
    InstanceFleetId: NotRequired[str],
    InstanceFleetType: NotRequired[InstanceFleetTypeType],  # (2)
    InstanceStates: NotRequired[Sequence[InstanceStateType]],  # (3)
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: InstanceGroupTypeType](./literals.md#instancegrouptypetype) 
2. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
3. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
## ReleaseLabelFilterTypeDef

```python
# ReleaseLabelFilterTypeDef definition

class ReleaseLabelFilterTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Application: NotRequired[str],
```

## ListSecurityConfigurationsInputRequestTypeDef

```python
# ListSecurityConfigurationsInputRequestTypeDef definition

class ListSecurityConfigurationsInputRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
```

## SecurityConfigurationSummaryTypeDef

```python
# SecurityConfigurationSummaryTypeDef definition

class SecurityConfigurationSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    CreationDateTime: NotRequired[datetime],
```

## ListStepsInputRequestTypeDef

```python
# ListStepsInputRequestTypeDef definition

class ListStepsInputRequestTypeDef(TypedDict):
    ClusterId: str,
    StepStates: NotRequired[Sequence[StepStateType]],  # (1)
    StepIds: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: StepStateType](./literals.md#stepstatetype) 
## ListStudioSessionMappingsInputRequestTypeDef

```python
# ListStudioSessionMappingsInputRequestTypeDef definition

class ListStudioSessionMappingsInputRequestTypeDef(TypedDict):
    StudioId: NotRequired[str],
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## SessionMappingSummaryTypeDef

```python
# SessionMappingSummaryTypeDef definition

class SessionMappingSummaryTypeDef(TypedDict):
    StudioId: NotRequired[str],
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    SessionPolicyArn: NotRequired[str],
    CreationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## ListStudiosInputRequestTypeDef

```python
# ListStudiosInputRequestTypeDef definition

class ListStudiosInputRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
```

## StudioSummaryTypeDef

```python
# StudioSummaryTypeDef definition

class StudioSummaryTypeDef(TypedDict):
    StudioId: NotRequired[str],
    Name: NotRequired[str],
    VpcId: NotRequired[str],
    Description: NotRequired[str],
    Url: NotRequired[str],
    AuthMode: NotRequired[AuthModeType],  # (1)
    CreationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
## ListSupportedInstanceTypesInputRequestTypeDef

```python
# ListSupportedInstanceTypesInputRequestTypeDef definition

class ListSupportedInstanceTypesInputRequestTypeDef(TypedDict):
    ReleaseLabel: str,
    Marker: NotRequired[str],
```

## SupportedInstanceTypeTypeDef

```python
# SupportedInstanceTypeTypeDef definition

class SupportedInstanceTypeTypeDef(TypedDict):
    Type: NotRequired[str],
    MemoryGB: NotRequired[float],
    StorageGB: NotRequired[int],
    VCPU: NotRequired[int],
    Is64BitsOnly: NotRequired[bool],
    InstanceFamilyId: NotRequired[str],
    EbsOptimizedAvailable: NotRequired[bool],
    EbsOptimizedByDefault: NotRequired[bool],
    NumberOfDisks: NotRequired[int],
    EbsStorageOnly: NotRequired[bool],
    Architecture: NotRequired[str],
```

## ModifyClusterInputRequestTypeDef

```python
# ModifyClusterInputRequestTypeDef definition

class ModifyClusterInputRequestTypeDef(TypedDict):
    ClusterId: str,
    StepConcurrencyLevel: NotRequired[int],
```

## NotebookS3LocationForOutputTypeDef

```python
# NotebookS3LocationForOutputTypeDef definition

class NotebookS3LocationForOutputTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Key: NotRequired[str],
```

## OutputNotebookS3LocationForOutputTypeDef

```python
# OutputNotebookS3LocationForOutputTypeDef definition

class OutputNotebookS3LocationForOutputTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Key: NotRequired[str],
```

## NotebookS3LocationFromInputTypeDef

```python
# NotebookS3LocationFromInputTypeDef definition

class NotebookS3LocationFromInputTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Key: NotRequired[str],
```

## OnDemandCapacityReservationOptionsTypeDef

```python
# OnDemandCapacityReservationOptionsTypeDef definition

class OnDemandCapacityReservationOptionsTypeDef(TypedDict):
    UsageStrategy: NotRequired[OnDemandCapacityReservationUsageStrategyType],  # (1)
    CapacityReservationPreference: NotRequired[OnDemandCapacityReservationPreferenceType],  # (2)
    CapacityReservationResourceGroupArn: NotRequired[str],
```

1. See [:material-code-brackets: OnDemandCapacityReservationUsageStrategyType](./literals.md#ondemandcapacityreservationusagestrategytype) 
2. See [:material-code-brackets: OnDemandCapacityReservationPreferenceType](./literals.md#ondemandcapacityreservationpreferencetype) 
## OutputNotebookS3LocationFromInputTypeDef

```python
# OutputNotebookS3LocationFromInputTypeDef definition

class OutputNotebookS3LocationFromInputTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Key: NotRequired[str],
```

## PlacementTypeTypeDef

```python
# PlacementTypeTypeDef definition

class PlacementTypeTypeDef(TypedDict):
    AvailabilityZone: NotRequired[str],
    AvailabilityZones: NotRequired[Sequence[str]],
```

## RemoveAutoScalingPolicyInputRequestTypeDef

```python
# RemoveAutoScalingPolicyInputRequestTypeDef definition

class RemoveAutoScalingPolicyInputRequestTypeDef(TypedDict):
    ClusterId: str,
    InstanceGroupId: str,
```

## RemoveAutoTerminationPolicyInputRequestTypeDef

```python
# RemoveAutoTerminationPolicyInputRequestTypeDef definition

class RemoveAutoTerminationPolicyInputRequestTypeDef(TypedDict):
    ClusterId: str,
```

## RemoveManagedScalingPolicyInputRequestTypeDef

```python
# RemoveManagedScalingPolicyInputRequestTypeDef definition

class RemoveManagedScalingPolicyInputRequestTypeDef(TypedDict):
    ClusterId: str,
```

## RemoveTagsInputRequestTypeDef

```python
# RemoveTagsInputRequestTypeDef definition

class RemoveTagsInputRequestTypeDef(TypedDict):
    ResourceId: str,
    TagKeys: Sequence[str],
```

## SupportedProductConfigTypeDef

```python
# SupportedProductConfigTypeDef definition

class SupportedProductConfigTypeDef(TypedDict):
    Name: NotRequired[str],
    Args: NotRequired[Sequence[str]],
```

## SimpleScalingPolicyConfigurationTypeDef

```python
# SimpleScalingPolicyConfigurationTypeDef definition

class SimpleScalingPolicyConfigurationTypeDef(TypedDict):
    ScalingAdjustment: int,
    AdjustmentType: NotRequired[AdjustmentTypeType],  # (1)
    CoolDown: NotRequired[int],
```

1. See [:material-code-brackets: AdjustmentTypeType](./literals.md#adjustmenttypetype) 
## ScriptBootstrapActionConfigTypeDef

```python
# ScriptBootstrapActionConfigTypeDef definition

class ScriptBootstrapActionConfigTypeDef(TypedDict):
    Path: str,
    Args: NotRequired[Sequence[str]],
```

## SetKeepJobFlowAliveWhenNoStepsInputRequestTypeDef

```python
# SetKeepJobFlowAliveWhenNoStepsInputRequestTypeDef definition

class SetKeepJobFlowAliveWhenNoStepsInputRequestTypeDef(TypedDict):
    JobFlowIds: Sequence[str],
    KeepJobFlowAliveWhenNoSteps: bool,
```

## SetTerminationProtectionInputRequestTypeDef

```python
# SetTerminationProtectionInputRequestTypeDef definition

class SetTerminationProtectionInputRequestTypeDef(TypedDict):
    JobFlowIds: Sequence[str],
    TerminationProtected: bool,
```

## SetUnhealthyNodeReplacementInputRequestTypeDef

```python
# SetUnhealthyNodeReplacementInputRequestTypeDef definition

class SetUnhealthyNodeReplacementInputRequestTypeDef(TypedDict):
    JobFlowIds: Sequence[str],
    UnhealthyNodeReplacement: bool,
```

## SetVisibleToAllUsersInputRequestTypeDef

```python
# SetVisibleToAllUsersInputRequestTypeDef definition

class SetVisibleToAllUsersInputRequestTypeDef(TypedDict):
    JobFlowIds: Sequence[str],
    VisibleToAllUsers: bool,
```

## StepExecutionStatusDetailTypeDef

```python
# StepExecutionStatusDetailTypeDef definition

class StepExecutionStatusDetailTypeDef(TypedDict):
    State: StepExecutionStateType,  # (1)
    CreationDateTime: datetime,
    StartDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
    LastStateChangeReason: NotRequired[str],
```

1. See [:material-code-brackets: StepExecutionStateType](./literals.md#stepexecutionstatetype) 
## StepStateChangeReasonTypeDef

```python
# StepStateChangeReasonTypeDef definition

class StepStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[StepStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: StepStateChangeReasonCodeType](./literals.md#stepstatechangereasoncodetype) 
## StepTimelineTypeDef

```python
# StepTimelineTypeDef definition

class StepTimelineTypeDef(TypedDict):
    CreationDateTime: NotRequired[datetime],
    StartDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
```

## StopNotebookExecutionInputRequestTypeDef

```python
# StopNotebookExecutionInputRequestTypeDef definition

class StopNotebookExecutionInputRequestTypeDef(TypedDict):
    NotebookExecutionId: str,
```

## TerminateJobFlowsInputRequestTypeDef

```python
# TerminateJobFlowsInputRequestTypeDef definition

class TerminateJobFlowsInputRequestTypeDef(TypedDict):
    JobFlowIds: Sequence[str],
```

## UpdateStudioInputRequestTypeDef

```python
# UpdateStudioInputRequestTypeDef definition

class UpdateStudioInputRequestTypeDef(TypedDict):
    StudioId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    SubnetIds: NotRequired[Sequence[str]],
    DefaultS3Location: NotRequired[str],
    EncryptionKeyArn: NotRequired[str],
```

## UpdateStudioSessionMappingInputRequestTypeDef

```python
# UpdateStudioSessionMappingInputRequestTypeDef definition

class UpdateStudioSessionMappingInputRequestTypeDef(TypedDict):
    StudioId: str,
    IdentityType: IdentityTypeType,  # (1)
    SessionPolicyArn: str,
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## AddInstanceFleetOutputTypeDef

```python
# AddInstanceFleetOutputTypeDef definition

class AddInstanceFleetOutputTypeDef(TypedDict):
    ClusterId: str,
    InstanceFleetId: str,
    ClusterArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddInstanceGroupsOutputTypeDef

```python
# AddInstanceGroupsOutputTypeDef definition

class AddInstanceGroupsOutputTypeDef(TypedDict):
    JobFlowId: str,
    InstanceGroupIds: List[str],
    ClusterArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddJobFlowStepsOutputTypeDef

```python
# AddJobFlowStepsOutputTypeDef definition

class AddJobFlowStepsOutputTypeDef(TypedDict):
    StepIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSecurityConfigurationOutputTypeDef

```python
# CreateSecurityConfigurationOutputTypeDef definition

class CreateSecurityConfigurationOutputTypeDef(TypedDict):
    Name: str,
    CreationDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStudioOutputTypeDef

```python
# CreateStudioOutputTypeDef definition

class CreateStudioOutputTypeDef(TypedDict):
    StudioId: str,
    Url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSecurityConfigurationOutputTypeDef

```python
# DescribeSecurityConfigurationOutputTypeDef definition

class DescribeSecurityConfigurationOutputTypeDef(TypedDict):
    Name: str,
    SecurityConfiguration: str,
    CreationDateTime: datetime,
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
## ListReleaseLabelsOutputTypeDef

```python
# ListReleaseLabelsOutputTypeDef definition

class ListReleaseLabelsOutputTypeDef(TypedDict):
    ReleaseLabels: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyClusterOutputTypeDef

```python
# ModifyClusterOutputTypeDef definition

class ModifyClusterOutputTypeDef(TypedDict):
    StepConcurrencyLevel: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunJobFlowOutputTypeDef

```python
# RunJobFlowOutputTypeDef definition

class RunJobFlowOutputTypeDef(TypedDict):
    JobFlowId: str,
    ClusterArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartNotebookExecutionOutputTypeDef

```python
# StartNotebookExecutionOutputTypeDef definition

class StartNotebookExecutionOutputTypeDef(TypedDict):
    NotebookExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddTagsInputRequestTypeDef

```python
# AddTagsInputRequestTypeDef definition

class AddTagsInputRequestTypeDef(TypedDict):
    ResourceId: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateStudioInputRequestTypeDef

```python
# CreateStudioInputRequestTypeDef definition

class CreateStudioInputRequestTypeDef(TypedDict):
    Name: str,
    AuthMode: AuthModeType,  # (1)
    VpcId: str,
    SubnetIds: Sequence[str],
    ServiceRole: str,
    WorkspaceSecurityGroupId: str,
    EngineSecurityGroupId: str,
    DefaultS3Location: str,
    Description: NotRequired[str],
    UserRole: NotRequired[str],
    IdpAuthUrl: NotRequired[str],
    IdpRelayStateParameterName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    TrustedIdentityPropagationEnabled: NotRequired[bool],
    IdcUserAssignment: NotRequired[IdcUserAssignmentType],  # (3)
    IdcInstanceArn: NotRequired[str],
    EncryptionKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: IdcUserAssignmentType](./literals.md#idcuserassignmenttype) 
## StudioTypeDef

```python
# StudioTypeDef definition

class StudioTypeDef(TypedDict):
    StudioId: NotRequired[str],
    StudioArn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    AuthMode: NotRequired[AuthModeType],  # (1)
    VpcId: NotRequired[str],
    SubnetIds: NotRequired[List[str]],
    ServiceRole: NotRequired[str],
    UserRole: NotRequired[str],
    WorkspaceSecurityGroupId: NotRequired[str],
    EngineSecurityGroupId: NotRequired[str],
    Url: NotRequired[str],
    CreationTime: NotRequired[datetime],
    DefaultS3Location: NotRequired[str],
    IdpAuthUrl: NotRequired[str],
    IdpRelayStateParameterName: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    IdcInstanceArn: NotRequired[str],
    TrustedIdentityPropagationEnabled: NotRequired[bool],
    IdcUserAssignment: NotRequired[IdcUserAssignmentType],  # (3)
    EncryptionKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: IdcUserAssignmentType](./literals.md#idcuserassignmenttype) 
## AutoScalingPolicyStatusTypeDef

```python
# AutoScalingPolicyStatusTypeDef definition

class AutoScalingPolicyStatusTypeDef(TypedDict):
    State: NotRequired[AutoScalingPolicyStateType],  # (1)
    StateChangeReason: NotRequired[AutoScalingPolicyStateChangeReasonTypeDef],  # (2)
```

1. See [:material-code-brackets: AutoScalingPolicyStateType](./literals.md#autoscalingpolicystatetype) 
2. See [:material-code-braces: AutoScalingPolicyStateChangeReasonTypeDef](./type_defs.md#autoscalingpolicystatechangereasontypedef) 
## GetAutoTerminationPolicyOutputTypeDef

```python
# GetAutoTerminationPolicyOutputTypeDef definition

class GetAutoTerminationPolicyOutputTypeDef(TypedDict):
    AutoTerminationPolicy: AutoTerminationPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoTerminationPolicyTypeDef](./type_defs.md#autoterminationpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAutoTerminationPolicyInputRequestTypeDef

```python
# PutAutoTerminationPolicyInputRequestTypeDef definition

class PutAutoTerminationPolicyInputRequestTypeDef(TypedDict):
    ClusterId: str,
    AutoTerminationPolicy: NotRequired[AutoTerminationPolicyTypeDef],  # (1)
```

1. See [:material-code-braces: AutoTerminationPolicyTypeDef](./type_defs.md#autoterminationpolicytypedef) 
## BlockPublicAccessConfigurationOutputTypeDef

```python
# BlockPublicAccessConfigurationOutputTypeDef definition

class BlockPublicAccessConfigurationOutputTypeDef(TypedDict):
    BlockPublicSecurityGroupRules: bool,
    PermittedPublicSecurityGroupRuleRanges: NotRequired[List[PortRangeTypeDef]],  # (1)
```

1. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
## BlockPublicAccessConfigurationTypeDef

```python
# BlockPublicAccessConfigurationTypeDef definition

class BlockPublicAccessConfigurationTypeDef(TypedDict):
    BlockPublicSecurityGroupRules: bool,
    PermittedPublicSecurityGroupRuleRanges: NotRequired[Sequence[PortRangeTypeDef]],  # (1)
```

1. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
## BootstrapActionConfigOutputTypeDef

```python
# BootstrapActionConfigOutputTypeDef definition

class BootstrapActionConfigOutputTypeDef(TypedDict):
    Name: str,
    ScriptBootstrapAction: ScriptBootstrapActionConfigOutputTypeDef,  # (1)
```

1. See [:material-code-braces: ScriptBootstrapActionConfigOutputTypeDef](./type_defs.md#scriptbootstrapactionconfigoutputtypedef) 
## CancelStepsOutputTypeDef

```python
# CancelStepsOutputTypeDef definition

class CancelStepsOutputTypeDef(TypedDict):
    CancelStepsInfoList: List[CancelStepsInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CancelStepsInfoTypeDef](./type_defs.md#cancelstepsinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CloudWatchAlarmDefinitionOutputTypeDef

```python
# CloudWatchAlarmDefinitionOutputTypeDef definition

class CloudWatchAlarmDefinitionOutputTypeDef(TypedDict):
    ComparisonOperator: ComparisonOperatorType,  # (1)
    MetricName: str,
    Period: int,
    Threshold: float,
    EvaluationPeriods: NotRequired[int],
    Namespace: NotRequired[str],
    Statistic: NotRequired[StatisticType],  # (2)
    Unit: NotRequired[UnitType],  # (3)
    Dimensions: NotRequired[List[MetricDimensionTypeDef]],  # (4)
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-brackets: UnitType](./literals.md#unittype) 
4. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
## CloudWatchAlarmDefinitionTypeDef

```python
# CloudWatchAlarmDefinitionTypeDef definition

class CloudWatchAlarmDefinitionTypeDef(TypedDict):
    ComparisonOperator: ComparisonOperatorType,  # (1)
    MetricName: str,
    Period: int,
    Threshold: float,
    EvaluationPeriods: NotRequired[int],
    Namespace: NotRequired[str],
    Statistic: NotRequired[StatisticType],  # (2)
    Unit: NotRequired[UnitType],  # (3)
    Dimensions: NotRequired[Sequence[MetricDimensionTypeDef]],  # (4)
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-brackets: UnitType](./literals.md#unittype) 
4. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
## ClusterStatusTypeDef

```python
# ClusterStatusTypeDef definition

class ClusterStatusTypeDef(TypedDict):
    State: NotRequired[ClusterStateType],  # (1)
    StateChangeReason: NotRequired[ClusterStateChangeReasonTypeDef],  # (2)
    Timeline: NotRequired[ClusterTimelineTypeDef],  # (3)
    ErrorDetails: NotRequired[List[ErrorDetailTypeDef]],  # (4)
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
2. See [:material-code-braces: ClusterStateChangeReasonTypeDef](./type_defs.md#clusterstatechangereasontypedef) 
3. See [:material-code-braces: ClusterTimelineTypeDef](./type_defs.md#clustertimelinetypedef) 
4. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## ListBootstrapActionsOutputTypeDef

```python
# ListBootstrapActionsOutputTypeDef definition

class ListBootstrapActionsOutputTypeDef(TypedDict):
    BootstrapActions: List[CommandTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommandTypeDef](./type_defs.md#commandtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ManagedScalingPolicyTypeDef

```python
# ManagedScalingPolicyTypeDef definition

class ManagedScalingPolicyTypeDef(TypedDict):
    ComputeLimits: NotRequired[ComputeLimitsTypeDef],  # (1)
    UtilizationPerformanceIndex: NotRequired[int],
    ScalingStrategy: NotRequired[ScalingStrategyType],  # (2)
```

1. See [:material-code-braces: ComputeLimitsTypeDef](./type_defs.md#computelimitstypedef) 
2. See [:material-code-brackets: ScalingStrategyType](./literals.md#scalingstrategytype) 
## CredentialsTypeDef

```python
# CredentialsTypeDef definition

class CredentialsTypeDef(TypedDict):
    UsernamePassword: NotRequired[UsernamePasswordTypeDef],  # (1)
```

1. See [:material-code-braces: UsernamePasswordTypeDef](./type_defs.md#usernamepasswordtypedef) 
## DescribeClusterInputWaitTypeDef

```python
# DescribeClusterInputWaitTypeDef definition

class DescribeClusterInputWaitTypeDef(TypedDict):
    ClusterId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeStepInputWaitTypeDef

```python
# DescribeStepInputWaitTypeDef definition

class DescribeStepInputWaitTypeDef(TypedDict):
    ClusterId: str,
    StepId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeJobFlowsInputRequestTypeDef

```python
# DescribeJobFlowsInputRequestTypeDef definition

class DescribeJobFlowsInputRequestTypeDef(TypedDict):
    CreatedAfter: NotRequired[TimestampTypeDef],
    CreatedBefore: NotRequired[TimestampTypeDef],
    JobFlowIds: NotRequired[Sequence[str]],
    JobFlowStates: NotRequired[Sequence[JobFlowExecutionStateType]],  # (1)
```

1. See [:material-code-brackets: JobFlowExecutionStateType](./literals.md#jobflowexecutionstatetype) 
## ListClustersInputRequestTypeDef

```python
# ListClustersInputRequestTypeDef definition

class ListClustersInputRequestTypeDef(TypedDict):
    CreatedAfter: NotRequired[TimestampTypeDef],
    CreatedBefore: NotRequired[TimestampTypeDef],
    ClusterStates: NotRequired[Sequence[ClusterStateType]],  # (1)
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
## ListNotebookExecutionsInputRequestTypeDef

```python
# ListNotebookExecutionsInputRequestTypeDef definition

class ListNotebookExecutionsInputRequestTypeDef(TypedDict):
    EditorId: NotRequired[str],
    Status: NotRequired[NotebookExecutionStatusType],  # (1)
    From: NotRequired[TimestampTypeDef],
    To: NotRequired[TimestampTypeDef],
    Marker: NotRequired[str],
    ExecutionEngineId: NotRequired[str],
```

1. See [:material-code-brackets: NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype) 
## DescribeReleaseLabelOutputTypeDef

```python
# DescribeReleaseLabelOutputTypeDef definition

class DescribeReleaseLabelOutputTypeDef(TypedDict):
    ReleaseLabel: str,
    Applications: List[SimplifiedApplicationTypeDef],  # (1)
    AvailableOSReleases: List[OSReleaseTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SimplifiedApplicationTypeDef](./type_defs.md#simplifiedapplicationtypedef) 
2. See [:material-code-braces: OSReleaseTypeDef](./type_defs.md#osreleasetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EbsBlockDeviceConfigTypeDef

```python
# EbsBlockDeviceConfigTypeDef definition

class EbsBlockDeviceConfigTypeDef(TypedDict):
    VolumeSpecification: VolumeSpecificationTypeDef,  # (1)
    VolumesPerInstance: NotRequired[int],
```

1. See [:material-code-braces: VolumeSpecificationTypeDef](./type_defs.md#volumespecificationtypedef) 
## EbsBlockDeviceTypeDef

```python
# EbsBlockDeviceTypeDef definition

class EbsBlockDeviceTypeDef(TypedDict):
    VolumeSpecification: NotRequired[VolumeSpecificationTypeDef],  # (1)
    Device: NotRequired[str],
```

1. See [:material-code-braces: VolumeSpecificationTypeDef](./type_defs.md#volumespecificationtypedef) 
## GetStudioSessionMappingOutputTypeDef

```python
# GetStudioSessionMappingOutputTypeDef definition

class GetStudioSessionMappingOutputTypeDef(TypedDict):
    SessionMapping: SessionMappingDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionMappingDetailTypeDef](./type_defs.md#sessionmappingdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HadoopJarStepConfigOutputTypeDef

```python
# HadoopJarStepConfigOutputTypeDef definition

class HadoopJarStepConfigOutputTypeDef(TypedDict):
    Jar: str,
    Properties: NotRequired[List[KeyValueTypeDef]],  # (1)
    MainClass: NotRequired[str],
    Args: NotRequired[List[str]],
```

1. See [:material-code-braces: KeyValueTypeDef](./type_defs.md#keyvaluetypedef) 
## HadoopJarStepConfigTypeDef

```python
# HadoopJarStepConfigTypeDef definition

class HadoopJarStepConfigTypeDef(TypedDict):
    Jar: str,
    Properties: NotRequired[Sequence[KeyValueTypeDef]],  # (1)
    MainClass: NotRequired[str],
    Args: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: KeyValueTypeDef](./type_defs.md#keyvaluetypedef) 
## InstanceFleetStatusTypeDef

```python
# InstanceFleetStatusTypeDef definition

class InstanceFleetStatusTypeDef(TypedDict):
    State: NotRequired[InstanceFleetStateType],  # (1)
    StateChangeReason: NotRequired[InstanceFleetStateChangeReasonTypeDef],  # (2)
    Timeline: NotRequired[InstanceFleetTimelineTypeDef],  # (3)
```

1. See [:material-code-brackets: InstanceFleetStateType](./literals.md#instancefleetstatetype) 
2. See [:material-code-braces: InstanceFleetStateChangeReasonTypeDef](./type_defs.md#instancefleetstatechangereasontypedef) 
3. See [:material-code-braces: InstanceFleetTimelineTypeDef](./type_defs.md#instancefleettimelinetypedef) 
## InstanceGroupStatusTypeDef

```python
# InstanceGroupStatusTypeDef definition

class InstanceGroupStatusTypeDef(TypedDict):
    State: NotRequired[InstanceGroupStateType],  # (1)
    StateChangeReason: NotRequired[InstanceGroupStateChangeReasonTypeDef],  # (2)
    Timeline: NotRequired[InstanceGroupTimelineTypeDef],  # (3)
```

1. See [:material-code-brackets: InstanceGroupStateType](./literals.md#instancegroupstatetype) 
2. See [:material-code-braces: InstanceGroupStateChangeReasonTypeDef](./type_defs.md#instancegroupstatechangereasontypedef) 
3. See [:material-code-braces: InstanceGroupTimelineTypeDef](./type_defs.md#instancegrouptimelinetypedef) 
## ShrinkPolicyOutputTypeDef

```python
# ShrinkPolicyOutputTypeDef definition

class ShrinkPolicyOutputTypeDef(TypedDict):
    DecommissionTimeout: NotRequired[int],
    InstanceResizePolicy: NotRequired[InstanceResizePolicyOutputTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceResizePolicyOutputTypeDef](./type_defs.md#instanceresizepolicyoutputtypedef) 
## InstanceStatusTypeDef

```python
# InstanceStatusTypeDef definition

class InstanceStatusTypeDef(TypedDict):
    State: NotRequired[InstanceStateType],  # (1)
    StateChangeReason: NotRequired[InstanceStateChangeReasonTypeDef],  # (2)
    Timeline: NotRequired[InstanceTimelineTypeDef],  # (3)
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
2. See [:material-code-braces: InstanceStateChangeReasonTypeDef](./type_defs.md#instancestatechangereasontypedef) 
3. See [:material-code-braces: InstanceTimelineTypeDef](./type_defs.md#instancetimelinetypedef) 
## JobFlowInstancesDetailTypeDef

```python
# JobFlowInstancesDetailTypeDef definition

class JobFlowInstancesDetailTypeDef(TypedDict):
    MasterInstanceType: str,
    SlaveInstanceType: str,
    InstanceCount: int,
    MasterPublicDnsName: NotRequired[str],
    MasterInstanceId: NotRequired[str],
    InstanceGroups: NotRequired[List[InstanceGroupDetailTypeDef]],  # (1)
    NormalizedInstanceHours: NotRequired[int],
    Ec2KeyName: NotRequired[str],
    Ec2SubnetId: NotRequired[str],
    Placement: NotRequired[PlacementTypeOutputTypeDef],  # (2)
    KeepJobFlowAliveWhenNoSteps: NotRequired[bool],
    TerminationProtected: NotRequired[bool],
    UnhealthyNodeReplacement: NotRequired[bool],
    HadoopVersion: NotRequired[str],
```

1. See [:material-code-braces: InstanceGroupDetailTypeDef](./type_defs.md#instancegroupdetailtypedef) 
2. See [:material-code-braces: PlacementTypeOutputTypeDef](./type_defs.md#placementtypeoutputtypedef) 
## ListBootstrapActionsInputPaginateTypeDef

```python
# ListBootstrapActionsInputPaginateTypeDef definition

class ListBootstrapActionsInputPaginateTypeDef(TypedDict):
    ClusterId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersInputPaginateTypeDef

```python
# ListClustersInputPaginateTypeDef definition

class ListClustersInputPaginateTypeDef(TypedDict):
    CreatedAfter: NotRequired[TimestampTypeDef],
    CreatedBefore: NotRequired[TimestampTypeDef],
    ClusterStates: NotRequired[Sequence[ClusterStateType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceFleetsInputPaginateTypeDef

```python
# ListInstanceFleetsInputPaginateTypeDef definition

class ListInstanceFleetsInputPaginateTypeDef(TypedDict):
    ClusterId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceGroupsInputPaginateTypeDef

```python
# ListInstanceGroupsInputPaginateTypeDef definition

class ListInstanceGroupsInputPaginateTypeDef(TypedDict):
    ClusterId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstancesInputPaginateTypeDef

```python
# ListInstancesInputPaginateTypeDef definition

class ListInstancesInputPaginateTypeDef(TypedDict):
    ClusterId: str,
    InstanceGroupId: NotRequired[str],
    InstanceGroupTypes: NotRequired[Sequence[InstanceGroupTypeType]],  # (1)
    InstanceFleetId: NotRequired[str],
    InstanceFleetType: NotRequired[InstanceFleetTypeType],  # (2)
    InstanceStates: NotRequired[Sequence[InstanceStateType]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: InstanceGroupTypeType](./literals.md#instancegrouptypetype) 
2. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
3. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotebookExecutionsInputPaginateTypeDef

```python
# ListNotebookExecutionsInputPaginateTypeDef definition

class ListNotebookExecutionsInputPaginateTypeDef(TypedDict):
    EditorId: NotRequired[str],
    Status: NotRequired[NotebookExecutionStatusType],  # (1)
    From: NotRequired[TimestampTypeDef],
    To: NotRequired[TimestampTypeDef],
    ExecutionEngineId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityConfigurationsInputPaginateTypeDef

```python
# ListSecurityConfigurationsInputPaginateTypeDef definition

class ListSecurityConfigurationsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStepsInputPaginateTypeDef

```python
# ListStepsInputPaginateTypeDef definition

class ListStepsInputPaginateTypeDef(TypedDict):
    ClusterId: str,
    StepStates: NotRequired[Sequence[StepStateType]],  # (1)
    StepIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: StepStateType](./literals.md#stepstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStudioSessionMappingsInputPaginateTypeDef

```python
# ListStudioSessionMappingsInputPaginateTypeDef definition

class ListStudioSessionMappingsInputPaginateTypeDef(TypedDict):
    StudioId: NotRequired[str],
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStudiosInputPaginateTypeDef

```python
# ListStudiosInputPaginateTypeDef definition

class ListStudiosInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReleaseLabelsInputRequestTypeDef

```python
# ListReleaseLabelsInputRequestTypeDef definition

class ListReleaseLabelsInputRequestTypeDef(TypedDict):
    Filters: NotRequired[ReleaseLabelFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ReleaseLabelFilterTypeDef](./type_defs.md#releaselabelfiltertypedef) 
## ListSecurityConfigurationsOutputTypeDef

```python
# ListSecurityConfigurationsOutputTypeDef definition

class ListSecurityConfigurationsOutputTypeDef(TypedDict):
    SecurityConfigurations: List[SecurityConfigurationSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityConfigurationSummaryTypeDef](./type_defs.md#securityconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStudioSessionMappingsOutputTypeDef

```python
# ListStudioSessionMappingsOutputTypeDef definition

class ListStudioSessionMappingsOutputTypeDef(TypedDict):
    SessionMappings: List[SessionMappingSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionMappingSummaryTypeDef](./type_defs.md#sessionmappingsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStudiosOutputTypeDef

```python
# ListStudiosOutputTypeDef definition

class ListStudiosOutputTypeDef(TypedDict):
    Studios: List[StudioSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioSummaryTypeDef](./type_defs.md#studiosummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSupportedInstanceTypesOutputTypeDef

```python
# ListSupportedInstanceTypesOutputTypeDef definition

class ListSupportedInstanceTypesOutputTypeDef(TypedDict):
    SupportedInstanceTypes: List[SupportedInstanceTypeTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SupportedInstanceTypeTypeDef](./type_defs.md#supportedinstancetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NotebookExecutionSummaryTypeDef

```python
# NotebookExecutionSummaryTypeDef definition

class NotebookExecutionSummaryTypeDef(TypedDict):
    NotebookExecutionId: NotRequired[str],
    EditorId: NotRequired[str],
    NotebookExecutionName: NotRequired[str],
    Status: NotRequired[NotebookExecutionStatusType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    NotebookS3Location: NotRequired[NotebookS3LocationForOutputTypeDef],  # (2)
    ExecutionEngineId: NotRequired[str],
```

1. See [:material-code-brackets: NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype) 
2. See [:material-code-braces: NotebookS3LocationForOutputTypeDef](./type_defs.md#notebooks3locationforoutputtypedef) 
## NotebookExecutionTypeDef

```python
# NotebookExecutionTypeDef definition

class NotebookExecutionTypeDef(TypedDict):
    NotebookExecutionId: NotRequired[str],
    EditorId: NotRequired[str],
    ExecutionEngine: NotRequired[ExecutionEngineConfigTypeDef],  # (1)
    NotebookExecutionName: NotRequired[str],
    NotebookParams: NotRequired[str],
    Status: NotRequired[NotebookExecutionStatusType],  # (2)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Arn: NotRequired[str],
    OutputNotebookURI: NotRequired[str],
    LastStateChangeReason: NotRequired[str],
    NotebookInstanceSecurityGroupId: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (3)
    NotebookS3Location: NotRequired[NotebookS3LocationForOutputTypeDef],  # (4)
    OutputNotebookS3Location: NotRequired[OutputNotebookS3LocationForOutputTypeDef],  # (5)
    OutputNotebookFormat: NotRequired[OutputNotebookFormatType],  # (6)
    EnvironmentVariables: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ExecutionEngineConfigTypeDef](./type_defs.md#executionengineconfigtypedef) 
2. See [:material-code-brackets: NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: NotebookS3LocationForOutputTypeDef](./type_defs.md#notebooks3locationforoutputtypedef) 
5. See [:material-code-braces: OutputNotebookS3LocationForOutputTypeDef](./type_defs.md#outputnotebooks3locationforoutputtypedef) 
6. See [:material-code-brackets: OutputNotebookFormatType](./literals.md#outputnotebookformattype) 
## OnDemandProvisioningSpecificationTypeDef

```python
# OnDemandProvisioningSpecificationTypeDef definition

class OnDemandProvisioningSpecificationTypeDef(TypedDict):
    AllocationStrategy: OnDemandProvisioningAllocationStrategyType,  # (1)
    CapacityReservationOptions: NotRequired[OnDemandCapacityReservationOptionsTypeDef],  # (2)
```

1. See [:material-code-brackets: OnDemandProvisioningAllocationStrategyType](./literals.md#ondemandprovisioningallocationstrategytype) 
2. See [:material-code-braces: OnDemandCapacityReservationOptionsTypeDef](./type_defs.md#ondemandcapacityreservationoptionstypedef) 
## OnDemandResizingSpecificationTypeDef

```python
# OnDemandResizingSpecificationTypeDef definition

class OnDemandResizingSpecificationTypeDef(TypedDict):
    TimeoutDurationMinutes: NotRequired[int],
    AllocationStrategy: NotRequired[OnDemandProvisioningAllocationStrategyType],  # (1)
    CapacityReservationOptions: NotRequired[OnDemandCapacityReservationOptionsTypeDef],  # (2)
```

1. See [:material-code-brackets: OnDemandProvisioningAllocationStrategyType](./literals.md#ondemandprovisioningallocationstrategytype) 
2. See [:material-code-braces: OnDemandCapacityReservationOptionsTypeDef](./type_defs.md#ondemandcapacityreservationoptionstypedef) 
## StartNotebookExecutionInputRequestTypeDef

```python
# StartNotebookExecutionInputRequestTypeDef definition

class StartNotebookExecutionInputRequestTypeDef(TypedDict):
    ExecutionEngine: ExecutionEngineConfigTypeDef,  # (1)
    ServiceRole: str,
    EditorId: NotRequired[str],
    RelativePath: NotRequired[str],
    NotebookExecutionName: NotRequired[str],
    NotebookParams: NotRequired[str],
    NotebookInstanceSecurityGroupId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    NotebookS3Location: NotRequired[NotebookS3LocationFromInputTypeDef],  # (3)
    OutputNotebookS3Location: NotRequired[OutputNotebookS3LocationFromInputTypeDef],  # (4)
    OutputNotebookFormat: NotRequired[OutputNotebookFormatType],  # (5)
    EnvironmentVariables: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ExecutionEngineConfigTypeDef](./type_defs.md#executionengineconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: NotebookS3LocationFromInputTypeDef](./type_defs.md#notebooks3locationfrominputtypedef) 
4. See [:material-code-braces: OutputNotebookS3LocationFromInputTypeDef](./type_defs.md#outputnotebooks3locationfrominputtypedef) 
5. See [:material-code-brackets: OutputNotebookFormatType](./literals.md#outputnotebookformattype) 
## ScalingActionTypeDef

```python
# ScalingActionTypeDef definition

class ScalingActionTypeDef(TypedDict):
    SimpleScalingPolicyConfiguration: SimpleScalingPolicyConfigurationTypeDef,  # (2)
    Market: NotRequired[MarketTypeType],  # (1)
```

1. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
2. See [:material-code-braces: SimpleScalingPolicyConfigurationTypeDef](./type_defs.md#simplescalingpolicyconfigurationtypedef) 
## StepStatusTypeDef

```python
# StepStatusTypeDef definition

class StepStatusTypeDef(TypedDict):
    State: NotRequired[StepStateType],  # (1)
    StateChangeReason: NotRequired[StepStateChangeReasonTypeDef],  # (2)
    FailureDetails: NotRequired[FailureDetailsTypeDef],  # (3)
    Timeline: NotRequired[StepTimelineTypeDef],  # (4)
```

1. See [:material-code-brackets: StepStateType](./literals.md#stepstatetype) 
2. See [:material-code-braces: StepStateChangeReasonTypeDef](./type_defs.md#stepstatechangereasontypedef) 
3. See [:material-code-braces: FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef) 
4. See [:material-code-braces: StepTimelineTypeDef](./type_defs.md#steptimelinetypedef) 
## DescribeStudioOutputTypeDef

```python
# DescribeStudioOutputTypeDef definition

class DescribeStudioOutputTypeDef(TypedDict):
    Studio: StudioTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioTypeDef](./type_defs.md#studiotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlockPublicAccessConfigurationOutputTypeDef

```python
# GetBlockPublicAccessConfigurationOutputTypeDef definition

class GetBlockPublicAccessConfigurationOutputTypeDef(TypedDict):
    BlockPublicAccessConfiguration: BlockPublicAccessConfigurationOutputTypeDef,  # (1)
    BlockPublicAccessConfigurationMetadata: BlockPublicAccessConfigurationMetadataTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BlockPublicAccessConfigurationOutputTypeDef](./type_defs.md#blockpublicaccessconfigurationoutputtypedef) 
2. See [:material-code-braces: BlockPublicAccessConfigurationMetadataTypeDef](./type_defs.md#blockpublicaccessconfigurationmetadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBlockPublicAccessConfigurationInputRequestTypeDef

```python
# PutBlockPublicAccessConfigurationInputRequestTypeDef definition

class PutBlockPublicAccessConfigurationInputRequestTypeDef(TypedDict):
    BlockPublicAccessConfiguration: BlockPublicAccessConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: BlockPublicAccessConfigurationTypeDef](./type_defs.md#blockpublicaccessconfigurationtypedef) 
## BootstrapActionDetailTypeDef

```python
# BootstrapActionDetailTypeDef definition

class BootstrapActionDetailTypeDef(TypedDict):
    BootstrapActionConfig: NotRequired[BootstrapActionConfigOutputTypeDef],  # (1)
```

1. See [:material-code-braces: BootstrapActionConfigOutputTypeDef](./type_defs.md#bootstrapactionconfigoutputtypedef) 
## ScalingTriggerOutputTypeDef

```python
# ScalingTriggerOutputTypeDef definition

class ScalingTriggerOutputTypeDef(TypedDict):
    CloudWatchAlarmDefinition: CloudWatchAlarmDefinitionOutputTypeDef,  # (1)
```

1. See [:material-code-braces: CloudWatchAlarmDefinitionOutputTypeDef](./type_defs.md#cloudwatchalarmdefinitionoutputtypedef) 
## ClusterSummaryTypeDef

```python
# ClusterSummaryTypeDef definition

class ClusterSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ClusterStatusTypeDef],  # (1)
    NormalizedInstanceHours: NotRequired[int],
    ClusterArn: NotRequired[str],
    OutpostArn: NotRequired[str],
```

1. See [:material-code-braces: ClusterStatusTypeDef](./type_defs.md#clusterstatustypedef) 
## ClusterTypeDef

```python
# ClusterTypeDef definition

class ClusterTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ClusterStatusTypeDef],  # (1)
    Ec2InstanceAttributes: NotRequired[Ec2InstanceAttributesTypeDef],  # (2)
    InstanceCollectionType: NotRequired[InstanceCollectionTypeType],  # (3)
    LogUri: NotRequired[str],
    LogEncryptionKmsKeyId: NotRequired[str],
    RequestedAmiVersion: NotRequired[str],
    RunningAmiVersion: NotRequired[str],
    ReleaseLabel: NotRequired[str],
    AutoTerminate: NotRequired[bool],
    TerminationProtected: NotRequired[bool],
    UnhealthyNodeReplacement: NotRequired[bool],
    VisibleToAllUsers: NotRequired[bool],
    Applications: NotRequired[List[ApplicationOutputTypeDef]],  # (4)
    Tags: NotRequired[List[TagTypeDef]],  # (5)
    ServiceRole: NotRequired[str],
    NormalizedInstanceHours: NotRequired[int],
    MasterPublicDnsName: NotRequired[str],
    Configurations: NotRequired[List[ConfigurationOutputTypeDef]],  # (6)
    SecurityConfiguration: NotRequired[str],
    AutoScalingRole: NotRequired[str],
    ScaleDownBehavior: NotRequired[ScaleDownBehaviorType],  # (7)
    CustomAmiId: NotRequired[str],
    EbsRootVolumeSize: NotRequired[int],
    RepoUpgradeOnBoot: NotRequired[RepoUpgradeOnBootType],  # (8)
    KerberosAttributes: NotRequired[KerberosAttributesTypeDef],  # (9)
    ClusterArn: NotRequired[str],
    OutpostArn: NotRequired[str],
    StepConcurrencyLevel: NotRequired[int],
    PlacementGroups: NotRequired[List[PlacementGroupConfigTypeDef]],  # (10)
    OSReleaseLabel: NotRequired[str],
    EbsRootVolumeIops: NotRequired[int],
    EbsRootVolumeThroughput: NotRequired[int],
```

1. See [:material-code-braces: ClusterStatusTypeDef](./type_defs.md#clusterstatustypedef) 
2. See [:material-code-braces: Ec2InstanceAttributesTypeDef](./type_defs.md#ec2instanceattributestypedef) 
3. See [:material-code-brackets: InstanceCollectionTypeType](./literals.md#instancecollectiontypetype) 
4. See [:material-code-braces: ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
7. See [:material-code-brackets: ScaleDownBehaviorType](./literals.md#scaledownbehaviortype) 
8. See [:material-code-brackets: RepoUpgradeOnBootType](./literals.md#repoupgradeonboottype) 
9. See [:material-code-braces: KerberosAttributesTypeDef](./type_defs.md#kerberosattributestypedef) 
10. See [:material-code-braces: PlacementGroupConfigTypeDef](./type_defs.md#placementgroupconfigtypedef) 
## GetManagedScalingPolicyOutputTypeDef

```python
# GetManagedScalingPolicyOutputTypeDef definition

class GetManagedScalingPolicyOutputTypeDef(TypedDict):
    ManagedScalingPolicy: ManagedScalingPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedScalingPolicyTypeDef](./type_defs.md#managedscalingpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutManagedScalingPolicyInputRequestTypeDef

```python
# PutManagedScalingPolicyInputRequestTypeDef definition

class PutManagedScalingPolicyInputRequestTypeDef(TypedDict):
    ClusterId: str,
    ManagedScalingPolicy: ManagedScalingPolicyTypeDef,  # (1)
```

1. See [:material-code-braces: ManagedScalingPolicyTypeDef](./type_defs.md#managedscalingpolicytypedef) 
## GetClusterSessionCredentialsOutputTypeDef

```python
# GetClusterSessionCredentialsOutputTypeDef definition

class GetClusterSessionCredentialsOutputTypeDef(TypedDict):
    Credentials: CredentialsTypeDef,  # (1)
    ExpiresAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EbsConfigurationTypeDef

```python
# EbsConfigurationTypeDef definition

class EbsConfigurationTypeDef(TypedDict):
    EbsBlockDeviceConfigs: NotRequired[Sequence[EbsBlockDeviceConfigTypeDef]],  # (1)
    EbsOptimized: NotRequired[bool],
```

1. See [:material-code-braces: EbsBlockDeviceConfigTypeDef](./type_defs.md#ebsblockdeviceconfigtypedef) 
## InstanceTypeSpecificationPaginatorTypeDef

```python
# InstanceTypeSpecificationPaginatorTypeDef definition

class InstanceTypeSpecificationPaginatorTypeDef(TypedDict):
    InstanceType: NotRequired[str],
    WeightedCapacity: NotRequired[int],
    BidPrice: NotRequired[str],
    BidPriceAsPercentageOfOnDemandPrice: NotRequired[float],
    Configurations: NotRequired[List[ConfigurationPaginatorTypeDef]],  # (1)
    EbsBlockDevices: NotRequired[List[EbsBlockDeviceTypeDef]],  # (2)
    EbsOptimized: NotRequired[bool],
    CustomAmiId: NotRequired[str],
    Priority: NotRequired[float],
```

1. See [:material-code-braces: ConfigurationPaginatorTypeDef](./type_defs.md#configurationpaginatortypedef) 
2. See [:material-code-braces: EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef) 
## InstanceTypeSpecificationTypeDef

```python
# InstanceTypeSpecificationTypeDef definition

class InstanceTypeSpecificationTypeDef(TypedDict):
    InstanceType: NotRequired[str],
    WeightedCapacity: NotRequired[int],
    BidPrice: NotRequired[str],
    BidPriceAsPercentageOfOnDemandPrice: NotRequired[float],
    Configurations: NotRequired[List[ConfigurationOutputTypeDef]],  # (1)
    EbsBlockDevices: NotRequired[List[EbsBlockDeviceTypeDef]],  # (2)
    EbsOptimized: NotRequired[bool],
    CustomAmiId: NotRequired[str],
    Priority: NotRequired[float],
```

1. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
2. See [:material-code-braces: EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef) 
## StepConfigOutputTypeDef

```python
# StepConfigOutputTypeDef definition

class StepConfigOutputTypeDef(TypedDict):
    Name: str,
    HadoopJarStep: HadoopJarStepConfigOutputTypeDef,  # (2)
    ActionOnFailure: NotRequired[ActionOnFailureType],  # (1)
```

1. See [:material-code-brackets: ActionOnFailureType](./literals.md#actiononfailuretype) 
2. See [:material-code-braces: HadoopJarStepConfigOutputTypeDef](./type_defs.md#hadoopjarstepconfigoutputtypedef) 
## ShrinkPolicyTypeDef

```python
# ShrinkPolicyTypeDef definition

class ShrinkPolicyTypeDef(TypedDict):
    DecommissionTimeout: NotRequired[int],
    InstanceResizePolicy: NotRequired[InstanceResizePolicyUnionTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceResizePolicyTypeDef](./type_defs.md#instanceresizepolicytypedef) [:material-code-braces: InstanceResizePolicyOutputTypeDef](./type_defs.md#instanceresizepolicyoutputtypedef) 
## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    Id: NotRequired[str],
    Ec2InstanceId: NotRequired[str],
    PublicDnsName: NotRequired[str],
    PublicIpAddress: NotRequired[str],
    PrivateDnsName: NotRequired[str],
    PrivateIpAddress: NotRequired[str],
    Status: NotRequired[InstanceStatusTypeDef],  # (1)
    InstanceGroupId: NotRequired[str],
    InstanceFleetId: NotRequired[str],
    Market: NotRequired[MarketTypeType],  # (2)
    InstanceType: NotRequired[str],
    EbsVolumes: NotRequired[List[EbsVolumeTypeDef]],  # (3)
```

1. See [:material-code-braces: InstanceStatusTypeDef](./type_defs.md#instancestatustypedef) 
2. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
3. See [:material-code-braces: EbsVolumeTypeDef](./type_defs.md#ebsvolumetypedef) 
## ListNotebookExecutionsOutputTypeDef

```python
# ListNotebookExecutionsOutputTypeDef definition

class ListNotebookExecutionsOutputTypeDef(TypedDict):
    NotebookExecutions: List[NotebookExecutionSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotebookExecutionSummaryTypeDef](./type_defs.md#notebookexecutionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNotebookExecutionOutputTypeDef

```python
# DescribeNotebookExecutionOutputTypeDef definition

class DescribeNotebookExecutionOutputTypeDef(TypedDict):
    NotebookExecution: NotebookExecutionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotebookExecutionTypeDef](./type_defs.md#notebookexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceFleetProvisioningSpecificationsTypeDef

```python
# InstanceFleetProvisioningSpecificationsTypeDef definition

class InstanceFleetProvisioningSpecificationsTypeDef(TypedDict):
    SpotSpecification: NotRequired[SpotProvisioningSpecificationTypeDef],  # (1)
    OnDemandSpecification: NotRequired[OnDemandProvisioningSpecificationTypeDef],  # (2)
```

1. See [:material-code-braces: SpotProvisioningSpecificationTypeDef](./type_defs.md#spotprovisioningspecificationtypedef) 
2. See [:material-code-braces: OnDemandProvisioningSpecificationTypeDef](./type_defs.md#ondemandprovisioningspecificationtypedef) 
## InstanceFleetResizingSpecificationsTypeDef

```python
# InstanceFleetResizingSpecificationsTypeDef definition

class InstanceFleetResizingSpecificationsTypeDef(TypedDict):
    SpotResizeSpecification: NotRequired[SpotResizingSpecificationTypeDef],  # (1)
    OnDemandResizeSpecification: NotRequired[OnDemandResizingSpecificationTypeDef],  # (2)
```

1. See [:material-code-braces: SpotResizingSpecificationTypeDef](./type_defs.md#spotresizingspecificationtypedef) 
2. See [:material-code-braces: OnDemandResizingSpecificationTypeDef](./type_defs.md#ondemandresizingspecificationtypedef) 
## BootstrapActionConfigTypeDef

```python
# BootstrapActionConfigTypeDef definition

class BootstrapActionConfigTypeDef(TypedDict):
    Name: str,
    ScriptBootstrapAction: ScriptBootstrapActionConfigUnionTypeDef,  # (1)
```

1. See [:material-code-braces: ScriptBootstrapActionConfigTypeDef](./type_defs.md#scriptbootstrapactionconfigtypedef) [:material-code-braces: ScriptBootstrapActionConfigOutputTypeDef](./type_defs.md#scriptbootstrapactionconfigoutputtypedef) 
## StepSummaryTypeDef

```python
# StepSummaryTypeDef definition

class StepSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Config: NotRequired[HadoopStepConfigTypeDef],  # (1)
    ActionOnFailure: NotRequired[ActionOnFailureType],  # (2)
    Status: NotRequired[StepStatusTypeDef],  # (3)
```

1. See [:material-code-braces: HadoopStepConfigTypeDef](./type_defs.md#hadoopstepconfigtypedef) 
2. See [:material-code-brackets: ActionOnFailureType](./literals.md#actiononfailuretype) 
3. See [:material-code-braces: StepStatusTypeDef](./type_defs.md#stepstatustypedef) 
## StepTypeDef

```python
# StepTypeDef definition

class StepTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Config: NotRequired[HadoopStepConfigTypeDef],  # (1)
    ActionOnFailure: NotRequired[ActionOnFailureType],  # (2)
    Status: NotRequired[StepStatusTypeDef],  # (3)
    ExecutionRoleArn: NotRequired[str],
```

1. See [:material-code-braces: HadoopStepConfigTypeDef](./type_defs.md#hadoopstepconfigtypedef) 
2. See [:material-code-brackets: ActionOnFailureType](./literals.md#actiononfailuretype) 
3. See [:material-code-braces: StepStatusTypeDef](./type_defs.md#stepstatustypedef) 
## ScalingRuleOutputTypeDef

```python
# ScalingRuleOutputTypeDef definition

class ScalingRuleOutputTypeDef(TypedDict):
    Name: str,
    Action: ScalingActionTypeDef,  # (1)
    Trigger: ScalingTriggerOutputTypeDef,  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ScalingActionTypeDef](./type_defs.md#scalingactiontypedef) 
2. See [:material-code-braces: ScalingTriggerOutputTypeDef](./type_defs.md#scalingtriggeroutputtypedef) 
## ScalingTriggerTypeDef

```python
# ScalingTriggerTypeDef definition

class ScalingTriggerTypeDef(TypedDict):
    CloudWatchAlarmDefinition: CloudWatchAlarmDefinitionUnionTypeDef,  # (1)
```

1. See [:material-code-braces: CloudWatchAlarmDefinitionTypeDef](./type_defs.md#cloudwatchalarmdefinitiontypedef) [:material-code-braces: CloudWatchAlarmDefinitionOutputTypeDef](./type_defs.md#cloudwatchalarmdefinitionoutputtypedef) 
## ListClustersOutputTypeDef

```python
# ListClustersOutputTypeDef definition

class ListClustersOutputTypeDef(TypedDict):
    Clusters: List[ClusterSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSummaryTypeDef](./type_defs.md#clustersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeClusterOutputTypeDef

```python
# DescribeClusterOutputTypeDef definition

class DescribeClusterOutputTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceTypeConfigTypeDef

```python
# InstanceTypeConfigTypeDef definition

class InstanceTypeConfigTypeDef(TypedDict):
    InstanceType: str,
    WeightedCapacity: NotRequired[int],
    BidPrice: NotRequired[str],
    BidPriceAsPercentageOfOnDemandPrice: NotRequired[float],
    EbsConfiguration: NotRequired[EbsConfigurationTypeDef],  # (1)
    Configurations: NotRequired[Sequence[ConfigurationUnionTypeDef]],  # (2)
    CustomAmiId: NotRequired[str],
    Priority: NotRequired[float],
```

1. See [:material-code-braces: EbsConfigurationTypeDef](./type_defs.md#ebsconfigurationtypedef) 
2. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
## StepDetailTypeDef

```python
# StepDetailTypeDef definition

class StepDetailTypeDef(TypedDict):
    StepConfig: StepConfigOutputTypeDef,  # (1)
    ExecutionStatusDetail: StepExecutionStatusDetailTypeDef,  # (2)
```

1. See [:material-code-braces: StepConfigOutputTypeDef](./type_defs.md#stepconfigoutputtypedef) 
2. See [:material-code-braces: StepExecutionStatusDetailTypeDef](./type_defs.md#stepexecutionstatusdetailtypedef) 
## StepConfigTypeDef

```python
# StepConfigTypeDef definition

class StepConfigTypeDef(TypedDict):
    Name: str,
    HadoopJarStep: HadoopJarStepConfigUnionTypeDef,  # (2)
    ActionOnFailure: NotRequired[ActionOnFailureType],  # (1)
```

1. See [:material-code-brackets: ActionOnFailureType](./literals.md#actiononfailuretype) 
2. See [:material-code-braces: HadoopJarStepConfigTypeDef](./type_defs.md#hadoopjarstepconfigtypedef) [:material-code-braces: HadoopJarStepConfigOutputTypeDef](./type_defs.md#hadoopjarstepconfigoutputtypedef) 
## ListInstancesOutputTypeDef

```python
# ListInstancesOutputTypeDef definition

class ListInstancesOutputTypeDef(TypedDict):
    Instances: List[InstanceTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceFleetPaginatorTypeDef

```python
# InstanceFleetPaginatorTypeDef definition

class InstanceFleetPaginatorTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[InstanceFleetStatusTypeDef],  # (1)
    InstanceFleetType: NotRequired[InstanceFleetTypeType],  # (2)
    TargetOnDemandCapacity: NotRequired[int],
    TargetSpotCapacity: NotRequired[int],
    ProvisionedOnDemandCapacity: NotRequired[int],
    ProvisionedSpotCapacity: NotRequired[int],
    InstanceTypeSpecifications: NotRequired[List[InstanceTypeSpecificationPaginatorTypeDef]],  # (3)
    LaunchSpecifications: NotRequired[InstanceFleetProvisioningSpecificationsTypeDef],  # (4)
    ResizeSpecifications: NotRequired[InstanceFleetResizingSpecificationsTypeDef],  # (5)
    Context: NotRequired[str],
```

1. See [:material-code-braces: InstanceFleetStatusTypeDef](./type_defs.md#instancefleetstatustypedef) 
2. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
3. See [:material-code-braces: InstanceTypeSpecificationPaginatorTypeDef](./type_defs.md#instancetypespecificationpaginatortypedef) 
4. See [:material-code-braces: InstanceFleetProvisioningSpecificationsTypeDef](./type_defs.md#instancefleetprovisioningspecificationstypedef) 
5. See [:material-code-braces: InstanceFleetResizingSpecificationsTypeDef](./type_defs.md#instancefleetresizingspecificationstypedef) 
## InstanceFleetTypeDef

```python
# InstanceFleetTypeDef definition

class InstanceFleetTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[InstanceFleetStatusTypeDef],  # (1)
    InstanceFleetType: NotRequired[InstanceFleetTypeType],  # (2)
    TargetOnDemandCapacity: NotRequired[int],
    TargetSpotCapacity: NotRequired[int],
    ProvisionedOnDemandCapacity: NotRequired[int],
    ProvisionedSpotCapacity: NotRequired[int],
    InstanceTypeSpecifications: NotRequired[List[InstanceTypeSpecificationTypeDef]],  # (3)
    LaunchSpecifications: NotRequired[InstanceFleetProvisioningSpecificationsTypeDef],  # (4)
    ResizeSpecifications: NotRequired[InstanceFleetResizingSpecificationsTypeDef],  # (5)
    Context: NotRequired[str],
```

1. See [:material-code-braces: InstanceFleetStatusTypeDef](./type_defs.md#instancefleetstatustypedef) 
2. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
3. See [:material-code-braces: InstanceTypeSpecificationTypeDef](./type_defs.md#instancetypespecificationtypedef) 
4. See [:material-code-braces: InstanceFleetProvisioningSpecificationsTypeDef](./type_defs.md#instancefleetprovisioningspecificationstypedef) 
5. See [:material-code-braces: InstanceFleetResizingSpecificationsTypeDef](./type_defs.md#instancefleetresizingspecificationstypedef) 
## ListStepsOutputTypeDef

```python
# ListStepsOutputTypeDef definition

class ListStepsOutputTypeDef(TypedDict):
    Steps: List[StepSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StepSummaryTypeDef](./type_defs.md#stepsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStepOutputTypeDef

```python
# DescribeStepOutputTypeDef definition

class DescribeStepOutputTypeDef(TypedDict):
    Step: StepTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoScalingPolicyDescriptionTypeDef

```python
# AutoScalingPolicyDescriptionTypeDef definition

class AutoScalingPolicyDescriptionTypeDef(TypedDict):
    Status: NotRequired[AutoScalingPolicyStatusTypeDef],  # (1)
    Constraints: NotRequired[ScalingConstraintsTypeDef],  # (2)
    Rules: NotRequired[List[ScalingRuleOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: AutoScalingPolicyStatusTypeDef](./type_defs.md#autoscalingpolicystatustypedef) 
2. See [:material-code-braces: ScalingConstraintsTypeDef](./type_defs.md#scalingconstraintstypedef) 
3. See [:material-code-braces: ScalingRuleOutputTypeDef](./type_defs.md#scalingruleoutputtypedef) 
## InstanceFleetConfigTypeDef

```python
# InstanceFleetConfigTypeDef definition

class InstanceFleetConfigTypeDef(TypedDict):
    InstanceFleetType: InstanceFleetTypeType,  # (1)
    Name: NotRequired[str],
    TargetOnDemandCapacity: NotRequired[int],
    TargetSpotCapacity: NotRequired[int],
    InstanceTypeConfigs: NotRequired[Sequence[InstanceTypeConfigTypeDef]],  # (2)
    LaunchSpecifications: NotRequired[InstanceFleetProvisioningSpecificationsTypeDef],  # (3)
    ResizeSpecifications: NotRequired[InstanceFleetResizingSpecificationsTypeDef],  # (4)
    Context: NotRequired[str],
```

1. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
2. See [:material-code-braces: InstanceTypeConfigTypeDef](./type_defs.md#instancetypeconfigtypedef) 
3. See [:material-code-braces: InstanceFleetProvisioningSpecificationsTypeDef](./type_defs.md#instancefleetprovisioningspecificationstypedef) 
4. See [:material-code-braces: InstanceFleetResizingSpecificationsTypeDef](./type_defs.md#instancefleetresizingspecificationstypedef) 
## InstanceFleetModifyConfigTypeDef

```python
# InstanceFleetModifyConfigTypeDef definition

class InstanceFleetModifyConfigTypeDef(TypedDict):
    InstanceFleetId: str,
    TargetOnDemandCapacity: NotRequired[int],
    TargetSpotCapacity: NotRequired[int],
    ResizeSpecifications: NotRequired[InstanceFleetResizingSpecificationsTypeDef],  # (1)
    InstanceTypeConfigs: NotRequired[Sequence[InstanceTypeConfigTypeDef]],  # (2)
    Context: NotRequired[str],
```

1. See [:material-code-braces: InstanceFleetResizingSpecificationsTypeDef](./type_defs.md#instancefleetresizingspecificationstypedef) 
2. See [:material-code-braces: InstanceTypeConfigTypeDef](./type_defs.md#instancetypeconfigtypedef) 
## JobFlowDetailTypeDef

```python
# JobFlowDetailTypeDef definition

class JobFlowDetailTypeDef(TypedDict):
    JobFlowId: str,
    Name: str,
    ExecutionStatusDetail: JobFlowExecutionStatusDetailTypeDef,  # (1)
    Instances: JobFlowInstancesDetailTypeDef,  # (2)
    LogUri: NotRequired[str],
    LogEncryptionKmsKeyId: NotRequired[str],
    AmiVersion: NotRequired[str],
    Steps: NotRequired[List[StepDetailTypeDef]],  # (3)
    BootstrapActions: NotRequired[List[BootstrapActionDetailTypeDef]],  # (4)
    SupportedProducts: NotRequired[List[str]],
    VisibleToAllUsers: NotRequired[bool],
    JobFlowRole: NotRequired[str],
    ServiceRole: NotRequired[str],
    AutoScalingRole: NotRequired[str],
    ScaleDownBehavior: NotRequired[ScaleDownBehaviorType],  # (5)
```

1. See [:material-code-braces: JobFlowExecutionStatusDetailTypeDef](./type_defs.md#jobflowexecutionstatusdetailtypedef) 
2. See [:material-code-braces: JobFlowInstancesDetailTypeDef](./type_defs.md#jobflowinstancesdetailtypedef) 
3. See [:material-code-braces: StepDetailTypeDef](./type_defs.md#stepdetailtypedef) 
4. See [:material-code-braces: BootstrapActionDetailTypeDef](./type_defs.md#bootstrapactiondetailtypedef) 
5. See [:material-code-brackets: ScaleDownBehaviorType](./literals.md#scaledownbehaviortype) 
## InstanceGroupModifyConfigTypeDef

```python
# InstanceGroupModifyConfigTypeDef definition

class InstanceGroupModifyConfigTypeDef(TypedDict):
    InstanceGroupId: str,
    InstanceCount: NotRequired[int],
    EC2InstanceIdsToTerminate: NotRequired[Sequence[str]],
    ShrinkPolicy: NotRequired[ShrinkPolicyUnionTypeDef],  # (1)
    ReconfigurationType: NotRequired[ReconfigurationTypeType],  # (2)
    Configurations: NotRequired[Sequence[ConfigurationUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: ShrinkPolicyTypeDef](./type_defs.md#shrinkpolicytypedef) [:material-code-braces: ShrinkPolicyOutputTypeDef](./type_defs.md#shrinkpolicyoutputtypedef) 
2. See [:material-code-brackets: ReconfigurationTypeType](./literals.md#reconfigurationtypetype) 
3. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
## ListInstanceFleetsOutputPaginatorTypeDef

```python
# ListInstanceFleetsOutputPaginatorTypeDef definition

class ListInstanceFleetsOutputPaginatorTypeDef(TypedDict):
    InstanceFleets: List[InstanceFleetPaginatorTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceFleetPaginatorTypeDef](./type_defs.md#instancefleetpaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceFleetsOutputTypeDef

```python
# ListInstanceFleetsOutputTypeDef definition

class ListInstanceFleetsOutputTypeDef(TypedDict):
    InstanceFleets: List[InstanceFleetTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceFleetTypeDef](./type_defs.md#instancefleettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceGroupPaginatorTypeDef

```python
# InstanceGroupPaginatorTypeDef definition

class InstanceGroupPaginatorTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Market: NotRequired[MarketTypeType],  # (1)
    InstanceGroupType: NotRequired[InstanceGroupTypeType],  # (2)
    BidPrice: NotRequired[str],
    InstanceType: NotRequired[str],
    RequestedInstanceCount: NotRequired[int],
    RunningInstanceCount: NotRequired[int],
    Status: NotRequired[InstanceGroupStatusTypeDef],  # (3)
    Configurations: NotRequired[List[ConfigurationPaginatorTypeDef]],  # (4)
    ConfigurationsVersion: NotRequired[int],
    LastSuccessfullyAppliedConfigurations: NotRequired[List[ConfigurationPaginatorTypeDef]],  # (4)
    LastSuccessfullyAppliedConfigurationsVersion: NotRequired[int],
    EbsBlockDevices: NotRequired[List[EbsBlockDeviceTypeDef]],  # (6)
    EbsOptimized: NotRequired[bool],
    ShrinkPolicy: NotRequired[ShrinkPolicyOutputTypeDef],  # (7)
    AutoScalingPolicy: NotRequired[AutoScalingPolicyDescriptionTypeDef],  # (8)
    CustomAmiId: NotRequired[str],
```

1. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
2. See [:material-code-brackets: InstanceGroupTypeType](./literals.md#instancegrouptypetype) 
3. See [:material-code-braces: InstanceGroupStatusTypeDef](./type_defs.md#instancegroupstatustypedef) 
4. See [:material-code-braces: ConfigurationPaginatorTypeDef](./type_defs.md#configurationpaginatortypedef) 
5. See [:material-code-braces: ConfigurationPaginatorTypeDef](./type_defs.md#configurationpaginatortypedef) 
6. See [:material-code-braces: EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef) 
7. See [:material-code-braces: ShrinkPolicyOutputTypeDef](./type_defs.md#shrinkpolicyoutputtypedef) 
8. See [:material-code-braces: AutoScalingPolicyDescriptionTypeDef](./type_defs.md#autoscalingpolicydescriptiontypedef) 
## InstanceGroupTypeDef

```python
# InstanceGroupTypeDef definition

class InstanceGroupTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Market: NotRequired[MarketTypeType],  # (1)
    InstanceGroupType: NotRequired[InstanceGroupTypeType],  # (2)
    BidPrice: NotRequired[str],
    InstanceType: NotRequired[str],
    RequestedInstanceCount: NotRequired[int],
    RunningInstanceCount: NotRequired[int],
    Status: NotRequired[InstanceGroupStatusTypeDef],  # (3)
    Configurations: NotRequired[List[ConfigurationOutputTypeDef]],  # (4)
    ConfigurationsVersion: NotRequired[int],
    LastSuccessfullyAppliedConfigurations: NotRequired[List[ConfigurationOutputTypeDef]],  # (4)
    LastSuccessfullyAppliedConfigurationsVersion: NotRequired[int],
    EbsBlockDevices: NotRequired[List[EbsBlockDeviceTypeDef]],  # (6)
    EbsOptimized: NotRequired[bool],
    ShrinkPolicy: NotRequired[ShrinkPolicyOutputTypeDef],  # (7)
    AutoScalingPolicy: NotRequired[AutoScalingPolicyDescriptionTypeDef],  # (8)
    CustomAmiId: NotRequired[str],
```

1. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
2. See [:material-code-brackets: InstanceGroupTypeType](./literals.md#instancegrouptypetype) 
3. See [:material-code-braces: InstanceGroupStatusTypeDef](./type_defs.md#instancegroupstatustypedef) 
4. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
5. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
6. See [:material-code-braces: EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef) 
7. See [:material-code-braces: ShrinkPolicyOutputTypeDef](./type_defs.md#shrinkpolicyoutputtypedef) 
8. See [:material-code-braces: AutoScalingPolicyDescriptionTypeDef](./type_defs.md#autoscalingpolicydescriptiontypedef) 
## PutAutoScalingPolicyOutputTypeDef

```python
# PutAutoScalingPolicyOutputTypeDef definition

class PutAutoScalingPolicyOutputTypeDef(TypedDict):
    ClusterId: str,
    InstanceGroupId: str,
    AutoScalingPolicy: AutoScalingPolicyDescriptionTypeDef,  # (1)
    ClusterArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoScalingPolicyDescriptionTypeDef](./type_defs.md#autoscalingpolicydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScalingRuleTypeDef

```python
# ScalingRuleTypeDef definition

class ScalingRuleTypeDef(TypedDict):
    Name: str,
    Action: ScalingActionTypeDef,  # (1)
    Trigger: ScalingTriggerUnionTypeDef,  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ScalingActionTypeDef](./type_defs.md#scalingactiontypedef) 
2. See [:material-code-braces: ScalingTriggerTypeDef](./type_defs.md#scalingtriggertypedef) [:material-code-braces: ScalingTriggerOutputTypeDef](./type_defs.md#scalingtriggeroutputtypedef) 
## AddInstanceFleetInputRequestTypeDef

```python
# AddInstanceFleetInputRequestTypeDef definition

class AddInstanceFleetInputRequestTypeDef(TypedDict):
    ClusterId: str,
    InstanceFleet: InstanceFleetConfigTypeDef,  # (1)
```

1. See [:material-code-braces: InstanceFleetConfigTypeDef](./type_defs.md#instancefleetconfigtypedef) 
## ModifyInstanceFleetInputRequestTypeDef

```python
# ModifyInstanceFleetInputRequestTypeDef definition

class ModifyInstanceFleetInputRequestTypeDef(TypedDict):
    ClusterId: str,
    InstanceFleet: InstanceFleetModifyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: InstanceFleetModifyConfigTypeDef](./type_defs.md#instancefleetmodifyconfigtypedef) 
## DescribeJobFlowsOutputTypeDef

```python
# DescribeJobFlowsOutputTypeDef definition

class DescribeJobFlowsOutputTypeDef(TypedDict):
    JobFlows: List[JobFlowDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobFlowDetailTypeDef](./type_defs.md#jobflowdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddJobFlowStepsInputRequestTypeDef

```python
# AddJobFlowStepsInputRequestTypeDef definition

class AddJobFlowStepsInputRequestTypeDef(TypedDict):
    JobFlowId: str,
    Steps: Sequence[StepConfigUnionTypeDef],  # (1)
    ExecutionRoleArn: NotRequired[str],
```

1. See [:material-code-braces: StepConfigTypeDef](./type_defs.md#stepconfigtypedef) [:material-code-braces: StepConfigOutputTypeDef](./type_defs.md#stepconfigoutputtypedef) 
## ModifyInstanceGroupsInputRequestTypeDef

```python
# ModifyInstanceGroupsInputRequestTypeDef definition

class ModifyInstanceGroupsInputRequestTypeDef(TypedDict):
    ClusterId: NotRequired[str],
    InstanceGroups: NotRequired[Sequence[InstanceGroupModifyConfigTypeDef]],  # (1)
```

1. See [:material-code-braces: InstanceGroupModifyConfigTypeDef](./type_defs.md#instancegroupmodifyconfigtypedef) 
## ListInstanceGroupsOutputPaginatorTypeDef

```python
# ListInstanceGroupsOutputPaginatorTypeDef definition

class ListInstanceGroupsOutputPaginatorTypeDef(TypedDict):
    InstanceGroups: List[InstanceGroupPaginatorTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceGroupPaginatorTypeDef](./type_defs.md#instancegrouppaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceGroupsOutputTypeDef

```python
# ListInstanceGroupsOutputTypeDef definition

class ListInstanceGroupsOutputTypeDef(TypedDict):
    InstanceGroups: List[InstanceGroupTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceGroupTypeDef](./type_defs.md#instancegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoScalingPolicyTypeDef

```python
# AutoScalingPolicyTypeDef definition

class AutoScalingPolicyTypeDef(TypedDict):
    Constraints: ScalingConstraintsTypeDef,  # (1)
    Rules: Sequence[ScalingRuleUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ScalingConstraintsTypeDef](./type_defs.md#scalingconstraintstypedef) 
2. See [:material-code-braces: ScalingRuleTypeDef](./type_defs.md#scalingruletypedef) [:material-code-braces: ScalingRuleOutputTypeDef](./type_defs.md#scalingruleoutputtypedef) 
## InstanceGroupConfigTypeDef

```python
# InstanceGroupConfigTypeDef definition

class InstanceGroupConfigTypeDef(TypedDict):
    InstanceRole: InstanceRoleTypeType,  # (2)
    InstanceType: str,
    InstanceCount: int,
    Name: NotRequired[str],
    Market: NotRequired[MarketTypeType],  # (1)
    BidPrice: NotRequired[str],
    Configurations: NotRequired[Sequence[ConfigurationUnionTypeDef]],  # (3)
    EbsConfiguration: NotRequired[EbsConfigurationTypeDef],  # (4)
    AutoScalingPolicy: NotRequired[AutoScalingPolicyTypeDef],  # (5)
    CustomAmiId: NotRequired[str],
```

1. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
2. See [:material-code-brackets: InstanceRoleTypeType](./literals.md#instanceroletypetype) 
3. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
4. See [:material-code-braces: EbsConfigurationTypeDef](./type_defs.md#ebsconfigurationtypedef) 
5. See [:material-code-braces: AutoScalingPolicyTypeDef](./type_defs.md#autoscalingpolicytypedef) 
## PutAutoScalingPolicyInputRequestTypeDef

```python
# PutAutoScalingPolicyInputRequestTypeDef definition

class PutAutoScalingPolicyInputRequestTypeDef(TypedDict):
    ClusterId: str,
    InstanceGroupId: str,
    AutoScalingPolicy: AutoScalingPolicyTypeDef,  # (1)
```

1. See [:material-code-braces: AutoScalingPolicyTypeDef](./type_defs.md#autoscalingpolicytypedef) 
## AddInstanceGroupsInputRequestTypeDef

```python
# AddInstanceGroupsInputRequestTypeDef definition

class AddInstanceGroupsInputRequestTypeDef(TypedDict):
    InstanceGroups: Sequence[InstanceGroupConfigTypeDef],  # (1)
    JobFlowId: str,
```

1. See [:material-code-braces: InstanceGroupConfigTypeDef](./type_defs.md#instancegroupconfigtypedef) 
## JobFlowInstancesConfigTypeDef

```python
# JobFlowInstancesConfigTypeDef definition

class JobFlowInstancesConfigTypeDef(TypedDict):
    MasterInstanceType: NotRequired[str],
    SlaveInstanceType: NotRequired[str],
    InstanceCount: NotRequired[int],
    InstanceGroups: NotRequired[Sequence[InstanceGroupConfigTypeDef]],  # (1)
    InstanceFleets: NotRequired[Sequence[InstanceFleetConfigTypeDef]],  # (2)
    Ec2KeyName: NotRequired[str],
    Placement: NotRequired[PlacementTypeUnionTypeDef],  # (3)
    KeepJobFlowAliveWhenNoSteps: NotRequired[bool],
    TerminationProtected: NotRequired[bool],
    UnhealthyNodeReplacement: NotRequired[bool],
    HadoopVersion: NotRequired[str],
    Ec2SubnetId: NotRequired[str],
    Ec2SubnetIds: NotRequired[Sequence[str]],
    EmrManagedMasterSecurityGroup: NotRequired[str],
    EmrManagedSlaveSecurityGroup: NotRequired[str],
    ServiceAccessSecurityGroup: NotRequired[str],
    AdditionalMasterSecurityGroups: NotRequired[Sequence[str]],
    AdditionalSlaveSecurityGroups: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: InstanceGroupConfigTypeDef](./type_defs.md#instancegroupconfigtypedef) 
2. See [:material-code-braces: InstanceFleetConfigTypeDef](./type_defs.md#instancefleetconfigtypedef) 
3. See [:material-code-braces: PlacementTypeTypeDef](./type_defs.md#placementtypetypedef) [:material-code-braces: PlacementTypeOutputTypeDef](./type_defs.md#placementtypeoutputtypedef) 
## RunJobFlowInputRequestTypeDef

```python
# RunJobFlowInputRequestTypeDef definition

class RunJobFlowInputRequestTypeDef(TypedDict):
    Name: str,
    Instances: JobFlowInstancesConfigTypeDef,  # (1)
    LogUri: NotRequired[str],
    LogEncryptionKmsKeyId: NotRequired[str],
    AdditionalInfo: NotRequired[str],
    AmiVersion: NotRequired[str],
    ReleaseLabel: NotRequired[str],
    Steps: NotRequired[Sequence[StepConfigTypeDef]],  # (2)
    BootstrapActions: NotRequired[Sequence[BootstrapActionConfigUnionTypeDef]],  # (3)
    SupportedProducts: NotRequired[Sequence[str]],
    NewSupportedProducts: NotRequired[Sequence[SupportedProductConfigTypeDef]],  # (4)
    Applications: NotRequired[Sequence[ApplicationUnionTypeDef]],  # (5)
    Configurations: NotRequired[Sequence[ConfigurationUnionTypeDef]],  # (6)
    VisibleToAllUsers: NotRequired[bool],
    JobFlowRole: NotRequired[str],
    ServiceRole: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (7)
    SecurityConfiguration: NotRequired[str],
    AutoScalingRole: NotRequired[str],
    ScaleDownBehavior: NotRequired[ScaleDownBehaviorType],  # (8)
    CustomAmiId: NotRequired[str],
    EbsRootVolumeSize: NotRequired[int],
    RepoUpgradeOnBoot: NotRequired[RepoUpgradeOnBootType],  # (9)
    KerberosAttributes: NotRequired[KerberosAttributesTypeDef],  # (10)
    StepConcurrencyLevel: NotRequired[int],
    ManagedScalingPolicy: NotRequired[ManagedScalingPolicyTypeDef],  # (11)
    PlacementGroupConfigs: NotRequired[Sequence[PlacementGroupConfigTypeDef]],  # (12)
    AutoTerminationPolicy: NotRequired[AutoTerminationPolicyTypeDef],  # (13)
    OSReleaseLabel: NotRequired[str],
    EbsRootVolumeIops: NotRequired[int],
    EbsRootVolumeThroughput: NotRequired[int],
```

1. See [:material-code-braces: JobFlowInstancesConfigTypeDef](./type_defs.md#jobflowinstancesconfigtypedef) 
2. See [:material-code-braces: StepConfigTypeDef](./type_defs.md#stepconfigtypedef) 
3. See [:material-code-braces: BootstrapActionConfigTypeDef](./type_defs.md#bootstrapactionconfigtypedef) [:material-code-braces: BootstrapActionConfigOutputTypeDef](./type_defs.md#bootstrapactionconfigoutputtypedef) 
4. See [:material-code-braces: SupportedProductConfigTypeDef](./type_defs.md#supportedproductconfigtypedef) 
5. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) [:material-code-braces: ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef) 
6. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-brackets: ScaleDownBehaviorType](./literals.md#scaledownbehaviortype) 
9. See [:material-code-brackets: RepoUpgradeOnBootType](./literals.md#repoupgradeonboottype) 
10. See [:material-code-braces: KerberosAttributesTypeDef](./type_defs.md#kerberosattributestypedef) 
11. See [:material-code-braces: ManagedScalingPolicyTypeDef](./type_defs.md#managedscalingpolicytypedef) 
12. See [:material-code-braces: PlacementGroupConfigTypeDef](./type_defs.md#placementgroupconfigtypedef) 
13. See [:material-code-braces: AutoTerminationPolicyTypeDef](./type_defs.md#autoterminationpolicytypedef) 
