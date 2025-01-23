# Type definitions

> [Index](../README.md) > [CloudWatchInternetMonitor](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchInternetMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#cloudwatchinternetmonitor)
    type annotations stubs module [types-aiobotocore-internetmonitor](https://pypi.org/project/types-aiobotocore-internetmonitor/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AvailabilityMeasurementTypeDef

```python
# AvailabilityMeasurementTypeDef definition

class AvailabilityMeasurementTypeDef(TypedDict):
    ExperienceScore: NotRequired[float],
    PercentOfTotalTrafficImpacted: NotRequired[float],
    PercentOfClientLocationImpacted: NotRequired[float],
```

## ClientLocationTypeDef

```python
# ClientLocationTypeDef definition

class ClientLocationTypeDef(TypedDict):
    ASName: str,
    ASNumber: int,
    Country: str,
    City: str,
    Latitude: float,
    Longitude: float,
    Subdivision: NotRequired[str],
    Metro: NotRequired[str],
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

## DeleteMonitorInputRequestTypeDef

```python
# DeleteMonitorInputRequestTypeDef definition

class DeleteMonitorInputRequestTypeDef(TypedDict):
    MonitorName: str,
```

## FilterParameterTypeDef

```python
# FilterParameterTypeDef definition

class FilterParameterTypeDef(TypedDict):
    Field: NotRequired[str],
    Operator: NotRequired[OperatorType],  # (1)
    Values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## GetHealthEventInputRequestTypeDef

```python
# GetHealthEventInputRequestTypeDef definition

class GetHealthEventInputRequestTypeDef(TypedDict):
    MonitorName: str,
    EventId: str,
    LinkedAccountId: NotRequired[str],
```

## GetInternetEventInputRequestTypeDef

```python
# GetInternetEventInputRequestTypeDef definition

class GetInternetEventInputRequestTypeDef(TypedDict):
    EventId: str,
```

## GetMonitorInputRequestTypeDef

```python
# GetMonitorInputRequestTypeDef definition

class GetMonitorInputRequestTypeDef(TypedDict):
    MonitorName: str,
    LinkedAccountId: NotRequired[str],
```

## GetQueryResultsInputRequestTypeDef

```python
# GetQueryResultsInputRequestTypeDef definition

class GetQueryResultsInputRequestTypeDef(TypedDict):
    MonitorName: str,
    QueryId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## QueryFieldTypeDef

```python
# QueryFieldTypeDef definition

class QueryFieldTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[str],
```

## GetQueryStatusInputRequestTypeDef

```python
# GetQueryStatusInputRequestTypeDef definition

class GetQueryStatusInputRequestTypeDef(TypedDict):
    MonitorName: str,
    QueryId: str,
```

## LocalHealthEventsConfigTypeDef

```python
# LocalHealthEventsConfigTypeDef definition

class LocalHealthEventsConfigTypeDef(TypedDict):
    Status: NotRequired[LocalHealthEventsConfigStatusType],  # (1)
    HealthScoreThreshold: NotRequired[float],
    MinTrafficImpact: NotRequired[float],
```

1. See [:material-code-brackets: LocalHealthEventsConfigStatusType](./literals.md#localhealtheventsconfigstatustype) 
## S3ConfigTypeDef

```python
# S3ConfigTypeDef definition

class S3ConfigTypeDef(TypedDict):
    BucketName: NotRequired[str],
    BucketPrefix: NotRequired[str],
    LogDeliveryStatus: NotRequired[LogDeliveryStatusType],  # (1)
```

1. See [:material-code-brackets: LogDeliveryStatusType](./literals.md#logdeliverystatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListMonitorsInputRequestTypeDef

```python
# ListMonitorsInputRequestTypeDef definition

class ListMonitorsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    MonitorStatus: NotRequired[str],
    IncludeLinkedAccounts: NotRequired[bool],
```

## MonitorTypeDef

```python
# MonitorTypeDef definition

class MonitorTypeDef(TypedDict):
    MonitorName: str,
    MonitorArn: str,
    Status: MonitorConfigStateType,  # (1)
    ProcessingStatus: NotRequired[MonitorProcessingStatusCodeType],  # (2)
```

1. See [:material-code-brackets: MonitorConfigStateType](./literals.md#monitorconfigstatetype) 
2. See [:material-code-brackets: MonitorProcessingStatusCodeType](./literals.md#monitorprocessingstatuscodetype) 
## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## NetworkTypeDef

```python
# NetworkTypeDef definition

class NetworkTypeDef(TypedDict):
    ASName: str,
    ASNumber: int,
```

## RoundTripTimeTypeDef

```python
# RoundTripTimeTypeDef definition

class RoundTripTimeTypeDef(TypedDict):
    P50: NotRequired[float],
    P90: NotRequired[float],
    P95: NotRequired[float],
```

## StopQueryInputRequestTypeDef

```python
# StopQueryInputRequestTypeDef definition

class StopQueryInputRequestTypeDef(TypedDict):
    MonitorName: str,
    QueryId: str,
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## InternetEventSummaryTypeDef

```python
# InternetEventSummaryTypeDef definition

class InternetEventSummaryTypeDef(TypedDict):
    EventId: str,
    EventArn: str,
    StartedAt: datetime,
    ClientLocation: ClientLocationTypeDef,  # (1)
    EventType: InternetEventTypeType,  # (2)
    EventStatus: InternetEventStatusType,  # (3)
    EndedAt: NotRequired[datetime],
```

1. See [:material-code-braces: ClientLocationTypeDef](./type_defs.md#clientlocationtypedef) 
2. See [:material-code-brackets: InternetEventTypeType](./literals.md#interneteventtypetype) 
3. See [:material-code-brackets: InternetEventStatusType](./literals.md#interneteventstatustype) 
## CreateMonitorOutputTypeDef

```python
# CreateMonitorOutputTypeDef definition

class CreateMonitorOutputTypeDef(TypedDict):
    Arn: str,
    Status: MonitorConfigStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MonitorConfigStateType](./literals.md#monitorconfigstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInternetEventOutputTypeDef

```python
# GetInternetEventOutputTypeDef definition

class GetInternetEventOutputTypeDef(TypedDict):
    EventId: str,
    EventArn: str,
    StartedAt: datetime,
    EndedAt: datetime,
    ClientLocation: ClientLocationTypeDef,  # (1)
    EventType: InternetEventTypeType,  # (2)
    EventStatus: InternetEventStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ClientLocationTypeDef](./type_defs.md#clientlocationtypedef) 
2. See [:material-code-brackets: InternetEventTypeType](./literals.md#interneteventtypetype) 
3. See [:material-code-brackets: InternetEventStatusType](./literals.md#interneteventstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueryStatusOutputTypeDef

```python
# GetQueryStatusOutputTypeDef definition

class GetQueryStatusOutputTypeDef(TypedDict):
    Status: QueryStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartQueryOutputTypeDef

```python
# StartQueryOutputTypeDef definition

class StartQueryOutputTypeDef(TypedDict):
    QueryId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMonitorOutputTypeDef

```python
# UpdateMonitorOutputTypeDef definition

class UpdateMonitorOutputTypeDef(TypedDict):
    MonitorArn: str,
    Status: MonitorConfigStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MonitorConfigStateType](./literals.md#monitorconfigstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueryResultsOutputTypeDef

```python
# GetQueryResultsOutputTypeDef definition

class GetQueryResultsOutputTypeDef(TypedDict):
    Fields: List[QueryFieldTypeDef],  # (1)
    Data: List[List[str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QueryFieldTypeDef](./type_defs.md#queryfieldtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HealthEventsConfigTypeDef

```python
# HealthEventsConfigTypeDef definition

class HealthEventsConfigTypeDef(TypedDict):
    AvailabilityScoreThreshold: NotRequired[float],
    PerformanceScoreThreshold: NotRequired[float],
    AvailabilityLocalHealthEventsConfig: NotRequired[LocalHealthEventsConfigTypeDef],  # (1)
    PerformanceLocalHealthEventsConfig: NotRequired[LocalHealthEventsConfigTypeDef],  # (1)
```

1. See [:material-code-braces: LocalHealthEventsConfigTypeDef](./type_defs.md#localhealtheventsconfigtypedef) 
2. See [:material-code-braces: LocalHealthEventsConfigTypeDef](./type_defs.md#localhealtheventsconfigtypedef) 
## InternetMeasurementsLogDeliveryTypeDef

```python
# InternetMeasurementsLogDeliveryTypeDef definition

class InternetMeasurementsLogDeliveryTypeDef(TypedDict):
    S3Config: NotRequired[S3ConfigTypeDef],  # (1)
```

1. See [:material-code-braces: S3ConfigTypeDef](./type_defs.md#s3configtypedef) 
## ListMonitorsInputPaginateTypeDef

```python
# ListMonitorsInputPaginateTypeDef definition

class ListMonitorsInputPaginateTypeDef(TypedDict):
    MonitorStatus: NotRequired[str],
    IncludeLinkedAccounts: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHealthEventsInputPaginateTypeDef

```python
# ListHealthEventsInputPaginateTypeDef definition

class ListHealthEventsInputPaginateTypeDef(TypedDict):
    MonitorName: str,
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    EventStatus: NotRequired[HealthEventStatusType],  # (1)
    LinkedAccountId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: HealthEventStatusType](./literals.md#healtheventstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHealthEventsInputRequestTypeDef

```python
# ListHealthEventsInputRequestTypeDef definition

class ListHealthEventsInputRequestTypeDef(TypedDict):
    MonitorName: str,
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    EventStatus: NotRequired[HealthEventStatusType],  # (1)
    LinkedAccountId: NotRequired[str],
```

1. See [:material-code-brackets: HealthEventStatusType](./literals.md#healtheventstatustype) 
## ListInternetEventsInputPaginateTypeDef

```python
# ListInternetEventsInputPaginateTypeDef definition

class ListInternetEventsInputPaginateTypeDef(TypedDict):
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    EventStatus: NotRequired[str],
    EventType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInternetEventsInputRequestTypeDef

```python
# ListInternetEventsInputRequestTypeDef definition

class ListInternetEventsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    EventStatus: NotRequired[str],
    EventType: NotRequired[str],
```

## StartQueryInputRequestTypeDef

```python
# StartQueryInputRequestTypeDef definition

class StartQueryInputRequestTypeDef(TypedDict):
    MonitorName: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    QueryType: QueryTypeType,  # (1)
    FilterParameters: NotRequired[Sequence[FilterParameterTypeDef]],  # (2)
    LinkedAccountId: NotRequired[str],
```

1. See [:material-code-brackets: QueryTypeType](./literals.md#querytypetype) 
2. See [:material-code-braces: FilterParameterTypeDef](./type_defs.md#filterparametertypedef) 
## ListMonitorsOutputTypeDef

```python
# ListMonitorsOutputTypeDef definition

class ListMonitorsOutputTypeDef(TypedDict):
    Monitors: List[MonitorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MonitorTypeDef](./type_defs.md#monitortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkImpairmentTypeDef

```python
# NetworkImpairmentTypeDef definition

class NetworkImpairmentTypeDef(TypedDict):
    Networks: List[NetworkTypeDef],  # (1)
    AsPath: List[NetworkTypeDef],  # (1)
    NetworkEventType: TriangulationEventTypeType,  # (3)
```

1. See [:material-code-braces: NetworkTypeDef](./type_defs.md#networktypedef) 
2. See [:material-code-braces: NetworkTypeDef](./type_defs.md#networktypedef) 
3. See [:material-code-brackets: TriangulationEventTypeType](./literals.md#triangulationeventtypetype) 
## PerformanceMeasurementTypeDef

```python
# PerformanceMeasurementTypeDef definition

class PerformanceMeasurementTypeDef(TypedDict):
    ExperienceScore: NotRequired[float],
    PercentOfTotalTrafficImpacted: NotRequired[float],
    PercentOfClientLocationImpacted: NotRequired[float],
    RoundTripTime: NotRequired[RoundTripTimeTypeDef],  # (1)
```

1. See [:material-code-braces: RoundTripTimeTypeDef](./type_defs.md#roundtriptimetypedef) 
## ListInternetEventsOutputTypeDef

```python
# ListInternetEventsOutputTypeDef definition

class ListInternetEventsOutputTypeDef(TypedDict):
    InternetEvents: List[InternetEventSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InternetEventSummaryTypeDef](./type_defs.md#interneteventsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMonitorInputRequestTypeDef

```python
# CreateMonitorInputRequestTypeDef definition

class CreateMonitorInputRequestTypeDef(TypedDict):
    MonitorName: str,
    Resources: NotRequired[Sequence[str]],
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    MaxCityNetworksToMonitor: NotRequired[int],
    InternetMeasurementsLogDelivery: NotRequired[InternetMeasurementsLogDeliveryTypeDef],  # (1)
    TrafficPercentageToMonitor: NotRequired[int],
    HealthEventsConfig: NotRequired[HealthEventsConfigTypeDef],  # (2)
```

1. See [:material-code-braces: InternetMeasurementsLogDeliveryTypeDef](./type_defs.md#internetmeasurementslogdeliverytypedef) 
2. See [:material-code-braces: HealthEventsConfigTypeDef](./type_defs.md#healtheventsconfigtypedef) 
## GetMonitorOutputTypeDef

```python
# GetMonitorOutputTypeDef definition

class GetMonitorOutputTypeDef(TypedDict):
    MonitorName: str,
    MonitorArn: str,
    Resources: List[str],
    Status: MonitorConfigStateType,  # (1)
    CreatedAt: datetime,
    ModifiedAt: datetime,
    ProcessingStatus: MonitorProcessingStatusCodeType,  # (2)
    ProcessingStatusInfo: str,
    Tags: Dict[str, str],
    MaxCityNetworksToMonitor: int,
    InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef,  # (3)
    TrafficPercentageToMonitor: int,
    HealthEventsConfig: HealthEventsConfigTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: MonitorConfigStateType](./literals.md#monitorconfigstatetype) 
2. See [:material-code-brackets: MonitorProcessingStatusCodeType](./literals.md#monitorprocessingstatuscodetype) 
3. See [:material-code-braces: InternetMeasurementsLogDeliveryTypeDef](./type_defs.md#internetmeasurementslogdeliverytypedef) 
4. See [:material-code-braces: HealthEventsConfigTypeDef](./type_defs.md#healtheventsconfigtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMonitorInputRequestTypeDef

```python
# UpdateMonitorInputRequestTypeDef definition

class UpdateMonitorInputRequestTypeDef(TypedDict):
    MonitorName: str,
    ResourcesToAdd: NotRequired[Sequence[str]],
    ResourcesToRemove: NotRequired[Sequence[str]],
    Status: NotRequired[MonitorConfigStateType],  # (1)
    ClientToken: NotRequired[str],
    MaxCityNetworksToMonitor: NotRequired[int],
    InternetMeasurementsLogDelivery: NotRequired[InternetMeasurementsLogDeliveryTypeDef],  # (2)
    TrafficPercentageToMonitor: NotRequired[int],
    HealthEventsConfig: NotRequired[HealthEventsConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: MonitorConfigStateType](./literals.md#monitorconfigstatetype) 
2. See [:material-code-braces: InternetMeasurementsLogDeliveryTypeDef](./type_defs.md#internetmeasurementslogdeliverytypedef) 
3. See [:material-code-braces: HealthEventsConfigTypeDef](./type_defs.md#healtheventsconfigtypedef) 
## InternetHealthTypeDef

```python
# InternetHealthTypeDef definition

class InternetHealthTypeDef(TypedDict):
    Availability: NotRequired[AvailabilityMeasurementTypeDef],  # (1)
    Performance: NotRequired[PerformanceMeasurementTypeDef],  # (2)
```

1. See [:material-code-braces: AvailabilityMeasurementTypeDef](./type_defs.md#availabilitymeasurementtypedef) 
2. See [:material-code-braces: PerformanceMeasurementTypeDef](./type_defs.md#performancemeasurementtypedef) 
## ImpactedLocationTypeDef

```python
# ImpactedLocationTypeDef definition

class ImpactedLocationTypeDef(TypedDict):
    ASName: str,
    ASNumber: int,
    Country: str,
    Status: HealthEventStatusType,  # (1)
    Subdivision: NotRequired[str],
    Metro: NotRequired[str],
    City: NotRequired[str],
    Latitude: NotRequired[float],
    Longitude: NotRequired[float],
    CountryCode: NotRequired[str],
    SubdivisionCode: NotRequired[str],
    ServiceLocation: NotRequired[str],
    CausedBy: NotRequired[NetworkImpairmentTypeDef],  # (2)
    InternetHealth: NotRequired[InternetHealthTypeDef],  # (3)
    Ipv4Prefixes: NotRequired[List[str]],
```

1. See [:material-code-brackets: HealthEventStatusType](./literals.md#healtheventstatustype) 
2. See [:material-code-braces: NetworkImpairmentTypeDef](./type_defs.md#networkimpairmenttypedef) 
3. See [:material-code-braces: InternetHealthTypeDef](./type_defs.md#internethealthtypedef) 
## GetHealthEventOutputTypeDef

```python
# GetHealthEventOutputTypeDef definition

class GetHealthEventOutputTypeDef(TypedDict):
    EventArn: str,
    EventId: str,
    StartedAt: datetime,
    EndedAt: datetime,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    ImpactedLocations: List[ImpactedLocationTypeDef],  # (1)
    Status: HealthEventStatusType,  # (2)
    PercentOfTotalTrafficImpacted: float,
    ImpactType: HealthEventImpactTypeType,  # (3)
    HealthScoreThreshold: float,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ImpactedLocationTypeDef](./type_defs.md#impactedlocationtypedef) 
2. See [:material-code-brackets: HealthEventStatusType](./literals.md#healtheventstatustype) 
3. See [:material-code-brackets: HealthEventImpactTypeType](./literals.md#healtheventimpacttypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HealthEventTypeDef

```python
# HealthEventTypeDef definition

class HealthEventTypeDef(TypedDict):
    EventArn: str,
    EventId: str,
    StartedAt: datetime,
    LastUpdatedAt: datetime,
    ImpactedLocations: List[ImpactedLocationTypeDef],  # (1)
    Status: HealthEventStatusType,  # (2)
    ImpactType: HealthEventImpactTypeType,  # (3)
    EndedAt: NotRequired[datetime],
    CreatedAt: NotRequired[datetime],
    PercentOfTotalTrafficImpacted: NotRequired[float],
    HealthScoreThreshold: NotRequired[float],
```

1. See [:material-code-braces: ImpactedLocationTypeDef](./type_defs.md#impactedlocationtypedef) 
2. See [:material-code-brackets: HealthEventStatusType](./literals.md#healtheventstatustype) 
3. See [:material-code-brackets: HealthEventImpactTypeType](./literals.md#healtheventimpacttypetype) 
## ListHealthEventsOutputTypeDef

```python
# ListHealthEventsOutputTypeDef definition

class ListHealthEventsOutputTypeDef(TypedDict):
    HealthEvents: List[HealthEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HealthEventTypeDef](./type_defs.md#healtheventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
