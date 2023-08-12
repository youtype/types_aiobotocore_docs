# Type definitions

> [Index](../README.md) > [CloudWatchRUM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchRUM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
    type annotations stubs module [types-aiobotocore-rum](https://pypi.org/project/types-aiobotocore-rum/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AppMonitorConfigurationTypeDef

```python
# AppMonitorConfigurationTypeDef definition

class AppMonitorConfigurationTypeDef(TypedDict):
    AllowCookies: NotRequired[bool],
    EnableXRay: NotRequired[bool],
    ExcludedPages: NotRequired[Sequence[str]],
    FavoritePages: NotRequired[Sequence[str]],
    GuestRoleArn: NotRequired[str],
    IdentityPoolId: NotRequired[str],
    IncludedPages: NotRequired[Sequence[str]],
    SessionSampleRate: NotRequired[float],
    Telemetries: NotRequired[Sequence[TelemetryType]],  # (1)
```

1. See [:material-code-brackets: TelemetryType](./literals.md#telemetrytype) 
## AppMonitorDetailsTypeDef

```python
# AppMonitorDetailsTypeDef definition

class AppMonitorDetailsTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    version: NotRequired[str],
```

## AppMonitorSummaryTypeDef

```python
# AppMonitorSummaryTypeDef definition

class AppMonitorSummaryTypeDef(TypedDict):
    Created: NotRequired[str],
    Id: NotRequired[str],
    LastModified: NotRequired[str],
    Name: NotRequired[str],
    State: NotRequired[StateEnumType],  # (1)
```

1. See [:material-code-brackets: StateEnumType](./literals.md#stateenumtype) 
## CustomEventsTypeDef

```python
# CustomEventsTypeDef definition

class CustomEventsTypeDef(TypedDict):
    Status: NotRequired[CustomEventsStatusType],  # (1)
```

1. See [:material-code-brackets: CustomEventsStatusType](./literals.md#customeventsstatustype) 
## MetricDefinitionRequestTypeDef

```python
# MetricDefinitionRequestTypeDef definition

class MetricDefinitionRequestTypeDef(TypedDict):
    Name: str,
    DimensionKeys: NotRequired[Mapping[str, str]],
    EventPattern: NotRequired[str],
    Namespace: NotRequired[str],
    UnitLabel: NotRequired[str],
    ValueKey: NotRequired[str],
```

## MetricDefinitionTypeDef

```python
# MetricDefinitionTypeDef definition

class MetricDefinitionTypeDef(TypedDict):
    MetricDefinitionId: str,
    Name: str,
    DimensionKeys: NotRequired[Dict[str, str]],
    EventPattern: NotRequired[str],
    Namespace: NotRequired[str],
    UnitLabel: NotRequired[str],
    ValueKey: NotRequired[str],
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

## BatchDeleteRumMetricDefinitionsErrorTypeDef

```python
# BatchDeleteRumMetricDefinitionsErrorTypeDef definition

class BatchDeleteRumMetricDefinitionsErrorTypeDef(TypedDict):
    ErrorCode: str,
    ErrorMessage: str,
    MetricDefinitionId: str,
```

## BatchDeleteRumMetricDefinitionsRequestRequestTypeDef

```python
# BatchDeleteRumMetricDefinitionsRequestRequestTypeDef definition

class BatchDeleteRumMetricDefinitionsRequestRequestTypeDef(TypedDict):
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    MetricDefinitionIds: Sequence[str],
    DestinationArn: NotRequired[str],
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## BatchGetRumMetricDefinitionsRequestRequestTypeDef

```python
# BatchGetRumMetricDefinitionsRequestRequestTypeDef definition

class BatchGetRumMetricDefinitionsRequestRequestTypeDef(TypedDict):
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    DestinationArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
## CwLogTypeDef

```python
# CwLogTypeDef definition

class CwLogTypeDef(TypedDict):
    CwLogEnabled: NotRequired[bool],
    CwLogGroup: NotRequired[str],
```

## DeleteAppMonitorRequestRequestTypeDef

```python
# DeleteAppMonitorRequestRequestTypeDef definition

class DeleteAppMonitorRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteRumMetricsDestinationRequestRequestTypeDef

```python
# DeleteRumMetricsDestinationRequestRequestTypeDef definition

class DeleteRumMetricsDestinationRequestRequestTypeDef(TypedDict):
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    DestinationArn: NotRequired[str],
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
## QueryFilterTypeDef

```python
# QueryFilterTypeDef definition

class QueryFilterTypeDef(TypedDict):
    Name: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## TimeRangeTypeDef

```python
# TimeRangeTypeDef definition

class TimeRangeTypeDef(TypedDict):
    After: int,
    Before: NotRequired[int],
```

## GetAppMonitorRequestRequestTypeDef

```python
# GetAppMonitorRequestRequestTypeDef definition

class GetAppMonitorRequestRequestTypeDef(TypedDict):
    Name: str,
```

## ListAppMonitorsRequestRequestTypeDef

```python
# ListAppMonitorsRequestRequestTypeDef definition

class ListAppMonitorsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListRumMetricsDestinationsRequestRequestTypeDef

```python
# ListRumMetricsDestinationsRequestRequestTypeDef definition

class ListRumMetricsDestinationsRequestRequestTypeDef(TypedDict):
    AppMonitorName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## MetricDestinationSummaryTypeDef

```python
# MetricDestinationSummaryTypeDef definition

class MetricDestinationSummaryTypeDef(TypedDict):
    Destination: NotRequired[MetricDestinationType],  # (1)
    DestinationArn: NotRequired[str],
    IamRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## UserDetailsTypeDef

```python
# UserDetailsTypeDef definition

class UserDetailsTypeDef(TypedDict):
    sessionId: NotRequired[str],
    userId: NotRequired[str],
```

## PutRumMetricsDestinationRequestRequestTypeDef

```python
# PutRumMetricsDestinationRequestRequestTypeDef definition

class PutRumMetricsDestinationRequestRequestTypeDef(TypedDict):
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    DestinationArn: NotRequired[str],
    IamRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## CreateAppMonitorRequestRequestTypeDef

```python
# CreateAppMonitorRequestRequestTypeDef definition

class CreateAppMonitorRequestRequestTypeDef(TypedDict):
    Domain: str,
    Name: str,
    AppMonitorConfiguration: NotRequired[AppMonitorConfigurationTypeDef],  # (1)
    CustomEvents: NotRequired[CustomEventsTypeDef],  # (2)
    CwLogEnabled: NotRequired[bool],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AppMonitorConfigurationTypeDef](./type_defs.md#appmonitorconfigurationtypedef) 
2. See [:material-code-braces: CustomEventsTypeDef](./type_defs.md#customeventstypedef) 
## UpdateAppMonitorRequestRequestTypeDef

```python
# UpdateAppMonitorRequestRequestTypeDef definition

class UpdateAppMonitorRequestRequestTypeDef(TypedDict):
    Name: str,
    AppMonitorConfiguration: NotRequired[AppMonitorConfigurationTypeDef],  # (1)
    CustomEvents: NotRequired[CustomEventsTypeDef],  # (2)
    CwLogEnabled: NotRequired[bool],
    Domain: NotRequired[str],
```

1. See [:material-code-braces: AppMonitorConfigurationTypeDef](./type_defs.md#appmonitorconfigurationtypedef) 
2. See [:material-code-braces: CustomEventsTypeDef](./type_defs.md#customeventstypedef) 
## BatchCreateRumMetricDefinitionsErrorTypeDef

```python
# BatchCreateRumMetricDefinitionsErrorTypeDef definition

class BatchCreateRumMetricDefinitionsErrorTypeDef(TypedDict):
    ErrorCode: str,
    ErrorMessage: str,
    MetricDefinition: MetricDefinitionRequestTypeDef,  # (1)
```

1. See [:material-code-braces: MetricDefinitionRequestTypeDef](./type_defs.md#metricdefinitionrequesttypedef) 
## BatchCreateRumMetricDefinitionsRequestRequestTypeDef

```python
# BatchCreateRumMetricDefinitionsRequestRequestTypeDef definition

class BatchCreateRumMetricDefinitionsRequestRequestTypeDef(TypedDict):
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    MetricDefinitions: Sequence[MetricDefinitionRequestTypeDef],  # (2)
    DestinationArn: NotRequired[str],
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
2. See [:material-code-braces: MetricDefinitionRequestTypeDef](./type_defs.md#metricdefinitionrequesttypedef) 
## UpdateRumMetricDefinitionRequestRequestTypeDef

```python
# UpdateRumMetricDefinitionRequestRequestTypeDef definition

class UpdateRumMetricDefinitionRequestRequestTypeDef(TypedDict):
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    MetricDefinition: MetricDefinitionRequestTypeDef,  # (2)
    MetricDefinitionId: str,
    DestinationArn: NotRequired[str],
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
2. See [:material-code-braces: MetricDefinitionRequestTypeDef](./type_defs.md#metricdefinitionrequesttypedef) 
## BatchGetRumMetricDefinitionsResponseTypeDef

```python
# BatchGetRumMetricDefinitionsResponseTypeDef definition

class BatchGetRumMetricDefinitionsResponseTypeDef(TypedDict):
    MetricDefinitions: List[MetricDefinitionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppMonitorResponseTypeDef

```python
# CreateAppMonitorResponseTypeDef definition

class CreateAppMonitorResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppMonitorDataResponseTypeDef

```python
# GetAppMonitorDataResponseTypeDef definition

class GetAppMonitorDataResponseTypeDef(TypedDict):
    Events: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppMonitorsResponseTypeDef

```python
# ListAppMonitorsResponseTypeDef definition

class ListAppMonitorsResponseTypeDef(TypedDict):
    AppMonitorSummaries: List[AppMonitorSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppMonitorSummaryTypeDef](./type_defs.md#appmonitorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteRumMetricDefinitionsResponseTypeDef

```python
# BatchDeleteRumMetricDefinitionsResponseTypeDef definition

class BatchDeleteRumMetricDefinitionsResponseTypeDef(TypedDict):
    Errors: List[BatchDeleteRumMetricDefinitionsErrorTypeDef],  # (1)
    MetricDefinitionIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteRumMetricDefinitionsErrorTypeDef](./type_defs.md#batchdeleterummetricdefinitionserrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef

```python
# BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef definition

class BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef(TypedDict):
    AppMonitorName: str,
    Destination: MetricDestinationType,  # (1)
    DestinationArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: MetricDestinationType](./literals.md#metricdestinationtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAppMonitorsRequestListAppMonitorsPaginateTypeDef

```python
# ListAppMonitorsRequestListAppMonitorsPaginateTypeDef definition

class ListAppMonitorsRequestListAppMonitorsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef

```python
# ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef definition

class ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef(TypedDict):
    AppMonitorName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DataStorageTypeDef

```python
# DataStorageTypeDef definition

class DataStorageTypeDef(TypedDict):
    CwLog: NotRequired[CwLogTypeDef],  # (1)
```

1. See [:material-code-braces: CwLogTypeDef](./type_defs.md#cwlogtypedef) 
## GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef

```python
# GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef definition

class GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef(TypedDict):
    Name: str,
    TimeRange: TimeRangeTypeDef,  # (1)
    Filters: NotRequired[Sequence[QueryFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
2. See [:material-code-braces: QueryFilterTypeDef](./type_defs.md#queryfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetAppMonitorDataRequestRequestTypeDef

```python
# GetAppMonitorDataRequestRequestTypeDef definition

class GetAppMonitorDataRequestRequestTypeDef(TypedDict):
    Name: str,
    TimeRange: TimeRangeTypeDef,  # (1)
    Filters: NotRequired[Sequence[QueryFilterTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
2. See [:material-code-braces: QueryFilterTypeDef](./type_defs.md#queryfiltertypedef) 
## ListRumMetricsDestinationsResponseTypeDef

```python
# ListRumMetricsDestinationsResponseTypeDef definition

class ListRumMetricsDestinationsResponseTypeDef(TypedDict):
    Destinations: List[MetricDestinationSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricDestinationSummaryTypeDef](./type_defs.md#metricdestinationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RumEventTypeDef

```python
# RumEventTypeDef definition

class RumEventTypeDef(TypedDict):
    details: str,
    id: str,
    timestamp: Union[datetime, str],
    type: str,
    metadata: NotRequired[str],
```

## BatchCreateRumMetricDefinitionsResponseTypeDef

```python
# BatchCreateRumMetricDefinitionsResponseTypeDef definition

class BatchCreateRumMetricDefinitionsResponseTypeDef(TypedDict):
    Errors: List[BatchCreateRumMetricDefinitionsErrorTypeDef],  # (1)
    MetricDefinitions: List[MetricDefinitionTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchCreateRumMetricDefinitionsErrorTypeDef](./type_defs.md#batchcreaterummetricdefinitionserrortypedef) 
2. See [:material-code-braces: MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AppMonitorTypeDef

```python
# AppMonitorTypeDef definition

class AppMonitorTypeDef(TypedDict):
    AppMonitorConfiguration: NotRequired[AppMonitorConfigurationTypeDef],  # (1)
    Created: NotRequired[str],
    CustomEvents: NotRequired[CustomEventsTypeDef],  # (2)
    DataStorage: NotRequired[DataStorageTypeDef],  # (3)
    Domain: NotRequired[str],
    Id: NotRequired[str],
    LastModified: NotRequired[str],
    Name: NotRequired[str],
    State: NotRequired[StateEnumType],  # (4)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AppMonitorConfigurationTypeDef](./type_defs.md#appmonitorconfigurationtypedef) 
2. See [:material-code-braces: CustomEventsTypeDef](./type_defs.md#customeventstypedef) 
3. See [:material-code-braces: DataStorageTypeDef](./type_defs.md#datastoragetypedef) 
4. See [:material-code-brackets: StateEnumType](./literals.md#stateenumtype) 
## PutRumEventsRequestRequestTypeDef

```python
# PutRumEventsRequestRequestTypeDef definition

class PutRumEventsRequestRequestTypeDef(TypedDict):
    AppMonitorDetails: AppMonitorDetailsTypeDef,  # (1)
    BatchId: str,
    Id: str,
    RumEvents: Sequence[RumEventTypeDef],  # (2)
    UserDetails: UserDetailsTypeDef,  # (3)
```

1. See [:material-code-braces: AppMonitorDetailsTypeDef](./type_defs.md#appmonitordetailstypedef) 
2. See [:material-code-braces: RumEventTypeDef](./type_defs.md#rumeventtypedef) 
3. See [:material-code-braces: UserDetailsTypeDef](./type_defs.md#userdetailstypedef) 
## GetAppMonitorResponseTypeDef

```python
# GetAppMonitorResponseTypeDef definition

class GetAppMonitorResponseTypeDef(TypedDict):
    AppMonitor: AppMonitorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppMonitorTypeDef](./type_defs.md#appmonitortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
