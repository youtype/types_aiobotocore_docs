# Type definitions

> [Index](../README.md) > [AutoScalingPlans](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AutoScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
    type annotations stubs module [types-aiobotocore-autoscaling-plans](https://pypi.org/project/types-aiobotocore-autoscaling-plans/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## TagFilterUnionTypeDef

```python
# TagFilterUnionTypeDef definition

TagFilterUnionTypeDef = Union[
    TagFilterTypeDef,  # (1)
    TagFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
2. See [:material-code-braces: TagFilterOutputTypeDef](./type_defs.md#tagfilteroutputtypedef) 

## CustomizedLoadMetricSpecificationUnionTypeDef

```python
# CustomizedLoadMetricSpecificationUnionTypeDef definition

CustomizedLoadMetricSpecificationUnionTypeDef = Union[
    CustomizedLoadMetricSpecificationTypeDef,  # (1)
    CustomizedLoadMetricSpecificationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomizedLoadMetricSpecificationTypeDef](./type_defs.md#customizedloadmetricspecificationtypedef) 
2. See [:material-code-braces: CustomizedLoadMetricSpecificationOutputTypeDef](./type_defs.md#customizedloadmetricspecificationoutputtypedef) 

## CustomizedScalingMetricSpecificationUnionTypeDef

```python
# CustomizedScalingMetricSpecificationUnionTypeDef definition

CustomizedScalingMetricSpecificationUnionTypeDef = Union[
    CustomizedScalingMetricSpecificationTypeDef,  # (1)
    CustomizedScalingMetricSpecificationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomizedScalingMetricSpecificationTypeDef](./type_defs.md#customizedscalingmetricspecificationtypedef) 
2. See [:material-code-braces: CustomizedScalingMetricSpecificationOutputTypeDef](./type_defs.md#customizedscalingmetricspecificationoutputtypedef) 

## ApplicationSourceUnionTypeDef

```python
# ApplicationSourceUnionTypeDef definition

ApplicationSourceUnionTypeDef = Union[
    ApplicationSourceTypeDef,  # (1)
    ApplicationSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: ApplicationSourceOutputTypeDef](./type_defs.md#applicationsourceoutputtypedef) 

## TargetTrackingConfigurationUnionTypeDef

```python
# TargetTrackingConfigurationUnionTypeDef definition

TargetTrackingConfigurationUnionTypeDef = Union[
    TargetTrackingConfigurationTypeDef,  # (1)
    TargetTrackingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TargetTrackingConfigurationTypeDef](./type_defs.md#targettrackingconfigurationtypedef) 
2. See [:material-code-braces: TargetTrackingConfigurationOutputTypeDef](./type_defs.md#targettrackingconfigurationoutputtypedef) 

## ScalingInstructionUnionTypeDef

```python
# ScalingInstructionUnionTypeDef definition

ScalingInstructionUnionTypeDef = Union[
    ScalingInstructionTypeDef,  # (1)
    ScalingInstructionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef) 
2. See [:material-code-braces: ScalingInstructionOutputTypeDef](./type_defs.md#scalinginstructionoutputtypedef) 



## TagFilterOutputTypeDef

```python
# TagFilterOutputTypeDef definition

class TagFilterOutputTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[List[str]],
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

## MetricDimensionTypeDef

```python
# MetricDimensionTypeDef definition

class MetricDimensionTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## DatapointTypeDef

```python
# DatapointTypeDef definition

class DatapointTypeDef(TypedDict):
    Timestamp: NotRequired[datetime],
    Value: NotRequired[float],
```

## DeleteScalingPlanRequestRequestTypeDef

```python
# DeleteScalingPlanRequestRequestTypeDef definition

class DeleteScalingPlanRequestRequestTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeScalingPlanResourcesRequestRequestTypeDef

```python
# DescribeScalingPlanResourcesRequestRequestTypeDef definition

class DescribeScalingPlanResourcesRequestRequestTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PredefinedLoadMetricSpecificationTypeDef

```python
# PredefinedLoadMetricSpecificationTypeDef definition

class PredefinedLoadMetricSpecificationTypeDef(TypedDict):
    PredefinedLoadMetricType: LoadMetricTypeType,  # (1)
    ResourceLabel: NotRequired[str],
```

1. See [:material-code-brackets: LoadMetricTypeType](./literals.md#loadmetrictypetype) 
## PredefinedScalingMetricSpecificationTypeDef

```python
# PredefinedScalingMetricSpecificationTypeDef definition

class PredefinedScalingMetricSpecificationTypeDef(TypedDict):
    PredefinedScalingMetricType: ScalingMetricTypeType,  # (1)
    ResourceLabel: NotRequired[str],
```

1. See [:material-code-brackets: ScalingMetricTypeType](./literals.md#scalingmetrictypetype) 
## TagFilterTypeDef

```python
# TagFilterTypeDef definition

class TagFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## ApplicationSourceOutputTypeDef

```python
# ApplicationSourceOutputTypeDef definition

class ApplicationSourceOutputTypeDef(TypedDict):
    CloudFormationStackARN: NotRequired[str],
    TagFilters: NotRequired[List[TagFilterOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: TagFilterOutputTypeDef](./type_defs.md#tagfilteroutputtypedef) 
## CreateScalingPlanResponseTypeDef

```python
# CreateScalingPlanResponseTypeDef definition

class CreateScalingPlanResponseTypeDef(TypedDict):
    ScalingPlanVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomizedLoadMetricSpecificationOutputTypeDef

```python
# CustomizedLoadMetricSpecificationOutputTypeDef definition

class CustomizedLoadMetricSpecificationOutputTypeDef(TypedDict):
    MetricName: str,
    Namespace: str,
    Statistic: MetricStatisticType,  # (2)
    Dimensions: NotRequired[List[MetricDimensionTypeDef]],  # (1)
    Unit: NotRequired[str],
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## CustomizedLoadMetricSpecificationTypeDef

```python
# CustomizedLoadMetricSpecificationTypeDef definition

class CustomizedLoadMetricSpecificationTypeDef(TypedDict):
    MetricName: str,
    Namespace: str,
    Statistic: MetricStatisticType,  # (2)
    Dimensions: NotRequired[Sequence[MetricDimensionTypeDef]],  # (1)
    Unit: NotRequired[str],
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## CustomizedScalingMetricSpecificationOutputTypeDef

```python
# CustomizedScalingMetricSpecificationOutputTypeDef definition

class CustomizedScalingMetricSpecificationOutputTypeDef(TypedDict):
    MetricName: str,
    Namespace: str,
    Statistic: MetricStatisticType,  # (2)
    Dimensions: NotRequired[List[MetricDimensionTypeDef]],  # (1)
    Unit: NotRequired[str],
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## CustomizedScalingMetricSpecificationTypeDef

```python
# CustomizedScalingMetricSpecificationTypeDef definition

class CustomizedScalingMetricSpecificationTypeDef(TypedDict):
    MetricName: str,
    Namespace: str,
    Statistic: MetricStatisticType,  # (2)
    Dimensions: NotRequired[Sequence[MetricDimensionTypeDef]],  # (1)
    Unit: NotRequired[str],
```

1. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## GetScalingPlanResourceForecastDataResponseTypeDef

```python
# GetScalingPlanResourceForecastDataResponseTypeDef definition

class GetScalingPlanResourceForecastDataResponseTypeDef(TypedDict):
    Datapoints: List[DatapointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatapointTypeDef](./type_defs.md#datapointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef

```python
# DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef definition

class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetScalingPlanResourceForecastDataRequestRequestTypeDef

```python
# GetScalingPlanResourceForecastDataRequestRequestTypeDef definition

class GetScalingPlanResourceForecastDataRequestRequestTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    ForecastDataType: ForecastDataTypeType,  # (3)
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-brackets: ForecastDataTypeType](./literals.md#forecastdatatypetype) 
## TargetTrackingConfigurationOutputTypeDef

```python
# TargetTrackingConfigurationOutputTypeDef definition

class TargetTrackingConfigurationOutputTypeDef(TypedDict):
    TargetValue: float,
    PredefinedScalingMetricSpecification: NotRequired[PredefinedScalingMetricSpecificationTypeDef],  # (1)
    CustomizedScalingMetricSpecification: NotRequired[CustomizedScalingMetricSpecificationOutputTypeDef],  # (2)
    DisableScaleIn: NotRequired[bool],
    ScaleOutCooldown: NotRequired[int],
    ScaleInCooldown: NotRequired[int],
    EstimatedInstanceWarmup: NotRequired[int],
```

1. See [:material-code-braces: PredefinedScalingMetricSpecificationTypeDef](./type_defs.md#predefinedscalingmetricspecificationtypedef) 
2. See [:material-code-braces: CustomizedScalingMetricSpecificationOutputTypeDef](./type_defs.md#customizedscalingmetricspecificationoutputtypedef) 
## ApplicationSourceTypeDef

```python
# ApplicationSourceTypeDef definition

class ApplicationSourceTypeDef(TypedDict):
    CloudFormationStackARN: NotRequired[str],
    TagFilters: NotRequired[Sequence[TagFilterUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) [:material-code-braces: TagFilterOutputTypeDef](./type_defs.md#tagfilteroutputtypedef) 
## ScalingInstructionOutputTypeDef

```python
# ScalingInstructionOutputTypeDef definition

class ScalingInstructionOutputTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    MinCapacity: int,
    MaxCapacity: int,
    TargetTrackingConfigurations: List[TargetTrackingConfigurationOutputTypeDef],  # (3)
    PredefinedLoadMetricSpecification: NotRequired[PredefinedLoadMetricSpecificationTypeDef],  # (4)
    CustomizedLoadMetricSpecification: NotRequired[CustomizedLoadMetricSpecificationOutputTypeDef],  # (5)
    ScheduledActionBufferTime: NotRequired[int],
    PredictiveScalingMaxCapacityBehavior: NotRequired[PredictiveScalingMaxCapacityBehaviorType],  # (6)
    PredictiveScalingMaxCapacityBuffer: NotRequired[int],
    PredictiveScalingMode: NotRequired[PredictiveScalingModeType],  # (7)
    ScalingPolicyUpdateBehavior: NotRequired[ScalingPolicyUpdateBehaviorType],  # (8)
    DisableDynamicScaling: NotRequired[bool],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: TargetTrackingConfigurationOutputTypeDef](./type_defs.md#targettrackingconfigurationoutputtypedef) 
4. See [:material-code-braces: PredefinedLoadMetricSpecificationTypeDef](./type_defs.md#predefinedloadmetricspecificationtypedef) 
5. See [:material-code-braces: CustomizedLoadMetricSpecificationOutputTypeDef](./type_defs.md#customizedloadmetricspecificationoutputtypedef) 
6. See [:material-code-brackets: PredictiveScalingMaxCapacityBehaviorType](./literals.md#predictivescalingmaxcapacitybehaviortype) 
7. See [:material-code-brackets: PredictiveScalingModeType](./literals.md#predictivescalingmodetype) 
8. See [:material-code-brackets: ScalingPolicyUpdateBehaviorType](./literals.md#scalingpolicyupdatebehaviortype) 
## ScalingPolicyTypeDef

```python
# ScalingPolicyTypeDef definition

class ScalingPolicyTypeDef(TypedDict):
    PolicyName: str,
    PolicyType: PolicyTypeType,  # (1)
    TargetTrackingConfiguration: NotRequired[TargetTrackingConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: TargetTrackingConfigurationOutputTypeDef](./type_defs.md#targettrackingconfigurationoutputtypedef) 
## TargetTrackingConfigurationTypeDef

```python
# TargetTrackingConfigurationTypeDef definition

class TargetTrackingConfigurationTypeDef(TypedDict):
    TargetValue: float,
    PredefinedScalingMetricSpecification: NotRequired[PredefinedScalingMetricSpecificationTypeDef],  # (1)
    CustomizedScalingMetricSpecification: NotRequired[CustomizedScalingMetricSpecificationUnionTypeDef],  # (2)
    DisableScaleIn: NotRequired[bool],
    ScaleOutCooldown: NotRequired[int],
    ScaleInCooldown: NotRequired[int],
    EstimatedInstanceWarmup: NotRequired[int],
```

1. See [:material-code-braces: PredefinedScalingMetricSpecificationTypeDef](./type_defs.md#predefinedscalingmetricspecificationtypedef) 
2. See [:material-code-braces: CustomizedScalingMetricSpecificationTypeDef](./type_defs.md#customizedscalingmetricspecificationtypedef) [:material-code-braces: CustomizedScalingMetricSpecificationOutputTypeDef](./type_defs.md#customizedscalingmetricspecificationoutputtypedef) 
## DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef

```python
# DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef definition

class DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef(TypedDict):
    ScalingPlanNames: NotRequired[Sequence[str]],
    ScalingPlanVersion: NotRequired[int],
    ApplicationSources: NotRequired[Sequence[ApplicationSourceTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ScalingPlanTypeDef

```python
# ScalingPlanTypeDef definition

class ScalingPlanTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ApplicationSource: ApplicationSourceOutputTypeDef,  # (1)
    ScalingInstructions: List[ScalingInstructionOutputTypeDef],  # (2)
    StatusCode: ScalingPlanStatusCodeType,  # (3)
    StatusMessage: NotRequired[str],
    StatusStartTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
```

1. See [:material-code-braces: ApplicationSourceOutputTypeDef](./type_defs.md#applicationsourceoutputtypedef) 
2. See [:material-code-braces: ScalingInstructionOutputTypeDef](./type_defs.md#scalinginstructionoutputtypedef) 
3. See [:material-code-brackets: ScalingPlanStatusCodeType](./literals.md#scalingplanstatuscodetype) 
## ScalingPlanResourceTypeDef

```python
# ScalingPlanResourceTypeDef definition

class ScalingPlanResourceTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    ScalingStatusCode: ScalingStatusCodeType,  # (4)
    ScalingPolicies: NotRequired[List[ScalingPolicyTypeDef]],  # (3)
    ScalingStatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: ScalingPolicyTypeDef](./type_defs.md#scalingpolicytypedef) 
4. See [:material-code-brackets: ScalingStatusCodeType](./literals.md#scalingstatuscodetype) 
## DescribeScalingPlansRequestRequestTypeDef

```python
# DescribeScalingPlansRequestRequestTypeDef definition

class DescribeScalingPlansRequestRequestTypeDef(TypedDict):
    ScalingPlanNames: NotRequired[Sequence[str]],
    ScalingPlanVersion: NotRequired[int],
    ApplicationSources: NotRequired[Sequence[ApplicationSourceUnionTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) [:material-code-braces: ApplicationSourceOutputTypeDef](./type_defs.md#applicationsourceoutputtypedef) 
## DescribeScalingPlansResponseTypeDef

```python
# DescribeScalingPlansResponseTypeDef definition

class DescribeScalingPlansResponseTypeDef(TypedDict):
    ScalingPlans: List[ScalingPlanTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScalingPlanTypeDef](./type_defs.md#scalingplantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScalingPlanResourcesResponseTypeDef

```python
# DescribeScalingPlanResourcesResponseTypeDef definition

class DescribeScalingPlanResourcesResponseTypeDef(TypedDict):
    ScalingPlanResources: List[ScalingPlanResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScalingPlanResourceTypeDef](./type_defs.md#scalingplanresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScalingInstructionTypeDef

```python
# ScalingInstructionTypeDef definition

class ScalingInstructionTypeDef(TypedDict):
    ServiceNamespace: ServiceNamespaceType,  # (1)
    ResourceId: str,
    ScalableDimension: ScalableDimensionType,  # (2)
    MinCapacity: int,
    MaxCapacity: int,
    TargetTrackingConfigurations: Sequence[TargetTrackingConfigurationUnionTypeDef],  # (3)
    PredefinedLoadMetricSpecification: NotRequired[PredefinedLoadMetricSpecificationTypeDef],  # (4)
    CustomizedLoadMetricSpecification: NotRequired[CustomizedLoadMetricSpecificationUnionTypeDef],  # (5)
    ScheduledActionBufferTime: NotRequired[int],
    PredictiveScalingMaxCapacityBehavior: NotRequired[PredictiveScalingMaxCapacityBehaviorType],  # (6)
    PredictiveScalingMaxCapacityBuffer: NotRequired[int],
    PredictiveScalingMode: NotRequired[PredictiveScalingModeType],  # (7)
    ScalingPolicyUpdateBehavior: NotRequired[ScalingPolicyUpdateBehaviorType],  # (8)
    DisableDynamicScaling: NotRequired[bool],
```

1. See [:material-code-brackets: ServiceNamespaceType](./literals.md#servicenamespacetype) 
2. See [:material-code-brackets: ScalableDimensionType](./literals.md#scalabledimensiontype) 
3. See [:material-code-braces: TargetTrackingConfigurationTypeDef](./type_defs.md#targettrackingconfigurationtypedef) [:material-code-braces: TargetTrackingConfigurationOutputTypeDef](./type_defs.md#targettrackingconfigurationoutputtypedef) 
4. See [:material-code-braces: PredefinedLoadMetricSpecificationTypeDef](./type_defs.md#predefinedloadmetricspecificationtypedef) 
5. See [:material-code-braces: CustomizedLoadMetricSpecificationTypeDef](./type_defs.md#customizedloadmetricspecificationtypedef) [:material-code-braces: CustomizedLoadMetricSpecificationOutputTypeDef](./type_defs.md#customizedloadmetricspecificationoutputtypedef) 
6. See [:material-code-brackets: PredictiveScalingMaxCapacityBehaviorType](./literals.md#predictivescalingmaxcapacitybehaviortype) 
7. See [:material-code-brackets: PredictiveScalingModeType](./literals.md#predictivescalingmodetype) 
8. See [:material-code-brackets: ScalingPolicyUpdateBehaviorType](./literals.md#scalingpolicyupdatebehaviortype) 
## UpdateScalingPlanRequestRequestTypeDef

```python
# UpdateScalingPlanRequestRequestTypeDef definition

class UpdateScalingPlanRequestRequestTypeDef(TypedDict):
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    ApplicationSource: NotRequired[ApplicationSourceTypeDef],  # (1)
    ScalingInstructions: NotRequired[Sequence[ScalingInstructionTypeDef]],  # (2)
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef) 
## CreateScalingPlanRequestRequestTypeDef

```python
# CreateScalingPlanRequestRequestTypeDef definition

class CreateScalingPlanRequestRequestTypeDef(TypedDict):
    ScalingPlanName: str,
    ApplicationSource: ApplicationSourceTypeDef,  # (1)
    ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) 
2. See [:material-code-braces: ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef) [:material-code-braces: ScalingInstructionOutputTypeDef](./type_defs.md#scalinginstructionoutputtypedef) 
