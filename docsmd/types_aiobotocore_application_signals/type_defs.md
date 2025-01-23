# Type definitions

> [Index](../README.md) > [CloudWatchApplicationSignals](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchApplicationSignals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-signals.html#cloudwatchapplicationsignals)
    type annotations stubs module [types-aiobotocore-application-signals](https://pypi.org/project/types-aiobotocore-application-signals/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## CalendarIntervalUnionTypeDef

```python
# CalendarIntervalUnionTypeDef definition

CalendarIntervalUnionTypeDef = Union[
    CalendarIntervalTypeDef,  # (1)
    CalendarIntervalOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CalendarIntervalTypeDef](./type_defs.md#calendarintervaltypedef) 
2. See [:material-code-braces: CalendarIntervalOutputTypeDef](./type_defs.md#calendarintervaloutputtypedef) 

## MetricUnionTypeDef

```python
# MetricUnionTypeDef definition

MetricUnionTypeDef = Union[
    MetricTypeDef,  # (1)
    MetricOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: MetricOutputTypeDef](./type_defs.md#metricoutputtypedef) 

## IntervalUnionTypeDef

```python
# IntervalUnionTypeDef definition

IntervalUnionTypeDef = Union[
    IntervalTypeDef,  # (1)
    IntervalOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IntervalTypeDef](./type_defs.md#intervaltypedef) 
2. See [:material-code-braces: IntervalOutputTypeDef](./type_defs.md#intervaloutputtypedef) 

## MetricStatUnionTypeDef

```python
# MetricStatUnionTypeDef definition

MetricStatUnionTypeDef = Union[
    MetricStatTypeDef,  # (1)
    MetricStatOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricStatTypeDef](./type_defs.md#metricstattypedef) 
2. See [:material-code-braces: MetricStatOutputTypeDef](./type_defs.md#metricstatoutputtypedef) 

## MetricDataQueryUnionTypeDef

```python
# MetricDataQueryUnionTypeDef definition

MetricDataQueryUnionTypeDef = Union[
    MetricDataQueryTypeDef,  # (1)
    MetricDataQueryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
2. See [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 

## MonitoredRequestCountMetricDataQueriesUnionTypeDef

```python
# MonitoredRequestCountMetricDataQueriesUnionTypeDef definition

MonitoredRequestCountMetricDataQueriesUnionTypeDef = Union[
    MonitoredRequestCountMetricDataQueriesTypeDef,  # (1)
    MonitoredRequestCountMetricDataQueriesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MonitoredRequestCountMetricDataQueriesTypeDef](./type_defs.md#monitoredrequestcountmetricdataqueriestypedef) 
2. See [:material-code-braces: MonitoredRequestCountMetricDataQueriesOutputTypeDef](./type_defs.md#monitoredrequestcountmetricdataqueriesoutputtypedef) 



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

## ServiceLevelObjectiveBudgetReportErrorTypeDef

```python
# ServiceLevelObjectiveBudgetReportErrorTypeDef definition

class ServiceLevelObjectiveBudgetReportErrorTypeDef(TypedDict):
    Name: str,
    Arn: str,
    ErrorCode: str,
    ErrorMessage: str,
```

## BurnRateConfigurationTypeDef

```python
# BurnRateConfigurationTypeDef definition

class BurnRateConfigurationTypeDef(TypedDict):
    LookBackWindowMinutes: int,
```

## CalendarIntervalOutputTypeDef

```python
# CalendarIntervalOutputTypeDef definition

class CalendarIntervalOutputTypeDef(TypedDict):
    StartTime: datetime,
    DurationUnit: DurationUnitType,  # (1)
    Duration: int,
```

1. See [:material-code-brackets: DurationUnitType](./literals.md#durationunittype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DeleteServiceLevelObjectiveInputRequestTypeDef

```python
# DeleteServiceLevelObjectiveInputRequestTypeDef definition

class DeleteServiceLevelObjectiveInputRequestTypeDef(TypedDict):
    Id: str,
```

## DimensionTypeDef

```python
# DimensionTypeDef definition

class DimensionTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## GetServiceLevelObjectiveInputRequestTypeDef

```python
# GetServiceLevelObjectiveInputRequestTypeDef definition

class GetServiceLevelObjectiveInputRequestTypeDef(TypedDict):
    Id: str,
```

## RollingIntervalTypeDef

```python
# RollingIntervalTypeDef definition

class RollingIntervalTypeDef(TypedDict):
    DurationUnit: DurationUnitType,  # (1)
    Duration: int,
```

1. See [:material-code-brackets: DurationUnitType](./literals.md#durationunittype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListServiceLevelObjectivesInputRequestTypeDef

```python
# ListServiceLevelObjectivesInputRequestTypeDef definition

class ListServiceLevelObjectivesInputRequestTypeDef(TypedDict):
    KeyAttributes: NotRequired[Mapping[str, str]],
    OperationName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ServiceLevelObjectiveSummaryTypeDef

```python
# ServiceLevelObjectiveSummaryTypeDef definition

class ServiceLevelObjectiveSummaryTypeDef(TypedDict):
    Arn: str,
    Name: str,
    KeyAttributes: NotRequired[Dict[str, str]],
    OperationName: NotRequired[str],
    CreatedTime: NotRequired[datetime],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## BatchGetServiceLevelObjectiveBudgetReportInputRequestTypeDef

```python
# BatchGetServiceLevelObjectiveBudgetReportInputRequestTypeDef definition

class BatchGetServiceLevelObjectiveBudgetReportInputRequestTypeDef(TypedDict):
    Timestamp: TimestampTypeDef,
    SloIds: Sequence[str],
```

## CalendarIntervalTypeDef

```python
# CalendarIntervalTypeDef definition

class CalendarIntervalTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    DurationUnit: DurationUnitType,  # (1)
    Duration: int,
```

1. See [:material-code-brackets: DurationUnitType](./literals.md#durationunittype) 
## GetServiceInputRequestTypeDef

```python
# GetServiceInputRequestTypeDef definition

class GetServiceInputRequestTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    KeyAttributes: Mapping[str, str],
```

## ListServiceDependenciesInputRequestTypeDef

```python
# ListServiceDependenciesInputRequestTypeDef definition

class ListServiceDependenciesInputRequestTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    KeyAttributes: Mapping[str, str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListServiceDependentsInputRequestTypeDef

```python
# ListServiceDependentsInputRequestTypeDef definition

class ListServiceDependentsInputRequestTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    KeyAttributes: Mapping[str, str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListServiceOperationsInputRequestTypeDef

```python
# ListServiceOperationsInputRequestTypeDef definition

class ListServiceOperationsInputRequestTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    KeyAttributes: Mapping[str, str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListServicesInputRequestTypeDef

```python
# ListServicesInputRequestTypeDef definition

class ListServicesInputRequestTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## MetricOutputTypeDef

```python
# MetricOutputTypeDef definition

class MetricOutputTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[List[DimensionTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## MetricReferenceTypeDef

```python
# MetricReferenceTypeDef definition

class MetricReferenceTypeDef(TypedDict):
    Namespace: str,
    MetricType: str,
    MetricName: str,
    Dimensions: NotRequired[List[DimensionTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## MetricTypeDef

```python
# MetricTypeDef definition

class MetricTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## IntervalOutputTypeDef

```python
# IntervalOutputTypeDef definition

class IntervalOutputTypeDef(TypedDict):
    RollingInterval: NotRequired[RollingIntervalTypeDef],  # (1)
    CalendarInterval: NotRequired[CalendarIntervalOutputTypeDef],  # (2)
```

1. See [:material-code-braces: RollingIntervalTypeDef](./type_defs.md#rollingintervaltypedef) 
2. See [:material-code-braces: CalendarIntervalOutputTypeDef](./type_defs.md#calendarintervaloutputtypedef) 
## ListServiceDependenciesInputPaginateTypeDef

```python
# ListServiceDependenciesInputPaginateTypeDef definition

class ListServiceDependenciesInputPaginateTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    KeyAttributes: Mapping[str, str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceDependentsInputPaginateTypeDef

```python
# ListServiceDependentsInputPaginateTypeDef definition

class ListServiceDependentsInputPaginateTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    KeyAttributes: Mapping[str, str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceLevelObjectivesInputPaginateTypeDef

```python
# ListServiceLevelObjectivesInputPaginateTypeDef definition

class ListServiceLevelObjectivesInputPaginateTypeDef(TypedDict):
    KeyAttributes: NotRequired[Mapping[str, str]],
    OperationName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceOperationsInputPaginateTypeDef

```python
# ListServiceOperationsInputPaginateTypeDef definition

class ListServiceOperationsInputPaginateTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    KeyAttributes: Mapping[str, str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesInputPaginateTypeDef

```python
# ListServicesInputPaginateTypeDef definition

class ListServicesInputPaginateTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceLevelObjectivesOutputTypeDef

```python
# ListServiceLevelObjectivesOutputTypeDef definition

class ListServiceLevelObjectivesOutputTypeDef(TypedDict):
    SloSummaries: List[ServiceLevelObjectiveSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceLevelObjectiveSummaryTypeDef](./type_defs.md#servicelevelobjectivesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricStatOutputTypeDef

```python
# MetricStatOutputTypeDef definition

class MetricStatOutputTypeDef(TypedDict):
    Metric: MetricOutputTypeDef,  # (1)
    Period: int,
    Stat: str,
    Unit: NotRequired[StandardUnitType],  # (2)
```

1. See [:material-code-braces: MetricOutputTypeDef](./type_defs.md#metricoutputtypedef) 
2. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
## ServiceDependencyTypeDef

```python
# ServiceDependencyTypeDef definition

class ServiceDependencyTypeDef(TypedDict):
    OperationName: str,
    DependencyKeyAttributes: Dict[str, str],
    DependencyOperationName: str,
    MetricReferences: List[MetricReferenceTypeDef],  # (1)
```

1. See [:material-code-braces: MetricReferenceTypeDef](./type_defs.md#metricreferencetypedef) 
## ServiceDependentTypeDef

```python
# ServiceDependentTypeDef definition

class ServiceDependentTypeDef(TypedDict):
    DependentKeyAttributes: Dict[str, str],
    MetricReferences: List[MetricReferenceTypeDef],  # (1)
    OperationName: NotRequired[str],
    DependentOperationName: NotRequired[str],
```

1. See [:material-code-braces: MetricReferenceTypeDef](./type_defs.md#metricreferencetypedef) 
## ServiceOperationTypeDef

```python
# ServiceOperationTypeDef definition

class ServiceOperationTypeDef(TypedDict):
    Name: str,
    MetricReferences: List[MetricReferenceTypeDef],  # (1)
```

1. See [:material-code-braces: MetricReferenceTypeDef](./type_defs.md#metricreferencetypedef) 
## ServiceSummaryTypeDef

```python
# ServiceSummaryTypeDef definition

class ServiceSummaryTypeDef(TypedDict):
    KeyAttributes: Dict[str, str],
    MetricReferences: List[MetricReferenceTypeDef],  # (1)
    AttributeMaps: NotRequired[List[Dict[str, str]]],
```

1. See [:material-code-braces: MetricReferenceTypeDef](./type_defs.md#metricreferencetypedef) 
## ServiceTypeDef

```python
# ServiceTypeDef definition

class ServiceTypeDef(TypedDict):
    KeyAttributes: Dict[str, str],
    MetricReferences: List[MetricReferenceTypeDef],  # (1)
    AttributeMaps: NotRequired[List[Dict[str, str]]],
    LogGroupReferences: NotRequired[List[Dict[str, str]]],
```

1. See [:material-code-braces: MetricReferenceTypeDef](./type_defs.md#metricreferencetypedef) 
## GoalOutputTypeDef

```python
# GoalOutputTypeDef definition

class GoalOutputTypeDef(TypedDict):
    Interval: NotRequired[IntervalOutputTypeDef],  # (1)
    AttainmentGoal: NotRequired[float],
    WarningThreshold: NotRequired[float],
```

1. See [:material-code-braces: IntervalOutputTypeDef](./type_defs.md#intervaloutputtypedef) 
## IntervalTypeDef

```python
# IntervalTypeDef definition

class IntervalTypeDef(TypedDict):
    RollingInterval: NotRequired[RollingIntervalTypeDef],  # (1)
    CalendarInterval: NotRequired[CalendarIntervalUnionTypeDef],  # (2)
```

1. See [:material-code-braces: RollingIntervalTypeDef](./type_defs.md#rollingintervaltypedef) 
2. See [:material-code-braces: CalendarIntervalTypeDef](./type_defs.md#calendarintervaltypedef) [:material-code-braces: CalendarIntervalOutputTypeDef](./type_defs.md#calendarintervaloutputtypedef) 
## MetricDataQueryOutputTypeDef

```python
# MetricDataQueryOutputTypeDef definition

class MetricDataQueryOutputTypeDef(TypedDict):
    Id: str,
    MetricStat: NotRequired[MetricStatOutputTypeDef],  # (1)
    Expression: NotRequired[str],
    Label: NotRequired[str],
    ReturnData: NotRequired[bool],
    Period: NotRequired[int],
    AccountId: NotRequired[str],
```

1. See [:material-code-braces: MetricStatOutputTypeDef](./type_defs.md#metricstatoutputtypedef) 
## ListServiceDependenciesOutputTypeDef

```python
# ListServiceDependenciesOutputTypeDef definition

class ListServiceDependenciesOutputTypeDef(TypedDict):
    StartTime: datetime,
    EndTime: datetime,
    ServiceDependencies: List[ServiceDependencyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceDependencyTypeDef](./type_defs.md#servicedependencytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceDependentsOutputTypeDef

```python
# ListServiceDependentsOutputTypeDef definition

class ListServiceDependentsOutputTypeDef(TypedDict):
    StartTime: datetime,
    EndTime: datetime,
    ServiceDependents: List[ServiceDependentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceDependentTypeDef](./type_defs.md#servicedependenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceOperationsOutputTypeDef

```python
# ListServiceOperationsOutputTypeDef definition

class ListServiceOperationsOutputTypeDef(TypedDict):
    StartTime: datetime,
    EndTime: datetime,
    ServiceOperations: List[ServiceOperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceOperationTypeDef](./type_defs.md#serviceoperationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServicesOutputTypeDef

```python
# ListServicesOutputTypeDef definition

class ListServicesOutputTypeDef(TypedDict):
    StartTime: datetime,
    EndTime: datetime,
    ServiceSummaries: List[ServiceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceSummaryTypeDef](./type_defs.md#servicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceOutputTypeDef

```python
# GetServiceOutputTypeDef definition

class GetServiceOutputTypeDef(TypedDict):
    Service: ServiceTypeDef,  # (1)
    StartTime: datetime,
    EndTime: datetime,
    LogGroupReferences: List[Dict[str, str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricStatTypeDef

```python
# MetricStatTypeDef definition

class MetricStatTypeDef(TypedDict):
    Metric: MetricUnionTypeDef,  # (1)
    Period: int,
    Stat: str,
    Unit: NotRequired[StandardUnitType],  # (2)
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) [:material-code-braces: MetricOutputTypeDef](./type_defs.md#metricoutputtypedef) 
2. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
## MonitoredRequestCountMetricDataQueriesOutputTypeDef

```python
# MonitoredRequestCountMetricDataQueriesOutputTypeDef definition

class MonitoredRequestCountMetricDataQueriesOutputTypeDef(TypedDict):
    GoodCountMetric: NotRequired[List[MetricDataQueryOutputTypeDef]],  # (1)
    BadCountMetric: NotRequired[List[MetricDataQueryOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
2. See [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
## ServiceLevelIndicatorMetricTypeDef

```python
# ServiceLevelIndicatorMetricTypeDef definition

class ServiceLevelIndicatorMetricTypeDef(TypedDict):
    MetricDataQueries: List[MetricDataQueryOutputTypeDef],  # (2)
    KeyAttributes: NotRequired[Dict[str, str]],
    OperationName: NotRequired[str],
    MetricType: NotRequired[ServiceLevelIndicatorMetricTypeType],  # (1)
```

1. See [:material-code-brackets: ServiceLevelIndicatorMetricTypeType](./literals.md#servicelevelindicatormetrictypetype) 
2. See [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
## GoalTypeDef

```python
# GoalTypeDef definition

class GoalTypeDef(TypedDict):
    Interval: NotRequired[IntervalUnionTypeDef],  # (1)
    AttainmentGoal: NotRequired[float],
    WarningThreshold: NotRequired[float],
```

1. See [:material-code-braces: IntervalTypeDef](./type_defs.md#intervaltypedef) [:material-code-braces: IntervalOutputTypeDef](./type_defs.md#intervaloutputtypedef) 
## RequestBasedServiceLevelIndicatorMetricTypeDef

```python
# RequestBasedServiceLevelIndicatorMetricTypeDef definition

class RequestBasedServiceLevelIndicatorMetricTypeDef(TypedDict):
    TotalRequestCountMetric: List[MetricDataQueryOutputTypeDef],  # (2)
    MonitoredRequestCountMetric: MonitoredRequestCountMetricDataQueriesOutputTypeDef,  # (3)
    KeyAttributes: NotRequired[Dict[str, str]],
    OperationName: NotRequired[str],
    MetricType: NotRequired[ServiceLevelIndicatorMetricTypeType],  # (1)
```

1. See [:material-code-brackets: ServiceLevelIndicatorMetricTypeType](./literals.md#servicelevelindicatormetrictypetype) 
2. See [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
3. See [:material-code-braces: MonitoredRequestCountMetricDataQueriesOutputTypeDef](./type_defs.md#monitoredrequestcountmetricdataqueriesoutputtypedef) 
## ServiceLevelIndicatorTypeDef

```python
# ServiceLevelIndicatorTypeDef definition

class ServiceLevelIndicatorTypeDef(TypedDict):
    SliMetric: ServiceLevelIndicatorMetricTypeDef,  # (1)
    MetricThreshold: float,
    ComparisonOperator: ServiceLevelIndicatorComparisonOperatorType,  # (2)
```

1. See [:material-code-braces: ServiceLevelIndicatorMetricTypeDef](./type_defs.md#servicelevelindicatormetrictypedef) 
2. See [:material-code-brackets: ServiceLevelIndicatorComparisonOperatorType](./literals.md#servicelevelindicatorcomparisonoperatortype) 
## MetricDataQueryTypeDef

```python
# MetricDataQueryTypeDef definition

class MetricDataQueryTypeDef(TypedDict):
    Id: str,
    MetricStat: NotRequired[MetricStatUnionTypeDef],  # (1)
    Expression: NotRequired[str],
    Label: NotRequired[str],
    ReturnData: NotRequired[bool],
    Period: NotRequired[int],
    AccountId: NotRequired[str],
```

1. See [:material-code-braces: MetricStatTypeDef](./type_defs.md#metricstattypedef) [:material-code-braces: MetricStatOutputTypeDef](./type_defs.md#metricstatoutputtypedef) 
## RequestBasedServiceLevelIndicatorTypeDef

```python
# RequestBasedServiceLevelIndicatorTypeDef definition

class RequestBasedServiceLevelIndicatorTypeDef(TypedDict):
    RequestBasedSliMetric: RequestBasedServiceLevelIndicatorMetricTypeDef,  # (1)
    MetricThreshold: NotRequired[float],
    ComparisonOperator: NotRequired[ServiceLevelIndicatorComparisonOperatorType],  # (2)
```

1. See [:material-code-braces: RequestBasedServiceLevelIndicatorMetricTypeDef](./type_defs.md#requestbasedservicelevelindicatormetrictypedef) 
2. See [:material-code-brackets: ServiceLevelIndicatorComparisonOperatorType](./literals.md#servicelevelindicatorcomparisonoperatortype) 
## MonitoredRequestCountMetricDataQueriesTypeDef

```python
# MonitoredRequestCountMetricDataQueriesTypeDef definition

class MonitoredRequestCountMetricDataQueriesTypeDef(TypedDict):
    GoodCountMetric: NotRequired[Sequence[MetricDataQueryTypeDef]],  # (1)
    BadCountMetric: NotRequired[Sequence[MetricDataQueryTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
2. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
## ServiceLevelObjectiveBudgetReportTypeDef

```python
# ServiceLevelObjectiveBudgetReportTypeDef definition

class ServiceLevelObjectiveBudgetReportTypeDef(TypedDict):
    Arn: str,
    Name: str,
    BudgetStatus: ServiceLevelObjectiveBudgetStatusType,  # (2)
    EvaluationType: NotRequired[EvaluationTypeType],  # (1)
    Attainment: NotRequired[float],
    TotalBudgetSeconds: NotRequired[int],
    BudgetSecondsRemaining: NotRequired[int],
    TotalBudgetRequests: NotRequired[int],
    BudgetRequestsRemaining: NotRequired[int],
    Sli: NotRequired[ServiceLevelIndicatorTypeDef],  # (3)
    RequestBasedSli: NotRequired[RequestBasedServiceLevelIndicatorTypeDef],  # (4)
    Goal: NotRequired[GoalOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: EvaluationTypeType](./literals.md#evaluationtypetype) 
2. See [:material-code-brackets: ServiceLevelObjectiveBudgetStatusType](./literals.md#servicelevelobjectivebudgetstatustype) 
3. See [:material-code-braces: ServiceLevelIndicatorTypeDef](./type_defs.md#servicelevelindicatortypedef) 
4. See [:material-code-braces: RequestBasedServiceLevelIndicatorTypeDef](./type_defs.md#requestbasedservicelevelindicatortypedef) 
5. See [:material-code-braces: GoalOutputTypeDef](./type_defs.md#goaloutputtypedef) 
## ServiceLevelObjectiveTypeDef

```python
# ServiceLevelObjectiveTypeDef definition

class ServiceLevelObjectiveTypeDef(TypedDict):
    Arn: str,
    Name: str,
    CreatedTime: datetime,
    LastUpdatedTime: datetime,
    Goal: GoalOutputTypeDef,  # (4)
    Description: NotRequired[str],
    Sli: NotRequired[ServiceLevelIndicatorTypeDef],  # (1)
    RequestBasedSli: NotRequired[RequestBasedServiceLevelIndicatorTypeDef],  # (2)
    EvaluationType: NotRequired[EvaluationTypeType],  # (3)
    BurnRateConfigurations: NotRequired[List[BurnRateConfigurationTypeDef]],  # (5)
```

1. See [:material-code-braces: ServiceLevelIndicatorTypeDef](./type_defs.md#servicelevelindicatortypedef) 
2. See [:material-code-braces: RequestBasedServiceLevelIndicatorTypeDef](./type_defs.md#requestbasedservicelevelindicatortypedef) 
3. See [:material-code-brackets: EvaluationTypeType](./literals.md#evaluationtypetype) 
4. See [:material-code-braces: GoalOutputTypeDef](./type_defs.md#goaloutputtypedef) 
5. See [:material-code-braces: BurnRateConfigurationTypeDef](./type_defs.md#burnrateconfigurationtypedef) 
## ServiceLevelIndicatorMetricConfigTypeDef

```python
# ServiceLevelIndicatorMetricConfigTypeDef definition

class ServiceLevelIndicatorMetricConfigTypeDef(TypedDict):
    KeyAttributes: NotRequired[Mapping[str, str]],
    OperationName: NotRequired[str],
    MetricType: NotRequired[ServiceLevelIndicatorMetricTypeType],  # (1)
    Statistic: NotRequired[str],
    PeriodSeconds: NotRequired[int],
    MetricDataQueries: NotRequired[Sequence[MetricDataQueryUnionTypeDef]],  # (2)
```

1. See [:material-code-brackets: ServiceLevelIndicatorMetricTypeType](./literals.md#servicelevelindicatormetrictypetype) 
2. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
## BatchGetServiceLevelObjectiveBudgetReportOutputTypeDef

```python
# BatchGetServiceLevelObjectiveBudgetReportOutputTypeDef definition

class BatchGetServiceLevelObjectiveBudgetReportOutputTypeDef(TypedDict):
    Timestamp: datetime,
    Reports: List[ServiceLevelObjectiveBudgetReportTypeDef],  # (1)
    Errors: List[ServiceLevelObjectiveBudgetReportErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ServiceLevelObjectiveBudgetReportTypeDef](./type_defs.md#servicelevelobjectivebudgetreporttypedef) 
2. See [:material-code-braces: ServiceLevelObjectiveBudgetReportErrorTypeDef](./type_defs.md#servicelevelobjectivebudgetreporterrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceLevelObjectiveOutputTypeDef

```python
# CreateServiceLevelObjectiveOutputTypeDef definition

class CreateServiceLevelObjectiveOutputTypeDef(TypedDict):
    Slo: ServiceLevelObjectiveTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceLevelObjectiveTypeDef](./type_defs.md#servicelevelobjectivetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceLevelObjectiveOutputTypeDef

```python
# GetServiceLevelObjectiveOutputTypeDef definition

class GetServiceLevelObjectiveOutputTypeDef(TypedDict):
    Slo: ServiceLevelObjectiveTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceLevelObjectiveTypeDef](./type_defs.md#servicelevelobjectivetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceLevelObjectiveOutputTypeDef

```python
# UpdateServiceLevelObjectiveOutputTypeDef definition

class UpdateServiceLevelObjectiveOutputTypeDef(TypedDict):
    Slo: ServiceLevelObjectiveTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceLevelObjectiveTypeDef](./type_defs.md#servicelevelobjectivetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceLevelIndicatorConfigTypeDef

```python
# ServiceLevelIndicatorConfigTypeDef definition

class ServiceLevelIndicatorConfigTypeDef(TypedDict):
    SliMetricConfig: ServiceLevelIndicatorMetricConfigTypeDef,  # (1)
    MetricThreshold: float,
    ComparisonOperator: ServiceLevelIndicatorComparisonOperatorType,  # (2)
```

1. See [:material-code-braces: ServiceLevelIndicatorMetricConfigTypeDef](./type_defs.md#servicelevelindicatormetricconfigtypedef) 
2. See [:material-code-brackets: ServiceLevelIndicatorComparisonOperatorType](./literals.md#servicelevelindicatorcomparisonoperatortype) 
## RequestBasedServiceLevelIndicatorMetricConfigTypeDef

```python
# RequestBasedServiceLevelIndicatorMetricConfigTypeDef definition

class RequestBasedServiceLevelIndicatorMetricConfigTypeDef(TypedDict):
    KeyAttributes: NotRequired[Mapping[str, str]],
    OperationName: NotRequired[str],
    MetricType: NotRequired[ServiceLevelIndicatorMetricTypeType],  # (1)
    TotalRequestCountMetric: NotRequired[Sequence[MetricDataQueryUnionTypeDef]],  # (2)
    MonitoredRequestCountMetric: NotRequired[MonitoredRequestCountMetricDataQueriesUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: ServiceLevelIndicatorMetricTypeType](./literals.md#servicelevelindicatormetrictypetype) 
2. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
3. See [:material-code-braces: MonitoredRequestCountMetricDataQueriesTypeDef](./type_defs.md#monitoredrequestcountmetricdataqueriestypedef) [:material-code-braces: MonitoredRequestCountMetricDataQueriesOutputTypeDef](./type_defs.md#monitoredrequestcountmetricdataqueriesoutputtypedef) 
## RequestBasedServiceLevelIndicatorConfigTypeDef

```python
# RequestBasedServiceLevelIndicatorConfigTypeDef definition

class RequestBasedServiceLevelIndicatorConfigTypeDef(TypedDict):
    RequestBasedSliMetricConfig: RequestBasedServiceLevelIndicatorMetricConfigTypeDef,  # (1)
    MetricThreshold: NotRequired[float],
    ComparisonOperator: NotRequired[ServiceLevelIndicatorComparisonOperatorType],  # (2)
```

1. See [:material-code-braces: RequestBasedServiceLevelIndicatorMetricConfigTypeDef](./type_defs.md#requestbasedservicelevelindicatormetricconfigtypedef) 
2. See [:material-code-brackets: ServiceLevelIndicatorComparisonOperatorType](./literals.md#servicelevelindicatorcomparisonoperatortype) 
## CreateServiceLevelObjectiveInputRequestTypeDef

```python
# CreateServiceLevelObjectiveInputRequestTypeDef definition

class CreateServiceLevelObjectiveInputRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    SliConfig: NotRequired[ServiceLevelIndicatorConfigTypeDef],  # (1)
    RequestBasedSliConfig: NotRequired[RequestBasedServiceLevelIndicatorConfigTypeDef],  # (2)
    Goal: NotRequired[GoalTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    BurnRateConfigurations: NotRequired[Sequence[BurnRateConfigurationTypeDef]],  # (5)
```

1. See [:material-code-braces: ServiceLevelIndicatorConfigTypeDef](./type_defs.md#servicelevelindicatorconfigtypedef) 
2. See [:material-code-braces: RequestBasedServiceLevelIndicatorConfigTypeDef](./type_defs.md#requestbasedservicelevelindicatorconfigtypedef) 
3. See [:material-code-braces: GoalTypeDef](./type_defs.md#goaltypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: BurnRateConfigurationTypeDef](./type_defs.md#burnrateconfigurationtypedef) 
## UpdateServiceLevelObjectiveInputRequestTypeDef

```python
# UpdateServiceLevelObjectiveInputRequestTypeDef definition

class UpdateServiceLevelObjectiveInputRequestTypeDef(TypedDict):
    Id: str,
    Description: NotRequired[str],
    SliConfig: NotRequired[ServiceLevelIndicatorConfigTypeDef],  # (1)
    RequestBasedSliConfig: NotRequired[RequestBasedServiceLevelIndicatorConfigTypeDef],  # (2)
    Goal: NotRequired[GoalTypeDef],  # (3)
    BurnRateConfigurations: NotRequired[Sequence[BurnRateConfigurationTypeDef]],  # (4)
```

1. See [:material-code-braces: ServiceLevelIndicatorConfigTypeDef](./type_defs.md#servicelevelindicatorconfigtypedef) 
2. See [:material-code-braces: RequestBasedServiceLevelIndicatorConfigTypeDef](./type_defs.md#requestbasedservicelevelindicatorconfigtypedef) 
3. See [:material-code-braces: GoalTypeDef](./type_defs.md#goaltypedef) 
4. See [:material-code-braces: BurnRateConfigurationTypeDef](./type_defs.md#burnrateconfigurationtypedef) 
