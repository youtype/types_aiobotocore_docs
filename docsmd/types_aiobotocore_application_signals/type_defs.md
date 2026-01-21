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
    datetime.datetime,
    str,
]
```


## AttributeFilterUnionTypeDef

```python
# AttributeFilterUnionTypeDef Union usage example

from types_aiobotocore_application_signals.type_defs import AttributeFilterUnionTypeDef


def get_value() -> AttributeFilterUnionTypeDef:
    return ...


# AttributeFilterUnionTypeDef definition

AttributeFilterUnionTypeDef = Union[
    AttributeFilterTypeDef,  # (1)
    AttributeFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef)
2. See [:material-code-braces: AttributeFilterOutputTypeDef](./type_defs.md#attributefilteroutputtypedef)

## DependencyConfigUnionTypeDef

```python
# DependencyConfigUnionTypeDef Union usage example

from types_aiobotocore_application_signals.type_defs import DependencyConfigUnionTypeDef


def get_value() -> DependencyConfigUnionTypeDef:
    return ...


# DependencyConfigUnionTypeDef definition

DependencyConfigUnionTypeDef = Union[
    DependencyConfigTypeDef,  # (1)
    DependencyConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DependencyConfigTypeDef](./type_defs.md#dependencyconfigtypedef)
2. See [:material-code-braces: DependencyConfigOutputTypeDef](./type_defs.md#dependencyconfigoutputtypedef)

## GroupingAttributeDefinitionUnionTypeDef

```python
# GroupingAttributeDefinitionUnionTypeDef Union usage example

from types_aiobotocore_application_signals.type_defs import GroupingAttributeDefinitionUnionTypeDef


def get_value() -> GroupingAttributeDefinitionUnionTypeDef:
    return ...


# GroupingAttributeDefinitionUnionTypeDef definition

GroupingAttributeDefinitionUnionTypeDef = Union[
    GroupingAttributeDefinitionTypeDef,  # (1)
    GroupingAttributeDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GroupingAttributeDefinitionTypeDef](./type_defs.md#groupingattributedefinitiontypedef)
2. See [:material-code-braces: GroupingAttributeDefinitionOutputTypeDef](./type_defs.md#groupingattributedefinitionoutputtypedef)

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

## ExclusionWindowUnionTypeDef

```python
# ExclusionWindowUnionTypeDef Union usage example

from types_aiobotocore_application_signals.type_defs import ExclusionWindowUnionTypeDef


def get_value() -> ExclusionWindowUnionTypeDef:
    return ...


# ExclusionWindowUnionTypeDef definition

ExclusionWindowUnionTypeDef = Union[
    ExclusionWindowTypeDef,  # (1)
    ExclusionWindowOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExclusionWindowTypeDef](./type_defs.md#exclusionwindowtypedef)
2. See [:material-code-braces: ExclusionWindowOutputTypeDef](./type_defs.md#exclusionwindowoutputtypedef)

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



## AttributeFilterOutputTypeDef

```python
# AttributeFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import AttributeFilterOutputTypeDef


def get_value() -> AttributeFilterOutputTypeDef:
    return {
        "AttributeFilterName": ...,
    }


# AttributeFilterOutputTypeDef definition

class AttributeFilterOutputTypeDef(TypedDict):
    AttributeFilterName: str,
    AttributeFilterValues: list[str],
```


## AttributeFilterTypeDef

```python
# AttributeFilterTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import AttributeFilterTypeDef


def get_value() -> AttributeFilterTypeDef:
    return {
        "AttributeFilterName": ...,
    }


# AttributeFilterTypeDef definition

class AttributeFilterTypeDef(TypedDict):
    AttributeFilterName: str,
    AttributeFilterValues: Sequence[str],
```


## AuditorResultTypeDef

```python
# AuditorResultTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import AuditorResultTypeDef


def get_value() -> AuditorResultTypeDef:
    return {
        "Auditor": ...,
    }


# AuditorResultTypeDef definition

class AuditorResultTypeDef(TypedDict):
    Auditor: NotRequired[str],
    Description: NotRequired[str],
    Data: NotRequired[dict[str, str]],
    Severity: NotRequired[SeverityType],  # (1)
```

1. See [:material-code-brackets: SeverityType](./literals.md#severitytype)

## CanaryEntityTypeDef

```python
# CanaryEntityTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import CanaryEntityTypeDef


def get_value() -> CanaryEntityTypeDef:
    return {
        "CanaryName": ...,
    }


# CanaryEntityTypeDef definition

class CanaryEntityTypeDef(TypedDict):
    CanaryName: str,
```


## ServiceEntityTypeDef

```python
# ServiceEntityTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceEntityTypeDef


def get_value() -> ServiceEntityTypeDef:
    return {
        "Type": ...,
    }


# ServiceEntityTypeDef definition

class ServiceEntityTypeDef(TypedDict):
    Type: NotRequired[str],
    Name: NotRequired[str],
    Environment: NotRequired[str],
    AwsAccountId: NotRequired[str],
```


## ServiceLevelObjectiveEntityTypeDef

```python
# ServiceLevelObjectiveEntityTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceLevelObjectiveEntityTypeDef


def get_value() -> ServiceLevelObjectiveEntityTypeDef:
    return {
        "SloName": ...,
    }


# ServiceLevelObjectiveEntityTypeDef definition

class ServiceLevelObjectiveEntityTypeDef(TypedDict):
    SloName: NotRequired[str],
    SloArn: NotRequired[str],
```


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
    HTTPHeaders: dict[str, str],
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


## BatchUpdateExclusionWindowsErrorTypeDef

```python
# BatchUpdateExclusionWindowsErrorTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import BatchUpdateExclusionWindowsErrorTypeDef


def get_value() -> BatchUpdateExclusionWindowsErrorTypeDef:
    return {
        "SloId": ...,
    }


# BatchUpdateExclusionWindowsErrorTypeDef definition

class BatchUpdateExclusionWindowsErrorTypeDef(TypedDict):
    SloId: str,
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
    StartTime: datetime.datetime,
    DurationUnit: DurationUnitType,  # (1)
    Duration: int,
```

1. See [:material-code-brackets: DurationUnitType](./literals.md#durationunittype)

## ChangeEventTypeDef

```python
# ChangeEventTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ChangeEventTypeDef


def get_value() -> ChangeEventTypeDef:
    return {
        "Timestamp": ...,
    }


# ChangeEventTypeDef definition

class ChangeEventTypeDef(TypedDict):
    Timestamp: datetime.datetime,
    AccountId: str,
    Region: str,
    Entity: dict[str, str],
    ChangeEventType: ChangeEventTypeType,  # (1)
    EventId: str,
    UserName: NotRequired[str],
    EventName: NotRequired[str],
```

1. See [:material-code-brackets: ChangeEventTypeType](./literals.md#changeeventtypetype)

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


## DependencyConfigOutputTypeDef

```python
# DependencyConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import DependencyConfigOutputTypeDef


def get_value() -> DependencyConfigOutputTypeDef:
    return {
        "DependencyKeyAttributes": ...,
    }


# DependencyConfigOutputTypeDef definition

class DependencyConfigOutputTypeDef(TypedDict):
    DependencyKeyAttributes: dict[str, str],
    DependencyOperationName: str,
```


## DependencyConfigTypeDef

```python
# DependencyConfigTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import DependencyConfigTypeDef


def get_value() -> DependencyConfigTypeDef:
    return {
        "DependencyKeyAttributes": ...,
    }


# DependencyConfigTypeDef definition

class DependencyConfigTypeDef(TypedDict):
    DependencyKeyAttributes: Mapping[str, str],
    DependencyOperationName: str,
```


## EdgeTypeDef

```python
# EdgeTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import EdgeTypeDef


def get_value() -> EdgeTypeDef:
    return {
        "SourceNodeId": ...,
    }


# EdgeTypeDef definition

class EdgeTypeDef(TypedDict):
    SourceNodeId: NotRequired[str],
    DestinationNodeId: NotRequired[str],
    Duration: NotRequired[float],
    ConnectionType: NotRequired[ConnectionTypeType],  # (1)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype)

## NodeTypeDef

```python
# NodeTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import NodeTypeDef


def get_value() -> NodeTypeDef:
    return {
        "KeyAttributes": ...,
    }


# NodeTypeDef definition

class NodeTypeDef(TypedDict):
    KeyAttributes: dict[str, str],
    Name: str,
    NodeId: str,
    Operation: NotRequired[str],
    Type: NotRequired[str],
    Duration: NotRequired[float],
    Status: NotRequired[str],
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


## RecurrenceRuleTypeDef

```python
# RecurrenceRuleTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import RecurrenceRuleTypeDef


def get_value() -> RecurrenceRuleTypeDef:
    return {
        "Expression": ...,
    }


# RecurrenceRuleTypeDef definition

class RecurrenceRuleTypeDef(TypedDict):
    Expression: str,
```


## WindowTypeDef

```python
# WindowTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import WindowTypeDef


def get_value() -> WindowTypeDef:
    return {
        "DurationUnit": ...,
    }


# WindowTypeDef definition

class WindowTypeDef(TypedDict):
    DurationUnit: DurationUnitType,  # (1)
    Duration: int,
```

1. See [:material-code-brackets: DurationUnitType](./literals.md#durationunittype)

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


## GroupingAttributeDefinitionOutputTypeDef

```python
# GroupingAttributeDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import GroupingAttributeDefinitionOutputTypeDef


def get_value() -> GroupingAttributeDefinitionOutputTypeDef:
    return {
        "GroupingName": ...,
    }


# GroupingAttributeDefinitionOutputTypeDef definition

class GroupingAttributeDefinitionOutputTypeDef(TypedDict):
    GroupingName: str,
    GroupingSourceKeys: NotRequired[list[str]],
    DefaultGroupingValue: NotRequired[str],
```


## GroupingAttributeDefinitionTypeDef

```python
# GroupingAttributeDefinitionTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import GroupingAttributeDefinitionTypeDef


def get_value() -> GroupingAttributeDefinitionTypeDef:
    return {
        "GroupingName": ...,
    }


# GroupingAttributeDefinitionTypeDef definition

class GroupingAttributeDefinitionTypeDef(TypedDict):
    GroupingName: str,
    GroupingSourceKeys: NotRequired[Sequence[str]],
    DefaultGroupingValue: NotRequired[str],
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


## ListGroupingAttributeDefinitionsInputTypeDef

```python
# ListGroupingAttributeDefinitionsInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListGroupingAttributeDefinitionsInputTypeDef


def get_value() -> ListGroupingAttributeDefinitionsInputTypeDef:
    return {
        "NextToken": ...,
    }


# ListGroupingAttributeDefinitionsInputTypeDef definition

class ListGroupingAttributeDefinitionsInputTypeDef(TypedDict):
    NextToken: NotRequired[str],
    AwsAccountId: NotRequired[str],
    IncludeLinkedAccounts: NotRequired[bool],
```


## ListServiceLevelObjectiveExclusionWindowsInputTypeDef

```python
# ListServiceLevelObjectiveExclusionWindowsInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceLevelObjectiveExclusionWindowsInputTypeDef


def get_value() -> ListServiceLevelObjectiveExclusionWindowsInputTypeDef:
    return {
        "Id": ...,
    }


# ListServiceLevelObjectiveExclusionWindowsInputTypeDef definition

class ListServiceLevelObjectiveExclusionWindowsInputTypeDef(TypedDict):
    Id: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
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


## ServiceGroupTypeDef

```python
# ServiceGroupTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceGroupTypeDef


def get_value() -> ServiceGroupTypeDef:
    return {
        "GroupName": ...,
    }


# ServiceGroupTypeDef definition

class ServiceGroupTypeDef(TypedDict):
    GroupName: str,
    GroupValue: str,
    GroupSource: str,
    GroupIdentifier: str,
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


## ServiceOperationEntityTypeDef

```python
# ServiceOperationEntityTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceOperationEntityTypeDef


def get_value() -> ServiceOperationEntityTypeDef:
    return {
        "Service": ...,
    }


# ServiceOperationEntityTypeDef definition

class ServiceOperationEntityTypeDef(TypedDict):
    Service: NotRequired[ServiceEntityTypeDef],  # (1)
    Operation: NotRequired[str],
    MetricType: NotRequired[str],
```

1. See [:material-code-braces: ServiceEntityTypeDef](./type_defs.md#serviceentitytypedef)

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


## ListEntityEventsInputTypeDef

```python
# ListEntityEventsInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListEntityEventsInputTypeDef


def get_value() -> ListEntityEventsInputTypeDef:
    return {
        "Entity": ...,
    }


# ListEntityEventsInputTypeDef definition

class ListEntityEventsInputTypeDef(TypedDict):
    Entity: Mapping[str, str],
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
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
    IncludeLinkedAccounts: NotRequired[bool],
    AwsAccountId: NotRequired[str],
```


## BatchUpdateExclusionWindowsOutputTypeDef

```python
# BatchUpdateExclusionWindowsOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import BatchUpdateExclusionWindowsOutputTypeDef


def get_value() -> BatchUpdateExclusionWindowsOutputTypeDef:
    return {
        "SloIds": ...,
    }


# BatchUpdateExclusionWindowsOutputTypeDef definition

class BatchUpdateExclusionWindowsOutputTypeDef(TypedDict):
    SloIds: list[str],
    Errors: list[BatchUpdateExclusionWindowsErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `list[BatchUpdateExclusionWindowsErrorTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListEntityEventsOutputTypeDef

```python
# ListEntityEventsOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListEntityEventsOutputTypeDef


def get_value() -> ListEntityEventsOutputTypeDef:
    return {
        "StartTime": ...,
    }


# ListEntityEventsOutputTypeDef definition

class ListEntityEventsOutputTypeDef(TypedDict):
    StartTime: datetime.datetime,
    EndTime: datetime.datetime,
    ChangeEvents: list[ChangeEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[ChangeEventTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ServiceStateTypeDef

```python
# ServiceStateTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ServiceStateTypeDef


def get_value() -> ServiceStateTypeDef:
    return {
        "AttributeFilters": ...,
    }


# ServiceStateTypeDef definition

class ServiceStateTypeDef(TypedDict):
    Service: dict[str, str],
    LatestChangeEvents: list[ChangeEventTypeDef],  # (2)
    AttributeFilters: NotRequired[list[AttributeFilterOutputTypeDef]],  # (1)
```

1. See `list[AttributeFilterOutputTypeDef]`
2. See `list[ChangeEventTypeDef]`

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
    Tags: list[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `list[TagTypeDef]`
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

1. See `Sequence[TagTypeDef]`

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
    KeyAttributes: NotRequired[dict[str, str]],
    OperationName: NotRequired[str],
    DependencyConfig: NotRequired[DependencyConfigOutputTypeDef],  # (1)
    CreatedTime: NotRequired[datetime.datetime],
    EvaluationType: NotRequired[EvaluationTypeType],  # (2)
    MetricSourceType: NotRequired[MetricSourceTypeType],  # (3)
```

1. See [:material-code-braces: DependencyConfigOutputTypeDef](./type_defs.md#dependencyconfigoutputtypedef)
2. See [:material-code-brackets: EvaluationTypeType](./literals.md#evaluationtypetype)
3. See [:material-code-brackets: MetricSourceTypeType](./literals.md#metricsourcetypetype)

## DependencyGraphTypeDef

```python
# DependencyGraphTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import DependencyGraphTypeDef


def get_value() -> DependencyGraphTypeDef:
    return {
        "Nodes": ...,
    }


# DependencyGraphTypeDef definition

class DependencyGraphTypeDef(TypedDict):
    Nodes: NotRequired[list[NodeTypeDef]],  # (1)
    Edges: NotRequired[list[EdgeTypeDef]],  # (2)
```

1. See `list[NodeTypeDef]`
2. See `list[EdgeTypeDef]`

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
    Dimensions: NotRequired[list[DimensionTypeDef]],  # (1)
```

1. See `list[DimensionTypeDef]`

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
    Dimensions: NotRequired[list[DimensionTypeDef]],  # (1)
    AccountId: NotRequired[str],
```

1. See `list[DimensionTypeDef]`

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

1. See `Sequence[DimensionTypeDef]`

## ExclusionWindowOutputTypeDef

```python
# ExclusionWindowOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ExclusionWindowOutputTypeDef


def get_value() -> ExclusionWindowOutputTypeDef:
    return {
        "Window": ...,
    }


# ExclusionWindowOutputTypeDef definition

class ExclusionWindowOutputTypeDef(TypedDict):
    Window: WindowTypeDef,  # (1)
    StartTime: NotRequired[datetime.datetime],
    RecurrenceRule: NotRequired[RecurrenceRuleTypeDef],  # (2)
    Reason: NotRequired[str],
```

1. See [:material-code-braces: WindowTypeDef](./type_defs.md#windowtypedef)
2. See [:material-code-braces: RecurrenceRuleTypeDef](./type_defs.md#recurrenceruletypedef)

## ExclusionWindowTypeDef

```python
# ExclusionWindowTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ExclusionWindowTypeDef


def get_value() -> ExclusionWindowTypeDef:
    return {
        "Window": ...,
    }


# ExclusionWindowTypeDef definition

class ExclusionWindowTypeDef(TypedDict):
    Window: WindowTypeDef,  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    RecurrenceRule: NotRequired[RecurrenceRuleTypeDef],  # (2)
    Reason: NotRequired[str],
```

1. See [:material-code-braces: WindowTypeDef](./type_defs.md#windowtypedef)
2. See [:material-code-braces: RecurrenceRuleTypeDef](./type_defs.md#recurrenceruletypedef)

## GroupingConfigurationTypeDef

```python
# GroupingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import GroupingConfigurationTypeDef


def get_value() -> GroupingConfigurationTypeDef:
    return {
        "GroupingAttributeDefinitions": ...,
    }


# GroupingConfigurationTypeDef definition

class GroupingConfigurationTypeDef(TypedDict):
    GroupingAttributeDefinitions: list[GroupingAttributeDefinitionOutputTypeDef],  # (1)
    UpdatedAt: datetime.datetime,
```

1. See `list[GroupingAttributeDefinitionOutputTypeDef]`

## ListGroupingAttributeDefinitionsOutputTypeDef

```python
# ListGroupingAttributeDefinitionsOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListGroupingAttributeDefinitionsOutputTypeDef


def get_value() -> ListGroupingAttributeDefinitionsOutputTypeDef:
    return {
        "GroupingAttributeDefinitions": ...,
    }


# ListGroupingAttributeDefinitionsOutputTypeDef definition

class ListGroupingAttributeDefinitionsOutputTypeDef(TypedDict):
    GroupingAttributeDefinitions: list[GroupingAttributeDefinitionOutputTypeDef],  # (1)
    UpdatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[GroupingAttributeDefinitionOutputTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

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

## ListEntityEventsInputPaginateTypeDef

```python
# ListEntityEventsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListEntityEventsInputPaginateTypeDef


def get_value() -> ListEntityEventsInputPaginateTypeDef:
    return {
        "Entity": ...,
    }


# ListEntityEventsInputPaginateTypeDef definition

class ListEntityEventsInputPaginateTypeDef(TypedDict):
    Entity: Mapping[str, str],
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

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

## ListServiceLevelObjectiveExclusionWindowsInputPaginateTypeDef

```python
# ListServiceLevelObjectiveExclusionWindowsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceLevelObjectiveExclusionWindowsInputPaginateTypeDef


def get_value() -> ListServiceLevelObjectiveExclusionWindowsInputPaginateTypeDef:
    return {
        "Id": ...,
    }


# ListServiceLevelObjectiveExclusionWindowsInputPaginateTypeDef definition

class ListServiceLevelObjectiveExclusionWindowsInputPaginateTypeDef(TypedDict):
    Id: str,
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
    IncludeLinkedAccounts: NotRequired[bool],
    AwsAccountId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListServiceStatesInputPaginateTypeDef

```python
# ListServiceStatesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceStatesInputPaginateTypeDef


def get_value() -> ListServiceStatesInputPaginateTypeDef:
    return {
        "StartTime": ...,
    }


# ListServiceStatesInputPaginateTypeDef definition

class ListServiceStatesInputPaginateTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    IncludeLinkedAccounts: NotRequired[bool],
    AwsAccountId: NotRequired[str],
    AttributeFilters: NotRequired[Sequence[AttributeFilterUnionTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See `Sequence[AttributeFilterUnionTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListServiceStatesInputTypeDef

```python
# ListServiceStatesInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceStatesInputTypeDef


def get_value() -> ListServiceStatesInputTypeDef:
    return {
        "StartTime": ...,
    }


# ListServiceStatesInputTypeDef definition

class ListServiceStatesInputTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    IncludeLinkedAccounts: NotRequired[bool],
    AwsAccountId: NotRequired[str],
    AttributeFilters: NotRequired[Sequence[AttributeFilterUnionTypeDef]],  # (1)
```

1. See `Sequence[AttributeFilterUnionTypeDef]`

## AuditTargetEntityTypeDef

```python
# AuditTargetEntityTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import AuditTargetEntityTypeDef


def get_value() -> AuditTargetEntityTypeDef:
    return {
        "Service": ...,
    }


# AuditTargetEntityTypeDef definition

class AuditTargetEntityTypeDef(TypedDict):
    Service: NotRequired[ServiceEntityTypeDef],  # (1)
    Slo: NotRequired[ServiceLevelObjectiveEntityTypeDef],  # (2)
    ServiceOperation: NotRequired[ServiceOperationEntityTypeDef],  # (3)
    Canary: NotRequired[CanaryEntityTypeDef],  # (4)
```

1. See [:material-code-braces: ServiceEntityTypeDef](./type_defs.md#serviceentitytypedef)
2. See [:material-code-braces: ServiceLevelObjectiveEntityTypeDef](./type_defs.md#servicelevelobjectiveentitytypedef)
3. See [:material-code-braces: ServiceOperationEntityTypeDef](./type_defs.md#serviceoperationentitytypedef)
4. See [:material-code-braces: CanaryEntityTypeDef](./type_defs.md#canaryentitytypedef)

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

## ListServiceStatesOutputTypeDef

```python
# ListServiceStatesOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceStatesOutputTypeDef


def get_value() -> ListServiceStatesOutputTypeDef:
    return {
        "StartTime": ...,
    }


# ListServiceStatesOutputTypeDef definition

class ListServiceStatesOutputTypeDef(TypedDict):
    StartTime: datetime.datetime,
    EndTime: datetime.datetime,
    ServiceStates: list[ServiceStateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[ServiceStateTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

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
    SloSummaries: list[ServiceLevelObjectiveSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[ServiceLevelObjectiveSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

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
    DependencyConfig: NotRequired[DependencyConfigUnionTypeDef],  # (1)
    IncludeLinkedAccounts: NotRequired[bool],
    SloOwnerAwsAccountId: NotRequired[str],
    MetricSourceTypes: NotRequired[Sequence[MetricSourceTypeType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: DependencyConfigUnionTypeDef](#dependencyconfiguniontypedef)
2. See `Sequence[MetricSourceTypeType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

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
    DependencyConfig: NotRequired[DependencyConfigUnionTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    IncludeLinkedAccounts: NotRequired[bool],
    SloOwnerAwsAccountId: NotRequired[str],
    MetricSourceTypes: NotRequired[Sequence[MetricSourceTypeType]],  # (2)
```

1. See [:material-code-braces: DependencyConfigUnionTypeDef](#dependencyconfiguniontypedef)
2. See `Sequence[MetricSourceTypeType]`

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
    DependencyKeyAttributes: dict[str, str],
    DependencyOperationName: str,
    MetricReferences: list[MetricReferenceTypeDef],  # (1)
```

1. See `list[MetricReferenceTypeDef]`

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
    DependentKeyAttributes: dict[str, str],
    MetricReferences: list[MetricReferenceTypeDef],  # (1)
    OperationName: NotRequired[str],
    DependentOperationName: NotRequired[str],
```

1. See `list[MetricReferenceTypeDef]`

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
    MetricReferences: list[MetricReferenceTypeDef],  # (1)
```

1. See `list[MetricReferenceTypeDef]`

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
    KeyAttributes: dict[str, str],
    MetricReferences: list[MetricReferenceTypeDef],  # (1)
    AttributeMaps: NotRequired[list[dict[str, str]]],
    ServiceGroups: NotRequired[list[ServiceGroupTypeDef]],  # (2)
```

1. See `list[MetricReferenceTypeDef]`
2. See `list[ServiceGroupTypeDef]`

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
    KeyAttributes: dict[str, str],
    MetricReferences: list[MetricReferenceTypeDef],  # (2)
    AttributeMaps: NotRequired[list[dict[str, str]]],
    ServiceGroups: NotRequired[list[ServiceGroupTypeDef]],  # (1)
    LogGroupReferences: NotRequired[list[dict[str, str]]],
```

1. See `list[ServiceGroupTypeDef]`
2. See `list[MetricReferenceTypeDef]`

## ListServiceLevelObjectiveExclusionWindowsOutputTypeDef

```python
# ListServiceLevelObjectiveExclusionWindowsOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListServiceLevelObjectiveExclusionWindowsOutputTypeDef


def get_value() -> ListServiceLevelObjectiveExclusionWindowsOutputTypeDef:
    return {
        "ExclusionWindows": ...,
    }


# ListServiceLevelObjectiveExclusionWindowsOutputTypeDef definition

class ListServiceLevelObjectiveExclusionWindowsOutputTypeDef(TypedDict):
    ExclusionWindows: list[ExclusionWindowOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[ExclusionWindowOutputTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## PutGroupingConfigurationOutputTypeDef

```python
# PutGroupingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import PutGroupingConfigurationOutputTypeDef


def get_value() -> PutGroupingConfigurationOutputTypeDef:
    return {
        "GroupingConfiguration": ...,
    }


# PutGroupingConfigurationOutputTypeDef definition

class PutGroupingConfigurationOutputTypeDef(TypedDict):
    GroupingConfiguration: GroupingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## PutGroupingConfigurationInputTypeDef

```python
# PutGroupingConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import PutGroupingConfigurationInputTypeDef


def get_value() -> PutGroupingConfigurationInputTypeDef:
    return {
        "GroupingAttributeDefinitions": ...,
    }


# PutGroupingConfigurationInputTypeDef definition

class PutGroupingConfigurationInputTypeDef(TypedDict):
    GroupingAttributeDefinitions: Sequence[GroupingAttributeDefinitionUnionTypeDef],  # (1)
```

1. See `Sequence[GroupingAttributeDefinitionUnionTypeDef]`

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

## AuditTargetTypeDef

```python
# AuditTargetTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import AuditTargetTypeDef


def get_value() -> AuditTargetTypeDef:
    return {
        "Type": ...,
    }


# AuditTargetTypeDef definition

class AuditTargetTypeDef(TypedDict):
    Type: str,
    Data: AuditTargetEntityTypeDef,  # (1)
```

1. See [:material-code-braces: AuditTargetEntityTypeDef](./type_defs.md#audittargetentitytypedef)

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
    StartTime: datetime.datetime,
    EndTime: datetime.datetime,
    ServiceDependencies: list[ServiceDependencyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[ServiceDependencyTypeDef]`
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
    StartTime: datetime.datetime,
    EndTime: datetime.datetime,
    ServiceDependents: list[ServiceDependentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[ServiceDependentTypeDef]`
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
    StartTime: datetime.datetime,
    EndTime: datetime.datetime,
    ServiceOperations: list[ServiceOperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[ServiceOperationTypeDef]`
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
    StartTime: datetime.datetime,
    EndTime: datetime.datetime,
    ServiceSummaries: list[ServiceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[ServiceSummaryTypeDef]`
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
    StartTime: datetime.datetime,
    EndTime: datetime.datetime,
    LogGroupReferences: list[dict[str, str]],
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

1. See [:material-code-braces: MetricUnionTypeDef](#metricuniontypedef)
2. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype)

## BatchUpdateExclusionWindowsInputTypeDef

```python
# BatchUpdateExclusionWindowsInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import BatchUpdateExclusionWindowsInputTypeDef


def get_value() -> BatchUpdateExclusionWindowsInputTypeDef:
    return {
        "SloIds": ...,
    }


# BatchUpdateExclusionWindowsInputTypeDef definition

class BatchUpdateExclusionWindowsInputTypeDef(TypedDict):
    SloIds: Sequence[str],
    AddExclusionWindows: NotRequired[Sequence[ExclusionWindowUnionTypeDef]],  # (1)
    RemoveExclusionWindows: NotRequired[Sequence[ExclusionWindowUnionTypeDef]],  # (1)
```

1. See `Sequence[ExclusionWindowUnionTypeDef]`
2. See `Sequence[ExclusionWindowUnionTypeDef]`

## ListAuditFindingsInputTypeDef

```python
# ListAuditFindingsInputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListAuditFindingsInputTypeDef


def get_value() -> ListAuditFindingsInputTypeDef:
    return {
        "StartTime": ...,
    }


# ListAuditFindingsInputTypeDef definition

class ListAuditFindingsInputTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    AuditTargets: Sequence[AuditTargetTypeDef],  # (1)
    Auditors: NotRequired[Sequence[str]],
    DetailLevel: NotRequired[DetailLevelType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See `Sequence[AuditTargetTypeDef]`
2. See [:material-code-brackets: DetailLevelType](./literals.md#detailleveltype)

## MetricGraphTypeDef

```python
# MetricGraphTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import MetricGraphTypeDef


def get_value() -> MetricGraphTypeDef:
    return {
        "MetricDataQueries": ...,
    }


# MetricGraphTypeDef definition

class MetricGraphTypeDef(TypedDict):
    MetricDataQueries: NotRequired[list[MetricDataQueryOutputTypeDef]],  # (1)
    StartTime: NotRequired[datetime.datetime],
    EndTime: NotRequired[datetime.datetime],
```

1. See `list[MetricDataQueryOutputTypeDef]`

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
    GoodCountMetric: NotRequired[list[MetricDataQueryOutputTypeDef]],  # (1)
    BadCountMetric: NotRequired[list[MetricDataQueryOutputTypeDef]],  # (1)
```

1. See `list[MetricDataQueryOutputTypeDef]`
2. See `list[MetricDataQueryOutputTypeDef]`

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
    MetricDataQueries: list[MetricDataQueryOutputTypeDef],  # (2)
    KeyAttributes: NotRequired[dict[str, str]],
    OperationName: NotRequired[str],
    MetricType: NotRequired[ServiceLevelIndicatorMetricTypeType],  # (1)
    DependencyConfig: NotRequired[DependencyConfigOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: ServiceLevelIndicatorMetricTypeType](./literals.md#servicelevelindicatormetrictypetype)
2. See `list[MetricDataQueryOutputTypeDef]`
3. See [:material-code-braces: DependencyConfigOutputTypeDef](./type_defs.md#dependencyconfigoutputtypedef)

## AuditFindingTypeDef

```python
# AuditFindingTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import AuditFindingTypeDef


def get_value() -> AuditFindingTypeDef:
    return {
        "KeyAttributes": ...,
    }


# AuditFindingTypeDef definition

class AuditFindingTypeDef(TypedDict):
    KeyAttributes: dict[str, str],
    AuditorResults: NotRequired[list[AuditorResultTypeDef]],  # (1)
    Operation: NotRequired[str],
    MetricGraph: NotRequired[MetricGraphTypeDef],  # (2)
    DependencyGraph: NotRequired[DependencyGraphTypeDef],  # (3)
    Type: NotRequired[str],
```

1. See `list[AuditorResultTypeDef]`
2. See [:material-code-braces: MetricGraphTypeDef](./type_defs.md#metricgraphtypedef)
3. See [:material-code-braces: DependencyGraphTypeDef](./type_defs.md#dependencygraphtypedef)

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
    TotalRequestCountMetric: list[MetricDataQueryOutputTypeDef],  # (2)
    MonitoredRequestCountMetric: MonitoredRequestCountMetricDataQueriesOutputTypeDef,  # (3)
    KeyAttributes: NotRequired[dict[str, str]],
    OperationName: NotRequired[str],
    MetricType: NotRequired[ServiceLevelIndicatorMetricTypeType],  # (1)
    DependencyConfig: NotRequired[DependencyConfigOutputTypeDef],  # (4)
```

1. See [:material-code-brackets: ServiceLevelIndicatorMetricTypeType](./literals.md#servicelevelindicatormetrictypetype)
2. See `list[MetricDataQueryOutputTypeDef]`
3. See [:material-code-braces: MonitoredRequestCountMetricDataQueriesOutputTypeDef](./type_defs.md#monitoredrequestcountmetricdataqueriesoutputtypedef)
4. See [:material-code-braces: DependencyConfigOutputTypeDef](./type_defs.md#dependencyconfigoutputtypedef)

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

1. See [:material-code-braces: MetricStatUnionTypeDef](#metricstatuniontypedef)

## ListAuditFindingsOutputTypeDef

```python
# ListAuditFindingsOutputTypeDef TypedDict usage example

from types_aiobotocore_application_signals.type_defs import ListAuditFindingsOutputTypeDef


def get_value() -> ListAuditFindingsOutputTypeDef:
    return {
        "StartTime": ...,
    }


# ListAuditFindingsOutputTypeDef definition

class ListAuditFindingsOutputTypeDef(TypedDict):
    StartTime: datetime.datetime,
    EndTime: datetime.datetime,
    AuditFindings: list[AuditFindingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `list[AuditFindingTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

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
    CreatedTime: datetime.datetime,
    LastUpdatedTime: datetime.datetime,
    Goal: GoalOutputTypeDef,  # (4)
    Description: NotRequired[str],
    Sli: NotRequired[ServiceLevelIndicatorTypeDef],  # (1)
    RequestBasedSli: NotRequired[RequestBasedServiceLevelIndicatorTypeDef],  # (2)
    EvaluationType: NotRequired[EvaluationTypeType],  # (3)
    BurnRateConfigurations: NotRequired[list[BurnRateConfigurationTypeDef]],  # (5)
    MetricSourceType: NotRequired[MetricSourceTypeType],  # (6)
```

1. See [:material-code-braces: ServiceLevelIndicatorTypeDef](./type_defs.md#servicelevelindicatortypedef)
2. See [:material-code-braces: RequestBasedServiceLevelIndicatorTypeDef](./type_defs.md#requestbasedservicelevelindicatortypedef)
3. See [:material-code-brackets: EvaluationTypeType](./literals.md#evaluationtypetype)
4. See [:material-code-braces: GoalOutputTypeDef](./type_defs.md#goaloutputtypedef)
5. See `list[BurnRateConfigurationTypeDef]`
6. See [:material-code-brackets: MetricSourceTypeType](./literals.md#metricsourcetypetype)

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

1. See `Sequence[MetricDataQueryUnionTypeDef]`
2. See `Sequence[MetricDataQueryTypeDef]`

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
    MetricName: NotRequired[str],
    Statistic: NotRequired[str],
    PeriodSeconds: NotRequired[int],
    MetricDataQueries: NotRequired[Sequence[MetricDataQueryUnionTypeDef]],  # (2)
    DependencyConfig: NotRequired[DependencyConfigUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: ServiceLevelIndicatorMetricTypeType](./literals.md#servicelevelindicatormetrictypetype)
2. See `Sequence[MetricDataQueryUnionTypeDef]`
3. See [:material-code-braces: DependencyConfigUnionTypeDef](#dependencyconfiguniontypedef)

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
    Timestamp: datetime.datetime,
    Reports: list[ServiceLevelObjectiveBudgetReportTypeDef],  # (1)
    Errors: list[ServiceLevelObjectiveBudgetReportErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See `list[ServiceLevelObjectiveBudgetReportTypeDef]`
2. See `list[ServiceLevelObjectiveBudgetReportErrorTypeDef]`
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
    DependencyConfig: NotRequired[DependencyConfigUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: ServiceLevelIndicatorMetricTypeType](./literals.md#servicelevelindicatormetrictypetype)
2. See `Sequence[MetricDataQueryUnionTypeDef]`
3. See [:material-code-braces: MonitoredRequestCountMetricDataQueriesUnionTypeDef](#monitoredrequestcountmetricdataqueriesuniontypedef)
4. See [:material-code-braces: DependencyConfigUnionTypeDef](#dependencyconfiguniontypedef)

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
3. See [:material-code-braces: GoalUnionTypeDef](#goaluniontypedef)
4. See `Sequence[TagTypeDef]`
5. See `Sequence[BurnRateConfigurationTypeDef]`

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
3. See [:material-code-braces: GoalUnionTypeDef](#goaluniontypedef)
4. See `Sequence[BurnRateConfigurationTypeDef]`

