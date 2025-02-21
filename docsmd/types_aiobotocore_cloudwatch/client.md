# CloudWatchClient

> [Index](../README.md) > [CloudWatch](./README.md) > CloudWatchClient

!!! note ""

    Auto-generated documentation for [CloudWatch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#cloudwatch)
    type annotations stubs module [types-aiobotocore-cloudwatch](https://pypi.org/project/types-aiobotocore-cloudwatch/).

## CloudWatchClient

Type annotations and code completion for `#!python session.create_client("cloudwatch")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client)

```python
# CloudWatchClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_cloudwatch.client import CloudWatchClient

session = get_session()
async with session.create_client("cloudwatch") as client:
    client: CloudWatchClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cloudwatch").exceptions` structure.

```python
# CloudWatchClient.exceptions usage example

async with session.create_client("cloudwatch") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConcurrentModificationException,
        client.DashboardInvalidInputError,
        client.DashboardNotFoundError,
        client.InternalServiceFault,
        client.InvalidFormatFault,
        client.InvalidNextToken,
        client.InvalidParameterCombinationException,
        client.InvalidParameterValueException,
        client.LimitExceededException,
        client.LimitExceededFault,
        client.MissingRequiredParameterException,
        client.ResourceNotFound,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# CloudWatchClient usage type checking example

from types_aiobotocore_cloudwatch.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("cloudwatch").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("cloudwatch").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### delete\_alarms

Deletes the specified alarms.

Type annotations and code completion for `#!python session.create_client("cloudwatch").delete_alarms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/delete_alarms.html)

```python
# delete_alarms method definition

await def delete_alarms(
    self,
    *,
    AlarmNames: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_alarms method usage example with argument unpacking

kwargs: DeleteAlarmsInputTypeDef = {  # (1)
    "AlarmNames": ...,
}

parent.delete_alarms(**kwargs)
```

1. See [:material-code-braces: DeleteAlarmsInputTypeDef](./type_defs.md#deletealarmsinputtypedef) 

### delete\_anomaly\_detector

Deletes the specified anomaly detection model from your account.

Type annotations and code completion for `#!python session.create_client("cloudwatch").delete_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/delete_anomaly_detector.html)

```python
# delete_anomaly_detector method definition

await def delete_anomaly_detector(
    self,
    *,
    Namespace: str = ...,
    MetricName: str = ...,
    Dimensions: Sequence[DimensionTypeDef] = ...,  # (1)
    Stat: str = ...,
    SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,  # (2)
    MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...,  # (3)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-braces: SingleMetricAnomalyDetectorTypeDef](./type_defs.md#singlemetricanomalydetectortypedef) [:material-code-braces: SingleMetricAnomalyDetectorOutputTypeDef](./type_defs.md#singlemetricanomalydetectoroutputtypedef) 
3. See [:material-code-braces: MetricMathAnomalyDetectorTypeDef](./type_defs.md#metricmathanomalydetectortypedef) [:material-code-braces: MetricMathAnomalyDetectorOutputTypeDef](./type_defs.md#metricmathanomalydetectoroutputtypedef) 


```python
# delete_anomaly_detector method usage example with argument unpacking

kwargs: DeleteAnomalyDetectorInputTypeDef = {  # (1)
    "Namespace": ...,
}

parent.delete_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: DeleteAnomalyDetectorInputTypeDef](./type_defs.md#deleteanomalydetectorinputtypedef) 

### delete\_dashboards

Deletes all dashboards that you specify.

Type annotations and code completion for `#!python session.create_client("cloudwatch").delete_dashboards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/delete_dashboards.html)

```python
# delete_dashboards method definition

await def delete_dashboards(
    self,
    *,
    DashboardNames: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# delete_dashboards method usage example with argument unpacking

kwargs: DeleteDashboardsInputTypeDef = {  # (1)
    "DashboardNames": ...,
}

parent.delete_dashboards(**kwargs)
```

1. See [:material-code-braces: DeleteDashboardsInputTypeDef](./type_defs.md#deletedashboardsinputtypedef) 

### delete\_insight\_rules

Permanently deletes the specified Contributor Insights rules.

Type annotations and code completion for `#!python session.create_client("cloudwatch").delete_insight_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/delete_insight_rules.html)

```python
# delete_insight_rules method definition

await def delete_insight_rules(
    self,
    *,
    RuleNames: Sequence[str],
) -> DeleteInsightRulesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteInsightRulesOutputTypeDef](./type_defs.md#deleteinsightrulesoutputtypedef) 


```python
# delete_insight_rules method usage example with argument unpacking

kwargs: DeleteInsightRulesInputTypeDef = {  # (1)
    "RuleNames": ...,
}

parent.delete_insight_rules(**kwargs)
```

1. See [:material-code-braces: DeleteInsightRulesInputTypeDef](./type_defs.md#deleteinsightrulesinputtypedef) 

### delete\_metric\_stream

Permanently deletes the metric stream that you specify.

Type annotations and code completion for `#!python session.create_client("cloudwatch").delete_metric_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/delete_metric_stream.html)

```python
# delete_metric_stream method definition

await def delete_metric_stream(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_metric_stream method usage example with argument unpacking

kwargs: DeleteMetricStreamInputTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_metric_stream(**kwargs)
```

1. See [:material-code-braces: DeleteMetricStreamInputTypeDef](./type_defs.md#deletemetricstreaminputtypedef) 

### describe\_alarm\_history

Retrieves the history for the specified alarm.

Type annotations and code completion for `#!python session.create_client("cloudwatch").describe_alarm_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/describe_alarm_history.html)

```python
# describe_alarm_history method definition

await def describe_alarm_history(
    self,
    *,
    AlarmName: str = ...,
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
# describe_alarm_history method usage example with argument unpacking

kwargs: DescribeAlarmHistoryInputTypeDef = {  # (1)
    "AlarmName": ...,
}

parent.describe_alarm_history(**kwargs)
```

1. See [:material-code-braces: DescribeAlarmHistoryInputTypeDef](./type_defs.md#describealarmhistoryinputtypedef) 

### describe\_alarms

Retrieves the specified alarms.

Type annotations and code completion for `#!python session.create_client("cloudwatch").describe_alarms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/describe_alarms.html)

```python
# describe_alarms method definition

await def describe_alarms(
    self,
    *,
    AlarmNames: Sequence[str] = ...,
    AlarmNamePrefix: str = ...,
    AlarmTypes: Sequence[AlarmTypeType] = ...,  # (1)
    ChildrenOfAlarmName: str = ...,
    ParentsOfAlarmName: str = ...,
    StateValue: StateValueType = ...,  # (2)
    ActionPrefix: str = ...,
    MaxRecords: int = ...,
    NextToken: str = ...,
) -> DescribeAlarmsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
3. See [:material-code-braces: DescribeAlarmsOutputTypeDef](./type_defs.md#describealarmsoutputtypedef) 


```python
# describe_alarms method usage example with argument unpacking

kwargs: DescribeAlarmsInputTypeDef = {  # (1)
    "AlarmNames": ...,
}

parent.describe_alarms(**kwargs)
```

1. See [:material-code-braces: DescribeAlarmsInputTypeDef](./type_defs.md#describealarmsinputtypedef) 

### describe\_alarms\_for\_metric

Retrieves the alarms for the specified metric.

Type annotations and code completion for `#!python session.create_client("cloudwatch").describe_alarms_for_metric` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/describe_alarms_for_metric.html)

```python
# describe_alarms_for_metric method definition

await def describe_alarms_for_metric(
    self,
    *,
    MetricName: str,
    Namespace: str,
    Statistic: StatisticType = ...,  # (1)
    ExtendedStatistic: str = ...,
    Dimensions: Sequence[DimensionTypeDef] = ...,  # (2)
    Period: int = ...,
    Unit: StandardUnitType = ...,  # (3)
) -> DescribeAlarmsForMetricOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
2. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
3. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
4. See [:material-code-braces: DescribeAlarmsForMetricOutputTypeDef](./type_defs.md#describealarmsformetricoutputtypedef) 


```python
# describe_alarms_for_metric method usage example with argument unpacking

kwargs: DescribeAlarmsForMetricInputTypeDef = {  # (1)
    "MetricName": ...,
    "Namespace": ...,
}

parent.describe_alarms_for_metric(**kwargs)
```

1. See [:material-code-braces: DescribeAlarmsForMetricInputTypeDef](./type_defs.md#describealarmsformetricinputtypedef) 

### describe\_anomaly\_detectors

Lists the anomaly detection models that you have created in your account.

Type annotations and code completion for `#!python session.create_client("cloudwatch").describe_anomaly_detectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/describe_anomaly_detectors.html)

```python
# describe_anomaly_detectors method definition

await def describe_anomaly_detectors(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Namespace: str = ...,
    MetricName: str = ...,
    Dimensions: Sequence[DimensionTypeDef] = ...,  # (1)
    AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,  # (2)
) -> DescribeAnomalyDetectorsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-brackets: AnomalyDetectorTypeType](./literals.md#anomalydetectortypetype) 
3. See [:material-code-braces: DescribeAnomalyDetectorsOutputTypeDef](./type_defs.md#describeanomalydetectorsoutputtypedef) 


```python
# describe_anomaly_detectors method usage example with argument unpacking

kwargs: DescribeAnomalyDetectorsInputTypeDef = {  # (1)
    "NextToken": ...,
}

parent.describe_anomaly_detectors(**kwargs)
```

1. See [:material-code-braces: DescribeAnomalyDetectorsInputTypeDef](./type_defs.md#describeanomalydetectorsinputtypedef) 

### describe\_insight\_rules

Returns a list of all the Contributor Insights rules in your account.

Type annotations and code completion for `#!python session.create_client("cloudwatch").describe_insight_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/describe_insight_rules.html)

```python
# describe_insight_rules method definition

await def describe_insight_rules(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeInsightRulesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInsightRulesOutputTypeDef](./type_defs.md#describeinsightrulesoutputtypedef) 


```python
# describe_insight_rules method usage example with argument unpacking

kwargs: DescribeInsightRulesInputTypeDef = {  # (1)
    "NextToken": ...,
}

parent.describe_insight_rules(**kwargs)
```

1. See [:material-code-braces: DescribeInsightRulesInputTypeDef](./type_defs.md#describeinsightrulesinputtypedef) 

### disable\_alarm\_actions

Disables the actions for the specified alarms.

Type annotations and code completion for `#!python session.create_client("cloudwatch").disable_alarm_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/disable_alarm_actions.html)

```python
# disable_alarm_actions method definition

await def disable_alarm_actions(
    self,
    *,
    AlarmNames: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disable_alarm_actions method usage example with argument unpacking

kwargs: DisableAlarmActionsInputTypeDef = {  # (1)
    "AlarmNames": ...,
}

parent.disable_alarm_actions(**kwargs)
```

1. See [:material-code-braces: DisableAlarmActionsInputTypeDef](./type_defs.md#disablealarmactionsinputtypedef) 

### disable\_insight\_rules

Disables the specified Contributor Insights rules.

Type annotations and code completion for `#!python session.create_client("cloudwatch").disable_insight_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/disable_insight_rules.html)

```python
# disable_insight_rules method definition

await def disable_insight_rules(
    self,
    *,
    RuleNames: Sequence[str],
) -> DisableInsightRulesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisableInsightRulesOutputTypeDef](./type_defs.md#disableinsightrulesoutputtypedef) 


```python
# disable_insight_rules method usage example with argument unpacking

kwargs: DisableInsightRulesInputTypeDef = {  # (1)
    "RuleNames": ...,
}

parent.disable_insight_rules(**kwargs)
```

1. See [:material-code-braces: DisableInsightRulesInputTypeDef](./type_defs.md#disableinsightrulesinputtypedef) 

### enable\_alarm\_actions

Enables the actions for the specified alarms.

Type annotations and code completion for `#!python session.create_client("cloudwatch").enable_alarm_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/enable_alarm_actions.html)

```python
# enable_alarm_actions method definition

await def enable_alarm_actions(
    self,
    *,
    AlarmNames: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# enable_alarm_actions method usage example with argument unpacking

kwargs: EnableAlarmActionsInputTypeDef = {  # (1)
    "AlarmNames": ...,
}

parent.enable_alarm_actions(**kwargs)
```

1. See [:material-code-braces: EnableAlarmActionsInputTypeDef](./type_defs.md#enablealarmactionsinputtypedef) 

### enable\_insight\_rules

Enables the specified Contributor Insights rules.

Type annotations and code completion for `#!python session.create_client("cloudwatch").enable_insight_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/enable_insight_rules.html)

```python
# enable_insight_rules method definition

await def enable_insight_rules(
    self,
    *,
    RuleNames: Sequence[str],
) -> EnableInsightRulesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EnableInsightRulesOutputTypeDef](./type_defs.md#enableinsightrulesoutputtypedef) 


```python
# enable_insight_rules method usage example with argument unpacking

kwargs: EnableInsightRulesInputTypeDef = {  # (1)
    "RuleNames": ...,
}

parent.enable_insight_rules(**kwargs)
```

1. See [:material-code-braces: EnableInsightRulesInputTypeDef](./type_defs.md#enableinsightrulesinputtypedef) 

### get\_dashboard

Displays the details of the dashboard that you specify.

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/get_dashboard.html)

```python
# get_dashboard method definition

await def get_dashboard(
    self,
    *,
    DashboardName: str,
) -> GetDashboardOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDashboardOutputTypeDef](./type_defs.md#getdashboardoutputtypedef) 


```python
# get_dashboard method usage example with argument unpacking

kwargs: GetDashboardInputTypeDef = {  # (1)
    "DashboardName": ...,
}

parent.get_dashboard(**kwargs)
```

1. See [:material-code-braces: GetDashboardInputTypeDef](./type_defs.md#getdashboardinputtypedef) 

### get\_insight\_rule\_report

This operation returns the time series data collected by a Contributor Insights
rule.

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_insight_rule_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/get_insight_rule_report.html)

```python
# get_insight_rule_report method definition

await def get_insight_rule_report(
    self,
    *,
    RuleName: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Period: int,
    MaxContributorCount: int = ...,
    Metrics: Sequence[str] = ...,
    OrderBy: str = ...,
) -> GetInsightRuleReportOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInsightRuleReportOutputTypeDef](./type_defs.md#getinsightrulereportoutputtypedef) 


```python
# get_insight_rule_report method usage example with argument unpacking

kwargs: GetInsightRuleReportInputTypeDef = {  # (1)
    "RuleName": ...,
    "StartTime": ...,
    "EndTime": ...,
    "Period": ...,
}

parent.get_insight_rule_report(**kwargs)
```

1. See [:material-code-braces: GetInsightRuleReportInputTypeDef](./type_defs.md#getinsightrulereportinputtypedef) 

### get\_metric\_data

You can use the <code>GetMetricData</code> API to retrieve CloudWatch metric
values.

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_metric_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/get_metric_data.html)

```python
# get_metric_data method definition

await def get_metric_data(
    self,
    *,
    MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],  # (1)
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    NextToken: str = ...,
    ScanBy: ScanByType = ...,  # (2)
    MaxDatapoints: int = ...,
    LabelOptions: LabelOptionsTypeDef = ...,  # (3)
) -> GetMetricDataOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
2. See [:material-code-brackets: ScanByType](./literals.md#scanbytype) 
3. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
4. See [:material-code-braces: GetMetricDataOutputTypeDef](./type_defs.md#getmetricdataoutputtypedef) 


```python
# get_metric_data method usage example with argument unpacking

kwargs: GetMetricDataInputTypeDef = {  # (1)
    "MetricDataQueries": ...,
    "StartTime": ...,
    "EndTime": ...,
}

parent.get_metric_data(**kwargs)
```

1. See [:material-code-braces: GetMetricDataInputTypeDef](./type_defs.md#getmetricdatainputtypedef) 

### get\_metric\_statistics

Gets statistics for the specified metric.

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_metric_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/get_metric_statistics.html)

```python
# get_metric_statistics method definition

await def get_metric_statistics(
    self,
    *,
    Namespace: str,
    MetricName: str,
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
# get_metric_statistics method usage example with argument unpacking

kwargs: GetMetricStatisticsInputTypeDef = {  # (1)
    "Namespace": ...,
    "MetricName": ...,
    "StartTime": ...,
    "EndTime": ...,
    "Period": ...,
}

parent.get_metric_statistics(**kwargs)
```

1. See [:material-code-braces: GetMetricStatisticsInputTypeDef](./type_defs.md#getmetricstatisticsinputtypedef) 

### get\_metric\_stream

Returns information about the metric stream that you specify.

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_metric_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/get_metric_stream.html)

```python
# get_metric_stream method definition

await def get_metric_stream(
    self,
    *,
    Name: str,
) -> GetMetricStreamOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMetricStreamOutputTypeDef](./type_defs.md#getmetricstreamoutputtypedef) 


```python
# get_metric_stream method usage example with argument unpacking

kwargs: GetMetricStreamInputTypeDef = {  # (1)
    "Name": ...,
}

parent.get_metric_stream(**kwargs)
```

1. See [:material-code-braces: GetMetricStreamInputTypeDef](./type_defs.md#getmetricstreaminputtypedef) 

### get\_metric\_widget\_image

You can use the <code>GetMetricWidgetImage</code> API to retrieve a snapshot
graph of one or more Amazon CloudWatch metrics as a bitmap image.

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_metric_widget_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/get_metric_widget_image.html)

```python
# get_metric_widget_image method definition

await def get_metric_widget_image(
    self,
    *,
    MetricWidget: str,
    OutputFormat: str = ...,
) -> GetMetricWidgetImageOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMetricWidgetImageOutputTypeDef](./type_defs.md#getmetricwidgetimageoutputtypedef) 


```python
# get_metric_widget_image method usage example with argument unpacking

kwargs: GetMetricWidgetImageInputTypeDef = {  # (1)
    "MetricWidget": ...,
}

parent.get_metric_widget_image(**kwargs)
```

1. See [:material-code-braces: GetMetricWidgetImageInputTypeDef](./type_defs.md#getmetricwidgetimageinputtypedef) 

### list\_dashboards

Returns a list of the dashboards for your account.

Type annotations and code completion for `#!python session.create_client("cloudwatch").list_dashboards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/list_dashboards.html)

```python
# list_dashboards method definition

await def list_dashboards(
    self,
    *,
    DashboardNamePrefix: str = ...,
    NextToken: str = ...,
) -> ListDashboardsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDashboardsOutputTypeDef](./type_defs.md#listdashboardsoutputtypedef) 


```python
# list_dashboards method usage example with argument unpacking

kwargs: ListDashboardsInputTypeDef = {  # (1)
    "DashboardNamePrefix": ...,
}

parent.list_dashboards(**kwargs)
```

1. See [:material-code-braces: ListDashboardsInputTypeDef](./type_defs.md#listdashboardsinputtypedef) 

### list\_managed\_insight\_rules

Returns a list that contains the number of managed Contributor Insights rules
in your account.

Type annotations and code completion for `#!python session.create_client("cloudwatch").list_managed_insight_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/list_managed_insight_rules.html)

```python
# list_managed_insight_rules method definition

await def list_managed_insight_rules(
    self,
    *,
    ResourceARN: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListManagedInsightRulesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListManagedInsightRulesOutputTypeDef](./type_defs.md#listmanagedinsightrulesoutputtypedef) 


```python
# list_managed_insight_rules method usage example with argument unpacking

kwargs: ListManagedInsightRulesInputTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_managed_insight_rules(**kwargs)
```

1. See [:material-code-braces: ListManagedInsightRulesInputTypeDef](./type_defs.md#listmanagedinsightrulesinputtypedef) 

### list\_metric\_streams

Returns a list of metric streams in this account.

Type annotations and code completion for `#!python session.create_client("cloudwatch").list_metric_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/list_metric_streams.html)

```python
# list_metric_streams method definition

await def list_metric_streams(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMetricStreamsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMetricStreamsOutputTypeDef](./type_defs.md#listmetricstreamsoutputtypedef) 


```python
# list_metric_streams method usage example with argument unpacking

kwargs: ListMetricStreamsInputTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_metric_streams(**kwargs)
```

1. See [:material-code-braces: ListMetricStreamsInputTypeDef](./type_defs.md#listmetricstreamsinputtypedef) 

### list\_metrics

List the specified metrics.

Type annotations and code completion for `#!python session.create_client("cloudwatch").list_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/list_metrics.html)

```python
# list_metrics method definition

await def list_metrics(
    self,
    *,
    Namespace: str = ...,
    MetricName: str = ...,
    Dimensions: Sequence[DimensionFilterTypeDef] = ...,  # (1)
    NextToken: str = ...,
    RecentlyActive: RecentlyActiveType = ...,  # (2)
    IncludeLinkedAccounts: bool = ...,
    OwningAccount: str = ...,
) -> ListMetricsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DimensionFilterTypeDef](./type_defs.md#dimensionfiltertypedef) 
2. See [:material-code-brackets: RecentlyActiveType](./literals.md#recentlyactivetype) 
3. See [:material-code-braces: ListMetricsOutputTypeDef](./type_defs.md#listmetricsoutputtypedef) 


```python
# list_metrics method usage example with argument unpacking

kwargs: ListMetricsInputTypeDef = {  # (1)
    "Namespace": ...,
}

parent.list_metrics(**kwargs)
```

1. See [:material-code-braces: ListMetricsInputTypeDef](./type_defs.md#listmetricsinputtypedef) 

### list\_tags\_for\_resource

Displays the tags associated with a CloudWatch resource.

Type annotations and code completion for `#!python session.create_client("cloudwatch").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef) 

### put\_anomaly\_detector

Creates an anomaly detection model for a CloudWatch metric.

Type annotations and code completion for `#!python session.create_client("cloudwatch").put_anomaly_detector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/put_anomaly_detector.html)

```python
# put_anomaly_detector method definition

await def put_anomaly_detector(
    self,
    *,
    Namespace: str = ...,
    MetricName: str = ...,
    Dimensions: Sequence[DimensionTypeDef] = ...,  # (1)
    Stat: str = ...,
    Configuration: AnomalyDetectorConfigurationUnionTypeDef = ...,  # (2)
    MetricCharacteristics: MetricCharacteristicsTypeDef = ...,  # (3)
    SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,  # (4)
    MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...,  # (5)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-braces: AnomalyDetectorConfigurationTypeDef](./type_defs.md#anomalydetectorconfigurationtypedef) [:material-code-braces: AnomalyDetectorConfigurationOutputTypeDef](./type_defs.md#anomalydetectorconfigurationoutputtypedef) 
3. See [:material-code-braces: MetricCharacteristicsTypeDef](./type_defs.md#metriccharacteristicstypedef) 
4. See [:material-code-braces: SingleMetricAnomalyDetectorTypeDef](./type_defs.md#singlemetricanomalydetectortypedef) [:material-code-braces: SingleMetricAnomalyDetectorOutputTypeDef](./type_defs.md#singlemetricanomalydetectoroutputtypedef) 
5. See [:material-code-braces: MetricMathAnomalyDetectorTypeDef](./type_defs.md#metricmathanomalydetectortypedef) [:material-code-braces: MetricMathAnomalyDetectorOutputTypeDef](./type_defs.md#metricmathanomalydetectoroutputtypedef) 


```python
# put_anomaly_detector method usage example with argument unpacking

kwargs: PutAnomalyDetectorInputTypeDef = {  # (1)
    "Namespace": ...,
}

parent.put_anomaly_detector(**kwargs)
```

1. See [:material-code-braces: PutAnomalyDetectorInputTypeDef](./type_defs.md#putanomalydetectorinputtypedef) 

### put\_composite\_alarm

Creates or updates a <i>composite alarm</i>.

Type annotations and code completion for `#!python session.create_client("cloudwatch").put_composite_alarm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/put_composite_alarm.html)

```python
# put_composite_alarm method definition

await def put_composite_alarm(
    self,
    *,
    AlarmName: str,
    AlarmRule: str,
    ActionsEnabled: bool = ...,
    AlarmActions: Sequence[str] = ...,
    AlarmDescription: str = ...,
    InsufficientDataActions: Sequence[str] = ...,
    OKActions: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    ActionsSuppressor: str = ...,
    ActionsSuppressorWaitPeriod: int = ...,
    ActionsSuppressorExtensionPeriod: int = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_composite_alarm method usage example with argument unpacking

kwargs: PutCompositeAlarmInputTypeDef = {  # (1)
    "AlarmName": ...,
    "AlarmRule": ...,
}

parent.put_composite_alarm(**kwargs)
```

1. See [:material-code-braces: PutCompositeAlarmInputTypeDef](./type_defs.md#putcompositealarminputtypedef) 

### put\_dashboard

Creates a dashboard if it does not already exist, or updates an existing
dashboard.

Type annotations and code completion for `#!python session.create_client("cloudwatch").put_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/put_dashboard.html)

```python
# put_dashboard method definition

await def put_dashboard(
    self,
    *,
    DashboardName: str,
    DashboardBody: str,
) -> PutDashboardOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutDashboardOutputTypeDef](./type_defs.md#putdashboardoutputtypedef) 


```python
# put_dashboard method usage example with argument unpacking

kwargs: PutDashboardInputTypeDef = {  # (1)
    "DashboardName": ...,
    "DashboardBody": ...,
}

parent.put_dashboard(**kwargs)
```

1. See [:material-code-braces: PutDashboardInputTypeDef](./type_defs.md#putdashboardinputtypedef) 

### put\_insight\_rule

Creates a Contributor Insights rule.

Type annotations and code completion for `#!python session.create_client("cloudwatch").put_insight_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/put_insight_rule.html)

```python
# put_insight_rule method definition

await def put_insight_rule(
    self,
    *,
    RuleName: str,
    RuleDefinition: str,
    RuleState: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# put_insight_rule method usage example with argument unpacking

kwargs: PutInsightRuleInputTypeDef = {  # (1)
    "RuleName": ...,
    "RuleDefinition": ...,
}

parent.put_insight_rule(**kwargs)
```

1. See [:material-code-braces: PutInsightRuleInputTypeDef](./type_defs.md#putinsightruleinputtypedef) 

### put\_managed\_insight\_rules

Creates a managed Contributor Insights rule for a specified Amazon Web Services
resource.

Type annotations and code completion for `#!python session.create_client("cloudwatch").put_managed_insight_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/put_managed_insight_rules.html)

```python
# put_managed_insight_rules method definition

await def put_managed_insight_rules(
    self,
    *,
    ManagedRules: Sequence[ManagedRuleTypeDef],  # (1)
) -> PutManagedInsightRulesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ManagedRuleTypeDef](./type_defs.md#managedruletypedef) 
2. See [:material-code-braces: PutManagedInsightRulesOutputTypeDef](./type_defs.md#putmanagedinsightrulesoutputtypedef) 


```python
# put_managed_insight_rules method usage example with argument unpacking

kwargs: PutManagedInsightRulesInputTypeDef = {  # (1)
    "ManagedRules": ...,
}

parent.put_managed_insight_rules(**kwargs)
```

1. See [:material-code-braces: PutManagedInsightRulesInputTypeDef](./type_defs.md#putmanagedinsightrulesinputtypedef) 

### put\_metric\_alarm

Creates or updates an alarm and associates it with the specified metric, metric
math expression, anomaly detection model, or Metrics Insights query.

Type annotations and code completion for `#!python session.create_client("cloudwatch").put_metric_alarm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/put_metric_alarm.html)

```python
# put_metric_alarm method definition

await def put_metric_alarm(
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
    MetricName: str = ...,
    Namespace: str = ...,
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
) -> EmptyResponseMetadataTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
4. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
5. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_metric_alarm method usage example with argument unpacking

kwargs: PutMetricAlarmInputTypeDef = {  # (1)
    "AlarmName": ...,
    "EvaluationPeriods": ...,
    "ComparisonOperator": ...,
}

parent.put_metric_alarm(**kwargs)
```

1. See [:material-code-braces: PutMetricAlarmInputTypeDef](./type_defs.md#putmetricalarminputtypedef) 

### put\_metric\_data

Publishes metric data to Amazon CloudWatch.

Type annotations and code completion for `#!python session.create_client("cloudwatch").put_metric_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/put_metric_data.html)

```python
# put_metric_data method definition

await def put_metric_data(
    self,
    *,
    Namespace: str,
    MetricData: Sequence[MetricDatumTypeDef] = ...,  # (1)
    EntityMetricData: Sequence[EntityMetricDataTypeDef] = ...,  # (2)
    StrictEntityValidation: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MetricDatumTypeDef](./type_defs.md#metricdatumtypedef) 
2. See [:material-code-braces: EntityMetricDataTypeDef](./type_defs.md#entitymetricdatatypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_metric_data method usage example with argument unpacking

kwargs: PutMetricDataInputTypeDef = {  # (1)
    "Namespace": ...,
}

parent.put_metric_data(**kwargs)
```

1. See [:material-code-braces: PutMetricDataInputTypeDef](./type_defs.md#putmetricdatainputtypedef) 

### put\_metric\_stream

Creates or updates a metric stream.

Type annotations and code completion for `#!python session.create_client("cloudwatch").put_metric_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/put_metric_stream.html)

```python
# put_metric_stream method definition

await def put_metric_stream(
    self,
    *,
    Name: str,
    FirehoseArn: str,
    RoleArn: str,
    OutputFormat: MetricStreamOutputFormatType,  # (1)
    IncludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,  # (2)
    ExcludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationUnionTypeDef] = ...,  # (5)
    IncludeLinkedAccountsMetrics: bool = ...,
) -> PutMetricStreamOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: MetricStreamOutputFormatType](./literals.md#metricstreamoutputformattype) 
2. See [:material-code-braces: MetricStreamFilterTypeDef](./type_defs.md#metricstreamfiltertypedef) [:material-code-braces: MetricStreamFilterOutputTypeDef](./type_defs.md#metricstreamfilteroutputtypedef) 
3. See [:material-code-braces: MetricStreamFilterTypeDef](./type_defs.md#metricstreamfiltertypedef) [:material-code-braces: MetricStreamFilterOutputTypeDef](./type_defs.md#metricstreamfilteroutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: MetricStreamStatisticsConfigurationTypeDef](./type_defs.md#metricstreamstatisticsconfigurationtypedef) [:material-code-braces: MetricStreamStatisticsConfigurationOutputTypeDef](./type_defs.md#metricstreamstatisticsconfigurationoutputtypedef) 
6. See [:material-code-braces: PutMetricStreamOutputTypeDef](./type_defs.md#putmetricstreamoutputtypedef) 


```python
# put_metric_stream method usage example with argument unpacking

kwargs: PutMetricStreamInputTypeDef = {  # (1)
    "Name": ...,
    "FirehoseArn": ...,
    "RoleArn": ...,
    "OutputFormat": ...,
}

parent.put_metric_stream(**kwargs)
```

1. See [:material-code-braces: PutMetricStreamInputTypeDef](./type_defs.md#putmetricstreaminputtypedef) 

### set\_alarm\_state

Temporarily sets the state of an alarm for testing purposes.

Type annotations and code completion for `#!python session.create_client("cloudwatch").set_alarm_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/set_alarm_state.html)

```python
# set_alarm_state method definition

await def set_alarm_state(
    self,
    *,
    AlarmName: str,
    StateValue: StateValueType,  # (1)
    StateReason: str,
    StateReasonData: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_alarm_state method usage example with argument unpacking

kwargs: SetAlarmStateInputTypeDef = {  # (1)
    "AlarmName": ...,
    "StateValue": ...,
    "StateReason": ...,
}

parent.set_alarm_state(**kwargs)
```

1. See [:material-code-braces: SetAlarmStateInputTypeDef](./type_defs.md#setalarmstateinputtypedef) 

### start\_metric\_streams

Starts the streaming of metrics for one or more of your metric streams.

Type annotations and code completion for `#!python session.create_client("cloudwatch").start_metric_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/start_metric_streams.html)

```python
# start_metric_streams method definition

await def start_metric_streams(
    self,
    *,
    Names: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# start_metric_streams method usage example with argument unpacking

kwargs: StartMetricStreamsInputTypeDef = {  # (1)
    "Names": ...,
}

parent.start_metric_streams(**kwargs)
```

1. See [:material-code-braces: StartMetricStreamsInputTypeDef](./type_defs.md#startmetricstreamsinputtypedef) 

### stop\_metric\_streams

Stops the streaming of metrics for one or more of your metric streams.

Type annotations and code completion for `#!python session.create_client("cloudwatch").stop_metric_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/stop_metric_streams.html)

```python
# stop_metric_streams method definition

await def stop_metric_streams(
    self,
    *,
    Names: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# stop_metric_streams method usage example with argument unpacking

kwargs: StopMetricStreamsInputTypeDef = {  # (1)
    "Names": ...,
}

parent.stop_metric_streams(**kwargs)
```

1. See [:material-code-braces: StopMetricStreamsInputTypeDef](./type_defs.md#stopmetricstreamsinputtypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified CloudWatch resource.

Type annotations and code completion for `#!python session.create_client("cloudwatch").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef) 

### untag\_resource

Removes one or more tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("cloudwatch").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cloudwatch").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cloudwatch").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_paginator` method with overloads.

- `client.get_paginator("describe_alarm_history")` -> [DescribeAlarmHistoryPaginator](./paginators.md#describealarmhistorypaginator)
- `client.get_paginator("describe_alarms")` -> [DescribeAlarmsPaginator](./paginators.md#describealarmspaginator)
- `client.get_paginator("describe_anomaly_detectors")` -> [DescribeAnomalyDetectorsPaginator](./paginators.md#describeanomalydetectorspaginator)
- `client.get_paginator("get_metric_data")` -> [GetMetricDataPaginator](./paginators.md#getmetricdatapaginator)
- `client.get_paginator("list_dashboards")` -> [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
- `client.get_paginator("list_metrics")` -> [ListMetricsPaginator](./paginators.md#listmetricspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_waiter` method with overloads.

- `client.get_waiter("alarm_exists")` -> [AlarmExistsWaiter](./waiters.md#alarmexistswaiter)
- `client.get_waiter("composite_alarm_exists")` -> [CompositeAlarmExistsWaiter](./waiters.md#compositealarmexistswaiter)

