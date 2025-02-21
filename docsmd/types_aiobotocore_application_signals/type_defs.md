# Type definitions

> [Index](../README.md) > [CloudWatchApplicationSignals](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchApplicationSignals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-signals.html#cloudwatchapplicationsignals)
    type annotations stubs module [types-aiobotocore-application-signals](https://pypi.org/project/types-aiobotocore-application-signals/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_application_signals.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## MetricUnionTypeDef

```python
# MetricUnionTypeDef Union usage example

from types_aiobotocore_application_signals.type_defs import MetricUnionTypeDef


def get_value() -> MetricUnionTypeDef:
    return ...


# MetricUnionTypeDef definition

MetricUnionTypeDef = Union[
    MetricTypeDef,  # (1)
    MetricOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: MetricOutputTypeDef](./type_defs.md#metricoutputtypedef) 

## GoalUnionTypeDef

```python
# GoalUnionTypeDef Union usage example

from types_aiobotocore_application_signals.type_defs import GoalUnionTypeDef


def get_value() -> GoalUnionTypeDef:
    return ...


# GoalUnionTypeDef definition

GoalUnionTypeDef = Union[
    GoalTypeDef,  # (1)
    GoalOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GoalTypeDef](./type_defs.md#goaltypedef) 
2. See [:material-code-braces: GoalOutputTypeDef](./type_defs.md#goaloutputtypedef) 

## MetricStatUnionTypeDef

```python
# MetricStatUnionTypeDef Union usage example

from types_aiobotocore_application_signals.type_defs import MetricStatUnionTypeDef


def get_value() -> MetricStatUnionTypeDef:
    return ...


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
# MetricDataQueryUnionTypeDef Union usage example

from types_aiobotocore_application_signals.type_defs import MetricDataQueryUnionTypeDef


def get_value() -> MetricDataQueryUnionTypeDef:
    return ...


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
# MonitoredRequestCountMetricDataQueriesUnionTypeDef Union usage example

from types_aiobotocore_application_signals.type_defs import MonitoredRequestCountMetricDataQueriesUnionTypeDef


def get_value() -> MonitoredRequestCountMetricDataQueriesUnionTypeDef:
    return ...


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
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ResponseMetadataTypeDef


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

## ServiceLevelObjectiveBudgetReportErrorTypeDef

```python
# ServiceLevelObjectiveBudgetReportErrorTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceLevelObjectiveBudgetReportErrorTypeDef


def get_value() -> ServiceLevelObjectiveBudgetReportErrorTypeDef:
    return {
        "Name": ...,
    }


# ServiceLevelObjectiveBudgetReportErrorTypeDef definition

class ServiceLevelObjectiveBudgetReportErrorTypeDef(TypedDict):
    Name: str,
    Arn: str,
    ErrorCode: str,
    ErrorMessage: str,
```

## BurnRateConfigurationTypeDef

```python
# BurnRateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import BurnRateConfigurationTypeDef


def get_value() -> BurnRateConfigurationTypeDef:
    return {
        "LookBackWindowMinutes": ...,
    }


# BurnRateConfigurationTypeDef definition

class BurnRateConfigurationTypeDef(TypedDict):
    LookBackWindowMinutes: int,
```

## CalendarIntervalOutputTypeDef

```python
# CalendarIntervalOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import CalendarIntervalOutputTypeDef


def get_value() -> CalendarIntervalOutputTypeDef:
    return {
        "StartTime": ...,
    }


# CalendarIntervalOutputTypeDef definition

class CalendarIntervalOutputTypeDef(TypedDict):
    StartTime: datetime,
    DurationUnit: DurationUnitType,  # (1)
    Duration: int,
```

1. See [:material-code-brackets: DurationUnitType](./literals.md#durationunittype) 
## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DeleteServiceLevelObjectiveInputTypeDef

```python
# DeleteServiceLevelObjectiveInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import DeleteServiceLevelObjectiveInputTypeDef


def get_value() -> DeleteServiceLevelObjectiveInputTypeDef:
    return {
        "Id": ...,
    }


# DeleteServiceLevelObjectiveInputTypeDef definition

class DeleteServiceLevelObjectiveInputTypeDef(TypedDict):
    Id: str,
```

## DimensionTypeDef

```python
# DimensionTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import DimensionTypeDef


def get_value() -> DimensionTypeDef:
    return {
        "Name": ...,
    }


# DimensionTypeDef definition

class DimensionTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## GetServiceLevelObjectiveInputTypeDef

```python
# GetServiceLevelObjectiveInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import GetServiceLevelObjectiveInputTypeDef


def get_value() -> GetServiceLevelObjectiveInputTypeDef:
    return {
        "Id": ...,
    }


# GetServiceLevelObjectiveInputTypeDef definition

class GetServiceLevelObjectiveInputTypeDef(TypedDict):
    Id: str,
```

## RollingIntervalTypeDef

```python
# RollingIntervalTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import RollingIntervalTypeDef


def get_value() -> RollingIntervalTypeDef:
    return {
        "DurationUnit": ...,
    }


# RollingIntervalTypeDef definition

class RollingIntervalTypeDef(TypedDict):
    DurationUnit: DurationUnitType,  # (1)
    Duration: int,
```

1. See [:material-code-brackets: DurationUnitType](./literals.md#durationunittype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import PaginatorConfigTypeDef


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

## ListServiceLevelObjectivesInputTypeDef

```python
# ListServiceLevelObjectivesInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceLevelObjectivesInputTypeDef


def get_value() -> ListServiceLevelObjectivesInputTypeDef:
    return {
        "KeyAttributes": ...,
    }


# ListServiceLevelObjectivesInputTypeDef definition

class ListServiceLevelObjectivesInputTypeDef(TypedDict):
    KeyAttributes: NotRequired[Mapping[str, str]],
    OperationName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ServiceLevelObjectiveSummaryTypeDef

```python
# ServiceLevelObjectiveSummaryTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceLevelObjectiveSummaryTypeDef


def get_value() -> ServiceLevelObjectiveSummaryTypeDef:
    return {
        "Arn": ...,
    }


# ServiceLevelObjectiveSummaryTypeDef definition

class ServiceLevelObjectiveSummaryTypeDef(TypedDict):
    Arn: str,
    Name: str,
    KeyAttributes: NotRequired[Dict[str, str]],
    OperationName: NotRequired[str],
    CreatedTime: NotRequired[datetime],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## BatchGetServiceLevelObjectiveBudgetReportInputTypeDef

```python
# BatchGetServiceLevelObjectiveBudgetReportInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import BatchGetServiceLevelObjectiveBudgetReportInputTypeDef


def get_value() -> BatchGetServiceLevelObjectiveBudgetReportInputTypeDef:
    return {
        "Timestamp": ...,
    }


# BatchGetServiceLevelObjectiveBudgetReportInputTypeDef definition

class BatchGetServiceLevelObjectiveBudgetReportInputTypeDef(TypedDict):
    Timestamp: TimestampTypeDef,
    SloIds: Sequence[str],
```

## CalendarIntervalTypeDef

```python
# CalendarIntervalTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import CalendarIntervalTypeDef


def get_value() -> CalendarIntervalTypeDef:
    return {
        "StartTime": ...,
    }


# CalendarIntervalTypeDef definition

class CalendarIntervalTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    DurationUnit: DurationUnitType,  # (1)
    Duration: int,
```

1. See [:material-code-brackets: DurationUnitType](./literals.md#durationunittype) 
## GetServiceInputTypeDef

```python
# GetServiceInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import GetServiceInputTypeDef


def get_value() -> GetServiceInputTypeDef:
    return {
        "StartTime": ...,
    }


# GetServiceInputTypeDef definition

class GetServiceInputTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    KeyAttributes: Mapping[str, str],
```

## ListServiceDependenciesInputTypeDef

```python
# ListServiceDependenciesInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceDependenciesInputTypeDef


def get_value() -> ListServiceDependenciesInputTypeDef:
    return {
        "StartTime": ...,
    }


# ListServiceDependenciesInputTypeDef definition

class ListServiceDependenciesInputTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    KeyAttributes: Mapping[str, str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListServiceDependentsInputTypeDef

```python
# ListServiceDependentsInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceDependentsInputTypeDef


def get_value() -> ListServiceDependentsInputTypeDef:
    return {
        "StartTime": ...,
    }


# ListServiceDependentsInputTypeDef definition

class ListServiceDependentsInputTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    KeyAttributes: Mapping[str, str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListServiceOperationsInputTypeDef

```python
# ListServiceOperationsInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceOperationsInputTypeDef


def get_value() -> ListServiceOperationsInputTypeDef:
    return {
        "StartTime": ...,
    }


# ListServiceOperationsInputTypeDef definition

class ListServiceOperationsInputTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    KeyAttributes: Mapping[str, str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListServicesInputTypeDef

```python
# ListServicesInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServicesInputTypeDef


def get_value() -> ListServicesInputTypeDef:
    return {
        "StartTime": ...,
    }


# ListServicesInputTypeDef definition

class ListServicesInputTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## MetricOutputTypeDef

```python
# MetricOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import MetricOutputTypeDef


def get_value() -> MetricOutputTypeDef:
    return {
        "Namespace": ...,
    }


# MetricOutputTypeDef definition

class MetricOutputTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[List[DimensionTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## MetricReferenceTypeDef

```python
# MetricReferenceTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import MetricReferenceTypeDef


def get_value() -> MetricReferenceTypeDef:
    return {
        "Namespace": ...,
    }


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
# MetricTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import MetricTypeDef


def get_value() -> MetricTypeDef:
    return {
        "Namespace": ...,
    }


# MetricTypeDef definition

class MetricTypeDef(TypedDict):
    Namespace: NotRequired[str],
    MetricName: NotRequired[str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## IntervalOutputTypeDef

```python
# IntervalOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import IntervalOutputTypeDef


def get_value() -> IntervalOutputTypeDef:
    return {
        "RollingInterval": ...,
    }


# IntervalOutputTypeDef definition

class IntervalOutputTypeDef(TypedDict):
    RollingInterval: NotRequired[RollingIntervalTypeDef],  # (1)
    CalendarInterval: NotRequired[CalendarIntervalOutputTypeDef],  # (2)
```

1. See [:material-code-braces: RollingIntervalTypeDef](./type_defs.md#rollingintervaltypedef) 
2. See [:material-code-braces: CalendarIntervalOutputTypeDef](./type_defs.md#calendarintervaloutputtypedef) 
## ListServiceDependenciesInputPaginateTypeDef

```python
# ListServiceDependenciesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceDependenciesInputPaginateTypeDef


def get_value() -> ListServiceDependenciesInputPaginateTypeDef:
    return {
        "StartTime": ...,
    }


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
# ListServiceDependentsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceDependentsInputPaginateTypeDef


def get_value() -> ListServiceDependentsInputPaginateTypeDef:
    return {
        "StartTime": ...,
    }


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
# ListServiceLevelObjectivesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceLevelObjectivesInputPaginateTypeDef


def get_value() -> ListServiceLevelObjectivesInputPaginateTypeDef:
    return {
        "KeyAttributes": ...,
    }


# ListServiceLevelObjectivesInputPaginateTypeDef definition

class ListServiceLevelObjectivesInputPaginateTypeDef(TypedDict):
    KeyAttributes: NotRequired[Mapping[str, str]],
    OperationName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceOperationsInputPaginateTypeDef

```python
# ListServiceOperationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceOperationsInputPaginateTypeDef


def get_value() -> ListServiceOperationsInputPaginateTypeDef:
    return {
        "StartTime": ...,
    }


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
# ListServicesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServicesInputPaginateTypeDef


def get_value() -> ListServicesInputPaginateTypeDef:
    return {
        "StartTime": ...,
    }


# ListServicesInputPaginateTypeDef definition

class ListServicesInputPaginateTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceLevelObjectivesOutputTypeDef

```python
# ListServiceLevelObjectivesOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceLevelObjectivesOutputTypeDef


def get_value() -> ListServiceLevelObjectivesOutputTypeDef:
    return {
        "SloSummaries": ...,
    }


# ListServiceLevelObjectivesOutputTypeDef definition

class ListServiceLevelObjectivesOutputTypeDef(TypedDict):
    SloSummaries: List[ServiceLevelObjectiveSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceLevelObjectiveSummaryTypeDef](./type_defs.md#servicelevelobjectivesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntervalTypeDef

```python
# IntervalTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import IntervalTypeDef


def get_value() -> IntervalTypeDef:
    return {
        "RollingInterval": ...,
    }


# IntervalTypeDef definition

class IntervalTypeDef(TypedDict):
    RollingInterval: NotRequired[RollingIntervalTypeDef],  # (1)
    CalendarInterval: NotRequired[CalendarIntervalTypeDef],  # (2)
```

1. See [:material-code-braces: RollingIntervalTypeDef](./type_defs.md#rollingintervaltypedef) 
2. See [:material-code-braces: CalendarIntervalTypeDef](./type_defs.md#calendarintervaltypedef) 
## MetricStatOutputTypeDef

```python
# MetricStatOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import MetricStatOutputTypeDef


def get_value() -> MetricStatOutputTypeDef:
    return {
        "Metric": ...,
    }


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
# ServiceDependencyTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceDependencyTypeDef


def get_value() -> ServiceDependencyTypeDef:
    return {
        "OperationName": ...,
    }


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
# ServiceDependentTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceDependentTypeDef


def get_value() -> ServiceDependentTypeDef:
    return {
        "OperationName": ...,
    }


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
# ServiceOperationTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceOperationTypeDef


def get_value() -> ServiceOperationTypeDef:
    return {
        "Name": ...,
    }


# ServiceOperationTypeDef definition

class ServiceOperationTypeDef(TypedDict):
    Name: str,
    MetricReferences: List[MetricReferenceTypeDef],  # (1)
```

1. See [:material-code-braces: MetricReferenceTypeDef](./type_defs.md#metricreferencetypedef) 
## ServiceSummaryTypeDef

```python
# ServiceSummaryTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceSummaryTypeDef


def get_value() -> ServiceSummaryTypeDef:
    return {
        "KeyAttributes": ...,
    }


# ServiceSummaryTypeDef definition

class ServiceSummaryTypeDef(TypedDict):
    KeyAttributes: Dict[str, str],
    MetricReferences: List[MetricReferenceTypeDef],  # (1)
    AttributeMaps: NotRequired[List[Dict[str, str]]],
```

1. See [:material-code-braces: MetricReferenceTypeDef](./type_defs.md#metricreferencetypedef) 
## ServiceTypeDef

```python
# ServiceTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceTypeDef


def get_value() -> ServiceTypeDef:
    return {
        "KeyAttributes": ...,
    }


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
# GoalOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import GoalOutputTypeDef


def get_value() -> GoalOutputTypeDef:
    return {
        "Interval": ...,
    }


# GoalOutputTypeDef definition

class GoalOutputTypeDef(TypedDict):
    Interval: NotRequired[IntervalOutputTypeDef],  # (1)
    AttainmentGoal: NotRequired[float],
    WarningThreshold: NotRequired[float],
```

1. See [:material-code-braces: IntervalOutputTypeDef](./type_defs.md#intervaloutputtypedef) 
## GoalTypeDef

```python
# GoalTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import GoalTypeDef


def get_value() -> GoalTypeDef:
    return {
        "Interval": ...,
    }


# GoalTypeDef definition

class GoalTypeDef(TypedDict):
    Interval: NotRequired[IntervalTypeDef],  # (1)
    AttainmentGoal: NotRequired[float],
    WarningThreshold: NotRequired[float],
```

1. See [:material-code-braces: IntervalTypeDef](./type_defs.md#intervaltypedef) 
## MetricDataQueryOutputTypeDef

```python
# MetricDataQueryOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import MetricDataQueryOutputTypeDef


def get_value() -> MetricDataQueryOutputTypeDef:
    return {
        "Id": ...,
    }


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
# ListServiceDependenciesOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceDependenciesOutputTypeDef


def get_value() -> ListServiceDependenciesOutputTypeDef:
    return {
        "StartTime": ...,
    }


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
# ListServiceDependentsOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceDependentsOutputTypeDef


def get_value() -> ListServiceDependentsOutputTypeDef:
    return {
        "StartTime": ...,
    }


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
# ListServiceOperationsOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceOperationsOutputTypeDef


def get_value() -> ListServiceOperationsOutputTypeDef:
    return {
        "StartTime": ...,
    }


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
# ListServicesOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServicesOutputTypeDef


def get_value() -> ListServicesOutputTypeDef:
    return {
        "StartTime": ...,
    }


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
# GetServiceOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import GetServiceOutputTypeDef


def get_value() -> GetServiceOutputTypeDef:
    return {
        "Service": ...,
    }


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
# MetricStatTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import MetricStatTypeDef


def get_value() -> MetricStatTypeDef:
    return {
        "Metric": ...,
    }


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
# MonitoredRequestCountMetricDataQueriesOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import MonitoredRequestCountMetricDataQueriesOutputTypeDef


def get_value() -> MonitoredRequestCountMetricDataQueriesOutputTypeDef:
    return {
        "GoodCountMetric": ...,
    }


# MonitoredRequestCountMetricDataQueriesOutputTypeDef definition

class MonitoredRequestCountMetricDataQueriesOutputTypeDef(TypedDict):
    GoodCountMetric: NotRequired[List[MetricDataQueryOutputTypeDef]],  # (1)
    BadCountMetric: NotRequired[List[MetricDataQueryOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
2. See [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
## ServiceLevelIndicatorMetricTypeDef

```python
# ServiceLevelIndicatorMetricTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceLevelIndicatorMetricTypeDef


def get_value() -> ServiceLevelIndicatorMetricTypeDef:
    return {
        "KeyAttributes": ...,
    }


# ServiceLevelIndicatorMetricTypeDef definition

class ServiceLevelIndicatorMetricTypeDef(TypedDict):
    MetricDataQueries: List[MetricDataQueryOutputTypeDef],  # (2)
    KeyAttributes: NotRequired[Dict[str, str]],
    OperationName: NotRequired[str],
    MetricType: NotRequired[ServiceLevelIndicatorMetricTypeType],  # (1)
```

1. See [:material-code-brackets: ServiceLevelIndicatorMetricTypeType](./literals.md#servicelevelindicatormetrictypetype) 
2. See [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
## RequestBasedServiceLevelIndicatorMetricTypeDef

```python
# RequestBasedServiceLevelIndicatorMetricTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import RequestBasedServiceLevelIndicatorMetricTypeDef


def get_value() -> RequestBasedServiceLevelIndicatorMetricTypeDef:
    return {
        "KeyAttributes": ...,
    }


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
# ServiceLevelIndicatorTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceLevelIndicatorTypeDef


def get_value() -> ServiceLevelIndicatorTypeDef:
    return {
        "SliMetric": ...,
    }


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
# MetricDataQueryTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import MetricDataQueryTypeDef


def get_value() -> MetricDataQueryTypeDef:
    return {
        "Id": ...,
    }


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
# RequestBasedServiceLevelIndicatorTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import RequestBasedServiceLevelIndicatorTypeDef


def get_value() -> RequestBasedServiceLevelIndicatorTypeDef:
    return {
        "RequestBasedSliMetric": ...,
    }


# RequestBasedServiceLevelIndicatorTypeDef definition

class RequestBasedServiceLevelIndicatorTypeDef(TypedDict):
    RequestBasedSliMetric: RequestBasedServiceLevelIndicatorMetricTypeDef,  # (1)
    MetricThreshold: NotRequired[float],
    ComparisonOperator: NotRequired[ServiceLevelIndicatorComparisonOperatorType],  # (2)
```

1. See [:material-code-braces: RequestBasedServiceLevelIndicatorMetricTypeDef](./type_defs.md#requestbasedservicelevelindicatormetrictypedef) 
2. See [:material-code-brackets: ServiceLevelIndicatorComparisonOperatorType](./literals.md#servicelevelindicatorcomparisonoperatortype) 
## ServiceLevelObjectiveBudgetReportTypeDef

```python
# ServiceLevelObjectiveBudgetReportTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceLevelObjectiveBudgetReportTypeDef


def get_value() -> ServiceLevelObjectiveBudgetReportTypeDef:
    return {
        "Arn": ...,
    }


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
# ServiceLevelObjectiveTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceLevelObjectiveTypeDef


def get_value() -> ServiceLevelObjectiveTypeDef:
    return {
        "Arn": ...,
    }


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
## MonitoredRequestCountMetricDataQueriesTypeDef

```python
# MonitoredRequestCountMetricDataQueriesTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import MonitoredRequestCountMetricDataQueriesTypeDef


def get_value() -> MonitoredRequestCountMetricDataQueriesTypeDef:
    return {
        "GoodCountMetric": ...,
    }


# MonitoredRequestCountMetricDataQueriesTypeDef definition

class MonitoredRequestCountMetricDataQueriesTypeDef(TypedDict):
    GoodCountMetric: NotRequired[Sequence[MetricDataQueryUnionTypeDef]],  # (1)
    BadCountMetric: NotRequired[Sequence[MetricDataQueryTypeDef]],  # (2)
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
2. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) 
## ServiceLevelIndicatorMetricConfigTypeDef

```python
# ServiceLevelIndicatorMetricConfigTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceLevelIndicatorMetricConfigTypeDef


def get_value() -> ServiceLevelIndicatorMetricConfigTypeDef:
    return {
        "KeyAttributes": ...,
    }


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
# BatchGetServiceLevelObjectiveBudgetReportOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import BatchGetServiceLevelObjectiveBudgetReportOutputTypeDef


def get_value() -> BatchGetServiceLevelObjectiveBudgetReportOutputTypeDef:
    return {
        "Timestamp": ...,
    }


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
# CreateServiceLevelObjectiveOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import CreateServiceLevelObjectiveOutputTypeDef


def get_value() -> CreateServiceLevelObjectiveOutputTypeDef:
    return {
        "Slo": ...,
    }


# CreateServiceLevelObjectiveOutputTypeDef definition

class CreateServiceLevelObjectiveOutputTypeDef(TypedDict):
    Slo: ServiceLevelObjectiveTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceLevelObjectiveTypeDef](./type_defs.md#servicelevelobjectivetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceLevelObjectiveOutputTypeDef

```python
# GetServiceLevelObjectiveOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import GetServiceLevelObjectiveOutputTypeDef


def get_value() -> GetServiceLevelObjectiveOutputTypeDef:
    return {
        "Slo": ...,
    }


# GetServiceLevelObjectiveOutputTypeDef definition

class GetServiceLevelObjectiveOutputTypeDef(TypedDict):
    Slo: ServiceLevelObjectiveTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceLevelObjectiveTypeDef](./type_defs.md#servicelevelobjectivetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceLevelObjectiveOutputTypeDef

```python
# UpdateServiceLevelObjectiveOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import UpdateServiceLevelObjectiveOutputTypeDef


def get_value() -> UpdateServiceLevelObjectiveOutputTypeDef:
    return {
        "Slo": ...,
    }


# UpdateServiceLevelObjectiveOutputTypeDef definition

class UpdateServiceLevelObjectiveOutputTypeDef(TypedDict):
    Slo: ServiceLevelObjectiveTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceLevelObjectiveTypeDef](./type_defs.md#servicelevelobjectivetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceLevelIndicatorConfigTypeDef

```python
# ServiceLevelIndicatorConfigTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceLevelIndicatorConfigTypeDef


def get_value() -> ServiceLevelIndicatorConfigTypeDef:
    return {
        "SliMetricConfig": ...,
    }


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
# RequestBasedServiceLevelIndicatorMetricConfigTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import RequestBasedServiceLevelIndicatorMetricConfigTypeDef


def get_value() -> RequestBasedServiceLevelIndicatorMetricConfigTypeDef:
    return {
        "KeyAttributes": ...,
    }


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
# RequestBasedServiceLevelIndicatorConfigTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import RequestBasedServiceLevelIndicatorConfigTypeDef


def get_value() -> RequestBasedServiceLevelIndicatorConfigTypeDef:
    return {
        "RequestBasedSliMetricConfig": ...,
    }


# RequestBasedServiceLevelIndicatorConfigTypeDef definition

class RequestBasedServiceLevelIndicatorConfigTypeDef(TypedDict):
    RequestBasedSliMetricConfig: RequestBasedServiceLevelIndicatorMetricConfigTypeDef,  # (1)
    MetricThreshold: NotRequired[float],
    ComparisonOperator: NotRequired[ServiceLevelIndicatorComparisonOperatorType],  # (2)
```

1. See [:material-code-braces: RequestBasedServiceLevelIndicatorMetricConfigTypeDef](./type_defs.md#requestbasedservicelevelindicatormetricconfigtypedef) 
2. See [:material-code-brackets: ServiceLevelIndicatorComparisonOperatorType](./literals.md#servicelevelindicatorcomparisonoperatortype) 
## CreateServiceLevelObjectiveInputTypeDef

```python
# CreateServiceLevelObjectiveInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import CreateServiceLevelObjectiveInputTypeDef


def get_value() -> CreateServiceLevelObjectiveInputTypeDef:
    return {
        "Name": ...,
    }


# CreateServiceLevelObjectiveInputTypeDef definition

class CreateServiceLevelObjectiveInputTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    SliConfig: NotRequired[ServiceLevelIndicatorConfigTypeDef],  # (1)
    RequestBasedSliConfig: NotRequired[RequestBasedServiceLevelIndicatorConfigTypeDef],  # (2)
    Goal: NotRequired[GoalUnionTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    BurnRateConfigurations: NotRequired[Sequence[BurnRateConfigurationTypeDef]],  # (5)
```

1. See [:material-code-braces: ServiceLevelIndicatorConfigTypeDef](./type_defs.md#servicelevelindicatorconfigtypedef) 
2. See [:material-code-braces: RequestBasedServiceLevelIndicatorConfigTypeDef](./type_defs.md#requestbasedservicelevelindicatorconfigtypedef) 
3. See [:material-code-braces: GoalTypeDef](./type_defs.md#goaltypedef) [:material-code-braces: GoalOutputTypeDef](./type_defs.md#goaloutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: BurnRateConfigurationTypeDef](./type_defs.md#burnrateconfigurationtypedef) 
## UpdateServiceLevelObjectiveInputTypeDef

```python
# UpdateServiceLevelObjectiveInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import UpdateServiceLevelObjectiveInputTypeDef


def get_value() -> UpdateServiceLevelObjectiveInputTypeDef:
    return {
        "Id": ...,
    }


# UpdateServiceLevelObjectiveInputTypeDef definition

class UpdateServiceLevelObjectiveInputTypeDef(TypedDict):
    Id: str,
    Description: NotRequired[str],
    SliConfig: NotRequired[ServiceLevelIndicatorConfigTypeDef],  # (1)
    RequestBasedSliConfig: NotRequired[RequestBasedServiceLevelIndicatorConfigTypeDef],  # (2)
    Goal: NotRequired[GoalUnionTypeDef],  # (3)
    BurnRateConfigurations: NotRequired[Sequence[BurnRateConfigurationTypeDef]],  # (4)
```

1. See [:material-code-braces: ServiceLevelIndicatorConfigTypeDef](./type_defs.md#servicelevelindicatorconfigtypedef) 
2. See [:material-code-braces: RequestBasedServiceLevelIndicatorConfigTypeDef](./type_defs.md#requestbasedservicelevelindicatorconfigtypedef) 
3. See [:material-code-braces: GoalTypeDef](./type_defs.md#goaltypedef) [:material-code-braces: GoalOutputTypeDef](./type_defs.md#goaloutputtypedef) 
4. See [:material-code-braces: BurnRateConfigurationTypeDef](./type_defs.md#burnrateconfigurationtypedef) 
