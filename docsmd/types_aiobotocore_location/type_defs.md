# Type definitions

> [Index](../README.md) > [LocationService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
    type annotations stubs module [types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ApiKeyFilterTypeDef

```python
# ApiKeyFilterTypeDef definition

class ApiKeyFilterTypeDef(TypedDict):
    KeyStatus: NotRequired[StatusType],  # (1)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
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
    ConsumerArn: str,
    TrackerName: str,
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
    DeviceIds: Sequence[str],
    TrackerName: str,
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
    DeviceIds: Sequence[str],
    TrackerName: str,
```

## BatchPutGeofenceSuccessTypeDef

```python
# BatchPutGeofenceSuccessTypeDef definition

class BatchPutGeofenceSuccessTypeDef(TypedDict):
    CreateTime: datetime,
    GeofenceId: str,
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
    DistanceUnit: DistanceUnitType,  # (1)
    ErrorCount: int,
    RouteCount: int,
```

1. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
## CalculateRouteSummaryTypeDef

```python
# CalculateRouteSummaryTypeDef definition

class CalculateRouteSummaryTypeDef(TypedDict):
    DataSource: str,
    Distance: float,
    DistanceUnit: DistanceUnitType,  # (1)
    DurationSeconds: float,
    RouteBBox: List[float],
```

1. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
## TruckDimensionsTypeDef

```python
# TruckDimensionsTypeDef definition

class TruckDimensionsTypeDef(TypedDict):
    Height: NotRequired[float],
    Length: NotRequired[float],
    Unit: NotRequired[DimensionUnitType],  # (1)
    Width: NotRequired[float],
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
    Description: NotRequired[str],
    KmsKeyId: NotRequired[str],
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    PricingPlanDataSource: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## MapConfigurationTypeDef

```python
# MapConfigurationTypeDef definition

class MapConfigurationTypeDef(TypedDict):
    Style: str,
    PoliticalView: NotRequired[str],
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
    Description: NotRequired[str],
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## CreateTrackerRequestRequestTypeDef

```python
# CreateTrackerRequestRequestTypeDef definition

class CreateTrackerRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    Description: NotRequired[str],
    EventBridgeEnabled: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    PositionFiltering: NotRequired[PositionFilteringType],  # (1)
    PricingPlan: NotRequired[PricingPlanType],  # (2)
    PricingPlanDataSource: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PositionFilteringType](./literals.md#positionfilteringtype) 
2. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
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

## DisassociateTrackerConsumerRequestRequestTypeDef

```python
# DisassociateTrackerConsumerRequestRequestTypeDef definition

class DisassociateTrackerConsumerRequestRequestTypeDef(TypedDict):
    ConsumerArn: str,
    TrackerName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetDevicePositionRequestRequestTypeDef

```python
# GetDevicePositionRequestRequestTypeDef definition

class GetDevicePositionRequestRequestTypeDef(TypedDict):
    DeviceId: str,
    TrackerName: str,
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
    FontStack: str,
    FontUnicodeRange: str,
    MapName: str,
    Key: NotRequired[str],
```

## GetMapSpritesRequestRequestTypeDef

```python
# GetMapSpritesRequestRequestTypeDef definition

class GetMapSpritesRequestRequestTypeDef(TypedDict):
    FileName: str,
    MapName: str,
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
    X: str,
    Y: str,
    Z: str,
    Key: NotRequired[str],
```

## GetPlaceRequestRequestTypeDef

```python
# GetPlaceRequestRequestTypeDef definition

class GetPlaceRequestRequestTypeDef(TypedDict):
    IndexName: str,
    PlaceId: str,
    Key: NotRequired[str],
    Language: NotRequired[str],
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
    Distance: float,
    DurationSeconds: float,
    EndPosition: List[float],
    StartPosition: List[float],
    GeometryOffset: NotRequired[int],
```

## ListDevicePositionsRequestRequestTypeDef

```python
# ListDevicePositionsRequestRequestTypeDef definition

class ListDevicePositionsRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
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
    CreateTime: datetime,
    Description: str,
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
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
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
    CreateTime: datetime,
    DataSource: str,
    Description: str,
    MapName: str,
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
    CreateTime: datetime,
    DataSource: str,
    Description: str,
    IndexName: str,
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
    CreateTime: datetime,
    DataSource: str,
    Description: str,
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
    CreateTime: datetime,
    Description: str,
    TrackerName: str,
    UpdateTime: datetime,
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    PricingPlanDataSource: NotRequired[str],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## MapConfigurationUpdateTypeDef

```python
# MapConfigurationUpdateTypeDef definition

class MapConfigurationUpdateTypeDef(TypedDict):
    PoliticalView: NotRequired[str],
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
    Categories: NotRequired[List[str]],
    PlaceId: NotRequired[str],
    SupplementalCategories: NotRequired[List[str]],
```

## SearchPlaceIndexForPositionRequestRequestTypeDef

```python
# SearchPlaceIndexForPositionRequestRequestTypeDef definition

class SearchPlaceIndexForPositionRequestRequestTypeDef(TypedDict):
    IndexName: str,
    Position: Sequence[float],
    Key: NotRequired[str],
    Language: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SearchPlaceIndexForPositionSummaryTypeDef

```python
# SearchPlaceIndexForPositionSummaryTypeDef definition

class SearchPlaceIndexForPositionSummaryTypeDef(TypedDict):
    DataSource: str,
    Position: List[float],
    Language: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SearchPlaceIndexForSuggestionsRequestRequestTypeDef

```python
# SearchPlaceIndexForSuggestionsRequestRequestTypeDef definition

class SearchPlaceIndexForSuggestionsRequestRequestTypeDef(TypedDict):
    IndexName: str,
    Text: str,
    BiasPosition: NotRequired[Sequence[float]],
    FilterBBox: NotRequired[Sequence[float]],
    FilterCategories: NotRequired[Sequence[str]],
    FilterCountries: NotRequired[Sequence[str]],
    Key: NotRequired[str],
    Language: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SearchPlaceIndexForSuggestionsSummaryTypeDef

```python
# SearchPlaceIndexForSuggestionsSummaryTypeDef definition

class SearchPlaceIndexForSuggestionsSummaryTypeDef(TypedDict):
    DataSource: str,
    Text: str,
    BiasPosition: NotRequired[List[float]],
    FilterBBox: NotRequired[List[float]],
    FilterCategories: NotRequired[List[str]],
    FilterCountries: NotRequired[List[str]],
    Language: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SearchPlaceIndexForTextRequestRequestTypeDef

```python
# SearchPlaceIndexForTextRequestRequestTypeDef definition

class SearchPlaceIndexForTextRequestRequestTypeDef(TypedDict):
    IndexName: str,
    Text: str,
    BiasPosition: NotRequired[Sequence[float]],
    FilterBBox: NotRequired[Sequence[float]],
    FilterCategories: NotRequired[Sequence[str]],
    FilterCountries: NotRequired[Sequence[str]],
    Key: NotRequired[str],
    Language: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SearchPlaceIndexForTextSummaryTypeDef

```python
# SearchPlaceIndexForTextSummaryTypeDef definition

class SearchPlaceIndexForTextSummaryTypeDef(TypedDict):
    DataSource: str,
    Text: str,
    BiasPosition: NotRequired[List[float]],
    FilterBBox: NotRequired[List[float]],
    FilterCategories: NotRequired[List[str]],
    FilterCountries: NotRequired[List[str]],
    Language: NotRequired[str],
    MaxResults: NotRequired[int],
    ResultBBox: NotRequired[List[float]],
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
    Description: NotRequired[str],
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    PricingPlanDataSource: NotRequired[str],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## UpdateRouteCalculatorRequestRequestTypeDef

```python
# UpdateRouteCalculatorRequestRequestTypeDef definition

class UpdateRouteCalculatorRequestRequestTypeDef(TypedDict):
    CalculatorName: str,
    Description: NotRequired[str],
    PricingPlan: NotRequired[PricingPlanType],  # (1)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## UpdateTrackerRequestRequestTypeDef

```python
# UpdateTrackerRequestRequestTypeDef definition

class UpdateTrackerRequestRequestTypeDef(TypedDict):
    TrackerName: str,
    Description: NotRequired[str],
    EventBridgeEnabled: NotRequired[bool],
    PositionFiltering: NotRequired[PositionFilteringType],  # (1)
    PricingPlan: NotRequired[PricingPlanType],  # (2)
    PricingPlanDataSource: NotRequired[str],
```

1. See [:material-code-brackets: PositionFilteringType](./literals.md#positionfilteringtype) 
2. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## ListKeysRequestRequestTypeDef

```python
# ListKeysRequestRequestTypeDef definition

class ListKeysRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[ApiKeyFilterTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApiKeyFilterTypeDef](./type_defs.md#apikeyfiltertypedef) 
## ListKeysResponseEntryTypeDef

```python
# ListKeysResponseEntryTypeDef definition

class ListKeysResponseEntryTypeDef(TypedDict):
    CreateTime: datetime,
    ExpireTime: datetime,
    KeyName: str,
    Restrictions: ApiKeyRestrictionsTypeDef,  # (1)
    UpdateTime: datetime,
    Description: NotRequired[str],
```

1. See [:material-code-braces: ApiKeyRestrictionsTypeDef](./type_defs.md#apikeyrestrictionstypedef) 
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
    Error: BatchItemErrorTypeDef,  # (1)
    GeofenceId: str,
```

1. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
## BatchEvaluateGeofencesErrorTypeDef

```python
# BatchEvaluateGeofencesErrorTypeDef definition

class BatchEvaluateGeofencesErrorTypeDef(TypedDict):
    DeviceId: str,
    Error: BatchItemErrorTypeDef,  # (1)
    SampleTime: datetime,
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
    Error: BatchItemErrorTypeDef,  # (1)
    GeofenceId: str,
```

1. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
## BatchUpdateDevicePositionErrorTypeDef

```python
# BatchUpdateDevicePositionErrorTypeDef definition

class BatchUpdateDevicePositionErrorTypeDef(TypedDict):
    DeviceId: str,
    Error: BatchItemErrorTypeDef,  # (1)
    SampleTime: datetime,
```

1. See [:material-code-braces: BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef) 
## CreateGeofenceCollectionResponseTypeDef

```python
# CreateGeofenceCollectionResponseTypeDef definition

class CreateGeofenceCollectionResponseTypeDef(TypedDict):
    CollectionArn: str,
    CollectionName: str,
    CreateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKeyResponseTypeDef

```python
# CreateKeyResponseTypeDef definition

class CreateKeyResponseTypeDef(TypedDict):
    CreateTime: datetime,
    Key: str,
    KeyArn: str,
    KeyName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMapResponseTypeDef

```python
# CreateMapResponseTypeDef definition

class CreateMapResponseTypeDef(TypedDict):
    CreateTime: datetime,
    MapArn: str,
    MapName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePlaceIndexResponseTypeDef

```python
# CreatePlaceIndexResponseTypeDef definition

class CreatePlaceIndexResponseTypeDef(TypedDict):
    CreateTime: datetime,
    IndexArn: str,
    IndexName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRouteCalculatorResponseTypeDef

```python
# CreateRouteCalculatorResponseTypeDef definition

class CreateRouteCalculatorResponseTypeDef(TypedDict):
    CalculatorArn: str,
    CalculatorName: str,
    CreateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrackerResponseTypeDef

```python
# CreateTrackerResponseTypeDef definition

class CreateTrackerResponseTypeDef(TypedDict):
    CreateTime: datetime,
    TrackerArn: str,
    TrackerName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGeofenceCollectionResponseTypeDef

```python
# DescribeGeofenceCollectionResponseTypeDef definition

class DescribeGeofenceCollectionResponseTypeDef(TypedDict):
    CollectionArn: str,
    CollectionName: str,
    CreateTime: datetime,
    Description: str,
    KmsKeyId: str,
    PricingPlan: PricingPlanType,  # (1)
    PricingPlanDataSource: str,
    Tags: Dict[str, str],
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeKeyResponseTypeDef

```python
# DescribeKeyResponseTypeDef definition

class DescribeKeyResponseTypeDef(TypedDict):
    CreateTime: datetime,
    Description: str,
    ExpireTime: datetime,
    Key: str,
    KeyArn: str,
    KeyName: str,
    Restrictions: ApiKeyRestrictionsTypeDef,  # (1)
    Tags: Dict[str, str],
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApiKeyRestrictionsTypeDef](./type_defs.md#apikeyrestrictionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRouteCalculatorResponseTypeDef

```python
# DescribeRouteCalculatorResponseTypeDef definition

class DescribeRouteCalculatorResponseTypeDef(TypedDict):
    CalculatorArn: str,
    CalculatorName: str,
    CreateTime: datetime,
    DataSource: str,
    Description: str,
    PricingPlan: PricingPlanType,  # (1)
    Tags: Dict[str, str],
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrackerResponseTypeDef

```python
# DescribeTrackerResponseTypeDef definition

class DescribeTrackerResponseTypeDef(TypedDict):
    CreateTime: datetime,
    Description: str,
    EventBridgeEnabled: bool,
    KmsKeyId: str,
    PositionFiltering: PositionFilteringType,  # (1)
    PricingPlan: PricingPlanType,  # (2)
    PricingPlanDataSource: str,
    Tags: Dict[str, str],
    TrackerArn: str,
    TrackerName: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PositionFilteringType](./literals.md#positionfilteringtype) 
2. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMapGlyphsResponseTypeDef

```python
# GetMapGlyphsResponseTypeDef definition

class GetMapGlyphsResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    CacheControl: str,
    ContentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMapSpritesResponseTypeDef

```python
# GetMapSpritesResponseTypeDef definition

class GetMapSpritesResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    CacheControl: str,
    ContentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMapStyleDescriptorResponseTypeDef

```python
# GetMapStyleDescriptorResponseTypeDef definition

class GetMapStyleDescriptorResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    CacheControl: str,
    ContentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMapTileResponseTypeDef

```python
# GetMapTileResponseTypeDef definition

class GetMapTileResponseTypeDef(TypedDict):
    Blob: StreamingBody,
    CacheControl: str,
    ContentType: str,
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutGeofenceResponseTypeDef

```python
# PutGeofenceResponseTypeDef definition

class PutGeofenceResponseTypeDef(TypedDict):
    CreateTime: datetime,
    GeofenceId: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGeofenceCollectionResponseTypeDef

```python
# UpdateGeofenceCollectionResponseTypeDef definition

class UpdateGeofenceCollectionResponseTypeDef(TypedDict):
    CollectionArn: str,
    CollectionName: str,
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
    MapArn: str,
    MapName: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePlaceIndexResponseTypeDef

```python
# UpdatePlaceIndexResponseTypeDef definition

class UpdatePlaceIndexResponseTypeDef(TypedDict):
    IndexArn: str,
    IndexName: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRouteCalculatorResponseTypeDef

```python
# UpdateRouteCalculatorResponseTypeDef definition

class UpdateRouteCalculatorResponseTypeDef(TypedDict):
    CalculatorArn: str,
    CalculatorName: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrackerResponseTypeDef

```python
# UpdateTrackerResponseTypeDef definition

class UpdateTrackerResponseTypeDef(TypedDict):
    TrackerArn: str,
    TrackerName: str,
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
    ExpireTime: NotRequired[Union[datetime, str]],
    NoExpiry: NotRequired[bool],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ApiKeyRestrictionsTypeDef](./type_defs.md#apikeyrestrictionstypedef) 
## GetDevicePositionHistoryRequestRequestTypeDef

```python
# GetDevicePositionHistoryRequestRequestTypeDef definition

class GetDevicePositionHistoryRequestRequestTypeDef(TypedDict):
    DeviceId: str,
    TrackerName: str,
    EndTimeExclusive: NotRequired[Union[datetime, str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    StartTimeInclusive: NotRequired[Union[datetime, str]],
```

## UpdateKeyRequestRequestTypeDef

```python
# UpdateKeyRequestRequestTypeDef definition

class UpdateKeyRequestRequestTypeDef(TypedDict):
    KeyName: str,
    Description: NotRequired[str],
    ExpireTime: NotRequired[Union[datetime, str]],
    ForceUpdate: NotRequired[bool],
    NoExpiry: NotRequired[bool],
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
## GeofenceGeometryTypeDef

```python
# GeofenceGeometryTypeDef definition

class GeofenceGeometryTypeDef(TypedDict):
    Circle: NotRequired[CircleTypeDef],  # (1)
    Polygon: NotRequired[Sequence[Sequence[Sequence[float]]]],
```

1. See [:material-code-braces: CircleTypeDef](./type_defs.md#circletypedef) 
## CreateMapRequestRequestTypeDef

```python
# CreateMapRequestRequestTypeDef definition

class CreateMapRequestRequestTypeDef(TypedDict):
    Configuration: MapConfigurationTypeDef,  # (1)
    MapName: str,
    Description: NotRequired[str],
    PricingPlan: NotRequired[PricingPlanType],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MapConfigurationTypeDef](./type_defs.md#mapconfigurationtypedef) 
2. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## DescribeMapResponseTypeDef

```python
# DescribeMapResponseTypeDef definition

class DescribeMapResponseTypeDef(TypedDict):
    Configuration: MapConfigurationTypeDef,  # (1)
    CreateTime: datetime,
    DataSource: str,
    Description: str,
    MapArn: str,
    MapName: str,
    PricingPlan: PricingPlanType,  # (2)
    Tags: Dict[str, str],
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MapConfigurationTypeDef](./type_defs.md#mapconfigurationtypedef) 
2. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePlaceIndexRequestRequestTypeDef

```python
# CreatePlaceIndexRequestRequestTypeDef definition

class CreatePlaceIndexRequestRequestTypeDef(TypedDict):
    DataSource: str,
    IndexName: str,
    DataSourceConfiguration: NotRequired[DataSourceConfigurationTypeDef],  # (1)
    Description: NotRequired[str],
    PricingPlan: NotRequired[PricingPlanType],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## DescribePlaceIndexResponseTypeDef

```python
# DescribePlaceIndexResponseTypeDef definition

class DescribePlaceIndexResponseTypeDef(TypedDict):
    CreateTime: datetime,
    DataSource: str,
    DataSourceConfiguration: DataSourceConfigurationTypeDef,  # (1)
    Description: str,
    IndexArn: str,
    IndexName: str,
    PricingPlan: PricingPlanType,  # (2)
    Tags: Dict[str, str],
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePlaceIndexRequestRequestTypeDef

```python
# UpdatePlaceIndexRequestRequestTypeDef definition

class UpdatePlaceIndexRequestRequestTypeDef(TypedDict):
    IndexName: str,
    DataSourceConfiguration: NotRequired[DataSourceConfigurationTypeDef],  # (1)
    Description: NotRequired[str],
    PricingPlan: NotRequired[PricingPlanType],  # (2)
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## DevicePositionTypeDef

```python
# DevicePositionTypeDef definition

class DevicePositionTypeDef(TypedDict):
    Position: List[float],
    ReceivedTime: datetime,
    SampleTime: datetime,
    Accuracy: NotRequired[PositionalAccuracyTypeDef],  # (1)
    DeviceId: NotRequired[str],
    PositionProperties: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: PositionalAccuracyTypeDef](./type_defs.md#positionalaccuracytypedef) 
## DevicePositionUpdateTypeDef

```python
# DevicePositionUpdateTypeDef definition

class DevicePositionUpdateTypeDef(TypedDict):
    DeviceId: str,
    Position: Sequence[float],
    SampleTime: Union[datetime, str],
    Accuracy: NotRequired[PositionalAccuracyTypeDef],  # (1)
    PositionProperties: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: PositionalAccuracyTypeDef](./type_defs.md#positionalaccuracytypedef) 
## GetDevicePositionResponseTypeDef

```python
# GetDevicePositionResponseTypeDef definition

class GetDevicePositionResponseTypeDef(TypedDict):
    Accuracy: PositionalAccuracyTypeDef,  # (1)
    DeviceId: str,
    Position: List[float],
    PositionProperties: Dict[str, str],
    ReceivedTime: datetime,
    SampleTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PositionalAccuracyTypeDef](./type_defs.md#positionalaccuracytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDevicePositionsResponseEntryTypeDef

```python
# ListDevicePositionsResponseEntryTypeDef definition

class ListDevicePositionsResponseEntryTypeDef(TypedDict):
    DeviceId: str,
    Position: List[float],
    SampleTime: datetime,
    Accuracy: NotRequired[PositionalAccuracyTypeDef],  # (1)
    PositionProperties: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: PositionalAccuracyTypeDef](./type_defs.md#positionalaccuracytypedef) 
## GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef

```python
# GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef definition

class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(TypedDict):
    DeviceId: str,
    TrackerName: str,
    EndTimeExclusive: NotRequired[Union[datetime, str]],
    StartTimeInclusive: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDevicePositionsRequestListDevicePositionsPaginateTypeDef

```python
# ListDevicePositionsRequestListDevicePositionsPaginateTypeDef definition

class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(TypedDict):
    TrackerName: str,
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
## LegTypeDef

```python
# LegTypeDef definition

class LegTypeDef(TypedDict):
    Distance: float,
    DurationSeconds: float,
    EndPosition: List[float],
    StartPosition: List[float],
    Steps: List[StepTypeDef],  # (2)
    Geometry: NotRequired[LegGeometryTypeDef],  # (1)
```

1. See [:material-code-braces: LegGeometryTypeDef](./type_defs.md#leggeometrytypedef) 
2. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
## ListGeofenceCollectionsResponseTypeDef

```python
# ListGeofenceCollectionsResponseTypeDef definition

class ListGeofenceCollectionsResponseTypeDef(TypedDict):
    Entries: List[ListGeofenceCollectionsResponseEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListGeofenceCollectionsResponseEntryTypeDef](./type_defs.md#listgeofencecollectionsresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMapsResponseTypeDef

```python
# ListMapsResponseTypeDef definition

class ListMapsResponseTypeDef(TypedDict):
    Entries: List[ListMapsResponseEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListMapsResponseEntryTypeDef](./type_defs.md#listmapsresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPlaceIndexesResponseTypeDef

```python
# ListPlaceIndexesResponseTypeDef definition

class ListPlaceIndexesResponseTypeDef(TypedDict):
    Entries: List[ListPlaceIndexesResponseEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListPlaceIndexesResponseEntryTypeDef](./type_defs.md#listplaceindexesresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRouteCalculatorsResponseTypeDef

```python
# ListRouteCalculatorsResponseTypeDef definition

class ListRouteCalculatorsResponseTypeDef(TypedDict):
    Entries: List[ListRouteCalculatorsResponseEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListRouteCalculatorsResponseEntryTypeDef](./type_defs.md#listroutecalculatorsresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrackersResponseTypeDef

```python
# ListTrackersResponseTypeDef definition

class ListTrackersResponseTypeDef(TypedDict):
    Entries: List[ListTrackersResponseEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListTrackersResponseEntryTypeDef](./type_defs.md#listtrackersresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMapRequestRequestTypeDef

```python
# UpdateMapRequestRequestTypeDef definition

class UpdateMapRequestRequestTypeDef(TypedDict):
    MapName: str,
    ConfigurationUpdate: NotRequired[MapConfigurationUpdateTypeDef],  # (1)
    Description: NotRequired[str],
    PricingPlan: NotRequired[PricingPlanType],  # (2)
```

1. See [:material-code-braces: MapConfigurationUpdateTypeDef](./type_defs.md#mapconfigurationupdatetypedef) 
2. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
## PlaceTypeDef

```python
# PlaceTypeDef definition

class PlaceTypeDef(TypedDict):
    Geometry: PlaceGeometryTypeDef,  # (1)
    AddressNumber: NotRequired[str],
    Categories: NotRequired[List[str]],
    Country: NotRequired[str],
    Interpolated: NotRequired[bool],
    Label: NotRequired[str],
    Municipality: NotRequired[str],
    Neighborhood: NotRequired[str],
    PostalCode: NotRequired[str],
    Region: NotRequired[str],
    Street: NotRequired[str],
    SubRegion: NotRequired[str],
    SupplementalCategories: NotRequired[List[str]],
    TimeZone: NotRequired[TimeZoneTypeDef],  # (2)
    UnitNumber: NotRequired[str],
    UnitType: NotRequired[str],
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
    Results: List[SearchForSuggestionsResultTypeDef],  # (1)
    Summary: SearchPlaceIndexForSuggestionsSummaryTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SearchForSuggestionsResultTypeDef](./type_defs.md#searchforsuggestionsresulttypedef) 
2. See [:material-code-braces: SearchPlaceIndexForSuggestionsSummaryTypeDef](./type_defs.md#searchplaceindexforsuggestionssummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKeysResponseTypeDef

```python
# ListKeysResponseTypeDef definition

class ListKeysResponseTypeDef(TypedDict):
    Entries: List[ListKeysResponseEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    Errors: List[BatchPutGeofenceErrorTypeDef],  # (1)
    Successes: List[BatchPutGeofenceSuccessTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchPutGeofenceErrorTypeDef](./type_defs.md#batchputgeofenceerrortypedef) 
2. See [:material-code-braces: BatchPutGeofenceSuccessTypeDef](./type_defs.md#batchputgeofencesuccesstypedef) 
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
    CarModeOptions: NotRequired[CalculateRouteCarModeOptionsTypeDef],  # (1)
    DepartNow: NotRequired[bool],
    DepartureTime: NotRequired[Union[datetime, str]],
    DistanceUnit: NotRequired[DistanceUnitType],  # (2)
    Key: NotRequired[str],
    TravelMode: NotRequired[TravelModeType],  # (3)
    TruckModeOptions: NotRequired[CalculateRouteTruckModeOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: CalculateRouteCarModeOptionsTypeDef](./type_defs.md#calculateroutecarmodeoptionstypedef) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-brackets: TravelModeType](./literals.md#travelmodetype) 
4. See [:material-code-braces: CalculateRouteTruckModeOptionsTypeDef](./type_defs.md#calculateroutetruckmodeoptionstypedef) 
## CalculateRouteRequestRequestTypeDef

```python
# CalculateRouteRequestRequestTypeDef definition

class CalculateRouteRequestRequestTypeDef(TypedDict):
    CalculatorName: str,
    DeparturePosition: Sequence[float],
    DestinationPosition: Sequence[float],
    CarModeOptions: NotRequired[CalculateRouteCarModeOptionsTypeDef],  # (1)
    DepartNow: NotRequired[bool],
    DepartureTime: NotRequired[Union[datetime, str]],
    DistanceUnit: NotRequired[DistanceUnitType],  # (2)
    IncludeLegGeometry: NotRequired[bool],
    Key: NotRequired[str],
    TravelMode: NotRequired[TravelModeType],  # (3)
    TruckModeOptions: NotRequired[CalculateRouteTruckModeOptionsTypeDef],  # (4)
    WaypointPositions: NotRequired[Sequence[Sequence[float]]],
```

1. See [:material-code-braces: CalculateRouteCarModeOptionsTypeDef](./type_defs.md#calculateroutecarmodeoptionstypedef) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-brackets: TravelModeType](./literals.md#travelmodetype) 
4. See [:material-code-braces: CalculateRouteTruckModeOptionsTypeDef](./type_defs.md#calculateroutetruckmodeoptionstypedef) 
## BatchPutGeofenceRequestEntryTypeDef

```python
# BatchPutGeofenceRequestEntryTypeDef definition

class BatchPutGeofenceRequestEntryTypeDef(TypedDict):
    GeofenceId: str,
    Geometry: GeofenceGeometryTypeDef,  # (1)
    GeofenceProperties: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: GeofenceGeometryTypeDef](./type_defs.md#geofencegeometrytypedef) 
## GetGeofenceResponseTypeDef

```python
# GetGeofenceResponseTypeDef definition

class GetGeofenceResponseTypeDef(TypedDict):
    CreateTime: datetime,
    GeofenceId: str,
    GeofenceProperties: Dict[str, str],
    Geometry: GeofenceGeometryTypeDef,  # (1)
    Status: str,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeofenceGeometryTypeDef](./type_defs.md#geofencegeometrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGeofenceResponseEntryTypeDef

```python
# ListGeofenceResponseEntryTypeDef definition

class ListGeofenceResponseEntryTypeDef(TypedDict):
    CreateTime: datetime,
    GeofenceId: str,
    Geometry: GeofenceGeometryTypeDef,  # (1)
    Status: str,
    UpdateTime: datetime,
    GeofenceProperties: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: GeofenceGeometryTypeDef](./type_defs.md#geofencegeometrytypedef) 
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
## BatchGetDevicePositionResponseTypeDef

```python
# BatchGetDevicePositionResponseTypeDef definition

class BatchGetDevicePositionResponseTypeDef(TypedDict):
    DevicePositions: List[DevicePositionTypeDef],  # (1)
    Errors: List[BatchGetDevicePositionErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DevicePositionTypeDef](./type_defs.md#devicepositiontypedef) 
2. See [:material-code-braces: BatchGetDevicePositionErrorTypeDef](./type_defs.md#batchgetdevicepositionerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDevicePositionHistoryResponseTypeDef

```python
# GetDevicePositionHistoryResponseTypeDef definition

class GetDevicePositionHistoryResponseTypeDef(TypedDict):
    DevicePositions: List[DevicePositionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
## ListDevicePositionsResponseTypeDef

```python
# ListDevicePositionsResponseTypeDef definition

class ListDevicePositionsResponseTypeDef(TypedDict):
    Entries: List[ListDevicePositionsResponseEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    Distance: float,
    Place: PlaceTypeDef,  # (1)
    PlaceId: NotRequired[str],
```

1. See [:material-code-braces: PlaceTypeDef](./type_defs.md#placetypedef) 
## SearchForTextResultTypeDef

```python
# SearchForTextResultTypeDef definition

class SearchForTextResultTypeDef(TypedDict):
    Place: PlaceTypeDef,  # (1)
    Distance: NotRequired[float],
    PlaceId: NotRequired[str],
    Relevance: NotRequired[float],
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
## BatchPutGeofenceRequestRequestTypeDef

```python
# BatchPutGeofenceRequestRequestTypeDef definition

class BatchPutGeofenceRequestRequestTypeDef(TypedDict):
    CollectionName: str,
    Entries: Sequence[BatchPutGeofenceRequestEntryTypeDef],  # (1)
```

1. See [:material-code-braces: BatchPutGeofenceRequestEntryTypeDef](./type_defs.md#batchputgeofencerequestentrytypedef) 
## ListGeofencesResponseTypeDef

```python
# ListGeofencesResponseTypeDef definition

class ListGeofencesResponseTypeDef(TypedDict):
    Entries: List[ListGeofenceResponseEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListGeofenceResponseEntryTypeDef](./type_defs.md#listgeofenceresponseentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchPlaceIndexForPositionResponseTypeDef

```python
# SearchPlaceIndexForPositionResponseTypeDef definition

class SearchPlaceIndexForPositionResponseTypeDef(TypedDict):
    Results: List[SearchForPositionResultTypeDef],  # (1)
    Summary: SearchPlaceIndexForPositionSummaryTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SearchForPositionResultTypeDef](./type_defs.md#searchforpositionresulttypedef) 
2. See [:material-code-braces: SearchPlaceIndexForPositionSummaryTypeDef](./type_defs.md#searchplaceindexforpositionsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchPlaceIndexForTextResponseTypeDef

```python
# SearchPlaceIndexForTextResponseTypeDef definition

class SearchPlaceIndexForTextResponseTypeDef(TypedDict):
    Results: List[SearchForTextResultTypeDef],  # (1)
    Summary: SearchPlaceIndexForTextSummaryTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SearchForTextResultTypeDef](./type_defs.md#searchfortextresulttypedef) 
2. See [:material-code-braces: SearchPlaceIndexForTextSummaryTypeDef](./type_defs.md#searchplaceindexfortextsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
