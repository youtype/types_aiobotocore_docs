# CloudWatchServiceResource

> [Index](../README.md) > [CloudWatch](./README.md) > CloudWatchServiceResource

!!! note ""

    Auto-generated documentation for [CloudWatch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#cloudwatch)
    type annotations stubs module [types-aiobotocore-cloudwatch](https://pypi.org/project/types-aiobotocore-cloudwatch/).

## CloudWatchServiceResource

Type annotations and code completion for `#!python session.resource("cloudwatch")`, included resources and collections.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/service-resource/index.html)

```python
# CloudWatchServiceResource usage example

from types_aiobotocore_cloudwatch.service_resource import CloudWatchServiceResource

def get_cloudwatch_resource() -> CloudWatchServiceResource:
    return session.resource("cloudwatch")
```


## Attributes


- `meta`: `CloudWatchResourceMeta`

- `alarms`: `ServiceResourceAlarmsCollection`

- `metrics`: `ServiceResourceMetricsCollection`




## Collections

### ServiceResourceAlarmsCollection

Provides access to [Alarm](#alarm) resource.

Type annotations and code completion for `#!python session.resource("cloudwatch").alarms` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/service-resource/alarms.html#CloudWatch.ServiceResource.alarms)

```python
# ServiceResourceAlarmsCollection usage example

from types_aiobotocore_cloudwatch.service_resource import ServiceResourceAlarmsCollection

def get_collection() -> ServiceResourceAlarmsCollection:
    return session.resource("cloudwatch").alarms
```

### ServiceResourceMetricsCollection

Provides access to [Metric](#metric) resource.

Type annotations and code completion for `#!python session.resource("cloudwatch").metrics` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/service-resource/metrics.html#CloudWatch.ServiceResource.metrics)

```python
# ServiceResourceMetricsCollection usage example

from types_aiobotocore_cloudwatch.service_resource import ServiceResourceMetricsCollection

def get_collection() -> ServiceResourceMetricsCollection:
    return session.resource("cloudwatch").metrics
```



## Methods

### CloudWatchServiceResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this resource.

Type annotations and code completion for `#!python session.resource("cloudwatch").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/service-resource/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


### CloudWatchServiceResource.Alarm method

Creates a Alarm resource.

Type annotations and code completion for `#!python session.resource("cloudwatch").Alarm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/service-resource/Alarm.html)

```python
# Alarm method definition

await def Alarm(
    self,
    name: str,
) -> _Alarm:
    ...
```


### CloudWatchServiceResource.Metric method

Creates a Metric resource.

Type annotations and code completion for `#!python session.resource("cloudwatch").Metric` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/service-resource/Metric.html)

```python
# Metric method definition

await def Metric(
    self,
    namespace: str,
    name: str,
) -> _Metric:
    ...
```




## Alarm

Type annotations and code completion for `#!python session.resource("cloudwatch").Alarm` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/alarm/index.html#CloudWatch.Alarm)

```python
# Alarm usage example

from types_aiobotocore_cloudwatch.service_resource import Alarm

def get_resource() -> Alarm:
    return session.resource("cloudwatch").Alarm(...)
```


### Alarm attributes


- `name`: `str`
- `metric`: `Metric`
- `alarm_name`: `Awaitable`[`str`]
- `alarm_arn`: `Awaitable`[`str`]
- `alarm_description`: `Awaitable`[`str`]
- `alarm_configuration_updated_timestamp`: `Awaitable`[`datetime`]
- `actions_enabled`: `Awaitable`[`bool`]
- `ok_actions`: `Awaitable`[`List`[`str`]]
- `alarm_actions`: `Awaitable`[`List`[`str`]]
- `insufficient_data_actions`: `Awaitable`[`List`[`str`]]
- `state_value`: `Awaitable`[[StateValueType](./literals.md#statevaluetype)]
- `state_reason`: `Awaitable`[`str`]
- `state_reason_data`: `Awaitable`[`str`]
- `state_updated_timestamp`: `Awaitable`[`datetime`]
- `metric_name`: `Awaitable`[`str`]
- `namespace`: `Awaitable`[`str`]
- `statistic`: `Awaitable`[[StatisticType](./literals.md#statistictype)]
- `extended_statistic`: `Awaitable`[`str`]
- `dimensions`: `Awaitable`[`List`[[DimensionTypeDef](./type_defs.md#dimensiontypedef)]]
- `period`: `Awaitable`[`int`]
- `unit`: `Awaitable`[[StandardUnitType](./literals.md#standardunittype)]
- `evaluation_periods`: `Awaitable`[`int`]
- `datapoints_to_alarm`: `Awaitable`[`int`]
- `threshold`: `Awaitable`[`float`]
- `comparison_operator`: `Awaitable`[[ComparisonOperatorType](./literals.md#comparisonoperatortype)]
- `treat_missing_data`: `Awaitable`[`str`]
- `evaluate_low_sample_count_percentile`: `Awaitable`[`str`]
- `metrics`: `Awaitable`[`List`[[MetricDataQueryAlarmTypeDef](./type_defs.md#metricdataqueryalarmtypedef)]]
- `threshold_metric_id`: `Awaitable`[`str`]
- `evaluation_state`: `Awaitable`[`Literal['PARTIAL_DATA']` (see [EvaluationStateType](./literals.md#evaluationstatetype))]
- `state_transitioned_timestamp`: `Awaitable`[`datetime`]
- `meta`: `CloudWatchResourceMeta`





### Alarm methods


#### Alarm.get\_available\_subresources method

Returns a list of all the available sub-resources for this Alarm.

Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/alarm/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Alarm.delete method

Deletes the specified alarms.

Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/alarm/delete.html)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Alarm.describe\_history method

Retrieves the history for the specified alarm.

Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").describe_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/alarm/describe_history.html)

```python
# describe_history method definition

await def describe_history(
    self,
    *,
    AlarmTypes: Sequence[AlarmTypeType] = ...,  # (1)
    HistoryItemType: HistoryItemTypeType = ...,  # (2)
    StartDate: TimestampTypeDef = ...,
    EndDate: TimestampTypeDef = ...,
    MaxRecords: int = ...,
    NextToken: str = ...,
    ScanBy: ScanByType = ...,  # (3)
) -> DescribeAlarmHistoryOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: HistoryItemTypeType](./literals.md#historyitemtypetype) 
3. See [:material-code-brackets: ScanByType](./literals.md#scanbytype) 
4. See [:material-code-braces: DescribeAlarmHistoryOutputTypeDef](./type_defs.md#describealarmhistoryoutputtypedef) 


```python
# describe_history method usage example with argument unpacking

kwargs: DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef = {  # (1)
    "AlarmTypes": ...,
}

parent.describe_history(**kwargs)
```

1. See [:material-code-braces: DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef](./type_defs.md#describealarmhistoryinputalarmdescribehistorytypedef) 

#### Alarm.disable\_actions method

Disables the actions for the specified alarms.

Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").disable_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/alarm/disable_actions.html)

```python
# disable_actions method definition

await def disable_actions(
    self,
) -> None:
    ...
```


#### Alarm.enable\_actions method

Enables the actions for the specified alarms.

Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").enable_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/alarm/enable_actions.html)

```python
# enable_actions method definition

await def enable_actions(
    self,
) -> None:
    ...
```


#### Alarm.set\_state method

Temporarily sets the state of an alarm for testing purposes.

Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").set_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/alarm/set_state.html)

```python
# set_state method definition

await def set_state(
    self,
    *,
    StateValue: StateValueType,  # (1)
    StateReason: str,
    StateReasonData: str = ...,
) -> None:
    ...
```

1. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 


```python
# set_state method usage example with argument unpacking

kwargs: SetAlarmStateInputAlarmSetStateTypeDef = {  # (1)
    "StateValue": ...,
    "StateReason": ...,
}

parent.set_state(**kwargs)
```

1. See [:material-code-braces: SetAlarmStateInputAlarmSetStateTypeDef](./type_defs.md#setalarmstateinputalarmsetstatetypedef) 

#### Alarm.load method



Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/alarm/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Alarm.reload method



Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/alarm/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```





## Metric

Type annotations and code completion for `#!python session.resource("cloudwatch").Metric` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/metric/index.html#CloudWatch.Metric)

```python
# Metric usage example

from types_aiobotocore_cloudwatch.service_resource import Metric

def get_resource() -> Metric:
    return session.resource("cloudwatch").Metric(...)
```


### Metric attributes


- `namespace`: `str`
- `name`: `str`
- `alarms`: `MetricAlarmsCollection`
- `metric_name`: `Awaitable`[`str`]
- `dimensions`: `Awaitable`[`List`[[DimensionTypeDef](./type_defs.md#dimensiontypedef)]]
- `meta`: `CloudWatchResourceMeta`



### Metric collections


#### Metric.alarms

Provides access to [Alarm](#alarm) resource.

Type annotations and code completion for `#!python session.resource("cloudwatch").Metric(...).alarms` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/metric/alarms.html#CloudWatch.Metric.alarms)

```python
# MetricAlarmsCollection usage example

from types_aiobotocore_cloudwatch.service_resource import MetricAlarmsCollection

def get_collection() -> MetricAlarmsCollection:
    resource = session.resource("cloudwatch").Metric(...)
    return resource.alarms
```




### Metric methods


#### Metric.get\_available\_subresources method

Returns a list of all the available sub-resources for this Metric.

Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/metric/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Metric.get\_statistics method

Gets statistics for the specified metric.

Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").get_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/metric/get_statistics.html)

```python
# get_statistics method definition

await def get_statistics(
    self,
    *,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Period: int,
    Dimensions: Sequence[DimensionTypeDef] = ...,  # (1)
    Statistics: Sequence[StatisticType] = ...,  # (2)
    ExtendedStatistics: Sequence[str] = ...,
    Unit: StandardUnitType = ...,  # (3)
) -> GetMetricStatisticsOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
4. See [:material-code-braces: GetMetricStatisticsOutputTypeDef](./type_defs.md#getmetricstatisticsoutputtypedef) 


```python
# get_statistics method usage example with argument unpacking

kwargs: GetMetricStatisticsInputMetricGetStatisticsTypeDef = {  # (1)
    "StartTime": ...,
    "EndTime": ...,
    "Period": ...,
}

parent.get_statistics(**kwargs)
```

1. See [:material-code-braces: GetMetricStatisticsInputMetricGetStatisticsTypeDef](./type_defs.md#getmetricstatisticsinputmetricgetstatisticstypedef) 

#### Metric.put\_alarm method

Creates or updates an alarm and associates it with the specified metric, metric
math expression, anomaly detection model, or Metrics Insights query.

Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").put_alarm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/metric/put_alarm.html)

```python
# put_alarm method definition

await def put_alarm(
    self,
    *,
    AlarmName: str,
    EvaluationPeriods: int,
    ComparisonOperator: ComparisonOperatorType,  # (1)
    AlarmDescription: str = ...,
    ActionsEnabled: bool = ...,
    OKActions: Sequence[str] = ...,
    AlarmActions: Sequence[str] = ...,
    InsufficientDataActions: Sequence[str] = ...,
    Statistic: StatisticType = ...,  # (2)
    ExtendedStatistic: str = ...,
    Dimensions: Sequence[DimensionTypeDef] = ...,  # (3)
    Period: int = ...,
    Unit: StandardUnitType = ...,  # (4)
    DatapointsToAlarm: int = ...,
    Threshold: float = ...,
    TreatMissingData: str = ...,
    EvaluateLowSampleCountPercentile: str = ...,
    Metrics: Sequence[MetricDataQueryUnionTypeDef] = ...,  # (5)
    Tags: Sequence[TagTypeDef] = ...,  # (6)
    ThresholdMetricId: str = ...,
) -> _Alarm:
    ...
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
4. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
5. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# put_alarm method usage example with argument unpacking

kwargs: PutMetricAlarmInputMetricPutAlarmTypeDef = {  # (1)
    "AlarmName": ...,
    "EvaluationPeriods": ...,
    "ComparisonOperator": ...,
}

parent.put_alarm(**kwargs)
```

1. See [:material-code-braces: PutMetricAlarmInputMetricPutAlarmTypeDef](./type_defs.md#putmetricalarminputmetricputalarmtypedef) 

#### Metric.put\_data method

Publishes metric data to Amazon CloudWatch.

Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").put_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/metric/put_data.html)

```python
# put_data method definition

await def put_data(
    self,
    *,
    EntityMetricData: Sequence[EntityMetricDataTypeDef] = ...,  # (1)
    StrictEntityValidation: bool = ...,
) -> None:
    ...
```

1. See [:material-code-braces: EntityMetricDataTypeDef](./type_defs.md#entitymetricdatatypedef) 


```python
# put_data method usage example with argument unpacking

kwargs: PutMetricDataInputMetricPutDataTypeDef = {  # (1)
    "EntityMetricData": ...,
}

parent.put_data(**kwargs)
```

1. See [:material-code-braces: PutMetricDataInputMetricPutDataTypeDef](./type_defs.md#putmetricdatainputmetricputdatatypedef) 

#### Metric.load method



Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/metric/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Metric.reload method



Type annotations and code completion for `#!python aiobotocore.resource("cloudwatch").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/metric/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```




