# Type definitions

> [Index](../README.md) > [LocationService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
    type annotations stubs module [types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## CircleUnionTypeDef

```python
# CircleUnionTypeDef definition

CircleUnionTypeDef = Union[
    CircleTypeDef,  # (1)
    CircleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CircleTypeDef](./type_defs.md#circletypedef) 
2. See [:material-code-braces: CircleOutputTypeDef](./type_defs.md#circleoutputtypedef) 

## GeofenceGeometryUnionTypeDef

```python
# GeofenceGeometryUnionTypeDef definition

GeofenceGeometryUnionTypeDef = Union[
    GeofenceGeometryTypeDef,  # (1)
    GeofenceGeometryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GeofenceGeometryTypeDef](./type_defs.md#geofencegeometrytypedef) 
2. See [:material-code-braces: GeofenceGeometryOutputTypeDef](./type_defs.md#geofencegeometryoutputtypedef) 



## ApiKeyFilterTypeDef

```python
# ApiKeyFilterTypeDef definition

class ApiKeyFilterTypeDef(TypedDict):
    KeyStatus: NotRequired[StatusType],  # (1)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ApiKeyRestrictionsOutputTypeDef

```python
# ApiKeyRestrictionsOutputTypeDef definition

class ApiKeyRestrictionsOutputTypeDef(TypedDict):
    AllowActions: List[str],
    AllowResources: List[str],
    AllowReferers: NotRequired[List[str]],
```

## ApiKeyRestrictionsTypeDef

```python
# ApiKeyRestrictionsTypeDef definition

class ApiKeyRestrictionsTypeDef(TypedDict):
    AllowActions: Sequence[str],
    AllowResources: Sequence[str],
    AllowReferers: NotRequired[Sequence[str]],
```

## AssociateTrackerConsumerRequestRequestTypeDef

```python
# AssociateTrackerConsumerRequestRequestTypeDef definition

class AssociateTrackerConsumerRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    ConsumerArn: str,
```

## BatchItemErrorTypeDef

```python
# BatchItemErrorTypeDef definition

class BatchItemErrorTypeDef(TypedDict):
    Code: NotRequired[BatchItemErrorCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: BatchItemErrorCodeType](./literals.md#batchitemerrorcodetype) 
## BatchDeleteDevicePositionHistoryRequestRequestTypeDef

```python
# BatchDeleteDevicePositionHistoryRequestRequestTypeDef definition

class BatchDeleteDevicePositionHistoryRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    DeviceIds: Sequence[str],
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

## BatchDeleteGeofenceRequestRequestTypeDef

```python
# BatchDeleteGeofenceRequestRequestTypeDef definition

class BatchDeleteGeofenceRequestRequestTypeDef(TypedDict):
    CollectionName: str,
    GeofenceIds: Sequence[str],
```

## BatchGetDevicePositionRequestRequestTypeDef

```python
# BatchGetDevicePositionRequestRequestTypeDef definition

class BatchGetDevicePositionRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    DeviceIds: Sequence[str],
```

## BatchPutGeofenceSuccessTypeDef

```python
# BatchPutGeofenceSuccessTypeDef definition

class BatchPutGeofenceSuccessTypeDef(TypedDict):
    GeofenceId: str,
    CreateTime: datetime,
    UpdateTime: datetime,
```

## CalculateRouteCarModeOptionsTypeDef

```python
# CalculateRouteCarModeOptionsTypeDef definition

class CalculateRouteCarModeOptionsTypeDef(TypedDict):
    AvoidFerries: NotRequired[bool],
    AvoidTolls: NotRequired[bool],
```

## CalculateRouteMatrixSummaryTypeDef

```python
# CalculateRouteMatrixSummaryTypeDef definition

class CalculateRouteMatrixSummaryTypeDef(TypedDict):
    DataSource: str,
    RouteCount: int,
    ErrorCount: int,
    DistanceUnit: DistanceUnitType,  # (1)
```

1. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
## CalculateRouteSummaryTypeDef

```python
# CalculateRouteSummaryTypeDef definition

class CalculateRouteSummaryTypeDef(TypedDict):
    RouteBBox: List[float],
    DataSource: str,
    Distance: float,
    DurationSeconds: float,
    DistanceUnit: DistanceUnitType,  # (1)
```

1. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
## TruckDimensionsTypeDef

```python
# TruckDimensionsTypeDef definition

class TruckDimensionsTypeDef(TypedDict):
    Length: NotRequired[float],
    Height: NotRequired[float],
    Width: NotRequired[float],
    Unit: NotRequired[DimensionUnitType],  # (1)
```

1. See [:material-code-brackets: DimensionUnitType](./literals.md#dimensionunittype) 
## TruckWeightTypeDef

```python
# TruckWeightTypeDef definition

class TruckWeightTypeDef(TypedDict):
    Total: NotRequired[float],
    Unit: NotRequired[VehicleWeightUnitType],  # (1)
```

1. See [:material-code-brackets: VehicleWeightUnitType](./literals.md#vehicleweightunittype) 
## CircleOutputTypeDef

```python
# CircleOutputTypeDef definition

class CircleOutputTypeDef(TypedDict):
    Center: List[float],
    Radius: float,
```

## CircleTypeDef

```python
# CircleTypeDef definition

class CircleTypeDef(TypedDict):
    Center: Sequence[float],
    Radius: float,
```

## CreateGeofenceCollectionRequestRequestTypeDef

```python
# CreateGeofenceCollectionRequestRequestTypeDef definition

class CreateGeofenceCollectionRequestRequestTypeDef(TypedDict):
    CollectionName: str,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    PricingPlanDataSource: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## MapConfigurationTypeDef

```python
# MapConfigurationTypeDef definition

class MapConfigurationTypeDef(TypedDict):
    Style: str,
    PoliticalView: NotRequired[str],
    CustomLayers: NotRequired[Sequence[str]],
```

## DataSourceConfigurationTypeDef

```python
# DataSourceConfigurationTypeDef definition

class DataSourceConfigurationTypeDef(TypedDict):
    IntendedUse: NotRequired[IntendedUseType],  # (1)
```

1. See [:material-code-brackets: IntendedUseType](./literals.md#intendedusetype) 
## CreateRouteCalculatorRequestRequestTypeDef

```python
# CreateRouteCalculatorRequestRequestTypeDef definition

class CreateRouteCalculatorRequestRequestTypeDef(TypedDict):
    CalculatorName: str,
    DataSource: str,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## CreateTrackerRequestRequestTypeDef

```python
# CreateTrackerRequestRequestTypeDef definition

class CreateTrackerRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    KmsKeyId: NotRequired[str],
    PricingPlanDataSource: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    PositionFiltering: NotRequired[PositionFilteringType],  # (2)
    EventBridgeEnabled: NotRequired[bool],
    KmsKeyEnableGeospatialQueries: NotRequired[bool],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-brackets: PositionFilteringType](./literals.md#positionfilteringtype) 
## DeleteGeofenceCollectionRequestRequestTypeDef

```python
# DeleteGeofenceCollectionRequestRequestTypeDef definition

class DeleteGeofenceCollectionRequestRequestTypeDef(TypedDict):
    CollectionName: str,
```

## DeleteKeyRequestRequestTypeDef

```python
# DeleteKeyRequestRequestTypeDef definition

class DeleteKeyRequestRequestTypeDef(TypedDict):
    KeyName: str,
    ForceDelete: NotRequired[bool],
```

## DeleteMapRequestRequestTypeDef

```python
# DeleteMapRequestRequestTypeDef definition

class DeleteMapRequestRequestTypeDef(TypedDict):
    MapName: str,
```

## DeletePlaceIndexRequestRequestTypeDef

```python
# DeletePlaceIndexRequestRequestTypeDef definition

class DeletePlaceIndexRequestRequestTypeDef(TypedDict):
    IndexName: str,
```

## DeleteRouteCalculatorRequestRequestTypeDef

```python
# DeleteRouteCalculatorRequestRequestTypeDef definition

class DeleteRouteCalculatorRequestRequestTypeDef(TypedDict):
    CalculatorName: str,
```

## DeleteTrackerRequestRequestTypeDef

```python
# DeleteTrackerRequestRequestTypeDef definition

class DeleteTrackerRequestRequestTypeDef(TypedDict):
    TrackerName: str,
```

## DescribeGeofenceCollectionRequestRequestTypeDef

```python
# DescribeGeofenceCollectionRequestRequestTypeDef definition

class DescribeGeofenceCollectionRequestRequestTypeDef(TypedDict):
    CollectionName: str,
```

## DescribeKeyRequestRequestTypeDef

```python
# DescribeKeyRequestRequestTypeDef definition

class DescribeKeyRequestRequestTypeDef(TypedDict):
    KeyName: str,
```

## DescribeMapRequestRequestTypeDef

```python
# DescribeMapRequestRequestTypeDef definition

class DescribeMapRequestRequestTypeDef(TypedDict):
    MapName: str,
```

## MapConfigurationOutputTypeDef

```python
# MapConfigurationOutputTypeDef definition

class MapConfigurationOutputTypeDef(TypedDict):
    Style: str,
    PoliticalView: NotRequired[str],
    CustomLayers: NotRequired[List[str]],
```

## DescribePlaceIndexRequestRequestTypeDef

```python
# DescribePlaceIndexRequestRequestTypeDef definition

class DescribePlaceIndexRequestRequestTypeDef(TypedDict):
    IndexName: str,
```

## DescribeRouteCalculatorRequestRequestTypeDef

```python
# DescribeRouteCalculatorRequestRequestTypeDef definition

class DescribeRouteCalculatorRequestRequestTypeDef(TypedDict):
    CalculatorName: str,
```

## DescribeTrackerRequestRequestTypeDef

```python
# DescribeTrackerRequestRequestTypeDef definition

class DescribeTrackerRequestRequestTypeDef(TypedDict):
    TrackerName: str,
```

## PositionalAccuracyTypeDef

```python
# PositionalAccuracyTypeDef definition

class PositionalAccuracyTypeDef(TypedDict):
    Horizontal: float,
```

## WiFiAccessPointTypeDef

```python
# WiFiAccessPointTypeDef definition

class WiFiAccessPointTypeDef(TypedDict):
    MacAddress: str,
    Rss: int,
```

## DisassociateTrackerConsumerRequestRequestTypeDef

```python
# DisassociateTrackerConsumerRequestRequestTypeDef definition

class DisassociateTrackerConsumerRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    ConsumerArn: str,
```

## ForecastGeofenceEventsDeviceStateTypeDef

```python
# ForecastGeofenceEventsDeviceStateTypeDef definition

class ForecastGeofenceEventsDeviceStateTypeDef(TypedDict):
    Position: Sequence[float],
    Speed: NotRequired[float],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ForecastedEventTypeDef

```python
# ForecastedEventTypeDef definition

class ForecastedEventTypeDef(TypedDict):
    EventId: str,
    GeofenceId: str,
    IsDeviceInGeofence: bool,
    NearestDistance: float,
    EventType: ForecastedGeofenceEventTypeType,  # (1)
    ForecastedBreachTime: NotRequired[datetime],
    GeofenceProperties: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ForecastedGeofenceEventTypeType](./literals.md#forecastedgeofenceeventtypetype) 
## GetDevicePositionRequestRequestTypeDef

```python
# GetDevicePositionRequestRequestTypeDef definition

class GetDevicePositionRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    DeviceId: str,
```

## GetGeofenceRequestRequestTypeDef

```python
# GetGeofenceRequestRequestTypeDef definition

class GetGeofenceRequestRequestTypeDef(TypedDict):
    CollectionName: str,
    GeofenceId: str,
```

## GetMapGlyphsRequestRequestTypeDef

```python
# GetMapGlyphsRequestRequestTypeDef definition

class GetMapGlyphsRequestRequestTypeDef(TypedDict):
    MapName: str,
    FontStack: str,
    FontUnicodeRange: str,
    Key: NotRequired[str],
```

## GetMapSpritesRequestRequestTypeDef

```python
# GetMapSpritesRequestRequestTypeDef definition

class GetMapSpritesRequestRequestTypeDef(TypedDict):
    MapName: str,
    FileName: str,
    Key: NotRequired[str],
```

## GetMapStyleDescriptorRequestRequestTypeDef

```python
# GetMapStyleDescriptorRequestRequestTypeDef definition

class GetMapStyleDescriptorRequestRequestTypeDef(TypedDict):
    MapName: str,
    Key: NotRequired[str],
```

## GetMapTileRequestRequestTypeDef

```python
# GetMapTileRequestRequestTypeDef definition

class GetMapTileRequestRequestTypeDef(TypedDict):
    MapName: str,
    Z: str,
    X: str,
    Y: str,
    Key: NotRequired[str],
```

## GetPlaceRequestRequestTypeDef

```python
# GetPlaceRequestRequestTypeDef definition

class GetPlaceRequestRequestTypeDef(TypedDict):
    IndexName: str,
    PlaceId: str,
    Language: NotRequired[str],
    Key: NotRequired[str],
```

## LegGeometryTypeDef

```python
# LegGeometryTypeDef definition

class LegGeometryTypeDef(TypedDict):
    LineString: NotRequired[List[List[float]]],
```

## StepTypeDef

```python
# StepTypeDef definition

class StepTypeDef(TypedDict):
    StartPosition: List[float],
    EndPosition: List[float],
    Distance: float,
    DurationSeconds: float,
    GeometryOffset: NotRequired[int],
```

## TrackingFilterGeometryTypeDef

```python
# TrackingFilterGeometryTypeDef definition

class TrackingFilterGeometryTypeDef(TypedDict):
    Polygon: NotRequired[Sequence[Sequence[Sequence[float]]]],
```

## ListGeofenceCollectionsRequestRequestTypeDef

```python
# ListGeofenceCollectionsRequestRequestTypeDef definition

class ListGeofenceCollectionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListGeofenceCollectionsResponseEntryTypeDef

```python
# ListGeofenceCollectionsResponseEntryTypeDef definition

class ListGeofenceCollectionsResponseEntryTypeDef(TypedDict):
    CollectionName: str,
    Description: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    PricingPlanDataSource: NotRequired[str],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## ListGeofencesRequestRequestTypeDef

```python
# ListGeofencesRequestRequestTypeDef definition

class ListGeofencesRequestRequestTypeDef(TypedDict):
    CollectionName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListMapsRequestRequestTypeDef

```python
# ListMapsRequestRequestTypeDef definition

class ListMapsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListMapsResponseEntryTypeDef

```python
# ListMapsResponseEntryTypeDef definition

class ListMapsResponseEntryTypeDef(TypedDict):
    MapName: str,
    Description: str,
    DataSource: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## ListPlaceIndexesRequestRequestTypeDef

```python
# ListPlaceIndexesRequestRequestTypeDef definition

class ListPlaceIndexesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListPlaceIndexesResponseEntryTypeDef

```python
# ListPlaceIndexesResponseEntryTypeDef definition

class ListPlaceIndexesResponseEntryTypeDef(TypedDict):
    IndexName: str,
    Description: str,
    DataSource: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## ListRouteCalculatorsRequestRequestTypeDef

```python
# ListRouteCalculatorsRequestRequestTypeDef definition

class ListRouteCalculatorsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListRouteCalculatorsResponseEntryTypeDef

```python
# ListRouteCalculatorsResponseEntryTypeDef definition

class ListRouteCalculatorsResponseEntryTypeDef(TypedDict):
    CalculatorName: str,
    Description: str,
    DataSource: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListTrackerConsumersRequestRequestTypeDef

```python
# ListTrackerConsumersRequestRequestTypeDef definition

class ListTrackerConsumersRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTrackersRequestRequestTypeDef

```python
# ListTrackersRequestRequestTypeDef definition

class ListTrackersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTrackersResponseEntryTypeDef

```python
# ListTrackersResponseEntryTypeDef definition

class ListTrackersResponseEntryTypeDef(TypedDict):
    TrackerName: str,
    Description: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    PricingPlanDataSource: NotRequired[str],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## LteLocalIdTypeDef

```python
# LteLocalIdTypeDef definition

class LteLocalIdTypeDef(TypedDict):
    Earfcn: int,
    Pci: int,
```

## LteNetworkMeasurementsTypeDef

```python
# LteNetworkMeasurementsTypeDef definition

class LteNetworkMeasurementsTypeDef(TypedDict):
    Earfcn: int,
    CellId: int,
    Pci: int,
    Rsrp: NotRequired[int],
    Rsrq: NotRequired[float],
```

## MapConfigurationUpdateTypeDef

```python
# MapConfigurationUpdateTypeDef definition

class MapConfigurationUpdateTypeDef(TypedDict):
    PoliticalView: NotRequired[str],
    CustomLayers: NotRequired[Sequence[str]],
```

## PlaceGeometryTypeDef

```python
# PlaceGeometryTypeDef definition

class PlaceGeometryTypeDef(TypedDict):
    Point: NotRequired[List[float]],
```

## TimeZoneTypeDef

```python
# TimeZoneTypeDef definition

class TimeZoneTypeDef(TypedDict):
    Name: str,
    Offset: NotRequired[int],
```

## RouteMatrixEntryErrorTypeDef

```python
# RouteMatrixEntryErrorTypeDef definition

class RouteMatrixEntryErrorTypeDef(TypedDict):
    Code: RouteMatrixErrorCodeType,  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: RouteMatrixErrorCodeType](./literals.md#routematrixerrorcodetype) 
## SearchForSuggestionsResultTypeDef

```python
# SearchForSuggestionsResultTypeDef definition

class SearchForSuggestionsResultTypeDef(TypedDict):
    Text: str,
    PlaceId: NotRequired[str],
    Categories: NotRequired[List[str]],
    SupplementalCategories: NotRequired[List[str]],
```

## SearchPlaceIndexForPositionRequestRequestTypeDef

```python
# SearchPlaceIndexForPositionRequestRequestTypeDef definition

class SearchPlaceIndexForPositionRequestRequestTypeDef(TypedDict):
    IndexName: str,
    Position: Sequence[float],
    MaxResults: NotRequired[int],
    Language: NotRequired[str],
    Key: NotRequired[str],
```

## SearchPlaceIndexForPositionSummaryTypeDef

```python
# SearchPlaceIndexForPositionSummaryTypeDef definition

class SearchPlaceIndexForPositionSummaryTypeDef(TypedDict):
    Position: List[float],
    DataSource: str,
    MaxResults: NotRequired[int],
    Language: NotRequired[str],
```

## SearchPlaceIndexForSuggestionsRequestRequestTypeDef

```python
# SearchPlaceIndexForSuggestionsRequestRequestTypeDef definition

class SearchPlaceIndexForSuggestionsRequestRequestTypeDef(TypedDict):
    IndexName: str,
    Text: str,
    BiasPosition: NotRequired[Sequence[float]],
    FilterBBox: NotRequired[Sequence[float]],
    FilterCountries: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    Language: NotRequired[str],
    FilterCategories: NotRequired[Sequence[str]],
    Key: NotRequired[str],
```

## SearchPlaceIndexForSuggestionsSummaryTypeDef

```python
# SearchPlaceIndexForSuggestionsSummaryTypeDef definition

class SearchPlaceIndexForSuggestionsSummaryTypeDef(TypedDict):
    Text: str,
    DataSource: str,
    BiasPosition: NotRequired[List[float]],
    FilterBBox: NotRequired[List[float]],
    FilterCountries: NotRequired[List[str]],
    MaxResults: NotRequired[int],
    Language: NotRequired[str],
    FilterCategories: NotRequired[List[str]],
```

## SearchPlaceIndexForTextRequestRequestTypeDef

```python
# SearchPlaceIndexForTextRequestRequestTypeDef definition

class SearchPlaceIndexForTextRequestRequestTypeDef(TypedDict):
    IndexName: str,
    Text: str,
    BiasPosition: NotRequired[Sequence[float]],
    FilterBBox: NotRequired[Sequence[float]],
    FilterCountries: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    Language: NotRequired[str],
    FilterCategories: NotRequired[Sequence[str]],
    Key: NotRequired[str],
```

## SearchPlaceIndexForTextSummaryTypeDef

```python
# SearchPlaceIndexForTextSummaryTypeDef definition

class SearchPlaceIndexForTextSummaryTypeDef(TypedDict):
    Text: str,
    DataSource: str,
    BiasPosition: NotRequired[List[float]],
    FilterBBox: NotRequired[List[float]],
    FilterCountries: NotRequired[List[str]],
    MaxResults: NotRequired[int],
    ResultBBox: NotRequired[List[float]],
    Language: NotRequired[str],
    FilterCategories: NotRequired[List[str]],
```

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

## UpdateGeofenceCollectionRequestRequestTypeDef

```python
# UpdateGeofenceCollectionRequestRequestTypeDef definition

class UpdateGeofenceCollectionRequestRequestTypeDef(TypedDict):
    CollectionName: str,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    PricingPlanDataSource: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## UpdateRouteCalculatorRequestRequestTypeDef

```python
# UpdateRouteCalculatorRequestRequestTypeDef definition

class UpdateRouteCalculatorRequestRequestTypeDef(TypedDict):
    CalculatorName: str,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## UpdateTrackerRequestRequestTypeDef

```python
# UpdateTrackerRequestRequestTypeDef definition

class UpdateTrackerRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    PricingPlanDataSource: NotRequired[str],
    Description: NotRequired[str],
    PositionFiltering: NotRequired[PositionFilteringType],  # (2)
    EventBridgeEnabled: NotRequired[bool],
    KmsKeyEnableGeospatialQueries: NotRequired[bool],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-brackets: PositionFilteringType](./literals.md#positionfilteringtype) 
## ListKeysRequestRequestTypeDef

```python
# ListKeysRequestRequestTypeDef definition

class ListKeysRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filter: NotRequired[ApiKeyFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ApiKeyFilterTypeDef](./type_defs.md#apikeyfiltertypedef) 
## ListKeysResponseEntryTypeDef

```python
# ListKeysResponseEntryTypeDef definition

class ListKeysResponseEntryTypeDef(TypedDict):
    KeyName: str,
    ExpireTime: datetime,
    Restrictions: ApiKeyRestrictionsOutputTypeDef,  # (1)
    CreateTime: datetime,
    UpdateTime: datetime,
    Description: NotRequired[str],
```

1. See [:material-code-braces: ApiKeyRestrictionsOutputTypeDef](./type_defs.md#apikeyrestrictionsoutputtypedef) 
## BatchDeleteDevicePositionHistoryErrorTypeDef

```python
# BatchDeleteDevicePositionHistoryErrorTypeDef definition

class BatchDeleteDevicePositionHistoryErrorTypeDef(TypedDict):
    DeviceId: str,
    Error: BatchItemErrorTypeDef,  # (1)
```

1. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
## BatchDeleteGeofenceErrorTypeDef

```python
# BatchDeleteGeofenceErrorTypeDef definition

class BatchDeleteGeofenceErrorTypeDef(TypedDict):
    GeofenceId: str,
    Error: BatchItemErrorTypeDef,  # (1)
```

1. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
## BatchEvaluateGeofencesErrorTypeDef

```python
# BatchEvaluateGeofencesErrorTypeDef definition

class BatchEvaluateGeofencesErrorTypeDef(TypedDict):
    DeviceId: str,
    SampleTime: datetime,
    Error: BatchItemErrorTypeDef,  # (1)
```

1. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
## BatchGetDevicePositionErrorTypeDef

```python
# BatchGetDevicePositionErrorTypeDef definition

class BatchGetDevicePositionErrorTypeDef(TypedDict):
    DeviceId: str,
    Error: BatchItemErrorTypeDef,  # (1)
```

1. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
## BatchPutGeofenceErrorTypeDef

```python
# BatchPutGeofenceErrorTypeDef definition

class BatchPutGeofenceErrorTypeDef(TypedDict):
    GeofenceId: str,
    Error: BatchItemErrorTypeDef,  # (1)
```

1. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
## BatchUpdateDevicePositionErrorTypeDef

```python
# BatchUpdateDevicePositionErrorTypeDef definition

class BatchUpdateDevicePositionErrorTypeDef(TypedDict):
    DeviceId: str,
    SampleTime: datetime,
    Error: BatchItemErrorTypeDef,  # (1)
```

1. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
## CreateGeofenceCollectionResponseTypeDef

```python
# CreateGeofenceCollectionResponseTypeDef definition

class CreateGeofenceCollectionResponseTypeDef(TypedDict):
    CollectionName: str,
    CollectionArn: str,
    CreateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKeyResponseTypeDef

```python
# CreateKeyResponseTypeDef definition

class CreateKeyResponseTypeDef(TypedDict):
    Key: str,
    KeyArn: str,
    KeyName: str,
    CreateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMapResponseTypeDef

```python
# CreateMapResponseTypeDef definition

class CreateMapResponseTypeDef(TypedDict):
    MapName: str,
    MapArn: str,
    CreateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePlaceIndexResponseTypeDef

```python
# CreatePlaceIndexResponseTypeDef definition

class CreatePlaceIndexResponseTypeDef(TypedDict):
    IndexName: str,
    IndexArn: str,
    CreateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRouteCalculatorResponseTypeDef

```python
# CreateRouteCalculatorResponseTypeDef definition

class CreateRouteCalculatorResponseTypeDef(TypedDict):
    CalculatorName: str,
    CalculatorArn: str,
    CreateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrackerResponseTypeDef

```python
# CreateTrackerResponseTypeDef definition

class CreateTrackerResponseTypeDef(TypedDict):
    TrackerName: str,
    TrackerArn: str,
    CreateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGeofenceCollectionResponseTypeDef

```python
# DescribeGeofenceCollectionResponseTypeDef definition

class DescribeGeofenceCollectionResponseTypeDef(TypedDict):
    CollectionName: str,
    CollectionArn: str,
    Description: str,
    PricingPlan: PricingPlanType,  # (1)
    PricingPlanDataSource: str,
    KmsKeyId: str,
    Tags: Dict[str, str],
    CreateTime: datetime,
    UpdateTime: datetime,
    GeofenceCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeKeyResponseTypeDef

```python
# DescribeKeyResponseTypeDef definition

class DescribeKeyResponseTypeDef(TypedDict):
    Key: str,
    KeyArn: str,
    KeyName: str,
    Restrictions: ApiKeyRestrictionsOutputTypeDef,  # (1)
    CreateTime: datetime,
    ExpireTime: datetime,
    UpdateTime: datetime,
    Description: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApiKeyRestrictionsOutputTypeDef](./type_defs.md#apikeyrestrictionsoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRouteCalculatorResponseTypeDef

```python
# DescribeRouteCalculatorResponseTypeDef definition

class DescribeRouteCalculatorResponseTypeDef(TypedDict):
    CalculatorName: str,
    CalculatorArn: str,
    PricingPlan: PricingPlanType,  # (1)
    Description: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    DataSource: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrackerResponseTypeDef

```python
# DescribeTrackerResponseTypeDef definition

class DescribeTrackerResponseTypeDef(TypedDict):
    TrackerName: str,
    TrackerArn: str,
    Description: str,
    PricingPlan: PricingPlanType,  # (1)
    PricingPlanDataSource: str,
    Tags: Dict[str, str],
    CreateTime: datetime,
    UpdateTime: datetime,
    KmsKeyId: str,
    PositionFiltering: PositionFilteringType,  # (2)
    EventBridgeEnabled: bool,
    KmsKeyEnableGeospatialQueries: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-brackets: PositionFilteringType](./literals.md#positionfilteringtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMapGlyphsResponseTypeDef

```python
# GetMapGlyphsResponseTypeDef definition

class GetMapGlyphsResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    ContentType: str,
    CacheControl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMapSpritesResponseTypeDef

```python
# GetMapSpritesResponseTypeDef definition

class GetMapSpritesResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    ContentType: str,
    CacheControl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMapStyleDescriptorResponseTypeDef

```python
# GetMapStyleDescriptorResponseTypeDef definition

class GetMapStyleDescriptorResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    ContentType: str,
    CacheControl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMapTileResponseTypeDef

```python
# GetMapTileResponseTypeDef definition

class GetMapTileResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    ContentType: str,
    CacheControl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrackerConsumersResponseTypeDef

```python
# ListTrackerConsumersResponseTypeDef definition

class ListTrackerConsumersResponseTypeDef(TypedDict):
    ConsumerArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutGeofenceResponseTypeDef

```python
# PutGeofenceResponseTypeDef definition

class PutGeofenceResponseTypeDef(TypedDict):
    GeofenceId: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGeofenceCollectionResponseTypeDef

```python
# UpdateGeofenceCollectionResponseTypeDef definition

class UpdateGeofenceCollectionResponseTypeDef(TypedDict):
    CollectionName: str,
    CollectionArn: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKeyResponseTypeDef

```python
# UpdateKeyResponseTypeDef definition

class UpdateKeyResponseTypeDef(TypedDict):
    KeyArn: str,
    KeyName: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMapResponseTypeDef

```python
# UpdateMapResponseTypeDef definition

class UpdateMapResponseTypeDef(TypedDict):
    MapName: str,
    MapArn: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePlaceIndexResponseTypeDef

```python
# UpdatePlaceIndexResponseTypeDef definition

class UpdatePlaceIndexResponseTypeDef(TypedDict):
    IndexName: str,
    IndexArn: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRouteCalculatorResponseTypeDef

```python
# UpdateRouteCalculatorResponseTypeDef definition

class UpdateRouteCalculatorResponseTypeDef(TypedDict):
    CalculatorName: str,
    CalculatorArn: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrackerResponseTypeDef

```python
# UpdateTrackerResponseTypeDef definition

class UpdateTrackerResponseTypeDef(TypedDict):
    TrackerName: str,
    TrackerArn: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKeyRequestRequestTypeDef

```python
# CreateKeyRequestRequestTypeDef definition

class CreateKeyRequestRequestTypeDef(TypedDict):
    KeyName: str,
    Restrictions: ApiKeyRestrictionsTypeDef,  # (1)
    Description: NotRequired[str],
    ExpireTime: NotRequired[TimestampTypeDef],
    NoExpiry: NotRequired[bool],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ApiKeyRestrictionsTypeDef](./type_defs.md#apikeyrestrictionstypedef) 
## GetDevicePositionHistoryRequestRequestTypeDef

```python
# GetDevicePositionHistoryRequestRequestTypeDef definition

class GetDevicePositionHistoryRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    DeviceId: str,
    NextToken: NotRequired[str],
    StartTimeInclusive: NotRequired[TimestampTypeDef],
    EndTimeExclusive: NotRequired[TimestampTypeDef],
    MaxResults: NotRequired[int],
```

## UpdateKeyRequestRequestTypeDef

```python
# UpdateKeyRequestRequestTypeDef definition

class UpdateKeyRequestRequestTypeDef(TypedDict):
    KeyName: str,
    Description: NotRequired[str],
    ExpireTime: NotRequired[TimestampTypeDef],
    NoExpiry: NotRequired[bool],
    ForceUpdate: NotRequired[bool],
    Restrictions: NotRequired[ApiKeyRestrictionsTypeDef],  # (1)
```

1. See [:material-code-braces: ApiKeyRestrictionsTypeDef](./type_defs.md#apikeyrestrictionstypedef) 
## CalculateRouteTruckModeOptionsTypeDef

```python
# CalculateRouteTruckModeOptionsTypeDef definition

class CalculateRouteTruckModeOptionsTypeDef(TypedDict):
    AvoidFerries: NotRequired[bool],
    AvoidTolls: NotRequired[bool],
    Dimensions: NotRequired[TruckDimensionsTypeDef],  # (1)
    Weight: NotRequired[TruckWeightTypeDef],  # (2)
```

1. See [:material-code-braces: TruckDimensionsTypeDef](./type_defs.md#truckdimensionstypedef) 
2. See [:material-code-braces: TruckWeightTypeDef](./type_defs.md#truckweighttypedef) 
## GeofenceGeometryOutputTypeDef

```python
# GeofenceGeometryOutputTypeDef definition

class GeofenceGeometryOutputTypeDef(TypedDict):
    Polygon: NotRequired[List[List[List[float]]]],
    Circle: NotRequired[CircleOutputTypeDef],  # (1)
    Geobuf: NotRequired[bytes],
```

1. See [:material-code-braces: CircleOutputTypeDef](./type_defs.md#circleoutputtypedef) 
## CreateMapRequestRequestTypeDef

```python
# CreateMapRequestRequestTypeDef definition

class CreateMapRequestRequestTypeDef(TypedDict):
    MapName: str,
    Configuration: MapConfigurationTypeDef,  # (1)
    PricingPlan: NotRequired[PricingPlanType],  # (2)
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MapConfigurationTypeDef](./type_defs.md#mapconfigurationtypedef) 
2. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## CreatePlaceIndexRequestRequestTypeDef

```python
# CreatePlaceIndexRequestRequestTypeDef definition

class CreatePlaceIndexRequestRequestTypeDef(TypedDict):
    IndexName: str,
    DataSource: str,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    Description: NotRequired[str],
    DataSourceConfiguration: NotRequired[DataSourceConfigurationTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
## DescribePlaceIndexResponseTypeDef

```python
# DescribePlaceIndexResponseTypeDef definition

class DescribePlaceIndexResponseTypeDef(TypedDict):
    IndexName: str,
    IndexArn: str,
    PricingPlan: PricingPlanType,  # (1)
    Description: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    DataSource: str,
    DataSourceConfiguration: DataSourceConfigurationTypeDef,  # (2)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePlaceIndexRequestRequestTypeDef

```python
# UpdatePlaceIndexRequestRequestTypeDef definition

class UpdatePlaceIndexRequestRequestTypeDef(TypedDict):
    IndexName: str,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    Description: NotRequired[str],
    DataSourceConfiguration: NotRequired[DataSourceConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
## DescribeMapResponseTypeDef

```python
# DescribeMapResponseTypeDef definition

class DescribeMapResponseTypeDef(TypedDict):
    MapName: str,
    MapArn: str,
    PricingPlan: PricingPlanType,  # (1)
    DataSource: str,
    Configuration: MapConfigurationOutputTypeDef,  # (2)
    Description: str,
    Tags: Dict[str, str],
    CreateTime: datetime,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: MapConfigurationOutputTypeDef](./type_defs.md#mapconfigurationoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DevicePositionTypeDef

```python
# DevicePositionTypeDef definition

class DevicePositionTypeDef(TypedDict):
    SampleTime: datetime,
    ReceivedTime: datetime,
    Position: List[float],
    DeviceId: NotRequired[str],
    Accuracy: NotRequired[PositionalAccuracyTypeDef],  # (1)
    PositionProperties: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: PositionalAccuracyTypeDef](./type_defs.md#positionalaccuracytypedef) 
## DevicePositionUpdateTypeDef

```python
# DevicePositionUpdateTypeDef definition

class DevicePositionUpdateTypeDef(TypedDict):
    DeviceId: str,
    SampleTime: TimestampTypeDef,
    Position: Sequence[float],
    Accuracy: NotRequired[PositionalAccuracyTypeDef],  # (1)
    PositionProperties: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: PositionalAccuracyTypeDef](./type_defs.md#positionalaccuracytypedef) 
## GetDevicePositionResponseTypeDef

```python
# GetDevicePositionResponseTypeDef definition

class GetDevicePositionResponseTypeDef(TypedDict):
    DeviceId: str,
    SampleTime: datetime,
    ReceivedTime: datetime,
    Position: List[float],
    Accuracy: PositionalAccuracyTypeDef,  # (1)
    PositionProperties: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PositionalAccuracyTypeDef](./type_defs.md#positionalaccuracytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InferredStateTypeDef

```python
# InferredStateTypeDef definition

class InferredStateTypeDef(TypedDict):
    ProxyDetected: bool,
    Position: NotRequired[List[float]],
    Accuracy: NotRequired[PositionalAccuracyTypeDef],  # (1)
    DeviationDistance: NotRequired[float],
```

1. See [:material-code-braces: PositionalAccuracyTypeDef](./type_defs.md#positionalaccuracytypedef) 
## ListDevicePositionsResponseEntryTypeDef

```python
# ListDevicePositionsResponseEntryTypeDef definition

class ListDevicePositionsResponseEntryTypeDef(TypedDict):
    DeviceId: str,
    SampleTime: datetime,
    Position: List[float],
    Accuracy: NotRequired[PositionalAccuracyTypeDef],  # (1)
    PositionProperties: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: PositionalAccuracyTypeDef](./type_defs.md#positionalaccuracytypedef) 
## ForecastGeofenceEventsRequestRequestTypeDef

```python
# ForecastGeofenceEventsRequestRequestTypeDef definition

class ForecastGeofenceEventsRequestRequestTypeDef(TypedDict):
    CollectionName: str,
    DeviceState: ForecastGeofenceEventsDeviceStateTypeDef,  # (1)
    TimeHorizonMinutes: NotRequired[float],
    DistanceUnit: NotRequired[DistanceUnitType],  # (2)
    SpeedUnit: NotRequired[SpeedUnitType],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ForecastGeofenceEventsDeviceStateTypeDef](./type_defs.md#forecastgeofenceeventsdevicestatetypedef) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-brackets: SpeedUnitType](./literals.md#speedunittype) 
## ForecastGeofenceEventsRequestForecastGeofenceEventsPaginateTypeDef

```python
# ForecastGeofenceEventsRequestForecastGeofenceEventsPaginateTypeDef definition

class ForecastGeofenceEventsRequestForecastGeofenceEventsPaginateTypeDef(TypedDict):
    CollectionName: str,
    DeviceState: ForecastGeofenceEventsDeviceStateTypeDef,  # (1)
    TimeHorizonMinutes: NotRequired[float],
    DistanceUnit: NotRequired[DistanceUnitType],  # (2)
    SpeedUnit: NotRequired[SpeedUnitType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: ForecastGeofenceEventsDeviceStateTypeDef](./type_defs.md#forecastgeofenceeventsdevicestatetypedef) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-brackets: SpeedUnitType](./literals.md#speedunittype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef

```python
# GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef definition

class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(TypedDict):
    TrackerName: str,
    DeviceId: str,
    StartTimeInclusive: NotRequired[TimestampTypeDef],
    EndTimeExclusive: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef

```python
# ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef definition

class ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGeofencesRequestListGeofencesPaginateTypeDef

```python
# ListGeofencesRequestListGeofencesPaginateTypeDef definition

class ListGeofencesRequestListGeofencesPaginateTypeDef(TypedDict):
    CollectionName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKeysRequestListKeysPaginateTypeDef

```python
# ListKeysRequestListKeysPaginateTypeDef definition

class ListKeysRequestListKeysPaginateTypeDef(TypedDict):
    Filter: NotRequired[ApiKeyFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ApiKeyFilterTypeDef](./type_defs.md#apikeyfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMapsRequestListMapsPaginateTypeDef

```python
# ListMapsRequestListMapsPaginateTypeDef definition

class ListMapsRequestListMapsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef

```python
# ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef definition

class ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef

```python
# ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef definition

class ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef

```python
# ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef definition

class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(TypedDict):
    TrackerName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrackersRequestListTrackersPaginateTypeDef

```python
# ListTrackersRequestListTrackersPaginateTypeDef definition

class ListTrackersRequestListTrackersPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ForecastGeofenceEventsResponseTypeDef

```python
# ForecastGeofenceEventsResponseTypeDef definition

class ForecastGeofenceEventsResponseTypeDef(TypedDict):
    ForecastedEvents: List[ForecastedEventTypeDef],  # (1)
    DistanceUnit: DistanceUnitType,  # (2)
    SpeedUnit: SpeedUnitType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ForecastedEventTypeDef](./type_defs.md#forecastedeventtypedef) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-brackets: SpeedUnitType](./literals.md#speedunittype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LegTypeDef

```python
# LegTypeDef definition

class LegTypeDef(TypedDict):
    StartPosition: List[float],
    EndPosition: List[float],
    Distance: float,
    DurationSeconds: float,
    Steps: List[StepTypeDef],  # (2)
    Geometry: NotRequired[LegGeometryTypeDef],  # (1)
```

1. See [:material-code-braces: LegGeometryTypeDef](./type_defs.md#leggeometrytypedef) 
2. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
## ListDevicePositionsRequestListDevicePositionsPaginateTypeDef

```python
# ListDevicePositionsRequestListDevicePositionsPaginateTypeDef definition

class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(TypedDict):
    TrackerName: str,
    FilterGeometry: NotRequired[TrackingFilterGeometryTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TrackingFilterGeometryTypeDef](./type_defs.md#trackingfiltergeometrytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDevicePositionsRequestRequestTypeDef

```python
# ListDevicePositionsRequestRequestTypeDef definition

class ListDevicePositionsRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    FilterGeometry: NotRequired[TrackingFilterGeometryTypeDef],  # (1)
```

1. See [:material-code-braces: TrackingFilterGeometryTypeDef](./type_defs.md#trackingfiltergeometrytypedef) 
## ListGeofenceCollectionsResponseTypeDef

```python
# ListGeofenceCollectionsResponseTypeDef definition

class ListGeofenceCollectionsResponseTypeDef(TypedDict):
    Entries: List[ListGeofenceCollectionsResponseEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListGeofenceCollectionsResponseEntryTypeDef](./type_defs.md#listgeofencecollectionsresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMapsResponseTypeDef

```python
# ListMapsResponseTypeDef definition

class ListMapsResponseTypeDef(TypedDict):
    Entries: List[ListMapsResponseEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListMapsResponseEntryTypeDef](./type_defs.md#listmapsresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPlaceIndexesResponseTypeDef

```python
# ListPlaceIndexesResponseTypeDef definition

class ListPlaceIndexesResponseTypeDef(TypedDict):
    Entries: List[ListPlaceIndexesResponseEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListPlaceIndexesResponseEntryTypeDef](./type_defs.md#listplaceindexesresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRouteCalculatorsResponseTypeDef

```python
# ListRouteCalculatorsResponseTypeDef definition

class ListRouteCalculatorsResponseTypeDef(TypedDict):
    Entries: List[ListRouteCalculatorsResponseEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListRouteCalculatorsResponseEntryTypeDef](./type_defs.md#listroutecalculatorsresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrackersResponseTypeDef

```python
# ListTrackersResponseTypeDef definition

class ListTrackersResponseTypeDef(TypedDict):
    Entries: List[ListTrackersResponseEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListTrackersResponseEntryTypeDef](./type_defs.md#listtrackersresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LteCellDetailsTypeDef

```python
# LteCellDetailsTypeDef definition

class LteCellDetailsTypeDef(TypedDict):
    CellId: int,
    Mcc: int,
    Mnc: int,
    LocalId: NotRequired[LteLocalIdTypeDef],  # (1)
    NetworkMeasurements: NotRequired[Sequence[LteNetworkMeasurementsTypeDef]],  # (2)
    TimingAdvance: NotRequired[int],
    NrCapable: NotRequired[bool],
    Rsrp: NotRequired[int],
    Rsrq: NotRequired[float],
    Tac: NotRequired[int],
```

1. See [:material-code-braces: LteLocalIdTypeDef](./type_defs.md#ltelocalidtypedef) 
2. See [:material-code-braces: LteNetworkMeasurementsTypeDef](./type_defs.md#ltenetworkmeasurementstypedef) 
## UpdateMapRequestRequestTypeDef

```python
# UpdateMapRequestRequestTypeDef definition

class UpdateMapRequestRequestTypeDef(TypedDict):
    MapName: str,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    Description: NotRequired[str],
    ConfigurationUpdate: NotRequired[MapConfigurationUpdateTypeDef],  # (2)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: MapConfigurationUpdateTypeDef](./type_defs.md#mapconfigurationupdatetypedef) 
## PlaceTypeDef

```python
# PlaceTypeDef definition

class PlaceTypeDef(TypedDict):
    Geometry: PlaceGeometryTypeDef,  # (1)
    Label: NotRequired[str],
    AddressNumber: NotRequired[str],
    Street: NotRequired[str],
    Neighborhood: NotRequired[str],
    Municipality: NotRequired[str],
    SubRegion: NotRequired[str],
    Region: NotRequired[str],
    Country: NotRequired[str],
    PostalCode: NotRequired[str],
    Interpolated: NotRequired[bool],
    TimeZone: NotRequired[TimeZoneTypeDef],  # (2)
    UnitType: NotRequired[str],
    UnitNumber: NotRequired[str],
    Categories: NotRequired[List[str]],
    SupplementalCategories: NotRequired[List[str]],
    SubMunicipality: NotRequired[str],
```

1. See [:material-code-braces: PlaceGeometryTypeDef](./type_defs.md#placegeometrytypedef) 
2. See [:material-code-braces: TimeZoneTypeDef](./type_defs.md#timezonetypedef) 
## RouteMatrixEntryTypeDef

```python
# RouteMatrixEntryTypeDef definition

class RouteMatrixEntryTypeDef(TypedDict):
    Distance: NotRequired[float],
    DurationSeconds: NotRequired[float],
    Error: NotRequired[RouteMatrixEntryErrorTypeDef],  # (1)
```

1. See [:material-code-braces: RouteMatrixEntryErrorTypeDef](./type_defs.md#routematrixentryerrortypedef) 
## SearchPlaceIndexForSuggestionsResponseTypeDef

```python
# SearchPlaceIndexForSuggestionsResponseTypeDef definition

class SearchPlaceIndexForSuggestionsResponseTypeDef(TypedDict):
    Summary: SearchPlaceIndexForSuggestionsSummaryTypeDef,  # (1)
    Results: List[SearchForSuggestionsResultTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SearchPlaceIndexForSuggestionsSummaryTypeDef](./type_defs.md#searchplaceindexforsuggestionssummarytypedef) 
2. See [:material-code-braces: SearchForSuggestionsResultTypeDef](./type_defs.md#searchforsuggestionsresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKeysResponseTypeDef

```python
# ListKeysResponseTypeDef definition

class ListKeysResponseTypeDef(TypedDict):
    Entries: List[ListKeysResponseEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListKeysResponseEntryTypeDef](./type_defs.md#listkeysresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteDevicePositionHistoryResponseTypeDef

```python
# BatchDeleteDevicePositionHistoryResponseTypeDef definition

class BatchDeleteDevicePositionHistoryResponseTypeDef(TypedDict):
    Errors: List[BatchDeleteDevicePositionHistoryErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteDevicePositionHistoryErrorTypeDef](./type_defs.md#batchdeletedevicepositionhistoryerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteGeofenceResponseTypeDef

```python
# BatchDeleteGeofenceResponseTypeDef definition

class BatchDeleteGeofenceResponseTypeDef(TypedDict):
    Errors: List[BatchDeleteGeofenceErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteGeofenceErrorTypeDef](./type_defs.md#batchdeletegeofenceerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchEvaluateGeofencesResponseTypeDef

```python
# BatchEvaluateGeofencesResponseTypeDef definition

class BatchEvaluateGeofencesResponseTypeDef(TypedDict):
    Errors: List[BatchEvaluateGeofencesErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchEvaluateGeofencesErrorTypeDef](./type_defs.md#batchevaluategeofenceserrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutGeofenceResponseTypeDef

```python
# BatchPutGeofenceResponseTypeDef definition

class BatchPutGeofenceResponseTypeDef(TypedDict):
    Successes: List[BatchPutGeofenceSuccessTypeDef],  # (1)
    Errors: List[BatchPutGeofenceErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchPutGeofenceSuccessTypeDef](./type_defs.md#batchputgeofencesuccesstypedef) 
2. See [:material-code-braces: BatchPutGeofenceErrorTypeDef](./type_defs.md#batchputgeofenceerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateDevicePositionResponseTypeDef

```python
# BatchUpdateDevicePositionResponseTypeDef definition

class BatchUpdateDevicePositionResponseTypeDef(TypedDict):
    Errors: List[BatchUpdateDevicePositionErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchUpdateDevicePositionErrorTypeDef](./type_defs.md#batchupdatedevicepositionerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CalculateRouteMatrixRequestRequestTypeDef

```python
# CalculateRouteMatrixRequestRequestTypeDef definition

class CalculateRouteMatrixRequestRequestTypeDef(TypedDict):
    CalculatorName: str,
    DeparturePositions: Sequence[Sequence[float]],
    DestinationPositions: Sequence[Sequence[float]],
    TravelMode: NotRequired[TravelModeType],  # (1)
    DepartureTime: NotRequired[TimestampTypeDef],
    DepartNow: NotRequired[bool],
    DistanceUnit: NotRequired[DistanceUnitType],  # (2)
    CarModeOptions: NotRequired[CalculateRouteCarModeOptionsTypeDef],  # (3)
    TruckModeOptions: NotRequired[CalculateRouteTruckModeOptionsTypeDef],  # (4)
    Key: NotRequired[str],
```

1. See [:material-code-brackets: TravelModeType](./literals.md#travelmodetype) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-braces: CalculateRouteCarModeOptionsTypeDef](./type_defs.md#calculateroutecarmodeoptionstypedef) 
4. See [:material-code-braces: CalculateRouteTruckModeOptionsTypeDef](./type_defs.md#calculateroutetruckmodeoptionstypedef) 
## CalculateRouteRequestRequestTypeDef

```python
# CalculateRouteRequestRequestTypeDef definition

class CalculateRouteRequestRequestTypeDef(TypedDict):
    CalculatorName: str,
    DeparturePosition: Sequence[float],
    DestinationPosition: Sequence[float],
    WaypointPositions: NotRequired[Sequence[Sequence[float]]],
    TravelMode: NotRequired[TravelModeType],  # (1)
    DepartureTime: NotRequired[TimestampTypeDef],
    DepartNow: NotRequired[bool],
    DistanceUnit: NotRequired[DistanceUnitType],  # (2)
    IncludeLegGeometry: NotRequired[bool],
    CarModeOptions: NotRequired[CalculateRouteCarModeOptionsTypeDef],  # (3)
    TruckModeOptions: NotRequired[CalculateRouteTruckModeOptionsTypeDef],  # (4)
    ArrivalTime: NotRequired[TimestampTypeDef],
    OptimizeFor: NotRequired[OptimizationModeType],  # (5)
    Key: NotRequired[str],
```

1. See [:material-code-brackets: TravelModeType](./literals.md#travelmodetype) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-braces: CalculateRouteCarModeOptionsTypeDef](./type_defs.md#calculateroutecarmodeoptionstypedef) 
4. See [:material-code-braces: CalculateRouteTruckModeOptionsTypeDef](./type_defs.md#calculateroutetruckmodeoptionstypedef) 
5. See [:material-code-brackets: OptimizationModeType](./literals.md#optimizationmodetype) 
## GetGeofenceResponseTypeDef

```python
# GetGeofenceResponseTypeDef definition

class GetGeofenceResponseTypeDef(TypedDict):
    GeofenceId: str,
    Geometry: GeofenceGeometryOutputTypeDef,  # (1)
    Status: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    GeofenceProperties: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeofenceGeometryOutputTypeDef](./type_defs.md#geofencegeometryoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGeofenceResponseEntryTypeDef

```python
# ListGeofenceResponseEntryTypeDef definition

class ListGeofenceResponseEntryTypeDef(TypedDict):
    GeofenceId: str,
    Geometry: GeofenceGeometryOutputTypeDef,  # (1)
    Status: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    GeofenceProperties: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: GeofenceGeometryOutputTypeDef](./type_defs.md#geofencegeometryoutputtypedef) 
## GeofenceGeometryTypeDef

```python
# GeofenceGeometryTypeDef definition

class GeofenceGeometryTypeDef(TypedDict):
    Polygon: NotRequired[Sequence[Sequence[Sequence[float]]]],
    Circle: NotRequired[CircleUnionTypeDef],  # (1)
    Geobuf: NotRequired[BlobTypeDef],
```

1. See [:material-code-braces: CircleTypeDef](./type_defs.md#circletypedef) [:material-code-braces: CircleOutputTypeDef](./type_defs.md#circleoutputtypedef) 
## BatchGetDevicePositionResponseTypeDef

```python
# BatchGetDevicePositionResponseTypeDef definition

class BatchGetDevicePositionResponseTypeDef(TypedDict):
    Errors: List[BatchGetDevicePositionErrorTypeDef],  # (1)
    DevicePositions: List[DevicePositionTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchGetDevicePositionErrorTypeDef](./type_defs.md#batchgetdevicepositionerrortypedef) 
2. See [:material-code-braces: DevicePositionTypeDef](./type_defs.md#devicepositiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDevicePositionHistoryResponseTypeDef

```python
# GetDevicePositionHistoryResponseTypeDef definition

class GetDevicePositionHistoryResponseTypeDef(TypedDict):
    DevicePositions: List[DevicePositionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DevicePositionTypeDef](./type_defs.md#devicepositiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchEvaluateGeofencesRequestRequestTypeDef

```python
# BatchEvaluateGeofencesRequestRequestTypeDef definition

class BatchEvaluateGeofencesRequestRequestTypeDef(TypedDict):
    CollectionName: str,
    DevicePositionUpdates: Sequence[DevicePositionUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: DevicePositionUpdateTypeDef](./type_defs.md#devicepositionupdatetypedef) 
## BatchUpdateDevicePositionRequestRequestTypeDef

```python
# BatchUpdateDevicePositionRequestRequestTypeDef definition

class BatchUpdateDevicePositionRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    Updates: Sequence[DevicePositionUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: DevicePositionUpdateTypeDef](./type_defs.md#devicepositionupdatetypedef) 
## VerifyDevicePositionResponseTypeDef

```python
# VerifyDevicePositionResponseTypeDef definition

class VerifyDevicePositionResponseTypeDef(TypedDict):
    InferredState: InferredStateTypeDef,  # (1)
    DeviceId: str,
    SampleTime: datetime,
    ReceivedTime: datetime,
    DistanceUnit: DistanceUnitType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: InferredStateTypeDef](./type_defs.md#inferredstatetypedef) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDevicePositionsResponseTypeDef

```python
# ListDevicePositionsResponseTypeDef definition

class ListDevicePositionsResponseTypeDef(TypedDict):
    Entries: List[ListDevicePositionsResponseEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListDevicePositionsResponseEntryTypeDef](./type_defs.md#listdevicepositionsresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CalculateRouteResponseTypeDef

```python
# CalculateRouteResponseTypeDef definition

class CalculateRouteResponseTypeDef(TypedDict):
    Legs: List[LegTypeDef],  # (1)
    Summary: CalculateRouteSummaryTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: LegTypeDef](./type_defs.md#legtypedef) 
2. See [:material-code-braces: CalculateRouteSummaryTypeDef](./type_defs.md#calculateroutesummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CellSignalsTypeDef

```python
# CellSignalsTypeDef definition

class CellSignalsTypeDef(TypedDict):
    LteCellDetails: Sequence[LteCellDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: LteCellDetailsTypeDef](./type_defs.md#ltecelldetailstypedef) 
## GetPlaceResponseTypeDef

```python
# GetPlaceResponseTypeDef definition

class GetPlaceResponseTypeDef(TypedDict):
    Place: PlaceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaceTypeDef](./type_defs.md#placetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchForPositionResultTypeDef

```python
# SearchForPositionResultTypeDef definition

class SearchForPositionResultTypeDef(TypedDict):
    Place: PlaceTypeDef,  # (1)
    Distance: float,
    PlaceId: NotRequired[str],
```

1. See [:material-code-braces: PlaceTypeDef](./type_defs.md#placetypedef) 
## SearchForTextResultTypeDef

```python
# SearchForTextResultTypeDef definition

class SearchForTextResultTypeDef(TypedDict):
    Place: PlaceTypeDef,  # (1)
    Distance: NotRequired[float],
    Relevance: NotRequired[float],
    PlaceId: NotRequired[str],
```

1. See [:material-code-braces: PlaceTypeDef](./type_defs.md#placetypedef) 
## CalculateRouteMatrixResponseTypeDef

```python
# CalculateRouteMatrixResponseTypeDef definition

class CalculateRouteMatrixResponseTypeDef(TypedDict):
    RouteMatrix: List[List[RouteMatrixEntryTypeDef]],  # (1)
    SnappedDeparturePositions: List[List[float]],
    SnappedDestinationPositions: List[List[float]],
    Summary: CalculateRouteMatrixSummaryTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RouteMatrixEntryTypeDef](./type_defs.md#routematrixentrytypedef) 
2. See [:material-code-braces: CalculateRouteMatrixSummaryTypeDef](./type_defs.md#calculateroutematrixsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGeofencesResponseTypeDef

```python
# ListGeofencesResponseTypeDef definition

class ListGeofencesResponseTypeDef(TypedDict):
    Entries: List[ListGeofenceResponseEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListGeofenceResponseEntryTypeDef](./type_defs.md#listgeofenceresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutGeofenceRequestRequestTypeDef

```python
# PutGeofenceRequestRequestTypeDef definition

class PutGeofenceRequestRequestTypeDef(TypedDict):
    CollectionName: str,
    GeofenceId: str,
    Geometry: GeofenceGeometryTypeDef,  # (1)
    GeofenceProperties: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: GeofenceGeometryTypeDef](./type_defs.md#geofencegeometrytypedef) 
## DeviceStateTypeDef

```python
# DeviceStateTypeDef definition

class DeviceStateTypeDef(TypedDict):
    DeviceId: str,
    SampleTime: TimestampTypeDef,
    Position: Sequence[float],
    Accuracy: NotRequired[PositionalAccuracyTypeDef],  # (1)
    Ipv4Address: NotRequired[str],
    WiFiAccessPoints: NotRequired[Sequence[WiFiAccessPointTypeDef]],  # (2)
    CellSignals: NotRequired[CellSignalsTypeDef],  # (3)
```

1. See [:material-code-braces: PositionalAccuracyTypeDef](./type_defs.md#positionalaccuracytypedef) 
2. See [:material-code-braces: WiFiAccessPointTypeDef](./type_defs.md#wifiaccesspointtypedef) 
3. See [:material-code-braces: CellSignalsTypeDef](./type_defs.md#cellsignalstypedef) 
## SearchPlaceIndexForPositionResponseTypeDef

```python
# SearchPlaceIndexForPositionResponseTypeDef definition

class SearchPlaceIndexForPositionResponseTypeDef(TypedDict):
    Summary: SearchPlaceIndexForPositionSummaryTypeDef,  # (1)
    Results: List[SearchForPositionResultTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SearchPlaceIndexForPositionSummaryTypeDef](./type_defs.md#searchplaceindexforpositionsummarytypedef) 
2. See [:material-code-braces: SearchForPositionResultTypeDef](./type_defs.md#searchforpositionresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchPlaceIndexForTextResponseTypeDef

```python
# SearchPlaceIndexForTextResponseTypeDef definition

class SearchPlaceIndexForTextResponseTypeDef(TypedDict):
    Summary: SearchPlaceIndexForTextSummaryTypeDef,  # (1)
    Results: List[SearchForTextResultTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SearchPlaceIndexForTextSummaryTypeDef](./type_defs.md#searchplaceindexfortextsummarytypedef) 
2. See [:material-code-braces: SearchForTextResultTypeDef](./type_defs.md#searchfortextresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutGeofenceRequestEntryTypeDef

```python
# BatchPutGeofenceRequestEntryTypeDef definition

class BatchPutGeofenceRequestEntryTypeDef(TypedDict):
    GeofenceId: str,
    Geometry: GeofenceGeometryUnionTypeDef,  # (1)
    GeofenceProperties: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: GeofenceGeometryTypeDef](./type_defs.md#geofencegeometrytypedef) [:material-code-braces: GeofenceGeometryOutputTypeDef](./type_defs.md#geofencegeometryoutputtypedef) 
## VerifyDevicePositionRequestRequestTypeDef

```python
# VerifyDevicePositionRequestRequestTypeDef definition

class VerifyDevicePositionRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    DeviceState: DeviceStateTypeDef,  # (1)
    DistanceUnit: NotRequired[DistanceUnitType],  # (2)
```

1. See [:material-code-braces: DeviceStateTypeDef](./type_defs.md#devicestatetypedef) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
## BatchPutGeofenceRequestRequestTypeDef

```python
# BatchPutGeofenceRequestRequestTypeDef definition

class BatchPutGeofenceRequestRequestTypeDef(TypedDict):
    CollectionName: str,
    Entries: Sequence[BatchPutGeofenceRequestEntryTypeDef],  # (1)
```

1. See [:material-code-braces: BatchPutGeofenceRequestEntryTypeDef](./type_defs.md#batchputgeofencerequestentrytypedef) 
