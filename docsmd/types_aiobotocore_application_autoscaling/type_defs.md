# Type definitions

> [Index](../README.md) > [ApplicationAutoScaling](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ApplicationAutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
    type annotations stubs module [types-aiobotocore-application-autoscaling](https://pypi.org/project/types-aiobotocore-application-autoscaling/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## TargetTrackingMetricUnionTypeDef

```python
# TargetTrackingMetricUnionTypeDef definition

TargetTrackingMetricUnionTypeDef = Union[
    TargetTrackingMetricTypeDef,  # (1)
    TargetTrackingMetricOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TargetTrackingMetricTypeDef](./type_defs.md#targettrackingmetrictypedef) 
2. See [:material-code-braces: TargetTrackingMetricOutputTypeDef](./type_defs.md#targettrackingmetricoutputtypedef) 

## TargetTrackingMetricStatUnionTypeDef

```python
# TargetTrackingMetricStatUnionTypeDef definition

TargetTrackingMetricStatUnionTypeDef = Union[
    TargetTrackingMetricStatTypeDef,  # (1)
    TargetTrackingMetricStatOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TargetTrackingMetricStatTypeDef](./type_defs.md#targettrackingmetricstattypedef) 
2. See [:material-code-braces: TargetTrackingMetricStatOutputTypeDef](./type_defs.md#targettrackingmetricstatoutputtypedef) 

## TargetTrackingMetricDataQueryUnionTypeDef

```python
# TargetTrackingMetricDataQueryUnionTypeDef definition

TargetTrackingMetricDataQueryUnionTypeDef = Union[
    TargetTrackingMetricDataQueryTypeDef,  # (1)
    TargetTrackingMetricDataQueryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TargetTrackingMetricDataQueryTypeDef](./type_defs.md#targettrackingmetricdataquerytypedef) 
2. See [:material-code-braces: TargetTrackingMetricDataQueryOutputTypeDef](./type_defs.md#targettrackingmetricdataqueryoutputtypedef) 

## CustomizedMetricSpecificationUnionTypeDef

```python
# CustomizedMetricSpecificationUnionTypeDef definition

CustomizedMetricSpecificationUnionTypeDef = Union[
    CustomizedMetricSpecificationTypeDef,  # (1)
    CustomizedMetricSpecificationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomizedMetricSpecificationTypeDef](./type_defs.md#customizedmetricspecificationtypedef) 
2. See [:material-code-braces: CustomizedMetricSpecificationOutputTypeDef](./type_defs.md#customizedmetricspecificationoutputtypedef) 



## AlarmTypeDef

```python
# AlarmTypeDef definition

class AlarmTypeDef(TypedDict):
    AlarmName: str,
    AlarmARN: str,
```

## MetricDimensionTypeDef

```python
# MetricDimensionTypeDef definition

class MetricDimensionTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## DeleteScalingPolicyRequestRequestTypeDef

```python
# DeleteScalingPolicyRequestRequestTypeDef definition

class DeleteScalingPolicyRequestRequestTypeDef(TypedDict):
    PolicyName: str,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
## DeleteScheduledActionRequestRequestTypeDef

```python
# DeleteScheduledActionRequestRequestTypeDef definition

class DeleteScheduledActionRequestRequestTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ScheduledActionName: str,
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
## DeregisterScalableTargetRequestRequestTypeDef

```python
# DeregisterScalableTargetRequestRequestTypeDef definition

class DeregisterScalableTargetRequestRequestTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeScalableTargetsRequestRequestTypeDef

```python
# DescribeScalableTargetsRequestRequestTypeDef definition

class DescribeScalableTargetsRequestRequestTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceIds: NotRequired[Sequence[str]],
    ScalableDimension: NotRequired[ScalableDimensionType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
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

## DescribeScalingActivitiesRequestRequestTypeDef

```python
# DescribeScalingActivitiesRequestRequestTypeDef definition

class DescribeScalingActivitiesRequestRequestTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: NotRequired[str],
    ScalableDimension: NotRequired[ScalableDimensionType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    IncludeNotScaledActivities: NotRequired[bool],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
## DescribeScalingPoliciesRequestRequestTypeDef

```python
# DescribeScalingPoliciesRequestRequestTypeDef definition

class DescribeScalingPoliciesRequestRequestTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    PolicyNames: NotRequired[Sequence[str]],
    ResourceId: NotRequired[str],
    ScalableDimension: NotRequired[ScalableDimensionType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
## DescribeScheduledActionsRequestRequestTypeDef

```python
# DescribeScheduledActionsRequestRequestTypeDef definition

class DescribeScheduledActionsRequestRequestTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ScheduledActionNames: NotRequired[Sequence[str]],
    ResourceId: NotRequired[str],
    ScalableDimension: NotRequired[ScalableDimensionType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## NotScaledReasonTypeDef

```python
# NotScaledReasonTypeDef definition

class NotScaledReasonTypeDef(TypedDict):
    Code: str,
    MaxCapacity: NotRequired[int],
    MinCapacity: NotRequired[int],
    CurrentCapacity: NotRequired[int],
```

## PredefinedMetricSpecificationTypeDef

```python
# PredefinedMetricSpecificationTypeDef definition

class PredefinedMetricSpecificationTypeDef(TypedDict):
    PredefinedMetricType: MetricTypeType,  # (1)
    ResourceLabel: NotRequired[str],
```

1. See [:material-code-brackets: MetricTypeType](./literals.md#metrictypetype) 
## ScalableTargetActionTypeDef

```python
# ScalableTargetActionTypeDef definition

class ScalableTargetActionTypeDef(TypedDict):
    MinCapacity: NotRequired[int],
    MaxCapacity: NotRequired[int],
```

## SuspendedStateTypeDef

```python
# SuspendedStateTypeDef definition

class SuspendedStateTypeDef(TypedDict):
    DynamicScalingInSuspended: NotRequired[bool],
    DynamicScalingOutSuspended: NotRequired[bool],
    ScheduledScalingSuspended: NotRequired[bool],
```

## StepAdjustmentTypeDef

```python
# StepAdjustmentTypeDef definition

class StepAdjustmentTypeDef(TypedDict):
    ScalingAdjustment: int,
    MetricIntervalLowerBound: NotRequired[float],
    MetricIntervalUpperBound: NotRequired[float],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Mapping[str, str],
```

## TargetTrackingMetricDimensionTypeDef

```python
# TargetTrackingMetricDimensionTypeDef definition

class TargetTrackingMetricDimensionTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef

```python
# DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef definition

class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceIds: NotRequired[Sequence[str]],
    ScalableDimension: NotRequired[ScalableDimensionType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef

```python
# DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef definition

class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: NotRequired[str],
    ScalableDimension: NotRequired[ScalableDimensionType],  # (2)
    IncludeNotScaledActivities: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef

```python
# DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef definition

class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    PolicyNames: NotRequired[Sequence[str]],
    ResourceId: NotRequired[str],
    ScalableDimension: NotRequired[ScalableDimensionType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef

```python
# DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef definition

class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ScheduledActionNames: NotRequired[Sequence[str]],
    ResourceId: NotRequired[str],
    ScalableDimension: NotRequired[ScalableDimensionType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutScalingPolicyResponseTypeDef

```python
# PutScalingPolicyResponseTypeDef definition

class PutScalingPolicyResponseTypeDef(TypedDict):
    PolicyARN: str,
    Alarms: List[AlarmTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterScalableTargetResponseTypeDef

```python
# RegisterScalableTargetResponseTypeDef definition

class RegisterScalableTargetResponseTypeDef(TypedDict):
    ScalableTargetARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScalingActivityTypeDef

```python
# ScalingActivityTypeDef definition

class ScalingActivityTypeDef(TypedDict):
    ActivityId: str,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    Description: str,
    Cause: str,
    StartTime: datetime,
    StatusCode: ScalingActivityStatusCodeType,  # (3)
    EndTime: NotRequired[datetime],
    StatusMessage: NotRequired[str],
    Details: NotRequired[str],
    NotScaledReasons: NotRequired[List[NotScaledReasonTypeDef]],  # (4)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-brackets: ScalingActivityStatusCodeType](./literals.md#scalingactivitystatuscodetype) 
4. See [:material-code-braces: NotScaledReasonTypeDef](./type_defs.md#notscaledreasontypedef) 
## ScheduledActionTypeDef

```python
# ScheduledActionTypeDef definition

class ScheduledActionTypeDef(TypedDict):
    ScheduledActionName: str,
    ScheduledActionARN: str,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    Schedule: str,
    ResourceId: str,
    CreationTime: datetime,
    Timezone: NotRequired[str],
    ScalableDimension: NotRequired[ScalableDimensionType],  # (2)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    ScalableTargetAction: NotRequired[ScalableTargetActionTypeDef],  # (3)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: ScalableTargetActionTypeDef](./type_defs.md#scalabletargetactiontypedef) 
## PutScheduledActionRequestRequestTypeDef

```python
# PutScheduledActionRequestRequestTypeDef definition

class PutScheduledActionRequestRequestTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ScheduledActionName: str,
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    Schedule: NotRequired[str],
    Timezone: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    ScalableTargetAction: NotRequired[ScalableTargetActionTypeDef],  # (3)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: ScalableTargetActionTypeDef](./type_defs.md#scalabletargetactiontypedef) 
## RegisterScalableTargetRequestRequestTypeDef

```python
# RegisterScalableTargetRequestRequestTypeDef definition

class RegisterScalableTargetRequestRequestTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    MinCapacity: NotRequired[int],
    MaxCapacity: NotRequired[int],
    RoleARN: NotRequired[str],
    SuspendedState: NotRequired[SuspendedStateTypeDef],  # (3)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: SuspendedStateTypeDef](./type_defs.md#suspendedstatetypedef) 
## ScalableTargetTypeDef

```python
# ScalableTargetTypeDef definition

class ScalableTargetTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    MinCapacity: int,
    MaxCapacity: int,
    RoleARN: str,
    CreationTime: datetime,
    SuspendedState: NotRequired[SuspendedStateTypeDef],  # (3)
    ScalableTargetARN: NotRequired[str],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: SuspendedStateTypeDef](./type_defs.md#suspendedstatetypedef) 
## StepScalingPolicyConfigurationOutputTypeDef

```python
# StepScalingPolicyConfigurationOutputTypeDef definition

class StepScalingPolicyConfigurationOutputTypeDef(TypedDict):
    AdjustmentType: NotRequired[AdjustmentTypeType],  # (1)
    StepAdjustments: NotRequired[List[StepAdjustmentTypeDef]],  # (2)
    MinAdjustmentMagnitude: NotRequired[int],
    Cooldown: NotRequired[int],
    MetricAggregationType: NotRequired[MetricAggregationTypeType],  # (3)
```

1. See [:material-code-brackets: AdjustmentTypeType](./literals.md#adjustmenttypetype) 
2. See [:material-code-braces: StepAdjustmentTypeDef](./type_defs.md#stepadjustmenttypedef) 
3. See [:material-code-brackets: MetricAggregationTypeType](./literals.md#metricaggregationtypetype) 
## StepScalingPolicyConfigurationTypeDef

```python
# StepScalingPolicyConfigurationTypeDef definition

class StepScalingPolicyConfigurationTypeDef(TypedDict):
    AdjustmentType: NotRequired[AdjustmentTypeType],  # (1)
    StepAdjustments: NotRequired[Sequence[StepAdjustmentTypeDef]],  # (2)
    MinAdjustmentMagnitude: NotRequired[int],
    Cooldown: NotRequired[int],
    MetricAggregationType: NotRequired[MetricAggregationTypeType],  # (3)
```

1. See [:material-code-brackets: AdjustmentTypeType](./literals.md#adjustmenttypetype) 
2. See [:material-code-braces: StepAdjustmentTypeDef](./type_defs.md#stepadjustmenttypedef) 
3. See [:material-code-brackets: MetricAggregationTypeType](./literals.md#metricaggregationtypetype) 
## TargetTrackingMetricOutputTypeDef

```python
# TargetTrackingMetricOutputTypeDef definition

class TargetTrackingMetricOutputTypeDef(TypedDict):
    Dimensions: NotRequired[List[TargetTrackingMetricDimensionTypeDef]],  # (1)
    MetricName: NotRequired[str],
    Namespace: NotRequired[str],
```

1. See [:material-code-braces: TargetTrackingMetricDimensionTypeDef](./type_defs.md#targettrackingmetricdimensiontypedef) 
## TargetTrackingMetricTypeDef

```python
# TargetTrackingMetricTypeDef definition

class TargetTrackingMetricTypeDef(TypedDict):
    Dimensions: NotRequired[Sequence[TargetTrackingMetricDimensionTypeDef]],  # (1)
    MetricName: NotRequired[str],
    Namespace: NotRequired[str],
```

1. See [:material-code-braces: TargetTrackingMetricDimensionTypeDef](./type_defs.md#targettrackingmetricdimensiontypedef) 
## DescribeScalingActivitiesResponseTypeDef

```python
# DescribeScalingActivitiesResponseTypeDef definition

class DescribeScalingActivitiesResponseTypeDef(TypedDict):
    ScalingActivities: List[ScalingActivityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScalingActivityTypeDef](./type_defs.md#scalingactivitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScheduledActionsResponseTypeDef

```python
# DescribeScheduledActionsResponseTypeDef definition

class DescribeScheduledActionsResponseTypeDef(TypedDict):
    ScheduledActions: List[ScheduledActionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScheduledActionTypeDef](./type_defs.md#scheduledactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScalableTargetsResponseTypeDef

```python
# DescribeScalableTargetsResponseTypeDef definition

class DescribeScalableTargetsResponseTypeDef(TypedDict):
    ScalableTargets: List[ScalableTargetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScalableTargetTypeDef](./type_defs.md#scalabletargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TargetTrackingMetricStatOutputTypeDef

```python
# TargetTrackingMetricStatOutputTypeDef definition

class TargetTrackingMetricStatOutputTypeDef(TypedDict):
    Metric: TargetTrackingMetricOutputTypeDef,  # (1)
    Stat: str,
    Unit: NotRequired[str],
```

1. See [:material-code-braces: TargetTrackingMetricOutputTypeDef](./type_defs.md#targettrackingmetricoutputtypedef) 
## TargetTrackingMetricDataQueryOutputTypeDef

```python
# TargetTrackingMetricDataQueryOutputTypeDef definition

class TargetTrackingMetricDataQueryOutputTypeDef(TypedDict):
    Id: str,
    Expression: NotRequired[str],
    Label: NotRequired[str],
    MetricStat: NotRequired[TargetTrackingMetricStatOutputTypeDef],  # (1)
    ReturnData: NotRequired[bool],
```

1. See [:material-code-braces: TargetTrackingMetricStatOutputTypeDef](./type_defs.md#targettrackingmetricstatoutputtypedef) 
## TargetTrackingMetricStatTypeDef

```python
# TargetTrackingMetricStatTypeDef definition

class TargetTrackingMetricStatTypeDef(TypedDict):
    Metric: TargetTrackingMetricUnionTypeDef,  # (1)
    Stat: str,
    Unit: NotRequired[str],
```

1. See [:material-code-braces: TargetTrackingMetricTypeDef](./type_defs.md#targettrackingmetrictypedef) [:material-code-braces: TargetTrackingMetricOutputTypeDef](./type_defs.md#targettrackingmetricoutputtypedef) 
## CustomizedMetricSpecificationOutputTypeDef

```python
# CustomizedMetricSpecificationOutputTypeDef definition

class CustomizedMetricSpecificationOutputTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Namespace: NotRequired[str],
    Dimensions: NotRequired[List[MetricDimensionTypeDef]],  # (1)
    Statistic: NotRequired[MetricStatisticType],  # (2)
    Unit: NotRequired[str],
    Metrics: NotRequired[List[TargetTrackingMetricDataQueryOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
3. See [:material-code-braces: TargetTrackingMetricDataQueryOutputTypeDef](./type_defs.md#targettrackingmetricdataqueryoutputtypedef) 
## TargetTrackingScalingPolicyConfigurationOutputTypeDef

```python
# TargetTrackingScalingPolicyConfigurationOutputTypeDef definition

class TargetTrackingScalingPolicyConfigurationOutputTypeDef(TypedDict):
    TargetValue: float,
    PredefinedMetricSpecification: NotRequired[PredefinedMetricSpecificationTypeDef],  # (1)
    CustomizedMetricSpecification: NotRequired[CustomizedMetricSpecificationOutputTypeDef],  # (2)
    ScaleOutCooldown: NotRequired[int],
    ScaleInCooldown: NotRequired[int],
    DisableScaleIn: NotRequired[bool],
```

1. See [:material-code-braces: PredefinedMetricSpecificationTypeDef](./type_defs.md#predefinedmetricspecificationtypedef) 
2. See [:material-code-braces: CustomizedMetricSpecificationOutputTypeDef](./type_defs.md#customizedmetricspecificationoutputtypedef) 
## TargetTrackingMetricDataQueryTypeDef

```python
# TargetTrackingMetricDataQueryTypeDef definition

class TargetTrackingMetricDataQueryTypeDef(TypedDict):
    Id: str,
    Expression: NotRequired[str],
    Label: NotRequired[str],
    MetricStat: NotRequired[TargetTrackingMetricStatUnionTypeDef],  # (1)
    ReturnData: NotRequired[bool],
```

1. See [:material-code-braces: TargetTrackingMetricStatTypeDef](./type_defs.md#targettrackingmetricstattypedef) [:material-code-braces: TargetTrackingMetricStatOutputTypeDef](./type_defs.md#targettrackingmetricstatoutputtypedef) 
## ScalingPolicyTypeDef

```python
# ScalingPolicyTypeDef definition

class ScalingPolicyTypeDef(TypedDict):
    PolicyARN: str,
    PolicyName: str,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    PolicyType: PolicyTypeType,  # (3)
    CreationTime: datetime,
    StepScalingPolicyConfiguration: NotRequired[StepScalingPolicyConfigurationOutputTypeDef],  # (4)
    TargetTrackingScalingPolicyConfiguration: NotRequired[TargetTrackingScalingPolicyConfigurationOutputTypeDef],  # (5)
    Alarms: NotRequired[List[AlarmTypeDef]],  # (6)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
4. See [:material-code-braces: StepScalingPolicyConfigurationOutputTypeDef](./type_defs.md#stepscalingpolicyconfigurationoutputtypedef) 
5. See [:material-code-braces: TargetTrackingScalingPolicyConfigurationOutputTypeDef](./type_defs.md#targettrackingscalingpolicyconfigurationoutputtypedef) 
6. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
## DescribeScalingPoliciesResponseTypeDef

```python
# DescribeScalingPoliciesResponseTypeDef definition

class DescribeScalingPoliciesResponseTypeDef(TypedDict):
    ScalingPolicies: List[ScalingPolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScalingPolicyTypeDef](./type_defs.md#scalingpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomizedMetricSpecificationTypeDef

```python
# CustomizedMetricSpecificationTypeDef definition

class CustomizedMetricSpecificationTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Namespace: NotRequired[str],
    Dimensions: NotRequired[Sequence[MetricDimensionTypeDef]],  # (1)
    Statistic: NotRequired[MetricStatisticType],  # (2)
    Unit: NotRequired[str],
    Metrics: NotRequired[Sequence[TargetTrackingMetricDataQueryUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
3. See [:material-code-braces: TargetTrackingMetricDataQueryTypeDef](./type_defs.md#targettrackingmetricdataquerytypedef) [:material-code-braces: TargetTrackingMetricDataQueryOutputTypeDef](./type_defs.md#targettrackingmetricdataqueryoutputtypedef) 
## TargetTrackingScalingPolicyConfigurationTypeDef

```python
# TargetTrackingScalingPolicyConfigurationTypeDef definition

class TargetTrackingScalingPolicyConfigurationTypeDef(TypedDict):
    TargetValue: float,
    PredefinedMetricSpecification: NotRequired[PredefinedMetricSpecificationTypeDef],  # (1)
    CustomizedMetricSpecification: NotRequired[CustomizedMetricSpecificationUnionTypeDef],  # (2)
    ScaleOutCooldown: NotRequired[int],
    ScaleInCooldown: NotRequired[int],
    DisableScaleIn: NotRequired[bool],
```

1. See [:material-code-braces: PredefinedMetricSpecificationTypeDef](./type_defs.md#predefinedmetricspecificationtypedef) 
2. See [:material-code-braces: CustomizedMetricSpecificationTypeDef](./type_defs.md#customizedmetricspecificationtypedef) [:material-code-braces: CustomizedMetricSpecificationOutputTypeDef](./type_defs.md#customizedmetricspecificationoutputtypedef) 
## PutScalingPolicyRequestRequestTypeDef

```python
# PutScalingPolicyRequestRequestTypeDef definition

class PutScalingPolicyRequestRequestTypeDef(TypedDict):
    PolicyName: str,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    PolicyType: NotRequired[PolicyTypeType],  # (3)
    StepScalingPolicyConfiguration: NotRequired[StepScalingPolicyConfigurationTypeDef],  # (4)
    TargetTrackingScalingPolicyConfiguration: NotRequired[TargetTrackingScalingPolicyConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
4. See [:material-code-braces: StepScalingPolicyConfigurationTypeDef](./type_defs.md#stepscalingpolicyconfigurationtypedef) 
5. See [:material-code-braces: TargetTrackingScalingPolicyConfigurationTypeDef](./type_defs.md#targettrackingscalingpolicyconfigurationtypedef) 
