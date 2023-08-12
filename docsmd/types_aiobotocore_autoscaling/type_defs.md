# Type definitions

> [Index](../README.md) > [AutoScaling](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
    type annotations stubs module [types-aiobotocore-autoscaling](https://pypi.org/project/types-aiobotocore-autoscaling/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AcceleratorCountRequestTypeDef

```python
# AcceleratorCountRequestTypeDef definition

class AcceleratorCountRequestTypeDef(TypedDict):
    Min: NotRequired[int],
    Max: NotRequired[int],
```

## AcceleratorTotalMemoryMiBRequestTypeDef

```python
# AcceleratorTotalMemoryMiBRequestTypeDef definition

class AcceleratorTotalMemoryMiBRequestTypeDef(TypedDict):
    Min: NotRequired[int],
    Max: NotRequired[int],
```

## ActivityTypeDef

```python
# ActivityTypeDef definition

class ActivityTypeDef(TypedDict):
    ActivityId: str,
    AutoScalingGroupName: str,
    Cause: str,
    StartTime: datetime,
    StatusCode: ScalingActivityStatusCodeType,  # (1)
    Description: NotRequired[str],
    EndTime: NotRequired[datetime],
    StatusMessage: NotRequired[str],
    Progress: NotRequired[int],
    Details: NotRequired[str],
    AutoScalingGroupState: NotRequired[str],
    AutoScalingGroupARN: NotRequired[str],
```

1. See [:material-code-brackets: ScalingActivityStatusCodeType](./literals.md#scalingactivitystatuscodetype) 
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

## AdjustmentTypeTypeDef

```python
# AdjustmentTypeTypeDef definition

class AdjustmentTypeTypeDef(TypedDict):
    AdjustmentType: NotRequired[str],
```

## AlarmSpecificationTypeDef

```python
# AlarmSpecificationTypeDef definition

class AlarmSpecificationTypeDef(TypedDict):
    Alarms: NotRequired[List[str]],
```

## AlarmTypeDef

```python
# AlarmTypeDef definition

class AlarmTypeDef(TypedDict):
    AlarmName: NotRequired[str],
    AlarmARN: NotRequired[str],
```

## AttachInstancesQueryRequestTypeDef

```python
# AttachInstancesQueryRequestTypeDef definition

class AttachInstancesQueryRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    InstanceIds: NotRequired[Sequence[str]],
```

## AttachLoadBalancerTargetGroupsTypeRequestTypeDef

```python
# AttachLoadBalancerTargetGroupsTypeRequestTypeDef definition

class AttachLoadBalancerTargetGroupsTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    TargetGroupARNs: Sequence[str],
```

## AttachLoadBalancersTypeRequestTypeDef

```python
# AttachLoadBalancersTypeRequestTypeDef definition

class AttachLoadBalancersTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    LoadBalancerNames: Sequence[str],
```

## TrafficSourceIdentifierTypeDef

```python
# TrafficSourceIdentifierTypeDef definition

class TrafficSourceIdentifierTypeDef(TypedDict):
    Identifier: str,
    Type: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## EnabledMetricTypeDef

```python
# EnabledMetricTypeDef definition

class EnabledMetricTypeDef(TypedDict):
    Metric: NotRequired[str],
    Granularity: NotRequired[str],
```

## LaunchTemplateSpecificationTypeDef

```python
# LaunchTemplateSpecificationTypeDef definition

class LaunchTemplateSpecificationTypeDef(TypedDict):
    LaunchTemplateId: NotRequired[str],
    LaunchTemplateName: NotRequired[str],
    Version: NotRequired[str],
```

## SuspendedProcessTypeDef

```python
# SuspendedProcessTypeDef definition

class SuspendedProcessTypeDef(TypedDict):
    ProcessName: NotRequired[str],
    SuspensionReason: NotRequired[str],
```

## TagDescriptionTypeDef

```python
# TagDescriptionTypeDef definition

class TagDescriptionTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    ResourceType: NotRequired[str],
    Key: NotRequired[str],
    Value: NotRequired[str],
    PropagateAtLaunch: NotRequired[bool],
```

## BaselineEbsBandwidthMbpsRequestTypeDef

```python
# BaselineEbsBandwidthMbpsRequestTypeDef definition

class BaselineEbsBandwidthMbpsRequestTypeDef(TypedDict):
    Min: NotRequired[int],
    Max: NotRequired[int],
```

## FailedScheduledUpdateGroupActionRequestTypeDef

```python
# FailedScheduledUpdateGroupActionRequestTypeDef definition

class FailedScheduledUpdateGroupActionRequestTypeDef(TypedDict):
    ScheduledActionName: str,
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## BatchDeleteScheduledActionTypeRequestTypeDef

```python
# BatchDeleteScheduledActionTypeRequestTypeDef definition

class BatchDeleteScheduledActionTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    ScheduledActionNames: Sequence[str],
```

## EbsTypeDef

```python
# EbsTypeDef definition

class EbsTypeDef(TypedDict):
    SnapshotId: NotRequired[str],
    VolumeSize: NotRequired[int],
    VolumeType: NotRequired[str],
    DeleteOnTermination: NotRequired[bool],
    Iops: NotRequired[int],
    Encrypted: NotRequired[bool],
    Throughput: NotRequired[int],
```

## CancelInstanceRefreshTypeRequestTypeDef

```python
# CancelInstanceRefreshTypeRequestTypeDef definition

class CancelInstanceRefreshTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
```

## CapacityForecastTypeDef

```python
# CapacityForecastTypeDef definition

class CapacityForecastTypeDef(TypedDict):
    Timestamps: List[datetime],
    Values: List[float],
```

## CompleteLifecycleActionTypeRequestTypeDef

```python
# CompleteLifecycleActionTypeRequestTypeDef definition

class CompleteLifecycleActionTypeRequestTypeDef(TypedDict):
    LifecycleHookName: str,
    AutoScalingGroupName: str,
    LifecycleActionResult: str,
    LifecycleActionToken: NotRequired[str],
    InstanceId: NotRequired[str],
```

## LifecycleHookSpecificationTypeDef

```python
# LifecycleHookSpecificationTypeDef definition

class LifecycleHookSpecificationTypeDef(TypedDict):
    LifecycleHookName: str,
    LifecycleTransition: str,
    NotificationMetadata: NotRequired[str],
    HeartbeatTimeout: NotRequired[int],
    DefaultResult: NotRequired[str],
    NotificationTargetARN: NotRequired[str],
    RoleARN: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    ResourceId: NotRequired[str],
    ResourceType: NotRequired[str],
    Value: NotRequired[str],
    PropagateAtLaunch: NotRequired[bool],
```

## InstanceMetadataOptionsTypeDef

```python
# InstanceMetadataOptionsTypeDef definition

class InstanceMetadataOptionsTypeDef(TypedDict):
    HttpTokens: NotRequired[InstanceMetadataHttpTokensStateType],  # (1)
    HttpPutResponseHopLimit: NotRequired[int],
    HttpEndpoint: NotRequired[InstanceMetadataEndpointStateType],  # (2)
```

1. See [:material-code-brackets: InstanceMetadataHttpTokensStateType](./literals.md#instancemetadatahttptokensstatetype) 
2. See [:material-code-brackets: InstanceMetadataEndpointStateType](./literals.md#instancemetadataendpointstatetype) 
## InstanceMonitoringTypeDef

```python
# InstanceMonitoringTypeDef definition

class InstanceMonitoringTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## MetricDimensionTypeDef

```python
# MetricDimensionTypeDef definition

class MetricDimensionTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## DeleteAutoScalingGroupTypeRequestTypeDef

```python
# DeleteAutoScalingGroupTypeRequestTypeDef definition

class DeleteAutoScalingGroupTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    ForceDelete: NotRequired[bool],
```

## DeleteLifecycleHookTypeRequestTypeDef

```python
# DeleteLifecycleHookTypeRequestTypeDef definition

class DeleteLifecycleHookTypeRequestTypeDef(TypedDict):
    LifecycleHookName: str,
    AutoScalingGroupName: str,
```

## DeleteNotificationConfigurationTypeRequestTypeDef

```python
# DeleteNotificationConfigurationTypeRequestTypeDef definition

class DeleteNotificationConfigurationTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    TopicARN: str,
```

## DeletePolicyTypeRequestTypeDef

```python
# DeletePolicyTypeRequestTypeDef definition

class DeletePolicyTypeRequestTypeDef(TypedDict):
    PolicyName: str,
    AutoScalingGroupName: NotRequired[str],
```

## DeleteScheduledActionTypeRequestTypeDef

```python
# DeleteScheduledActionTypeRequestTypeDef definition

class DeleteScheduledActionTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    ScheduledActionName: str,
```

## DeleteWarmPoolTypeRequestTypeDef

```python
# DeleteWarmPoolTypeRequestTypeDef definition

class DeleteWarmPoolTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    ForceDelete: NotRequired[bool],
```

## DescribeAutoScalingInstancesTypeRequestTypeDef

```python
# DescribeAutoScalingInstancesTypeRequestTypeDef definition

class DescribeAutoScalingInstancesTypeRequestTypeDef(TypedDict):
    InstanceIds: NotRequired[Sequence[str]],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeInstanceRefreshesTypeRequestTypeDef

```python
# DescribeInstanceRefreshesTypeRequestTypeDef definition

class DescribeInstanceRefreshesTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    InstanceRefreshIds: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxRecords: NotRequired[int],
```

## LifecycleHookTypeDef

```python
# LifecycleHookTypeDef definition

class LifecycleHookTypeDef(TypedDict):
    LifecycleHookName: NotRequired[str],
    AutoScalingGroupName: NotRequired[str],
    LifecycleTransition: NotRequired[str],
    NotificationTargetARN: NotRequired[str],
    RoleARN: NotRequired[str],
    NotificationMetadata: NotRequired[str],
    HeartbeatTimeout: NotRequired[int],
    GlobalTimeout: NotRequired[int],
    DefaultResult: NotRequired[str],
```

## DescribeLifecycleHooksTypeRequestTypeDef

```python
# DescribeLifecycleHooksTypeRequestTypeDef definition

class DescribeLifecycleHooksTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    LifecycleHookNames: NotRequired[Sequence[str]],
```

## DescribeLoadBalancerTargetGroupsRequestRequestTypeDef

```python
# DescribeLoadBalancerTargetGroupsRequestRequestTypeDef definition

class DescribeLoadBalancerTargetGroupsRequestRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    NextToken: NotRequired[str],
    MaxRecords: NotRequired[int],
```

## LoadBalancerTargetGroupStateTypeDef

```python
# LoadBalancerTargetGroupStateTypeDef definition

class LoadBalancerTargetGroupStateTypeDef(TypedDict):
    LoadBalancerTargetGroupARN: NotRequired[str],
    State: NotRequired[str],
```

## DescribeLoadBalancersRequestRequestTypeDef

```python
# DescribeLoadBalancersRequestRequestTypeDef definition

class DescribeLoadBalancersRequestRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    NextToken: NotRequired[str],
    MaxRecords: NotRequired[int],
```

## LoadBalancerStateTypeDef

```python
# LoadBalancerStateTypeDef definition

class LoadBalancerStateTypeDef(TypedDict):
    LoadBalancerName: NotRequired[str],
    State: NotRequired[str],
```

## MetricCollectionTypeTypeDef

```python
# MetricCollectionTypeTypeDef definition

class MetricCollectionTypeTypeDef(TypedDict):
    Metric: NotRequired[str],
```

## MetricGranularityTypeTypeDef

```python
# MetricGranularityTypeTypeDef definition

class MetricGranularityTypeTypeDef(TypedDict):
    Granularity: NotRequired[str],
```

## NotificationConfigurationTypeDef

```python
# NotificationConfigurationTypeDef definition

class NotificationConfigurationTypeDef(TypedDict):
    AutoScalingGroupName: NotRequired[str],
    TopicARN: NotRequired[str],
    NotificationType: NotRequired[str],
```

## DescribeNotificationConfigurationsTypeRequestTypeDef

```python
# DescribeNotificationConfigurationsTypeRequestTypeDef definition

class DescribeNotificationConfigurationsTypeRequestTypeDef(TypedDict):
    AutoScalingGroupNames: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxRecords: NotRequired[int],
```

## DescribePoliciesTypeRequestTypeDef

```python
# DescribePoliciesTypeRequestTypeDef definition

class DescribePoliciesTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: NotRequired[str],
    PolicyNames: NotRequired[Sequence[str]],
    PolicyTypes: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxRecords: NotRequired[int],
```

## DescribeScalingActivitiesTypeRequestTypeDef

```python
# DescribeScalingActivitiesTypeRequestTypeDef definition

class DescribeScalingActivitiesTypeRequestTypeDef(TypedDict):
    ActivityIds: NotRequired[Sequence[str]],
    AutoScalingGroupName: NotRequired[str],
    IncludeDeletedGroups: NotRequired[bool],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeTrafficSourcesRequestRequestTypeDef

```python
# DescribeTrafficSourcesRequestRequestTypeDef definition

class DescribeTrafficSourcesRequestRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    TrafficSourceType: NotRequired[str],
    NextToken: NotRequired[str],
    MaxRecords: NotRequired[int],
```

## TrafficSourceStateTypeDef

```python
# TrafficSourceStateTypeDef definition

class TrafficSourceStateTypeDef(TypedDict):
    TrafficSource: NotRequired[str],
    State: NotRequired[str],
    Identifier: NotRequired[str],
    Type: NotRequired[str],
```

## DescribeWarmPoolTypeRequestTypeDef

```python
# DescribeWarmPoolTypeRequestTypeDef definition

class DescribeWarmPoolTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

## DetachInstancesQueryRequestTypeDef

```python
# DetachInstancesQueryRequestTypeDef definition

class DetachInstancesQueryRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    ShouldDecrementDesiredCapacity: bool,
    InstanceIds: NotRequired[Sequence[str]],
```

## DetachLoadBalancerTargetGroupsTypeRequestTypeDef

```python
# DetachLoadBalancerTargetGroupsTypeRequestTypeDef definition

class DetachLoadBalancerTargetGroupsTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    TargetGroupARNs: Sequence[str],
```

## DetachLoadBalancersTypeRequestTypeDef

```python
# DetachLoadBalancersTypeRequestTypeDef definition

class DetachLoadBalancersTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    LoadBalancerNames: Sequence[str],
```

## DisableMetricsCollectionQueryRequestTypeDef

```python
# DisableMetricsCollectionQueryRequestTypeDef definition

class DisableMetricsCollectionQueryRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    Metrics: NotRequired[Sequence[str]],
```

## EnableMetricsCollectionQueryRequestTypeDef

```python
# EnableMetricsCollectionQueryRequestTypeDef definition

class EnableMetricsCollectionQueryRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    Granularity: str,
    Metrics: NotRequired[Sequence[str]],
```

## EnterStandbyQueryRequestTypeDef

```python
# EnterStandbyQueryRequestTypeDef definition

class EnterStandbyQueryRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    ShouldDecrementDesiredCapacity: bool,
    InstanceIds: NotRequired[Sequence[str]],
```

## ExecutePolicyTypeRequestTypeDef

```python
# ExecutePolicyTypeRequestTypeDef definition

class ExecutePolicyTypeRequestTypeDef(TypedDict):
    PolicyName: str,
    AutoScalingGroupName: NotRequired[str],
    HonorCooldown: NotRequired[bool],
    MetricValue: NotRequired[float],
    BreachThreshold: NotRequired[float],
```

## ExitStandbyQueryRequestTypeDef

```python
# ExitStandbyQueryRequestTypeDef definition

class ExitStandbyQueryRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    InstanceIds: NotRequired[Sequence[str]],
```

## InstanceRefreshLivePoolProgressTypeDef

```python
# InstanceRefreshLivePoolProgressTypeDef definition

class InstanceRefreshLivePoolProgressTypeDef(TypedDict):
    PercentageComplete: NotRequired[int],
    InstancesToUpdate: NotRequired[int],
```

## InstanceRefreshWarmPoolProgressTypeDef

```python
# InstanceRefreshWarmPoolProgressTypeDef definition

class InstanceRefreshWarmPoolProgressTypeDef(TypedDict):
    PercentageComplete: NotRequired[int],
    InstancesToUpdate: NotRequired[int],
```

## MemoryGiBPerVCpuRequestTypeDef

```python
# MemoryGiBPerVCpuRequestTypeDef definition

class MemoryGiBPerVCpuRequestTypeDef(TypedDict):
    Min: NotRequired[float],
    Max: NotRequired[float],
```

## MemoryMiBRequestTypeDef

```python
# MemoryMiBRequestTypeDef definition

class MemoryMiBRequestTypeDef(TypedDict):
    Min: int,
    Max: NotRequired[int],
```

## NetworkBandwidthGbpsRequestTypeDef

```python
# NetworkBandwidthGbpsRequestTypeDef definition

class NetworkBandwidthGbpsRequestTypeDef(TypedDict):
    Min: NotRequired[float],
    Max: NotRequired[float],
```

## NetworkInterfaceCountRequestTypeDef

```python
# NetworkInterfaceCountRequestTypeDef definition

class NetworkInterfaceCountRequestTypeDef(TypedDict):
    Min: NotRequired[int],
    Max: NotRequired[int],
```

## TotalLocalStorageGBRequestTypeDef

```python
# TotalLocalStorageGBRequestTypeDef definition

class TotalLocalStorageGBRequestTypeDef(TypedDict):
    Min: NotRequired[float],
    Max: NotRequired[float],
```

## VCpuCountRequestTypeDef

```python
# VCpuCountRequestTypeDef definition

class VCpuCountRequestTypeDef(TypedDict):
    Min: int,
    Max: NotRequired[int],
```

## InstanceReusePolicyTypeDef

```python
# InstanceReusePolicyTypeDef definition

class InstanceReusePolicyTypeDef(TypedDict):
    ReuseOnScaleIn: NotRequired[bool],
```

## InstancesDistributionTypeDef

```python
# InstancesDistributionTypeDef definition

class InstancesDistributionTypeDef(TypedDict):
    OnDemandAllocationStrategy: NotRequired[str],
    OnDemandBaseCapacity: NotRequired[int],
    OnDemandPercentageAboveBaseCapacity: NotRequired[int],
    SpotAllocationStrategy: NotRequired[str],
    SpotInstancePools: NotRequired[int],
    SpotMaxPrice: NotRequired[str],
```

## LaunchConfigurationNameTypeRequestTypeDef

```python
# LaunchConfigurationNameTypeRequestTypeDef definition

class LaunchConfigurationNameTypeRequestTypeDef(TypedDict):
    LaunchConfigurationName: str,
```

## LaunchConfigurationNamesTypeRequestTypeDef

```python
# LaunchConfigurationNamesTypeRequestTypeDef definition

class LaunchConfigurationNamesTypeRequestTypeDef(TypedDict):
    LaunchConfigurationNames: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxRecords: NotRequired[int],
```

## PredefinedMetricSpecificationTypeDef

```python
# PredefinedMetricSpecificationTypeDef definition

class PredefinedMetricSpecificationTypeDef(TypedDict):
    PredefinedMetricType: MetricTypeType,  # (1)
    ResourceLabel: NotRequired[str],
```

1. See [:material-code-brackets: MetricTypeType](./literals.md#metrictypetype) 
## PredictiveScalingPredefinedLoadMetricTypeDef

```python
# PredictiveScalingPredefinedLoadMetricTypeDef definition

class PredictiveScalingPredefinedLoadMetricTypeDef(TypedDict):
    PredefinedMetricType: PredefinedLoadMetricTypeType,  # (1)
    ResourceLabel: NotRequired[str],
```

1. See [:material-code-brackets: PredefinedLoadMetricTypeType](./literals.md#predefinedloadmetrictypetype) 
## PredictiveScalingPredefinedMetricPairTypeDef

```python
# PredictiveScalingPredefinedMetricPairTypeDef definition

class PredictiveScalingPredefinedMetricPairTypeDef(TypedDict):
    PredefinedMetricType: PredefinedMetricPairTypeType,  # (1)
    ResourceLabel: NotRequired[str],
```

1. See [:material-code-brackets: PredefinedMetricPairTypeType](./literals.md#predefinedmetricpairtypetype) 
## PredictiveScalingPredefinedScalingMetricTypeDef

```python
# PredictiveScalingPredefinedScalingMetricTypeDef definition

class PredictiveScalingPredefinedScalingMetricTypeDef(TypedDict):
    PredefinedMetricType: PredefinedScalingMetricTypeType,  # (1)
    ResourceLabel: NotRequired[str],
```

1. See [:material-code-brackets: PredefinedScalingMetricTypeType](./literals.md#predefinedscalingmetrictypetype) 
## ProcessTypeTypeDef

```python
# ProcessTypeTypeDef definition

class ProcessTypeTypeDef(TypedDict):
    ProcessName: str,
```

## PutLifecycleHookTypeRequestTypeDef

```python
# PutLifecycleHookTypeRequestTypeDef definition

class PutLifecycleHookTypeRequestTypeDef(TypedDict):
    LifecycleHookName: str,
    AutoScalingGroupName: str,
    LifecycleTransition: NotRequired[str],
    RoleARN: NotRequired[str],
    NotificationTargetARN: NotRequired[str],
    NotificationMetadata: NotRequired[str],
    HeartbeatTimeout: NotRequired[int],
    DefaultResult: NotRequired[str],
```

## PutNotificationConfigurationTypeRequestTypeDef

```python
# PutNotificationConfigurationTypeRequestTypeDef definition

class PutNotificationConfigurationTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    TopicARN: str,
    NotificationTypes: Sequence[str],
```

## StepAdjustmentTypeDef

```python
# StepAdjustmentTypeDef definition

class StepAdjustmentTypeDef(TypedDict):
    ScalingAdjustment: int,
    MetricIntervalLowerBound: NotRequired[float],
    MetricIntervalUpperBound: NotRequired[float],
```

## RecordLifecycleActionHeartbeatTypeRequestTypeDef

```python
# RecordLifecycleActionHeartbeatTypeRequestTypeDef definition

class RecordLifecycleActionHeartbeatTypeRequestTypeDef(TypedDict):
    LifecycleHookName: str,
    AutoScalingGroupName: str,
    LifecycleActionToken: NotRequired[str],
    InstanceId: NotRequired[str],
```

## RollbackInstanceRefreshTypeRequestTypeDef

```python
# RollbackInstanceRefreshTypeRequestTypeDef definition

class RollbackInstanceRefreshTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
```

## ScalingProcessQueryRequestTypeDef

```python
# ScalingProcessQueryRequestTypeDef definition

class ScalingProcessQueryRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    ScalingProcesses: NotRequired[Sequence[str]],
```

## ScheduledUpdateGroupActionTypeDef

```python
# ScheduledUpdateGroupActionTypeDef definition

class ScheduledUpdateGroupActionTypeDef(TypedDict):
    AutoScalingGroupName: NotRequired[str],
    ScheduledActionName: NotRequired[str],
    ScheduledActionARN: NotRequired[str],
    Time: NotRequired[datetime],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Recurrence: NotRequired[str],
    MinSize: NotRequired[int],
    MaxSize: NotRequired[int],
    DesiredCapacity: NotRequired[int],
    TimeZone: NotRequired[str],
```

## SetDesiredCapacityTypeRequestTypeDef

```python
# SetDesiredCapacityTypeRequestTypeDef definition

class SetDesiredCapacityTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    DesiredCapacity: int,
    HonorCooldown: NotRequired[bool],
```

## SetInstanceHealthQueryRequestTypeDef

```python
# SetInstanceHealthQueryRequestTypeDef definition

class SetInstanceHealthQueryRequestTypeDef(TypedDict):
    InstanceId: str,
    HealthStatus: str,
    ShouldRespectGracePeriod: NotRequired[bool],
```

## SetInstanceProtectionQueryRequestTypeDef

```python
# SetInstanceProtectionQueryRequestTypeDef definition

class SetInstanceProtectionQueryRequestTypeDef(TypedDict):
    InstanceIds: Sequence[str],
    AutoScalingGroupName: str,
    ProtectedFromScaleIn: bool,
```

## TerminateInstanceInAutoScalingGroupTypeRequestTypeDef

```python
# TerminateInstanceInAutoScalingGroupTypeRequestTypeDef definition

class TerminateInstanceInAutoScalingGroupTypeRequestTypeDef(TypedDict):
    InstanceId: str,
    ShouldDecrementDesiredCapacity: bool,
```

## ActivitiesTypeTypeDef

```python
# ActivitiesTypeTypeDef definition

class ActivitiesTypeTypeDef(TypedDict):
    Activities: List[ActivityTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActivityTypeDef](./type_defs.md#activitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActivityTypeTypeDef

```python
# ActivityTypeTypeDef definition

class ActivityTypeTypeDef(TypedDict):
    Activity: ActivityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActivityTypeDef](./type_defs.md#activitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelInstanceRefreshAnswerTypeDef

```python
# CancelInstanceRefreshAnswerTypeDef definition

class CancelInstanceRefreshAnswerTypeDef(TypedDict):
    InstanceRefreshId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountLimitsAnswerTypeDef

```python
# DescribeAccountLimitsAnswerTypeDef definition

class DescribeAccountLimitsAnswerTypeDef(TypedDict):
    MaxNumberOfAutoScalingGroups: int,
    MaxNumberOfLaunchConfigurations: int,
    NumberOfAutoScalingGroups: int,
    NumberOfLaunchConfigurations: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAutoScalingNotificationTypesAnswerTypeDef

```python
# DescribeAutoScalingNotificationTypesAnswerTypeDef definition

class DescribeAutoScalingNotificationTypesAnswerTypeDef(TypedDict):
    AutoScalingNotificationTypes: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLifecycleHookTypesAnswerTypeDef

```python
# DescribeLifecycleHookTypesAnswerTypeDef definition

class DescribeLifecycleHookTypesAnswerTypeDef(TypedDict):
    LifecycleHookTypes: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTerminationPolicyTypesAnswerTypeDef

```python
# DescribeTerminationPolicyTypesAnswerTypeDef definition

class DescribeTerminationPolicyTypesAnswerTypeDef(TypedDict):
    TerminationPolicyTypes: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetachInstancesAnswerTypeDef

```python
# DetachInstancesAnswerTypeDef definition

class DetachInstancesAnswerTypeDef(TypedDict):
    Activities: List[ActivityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActivityTypeDef](./type_defs.md#activitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnterStandbyAnswerTypeDef

```python
# EnterStandbyAnswerTypeDef definition

class EnterStandbyAnswerTypeDef(TypedDict):
    Activities: List[ActivityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActivityTypeDef](./type_defs.md#activitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExitStandbyAnswerTypeDef

```python
# ExitStandbyAnswerTypeDef definition

class ExitStandbyAnswerTypeDef(TypedDict):
    Activities: List[ActivityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActivityTypeDef](./type_defs.md#activitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RollbackInstanceRefreshAnswerTypeDef

```python
# RollbackInstanceRefreshAnswerTypeDef definition

class RollbackInstanceRefreshAnswerTypeDef(TypedDict):
    InstanceRefreshId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartInstanceRefreshAnswerTypeDef

```python
# StartInstanceRefreshAnswerTypeDef definition

class StartInstanceRefreshAnswerTypeDef(TypedDict):
    InstanceRefreshId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAdjustmentTypesAnswerTypeDef

```python
# DescribeAdjustmentTypesAnswerTypeDef definition

class DescribeAdjustmentTypesAnswerTypeDef(TypedDict):
    AdjustmentTypes: List[AdjustmentTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AdjustmentTypeTypeDef](./type_defs.md#adjustmenttypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RefreshPreferencesTypeDef

```python
# RefreshPreferencesTypeDef definition

class RefreshPreferencesTypeDef(TypedDict):
    MinHealthyPercentage: NotRequired[int],
    InstanceWarmup: NotRequired[int],
    CheckpointPercentages: NotRequired[List[int]],
    CheckpointDelay: NotRequired[int],
    SkipMatching: NotRequired[bool],
    AutoRollback: NotRequired[bool],
    ScaleInProtectedInstances: NotRequired[ScaleInProtectedInstancesType],  # (1)
    StandbyInstances: NotRequired[StandbyInstancesType],  # (2)
    AlarmSpecification: NotRequired[AlarmSpecificationTypeDef],  # (3)
```

1. See [:material-code-brackets: ScaleInProtectedInstancesType](./literals.md#scaleinprotectedinstancestype) 
2. See [:material-code-brackets: StandbyInstancesType](./literals.md#standbyinstancestype) 
3. See [:material-code-braces: AlarmSpecificationTypeDef](./type_defs.md#alarmspecificationtypedef) 
## PolicyARNTypeTypeDef

```python
# PolicyARNTypeTypeDef definition

class PolicyARNTypeTypeDef(TypedDict):
    PolicyARN: str,
    Alarms: List[AlarmTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachTrafficSourcesTypeRequestTypeDef

```python
# AttachTrafficSourcesTypeRequestTypeDef definition

class AttachTrafficSourcesTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    TrafficSources: Sequence[TrafficSourceIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: TrafficSourceIdentifierTypeDef](./type_defs.md#trafficsourceidentifiertypedef) 
## DetachTrafficSourcesTypeRequestTypeDef

```python
# DetachTrafficSourcesTypeRequestTypeDef definition

class DetachTrafficSourcesTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    TrafficSources: Sequence[TrafficSourceIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: TrafficSourceIdentifierTypeDef](./type_defs.md#trafficsourceidentifiertypedef) 
## AutoScalingGroupNamesTypeRequestTypeDef

```python
# AutoScalingGroupNamesTypeRequestTypeDef definition

class AutoScalingGroupNamesTypeRequestTypeDef(TypedDict):
    AutoScalingGroupNames: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxRecords: NotRequired[int],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeTagsTypeRequestTypeDef

```python
# DescribeTagsTypeRequestTypeDef definition

class DescribeTagsTypeRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef

```python
# AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef definition

class AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef(TypedDict):
    AutoScalingGroupNames: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef

```python
# DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef definition

class DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef(TypedDict):
    InstanceIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef

```python
# DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef definition

class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(TypedDict):
    AutoScalingGroupName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef

```python
# DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef definition

class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(TypedDict):
    AutoScalingGroupName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef

```python
# DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef definition

class DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef(TypedDict):
    AutoScalingGroupNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePoliciesTypeDescribePoliciesPaginateTypeDef

```python
# DescribePoliciesTypeDescribePoliciesPaginateTypeDef definition

class DescribePoliciesTypeDescribePoliciesPaginateTypeDef(TypedDict):
    AutoScalingGroupName: NotRequired[str],
    PolicyNames: NotRequired[Sequence[str]],
    PolicyTypes: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef

```python
# DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef definition

class DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef(TypedDict):
    ActivityIds: NotRequired[Sequence[str]],
    AutoScalingGroupName: NotRequired[str],
    IncludeDeletedGroups: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeTagsTypeDescribeTagsPaginateTypeDef

```python
# DescribeTagsTypeDescribeTagsPaginateTypeDef definition

class DescribeTagsTypeDescribeTagsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef

```python
# DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef definition

class DescribeWarmPoolTypeDescribeWarmPoolPaginateTypeDef(TypedDict):
    AutoScalingGroupName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef

```python
# LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef definition

class LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef(TypedDict):
    LaunchConfigurationNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## AutoScalingInstanceDetailsTypeDef

```python
# AutoScalingInstanceDetailsTypeDef definition

class AutoScalingInstanceDetailsTypeDef(TypedDict):
    InstanceId: str,
    AutoScalingGroupName: str,
    AvailabilityZone: str,
    LifecycleState: str,
    HealthStatus: str,
    ProtectedFromScaleIn: bool,
    InstanceType: NotRequired[str],
    LaunchConfigurationName: NotRequired[str],
    LaunchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (1)
    WeightedCapacity: NotRequired[str],
```

1. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    InstanceId: str,
    AvailabilityZone: str,
    LifecycleState: LifecycleStateType,  # (1)
    HealthStatus: str,
    ProtectedFromScaleIn: bool,
    InstanceType: NotRequired[str],
    LaunchConfigurationName: NotRequired[str],
    LaunchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (2)
    WeightedCapacity: NotRequired[str],
```

1. See [:material-code-brackets: LifecycleStateType](./literals.md#lifecyclestatetype) 
2. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
## TagsTypeTypeDef

```python
# TagsTypeTypeDef definition

class TagsTypeTypeDef(TypedDict):
    Tags: List[TagDescriptionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagDescriptionTypeDef](./type_defs.md#tagdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteScheduledActionAnswerTypeDef

```python
# BatchDeleteScheduledActionAnswerTypeDef definition

class BatchDeleteScheduledActionAnswerTypeDef(TypedDict):
    FailedScheduledActions: List[FailedScheduledUpdateGroupActionRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedScheduledUpdateGroupActionRequestTypeDef](./type_defs.md#failedscheduledupdategroupactionrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutScheduledUpdateGroupActionAnswerTypeDef

```python
# BatchPutScheduledUpdateGroupActionAnswerTypeDef definition

class BatchPutScheduledUpdateGroupActionAnswerTypeDef(TypedDict):
    FailedScheduledUpdateGroupActions: List[FailedScheduledUpdateGroupActionRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedScheduledUpdateGroupActionRequestTypeDef](./type_defs.md#failedscheduledupdategroupactionrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BlockDeviceMappingTypeDef

```python
# BlockDeviceMappingTypeDef definition

class BlockDeviceMappingTypeDef(TypedDict):
    DeviceName: str,
    VirtualName: NotRequired[str],
    Ebs: NotRequired[EbsTypeDef],  # (1)
    NoDevice: NotRequired[bool],
```

1. See [:material-code-braces: EbsTypeDef](./type_defs.md#ebstypedef) 
## CreateOrUpdateTagsTypeRequestTypeDef

```python
# CreateOrUpdateTagsTypeRequestTypeDef definition

class CreateOrUpdateTagsTypeRequestTypeDef(TypedDict):
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteTagsTypeRequestTypeDef

```python
# DeleteTagsTypeRequestTypeDef definition

class DeleteTagsTypeRequestTypeDef(TypedDict):
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## MetricTypeDef

```python
# MetricTypeDef definition

class MetricTypeDef(TypedDict):
    Namespace: str,
    MetricName: str,
    Dimensions: NotRequired[List[MetricDimensionTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
## DescribeLifecycleHooksAnswerTypeDef

```python
# DescribeLifecycleHooksAnswerTypeDef definition

class DescribeLifecycleHooksAnswerTypeDef(TypedDict):
    LifecycleHooks: List[LifecycleHookTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LifecycleHookTypeDef](./type_defs.md#lifecyclehooktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLoadBalancerTargetGroupsResponseTypeDef

```python
# DescribeLoadBalancerTargetGroupsResponseTypeDef definition

class DescribeLoadBalancerTargetGroupsResponseTypeDef(TypedDict):
    LoadBalancerTargetGroups: List[LoadBalancerTargetGroupStateTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerTargetGroupStateTypeDef](./type_defs.md#loadbalancertargetgroupstatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLoadBalancersResponseTypeDef

```python
# DescribeLoadBalancersResponseTypeDef definition

class DescribeLoadBalancersResponseTypeDef(TypedDict):
    LoadBalancers: List[LoadBalancerStateTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerStateTypeDef](./type_defs.md#loadbalancerstatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMetricCollectionTypesAnswerTypeDef

```python
# DescribeMetricCollectionTypesAnswerTypeDef definition

class DescribeMetricCollectionTypesAnswerTypeDef(TypedDict):
    Metrics: List[MetricCollectionTypeTypeDef],  # (1)
    Granularities: List[MetricGranularityTypeTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MetricCollectionTypeTypeDef](./type_defs.md#metriccollectiontypetypedef) 
2. See [:material-code-braces: MetricGranularityTypeTypeDef](./type_defs.md#metricgranularitytypetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNotificationConfigurationsAnswerTypeDef

```python
# DescribeNotificationConfigurationsAnswerTypeDef definition

class DescribeNotificationConfigurationsAnswerTypeDef(TypedDict):
    NotificationConfigurations: List[NotificationConfigurationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef

```python
# DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef definition

class DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef(TypedDict):
    AutoScalingGroupName: NotRequired[str],
    ScheduledActionNames: NotRequired[Sequence[str]],
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeScheduledActionsTypeRequestTypeDef

```python
# DescribeScheduledActionsTypeRequestTypeDef definition

class DescribeScheduledActionsTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: NotRequired[str],
    ScheduledActionNames: NotRequired[Sequence[str]],
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    NextToken: NotRequired[str],
    MaxRecords: NotRequired[int],
```

## GetPredictiveScalingForecastTypeRequestTypeDef

```python
# GetPredictiveScalingForecastTypeRequestTypeDef definition

class GetPredictiveScalingForecastTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    PolicyName: str,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
```

## PutScheduledUpdateGroupActionTypeRequestTypeDef

```python
# PutScheduledUpdateGroupActionTypeRequestTypeDef definition

class PutScheduledUpdateGroupActionTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    ScheduledActionName: str,
    Time: NotRequired[Union[datetime, str]],
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    Recurrence: NotRequired[str],
    MinSize: NotRequired[int],
    MaxSize: NotRequired[int],
    DesiredCapacity: NotRequired[int],
    TimeZone: NotRequired[str],
```

## ScheduledUpdateGroupActionRequestTypeDef

```python
# ScheduledUpdateGroupActionRequestTypeDef definition

class ScheduledUpdateGroupActionRequestTypeDef(TypedDict):
    ScheduledActionName: str,
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    Recurrence: NotRequired[str],
    MinSize: NotRequired[int],
    MaxSize: NotRequired[int],
    DesiredCapacity: NotRequired[int],
    TimeZone: NotRequired[str],
```

## DescribeTrafficSourcesResponseTypeDef

```python
# DescribeTrafficSourcesResponseTypeDef definition

class DescribeTrafficSourcesResponseTypeDef(TypedDict):
    TrafficSources: List[TrafficSourceStateTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficSourceStateTypeDef](./type_defs.md#trafficsourcestatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceRefreshProgressDetailsTypeDef

```python
# InstanceRefreshProgressDetailsTypeDef definition

class InstanceRefreshProgressDetailsTypeDef(TypedDict):
    LivePoolProgress: NotRequired[InstanceRefreshLivePoolProgressTypeDef],  # (1)
    WarmPoolProgress: NotRequired[InstanceRefreshWarmPoolProgressTypeDef],  # (2)
```

1. See [:material-code-braces: InstanceRefreshLivePoolProgressTypeDef](./type_defs.md#instancerefreshlivepoolprogresstypedef) 
2. See [:material-code-braces: InstanceRefreshWarmPoolProgressTypeDef](./type_defs.md#instancerefreshwarmpoolprogresstypedef) 
## InstanceRequirementsTypeDef

```python
# InstanceRequirementsTypeDef definition

class InstanceRequirementsTypeDef(TypedDict):
    VCpuCount: VCpuCountRequestTypeDef,  # (1)
    MemoryMiB: MemoryMiBRequestTypeDef,  # (2)
    CpuManufacturers: NotRequired[Sequence[CpuManufacturerType]],  # (3)
    MemoryGiBPerVCpu: NotRequired[MemoryGiBPerVCpuRequestTypeDef],  # (4)
    ExcludedInstanceTypes: NotRequired[Sequence[str]],
    InstanceGenerations: NotRequired[Sequence[InstanceGenerationType]],  # (5)
    SpotMaxPricePercentageOverLowestPrice: NotRequired[int],
    OnDemandMaxPricePercentageOverLowestPrice: NotRequired[int],
    BareMetal: NotRequired[BareMetalType],  # (6)
    BurstablePerformance: NotRequired[BurstablePerformanceType],  # (7)
    RequireHibernateSupport: NotRequired[bool],
    NetworkInterfaceCount: NotRequired[NetworkInterfaceCountRequestTypeDef],  # (8)
    LocalStorage: NotRequired[LocalStorageType],  # (9)
    LocalStorageTypes: NotRequired[Sequence[LocalStorageTypeType]],  # (10)
    TotalLocalStorageGB: NotRequired[TotalLocalStorageGBRequestTypeDef],  # (11)
    BaselineEbsBandwidthMbps: NotRequired[BaselineEbsBandwidthMbpsRequestTypeDef],  # (12)
    AcceleratorTypes: NotRequired[Sequence[AcceleratorTypeType]],  # (13)
    AcceleratorCount: NotRequired[AcceleratorCountRequestTypeDef],  # (14)
    AcceleratorManufacturers: NotRequired[Sequence[AcceleratorManufacturerType]],  # (15)
    AcceleratorNames: NotRequired[Sequence[AcceleratorNameType]],  # (16)
    AcceleratorTotalMemoryMiB: NotRequired[AcceleratorTotalMemoryMiBRequestTypeDef],  # (17)
    NetworkBandwidthGbps: NotRequired[NetworkBandwidthGbpsRequestTypeDef],  # (18)
    AllowedInstanceTypes: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: VCpuCountRequestTypeDef](./type_defs.md#vcpucountrequesttypedef) 
2. See [:material-code-braces: MemoryMiBRequestTypeDef](./type_defs.md#memorymibrequesttypedef) 
3. See [:material-code-brackets: CpuManufacturerType](./literals.md#cpumanufacturertype) 
4. See [:material-code-braces: MemoryGiBPerVCpuRequestTypeDef](./type_defs.md#memorygibpervcpurequesttypedef) 
5. See [:material-code-brackets: InstanceGenerationType](./literals.md#instancegenerationtype) 
6. See [:material-code-brackets: BareMetalType](./literals.md#baremetaltype) 
7. See [:material-code-brackets: BurstablePerformanceType](./literals.md#burstableperformancetype) 
8. See [:material-code-braces: NetworkInterfaceCountRequestTypeDef](./type_defs.md#networkinterfacecountrequesttypedef) 
9. See [:material-code-brackets: LocalStorageType](./literals.md#localstoragetype) 
10. See [:material-code-brackets: LocalStorageTypeType](./literals.md#localstoragetypetype) 
11. See [:material-code-braces: TotalLocalStorageGBRequestTypeDef](./type_defs.md#totallocalstoragegbrequesttypedef) 
12. See [:material-code-braces: BaselineEbsBandwidthMbpsRequestTypeDef](./type_defs.md#baselineebsbandwidthmbpsrequesttypedef) 
13. See [:material-code-brackets: AcceleratorTypeType](./literals.md#acceleratortypetype) 
14. See [:material-code-braces: AcceleratorCountRequestTypeDef](./type_defs.md#acceleratorcountrequesttypedef) 
15. See [:material-code-brackets: AcceleratorManufacturerType](./literals.md#acceleratormanufacturertype) 
16. See [:material-code-brackets: AcceleratorNameType](./literals.md#acceleratornametype) 
17. See [:material-code-braces: AcceleratorTotalMemoryMiBRequestTypeDef](./type_defs.md#acceleratortotalmemorymibrequesttypedef) 
18. See [:material-code-braces: NetworkBandwidthGbpsRequestTypeDef](./type_defs.md#networkbandwidthgbpsrequesttypedef) 
## PutWarmPoolTypeRequestTypeDef

```python
# PutWarmPoolTypeRequestTypeDef definition

class PutWarmPoolTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    MaxGroupPreparedCapacity: NotRequired[int],
    MinSize: NotRequired[int],
    PoolState: NotRequired[WarmPoolStateType],  # (1)
    InstanceReusePolicy: NotRequired[InstanceReusePolicyTypeDef],  # (2)
```

1. See [:material-code-brackets: WarmPoolStateType](./literals.md#warmpoolstatetype) 
2. See [:material-code-braces: InstanceReusePolicyTypeDef](./type_defs.md#instancereusepolicytypedef) 
## WarmPoolConfigurationTypeDef

```python
# WarmPoolConfigurationTypeDef definition

class WarmPoolConfigurationTypeDef(TypedDict):
    MaxGroupPreparedCapacity: NotRequired[int],
    MinSize: NotRequired[int],
    PoolState: NotRequired[WarmPoolStateType],  # (1)
    Status: NotRequired[WarmPoolStatusType],  # (2)
    InstanceReusePolicy: NotRequired[InstanceReusePolicyTypeDef],  # (3)
```

1. See [:material-code-brackets: WarmPoolStateType](./literals.md#warmpoolstatetype) 
2. See [:material-code-brackets: WarmPoolStatusType](./literals.md#warmpoolstatustype) 
3. See [:material-code-braces: InstanceReusePolicyTypeDef](./type_defs.md#instancereusepolicytypedef) 
## ProcessesTypeTypeDef

```python
# ProcessesTypeTypeDef definition

class ProcessesTypeTypeDef(TypedDict):
    Processes: List[ProcessTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProcessTypeTypeDef](./type_defs.md#processtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScheduledActionsTypeTypeDef

```python
# ScheduledActionsTypeTypeDef definition

class ScheduledActionsTypeTypeDef(TypedDict):
    ScheduledUpdateGroupActions: List[ScheduledUpdateGroupActionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduledUpdateGroupActionTypeDef](./type_defs.md#scheduledupdategroupactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoScalingInstancesTypeTypeDef

```python
# AutoScalingInstancesTypeTypeDef definition

class AutoScalingInstancesTypeTypeDef(TypedDict):
    AutoScalingInstances: List[AutoScalingInstanceDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoScalingInstanceDetailsTypeDef](./type_defs.md#autoscalinginstancedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLaunchConfigurationTypeRequestTypeDef

```python
# CreateLaunchConfigurationTypeRequestTypeDef definition

class CreateLaunchConfigurationTypeRequestTypeDef(TypedDict):
    LaunchConfigurationName: str,
    ImageId: NotRequired[str],
    KeyName: NotRequired[str],
    SecurityGroups: NotRequired[Sequence[str]],
    ClassicLinkVPCId: NotRequired[str],
    ClassicLinkVPCSecurityGroups: NotRequired[Sequence[str]],
    UserData: NotRequired[str],
    InstanceId: NotRequired[str],
    InstanceType: NotRequired[str],
    KernelId: NotRequired[str],
    RamdiskId: NotRequired[str],
    BlockDeviceMappings: NotRequired[Sequence[BlockDeviceMappingTypeDef]],  # (1)
    InstanceMonitoring: NotRequired[InstanceMonitoringTypeDef],  # (2)
    SpotPrice: NotRequired[str],
    IamInstanceProfile: NotRequired[str],
    EbsOptimized: NotRequired[bool],
    AssociatePublicIpAddress: NotRequired[bool],
    PlacementTenancy: NotRequired[str],
    MetadataOptions: NotRequired[InstanceMetadataOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: BlockDeviceMappingTypeDef](./type_defs.md#blockdevicemappingtypedef) 
2. See [:material-code-braces: InstanceMonitoringTypeDef](./type_defs.md#instancemonitoringtypedef) 
3. See [:material-code-braces: InstanceMetadataOptionsTypeDef](./type_defs.md#instancemetadataoptionstypedef) 
## LaunchConfigurationTypeDef

```python
# LaunchConfigurationTypeDef definition

class LaunchConfigurationTypeDef(TypedDict):
    LaunchConfigurationName: str,
    ImageId: str,
    InstanceType: str,
    CreatedTime: datetime,
    LaunchConfigurationARN: NotRequired[str],
    KeyName: NotRequired[str],
    SecurityGroups: NotRequired[List[str]],
    ClassicLinkVPCId: NotRequired[str],
    ClassicLinkVPCSecurityGroups: NotRequired[List[str]],
    UserData: NotRequired[str],
    KernelId: NotRequired[str],
    RamdiskId: NotRequired[str],
    BlockDeviceMappings: NotRequired[List[BlockDeviceMappingTypeDef]],  # (1)
    InstanceMonitoring: NotRequired[InstanceMonitoringTypeDef],  # (2)
    SpotPrice: NotRequired[str],
    IamInstanceProfile: NotRequired[str],
    EbsOptimized: NotRequired[bool],
    AssociatePublicIpAddress: NotRequired[bool],
    PlacementTenancy: NotRequired[str],
    MetadataOptions: NotRequired[InstanceMetadataOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: BlockDeviceMappingTypeDef](./type_defs.md#blockdevicemappingtypedef) 
2. See [:material-code-braces: InstanceMonitoringTypeDef](./type_defs.md#instancemonitoringtypedef) 
3. See [:material-code-braces: InstanceMetadataOptionsTypeDef](./type_defs.md#instancemetadataoptionstypedef) 
## MetricStatTypeDef

```python
# MetricStatTypeDef definition

class MetricStatTypeDef(TypedDict):
    Metric: MetricTypeDef,  # (1)
    Stat: str,
    Unit: NotRequired[str],
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
## TargetTrackingMetricStatTypeDef

```python
# TargetTrackingMetricStatTypeDef definition

class TargetTrackingMetricStatTypeDef(TypedDict):
    Metric: MetricTypeDef,  # (1)
    Stat: str,
    Unit: NotRequired[str],
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
## BatchPutScheduledUpdateGroupActionTypeRequestTypeDef

```python
# BatchPutScheduledUpdateGroupActionTypeRequestTypeDef definition

class BatchPutScheduledUpdateGroupActionTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    ScheduledUpdateGroupActions: Sequence[ScheduledUpdateGroupActionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: ScheduledUpdateGroupActionRequestTypeDef](./type_defs.md#scheduledupdategroupactionrequesttypedef) 
## RollbackDetailsTypeDef

```python
# RollbackDetailsTypeDef definition

class RollbackDetailsTypeDef(TypedDict):
    RollbackReason: NotRequired[str],
    RollbackStartTime: NotRequired[datetime],
    PercentageCompleteOnRollback: NotRequired[int],
    InstancesToUpdateOnRollback: NotRequired[int],
    ProgressDetailsOnRollback: NotRequired[InstanceRefreshProgressDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceRefreshProgressDetailsTypeDef](./type_defs.md#instancerefreshprogressdetailstypedef) 
## LaunchTemplateOverridesTypeDef

```python
# LaunchTemplateOverridesTypeDef definition

class LaunchTemplateOverridesTypeDef(TypedDict):
    InstanceType: NotRequired[str],
    WeightedCapacity: NotRequired[str],
    LaunchTemplateSpecification: NotRequired[LaunchTemplateSpecificationTypeDef],  # (1)
    InstanceRequirements: NotRequired[InstanceRequirementsTypeDef],  # (2)
```

1. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
2. See [:material-code-braces: InstanceRequirementsTypeDef](./type_defs.md#instancerequirementstypedef) 
## DescribeWarmPoolAnswerTypeDef

```python
# DescribeWarmPoolAnswerTypeDef definition

class DescribeWarmPoolAnswerTypeDef(TypedDict):
    WarmPoolConfiguration: WarmPoolConfigurationTypeDef,  # (1)
    Instances: List[InstanceTypeDef],  # (2)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: WarmPoolConfigurationTypeDef](./type_defs.md#warmpoolconfigurationtypedef) 
2. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LaunchConfigurationsTypeTypeDef

```python
# LaunchConfigurationsTypeTypeDef definition

class LaunchConfigurationsTypeTypeDef(TypedDict):
    LaunchConfigurations: List[LaunchConfigurationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricDataQueryTypeDef

```python
# MetricDataQueryTypeDef definition

class MetricDataQueryTypeDef(TypedDict):
    Id: str,
    Expression: NotRequired[str],
    MetricStat: NotRequired[MetricStatTypeDef],  # (1)
    Label: NotRequired[str],
    ReturnData: NotRequired[bool],
```

1. See [:material-code-braces: MetricStatTypeDef](./type_defs.md#metricstattypedef) 
## TargetTrackingMetricDataQueryTypeDef

```python
# TargetTrackingMetricDataQueryTypeDef definition

class TargetTrackingMetricDataQueryTypeDef(TypedDict):
    Id: str,
    Expression: NotRequired[str],
    MetricStat: NotRequired[TargetTrackingMetricStatTypeDef],  # (1)
    Label: NotRequired[str],
    ReturnData: NotRequired[bool],
```

1. See [:material-code-braces: TargetTrackingMetricStatTypeDef](./type_defs.md#targettrackingmetricstattypedef) 
## LaunchTemplateTypeDef

```python
# LaunchTemplateTypeDef definition

class LaunchTemplateTypeDef(TypedDict):
    LaunchTemplateSpecification: NotRequired[LaunchTemplateSpecificationTypeDef],  # (1)
    Overrides: NotRequired[Sequence[LaunchTemplateOverridesTypeDef]],  # (2)
```

1. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
2. See [:material-code-braces: LaunchTemplateOverridesTypeDef](./type_defs.md#launchtemplateoverridestypedef) 
## PredictiveScalingCustomizedCapacityMetricTypeDef

```python
# PredictiveScalingCustomizedCapacityMetricTypeDef definition

class PredictiveScalingCustomizedCapacityMetricTypeDef(TypedDict):
    MetricDataQueries: List[MetricDataQueryTypeDef],  # (1)
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
## PredictiveScalingCustomizedLoadMetricTypeDef

```python
# PredictiveScalingCustomizedLoadMetricTypeDef definition

class PredictiveScalingCustomizedLoadMetricTypeDef(TypedDict):
    MetricDataQueries: List[MetricDataQueryTypeDef],  # (1)
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
## PredictiveScalingCustomizedScalingMetricTypeDef

```python
# PredictiveScalingCustomizedScalingMetricTypeDef definition

class PredictiveScalingCustomizedScalingMetricTypeDef(TypedDict):
    MetricDataQueries: List[MetricDataQueryTypeDef],  # (1)
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
## CustomizedMetricSpecificationTypeDef

```python
# CustomizedMetricSpecificationTypeDef definition

class CustomizedMetricSpecificationTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Namespace: NotRequired[str],
    Dimensions: NotRequired[List[MetricDimensionTypeDef]],  # (1)
    Statistic: NotRequired[MetricStatisticType],  # (2)
    Unit: NotRequired[str],
    Metrics: NotRequired[List[TargetTrackingMetricDataQueryTypeDef]],  # (3)
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
3. See [:material-code-braces: TargetTrackingMetricDataQueryTypeDef](./type_defs.md#targettrackingmetricdataquerytypedef) 
## MixedInstancesPolicyTypeDef

```python
# MixedInstancesPolicyTypeDef definition

class MixedInstancesPolicyTypeDef(TypedDict):
    LaunchTemplate: NotRequired[LaunchTemplateTypeDef],  # (1)
    InstancesDistribution: NotRequired[InstancesDistributionTypeDef],  # (2)
```

1. See [:material-code-braces: LaunchTemplateTypeDef](./type_defs.md#launchtemplatetypedef) 
2. See [:material-code-braces: InstancesDistributionTypeDef](./type_defs.md#instancesdistributiontypedef) 
## PredictiveScalingMetricSpecificationTypeDef

```python
# PredictiveScalingMetricSpecificationTypeDef definition

class PredictiveScalingMetricSpecificationTypeDef(TypedDict):
    TargetValue: float,
    PredefinedMetricPairSpecification: NotRequired[PredictiveScalingPredefinedMetricPairTypeDef],  # (1)
    PredefinedScalingMetricSpecification: NotRequired[PredictiveScalingPredefinedScalingMetricTypeDef],  # (2)
    PredefinedLoadMetricSpecification: NotRequired[PredictiveScalingPredefinedLoadMetricTypeDef],  # (3)
    CustomizedScalingMetricSpecification: NotRequired[PredictiveScalingCustomizedScalingMetricTypeDef],  # (4)
    CustomizedLoadMetricSpecification: NotRequired[PredictiveScalingCustomizedLoadMetricTypeDef],  # (5)
    CustomizedCapacityMetricSpecification: NotRequired[PredictiveScalingCustomizedCapacityMetricTypeDef],  # (6)
```

1. See [:material-code-braces: PredictiveScalingPredefinedMetricPairTypeDef](./type_defs.md#predictivescalingpredefinedmetricpairtypedef) 
2. See [:material-code-braces: PredictiveScalingPredefinedScalingMetricTypeDef](./type_defs.md#predictivescalingpredefinedscalingmetrictypedef) 
3. See [:material-code-braces: PredictiveScalingPredefinedLoadMetricTypeDef](./type_defs.md#predictivescalingpredefinedloadmetrictypedef) 
4. See [:material-code-braces: PredictiveScalingCustomizedScalingMetricTypeDef](./type_defs.md#predictivescalingcustomizedscalingmetrictypedef) 
5. See [:material-code-braces: PredictiveScalingCustomizedLoadMetricTypeDef](./type_defs.md#predictivescalingcustomizedloadmetrictypedef) 
6. See [:material-code-braces: PredictiveScalingCustomizedCapacityMetricTypeDef](./type_defs.md#predictivescalingcustomizedcapacitymetrictypedef) 
## TargetTrackingConfigurationTypeDef

```python
# TargetTrackingConfigurationTypeDef definition

class TargetTrackingConfigurationTypeDef(TypedDict):
    TargetValue: float,
    PredefinedMetricSpecification: NotRequired[PredefinedMetricSpecificationTypeDef],  # (1)
    CustomizedMetricSpecification: NotRequired[CustomizedMetricSpecificationTypeDef],  # (2)
    DisableScaleIn: NotRequired[bool],
```

1. See [:material-code-braces: PredefinedMetricSpecificationTypeDef](./type_defs.md#predefinedmetricspecificationtypedef) 
2. See [:material-code-braces: CustomizedMetricSpecificationTypeDef](./type_defs.md#customizedmetricspecificationtypedef) 
## AutoScalingGroupTypeDef

```python
# AutoScalingGroupTypeDef definition

class AutoScalingGroupTypeDef(TypedDict):
    AutoScalingGroupName: str,
    MinSize: int,
    MaxSize: int,
    DesiredCapacity: int,
    DefaultCooldown: int,
    AvailabilityZones: List[str],
    HealthCheckType: str,
    CreatedTime: datetime,
    AutoScalingGroupARN: NotRequired[str],
    LaunchConfigurationName: NotRequired[str],
    LaunchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (1)
    MixedInstancesPolicy: NotRequired[MixedInstancesPolicyTypeDef],  # (2)
    PredictedCapacity: NotRequired[int],
    LoadBalancerNames: NotRequired[List[str]],
    TargetGroupARNs: NotRequired[List[str]],
    HealthCheckGracePeriod: NotRequired[int],
    Instances: NotRequired[List[InstanceTypeDef]],  # (3)
    SuspendedProcesses: NotRequired[List[SuspendedProcessTypeDef]],  # (4)
    PlacementGroup: NotRequired[str],
    VPCZoneIdentifier: NotRequired[str],
    EnabledMetrics: NotRequired[List[EnabledMetricTypeDef]],  # (5)
    Status: NotRequired[str],
    Tags: NotRequired[List[TagDescriptionTypeDef]],  # (6)
    TerminationPolicies: NotRequired[List[str]],
    NewInstancesProtectedFromScaleIn: NotRequired[bool],
    ServiceLinkedRoleARN: NotRequired[str],
    MaxInstanceLifetime: NotRequired[int],
    CapacityRebalance: NotRequired[bool],
    WarmPoolConfiguration: NotRequired[WarmPoolConfigurationTypeDef],  # (7)
    WarmPoolSize: NotRequired[int],
    Context: NotRequired[str],
    DesiredCapacityType: NotRequired[str],
    DefaultInstanceWarmup: NotRequired[int],
    TrafficSources: NotRequired[List[TrafficSourceIdentifierTypeDef]],  # (8)
```

1. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
2. See [:material-code-braces: MixedInstancesPolicyTypeDef](./type_defs.md#mixedinstancespolicytypedef) 
3. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
4. See [:material-code-braces: SuspendedProcessTypeDef](./type_defs.md#suspendedprocesstypedef) 
5. See [:material-code-braces: EnabledMetricTypeDef](./type_defs.md#enabledmetrictypedef) 
6. See [:material-code-braces: TagDescriptionTypeDef](./type_defs.md#tagdescriptiontypedef) 
7. See [:material-code-braces: WarmPoolConfigurationTypeDef](./type_defs.md#warmpoolconfigurationtypedef) 
8. See [:material-code-braces: TrafficSourceIdentifierTypeDef](./type_defs.md#trafficsourceidentifiertypedef) 
## CreateAutoScalingGroupTypeRequestTypeDef

```python
# CreateAutoScalingGroupTypeRequestTypeDef definition

class CreateAutoScalingGroupTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    MinSize: int,
    MaxSize: int,
    LaunchConfigurationName: NotRequired[str],
    LaunchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (1)
    MixedInstancesPolicy: NotRequired[MixedInstancesPolicyTypeDef],  # (2)
    InstanceId: NotRequired[str],
    DesiredCapacity: NotRequired[int],
    DefaultCooldown: NotRequired[int],
    AvailabilityZones: NotRequired[Sequence[str]],
    LoadBalancerNames: NotRequired[Sequence[str]],
    TargetGroupARNs: NotRequired[Sequence[str]],
    HealthCheckType: NotRequired[str],
    HealthCheckGracePeriod: NotRequired[int],
    PlacementGroup: NotRequired[str],
    VPCZoneIdentifier: NotRequired[str],
    TerminationPolicies: NotRequired[Sequence[str]],
    NewInstancesProtectedFromScaleIn: NotRequired[bool],
    CapacityRebalance: NotRequired[bool],
    LifecycleHookSpecificationList: NotRequired[Sequence[LifecycleHookSpecificationTypeDef]],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    ServiceLinkedRoleARN: NotRequired[str],
    MaxInstanceLifetime: NotRequired[int],
    Context: NotRequired[str],
    DesiredCapacityType: NotRequired[str],
    DefaultInstanceWarmup: NotRequired[int],
    TrafficSources: NotRequired[Sequence[TrafficSourceIdentifierTypeDef]],  # (5)
```

1. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
2. See [:material-code-braces: MixedInstancesPolicyTypeDef](./type_defs.md#mixedinstancespolicytypedef) 
3. See [:material-code-braces: LifecycleHookSpecificationTypeDef](./type_defs.md#lifecyclehookspecificationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: TrafficSourceIdentifierTypeDef](./type_defs.md#trafficsourceidentifiertypedef) 
## DesiredConfigurationTypeDef

```python
# DesiredConfigurationTypeDef definition

class DesiredConfigurationTypeDef(TypedDict):
    LaunchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (1)
    MixedInstancesPolicy: NotRequired[MixedInstancesPolicyTypeDef],  # (2)
```

1. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
2. See [:material-code-braces: MixedInstancesPolicyTypeDef](./type_defs.md#mixedinstancespolicytypedef) 
## UpdateAutoScalingGroupTypeRequestTypeDef

```python
# UpdateAutoScalingGroupTypeRequestTypeDef definition

class UpdateAutoScalingGroupTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    LaunchConfigurationName: NotRequired[str],
    LaunchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (1)
    MixedInstancesPolicy: NotRequired[MixedInstancesPolicyTypeDef],  # (2)
    MinSize: NotRequired[int],
    MaxSize: NotRequired[int],
    DesiredCapacity: NotRequired[int],
    DefaultCooldown: NotRequired[int],
    AvailabilityZones: NotRequired[Sequence[str]],
    HealthCheckType: NotRequired[str],
    HealthCheckGracePeriod: NotRequired[int],
    PlacementGroup: NotRequired[str],
    VPCZoneIdentifier: NotRequired[str],
    TerminationPolicies: NotRequired[Sequence[str]],
    NewInstancesProtectedFromScaleIn: NotRequired[bool],
    ServiceLinkedRoleARN: NotRequired[str],
    MaxInstanceLifetime: NotRequired[int],
    CapacityRebalance: NotRequired[bool],
    Context: NotRequired[str],
    DesiredCapacityType: NotRequired[str],
    DefaultInstanceWarmup: NotRequired[int],
```

1. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
2. See [:material-code-braces: MixedInstancesPolicyTypeDef](./type_defs.md#mixedinstancespolicytypedef) 
## LoadForecastTypeDef

```python
# LoadForecastTypeDef definition

class LoadForecastTypeDef(TypedDict):
    Timestamps: List[datetime],
    Values: List[float],
    MetricSpecification: PredictiveScalingMetricSpecificationTypeDef,  # (1)
```

1. See [:material-code-braces: PredictiveScalingMetricSpecificationTypeDef](./type_defs.md#predictivescalingmetricspecificationtypedef) 
## PredictiveScalingConfigurationTypeDef

```python
# PredictiveScalingConfigurationTypeDef definition

class PredictiveScalingConfigurationTypeDef(TypedDict):
    MetricSpecifications: List[PredictiveScalingMetricSpecificationTypeDef],  # (1)
    Mode: NotRequired[PredictiveScalingModeType],  # (2)
    SchedulingBufferTime: NotRequired[int],
    MaxCapacityBreachBehavior: NotRequired[PredictiveScalingMaxCapacityBreachBehaviorType],  # (3)
    MaxCapacityBuffer: NotRequired[int],
```

1. See [:material-code-braces: PredictiveScalingMetricSpecificationTypeDef](./type_defs.md#predictivescalingmetricspecificationtypedef) 
2. See [:material-code-brackets: PredictiveScalingModeType](./literals.md#predictivescalingmodetype) 
3. See [:material-code-brackets: PredictiveScalingMaxCapacityBreachBehaviorType](./literals.md#predictivescalingmaxcapacitybreachbehaviortype) 
## AutoScalingGroupsTypeTypeDef

```python
# AutoScalingGroupsTypeTypeDef definition

class AutoScalingGroupsTypeTypeDef(TypedDict):
    AutoScalingGroups: List[AutoScalingGroupTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoScalingGroupTypeDef](./type_defs.md#autoscalinggrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceRefreshTypeDef

```python
# InstanceRefreshTypeDef definition

class InstanceRefreshTypeDef(TypedDict):
    InstanceRefreshId: NotRequired[str],
    AutoScalingGroupName: NotRequired[str],
    Status: NotRequired[InstanceRefreshStatusType],  # (1)
    StatusReason: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    PercentageComplete: NotRequired[int],
    InstancesToUpdate: NotRequired[int],
    ProgressDetails: NotRequired[InstanceRefreshProgressDetailsTypeDef],  # (2)
    Preferences: NotRequired[RefreshPreferencesTypeDef],  # (3)
    DesiredConfiguration: NotRequired[DesiredConfigurationTypeDef],  # (4)
    RollbackDetails: NotRequired[RollbackDetailsTypeDef],  # (5)
```

1. See [:material-code-brackets: InstanceRefreshStatusType](./literals.md#instancerefreshstatustype) 
2. See [:material-code-braces: InstanceRefreshProgressDetailsTypeDef](./type_defs.md#instancerefreshprogressdetailstypedef) 
3. See [:material-code-braces: RefreshPreferencesTypeDef](./type_defs.md#refreshpreferencestypedef) 
4. See [:material-code-braces: DesiredConfigurationTypeDef](./type_defs.md#desiredconfigurationtypedef) 
5. See [:material-code-braces: RollbackDetailsTypeDef](./type_defs.md#rollbackdetailstypedef) 
## StartInstanceRefreshTypeRequestTypeDef

```python
# StartInstanceRefreshTypeRequestTypeDef definition

class StartInstanceRefreshTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    Strategy: NotRequired[RefreshStrategyType],  # (1)
    DesiredConfiguration: NotRequired[DesiredConfigurationTypeDef],  # (2)
    Preferences: NotRequired[RefreshPreferencesTypeDef],  # (3)
```

1. See [:material-code-brackets: RefreshStrategyType](./literals.md#refreshstrategytype) 
2. See [:material-code-braces: DesiredConfigurationTypeDef](./type_defs.md#desiredconfigurationtypedef) 
3. See [:material-code-braces: RefreshPreferencesTypeDef](./type_defs.md#refreshpreferencestypedef) 
## GetPredictiveScalingForecastAnswerTypeDef

```python
# GetPredictiveScalingForecastAnswerTypeDef definition

class GetPredictiveScalingForecastAnswerTypeDef(TypedDict):
    LoadForecast: List[LoadForecastTypeDef],  # (1)
    CapacityForecast: CapacityForecastTypeDef,  # (2)
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: LoadForecastTypeDef](./type_defs.md#loadforecasttypedef) 
2. See [:material-code-braces: CapacityForecastTypeDef](./type_defs.md#capacityforecasttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutScalingPolicyTypeRequestTypeDef

```python
# PutScalingPolicyTypeRequestTypeDef definition

class PutScalingPolicyTypeRequestTypeDef(TypedDict):
    AutoScalingGroupName: str,
    PolicyName: str,
    PolicyType: NotRequired[str],
    AdjustmentType: NotRequired[str],
    MinAdjustmentStep: NotRequired[int],
    MinAdjustmentMagnitude: NotRequired[int],
    ScalingAdjustment: NotRequired[int],
    Cooldown: NotRequired[int],
    MetricAggregationType: NotRequired[str],
    StepAdjustments: NotRequired[Sequence[StepAdjustmentTypeDef]],  # (1)
    EstimatedInstanceWarmup: NotRequired[int],
    TargetTrackingConfiguration: NotRequired[TargetTrackingConfigurationTypeDef],  # (2)
    Enabled: NotRequired[bool],
    PredictiveScalingConfiguration: NotRequired[PredictiveScalingConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: StepAdjustmentTypeDef](./type_defs.md#stepadjustmenttypedef) 
2. See [:material-code-braces: TargetTrackingConfigurationTypeDef](./type_defs.md#targettrackingconfigurationtypedef) 
3. See [:material-code-braces: PredictiveScalingConfigurationTypeDef](./type_defs.md#predictivescalingconfigurationtypedef) 
## ScalingPolicyTypeDef

```python
# ScalingPolicyTypeDef definition

class ScalingPolicyTypeDef(TypedDict):
    AutoScalingGroupName: NotRequired[str],
    PolicyName: NotRequired[str],
    PolicyARN: NotRequired[str],
    PolicyType: NotRequired[str],
    AdjustmentType: NotRequired[str],
    MinAdjustmentStep: NotRequired[int],
    MinAdjustmentMagnitude: NotRequired[int],
    ScalingAdjustment: NotRequired[int],
    Cooldown: NotRequired[int],
    StepAdjustments: NotRequired[List[StepAdjustmentTypeDef]],  # (1)
    MetricAggregationType: NotRequired[str],
    EstimatedInstanceWarmup: NotRequired[int],
    Alarms: NotRequired[List[AlarmTypeDef]],  # (2)
    TargetTrackingConfiguration: NotRequired[TargetTrackingConfigurationTypeDef],  # (3)
    Enabled: NotRequired[bool],
    PredictiveScalingConfiguration: NotRequired[PredictiveScalingConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: StepAdjustmentTypeDef](./type_defs.md#stepadjustmenttypedef) 
2. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
3. See [:material-code-braces: TargetTrackingConfigurationTypeDef](./type_defs.md#targettrackingconfigurationtypedef) 
4. See [:material-code-braces: PredictiveScalingConfigurationTypeDef](./type_defs.md#predictivescalingconfigurationtypedef) 
## DescribeInstanceRefreshesAnswerTypeDef

```python
# DescribeInstanceRefreshesAnswerTypeDef definition

class DescribeInstanceRefreshesAnswerTypeDef(TypedDict):
    InstanceRefreshes: List[InstanceRefreshTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceRefreshTypeDef](./type_defs.md#instancerefreshtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PoliciesTypeTypeDef

```python
# PoliciesTypeTypeDef definition

class PoliciesTypeTypeDef(TypedDict):
    ScalingPolicies: List[ScalingPolicyTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScalingPolicyTypeDef](./type_defs.md#scalingpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
