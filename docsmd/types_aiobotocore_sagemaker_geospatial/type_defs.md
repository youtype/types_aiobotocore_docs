# Type definitions

> [Index](../README.md) > [SageMakergeospatialcapabilities](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SageMakergeospatialcapabilities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
    type annotations stubs module [types-aiobotocore-sagemaker-geospatial](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## MultiPolygonGeometryInputTypeDef

```python
# MultiPolygonGeometryInputTypeDef definition

class MultiPolygonGeometryInputTypeDef(TypedDict):
    Coordinates: List[List[List[List[float]]]],
```

## PolygonGeometryInputTypeDef

```python
# PolygonGeometryInputTypeDef definition

class PolygonGeometryInputTypeDef(TypedDict):
    Coordinates: List[List[List[float]]],
```

## AssetValueTypeDef

```python
# AssetValueTypeDef definition

class AssetValueTypeDef(TypedDict):
    Href: NotRequired[str],
```

## CloudRemovalConfigInputTypeDef

```python
# CloudRemovalConfigInputTypeDef definition

class CloudRemovalConfigInputTypeDef(TypedDict):
    AlgorithmName: NotRequired[AlgorithmNameCloudRemovalType],  # (1)
    InterpolationValue: NotRequired[str],
    TargetBands: NotRequired[List[str]],
```

1. See [:material-code-brackets: AlgorithmNameCloudRemovalType](./literals.md#algorithmnamecloudremovaltype) 
## OperationTypeDef

```python
# OperationTypeDef definition

class OperationTypeDef(TypedDict):
    Equation: str,
    Name: str,
    OutputType: NotRequired[OutputTypeType],  # (1)
```

1. See [:material-code-brackets: OutputTypeType](./literals.md#outputtypetype) 
## DeleteEarthObservationJobInputRequestTypeDef

```python
# DeleteEarthObservationJobInputRequestTypeDef definition

class DeleteEarthObservationJobInputRequestTypeDef(TypedDict):
    Arn: str,
```

## DeleteVectorEnrichmentJobInputRequestTypeDef

```python
# DeleteVectorEnrichmentJobInputRequestTypeDef definition

class DeleteVectorEnrichmentJobInputRequestTypeDef(TypedDict):
    Arn: str,
```

## EarthObservationJobErrorDetailsTypeDef

```python
# EarthObservationJobErrorDetailsTypeDef definition

class EarthObservationJobErrorDetailsTypeDef(TypedDict):
    Message: NotRequired[str],
    Type: NotRequired[EarthObservationJobErrorTypeType],  # (1)
```

1. See [:material-code-brackets: EarthObservationJobErrorTypeType](./literals.md#earthobservationjoberrortypetype) 
## EoCloudCoverInputTypeDef

```python
# EoCloudCoverInputTypeDef definition

class EoCloudCoverInputTypeDef(TypedDict):
    LowerBound: float,
    UpperBound: float,
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

## ExportErrorDetailsOutputTypeDef

```python
# ExportErrorDetailsOutputTypeDef definition

class ExportErrorDetailsOutputTypeDef(TypedDict):
    Message: NotRequired[str],
    Type: NotRequired[ExportErrorTypeType],  # (1)
```

1. See [:material-code-brackets: ExportErrorTypeType](./literals.md#exporterrortypetype) 
## ExportS3DataInputTypeDef

```python
# ExportS3DataInputTypeDef definition

class ExportS3DataInputTypeDef(TypedDict):
    S3Uri: str,
    KmsKeyId: NotRequired[str],
```

## VectorEnrichmentJobS3DataTypeDef

```python
# VectorEnrichmentJobS3DataTypeDef definition

class VectorEnrichmentJobS3DataTypeDef(TypedDict):
    S3Uri: str,
    KmsKeyId: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: str,
    Type: str,
    Maximum: NotRequired[float],
    Minimum: NotRequired[float],
```

## GeoMosaicConfigInputTypeDef

```python
# GeoMosaicConfigInputTypeDef definition

class GeoMosaicConfigInputTypeDef(TypedDict):
    AlgorithmName: NotRequired[AlgorithmNameGeoMosaicType],  # (1)
    TargetBands: NotRequired[List[str]],
```

1. See [:material-code-brackets: AlgorithmNameGeoMosaicType](./literals.md#algorithmnamegeomosaictype) 
## GeometryTypeDef

```python
# GeometryTypeDef definition

class GeometryTypeDef(TypedDict):
    Coordinates: List[List[List[float]]],
    Type: str,
```

## GetEarthObservationJobInputRequestTypeDef

```python
# GetEarthObservationJobInputRequestTypeDef definition

class GetEarthObservationJobInputRequestTypeDef(TypedDict):
    Arn: str,
```

## OutputBandTypeDef

```python
# OutputBandTypeDef definition

class OutputBandTypeDef(TypedDict):
    BandName: str,
    OutputDataType: OutputTypeType,  # (1)
```

1. See [:material-code-brackets: OutputTypeType](./literals.md#outputtypetype) 
## GetRasterDataCollectionInputRequestTypeDef

```python
# GetRasterDataCollectionInputRequestTypeDef definition

class GetRasterDataCollectionInputRequestTypeDef(TypedDict):
    Arn: str,
```

## GetTileInputRequestTypeDef

```python
# GetTileInputRequestTypeDef definition

class GetTileInputRequestTypeDef(TypedDict):
    Arn: str,
    ImageAssets: Sequence[str],
    Target: TargetOptionsType,  # (1)
    x: int,
    y: int,
    z: int,
    ExecutionRoleArn: NotRequired[str],
    ImageMask: NotRequired[bool],
    OutputDataType: NotRequired[OutputTypeType],  # (2)
    OutputFormat: NotRequired[str],
    PropertyFilters: NotRequired[str],
    TimeRangeFilter: NotRequired[str],
```

1. See [:material-code-brackets: TargetOptionsType](./literals.md#targetoptionstype) 
2. See [:material-code-brackets: OutputTypeType](./literals.md#outputtypetype) 
## GetVectorEnrichmentJobInputRequestTypeDef

```python
# GetVectorEnrichmentJobInputRequestTypeDef definition

class GetVectorEnrichmentJobInputRequestTypeDef(TypedDict):
    Arn: str,
```

## VectorEnrichmentJobErrorDetailsTypeDef

```python
# VectorEnrichmentJobErrorDetailsTypeDef definition

class VectorEnrichmentJobErrorDetailsTypeDef(TypedDict):
    ErrorMessage: NotRequired[str],
    ErrorType: NotRequired[VectorEnrichmentJobErrorTypeType],  # (1)
```

1. See [:material-code-brackets: VectorEnrichmentJobErrorTypeType](./literals.md#vectorenrichmentjoberrortypetype) 
## VectorEnrichmentJobExportErrorDetailsTypeDef

```python
# VectorEnrichmentJobExportErrorDetailsTypeDef definition

class VectorEnrichmentJobExportErrorDetailsTypeDef(TypedDict):
    Message: NotRequired[str],
    Type: NotRequired[VectorEnrichmentJobExportErrorTypeType],  # (1)
```

1. See [:material-code-brackets: VectorEnrichmentJobExportErrorTypeType](./literals.md#vectorenrichmentjobexporterrortypetype) 
## PropertiesTypeDef

```python
# PropertiesTypeDef definition

class PropertiesTypeDef(TypedDict):
    EoCloudCover: NotRequired[float],
    LandsatCloudCoverLand: NotRequired[float],
    Platform: NotRequired[str],
    ViewOffNadir: NotRequired[float],
    ViewSunAzimuth: NotRequired[float],
    ViewSunElevation: NotRequired[float],
```

## TemporalStatisticsConfigInputTypeDef

```python
# TemporalStatisticsConfigInputTypeDef definition

class TemporalStatisticsConfigInputTypeDef(TypedDict):
    Statistics: List[TemporalStatisticsType],  # (2)
    GroupBy: NotRequired[GroupByType],  # (1)
    TargetBands: NotRequired[List[str]],
```

1. See [:material-code-brackets: GroupByType](./literals.md#groupbytype) 
2. See [:material-code-brackets: TemporalStatisticsType](./literals.md#temporalstatisticstype) 
## ZonalStatisticsConfigInputTypeDef

```python
# ZonalStatisticsConfigInputTypeDef definition

class ZonalStatisticsConfigInputTypeDef(TypedDict):
    Statistics: List[ZonalStatisticsType],  # (1)
    ZoneS3Path: str,
    TargetBands: NotRequired[List[str]],
    ZoneS3PathKmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: ZonalStatisticsType](./literals.md#zonalstatisticstype) 
## LandsatCloudCoverLandInputTypeDef

```python
# LandsatCloudCoverLandInputTypeDef definition

class LandsatCloudCoverLandInputTypeDef(TypedDict):
    LowerBound: float,
    UpperBound: float,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEarthObservationJobInputRequestTypeDef

```python
# ListEarthObservationJobInputRequestTypeDef definition

class ListEarthObservationJobInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (1)
    StatusEquals: NotRequired[EarthObservationJobStatusType],  # (2)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: EarthObservationJobStatusType](./literals.md#earthobservationjobstatustype) 
## ListEarthObservationJobOutputConfigTypeDef

```python
# ListEarthObservationJobOutputConfigTypeDef definition

class ListEarthObservationJobOutputConfigTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    DurationInSeconds: int,
    Name: str,
    OperationType: str,
    Status: EarthObservationJobStatusType,  # (1)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: EarthObservationJobStatusType](./literals.md#earthobservationjobstatustype) 
## ListRasterDataCollectionsInputRequestTypeDef

```python
# ListRasterDataCollectionsInputRequestTypeDef definition

class ListRasterDataCollectionsInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListVectorEnrichmentJobInputRequestTypeDef

```python
# ListVectorEnrichmentJobInputRequestTypeDef definition

class ListVectorEnrichmentJobInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (1)
    StatusEquals: NotRequired[str],
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListVectorEnrichmentJobOutputConfigTypeDef

```python
# ListVectorEnrichmentJobOutputConfigTypeDef definition

class ListVectorEnrichmentJobOutputConfigTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    DurationInSeconds: int,
    Name: str,
    Status: VectorEnrichmentJobStatusType,  # (1)
    Type: VectorEnrichmentJobTypeType,  # (2)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: VectorEnrichmentJobStatusType](./literals.md#vectorenrichmentjobstatustype) 
2. See [:material-code-brackets: VectorEnrichmentJobTypeType](./literals.md#vectorenrichmentjobtypetype) 
## MapMatchingConfigTypeDef

```python
# MapMatchingConfigTypeDef definition

class MapMatchingConfigTypeDef(TypedDict):
    IdAttributeName: str,
    TimestampAttributeName: str,
    XAttributeName: str,
    YAttributeName: str,
```

## UserDefinedTypeDef

```python
# UserDefinedTypeDef definition

class UserDefinedTypeDef(TypedDict):
    Unit: UnitType,  # (1)
    Value: float,
```

1. See [:material-code-brackets: UnitType](./literals.md#unittype) 
## PlatformInputTypeDef

```python
# PlatformInputTypeDef definition

class PlatformInputTypeDef(TypedDict):
    Value: str,
    ComparisonOperator: NotRequired[ComparisonOperatorType],  # (1)
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## ViewOffNadirInputTypeDef

```python
# ViewOffNadirInputTypeDef definition

class ViewOffNadirInputTypeDef(TypedDict):
    LowerBound: float,
    UpperBound: float,
```

## ViewSunAzimuthInputTypeDef

```python
# ViewSunAzimuthInputTypeDef definition

class ViewSunAzimuthInputTypeDef(TypedDict):
    LowerBound: float,
    UpperBound: float,
```

## ViewSunElevationInputTypeDef

```python
# ViewSunElevationInputTypeDef definition

class ViewSunElevationInputTypeDef(TypedDict):
    LowerBound: float,
    UpperBound: float,
```

## TimeRangeFilterOutputTypeDef

```python
# TimeRangeFilterOutputTypeDef definition

class TimeRangeFilterOutputTypeDef(TypedDict):
    EndTime: datetime,
    StartTime: datetime,
```

## ReverseGeocodingConfigTypeDef

```python
# ReverseGeocodingConfigTypeDef definition

class ReverseGeocodingConfigTypeDef(TypedDict):
    XAttributeName: str,
    YAttributeName: str,
```

## StopEarthObservationJobInputRequestTypeDef

```python
# StopEarthObservationJobInputRequestTypeDef definition

class StopEarthObservationJobInputRequestTypeDef(TypedDict):
    Arn: str,
```

## StopVectorEnrichmentJobInputRequestTypeDef

```python
# StopVectorEnrichmentJobInputRequestTypeDef definition

class StopVectorEnrichmentJobInputRequestTypeDef(TypedDict):
    Arn: str,
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

## AreaOfInterestGeometryTypeDef

```python
# AreaOfInterestGeometryTypeDef definition

class AreaOfInterestGeometryTypeDef(TypedDict):
    MultiPolygonGeometry: NotRequired[MultiPolygonGeometryInputTypeDef],  # (1)
    PolygonGeometry: NotRequired[PolygonGeometryInputTypeDef],  # (2)
```

1. See [:material-code-braces: MultiPolygonGeometryInputTypeDef](./type_defs.md#multipolygongeometryinputtypedef) 
2. See [:material-code-braces: PolygonGeometryInputTypeDef](./type_defs.md#polygongeometryinputtypedef) 
## CustomIndicesInputTypeDef

```python
# CustomIndicesInputTypeDef definition

class CustomIndicesInputTypeDef(TypedDict):
    Operations: NotRequired[List[OperationTypeDef]],  # (1)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
## GetTileOutputTypeDef

```python
# GetTileOutputTypeDef definition

class GetTileOutputTypeDef(TypedDict):
    BinaryFile: StreamingBody,
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
## ExportErrorDetailsTypeDef

```python
# ExportErrorDetailsTypeDef definition

class ExportErrorDetailsTypeDef(TypedDict):
    ExportResults: NotRequired[ExportErrorDetailsOutputTypeDef],  # (1)
    ExportSourceImages: NotRequired[ExportErrorDetailsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ExportErrorDetailsOutputTypeDef](./type_defs.md#exporterrordetailsoutputtypedef) 
2. See [:material-code-braces: ExportErrorDetailsOutputTypeDef](./type_defs.md#exporterrordetailsoutputtypedef) 
## OutputConfigInputTypeDef

```python
# OutputConfigInputTypeDef definition

class OutputConfigInputTypeDef(TypedDict):
    S3Data: ExportS3DataInputTypeDef,  # (1)
```

1. See [:material-code-braces: ExportS3DataInputTypeDef](./type_defs.md#exports3datainputtypedef) 
## ExportVectorEnrichmentJobOutputConfigTypeDef

```python
# ExportVectorEnrichmentJobOutputConfigTypeDef definition

class ExportVectorEnrichmentJobOutputConfigTypeDef(TypedDict):
    S3Data: VectorEnrichmentJobS3DataTypeDef,  # (1)
```

1. See [:material-code-braces: VectorEnrichmentJobS3DataTypeDef](./type_defs.md#vectorenrichmentjobs3datatypedef) 
## VectorEnrichmentJobDataSourceConfigInputTypeDef

```python
# VectorEnrichmentJobDataSourceConfigInputTypeDef definition

class VectorEnrichmentJobDataSourceConfigInputTypeDef(TypedDict):
    S3Data: NotRequired[VectorEnrichmentJobS3DataTypeDef],  # (1)
```

1. See [:material-code-braces: VectorEnrichmentJobS3DataTypeDef](./type_defs.md#vectorenrichmentjobs3datatypedef) 
## GetRasterDataCollectionOutputTypeDef

```python
# GetRasterDataCollectionOutputTypeDef definition

class GetRasterDataCollectionOutputTypeDef(TypedDict):
    Arn: str,
    Description: str,
    DescriptionPageUrl: str,
    ImageSourceBands: List[str],
    Name: str,
    SupportedFilters: List[FilterTypeDef],  # (1)
    Tags: Dict[str, str],
    Type: DataCollectionTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: DataCollectionTypeType](./literals.md#datacollectiontypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RasterDataCollectionMetadataTypeDef

```python
# RasterDataCollectionMetadataTypeDef definition

class RasterDataCollectionMetadataTypeDef(TypedDict):
    Arn: str,
    Description: str,
    Name: str,
    SupportedFilters: List[FilterTypeDef],  # (1)
    Type: DataCollectionTypeType,  # (2)
    DescriptionPageUrl: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: DataCollectionTypeType](./literals.md#datacollectiontypetype) 
## ItemSourceTypeDef

```python
# ItemSourceTypeDef definition

class ItemSourceTypeDef(TypedDict):
    DateTime: datetime,
    Geometry: GeometryTypeDef,  # (2)
    Id: str,
    Assets: NotRequired[Dict[str, AssetValueTypeDef]],  # (1)
    Properties: NotRequired[PropertiesTypeDef],  # (3)
```

1. See [:material-code-braces: AssetValueTypeDef](./type_defs.md#assetvaluetypedef) 
2. See [:material-code-braces: GeometryTypeDef](./type_defs.md#geometrytypedef) 
3. See [:material-code-braces: PropertiesTypeDef](./type_defs.md#propertiestypedef) 
## ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef

```python
# ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef definition

class ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef(TypedDict):
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (1)
    StatusEquals: NotRequired[EarthObservationJobStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: EarthObservationJobStatusType](./literals.md#earthobservationjobstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef

```python
# ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef definition

class ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef

```python
# ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef definition

class ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef(TypedDict):
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (1)
    StatusEquals: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEarthObservationJobOutputTypeDef

```python
# ListEarthObservationJobOutputTypeDef definition

class ListEarthObservationJobOutputTypeDef(TypedDict):
    EarthObservationJobSummaries: List[ListEarthObservationJobOutputConfigTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListEarthObservationJobOutputConfigTypeDef](./type_defs.md#listearthobservationjoboutputconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVectorEnrichmentJobOutputTypeDef

```python
# ListVectorEnrichmentJobOutputTypeDef definition

class ListVectorEnrichmentJobOutputTypeDef(TypedDict):
    NextToken: str,
    VectorEnrichmentJobSummaries: List[ListVectorEnrichmentJobOutputConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListVectorEnrichmentJobOutputConfigTypeDef](./type_defs.md#listvectorenrichmentjoboutputconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OutputResolutionResamplingInputTypeDef

```python
# OutputResolutionResamplingInputTypeDef definition

class OutputResolutionResamplingInputTypeDef(TypedDict):
    UserDefined: UserDefinedTypeDef,  # (1)
```

1. See [:material-code-braces: UserDefinedTypeDef](./type_defs.md#userdefinedtypedef) 
## OutputResolutionStackInputTypeDef

```python
# OutputResolutionStackInputTypeDef definition

class OutputResolutionStackInputTypeDef(TypedDict):
    Predefined: NotRequired[PredefinedResolutionType],  # (1)
    UserDefined: NotRequired[UserDefinedTypeDef],  # (2)
```

1. See [:material-code-brackets: PredefinedResolutionType](./literals.md#predefinedresolutiontype) 
2. See [:material-code-braces: UserDefinedTypeDef](./type_defs.md#userdefinedtypedef) 
## PropertyTypeDef

```python
# PropertyTypeDef definition

class PropertyTypeDef(TypedDict):
    EoCloudCover: NotRequired[EoCloudCoverInputTypeDef],  # (1)
    LandsatCloudCoverLand: NotRequired[LandsatCloudCoverLandInputTypeDef],  # (2)
    Platform: NotRequired[PlatformInputTypeDef],  # (3)
    ViewOffNadir: NotRequired[ViewOffNadirInputTypeDef],  # (4)
    ViewSunAzimuth: NotRequired[ViewSunAzimuthInputTypeDef],  # (5)
    ViewSunElevation: NotRequired[ViewSunElevationInputTypeDef],  # (6)
```

1. See [:material-code-braces: EoCloudCoverInputTypeDef](./type_defs.md#eocloudcoverinputtypedef) 
2. See [:material-code-braces: LandsatCloudCoverLandInputTypeDef](./type_defs.md#landsatcloudcoverlandinputtypedef) 
3. See [:material-code-braces: PlatformInputTypeDef](./type_defs.md#platforminputtypedef) 
4. See [:material-code-braces: ViewOffNadirInputTypeDef](./type_defs.md#viewoffnadirinputtypedef) 
5. See [:material-code-braces: ViewSunAzimuthInputTypeDef](./type_defs.md#viewsunazimuthinputtypedef) 
6. See [:material-code-braces: ViewSunElevationInputTypeDef](./type_defs.md#viewsunelevationinputtypedef) 
## VectorEnrichmentJobConfigTypeDef

```python
# VectorEnrichmentJobConfigTypeDef definition

class VectorEnrichmentJobConfigTypeDef(TypedDict):
    MapMatchingConfig: NotRequired[MapMatchingConfigTypeDef],  # (1)
    ReverseGeocodingConfig: NotRequired[ReverseGeocodingConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MapMatchingConfigTypeDef](./type_defs.md#mapmatchingconfigtypedef) 
2. See [:material-code-braces: ReverseGeocodingConfigTypeDef](./type_defs.md#reversegeocodingconfigtypedef) 
## TimeRangeFilterInputTypeDef

```python
# TimeRangeFilterInputTypeDef definition

class TimeRangeFilterInputTypeDef(TypedDict):
    EndTime: Union[datetime, str],
    StartTime: Union[datetime, str],
```

## AreaOfInterestTypeDef

```python
# AreaOfInterestTypeDef definition

class AreaOfInterestTypeDef(TypedDict):
    AreaOfInterestGeometry: NotRequired[AreaOfInterestGeometryTypeDef],  # (1)
```

1. See [:material-code-braces: AreaOfInterestGeometryTypeDef](./type_defs.md#areaofinterestgeometrytypedef) 
## BandMathConfigInputTypeDef

```python
# BandMathConfigInputTypeDef definition

class BandMathConfigInputTypeDef(TypedDict):
    CustomIndices: NotRequired[CustomIndicesInputTypeDef],  # (1)
    PredefinedIndices: NotRequired[List[str]],
```

1. See [:material-code-braces: CustomIndicesInputTypeDef](./type_defs.md#customindicesinputtypedef) 
## ExportEarthObservationJobInputRequestTypeDef

```python
# ExportEarthObservationJobInputRequestTypeDef definition

class ExportEarthObservationJobInputRequestTypeDef(TypedDict):
    Arn: str,
    ExecutionRoleArn: str,
    OutputConfig: OutputConfigInputTypeDef,  # (1)
    ClientToken: NotRequired[str],
    ExportSourceImages: NotRequired[bool],
```

1. See [:material-code-braces: OutputConfigInputTypeDef](./type_defs.md#outputconfiginputtypedef) 
## ExportEarthObservationJobOutputTypeDef

```python
# ExportEarthObservationJobOutputTypeDef definition

class ExportEarthObservationJobOutputTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    ExecutionRoleArn: str,
    ExportSourceImages: bool,
    ExportStatus: EarthObservationJobExportStatusType,  # (1)
    OutputConfig: OutputConfigInputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EarthObservationJobExportStatusType](./literals.md#earthobservationjobexportstatustype) 
2. See [:material-code-braces: OutputConfigInputTypeDef](./type_defs.md#outputconfiginputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportVectorEnrichmentJobInputRequestTypeDef

```python
# ExportVectorEnrichmentJobInputRequestTypeDef definition

class ExportVectorEnrichmentJobInputRequestTypeDef(TypedDict):
    Arn: str,
    ExecutionRoleArn: str,
    OutputConfig: ExportVectorEnrichmentJobOutputConfigTypeDef,  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: ExportVectorEnrichmentJobOutputConfigTypeDef](./type_defs.md#exportvectorenrichmentjoboutputconfigtypedef) 
## ExportVectorEnrichmentJobOutputTypeDef

```python
# ExportVectorEnrichmentJobOutputTypeDef definition

class ExportVectorEnrichmentJobOutputTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    ExecutionRoleArn: str,
    ExportStatus: VectorEnrichmentJobExportStatusType,  # (1)
    OutputConfig: ExportVectorEnrichmentJobOutputConfigTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VectorEnrichmentJobExportStatusType](./literals.md#vectorenrichmentjobexportstatustype) 
2. See [:material-code-braces: ExportVectorEnrichmentJobOutputConfigTypeDef](./type_defs.md#exportvectorenrichmentjoboutputconfigtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VectorEnrichmentJobInputConfigTypeDef

```python
# VectorEnrichmentJobInputConfigTypeDef definition

class VectorEnrichmentJobInputConfigTypeDef(TypedDict):
    DataSourceConfig: VectorEnrichmentJobDataSourceConfigInputTypeDef,  # (1)
    DocumentType: VectorEnrichmentJobDocumentTypeType,  # (2)
```

1. See [:material-code-braces: VectorEnrichmentJobDataSourceConfigInputTypeDef](./type_defs.md#vectorenrichmentjobdatasourceconfiginputtypedef) 
2. See [:material-code-brackets: VectorEnrichmentJobDocumentTypeType](./literals.md#vectorenrichmentjobdocumenttypetype) 
## ListRasterDataCollectionsOutputTypeDef

```python
# ListRasterDataCollectionsOutputTypeDef definition

class ListRasterDataCollectionsOutputTypeDef(TypedDict):
    NextToken: str,
    RasterDataCollectionSummaries: List[RasterDataCollectionMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RasterDataCollectionMetadataTypeDef](./type_defs.md#rasterdatacollectionmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchRasterDataCollectionOutputTypeDef

```python
# SearchRasterDataCollectionOutputTypeDef definition

class SearchRasterDataCollectionOutputTypeDef(TypedDict):
    ApproximateResultCount: int,
    Items: List[ItemSourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ItemSourceTypeDef](./type_defs.md#itemsourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResamplingConfigInputTypeDef

```python
# ResamplingConfigInputTypeDef definition

class ResamplingConfigInputTypeDef(TypedDict):
    OutputResolution: OutputResolutionResamplingInputTypeDef,  # (2)
    AlgorithmName: NotRequired[AlgorithmNameResamplingType],  # (1)
    TargetBands: NotRequired[List[str]],
```

1. See [:material-code-brackets: AlgorithmNameResamplingType](./literals.md#algorithmnameresamplingtype) 
2. See [:material-code-braces: OutputResolutionResamplingInputTypeDef](./type_defs.md#outputresolutionresamplinginputtypedef) 
## StackConfigInputTypeDef

```python
# StackConfigInputTypeDef definition

class StackConfigInputTypeDef(TypedDict):
    OutputResolution: NotRequired[OutputResolutionStackInputTypeDef],  # (1)
    TargetBands: NotRequired[List[str]],
```

1. See [:material-code-braces: OutputResolutionStackInputTypeDef](./type_defs.md#outputresolutionstackinputtypedef) 
## PropertyFilterTypeDef

```python
# PropertyFilterTypeDef definition

class PropertyFilterTypeDef(TypedDict):
    Property: PropertyTypeDef,  # (1)
```

1. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
## GetVectorEnrichmentJobOutputTypeDef

```python
# GetVectorEnrichmentJobOutputTypeDef definition

class GetVectorEnrichmentJobOutputTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    DurationInSeconds: int,
    ErrorDetails: VectorEnrichmentJobErrorDetailsTypeDef,  # (1)
    ExecutionRoleArn: str,
    ExportErrorDetails: VectorEnrichmentJobExportErrorDetailsTypeDef,  # (2)
    ExportStatus: VectorEnrichmentJobExportStatusType,  # (3)
    InputConfig: VectorEnrichmentJobInputConfigTypeDef,  # (4)
    JobConfig: VectorEnrichmentJobConfigTypeDef,  # (5)
    KmsKeyId: str,
    Name: str,
    Status: VectorEnrichmentJobStatusType,  # (6)
    Tags: Dict[str, str],
    Type: VectorEnrichmentJobTypeType,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: VectorEnrichmentJobErrorDetailsTypeDef](./type_defs.md#vectorenrichmentjoberrordetailstypedef) 
2. See [:material-code-braces: VectorEnrichmentJobExportErrorDetailsTypeDef](./type_defs.md#vectorenrichmentjobexporterrordetailstypedef) 
3. See [:material-code-brackets: VectorEnrichmentJobExportStatusType](./literals.md#vectorenrichmentjobexportstatustype) 
4. See [:material-code-braces: VectorEnrichmentJobInputConfigTypeDef](./type_defs.md#vectorenrichmentjobinputconfigtypedef) 
5. See [:material-code-braces: VectorEnrichmentJobConfigTypeDef](./type_defs.md#vectorenrichmentjobconfigtypedef) 
6. See [:material-code-brackets: VectorEnrichmentJobStatusType](./literals.md#vectorenrichmentjobstatustype) 
7. See [:material-code-brackets: VectorEnrichmentJobTypeType](./literals.md#vectorenrichmentjobtypetype) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartVectorEnrichmentJobInputRequestTypeDef

```python
# StartVectorEnrichmentJobInputRequestTypeDef definition

class StartVectorEnrichmentJobInputRequestTypeDef(TypedDict):
    ExecutionRoleArn: str,
    InputConfig: VectorEnrichmentJobInputConfigTypeDef,  # (1)
    JobConfig: VectorEnrichmentJobConfigTypeDef,  # (2)
    Name: str,
    ClientToken: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: VectorEnrichmentJobInputConfigTypeDef](./type_defs.md#vectorenrichmentjobinputconfigtypedef) 
2. See [:material-code-braces: VectorEnrichmentJobConfigTypeDef](./type_defs.md#vectorenrichmentjobconfigtypedef) 
## StartVectorEnrichmentJobOutputTypeDef

```python
# StartVectorEnrichmentJobOutputTypeDef definition

class StartVectorEnrichmentJobOutputTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    DurationInSeconds: int,
    ExecutionRoleArn: str,
    InputConfig: VectorEnrichmentJobInputConfigTypeDef,  # (1)
    JobConfig: VectorEnrichmentJobConfigTypeDef,  # (2)
    KmsKeyId: str,
    Name: str,
    Status: VectorEnrichmentJobStatusType,  # (3)
    Tags: Dict[str, str],
    Type: VectorEnrichmentJobTypeType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: VectorEnrichmentJobInputConfigTypeDef](./type_defs.md#vectorenrichmentjobinputconfigtypedef) 
2. See [:material-code-braces: VectorEnrichmentJobConfigTypeDef](./type_defs.md#vectorenrichmentjobconfigtypedef) 
3. See [:material-code-brackets: VectorEnrichmentJobStatusType](./literals.md#vectorenrichmentjobstatustype) 
4. See [:material-code-brackets: VectorEnrichmentJobTypeType](./literals.md#vectorenrichmentjobtypetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobConfigInputTypeDef

```python
# JobConfigInputTypeDef definition

class JobConfigInputTypeDef(TypedDict):
    BandMathConfig: NotRequired[BandMathConfigInputTypeDef],  # (1)
    CloudMaskingConfig: NotRequired[Dict[str, Any]],
    CloudRemovalConfig: NotRequired[CloudRemovalConfigInputTypeDef],  # (2)
    GeoMosaicConfig: NotRequired[GeoMosaicConfigInputTypeDef],  # (3)
    LandCoverSegmentationConfig: NotRequired[Dict[str, Any]],
    ResamplingConfig: NotRequired[ResamplingConfigInputTypeDef],  # (4)
    StackConfig: NotRequired[StackConfigInputTypeDef],  # (5)
    TemporalStatisticsConfig: NotRequired[TemporalStatisticsConfigInputTypeDef],  # (6)
    ZonalStatisticsConfig: NotRequired[ZonalStatisticsConfigInputTypeDef],  # (7)
```

1. See [:material-code-braces: BandMathConfigInputTypeDef](./type_defs.md#bandmathconfiginputtypedef) 
2. See [:material-code-braces: CloudRemovalConfigInputTypeDef](./type_defs.md#cloudremovalconfiginputtypedef) 
3. See [:material-code-braces: GeoMosaicConfigInputTypeDef](./type_defs.md#geomosaicconfiginputtypedef) 
4. See [:material-code-braces: ResamplingConfigInputTypeDef](./type_defs.md#resamplingconfiginputtypedef) 
5. See [:material-code-braces: StackConfigInputTypeDef](./type_defs.md#stackconfiginputtypedef) 
6. See [:material-code-braces: TemporalStatisticsConfigInputTypeDef](./type_defs.md#temporalstatisticsconfiginputtypedef) 
7. See [:material-code-braces: ZonalStatisticsConfigInputTypeDef](./type_defs.md#zonalstatisticsconfiginputtypedef) 
## PropertyFiltersTypeDef

```python
# PropertyFiltersTypeDef definition

class PropertyFiltersTypeDef(TypedDict):
    LogicalOperator: NotRequired[LogicalOperatorType],  # (1)
    Properties: NotRequired[List[PropertyFilterTypeDef]],  # (2)
```

1. See [:material-code-brackets: LogicalOperatorType](./literals.md#logicaloperatortype) 
2. See [:material-code-braces: PropertyFilterTypeDef](./type_defs.md#propertyfiltertypedef) 
## RasterDataCollectionQueryInputTypeDef

```python
# RasterDataCollectionQueryInputTypeDef definition

class RasterDataCollectionQueryInputTypeDef(TypedDict):
    RasterDataCollectionArn: str,
    TimeRangeFilter: TimeRangeFilterInputTypeDef,  # (3)
    AreaOfInterest: NotRequired[AreaOfInterestTypeDef],  # (1)
    PropertyFilters: NotRequired[PropertyFiltersTypeDef],  # (2)
```

1. See [:material-code-braces: AreaOfInterestTypeDef](./type_defs.md#areaofinteresttypedef) 
2. See [:material-code-braces: PropertyFiltersTypeDef](./type_defs.md#propertyfilterstypedef) 
3. See [:material-code-braces: TimeRangeFilterInputTypeDef](./type_defs.md#timerangefilterinputtypedef) 
## RasterDataCollectionQueryOutputTypeDef

```python
# RasterDataCollectionQueryOutputTypeDef definition

class RasterDataCollectionQueryOutputTypeDef(TypedDict):
    RasterDataCollectionArn: str,
    RasterDataCollectionName: str,
    TimeRangeFilter: TimeRangeFilterOutputTypeDef,  # (3)
    AreaOfInterest: NotRequired[AreaOfInterestTypeDef],  # (1)
    PropertyFilters: NotRequired[PropertyFiltersTypeDef],  # (2)
```

1. See [:material-code-braces: AreaOfInterestTypeDef](./type_defs.md#areaofinteresttypedef) 
2. See [:material-code-braces: PropertyFiltersTypeDef](./type_defs.md#propertyfilterstypedef) 
3. See [:material-code-braces: TimeRangeFilterOutputTypeDef](./type_defs.md#timerangefilteroutputtypedef) 
## RasterDataCollectionQueryWithBandFilterInputTypeDef

```python
# RasterDataCollectionQueryWithBandFilterInputTypeDef definition

class RasterDataCollectionQueryWithBandFilterInputTypeDef(TypedDict):
    TimeRangeFilter: TimeRangeFilterInputTypeDef,  # (3)
    AreaOfInterest: NotRequired[AreaOfInterestTypeDef],  # (1)
    BandFilter: NotRequired[Sequence[str]],
    PropertyFilters: NotRequired[PropertyFiltersTypeDef],  # (2)
```

1. See [:material-code-braces: AreaOfInterestTypeDef](./type_defs.md#areaofinteresttypedef) 
2. See [:material-code-braces: PropertyFiltersTypeDef](./type_defs.md#propertyfilterstypedef) 
3. See [:material-code-braces: TimeRangeFilterInputTypeDef](./type_defs.md#timerangefilterinputtypedef) 
## InputConfigInputTypeDef

```python
# InputConfigInputTypeDef definition

class InputConfigInputTypeDef(TypedDict):
    PreviousEarthObservationJobArn: NotRequired[str],
    RasterDataCollectionQuery: NotRequired[RasterDataCollectionQueryInputTypeDef],  # (1)
```

1. See [:material-code-braces: RasterDataCollectionQueryInputTypeDef](./type_defs.md#rasterdatacollectionqueryinputtypedef) 
## InputConfigOutputTypeDef

```python
# InputConfigOutputTypeDef definition

class InputConfigOutputTypeDef(TypedDict):
    PreviousEarthObservationJobArn: NotRequired[str],
    RasterDataCollectionQuery: NotRequired[RasterDataCollectionQueryOutputTypeDef],  # (1)
```

1. See [:material-code-braces: RasterDataCollectionQueryOutputTypeDef](./type_defs.md#rasterdatacollectionqueryoutputtypedef) 
## SearchRasterDataCollectionInputRequestTypeDef

```python
# SearchRasterDataCollectionInputRequestTypeDef definition

class SearchRasterDataCollectionInputRequestTypeDef(TypedDict):
    Arn: str,
    RasterDataCollectionQuery: RasterDataCollectionQueryWithBandFilterInputTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RasterDataCollectionQueryWithBandFilterInputTypeDef](./type_defs.md#rasterdatacollectionquerywithbandfilterinputtypedef) 
## StartEarthObservationJobInputRequestTypeDef

```python
# StartEarthObservationJobInputRequestTypeDef definition

class StartEarthObservationJobInputRequestTypeDef(TypedDict):
    ExecutionRoleArn: str,
    InputConfig: InputConfigInputTypeDef,  # (1)
    JobConfig: JobConfigInputTypeDef,  # (2)
    Name: str,
    ClientToken: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: InputConfigInputTypeDef](./type_defs.md#inputconfiginputtypedef) 
2. See [:material-code-braces: JobConfigInputTypeDef](./type_defs.md#jobconfiginputtypedef) 
## GetEarthObservationJobOutputTypeDef

```python
# GetEarthObservationJobOutputTypeDef definition

class GetEarthObservationJobOutputTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    DurationInSeconds: int,
    ErrorDetails: EarthObservationJobErrorDetailsTypeDef,  # (1)
    ExecutionRoleArn: str,
    ExportErrorDetails: ExportErrorDetailsTypeDef,  # (2)
    ExportStatus: EarthObservationJobExportStatusType,  # (3)
    InputConfig: InputConfigOutputTypeDef,  # (4)
    JobConfig: JobConfigInputTypeDef,  # (5)
    KmsKeyId: str,
    Name: str,
    OutputBands: List[OutputBandTypeDef],  # (6)
    Status: EarthObservationJobStatusType,  # (7)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: EarthObservationJobErrorDetailsTypeDef](./type_defs.md#earthobservationjoberrordetailstypedef) 
2. See [:material-code-braces: ExportErrorDetailsTypeDef](./type_defs.md#exporterrordetailstypedef) 
3. See [:material-code-brackets: EarthObservationJobExportStatusType](./literals.md#earthobservationjobexportstatustype) 
4. See [:material-code-braces: InputConfigOutputTypeDef](./type_defs.md#inputconfigoutputtypedef) 
5. See [:material-code-braces: JobConfigInputTypeDef](./type_defs.md#jobconfiginputtypedef) 
6. See [:material-code-braces: OutputBandTypeDef](./type_defs.md#outputbandtypedef) 
7. See [:material-code-brackets: EarthObservationJobStatusType](./literals.md#earthobservationjobstatustype) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartEarthObservationJobOutputTypeDef

```python
# StartEarthObservationJobOutputTypeDef definition

class StartEarthObservationJobOutputTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    DurationInSeconds: int,
    ExecutionRoleArn: str,
    InputConfig: InputConfigOutputTypeDef,  # (1)
    JobConfig: JobConfigInputTypeDef,  # (2)
    KmsKeyId: str,
    Name: str,
    Status: EarthObservationJobStatusType,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: InputConfigOutputTypeDef](./type_defs.md#inputconfigoutputtypedef) 
2. See [:material-code-braces: JobConfigInputTypeDef](./type_defs.md#jobconfiginputtypedef) 
3. See [:material-code-brackets: EarthObservationJobStatusType](./literals.md#earthobservationjobstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
