# Type definitions

> [Index](../README.md) > [CloudWatch](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
    type annotations stubs module [types-aiobotocore-cloudwatch](https://pypi.org/project/types-aiobotocore-cloudwatch/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AlarmHistoryItemTypeDef

```python
# AlarmHistoryItemTypeDef definition

class AlarmHistoryItemTypeDef(TypedDict):
    AlarmName: NotRequired[str],
    AlarmType: NotRequired[AlarmTypeType],  # (1)
    Timestamp: NotRequired[datetime],
    HistoryItemType: NotRequired[HistoryItemTypeType],  # (2)
    HistorySummary: NotRequired[str],
    HistoryData: NotRequired[str],
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: HistoryItemTypeType](./literals.md#historyitemtypetype) 
## RangeTypeDef

```python
# RangeTypeDef definition

class RangeTypeDef(TypedDict):
    StartTime: datetime,
    EndTime: datetime,
```

## DimensionTypeDef

```python
# DimensionTypeDef definition

class DimensionTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## CompositeAlarmTypeDef

```python
# CompositeAlarmTypeDef definition

class CompositeAlarmTypeDef(TypedDict):
    ActionsEnabled: NotRequired[bool],
    AlarmActions: NotRequired[List[str]],
    AlarmArn: NotRequired[str],
    AlarmConfigurationUpdatedTimestamp: NotRequired[datetime],
    AlarmDescription: NotRequired[str],
    AlarmName: NotRequired[str],
    AlarmRule: NotRequired[str],
    InsufficientDataActions: NotRequired[List[str]],
    OKActions: NotRequired[List[str]],
    StateReason: NotRequired[str],
    StateReasonData: NotRequired[str],
    StateUpdatedTimestamp: NotRequired[datetime],
    StateValue: NotRequired[StateValueType],  # (1)
    StateTransitionedTimestamp: NotRequired[datetime],
    ActionsSuppressedBy: NotRequired[ActionsSuppressedByType],  # (2)
    ActionsSuppressedReason: NotRequired[str],
    ActionsSuppressor: NotRequired[str],
    ActionsSuppressorWaitPeriod: NotRequired[int],
    ActionsSuppressorExtensionPeriod: NotRequired[int],
```

1. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
2. See [:material-code-brackets: ActionsSuppressedByType](./literals.md#actionssuppressedbytype) 
## DashboardEntryTypeDef

```python
# DashboardEntryTypeDef definition

class DashboardEntryTypeDef(TypedDict):
    DashboardName: NotRequired[str],
    DashboardArn: NotRequired[str],
    LastModified: NotRequired[datetime],
    Size: NotRequired[int],
```

## DashboardValidationMessageTypeDef

```python
# DashboardValidationMessageTypeDef definition

class DashboardValidationMessageTypeDef(TypedDict):
    DataPath: NotRequired[str],
    Message: NotRequired[str],
```

## DatapointTypeDef

```python
# DatapointTypeDef definition

class DatapointTypeDef(TypedDict):
    Timestamp: NotRequired[datetime],
    SampleCount: NotRequired[float],
    Average: NotRequired[float],
    Sum: NotRequired[float],
    Minimum: NotRequired[float],
    Maximum: NotRequired[float],
    Unit: NotRequired[StandardUnitType],  # (1)
    ExtendedStatistics: NotRequired[Dict[str, float]],
```

1. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
## DeleteAlarmsInputRequestTypeDef

```python
# DeleteAlarmsInputRequestTypeDef definition

class DeleteAlarmsInputRequestTypeDef(TypedDict):
    AlarmNames: Sequence[str],
```

## DeleteDashboardsInputRequestTypeDef

```python
# DeleteDashboardsInputRequestTypeDef definition

class DeleteDashboardsInputRequestTypeDef(TypedDict):
    DashboardNames: Sequence[str],
```

## DeleteInsightRulesInputRequestTypeDef

```python
# DeleteInsightRulesInputRequestTypeDef definition

class DeleteInsightRulesInputRequestTypeDef(TypedDict):
    RuleNames: Sequence[str],
```

## PartialFailureTypeDef

```python
# PartialFailureTypeDef definition

class PartialFailureTypeDef(TypedDict):
    FailureResource: NotRequired[str],
    ExceptionType: NotRequired[str],
    FailureCode: NotRequired[str],
    FailureDescription: NotRequired[str],
```

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

## DeleteMetricStreamInputRequestTypeDef

```python
# DeleteMetricStreamInputRequestTypeDef definition

class DeleteMetricStreamInputRequestTypeDef(TypedDict):
    Name: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeAlarmsInputRequestTypeDef

```python
# DescribeAlarmsInputRequestTypeDef definition

class DescribeAlarmsInputRequestTypeDef(TypedDict):
    AlarmNames: NotRequired[Sequence[str]],
    AlarmNamePrefix: NotRequired[str],
    AlarmTypes: NotRequired[Sequence[AlarmTypeType]],  # (1)
    ChildrenOfAlarmName: NotRequired[str],
    ParentsOfAlarmName: NotRequired[str],
    StateValue: NotRequired[StateValueType],  # (2)
    ActionPrefix: NotRequired[str],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
## DescribeInsightRulesInputRequestTypeDef

```python
# DescribeInsightRulesInputRequestTypeDef definition

class DescribeInsightRulesInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## InsightRuleTypeDef

```python
# InsightRuleTypeDef definition

class InsightRuleTypeDef(TypedDict):
    Name: str,
    State: str,
    Schema: str,
    Definition: str,
    ManagedRule: NotRequired[bool],
```

## DimensionFilterTypeDef

```python
# DimensionFilterTypeDef definition

class DimensionFilterTypeDef(TypedDict):
    Name: str,
    Value: NotRequired[str],
```

## DisableAlarmActionsInputRequestTypeDef

```python
# DisableAlarmActionsInputRequestTypeDef definition

class DisableAlarmActionsInputRequestTypeDef(TypedDict):
    AlarmNames: Sequence[str],
```

## DisableInsightRulesInputRequestTypeDef

```python
# DisableInsightRulesInputRequestTypeDef definition

class DisableInsightRulesInputRequestTypeDef(TypedDict):
    RuleNames: Sequence[str],
```

## EnableAlarmActionsInputRequestTypeDef

```python
# EnableAlarmActionsInputRequestTypeDef definition

class EnableAlarmActionsInputRequestTypeDef(TypedDict):
    AlarmNames: Sequence[str],
```

## EnableInsightRulesInputRequestTypeDef

```python
# EnableInsightRulesInputRequestTypeDef definition

class EnableInsightRulesInputRequestTypeDef(TypedDict):
    RuleNames: Sequence[str],
```

## GetDashboardInputRequestTypeDef

```python
# GetDashboardInputRequestTypeDef definition

class GetDashboardInputRequestTypeDef(TypedDict):
    DashboardName: str,
```

## InsightRuleMetricDatapointTypeDef

```python
# InsightRuleMetricDatapointTypeDef definition

class InsightRuleMetricDatapointTypeDef(TypedDict):
    Timestamp: datetime,
    UniqueContributors: NotRequired[float],
    MaxContributorValue: NotRequired[float],
    SampleCount: NotRequired[float],
    Average: NotRequired[float],
    Sum: NotRequired[float],
    Minimum: NotRequired[float],
    Maximum: NotRequired[float],
```

## LabelOptionsTypeDef

```python
# LabelOptionsTypeDef definition

class LabelOptionsTypeDef(TypedDict):
    Timezone: NotRequired[str],
```

## MessageDataTypeDef

```python
# MessageDataTypeDef definition

class MessageDataTypeDef(TypedDict):
    Code: NotRequired[str],
    Value: NotRequired[str],
```

## GetMetricStreamInputRequestTypeDef

```python
# GetMetricStreamInputRequestTypeDef definition

class GetMetricStreamInputRequestTypeDef(TypedDict):
    Name: str,
```

## MetricStreamFilterTypeDef

```python
# MetricStreamFilterTypeDef definition

class MetricStreamFilterTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricNames: NotRequired[List[str]],
```

## GetMetricWidgetImageInputRequestTypeDef

```python
# GetMetricWidgetImageInputRequestTypeDef definition

class GetMetricWidgetImageInputRequestTypeDef(TypedDict):
    MetricWidget: str,
    OutputFormat: NotRequired[str],
```

## InsightRuleContributorDatapointTypeDef

```python
# InsightRuleContributorDatapointTypeDef definition

class InsightRuleContributorDatapointTypeDef(TypedDict):
    Timestamp: datetime,
    ApproximateValue: float,
```

## ListDashboardsInputRequestTypeDef

```python
# ListDashboardsInputRequestTypeDef definition

class ListDashboardsInputRequestTypeDef(TypedDict):
    DashboardNamePrefix: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListManagedInsightRulesInputRequestTypeDef

```python
# ListManagedInsightRulesInputRequestTypeDef definition

class ListManagedInsightRulesInputRequestTypeDef(TypedDict):
    ResourceARN: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListMetricStreamsInputRequestTypeDef

```python
# ListMetricStreamsInputRequestTypeDef definition

class ListMetricStreamsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MetricStreamEntryTypeDef

```python
# MetricStreamEntryTypeDef definition

class MetricStreamEntryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreationDate: NotRequired[datetime],
    LastUpdateDate: NotRequired[datetime],
    Name: NotRequired[str],
    FirehoseArn: NotRequired[str],
    State: NotRequired[str],
    OutputFormat: NotRequired[MetricStreamOutputFormatType],  # (1)
```

1. See [:material-code-brackets: MetricStreamOutputFormatType](./literals.md#metricstreamoutputformattype) 
## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## ManagedRuleStateTypeDef

```python
# ManagedRuleStateTypeDef definition

class ManagedRuleStateTypeDef(TypedDict):
    RuleName: str,
    State: str,
```

## StatisticSetTypeDef

```python
# StatisticSetTypeDef definition

class StatisticSetTypeDef(TypedDict):
    SampleCount: float,
    Sum: float,
    Minimum: float,
    Maximum: float,
```

## MetricStreamStatisticsMetricTypeDef

```python
# MetricStreamStatisticsMetricTypeDef definition

class MetricStreamStatisticsMetricTypeDef(TypedDict):
    Namespace: str,
    MetricName: str,
```

## PutDashboardInputRequestTypeDef

```python
# PutDashboardInputRequestTypeDef definition

class PutDashboardInputRequestTypeDef(TypedDict):
    DashboardName: str,
    DashboardBody: str,
```

## SetAlarmStateInputAlarmSetStateTypeDef

```python
# SetAlarmStateInputAlarmSetStateTypeDef definition

class SetAlarmStateInputAlarmSetStateTypeDef(TypedDict):
    StateValue: StateValueType,  # (1)
    StateReason: str,
    StateReasonData: NotRequired[str],
```

1. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
## SetAlarmStateInputRequestTypeDef

```python
# SetAlarmStateInputRequestTypeDef definition

class SetAlarmStateInputRequestTypeDef(TypedDict):
    AlarmName: str,
    StateValue: StateValueType,  # (1)
    StateReason: str,
    StateReasonData: NotRequired[str],
```

1. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
## StartMetricStreamsInputRequestTypeDef

```python
# StartMetricStreamsInputRequestTypeDef definition

class StartMetricStreamsInputRequestTypeDef(TypedDict):
    Names: Sequence[str],
```

## StopMetricStreamsInputRequestTypeDef

```python
# StopMetricStreamsInputRequestTypeDef definition

class StopMetricStreamsInputRequestTypeDef(TypedDict):
    Names: Sequence[str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## AnomalyDetectorConfigurationTypeDef

```python
# AnomalyDetectorConfigurationTypeDef definition

class AnomalyDetectorConfigurationTypeDef(TypedDict):
    ExcludedTimeRanges: NotRequired[List[RangeTypeDef]],  # (1)
    MetricTimezone: NotRequired[str],
```

1. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
## DescribeAlarmsForMetricInputRequestTypeDef

```python
# DescribeAlarmsForMetricInputRequestTypeDef definition

class DescribeAlarmsForMetricInputRequestTypeDef(TypedDict):
    MetricName: str,
    Namespace: str,
    Statistic: NotRequired[StatisticType],  # (1)
    ExtendedStatistic: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (2)
    Period: NotRequired[int],
    Unit: NotRequired[StandardUnitType],  # (3)
```

1. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
2. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
3. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
## DescribeAnomalyDetectorsInputRequestTypeDef

```python
# DescribeAnomalyDetectorsInputRequestTypeDef definition

class DescribeAnomalyDetectorsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
    AnomalyDetectorTypes: NotRequired[Sequence[AnomalyDetectorTypeType]],  # (2)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-brackets: AnomalyDetectorTypeType](./literals.md#anomalydetectortypetype) 
## MetricTypeDef

```python
# MetricTypeDef definition

class MetricTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## SingleMetricAnomalyDetectorMetricTypeDef

```python
# SingleMetricAnomalyDetectorMetricTypeDef definition

class SingleMetricAnomalyDetectorMetricTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[List[DimensionTypeDef]],  # (1)
    Stat: NotRequired[str],
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## SingleMetricAnomalyDetectorTypeDef

```python
# SingleMetricAnomalyDetectorTypeDef definition

class SingleMetricAnomalyDetectorTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
    Stat: NotRequired[str],
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## DeleteInsightRulesOutputTypeDef

```python
# DeleteInsightRulesOutputTypeDef definition

class DeleteInsightRulesOutputTypeDef(TypedDict):
    Failures: List[PartialFailureTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartialFailureTypeDef](./type_defs.md#partialfailuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAlarmHistoryOutputTypeDef

```python
# DescribeAlarmHistoryOutputTypeDef definition

class DescribeAlarmHistoryOutputTypeDef(TypedDict):
    AlarmHistoryItems: List[AlarmHistoryItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlarmHistoryItemTypeDef](./type_defs.md#alarmhistoryitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableInsightRulesOutputTypeDef

```python
# DisableInsightRulesOutputTypeDef definition

class DisableInsightRulesOutputTypeDef(TypedDict):
    Failures: List[PartialFailureTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartialFailureTypeDef](./type_defs.md#partialfailuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableInsightRulesOutputTypeDef

```python
# EnableInsightRulesOutputTypeDef definition

class EnableInsightRulesOutputTypeDef(TypedDict):
    Failures: List[PartialFailureTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartialFailureTypeDef](./type_defs.md#partialfailuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDashboardOutputTypeDef

```python
# GetDashboardOutputTypeDef definition

class GetDashboardOutputTypeDef(TypedDict):
    DashboardArn: str,
    DashboardBody: str,
    DashboardName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMetricStatisticsOutputTypeDef

```python
# GetMetricStatisticsOutputTypeDef definition

class GetMetricStatisticsOutputTypeDef(TypedDict):
    Label: str,
    Datapoints: List[DatapointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatapointTypeDef](./type_defs.md#datapointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMetricWidgetImageOutputTypeDef

```python
# GetMetricWidgetImageOutputTypeDef definition

class GetMetricWidgetImageOutputTypeDef(TypedDict):
    MetricWidgetImage: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDashboardsOutputTypeDef

```python
# ListDashboardsOutputTypeDef definition

class ListDashboardsOutputTypeDef(TypedDict):
    DashboardEntries: List[DashboardEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DashboardEntryTypeDef](./type_defs.md#dashboardentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDashboardOutputTypeDef

```python
# PutDashboardOutputTypeDef definition

class PutDashboardOutputTypeDef(TypedDict):
    DashboardValidationMessages: List[DashboardValidationMessageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DashboardValidationMessageTypeDef](./type_defs.md#dashboardvalidationmessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutManagedInsightRulesOutputTypeDef

```python
# PutManagedInsightRulesOutputTypeDef definition

class PutManagedInsightRulesOutputTypeDef(TypedDict):
    Failures: List[PartialFailureTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartialFailureTypeDef](./type_defs.md#partialfailuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutMetricStreamOutputTypeDef

```python
# PutMetricStreamOutputTypeDef definition

class PutMetricStreamOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef

```python
# DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef definition

class DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef(TypedDict):
    AlarmTypes: NotRequired[Sequence[AlarmTypeType]],  # (1)
    HistoryItemType: NotRequired[HistoryItemTypeType],  # (2)
    StartDate: NotRequired[Union[datetime, str]],
    EndDate: NotRequired[Union[datetime, str]],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
    ScanBy: NotRequired[ScanByType],  # (3)
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: HistoryItemTypeType](./literals.md#historyitemtypetype) 
3. See [:material-code-brackets: ScanByType](./literals.md#scanbytype) 
## DescribeAlarmHistoryInputRequestTypeDef

```python
# DescribeAlarmHistoryInputRequestTypeDef definition

class DescribeAlarmHistoryInputRequestTypeDef(TypedDict):
    AlarmName: NotRequired[str],
    AlarmTypes: NotRequired[Sequence[AlarmTypeType]],  # (1)
    HistoryItemType: NotRequired[HistoryItemTypeType],  # (2)
    StartDate: NotRequired[Union[datetime, str]],
    EndDate: NotRequired[Union[datetime, str]],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
    ScanBy: NotRequired[ScanByType],  # (3)
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: HistoryItemTypeType](./literals.md#historyitemtypetype) 
3. See [:material-code-brackets: ScanByType](./literals.md#scanbytype) 
## GetInsightRuleReportInputRequestTypeDef

```python
# GetInsightRuleReportInputRequestTypeDef definition

class GetInsightRuleReportInputRequestTypeDef(TypedDict):
    RuleName: str,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    Period: int,
    MaxContributorCount: NotRequired[int],
    Metrics: NotRequired[Sequence[str]],
    OrderBy: NotRequired[str],
```

## GetMetricStatisticsInputMetricGetStatisticsTypeDef

```python
# GetMetricStatisticsInputMetricGetStatisticsTypeDef definition

class GetMetricStatisticsInputMetricGetStatisticsTypeDef(TypedDict):
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    Period: int,
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
    Statistics: NotRequired[Sequence[StatisticType]],  # (2)
    ExtendedStatistics: NotRequired[Sequence[str]],
    Unit: NotRequired[StandardUnitType],  # (3)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
## GetMetricStatisticsInputRequestTypeDef

```python
# GetMetricStatisticsInputRequestTypeDef definition

class GetMetricStatisticsInputRequestTypeDef(TypedDict):
    Namespace: str,
    MetricName: str,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    Period: int,
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
    Statistics: NotRequired[Sequence[StatisticType]],  # (2)
    ExtendedStatistics: NotRequired[Sequence[str]],
    Unit: NotRequired[StandardUnitType],  # (3)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
## DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef

```python
# DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef definition

class DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef(TypedDict):
    AlarmName: NotRequired[str],
    AlarmTypes: NotRequired[Sequence[AlarmTypeType]],  # (1)
    HistoryItemType: NotRequired[HistoryItemTypeType],  # (2)
    StartDate: NotRequired[Union[datetime, str]],
    EndDate: NotRequired[Union[datetime, str]],
    ScanBy: NotRequired[ScanByType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: HistoryItemTypeType](./literals.md#historyitemtypetype) 
3. See [:material-code-brackets: ScanByType](./literals.md#scanbytype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAlarmsInputDescribeAlarmsPaginateTypeDef

```python
# DescribeAlarmsInputDescribeAlarmsPaginateTypeDef definition

class DescribeAlarmsInputDescribeAlarmsPaginateTypeDef(TypedDict):
    AlarmNames: NotRequired[Sequence[str]],
    AlarmNamePrefix: NotRequired[str],
    AlarmTypes: NotRequired[Sequence[AlarmTypeType]],  # (1)
    ChildrenOfAlarmName: NotRequired[str],
    ParentsOfAlarmName: NotRequired[str],
    StateValue: NotRequired[StateValueType],  # (2)
    ActionPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef

```python
# DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef definition

class DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
    AnomalyDetectorTypes: NotRequired[Sequence[AnomalyDetectorTypeType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-brackets: AnomalyDetectorTypeType](./literals.md#anomalydetectortypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDashboardsInputListDashboardsPaginateTypeDef

```python
# ListDashboardsInputListDashboardsPaginateTypeDef definition

class ListDashboardsInputListDashboardsPaginateTypeDef(TypedDict):
    DashboardNamePrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAlarmsInputAlarmExistsWaitTypeDef

```python
# DescribeAlarmsInputAlarmExistsWaitTypeDef definition

class DescribeAlarmsInputAlarmExistsWaitTypeDef(TypedDict):
    AlarmNames: NotRequired[Sequence[str]],
    AlarmNamePrefix: NotRequired[str],
    AlarmTypes: NotRequired[Sequence[AlarmTypeType]],  # (1)
    ChildrenOfAlarmName: NotRequired[str],
    ParentsOfAlarmName: NotRequired[str],
    StateValue: NotRequired[StateValueType],  # (2)
    ActionPrefix: NotRequired[str],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef

```python
# DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef definition

class DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef(TypedDict):
    AlarmNames: NotRequired[Sequence[str]],
    AlarmNamePrefix: NotRequired[str],
    AlarmTypes: NotRequired[Sequence[AlarmTypeType]],  # (1)
    ChildrenOfAlarmName: NotRequired[str],
    ParentsOfAlarmName: NotRequired[str],
    StateValue: NotRequired[StateValueType],  # (2)
    ActionPrefix: NotRequired[str],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInsightRulesOutputTypeDef

```python
# DescribeInsightRulesOutputTypeDef definition

class DescribeInsightRulesOutputTypeDef(TypedDict):
    NextToken: str,
    InsightRules: List[InsightRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InsightRuleTypeDef](./type_defs.md#insightruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMetricsInputListMetricsPaginateTypeDef

```python
# ListMetricsInputListMetricsPaginateTypeDef definition

class ListMetricsInputListMetricsPaginateTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionFilterTypeDef]],  # (1)
    RecentlyActive: NotRequired[RecentlyActiveType],  # (2)
    IncludeLinkedAccounts: NotRequired[bool],
    OwningAccount: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: DimensionFilterTypeDef](./type_defs.md#dimensionfiltertypedef) 
2. See [:material-code-brackets: RecentlyActiveType](./literals.md#recentlyactivetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMetricsInputRequestTypeDef

```python
# ListMetricsInputRequestTypeDef definition

class ListMetricsInputRequestTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    RecentlyActive: NotRequired[RecentlyActiveType],  # (2)
    IncludeLinkedAccounts: NotRequired[bool],
    OwningAccount: NotRequired[str],
```

1. See [:material-code-braces: DimensionFilterTypeDef](./type_defs.md#dimensionfiltertypedef) 
2. See [:material-code-brackets: RecentlyActiveType](./literals.md#recentlyactivetype) 
## MetricDataResultTypeDef

```python
# MetricDataResultTypeDef definition

class MetricDataResultTypeDef(TypedDict):
    Id: NotRequired[str],
    Label: NotRequired[str],
    Timestamps: NotRequired[List[datetime]],
    Values: NotRequired[List[float]],
    StatusCode: NotRequired[StatusCodeType],  # (1)
    Messages: NotRequired[List[MessageDataTypeDef]],  # (2)
```

1. See [:material-code-brackets: StatusCodeType](./literals.md#statuscodetype) 
2. See [:material-code-braces: MessageDataTypeDef](./type_defs.md#messagedatatypedef) 
## InsightRuleContributorTypeDef

```python
# InsightRuleContributorTypeDef definition

class InsightRuleContributorTypeDef(TypedDict):
    Keys: List[str],
    ApproximateAggregateValue: float,
    Datapoints: List[InsightRuleContributorDatapointTypeDef],  # (1)
```

1. See [:material-code-braces: InsightRuleContributorDatapointTypeDef](./type_defs.md#insightrulecontributordatapointtypedef) 
## ListMetricStreamsOutputTypeDef

```python
# ListMetricStreamsOutputTypeDef definition

class ListMetricStreamsOutputTypeDef(TypedDict):
    NextToken: str,
    Entries: List[MetricStreamEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricStreamEntryTypeDef](./type_defs.md#metricstreamentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ManagedRuleTypeDef

```python
# ManagedRuleTypeDef definition

class ManagedRuleTypeDef(TypedDict):
    TemplateName: str,
    ResourceARN: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutCompositeAlarmInputRequestTypeDef

```python
# PutCompositeAlarmInputRequestTypeDef definition

class PutCompositeAlarmInputRequestTypeDef(TypedDict):
    AlarmName: str,
    AlarmRule: str,
    ActionsEnabled: NotRequired[bool],
    AlarmActions: NotRequired[Sequence[str]],
    AlarmDescription: NotRequired[str],
    InsufficientDataActions: NotRequired[Sequence[str]],
    OKActions: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    ActionsSuppressor: NotRequired[str],
    ActionsSuppressorWaitPeriod: NotRequired[int],
    ActionsSuppressorExtensionPeriod: NotRequired[int],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutInsightRuleInputRequestTypeDef

```python
# PutInsightRuleInputRequestTypeDef definition

class PutInsightRuleInputRequestTypeDef(TypedDict):
    RuleName: str,
    RuleDefinition: str,
    RuleState: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ManagedRuleDescriptionTypeDef

```python
# ManagedRuleDescriptionTypeDef definition

class ManagedRuleDescriptionTypeDef(TypedDict):
    TemplateName: NotRequired[str],
    ResourceARN: NotRequired[str],
    RuleState: NotRequired[ManagedRuleStateTypeDef],  # (1)
```

1. See [:material-code-braces: ManagedRuleStateTypeDef](./type_defs.md#managedrulestatetypedef) 
## MetricDatumTypeDef

```python
# MetricDatumTypeDef definition

class MetricDatumTypeDef(TypedDict):
    MetricName: str,
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
    Timestamp: NotRequired[Union[datetime, str]],
    Value: NotRequired[float],
    StatisticValues: NotRequired[StatisticSetTypeDef],  # (2)
    Values: NotRequired[Sequence[float]],
    Counts: NotRequired[Sequence[float]],
    Unit: NotRequired[StandardUnitType],  # (3)
    StorageResolution: NotRequired[int],
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-braces: StatisticSetTypeDef](./type_defs.md#statisticsettypedef) 
3. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
## MetricStreamStatisticsConfigurationTypeDef

```python
# MetricStreamStatisticsConfigurationTypeDef definition

class MetricStreamStatisticsConfigurationTypeDef(TypedDict):
    IncludeMetrics: List[MetricStreamStatisticsMetricTypeDef],  # (1)
    AdditionalStatistics: List[str],
```

1. See [:material-code-braces: MetricStreamStatisticsMetricTypeDef](./type_defs.md#metricstreamstatisticsmetrictypedef) 
## ListMetricsOutputTypeDef

```python
# ListMetricsOutputTypeDef definition

class ListMetricsOutputTypeDef(TypedDict):
    Metrics: List[MetricTypeDef],  # (1)
    NextToken: str,
    OwningAccounts: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricStatTypeDef

```python
# MetricStatTypeDef definition

class MetricStatTypeDef(TypedDict):
    Metric: MetricTypeDef,  # (1)
    Period: int,
    Stat: str,
    Unit: NotRequired[StandardUnitType],  # (2)
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
## GetMetricDataOutputTypeDef

```python
# GetMetricDataOutputTypeDef definition

class GetMetricDataOutputTypeDef(TypedDict):
    MetricDataResults: List[MetricDataResultTypeDef],  # (1)
    NextToken: str,
    Messages: List[MessageDataTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MetricDataResultTypeDef](./type_defs.md#metricdataresulttypedef) 
2. See [:material-code-braces: MessageDataTypeDef](./type_defs.md#messagedatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInsightRuleReportOutputTypeDef

```python
# GetInsightRuleReportOutputTypeDef definition

class GetInsightRuleReportOutputTypeDef(TypedDict):
    KeyLabels: List[str],
    AggregationStatistic: str,
    AggregateValue: float,
    ApproximateUniqueCount: int,
    Contributors: List[InsightRuleContributorTypeDef],  # (1)
    MetricDatapoints: List[InsightRuleMetricDatapointTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: InsightRuleContributorTypeDef](./type_defs.md#insightrulecontributortypedef) 
2. See [:material-code-braces: InsightRuleMetricDatapointTypeDef](./type_defs.md#insightrulemetricdatapointtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutManagedInsightRulesInputRequestTypeDef

```python
# PutManagedInsightRulesInputRequestTypeDef definition

class PutManagedInsightRulesInputRequestTypeDef(TypedDict):
    ManagedRules: Sequence[ManagedRuleTypeDef],  # (1)
```

1. See [:material-code-braces: ManagedRuleTypeDef](./type_defs.md#managedruletypedef) 
## ListManagedInsightRulesOutputTypeDef

```python
# ListManagedInsightRulesOutputTypeDef definition

class ListManagedInsightRulesOutputTypeDef(TypedDict):
    ManagedRules: List[ManagedRuleDescriptionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedRuleDescriptionTypeDef](./type_defs.md#managedruledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutMetricDataInputRequestTypeDef

```python
# PutMetricDataInputRequestTypeDef definition

class PutMetricDataInputRequestTypeDef(TypedDict):
    Namespace: str,
    MetricData: Sequence[MetricDatumTypeDef],  # (1)
```

1. See [:material-code-braces: MetricDatumTypeDef](./type_defs.md#metricdatumtypedef) 
## GetMetricStreamOutputTypeDef

```python
# GetMetricStreamOutputTypeDef definition

class GetMetricStreamOutputTypeDef(TypedDict):
    Arn: str,
    Name: str,
    IncludeFilters: List[MetricStreamFilterTypeDef],  # (1)
    ExcludeFilters: List[MetricStreamFilterTypeDef],  # (1)
    FirehoseArn: str,
    RoleArn: str,
    State: str,
    CreationDate: datetime,
    LastUpdateDate: datetime,
    OutputFormat: MetricStreamOutputFormatType,  # (3)
    StatisticsConfigurations: List[MetricStreamStatisticsConfigurationTypeDef],  # (4)
    IncludeLinkedAccountsMetrics: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: MetricStreamFilterTypeDef](./type_defs.md#metricstreamfiltertypedef) 
2. See [:material-code-braces: MetricStreamFilterTypeDef](./type_defs.md#metricstreamfiltertypedef) 
3. See [:material-code-brackets: MetricStreamOutputFormatType](./literals.md#metricstreamoutputformattype) 
4. See [:material-code-braces: MetricStreamStatisticsConfigurationTypeDef](./type_defs.md#metricstreamstatisticsconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutMetricStreamInputRequestTypeDef

```python
# PutMetricStreamInputRequestTypeDef definition

class PutMetricStreamInputRequestTypeDef(TypedDict):
    Name: str,
    FirehoseArn: str,
    RoleArn: str,
    OutputFormat: MetricStreamOutputFormatType,  # (1)
    IncludeFilters: NotRequired[Sequence[MetricStreamFilterTypeDef]],  # (2)
    ExcludeFilters: NotRequired[Sequence[MetricStreamFilterTypeDef]],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    StatisticsConfigurations: NotRequired[Sequence[MetricStreamStatisticsConfigurationTypeDef]],  # (5)
    IncludeLinkedAccountsMetrics: NotRequired[bool],
```

1. See [:material-code-brackets: MetricStreamOutputFormatType](./literals.md#metricstreamoutputformattype) 
2. See [:material-code-braces: MetricStreamFilterTypeDef](./type_defs.md#metricstreamfiltertypedef) 
3. See [:material-code-braces: MetricStreamFilterTypeDef](./type_defs.md#metricstreamfiltertypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: MetricStreamStatisticsConfigurationTypeDef](./type_defs.md#metricstreamstatisticsconfigurationtypedef) 
## MetricDataQueryTypeDef

```python
# MetricDataQueryTypeDef definition

class MetricDataQueryTypeDef(TypedDict):
    Id: str,
    MetricStat: NotRequired[MetricStatTypeDef],  # (1)
    Expression: NotRequired[str],
    Label: NotRequired[str],
    ReturnData: NotRequired[bool],
    Period: NotRequired[int],
    AccountId: NotRequired[str],
```

1. See [:material-code-braces: MetricStatTypeDef](./type_defs.md#metricstattypedef) 
## GetMetricDataInputGetMetricDataPaginateTypeDef

```python
# GetMetricDataInputGetMetricDataPaginateTypeDef definition

class GetMetricDataInputGetMetricDataPaginateTypeDef(TypedDict):
    MetricDataQueries: Sequence[MetricDataQueryTypeDef],  # (1)
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    ScanBy: NotRequired[ScanByType],  # (2)
    LabelOptions: NotRequired[LabelOptionsTypeDef],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
2. See [:material-code-brackets: ScanByType](./literals.md#scanbytype) 
3. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetMetricDataInputRequestTypeDef

```python
# GetMetricDataInputRequestTypeDef definition

class GetMetricDataInputRequestTypeDef(TypedDict):
    MetricDataQueries: Sequence[MetricDataQueryTypeDef],  # (1)
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    NextToken: NotRequired[str],
    ScanBy: NotRequired[ScanByType],  # (2)
    MaxDatapoints: NotRequired[int],
    LabelOptions: NotRequired[LabelOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
2. See [:material-code-brackets: ScanByType](./literals.md#scanbytype) 
3. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
## MetricAlarmTypeDef

```python
# MetricAlarmTypeDef definition

class MetricAlarmTypeDef(TypedDict):
    AlarmName: NotRequired[str],
    AlarmArn: NotRequired[str],
    AlarmDescription: NotRequired[str],
    AlarmConfigurationUpdatedTimestamp: NotRequired[datetime],
    ActionsEnabled: NotRequired[bool],
    OKActions: NotRequired[List[str]],
    AlarmActions: NotRequired[List[str]],
    InsufficientDataActions: NotRequired[List[str]],
    StateValue: NotRequired[StateValueType],  # (1)
    StateReason: NotRequired[str],
    StateReasonData: NotRequired[str],
    StateUpdatedTimestamp: NotRequired[datetime],
    MetricName: NotRequired[str],
    Namespace: NotRequired[str],
    Statistic: NotRequired[StatisticType],  # (2)
    ExtendedStatistic: NotRequired[str],
    Dimensions: NotRequired[List[DimensionTypeDef]],  # (3)
    Period: NotRequired[int],
    Unit: NotRequired[StandardUnitType],  # (4)
    EvaluationPeriods: NotRequired[int],
    DatapointsToAlarm: NotRequired[int],
    Threshold: NotRequired[float],
    ComparisonOperator: NotRequired[ComparisonOperatorType],  # (5)
    TreatMissingData: NotRequired[str],
    EvaluateLowSampleCountPercentile: NotRequired[str],
    Metrics: NotRequired[List[MetricDataQueryTypeDef]],  # (6)
    ThresholdMetricId: NotRequired[str],
    EvaluationState: NotRequired[EvaluationStateType],  # (7)
    StateTransitionedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
4. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
5. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
6. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
7. See [:material-code-brackets: EvaluationStateType](./literals.md#evaluationstatetype) 
## MetricMathAnomalyDetectorMetricTypeDef

```python
# MetricMathAnomalyDetectorMetricTypeDef definition

class MetricMathAnomalyDetectorMetricTypeDef(TypedDict):
    MetricDataQueries: NotRequired[List[MetricDataQueryTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
## MetricMathAnomalyDetectorTypeDef

```python
# MetricMathAnomalyDetectorTypeDef definition

class MetricMathAnomalyDetectorTypeDef(TypedDict):
    MetricDataQueries: NotRequired[Sequence[MetricDataQueryTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
## PutMetricAlarmInputMetricPutAlarmTypeDef

```python
# PutMetricAlarmInputMetricPutAlarmTypeDef definition

class PutMetricAlarmInputMetricPutAlarmTypeDef(TypedDict):
    AlarmName: str,
    EvaluationPeriods: int,
    ComparisonOperator: ComparisonOperatorType,  # (1)
    AlarmDescription: NotRequired[str],
    ActionsEnabled: NotRequired[bool],
    OKActions: NotRequired[Sequence[str]],
    AlarmActions: NotRequired[Sequence[str]],
    InsufficientDataActions: NotRequired[Sequence[str]],
    Statistic: NotRequired[StatisticType],  # (2)
    ExtendedStatistic: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (3)
    Period: NotRequired[int],
    Unit: NotRequired[StandardUnitType],  # (4)
    DatapointsToAlarm: NotRequired[int],
    Threshold: NotRequired[float],
    TreatMissingData: NotRequired[str],
    EvaluateLowSampleCountPercentile: NotRequired[str],
    Metrics: NotRequired[Sequence[MetricDataQueryTypeDef]],  # (5)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (6)
    ThresholdMetricId: NotRequired[str],
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
4. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
5. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutMetricAlarmInputRequestTypeDef

```python
# PutMetricAlarmInputRequestTypeDef definition

class PutMetricAlarmInputRequestTypeDef(TypedDict):
    AlarmName: str,
    EvaluationPeriods: int,
    ComparisonOperator: ComparisonOperatorType,  # (1)
    AlarmDescription: NotRequired[str],
    ActionsEnabled: NotRequired[bool],
    OKActions: NotRequired[Sequence[str]],
    AlarmActions: NotRequired[Sequence[str]],
    InsufficientDataActions: NotRequired[Sequence[str]],
    MetricName: NotRequired[str],
    Namespace: NotRequired[str],
    Statistic: NotRequired[StatisticType],  # (2)
    ExtendedStatistic: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (3)
    Period: NotRequired[int],
    Unit: NotRequired[StandardUnitType],  # (4)
    DatapointsToAlarm: NotRequired[int],
    Threshold: NotRequired[float],
    TreatMissingData: NotRequired[str],
    EvaluateLowSampleCountPercentile: NotRequired[str],
    Metrics: NotRequired[Sequence[MetricDataQueryTypeDef]],  # (5)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (6)
    ThresholdMetricId: NotRequired[str],
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
4. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
5. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeAlarmsForMetricOutputTypeDef

```python
# DescribeAlarmsForMetricOutputTypeDef definition

class DescribeAlarmsForMetricOutputTypeDef(TypedDict):
    MetricAlarms: List[MetricAlarmTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricAlarmTypeDef](./type_defs.md#metricalarmtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAlarmsOutputTypeDef

```python
# DescribeAlarmsOutputTypeDef definition

class DescribeAlarmsOutputTypeDef(TypedDict):
    CompositeAlarms: List[CompositeAlarmTypeDef],  # (1)
    MetricAlarms: List[MetricAlarmTypeDef],  # (2)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CompositeAlarmTypeDef](./type_defs.md#compositealarmtypedef) 
2. See [:material-code-braces: MetricAlarmTypeDef](./type_defs.md#metricalarmtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricStatAlarmTypeDef

```python
# MetricStatAlarmTypeDef definition

class MetricStatAlarmTypeDef(TypedDict):
    Metric: MetricAlarmTypeDef,  # (1)
    Period: int,
    Stat: str,
    Unit: NotRequired[StandardUnitType],  # (2)
```

1. See [:material-code-braces: MetricAlarmTypeDef](./type_defs.md#metricalarmtypedef) 
2. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
## AnomalyDetectorMetricTypeDef

```python
# AnomalyDetectorMetricTypeDef definition

class AnomalyDetectorMetricTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[List[DimensionTypeDef]],  # (1)
    Stat: NotRequired[str],
    Configuration: NotRequired[AnomalyDetectorConfigurationTypeDef],  # (2)
    StateValue: NotRequired[AnomalyDetectorStateValueType],  # (3)
    SingleMetricAnomalyDetector: NotRequired[SingleMetricAnomalyDetectorMetricTypeDef],  # (4)
    MetricMathAnomalyDetector: NotRequired[MetricMathAnomalyDetectorMetricTypeDef],  # (5)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-braces: AnomalyDetectorConfigurationTypeDef](./type_defs.md#anomalydetectorconfigurationtypedef) 
3. See [:material-code-brackets: AnomalyDetectorStateValueType](./literals.md#anomalydetectorstatevaluetype) 
4. See [:material-code-braces: SingleMetricAnomalyDetectorMetricTypeDef](./type_defs.md#singlemetricanomalydetectormetrictypedef) 
5. See [:material-code-braces: MetricMathAnomalyDetectorMetricTypeDef](./type_defs.md#metricmathanomalydetectormetrictypedef) 
## AnomalyDetectorTypeDef

```python
# AnomalyDetectorTypeDef definition

class AnomalyDetectorTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[List[DimensionTypeDef]],  # (1)
    Stat: NotRequired[str],
    Configuration: NotRequired[AnomalyDetectorConfigurationTypeDef],  # (2)
    StateValue: NotRequired[AnomalyDetectorStateValueType],  # (3)
    SingleMetricAnomalyDetector: NotRequired[SingleMetricAnomalyDetectorTypeDef],  # (4)
    MetricMathAnomalyDetector: NotRequired[MetricMathAnomalyDetectorTypeDef],  # (5)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-braces: AnomalyDetectorConfigurationTypeDef](./type_defs.md#anomalydetectorconfigurationtypedef) 
3. See [:material-code-brackets: AnomalyDetectorStateValueType](./literals.md#anomalydetectorstatevaluetype) 
4. See [:material-code-braces: SingleMetricAnomalyDetectorTypeDef](./type_defs.md#singlemetricanomalydetectortypedef) 
5. See [:material-code-braces: MetricMathAnomalyDetectorTypeDef](./type_defs.md#metricmathanomalydetectortypedef) 
## DeleteAnomalyDetectorInputRequestTypeDef

```python
# DeleteAnomalyDetectorInputRequestTypeDef definition

class DeleteAnomalyDetectorInputRequestTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
    Stat: NotRequired[str],
    SingleMetricAnomalyDetector: NotRequired[SingleMetricAnomalyDetectorTypeDef],  # (2)
    MetricMathAnomalyDetector: NotRequired[MetricMathAnomalyDetectorTypeDef],  # (3)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-braces: SingleMetricAnomalyDetectorTypeDef](./type_defs.md#singlemetricanomalydetectortypedef) 
3. See [:material-code-braces: MetricMathAnomalyDetectorTypeDef](./type_defs.md#metricmathanomalydetectortypedef) 
## PutAnomalyDetectorInputRequestTypeDef

```python
# PutAnomalyDetectorInputRequestTypeDef definition

class PutAnomalyDetectorInputRequestTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
    Stat: NotRequired[str],
    Configuration: NotRequired[AnomalyDetectorConfigurationTypeDef],  # (2)
    SingleMetricAnomalyDetector: NotRequired[SingleMetricAnomalyDetectorTypeDef],  # (3)
    MetricMathAnomalyDetector: NotRequired[MetricMathAnomalyDetectorTypeDef],  # (4)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-braces: AnomalyDetectorConfigurationTypeDef](./type_defs.md#anomalydetectorconfigurationtypedef) 
3. See [:material-code-braces: SingleMetricAnomalyDetectorTypeDef](./type_defs.md#singlemetricanomalydetectortypedef) 
4. See [:material-code-braces: MetricMathAnomalyDetectorTypeDef](./type_defs.md#metricmathanomalydetectortypedef) 
## MetricDataQueryAlarmTypeDef

```python
# MetricDataQueryAlarmTypeDef definition

class MetricDataQueryAlarmTypeDef(TypedDict):
    Id: str,
    MetricStat: NotRequired[MetricStatAlarmTypeDef],  # (1)
    Expression: NotRequired[str],
    Label: NotRequired[str],
    ReturnData: NotRequired[bool],
    Period: NotRequired[int],
    AccountId: NotRequired[str],
```

1. See [:material-code-braces: MetricStatAlarmTypeDef](./type_defs.md#metricstatalarmtypedef) 
## DescribeAnomalyDetectorsOutputMetricTypeDef

```python
# DescribeAnomalyDetectorsOutputMetricTypeDef definition

class DescribeAnomalyDetectorsOutputMetricTypeDef(TypedDict):
    AnomalyDetectors: List[AnomalyDetectorMetricTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnomalyDetectorMetricTypeDef](./type_defs.md#anomalydetectormetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAnomalyDetectorsOutputTypeDef

```python
# DescribeAnomalyDetectorsOutputTypeDef definition

class DescribeAnomalyDetectorsOutputTypeDef(TypedDict):
    AnomalyDetectors: List[AnomalyDetectorTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnomalyDetectorTypeDef](./type_defs.md#anomalydetectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
