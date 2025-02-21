# Type definitions

> [Index](../README.md) > [LocationServiceRoutesV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LocationServiceRoutesV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-routes.html#locationserviceroutesv2)
    type annotations stubs module [types-aiobotocore-geo-routes](https://pypi.org/project/types-aiobotocore-geo-routes/).

## RouteMatrixBoundaryUnionTypeDef

```python
# RouteMatrixBoundaryUnionTypeDef Union usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixBoundaryUnionTypeDef


def get_value() -> RouteMatrixBoundaryUnionTypeDef:
    return ...


# RouteMatrixBoundaryUnionTypeDef definition

RouteMatrixBoundaryUnionTypeDef = Union[
    RouteMatrixBoundaryTypeDef,  # (1)
    RouteMatrixBoundaryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RouteMatrixBoundaryTypeDef](./type_defs.md#routematrixboundarytypedef) 
2. See [:material-code-braces: RouteMatrixBoundaryOutputTypeDef](./type_defs.md#routematrixboundaryoutputtypedef) 



## IsolineAllowOptionsTypeDef

```python
# IsolineAllowOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineAllowOptionsTypeDef


def get_value() -> IsolineAllowOptionsTypeDef:
    return {
        "Hot": ...,
    }


# IsolineAllowOptionsTypeDef definition

class IsolineAllowOptionsTypeDef(TypedDict):
    Hot: NotRequired[bool],
    Hov: NotRequired[bool],
```

## IsolineGranularityOptionsTypeDef

```python
# IsolineGranularityOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineGranularityOptionsTypeDef


def get_value() -> IsolineGranularityOptionsTypeDef:
    return {
        "MaxPoints": ...,
    }


# IsolineGranularityOptionsTypeDef definition

class IsolineGranularityOptionsTypeDef(TypedDict):
    MaxPoints: NotRequired[int],
    MaxResolution: NotRequired[int],
```

## IsolineThresholdsTypeDef

```python
# IsolineThresholdsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineThresholdsTypeDef


def get_value() -> IsolineThresholdsTypeDef:
    return {
        "Distance": ...,
    }


# IsolineThresholdsTypeDef definition

class IsolineThresholdsTypeDef(TypedDict):
    Distance: NotRequired[Sequence[int]],
    Time: NotRequired[Sequence[int]],
```

## IsolineTrafficOptionsTypeDef

```python
# IsolineTrafficOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineTrafficOptionsTypeDef


def get_value() -> IsolineTrafficOptionsTypeDef:
    return {
        "FlowEventThresholdOverride": ...,
    }


# IsolineTrafficOptionsTypeDef definition

class IsolineTrafficOptionsTypeDef(TypedDict):
    FlowEventThresholdOverride: NotRequired[int],
    Usage: NotRequired[TrafficUsageType],  # (1)
```

1. See [:material-code-brackets: TrafficUsageType](./literals.md#trafficusagetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import ResponseMetadataTypeDef


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

## RouteMatrixAllowOptionsTypeDef

```python
# RouteMatrixAllowOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixAllowOptionsTypeDef


def get_value() -> RouteMatrixAllowOptionsTypeDef:
    return {
        "Hot": ...,
    }


# RouteMatrixAllowOptionsTypeDef definition

class RouteMatrixAllowOptionsTypeDef(TypedDict):
    Hot: NotRequired[bool],
    Hov: NotRequired[bool],
```

## RouteMatrixExclusionOptionsTypeDef

```python
# RouteMatrixExclusionOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixExclusionOptionsTypeDef


def get_value() -> RouteMatrixExclusionOptionsTypeDef:
    return {
        "Countries": ...,
    }


# RouteMatrixExclusionOptionsTypeDef definition

class RouteMatrixExclusionOptionsTypeDef(TypedDict):
    Countries: Sequence[str],
```

## RouteMatrixTrafficOptionsTypeDef

```python
# RouteMatrixTrafficOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixTrafficOptionsTypeDef


def get_value() -> RouteMatrixTrafficOptionsTypeDef:
    return {
        "FlowEventThresholdOverride": ...,
    }


# RouteMatrixTrafficOptionsTypeDef definition

class RouteMatrixTrafficOptionsTypeDef(TypedDict):
    FlowEventThresholdOverride: NotRequired[int],
    Usage: NotRequired[TrafficUsageType],  # (1)
```

1. See [:material-code-brackets: TrafficUsageType](./literals.md#trafficusagetype) 
## RouteMatrixEntryTypeDef

```python
# RouteMatrixEntryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixEntryTypeDef


def get_value() -> RouteMatrixEntryTypeDef:
    return {
        "Distance": ...,
    }


# RouteMatrixEntryTypeDef definition

class RouteMatrixEntryTypeDef(TypedDict):
    Distance: int,
    Duration: int,
    Error: NotRequired[RouteMatrixErrorCodeType],  # (1)
```

1. See [:material-code-brackets: RouteMatrixErrorCodeType](./literals.md#routematrixerrorcodetype) 
## RouteAllowOptionsTypeDef

```python
# RouteAllowOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteAllowOptionsTypeDef


def get_value() -> RouteAllowOptionsTypeDef:
    return {
        "Hot": ...,
    }


# RouteAllowOptionsTypeDef definition

class RouteAllowOptionsTypeDef(TypedDict):
    Hot: NotRequired[bool],
    Hov: NotRequired[bool],
```

## RouteExclusionOptionsTypeDef

```python
# RouteExclusionOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteExclusionOptionsTypeDef


def get_value() -> RouteExclusionOptionsTypeDef:
    return {
        "Countries": ...,
    }


# RouteExclusionOptionsTypeDef definition

class RouteExclusionOptionsTypeDef(TypedDict):
    Countries: Sequence[str],
```

## RouteTrafficOptionsTypeDef

```python
# RouteTrafficOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTrafficOptionsTypeDef


def get_value() -> RouteTrafficOptionsTypeDef:
    return {
        "FlowEventThresholdOverride": ...,
    }


# RouteTrafficOptionsTypeDef definition

class RouteTrafficOptionsTypeDef(TypedDict):
    FlowEventThresholdOverride: NotRequired[int],
    Usage: NotRequired[TrafficUsageType],  # (1)
```

1. See [:material-code-brackets: TrafficUsageType](./literals.md#trafficusagetype) 
## RouteResponseNoticeTypeDef

```python
# RouteResponseNoticeTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteResponseNoticeTypeDef


def get_value() -> RouteResponseNoticeTypeDef:
    return {
        "Code": ...,
    }


# RouteResponseNoticeTypeDef definition

class RouteResponseNoticeTypeDef(TypedDict):
    Code: RouteResponseNoticeCodeType,  # (1)
    Impact: NotRequired[RouteNoticeImpactType],  # (2)
```

1. See [:material-code-brackets: RouteResponseNoticeCodeType](./literals.md#routeresponsenoticecodetype) 
2. See [:material-code-brackets: RouteNoticeImpactType](./literals.md#routenoticeimpacttype) 
## CircleOutputTypeDef

```python
# CircleOutputTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import CircleOutputTypeDef


def get_value() -> CircleOutputTypeDef:
    return {
        "Center": ...,
    }


# CircleOutputTypeDef definition

class CircleOutputTypeDef(TypedDict):
    Center: List[float],
    Radius: float,
```

## CircleTypeDef

```python
# CircleTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import CircleTypeDef


def get_value() -> CircleTypeDef:
    return {
        "Center": ...,
    }


# CircleTypeDef definition

class CircleTypeDef(TypedDict):
    Center: Sequence[float],
    Radius: float,
```

## CorridorTypeDef

```python
# CorridorTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import CorridorTypeDef


def get_value() -> CorridorTypeDef:
    return {
        "LineString": ...,
    }


# CorridorTypeDef definition

class CorridorTypeDef(TypedDict):
    LineString: Sequence[Sequence[float]],
    Radius: int,
```

## PolylineCorridorTypeDef

```python
# PolylineCorridorTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import PolylineCorridorTypeDef


def get_value() -> PolylineCorridorTypeDef:
    return {
        "Polyline": ...,
    }


# PolylineCorridorTypeDef definition

class PolylineCorridorTypeDef(TypedDict):
    Polyline: str,
    Radius: int,
```

## IsolineAvoidanceZoneCategoryTypeDef

```python
# IsolineAvoidanceZoneCategoryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineAvoidanceZoneCategoryTypeDef


def get_value() -> IsolineAvoidanceZoneCategoryTypeDef:
    return {
        "Category": ...,
    }


# IsolineAvoidanceZoneCategoryTypeDef definition

class IsolineAvoidanceZoneCategoryTypeDef(TypedDict):
    Category: NotRequired[IsolineZoneCategoryType],  # (1)
```

1. See [:material-code-brackets: IsolineZoneCategoryType](./literals.md#isolinezonecategorytype) 
## IsolineVehicleLicensePlateTypeDef

```python
# IsolineVehicleLicensePlateTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineVehicleLicensePlateTypeDef


def get_value() -> IsolineVehicleLicensePlateTypeDef:
    return {
        "LastCharacter": ...,
    }


# IsolineVehicleLicensePlateTypeDef definition

class IsolineVehicleLicensePlateTypeDef(TypedDict):
    LastCharacter: NotRequired[str],
```

## IsolineConnectionGeometryTypeDef

```python
# IsolineConnectionGeometryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineConnectionGeometryTypeDef


def get_value() -> IsolineConnectionGeometryTypeDef:
    return {
        "LineString": ...,
    }


# IsolineConnectionGeometryTypeDef definition

class IsolineConnectionGeometryTypeDef(TypedDict):
    LineString: NotRequired[List[List[float]]],
    Polyline: NotRequired[str],
```

## IsolineMatchingOptionsTypeDef

```python
# IsolineMatchingOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineMatchingOptionsTypeDef


def get_value() -> IsolineMatchingOptionsTypeDef:
    return {
        "NameHint": ...,
    }


# IsolineMatchingOptionsTypeDef definition

class IsolineMatchingOptionsTypeDef(TypedDict):
    NameHint: NotRequired[str],
    OnRoadThreshold: NotRequired[int],
    Radius: NotRequired[int],
    Strategy: NotRequired[MatchingStrategyType],  # (1)
```

1. See [:material-code-brackets: MatchingStrategyType](./literals.md#matchingstrategytype) 
## IsolineSideOfStreetOptionsTypeDef

```python
# IsolineSideOfStreetOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineSideOfStreetOptionsTypeDef


def get_value() -> IsolineSideOfStreetOptionsTypeDef:
    return {
        "Position": ...,
    }


# IsolineSideOfStreetOptionsTypeDef definition

class IsolineSideOfStreetOptionsTypeDef(TypedDict):
    Position: Sequence[float],
    UseWith: NotRequired[SideOfStreetMatchingStrategyType],  # (1)
```

1. See [:material-code-brackets: SideOfStreetMatchingStrategyType](./literals.md#sideofstreetmatchingstrategytype) 
## IsolineShapeGeometryTypeDef

```python
# IsolineShapeGeometryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineShapeGeometryTypeDef


def get_value() -> IsolineShapeGeometryTypeDef:
    return {
        "Polygon": ...,
    }


# IsolineShapeGeometryTypeDef definition

class IsolineShapeGeometryTypeDef(TypedDict):
    Polygon: NotRequired[List[List[List[float]]]],
    PolylinePolygon: NotRequired[List[str]],
```

## IsolineTrailerOptionsTypeDef

```python
# IsolineTrailerOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineTrailerOptionsTypeDef


def get_value() -> IsolineTrailerOptionsTypeDef:
    return {
        "AxleCount": ...,
    }


# IsolineTrailerOptionsTypeDef definition

class IsolineTrailerOptionsTypeDef(TypedDict):
    AxleCount: NotRequired[int],
    TrailerCount: NotRequired[int],
```

## WeightPerAxleGroupTypeDef

```python
# WeightPerAxleGroupTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WeightPerAxleGroupTypeDef


def get_value() -> WeightPerAxleGroupTypeDef:
    return {
        "Single": ...,
    }


# WeightPerAxleGroupTypeDef definition

class WeightPerAxleGroupTypeDef(TypedDict):
    Single: NotRequired[int],
    Tandem: NotRequired[int],
    Triple: NotRequired[int],
    Quad: NotRequired[int],
    Quint: NotRequired[int],
```

## LocalizedStringTypeDef

```python
# LocalizedStringTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import LocalizedStringTypeDef


def get_value() -> LocalizedStringTypeDef:
    return {
        "Language": ...,
    }


# LocalizedStringTypeDef definition

class LocalizedStringTypeDef(TypedDict):
    Value: str,
    Language: NotRequired[str],
```

## WaypointOptimizationExclusionOptionsTypeDef

```python
# WaypointOptimizationExclusionOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationExclusionOptionsTypeDef


def get_value() -> WaypointOptimizationExclusionOptionsTypeDef:
    return {
        "Countries": ...,
    }


# WaypointOptimizationExclusionOptionsTypeDef definition

class WaypointOptimizationExclusionOptionsTypeDef(TypedDict):
    Countries: Sequence[str],
```

## WaypointOptimizationOriginOptionsTypeDef

```python
# WaypointOptimizationOriginOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationOriginOptionsTypeDef


def get_value() -> WaypointOptimizationOriginOptionsTypeDef:
    return {
        "Id": ...,
    }


# WaypointOptimizationOriginOptionsTypeDef definition

class WaypointOptimizationOriginOptionsTypeDef(TypedDict):
    Id: NotRequired[str],
```

## WaypointOptimizationTrafficOptionsTypeDef

```python
# WaypointOptimizationTrafficOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationTrafficOptionsTypeDef


def get_value() -> WaypointOptimizationTrafficOptionsTypeDef:
    return {
        "Usage": ...,
    }


# WaypointOptimizationTrafficOptionsTypeDef definition

class WaypointOptimizationTrafficOptionsTypeDef(TypedDict):
    Usage: NotRequired[TrafficUsageType],  # (1)
```

1. See [:material-code-brackets: TrafficUsageType](./literals.md#trafficusagetype) 
## WaypointOptimizationConnectionTypeDef

```python
# WaypointOptimizationConnectionTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationConnectionTypeDef


def get_value() -> WaypointOptimizationConnectionTypeDef:
    return {
        "Distance": ...,
    }


# WaypointOptimizationConnectionTypeDef definition

class WaypointOptimizationConnectionTypeDef(TypedDict):
    Distance: int,
    From: str,
    RestDuration: int,
    To: str,
    TravelDuration: int,
    WaitDuration: int,
```

## WaypointOptimizationOptimizedWaypointTypeDef

```python
# WaypointOptimizationOptimizedWaypointTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationOptimizedWaypointTypeDef


def get_value() -> WaypointOptimizationOptimizedWaypointTypeDef:
    return {
        "ArrivalTime": ...,
    }


# WaypointOptimizationOptimizedWaypointTypeDef definition

class WaypointOptimizationOptimizedWaypointTypeDef(TypedDict):
    DepartureTime: str,
    Id: str,
    Position: List[float],
    ArrivalTime: NotRequired[str],
    ClusterIndex: NotRequired[int],
```

## WaypointOptimizationTimeBreakdownTypeDef

```python
# WaypointOptimizationTimeBreakdownTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationTimeBreakdownTypeDef


def get_value() -> WaypointOptimizationTimeBreakdownTypeDef:
    return {
        "RestDuration": ...,
    }


# WaypointOptimizationTimeBreakdownTypeDef definition

class WaypointOptimizationTimeBreakdownTypeDef(TypedDict):
    RestDuration: int,
    ServiceDuration: int,
    TravelDuration: int,
    WaitDuration: int,
```

## RoadSnapNoticeTypeDef

```python
# RoadSnapNoticeTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoadSnapNoticeTypeDef


def get_value() -> RoadSnapNoticeTypeDef:
    return {
        "Code": ...,
    }


# RoadSnapNoticeTypeDef definition

class RoadSnapNoticeTypeDef(TypedDict):
    Code: RoadSnapNoticeCodeType,  # (1)
    Title: str,
    TracePointIndexes: List[int],
```

1. See [:material-code-brackets: RoadSnapNoticeCodeType](./literals.md#roadsnapnoticecodetype) 
## RoadSnapSnappedGeometryTypeDef

```python
# RoadSnapSnappedGeometryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoadSnapSnappedGeometryTypeDef


def get_value() -> RoadSnapSnappedGeometryTypeDef:
    return {
        "LineString": ...,
    }


# RoadSnapSnappedGeometryTypeDef definition

class RoadSnapSnappedGeometryTypeDef(TypedDict):
    LineString: NotRequired[List[List[float]]],
    Polyline: NotRequired[str],
```

## RoadSnapSnappedTracePointTypeDef

```python
# RoadSnapSnappedTracePointTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoadSnapSnappedTracePointTypeDef


def get_value() -> RoadSnapSnappedTracePointTypeDef:
    return {
        "Confidence": ...,
    }


# RoadSnapSnappedTracePointTypeDef definition

class RoadSnapSnappedTracePointTypeDef(TypedDict):
    Confidence: float,
    OriginalPosition: List[float],
    SnappedPosition: List[float],
```

## RoadSnapTracePointTypeDef

```python
# RoadSnapTracePointTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoadSnapTracePointTypeDef


def get_value() -> RoadSnapTracePointTypeDef:
    return {
        "Heading": ...,
    }


# RoadSnapTracePointTypeDef definition

class RoadSnapTracePointTypeDef(TypedDict):
    Position: Sequence[float],
    Heading: NotRequired[float],
    Speed: NotRequired[float],
    Timestamp: NotRequired[str],
```

## RoadSnapTrailerOptionsTypeDef

```python
# RoadSnapTrailerOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoadSnapTrailerOptionsTypeDef


def get_value() -> RoadSnapTrailerOptionsTypeDef:
    return {
        "TrailerCount": ...,
    }


# RoadSnapTrailerOptionsTypeDef definition

class RoadSnapTrailerOptionsTypeDef(TypedDict):
    TrailerCount: NotRequired[int],
```

## RouteAvoidanceZoneCategoryTypeDef

```python
# RouteAvoidanceZoneCategoryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteAvoidanceZoneCategoryTypeDef


def get_value() -> RouteAvoidanceZoneCategoryTypeDef:
    return {
        "Category": ...,
    }


# RouteAvoidanceZoneCategoryTypeDef definition

class RouteAvoidanceZoneCategoryTypeDef(TypedDict):
    Category: RouteZoneCategoryType,  # (1)
```

1. See [:material-code-brackets: RouteZoneCategoryType](./literals.md#routezonecategorytype) 
## RouteVehicleLicensePlateTypeDef

```python
# RouteVehicleLicensePlateTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleLicensePlateTypeDef


def get_value() -> RouteVehicleLicensePlateTypeDef:
    return {
        "LastCharacter": ...,
    }


# RouteVehicleLicensePlateTypeDef definition

class RouteVehicleLicensePlateTypeDef(TypedDict):
    LastCharacter: NotRequired[str],
```

## RouteMatchingOptionsTypeDef

```python
# RouteMatchingOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatchingOptionsTypeDef


def get_value() -> RouteMatchingOptionsTypeDef:
    return {
        "NameHint": ...,
    }


# RouteMatchingOptionsTypeDef definition

class RouteMatchingOptionsTypeDef(TypedDict):
    NameHint: NotRequired[str],
    OnRoadThreshold: NotRequired[int],
    Radius: NotRequired[int],
    Strategy: NotRequired[MatchingStrategyType],  # (1)
```

1. See [:material-code-brackets: MatchingStrategyType](./literals.md#matchingstrategytype) 
## RouteSideOfStreetOptionsTypeDef

```python
# RouteSideOfStreetOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteSideOfStreetOptionsTypeDef


def get_value() -> RouteSideOfStreetOptionsTypeDef:
    return {
        "Position": ...,
    }


# RouteSideOfStreetOptionsTypeDef definition

class RouteSideOfStreetOptionsTypeDef(TypedDict):
    Position: Sequence[float],
    UseWith: NotRequired[SideOfStreetMatchingStrategyType],  # (1)
```

1. See [:material-code-brackets: SideOfStreetMatchingStrategyType](./literals.md#sideofstreetmatchingstrategytype) 
## RouteDriverScheduleIntervalTypeDef

```python
# RouteDriverScheduleIntervalTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteDriverScheduleIntervalTypeDef


def get_value() -> RouteDriverScheduleIntervalTypeDef:
    return {
        "DriveDuration": ...,
    }


# RouteDriverScheduleIntervalTypeDef definition

class RouteDriverScheduleIntervalTypeDef(TypedDict):
    DriveDuration: int,
    RestDuration: int,
```

## RouteEmissionTypeTypeDef

```python
# RouteEmissionTypeTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteEmissionTypeTypeDef


def get_value() -> RouteEmissionTypeTypeDef:
    return {
        "Co2EmissionClass": ...,
    }


# RouteEmissionTypeTypeDef definition

class RouteEmissionTypeTypeDef(TypedDict):
    Type: str,
    Co2EmissionClass: NotRequired[str],
```

## RouteFerryAfterTravelStepTypeDef

```python
# RouteFerryAfterTravelStepTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerryAfterTravelStepTypeDef


def get_value() -> RouteFerryAfterTravelStepTypeDef:
    return {
        "Duration": ...,
    }


# RouteFerryAfterTravelStepTypeDef definition

class RouteFerryAfterTravelStepTypeDef(TypedDict):
    Duration: int,
    Type: RouteFerryAfterTravelStepTypeType,  # (1)
    Instruction: NotRequired[str],
```

1. See [:material-code-brackets: RouteFerryAfterTravelStepTypeType](./literals.md#routeferryaftertravelsteptypetype) 
## RouteFerryPlaceTypeDef

```python
# RouteFerryPlaceTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerryPlaceTypeDef


def get_value() -> RouteFerryPlaceTypeDef:
    return {
        "Name": ...,
    }


# RouteFerryPlaceTypeDef definition

class RouteFerryPlaceTypeDef(TypedDict):
    Position: List[float],
    Name: NotRequired[str],
    OriginalPosition: NotRequired[List[float]],
    WaypointIndex: NotRequired[int],
```

## RouteFerryBeforeTravelStepTypeDef

```python
# RouteFerryBeforeTravelStepTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerryBeforeTravelStepTypeDef


def get_value() -> RouteFerryBeforeTravelStepTypeDef:
    return {
        "Duration": ...,
    }


# RouteFerryBeforeTravelStepTypeDef definition

class RouteFerryBeforeTravelStepTypeDef(TypedDict):
    Duration: int,
    Type: RouteFerryBeforeTravelStepTypeType,  # (1)
    Instruction: NotRequired[str],
```

1. See [:material-code-brackets: RouteFerryBeforeTravelStepTypeType](./literals.md#routeferrybeforetravelsteptypetype) 
## RouteFerryNoticeTypeDef

```python
# RouteFerryNoticeTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerryNoticeTypeDef


def get_value() -> RouteFerryNoticeTypeDef:
    return {
        "Code": ...,
    }


# RouteFerryNoticeTypeDef definition

class RouteFerryNoticeTypeDef(TypedDict):
    Code: RouteFerryNoticeCodeType,  # (1)
    Impact: NotRequired[RouteNoticeImpactType],  # (2)
```

1. See [:material-code-brackets: RouteFerryNoticeCodeType](./literals.md#routeferrynoticecodetype) 
2. See [:material-code-brackets: RouteNoticeImpactType](./literals.md#routenoticeimpacttype) 
## RouteFerryTravelStepTypeDef

```python
# RouteFerryTravelStepTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerryTravelStepTypeDef


def get_value() -> RouteFerryTravelStepTypeDef:
    return {
        "Distance": ...,
    }


# RouteFerryTravelStepTypeDef definition

class RouteFerryTravelStepTypeDef(TypedDict):
    Duration: int,
    Type: RouteFerryTravelStepTypeType,  # (1)
    Distance: NotRequired[int],
    GeometryOffset: NotRequired[int],
    Instruction: NotRequired[str],
```

1. See [:material-code-brackets: RouteFerryTravelStepTypeType](./literals.md#routeferrytravelsteptypetype) 
## RouteFerryOverviewSummaryTypeDef

```python
# RouteFerryOverviewSummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerryOverviewSummaryTypeDef


def get_value() -> RouteFerryOverviewSummaryTypeDef:
    return {
        "Distance": ...,
    }


# RouteFerryOverviewSummaryTypeDef definition

class RouteFerryOverviewSummaryTypeDef(TypedDict):
    Distance: int,
    Duration: int,
```

## RouteFerryTravelOnlySummaryTypeDef

```python
# RouteFerryTravelOnlySummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerryTravelOnlySummaryTypeDef


def get_value() -> RouteFerryTravelOnlySummaryTypeDef:
    return {
        "Duration": ...,
    }


# RouteFerryTravelOnlySummaryTypeDef definition

class RouteFerryTravelOnlySummaryTypeDef(TypedDict):
    Duration: int,
```

## RouteLegGeometryTypeDef

```python
# RouteLegGeometryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteLegGeometryTypeDef


def get_value() -> RouteLegGeometryTypeDef:
    return {
        "LineString": ...,
    }


# RouteLegGeometryTypeDef definition

class RouteLegGeometryTypeDef(TypedDict):
    LineString: NotRequired[List[List[float]]],
    Polyline: NotRequired[str],
```

## RouteNumberTypeDef

```python
# RouteNumberTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteNumberTypeDef


def get_value() -> RouteNumberTypeDef:
    return {
        "Direction": ...,
    }


# RouteNumberTypeDef definition

class RouteNumberTypeDef(TypedDict):
    Value: str,
    Direction: NotRequired[RouteDirectionType],  # (1)
    Language: NotRequired[str],
```

1. See [:material-code-brackets: RouteDirectionType](./literals.md#routedirectiontype) 
## RouteMatrixAutoCircleTypeDef

```python
# RouteMatrixAutoCircleTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixAutoCircleTypeDef


def get_value() -> RouteMatrixAutoCircleTypeDef:
    return {
        "Margin": ...,
    }


# RouteMatrixAutoCircleTypeDef definition

class RouteMatrixAutoCircleTypeDef(TypedDict):
    Margin: NotRequired[int],
    MaxRadius: NotRequired[int],
```

## RouteMatrixAvoidanceAreaGeometryTypeDef

```python
# RouteMatrixAvoidanceAreaGeometryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixAvoidanceAreaGeometryTypeDef


def get_value() -> RouteMatrixAvoidanceAreaGeometryTypeDef:
    return {
        "BoundingBox": ...,
    }


# RouteMatrixAvoidanceAreaGeometryTypeDef definition

class RouteMatrixAvoidanceAreaGeometryTypeDef(TypedDict):
    BoundingBox: NotRequired[Sequence[float]],
    Polygon: NotRequired[Sequence[Sequence[Sequence[float]]]],
    PolylinePolygon: NotRequired[Sequence[str]],
```

## RouteMatrixAvoidanceZoneCategoryTypeDef

```python
# RouteMatrixAvoidanceZoneCategoryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixAvoidanceZoneCategoryTypeDef


def get_value() -> RouteMatrixAvoidanceZoneCategoryTypeDef:
    return {
        "Category": ...,
    }


# RouteMatrixAvoidanceZoneCategoryTypeDef definition

class RouteMatrixAvoidanceZoneCategoryTypeDef(TypedDict):
    Category: NotRequired[RouteMatrixZoneCategoryType],  # (1)
```

1. See [:material-code-brackets: RouteMatrixZoneCategoryType](./literals.md#routematrixzonecategorytype) 
## RouteMatrixVehicleLicensePlateTypeDef

```python
# RouteMatrixVehicleLicensePlateTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixVehicleLicensePlateTypeDef


def get_value() -> RouteMatrixVehicleLicensePlateTypeDef:
    return {
        "LastCharacter": ...,
    }


# RouteMatrixVehicleLicensePlateTypeDef definition

class RouteMatrixVehicleLicensePlateTypeDef(TypedDict):
    LastCharacter: NotRequired[str],
```

## RouteMatrixMatchingOptionsTypeDef

```python
# RouteMatrixMatchingOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixMatchingOptionsTypeDef


def get_value() -> RouteMatrixMatchingOptionsTypeDef:
    return {
        "NameHint": ...,
    }


# RouteMatrixMatchingOptionsTypeDef definition

class RouteMatrixMatchingOptionsTypeDef(TypedDict):
    NameHint: NotRequired[str],
    OnRoadThreshold: NotRequired[int],
    Radius: NotRequired[int],
    Strategy: NotRequired[MatchingStrategyType],  # (1)
```

1. See [:material-code-brackets: MatchingStrategyType](./literals.md#matchingstrategytype) 
## RouteMatrixSideOfStreetOptionsTypeDef

```python
# RouteMatrixSideOfStreetOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixSideOfStreetOptionsTypeDef


def get_value() -> RouteMatrixSideOfStreetOptionsTypeDef:
    return {
        "Position": ...,
    }


# RouteMatrixSideOfStreetOptionsTypeDef definition

class RouteMatrixSideOfStreetOptionsTypeDef(TypedDict):
    Position: Sequence[float],
    UseWith: NotRequired[SideOfStreetMatchingStrategyType],  # (1)
```

1. See [:material-code-brackets: SideOfStreetMatchingStrategyType](./literals.md#sideofstreetmatchingstrategytype) 
## RouteMatrixTrailerOptionsTypeDef

```python
# RouteMatrixTrailerOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixTrailerOptionsTypeDef


def get_value() -> RouteMatrixTrailerOptionsTypeDef:
    return {
        "TrailerCount": ...,
    }


# RouteMatrixTrailerOptionsTypeDef definition

class RouteMatrixTrailerOptionsTypeDef(TypedDict):
    TrailerCount: NotRequired[int],
```

## RouteNoticeDetailRangeTypeDef

```python
# RouteNoticeDetailRangeTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteNoticeDetailRangeTypeDef


def get_value() -> RouteNoticeDetailRangeTypeDef:
    return {
        "Min": ...,
    }


# RouteNoticeDetailRangeTypeDef definition

class RouteNoticeDetailRangeTypeDef(TypedDict):
    Min: NotRequired[int],
    Max: NotRequired[int],
```

## RoutePassThroughPlaceTypeDef

```python
# RoutePassThroughPlaceTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePassThroughPlaceTypeDef


def get_value() -> RoutePassThroughPlaceTypeDef:
    return {
        "OriginalPosition": ...,
    }


# RoutePassThroughPlaceTypeDef definition

class RoutePassThroughPlaceTypeDef(TypedDict):
    Position: List[float],
    OriginalPosition: NotRequired[List[float]],
    WaypointIndex: NotRequired[int],
```

## RoutePedestrianPlaceTypeDef

```python
# RoutePedestrianPlaceTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePedestrianPlaceTypeDef


def get_value() -> RoutePedestrianPlaceTypeDef:
    return {
        "Name": ...,
    }


# RoutePedestrianPlaceTypeDef definition

class RoutePedestrianPlaceTypeDef(TypedDict):
    Position: List[float],
    Name: NotRequired[str],
    OriginalPosition: NotRequired[List[float]],
    SideOfStreet: NotRequired[RouteSideOfStreetType],  # (1)
    WaypointIndex: NotRequired[int],
```

1. See [:material-code-brackets: RouteSideOfStreetType](./literals.md#routesideofstreettype) 
## RoutePedestrianNoticeTypeDef

```python
# RoutePedestrianNoticeTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePedestrianNoticeTypeDef


def get_value() -> RoutePedestrianNoticeTypeDef:
    return {
        "Code": ...,
    }


# RoutePedestrianNoticeTypeDef definition

class RoutePedestrianNoticeTypeDef(TypedDict):
    Code: RoutePedestrianNoticeCodeType,  # (1)
    Impact: NotRequired[RouteNoticeImpactType],  # (2)
```

1. See [:material-code-brackets: RoutePedestrianNoticeCodeType](./literals.md#routepedestriannoticecodetype) 
2. See [:material-code-brackets: RouteNoticeImpactType](./literals.md#routenoticeimpacttype) 
## RoutePedestrianOptionsTypeDef

```python
# RoutePedestrianOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePedestrianOptionsTypeDef


def get_value() -> RoutePedestrianOptionsTypeDef:
    return {
        "Speed": ...,
    }


# RoutePedestrianOptionsTypeDef definition

class RoutePedestrianOptionsTypeDef(TypedDict):
    Speed: NotRequired[float],
```

## RoutePedestrianOverviewSummaryTypeDef

```python
# RoutePedestrianOverviewSummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePedestrianOverviewSummaryTypeDef


def get_value() -> RoutePedestrianOverviewSummaryTypeDef:
    return {
        "Distance": ...,
    }


# RoutePedestrianOverviewSummaryTypeDef definition

class RoutePedestrianOverviewSummaryTypeDef(TypedDict):
    Distance: int,
    Duration: int,
```

## RouteSpanDynamicSpeedDetailsTypeDef

```python
# RouteSpanDynamicSpeedDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteSpanDynamicSpeedDetailsTypeDef


def get_value() -> RouteSpanDynamicSpeedDetailsTypeDef:
    return {
        "BestCaseSpeed": ...,
    }


# RouteSpanDynamicSpeedDetailsTypeDef definition

class RouteSpanDynamicSpeedDetailsTypeDef(TypedDict):
    BestCaseSpeed: NotRequired[float],
    TurnDuration: NotRequired[int],
    TypicalSpeed: NotRequired[float],
```

## RouteSpanSpeedLimitDetailsTypeDef

```python
# RouteSpanSpeedLimitDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteSpanSpeedLimitDetailsTypeDef


def get_value() -> RouteSpanSpeedLimitDetailsTypeDef:
    return {
        "MaxSpeed": ...,
    }


# RouteSpanSpeedLimitDetailsTypeDef definition

class RouteSpanSpeedLimitDetailsTypeDef(TypedDict):
    MaxSpeed: NotRequired[float],
    Unlimited: NotRequired[bool],
```

## RoutePedestrianTravelOnlySummaryTypeDef

```python
# RoutePedestrianTravelOnlySummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePedestrianTravelOnlySummaryTypeDef


def get_value() -> RoutePedestrianTravelOnlySummaryTypeDef:
    return {
        "Duration": ...,
    }


# RoutePedestrianTravelOnlySummaryTypeDef definition

class RoutePedestrianTravelOnlySummaryTypeDef(TypedDict):
    Duration: int,
```

## RouteTollPassValidityPeriodTypeDef

```python
# RouteTollPassValidityPeriodTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTollPassValidityPeriodTypeDef


def get_value() -> RouteTollPassValidityPeriodTypeDef:
    return {
        "Period": ...,
    }


# RouteTollPassValidityPeriodTypeDef definition

class RouteTollPassValidityPeriodTypeDef(TypedDict):
    Period: RouteTollPassValidityPeriodTypeType,  # (1)
    PeriodCount: NotRequired[int],
```

1. See [:material-code-brackets: RouteTollPassValidityPeriodTypeType](./literals.md#routetollpassvalidityperiodtypetype) 
## RouteTollPaymentSiteTypeDef

```python
# RouteTollPaymentSiteTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTollPaymentSiteTypeDef


def get_value() -> RouteTollPaymentSiteTypeDef:
    return {
        "Name": ...,
    }


# RouteTollPaymentSiteTypeDef definition

class RouteTollPaymentSiteTypeDef(TypedDict):
    Position: List[float],
    Name: NotRequired[str],
```

## RouteTollPriceValueRangeTypeDef

```python
# RouteTollPriceValueRangeTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTollPriceValueRangeTypeDef


def get_value() -> RouteTollPriceValueRangeTypeDef:
    return {
        "Min": ...,
    }


# RouteTollPriceValueRangeTypeDef definition

class RouteTollPriceValueRangeTypeDef(TypedDict):
    Min: float,
    Max: float,
```

## RouteTransponderTypeDef

```python
# RouteTransponderTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTransponderTypeDef


def get_value() -> RouteTransponderTypeDef:
    return {
        "SystemName": ...,
    }


# RouteTransponderTypeDef definition

class RouteTransponderTypeDef(TypedDict):
    SystemName: NotRequired[str],
```

## RouteTollSystemTypeDef

```python
# RouteTollSystemTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTollSystemTypeDef


def get_value() -> RouteTollSystemTypeDef:
    return {
        "Name": ...,
    }


# RouteTollSystemTypeDef definition

class RouteTollSystemTypeDef(TypedDict):
    Name: NotRequired[str],
```

## RouteTrailerOptionsTypeDef

```python
# RouteTrailerOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTrailerOptionsTypeDef


def get_value() -> RouteTrailerOptionsTypeDef:
    return {
        "AxleCount": ...,
    }


# RouteTrailerOptionsTypeDef definition

class RouteTrailerOptionsTypeDef(TypedDict):
    AxleCount: NotRequired[int],
    TrailerCount: NotRequired[int],
```

## RouteVehiclePlaceTypeDef

```python
# RouteVehiclePlaceTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehiclePlaceTypeDef


def get_value() -> RouteVehiclePlaceTypeDef:
    return {
        "Name": ...,
    }


# RouteVehiclePlaceTypeDef definition

class RouteVehiclePlaceTypeDef(TypedDict):
    Position: List[float],
    Name: NotRequired[str],
    OriginalPosition: NotRequired[List[float]],
    SideOfStreet: NotRequired[RouteSideOfStreetType],  # (1)
    WaypointIndex: NotRequired[int],
```

1. See [:material-code-brackets: RouteSideOfStreetType](./literals.md#routesideofstreettype) 
## RouteVehicleIncidentTypeDef

```python
# RouteVehicleIncidentTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleIncidentTypeDef


def get_value() -> RouteVehicleIncidentTypeDef:
    return {
        "Description": ...,
    }


# RouteVehicleIncidentTypeDef definition

class RouteVehicleIncidentTypeDef(TypedDict):
    Description: NotRequired[str],
    EndTime: NotRequired[str],
    Severity: NotRequired[RouteVehicleIncidentSeverityType],  # (1)
    StartTime: NotRequired[str],
    Type: NotRequired[RouteVehicleIncidentTypeType],  # (2)
```

1. See [:material-code-brackets: RouteVehicleIncidentSeverityType](./literals.md#routevehicleincidentseveritytype) 
2. See [:material-code-brackets: RouteVehicleIncidentTypeType](./literals.md#routevehicleincidenttypetype) 
## RouteZoneTypeDef

```python
# RouteZoneTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteZoneTypeDef


def get_value() -> RouteZoneTypeDef:
    return {
        "Category": ...,
    }


# RouteZoneTypeDef definition

class RouteZoneTypeDef(TypedDict):
    Category: NotRequired[RouteZoneCategoryType],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-brackets: RouteZoneCategoryType](./literals.md#routezonecategorytype) 
## RouteVehicleOverviewSummaryTypeDef

```python
# RouteVehicleOverviewSummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleOverviewSummaryTypeDef


def get_value() -> RouteVehicleOverviewSummaryTypeDef:
    return {
        "BestCaseDuration": ...,
    }


# RouteVehicleOverviewSummaryTypeDef definition

class RouteVehicleOverviewSummaryTypeDef(TypedDict):
    Distance: int,
    Duration: int,
    BestCaseDuration: NotRequired[int],
    TypicalDuration: NotRequired[int],
```

## RouteVehicleTravelOnlySummaryTypeDef

```python
# RouteVehicleTravelOnlySummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleTravelOnlySummaryTypeDef


def get_value() -> RouteVehicleTravelOnlySummaryTypeDef:
    return {
        "BestCaseDuration": ...,
    }


# RouteVehicleTravelOnlySummaryTypeDef definition

class RouteVehicleTravelOnlySummaryTypeDef(TypedDict):
    Duration: int,
    BestCaseDuration: NotRequired[int],
    TypicalDuration: NotRequired[int],
```

## RouteWeightConstraintTypeDef

```python
# RouteWeightConstraintTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteWeightConstraintTypeDef


def get_value() -> RouteWeightConstraintTypeDef:
    return {
        "Type": ...,
    }


# RouteWeightConstraintTypeDef definition

class RouteWeightConstraintTypeDef(TypedDict):
    Type: RouteWeightConstraintTypeType,  # (1)
    Value: int,
```

1. See [:material-code-brackets: RouteWeightConstraintTypeType](./literals.md#routeweightconstrainttypetype) 
## WaypointOptimizationAccessHoursEntryTypeDef

```python
# WaypointOptimizationAccessHoursEntryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationAccessHoursEntryTypeDef


def get_value() -> WaypointOptimizationAccessHoursEntryTypeDef:
    return {
        "DayOfWeek": ...,
    }


# WaypointOptimizationAccessHoursEntryTypeDef definition

class WaypointOptimizationAccessHoursEntryTypeDef(TypedDict):
    DayOfWeek: DayOfWeekType,  # (1)
    TimeOfDay: str,
```

1. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
## WaypointOptimizationAvoidanceAreaGeometryTypeDef

```python
# WaypointOptimizationAvoidanceAreaGeometryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationAvoidanceAreaGeometryTypeDef


def get_value() -> WaypointOptimizationAvoidanceAreaGeometryTypeDef:
    return {
        "BoundingBox": ...,
    }


# WaypointOptimizationAvoidanceAreaGeometryTypeDef definition

class WaypointOptimizationAvoidanceAreaGeometryTypeDef(TypedDict):
    BoundingBox: NotRequired[Sequence[float]],
```

## WaypointOptimizationDrivingDistanceOptionsTypeDef

```python
# WaypointOptimizationDrivingDistanceOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationDrivingDistanceOptionsTypeDef


def get_value() -> WaypointOptimizationDrivingDistanceOptionsTypeDef:
    return {
        "DrivingDistance": ...,
    }


# WaypointOptimizationDrivingDistanceOptionsTypeDef definition

class WaypointOptimizationDrivingDistanceOptionsTypeDef(TypedDict):
    DrivingDistance: int,
```

## WaypointOptimizationSideOfStreetOptionsTypeDef

```python
# WaypointOptimizationSideOfStreetOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationSideOfStreetOptionsTypeDef


def get_value() -> WaypointOptimizationSideOfStreetOptionsTypeDef:
    return {
        "Position": ...,
    }


# WaypointOptimizationSideOfStreetOptionsTypeDef definition

class WaypointOptimizationSideOfStreetOptionsTypeDef(TypedDict):
    Position: Sequence[float],
    UseWith: NotRequired[SideOfStreetMatchingStrategyType],  # (1)
```

1. See [:material-code-brackets: SideOfStreetMatchingStrategyType](./literals.md#sideofstreetmatchingstrategytype) 
## WaypointOptimizationRestProfileTypeDef

```python
# WaypointOptimizationRestProfileTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationRestProfileTypeDef


def get_value() -> WaypointOptimizationRestProfileTypeDef:
    return {
        "Profile": ...,
    }


# WaypointOptimizationRestProfileTypeDef definition

class WaypointOptimizationRestProfileTypeDef(TypedDict):
    Profile: str,
```

## WaypointOptimizationFailedConstraintTypeDef

```python
# WaypointOptimizationFailedConstraintTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationFailedConstraintTypeDef


def get_value() -> WaypointOptimizationFailedConstraintTypeDef:
    return {
        "Constraint": ...,
    }


# WaypointOptimizationFailedConstraintTypeDef definition

class WaypointOptimizationFailedConstraintTypeDef(TypedDict):
    Constraint: NotRequired[WaypointOptimizationConstraintType],  # (1)
    Reason: NotRequired[str],
```

1. See [:material-code-brackets: WaypointOptimizationConstraintType](./literals.md#waypointoptimizationconstrainttype) 
## WaypointOptimizationPedestrianOptionsTypeDef

```python
# WaypointOptimizationPedestrianOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationPedestrianOptionsTypeDef


def get_value() -> WaypointOptimizationPedestrianOptionsTypeDef:
    return {
        "Speed": ...,
    }


# WaypointOptimizationPedestrianOptionsTypeDef definition

class WaypointOptimizationPedestrianOptionsTypeDef(TypedDict):
    Speed: NotRequired[float],
```

## WaypointOptimizationRestCycleDurationsTypeDef

```python
# WaypointOptimizationRestCycleDurationsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationRestCycleDurationsTypeDef


def get_value() -> WaypointOptimizationRestCycleDurationsTypeDef:
    return {
        "RestDuration": ...,
    }


# WaypointOptimizationRestCycleDurationsTypeDef definition

class WaypointOptimizationRestCycleDurationsTypeDef(TypedDict):
    RestDuration: int,
    WorkDuration: int,
```

## WaypointOptimizationTrailerOptionsTypeDef

```python
# WaypointOptimizationTrailerOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationTrailerOptionsTypeDef


def get_value() -> WaypointOptimizationTrailerOptionsTypeDef:
    return {
        "TrailerCount": ...,
    }


# WaypointOptimizationTrailerOptionsTypeDef definition

class WaypointOptimizationTrailerOptionsTypeDef(TypedDict):
    TrailerCount: NotRequired[int],
```

## IsolineAvoidanceAreaGeometryTypeDef

```python
# IsolineAvoidanceAreaGeometryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineAvoidanceAreaGeometryTypeDef


def get_value() -> IsolineAvoidanceAreaGeometryTypeDef:
    return {
        "BoundingBox": ...,
    }


# IsolineAvoidanceAreaGeometryTypeDef definition

class IsolineAvoidanceAreaGeometryTypeDef(TypedDict):
    BoundingBox: NotRequired[Sequence[float]],
    Corridor: NotRequired[CorridorTypeDef],  # (1)
    Polygon: NotRequired[Sequence[Sequence[Sequence[float]]]],
    PolylineCorridor: NotRequired[PolylineCorridorTypeDef],  # (2)
    PolylinePolygon: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: CorridorTypeDef](./type_defs.md#corridortypedef) 
2. See [:material-code-braces: PolylineCorridorTypeDef](./type_defs.md#polylinecorridortypedef) 
## RouteAvoidanceAreaGeometryTypeDef

```python
# RouteAvoidanceAreaGeometryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteAvoidanceAreaGeometryTypeDef


def get_value() -> RouteAvoidanceAreaGeometryTypeDef:
    return {
        "Corridor": ...,
    }


# RouteAvoidanceAreaGeometryTypeDef definition

class RouteAvoidanceAreaGeometryTypeDef(TypedDict):
    Corridor: NotRequired[CorridorTypeDef],  # (1)
    BoundingBox: NotRequired[Sequence[float]],
    Polygon: NotRequired[Sequence[Sequence[Sequence[float]]]],
    PolylineCorridor: NotRequired[PolylineCorridorTypeDef],  # (2)
    PolylinePolygon: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: CorridorTypeDef](./type_defs.md#corridortypedef) 
2. See [:material-code-braces: PolylineCorridorTypeDef](./type_defs.md#polylinecorridortypedef) 
## IsolineCarOptionsTypeDef

```python
# IsolineCarOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineCarOptionsTypeDef


def get_value() -> IsolineCarOptionsTypeDef:
    return {
        "EngineType": ...,
    }


# IsolineCarOptionsTypeDef definition

class IsolineCarOptionsTypeDef(TypedDict):
    EngineType: NotRequired[IsolineEngineTypeType],  # (1)
    LicensePlate: NotRequired[IsolineVehicleLicensePlateTypeDef],  # (2)
    MaxSpeed: NotRequired[float],
    Occupancy: NotRequired[int],
```

1. See [:material-code-brackets: IsolineEngineTypeType](./literals.md#isolineenginetypetype) 
2. See [:material-code-braces: IsolineVehicleLicensePlateTypeDef](./type_defs.md#isolinevehiclelicenseplatetypedef) 
## IsolineScooterOptionsTypeDef

```python
# IsolineScooterOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineScooterOptionsTypeDef


def get_value() -> IsolineScooterOptionsTypeDef:
    return {
        "EngineType": ...,
    }


# IsolineScooterOptionsTypeDef definition

class IsolineScooterOptionsTypeDef(TypedDict):
    EngineType: NotRequired[IsolineEngineTypeType],  # (1)
    LicensePlate: NotRequired[IsolineVehicleLicensePlateTypeDef],  # (2)
    MaxSpeed: NotRequired[float],
    Occupancy: NotRequired[int],
```

1. See [:material-code-brackets: IsolineEngineTypeType](./literals.md#isolineenginetypetype) 
2. See [:material-code-braces: IsolineVehicleLicensePlateTypeDef](./type_defs.md#isolinevehiclelicenseplatetypedef) 
## IsolineConnectionTypeDef

```python
# IsolineConnectionTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineConnectionTypeDef


def get_value() -> IsolineConnectionTypeDef:
    return {
        "FromPolygonIndex": ...,
    }


# IsolineConnectionTypeDef definition

class IsolineConnectionTypeDef(TypedDict):
    FromPolygonIndex: int,
    Geometry: IsolineConnectionGeometryTypeDef,  # (1)
    ToPolygonIndex: int,
```

1. See [:material-code-braces: IsolineConnectionGeometryTypeDef](./type_defs.md#isolineconnectiongeometrytypedef) 
## IsolineDestinationOptionsTypeDef

```python
# IsolineDestinationOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineDestinationOptionsTypeDef


def get_value() -> IsolineDestinationOptionsTypeDef:
    return {
        "AvoidActionsForDistance": ...,
    }


# IsolineDestinationOptionsTypeDef definition

class IsolineDestinationOptionsTypeDef(TypedDict):
    AvoidActionsForDistance: NotRequired[int],
    Heading: NotRequired[float],
    Matching: NotRequired[IsolineMatchingOptionsTypeDef],  # (1)
    SideOfStreet: NotRequired[IsolineSideOfStreetOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: IsolineMatchingOptionsTypeDef](./type_defs.md#isolinematchingoptionstypedef) 
2. See [:material-code-braces: IsolineSideOfStreetOptionsTypeDef](./type_defs.md#isolinesideofstreetoptionstypedef) 
## IsolineOriginOptionsTypeDef

```python
# IsolineOriginOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineOriginOptionsTypeDef


def get_value() -> IsolineOriginOptionsTypeDef:
    return {
        "AvoidActionsForDistance": ...,
    }


# IsolineOriginOptionsTypeDef definition

class IsolineOriginOptionsTypeDef(TypedDict):
    AvoidActionsForDistance: NotRequired[int],
    Heading: NotRequired[float],
    Matching: NotRequired[IsolineMatchingOptionsTypeDef],  # (1)
    SideOfStreet: NotRequired[IsolineSideOfStreetOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: IsolineMatchingOptionsTypeDef](./type_defs.md#isolinematchingoptionstypedef) 
2. See [:material-code-braces: IsolineSideOfStreetOptionsTypeDef](./type_defs.md#isolinesideofstreetoptionstypedef) 
## IsolineTruckOptionsTypeDef

```python
# IsolineTruckOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineTruckOptionsTypeDef


def get_value() -> IsolineTruckOptionsTypeDef:
    return {
        "AxleCount": ...,
    }


# IsolineTruckOptionsTypeDef definition

class IsolineTruckOptionsTypeDef(TypedDict):
    AxleCount: NotRequired[int],
    EngineType: NotRequired[IsolineEngineTypeType],  # (1)
    GrossWeight: NotRequired[int],
    HazardousCargos: NotRequired[Sequence[IsolineHazardousCargoTypeType]],  # (2)
    Height: NotRequired[int],
    HeightAboveFirstAxle: NotRequired[int],
    KpraLength: NotRequired[int],
    Length: NotRequired[int],
    LicensePlate: NotRequired[IsolineVehicleLicensePlateTypeDef],  # (3)
    MaxSpeed: NotRequired[float],
    Occupancy: NotRequired[int],
    PayloadCapacity: NotRequired[int],
    TireCount: NotRequired[int],
    Trailer: NotRequired[IsolineTrailerOptionsTypeDef],  # (4)
    TruckType: NotRequired[IsolineTruckTypeType],  # (5)
    TunnelRestrictionCode: NotRequired[str],
    WeightPerAxle: NotRequired[int],
    WeightPerAxleGroup: NotRequired[WeightPerAxleGroupTypeDef],  # (6)
    Width: NotRequired[int],
```

1. See [:material-code-brackets: IsolineEngineTypeType](./literals.md#isolineenginetypetype) 
2. See [:material-code-brackets: IsolineHazardousCargoTypeType](./literals.md#isolinehazardouscargotypetype) 
3. See [:material-code-braces: IsolineVehicleLicensePlateTypeDef](./type_defs.md#isolinevehiclelicenseplatetypedef) 
4. See [:material-code-braces: IsolineTrailerOptionsTypeDef](./type_defs.md#isolinetraileroptionstypedef) 
5. See [:material-code-brackets: IsolineTruckTypeType](./literals.md#isolinetrucktypetype) 
6. See [:material-code-braces: WeightPerAxleGroupTypeDef](./type_defs.md#weightperaxlegrouptypedef) 
## RouteContinueHighwayStepDetailsTypeDef

```python
# RouteContinueHighwayStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteContinueHighwayStepDetailsTypeDef


def get_value() -> RouteContinueHighwayStepDetailsTypeDef:
    return {
        "Intersection": ...,
    }


# RouteContinueHighwayStepDetailsTypeDef definition

class RouteContinueHighwayStepDetailsTypeDef(TypedDict):
    Intersection: List[LocalizedStringTypeDef],  # (1)
    SteeringDirection: NotRequired[RouteSteeringDirectionType],  # (2)
    TurnAngle: NotRequired[float],
    TurnIntensity: NotRequired[RouteTurnIntensityType],  # (3)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-brackets: RouteSteeringDirectionType](./literals.md#routesteeringdirectiontype) 
3. See [:material-code-brackets: RouteTurnIntensityType](./literals.md#routeturnintensitytype) 
## RouteContinueStepDetailsTypeDef

```python
# RouteContinueStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteContinueStepDetailsTypeDef


def get_value() -> RouteContinueStepDetailsTypeDef:
    return {
        "Intersection": ...,
    }


# RouteContinueStepDetailsTypeDef definition

class RouteContinueStepDetailsTypeDef(TypedDict):
    Intersection: List[LocalizedStringTypeDef],  # (1)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
## RouteEnterHighwayStepDetailsTypeDef

```python
# RouteEnterHighwayStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteEnterHighwayStepDetailsTypeDef


def get_value() -> RouteEnterHighwayStepDetailsTypeDef:
    return {
        "Intersection": ...,
    }


# RouteEnterHighwayStepDetailsTypeDef definition

class RouteEnterHighwayStepDetailsTypeDef(TypedDict):
    Intersection: List[LocalizedStringTypeDef],  # (1)
    SteeringDirection: NotRequired[RouteSteeringDirectionType],  # (2)
    TurnAngle: NotRequired[float],
    TurnIntensity: NotRequired[RouteTurnIntensityType],  # (3)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-brackets: RouteSteeringDirectionType](./literals.md#routesteeringdirectiontype) 
3. See [:material-code-brackets: RouteTurnIntensityType](./literals.md#routeturnintensitytype) 
## RouteExitStepDetailsTypeDef

```python
# RouteExitStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteExitStepDetailsTypeDef


def get_value() -> RouteExitStepDetailsTypeDef:
    return {
        "Intersection": ...,
    }


# RouteExitStepDetailsTypeDef definition

class RouteExitStepDetailsTypeDef(TypedDict):
    Intersection: List[LocalizedStringTypeDef],  # (1)
    RelativeExit: NotRequired[int],
    SteeringDirection: NotRequired[RouteSteeringDirectionType],  # (2)
    TurnAngle: NotRequired[float],
    TurnIntensity: NotRequired[RouteTurnIntensityType],  # (3)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-brackets: RouteSteeringDirectionType](./literals.md#routesteeringdirectiontype) 
3. See [:material-code-brackets: RouteTurnIntensityType](./literals.md#routeturnintensitytype) 
## RouteFerrySpanTypeDef

```python
# RouteFerrySpanTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerrySpanTypeDef


def get_value() -> RouteFerrySpanTypeDef:
    return {
        "Country": ...,
    }


# RouteFerrySpanTypeDef definition

class RouteFerrySpanTypeDef(TypedDict):
    Country: NotRequired[str],
    Distance: NotRequired[int],
    Duration: NotRequired[int],
    GeometryOffset: NotRequired[int],
    Names: NotRequired[List[LocalizedStringTypeDef]],  # (1)
    Region: NotRequired[str],
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
## RouteKeepStepDetailsTypeDef

```python
# RouteKeepStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteKeepStepDetailsTypeDef


def get_value() -> RouteKeepStepDetailsTypeDef:
    return {
        "Intersection": ...,
    }


# RouteKeepStepDetailsTypeDef definition

class RouteKeepStepDetailsTypeDef(TypedDict):
    Intersection: List[LocalizedStringTypeDef],  # (1)
    SteeringDirection: NotRequired[RouteSteeringDirectionType],  # (2)
    TurnAngle: NotRequired[float],
    TurnIntensity: NotRequired[RouteTurnIntensityType],  # (3)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-brackets: RouteSteeringDirectionType](./literals.md#routesteeringdirectiontype) 
3. See [:material-code-brackets: RouteTurnIntensityType](./literals.md#routeturnintensitytype) 
## RouteRampStepDetailsTypeDef

```python
# RouteRampStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteRampStepDetailsTypeDef


def get_value() -> RouteRampStepDetailsTypeDef:
    return {
        "Intersection": ...,
    }


# RouteRampStepDetailsTypeDef definition

class RouteRampStepDetailsTypeDef(TypedDict):
    Intersection: List[LocalizedStringTypeDef],  # (1)
    SteeringDirection: NotRequired[RouteSteeringDirectionType],  # (2)
    TurnAngle: NotRequired[float],
    TurnIntensity: NotRequired[RouteTurnIntensityType],  # (3)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-brackets: RouteSteeringDirectionType](./literals.md#routesteeringdirectiontype) 
3. See [:material-code-brackets: RouteTurnIntensityType](./literals.md#routeturnintensitytype) 
## RouteRoundaboutEnterStepDetailsTypeDef

```python
# RouteRoundaboutEnterStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteRoundaboutEnterStepDetailsTypeDef


def get_value() -> RouteRoundaboutEnterStepDetailsTypeDef:
    return {
        "Intersection": ...,
    }


# RouteRoundaboutEnterStepDetailsTypeDef definition

class RouteRoundaboutEnterStepDetailsTypeDef(TypedDict):
    Intersection: List[LocalizedStringTypeDef],  # (1)
    SteeringDirection: NotRequired[RouteSteeringDirectionType],  # (2)
    TurnAngle: NotRequired[float],
    TurnIntensity: NotRequired[RouteTurnIntensityType],  # (3)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-brackets: RouteSteeringDirectionType](./literals.md#routesteeringdirectiontype) 
3. See [:material-code-brackets: RouteTurnIntensityType](./literals.md#routeturnintensitytype) 
## RouteRoundaboutExitStepDetailsTypeDef

```python
# RouteRoundaboutExitStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteRoundaboutExitStepDetailsTypeDef


def get_value() -> RouteRoundaboutExitStepDetailsTypeDef:
    return {
        "Intersection": ...,
    }


# RouteRoundaboutExitStepDetailsTypeDef definition

class RouteRoundaboutExitStepDetailsTypeDef(TypedDict):
    Intersection: List[LocalizedStringTypeDef],  # (1)
    RelativeExit: NotRequired[int],
    RoundaboutAngle: NotRequired[float],
    SteeringDirection: NotRequired[RouteSteeringDirectionType],  # (2)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-brackets: RouteSteeringDirectionType](./literals.md#routesteeringdirectiontype) 
## RouteRoundaboutPassStepDetailsTypeDef

```python
# RouteRoundaboutPassStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteRoundaboutPassStepDetailsTypeDef


def get_value() -> RouteRoundaboutPassStepDetailsTypeDef:
    return {
        "Intersection": ...,
    }


# RouteRoundaboutPassStepDetailsTypeDef definition

class RouteRoundaboutPassStepDetailsTypeDef(TypedDict):
    Intersection: List[LocalizedStringTypeDef],  # (1)
    SteeringDirection: NotRequired[RouteSteeringDirectionType],  # (2)
    TurnAngle: NotRequired[float],
    TurnIntensity: NotRequired[RouteTurnIntensityType],  # (3)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-brackets: RouteSteeringDirectionType](./literals.md#routesteeringdirectiontype) 
3. See [:material-code-brackets: RouteTurnIntensityType](./literals.md#routeturnintensitytype) 
## RouteTurnStepDetailsTypeDef

```python
# RouteTurnStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTurnStepDetailsTypeDef


def get_value() -> RouteTurnStepDetailsTypeDef:
    return {
        "Intersection": ...,
    }


# RouteTurnStepDetailsTypeDef definition

class RouteTurnStepDetailsTypeDef(TypedDict):
    Intersection: List[LocalizedStringTypeDef],  # (1)
    SteeringDirection: NotRequired[RouteSteeringDirectionType],  # (2)
    TurnAngle: NotRequired[float],
    TurnIntensity: NotRequired[RouteTurnIntensityType],  # (3)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-brackets: RouteSteeringDirectionType](./literals.md#routesteeringdirectiontype) 
3. See [:material-code-brackets: RouteTurnIntensityType](./literals.md#routeturnintensitytype) 
## RouteUTurnStepDetailsTypeDef

```python
# RouteUTurnStepDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteUTurnStepDetailsTypeDef


def get_value() -> RouteUTurnStepDetailsTypeDef:
    return {
        "Intersection": ...,
    }


# RouteUTurnStepDetailsTypeDef definition

class RouteUTurnStepDetailsTypeDef(TypedDict):
    Intersection: List[LocalizedStringTypeDef],  # (1)
    SteeringDirection: NotRequired[RouteSteeringDirectionType],  # (2)
    TurnAngle: NotRequired[float],
    TurnIntensity: NotRequired[RouteTurnIntensityType],  # (3)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-brackets: RouteSteeringDirectionType](./literals.md#routesteeringdirectiontype) 
3. See [:material-code-brackets: RouteTurnIntensityType](./literals.md#routeturnintensitytype) 
## SnapToRoadsResponseTypeDef

```python
# SnapToRoadsResponseTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import SnapToRoadsResponseTypeDef


def get_value() -> SnapToRoadsResponseTypeDef:
    return {
        "Notices": ...,
    }


# SnapToRoadsResponseTypeDef definition

class SnapToRoadsResponseTypeDef(TypedDict):
    Notices: List[RoadSnapNoticeTypeDef],  # (1)
    PricingBucket: str,
    SnappedGeometry: RoadSnapSnappedGeometryTypeDef,  # (2)
    SnappedGeometryFormat: GeometryFormatType,  # (3)
    SnappedTracePoints: List[RoadSnapSnappedTracePointTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: RoadSnapNoticeTypeDef](./type_defs.md#roadsnapnoticetypedef) 
2. See [:material-code-braces: RoadSnapSnappedGeometryTypeDef](./type_defs.md#roadsnapsnappedgeometrytypedef) 
3. See [:material-code-brackets: GeometryFormatType](./literals.md#geometryformattype) 
4. See [:material-code-braces: RoadSnapSnappedTracePointTypeDef](./type_defs.md#roadsnapsnappedtracepointtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RoadSnapTruckOptionsTypeDef

```python
# RoadSnapTruckOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoadSnapTruckOptionsTypeDef


def get_value() -> RoadSnapTruckOptionsTypeDef:
    return {
        "GrossWeight": ...,
    }


# RoadSnapTruckOptionsTypeDef definition

class RoadSnapTruckOptionsTypeDef(TypedDict):
    GrossWeight: NotRequired[int],
    HazardousCargos: NotRequired[Sequence[RoadSnapHazardousCargoTypeType]],  # (1)
    Height: NotRequired[int],
    Length: NotRequired[int],
    Trailer: NotRequired[RoadSnapTrailerOptionsTypeDef],  # (2)
    TunnelRestrictionCode: NotRequired[str],
    Width: NotRequired[int],
```

1. See [:material-code-brackets: RoadSnapHazardousCargoTypeType](./literals.md#roadsnaphazardouscargotypetype) 
2. See [:material-code-braces: RoadSnapTrailerOptionsTypeDef](./type_defs.md#roadsnaptraileroptionstypedef) 
## RouteCarOptionsTypeDef

```python
# RouteCarOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteCarOptionsTypeDef


def get_value() -> RouteCarOptionsTypeDef:
    return {
        "EngineType": ...,
    }


# RouteCarOptionsTypeDef definition

class RouteCarOptionsTypeDef(TypedDict):
    EngineType: NotRequired[RouteEngineTypeType],  # (1)
    LicensePlate: NotRequired[RouteVehicleLicensePlateTypeDef],  # (2)
    MaxSpeed: NotRequired[float],
    Occupancy: NotRequired[int],
```

1. See [:material-code-brackets: RouteEngineTypeType](./literals.md#routeenginetypetype) 
2. See [:material-code-braces: RouteVehicleLicensePlateTypeDef](./type_defs.md#routevehiclelicenseplatetypedef) 
## RouteScooterOptionsTypeDef

```python
# RouteScooterOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteScooterOptionsTypeDef


def get_value() -> RouteScooterOptionsTypeDef:
    return {
        "EngineType": ...,
    }


# RouteScooterOptionsTypeDef definition

class RouteScooterOptionsTypeDef(TypedDict):
    EngineType: NotRequired[RouteEngineTypeType],  # (1)
    LicensePlate: NotRequired[RouteVehicleLicensePlateTypeDef],  # (2)
    MaxSpeed: NotRequired[float],
    Occupancy: NotRequired[int],
```

1. See [:material-code-brackets: RouteEngineTypeType](./literals.md#routeenginetypetype) 
2. See [:material-code-braces: RouteVehicleLicensePlateTypeDef](./type_defs.md#routevehiclelicenseplatetypedef) 
## RouteDestinationOptionsTypeDef

```python
# RouteDestinationOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteDestinationOptionsTypeDef


def get_value() -> RouteDestinationOptionsTypeDef:
    return {
        "AvoidActionsForDistance": ...,
    }


# RouteDestinationOptionsTypeDef definition

class RouteDestinationOptionsTypeDef(TypedDict):
    AvoidActionsForDistance: NotRequired[int],
    AvoidUTurns: NotRequired[bool],
    Heading: NotRequired[float],
    Matching: NotRequired[RouteMatchingOptionsTypeDef],  # (1)
    SideOfStreet: NotRequired[RouteSideOfStreetOptionsTypeDef],  # (2)
    StopDuration: NotRequired[int],
```

1. See [:material-code-braces: RouteMatchingOptionsTypeDef](./type_defs.md#routematchingoptionstypedef) 
2. See [:material-code-braces: RouteSideOfStreetOptionsTypeDef](./type_defs.md#routesideofstreetoptionstypedef) 
## RouteOriginOptionsTypeDef

```python
# RouteOriginOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteOriginOptionsTypeDef


def get_value() -> RouteOriginOptionsTypeDef:
    return {
        "AvoidActionsForDistance": ...,
    }


# RouteOriginOptionsTypeDef definition

class RouteOriginOptionsTypeDef(TypedDict):
    AvoidActionsForDistance: NotRequired[int],
    AvoidUTurns: NotRequired[bool],
    Heading: NotRequired[float],
    Matching: NotRequired[RouteMatchingOptionsTypeDef],  # (1)
    SideOfStreet: NotRequired[RouteSideOfStreetOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: RouteMatchingOptionsTypeDef](./type_defs.md#routematchingoptionstypedef) 
2. See [:material-code-braces: RouteSideOfStreetOptionsTypeDef](./type_defs.md#routesideofstreetoptionstypedef) 
## RouteWaypointTypeDef

```python
# RouteWaypointTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteWaypointTypeDef


def get_value() -> RouteWaypointTypeDef:
    return {
        "AvoidActionsForDistance": ...,
    }


# RouteWaypointTypeDef definition

class RouteWaypointTypeDef(TypedDict):
    Position: Sequence[float],
    AvoidActionsForDistance: NotRequired[int],
    AvoidUTurns: NotRequired[bool],
    Heading: NotRequired[float],
    Matching: NotRequired[RouteMatchingOptionsTypeDef],  # (1)
    PassThrough: NotRequired[bool],
    SideOfStreet: NotRequired[RouteSideOfStreetOptionsTypeDef],  # (2)
    StopDuration: NotRequired[int],
```

1. See [:material-code-braces: RouteMatchingOptionsTypeDef](./type_defs.md#routematchingoptionstypedef) 
2. See [:material-code-braces: RouteSideOfStreetOptionsTypeDef](./type_defs.md#routesideofstreetoptionstypedef) 
## RouteDriverOptionsTypeDef

```python
# RouteDriverOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteDriverOptionsTypeDef


def get_value() -> RouteDriverOptionsTypeDef:
    return {
        "Schedule": ...,
    }


# RouteDriverOptionsTypeDef definition

class RouteDriverOptionsTypeDef(TypedDict):
    Schedule: NotRequired[Sequence[RouteDriverScheduleIntervalTypeDef]],  # (1)
```

1. See [:material-code-braces: RouteDriverScheduleIntervalTypeDef](./type_defs.md#routedriverscheduleintervaltypedef) 
## RouteTollOptionsTypeDef

```python
# RouteTollOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTollOptionsTypeDef


def get_value() -> RouteTollOptionsTypeDef:
    return {
        "AllTransponders": ...,
    }


# RouteTollOptionsTypeDef definition

class RouteTollOptionsTypeDef(TypedDict):
    AllTransponders: NotRequired[bool],
    AllVignettes: NotRequired[bool],
    Currency: NotRequired[str],
    EmissionType: NotRequired[RouteEmissionTypeTypeDef],  # (1)
    VehicleCategory: NotRequired[RouteTollVehicleCategoryType],  # (2)
```

1. See [:material-code-braces: RouteEmissionTypeTypeDef](./type_defs.md#routeemissiontypetypedef) 
2. See [:material-code-brackets: RouteTollVehicleCategoryType](./literals.md#routetollvehiclecategorytype) 
## RouteFerryArrivalTypeDef

```python
# RouteFerryArrivalTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerryArrivalTypeDef


def get_value() -> RouteFerryArrivalTypeDef:
    return {
        "Place": ...,
    }


# RouteFerryArrivalTypeDef definition

class RouteFerryArrivalTypeDef(TypedDict):
    Place: RouteFerryPlaceTypeDef,  # (1)
    Time: NotRequired[str],
```

1. See [:material-code-braces: RouteFerryPlaceTypeDef](./type_defs.md#routeferryplacetypedef) 
## RouteFerryDepartureTypeDef

```python
# RouteFerryDepartureTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerryDepartureTypeDef


def get_value() -> RouteFerryDepartureTypeDef:
    return {
        "Place": ...,
    }


# RouteFerryDepartureTypeDef definition

class RouteFerryDepartureTypeDef(TypedDict):
    Place: RouteFerryPlaceTypeDef,  # (1)
    Time: NotRequired[str],
```

1. See [:material-code-braces: RouteFerryPlaceTypeDef](./type_defs.md#routeferryplacetypedef) 
## RouteFerrySummaryTypeDef

```python
# RouteFerrySummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerrySummaryTypeDef


def get_value() -> RouteFerrySummaryTypeDef:
    return {
        "Overview": ...,
    }


# RouteFerrySummaryTypeDef definition

class RouteFerrySummaryTypeDef(TypedDict):
    Overview: NotRequired[RouteFerryOverviewSummaryTypeDef],  # (1)
    TravelOnly: NotRequired[RouteFerryTravelOnlySummaryTypeDef],  # (2)
```

1. See [:material-code-braces: RouteFerryOverviewSummaryTypeDef](./type_defs.md#routeferryoverviewsummarytypedef) 
2. See [:material-code-braces: RouteFerryTravelOnlySummaryTypeDef](./type_defs.md#routeferrytravelonlysummarytypedef) 
## RouteMajorRoadLabelTypeDef

```python
# RouteMajorRoadLabelTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMajorRoadLabelTypeDef


def get_value() -> RouteMajorRoadLabelTypeDef:
    return {
        "RoadName": ...,
    }


# RouteMajorRoadLabelTypeDef definition

class RouteMajorRoadLabelTypeDef(TypedDict):
    RoadName: NotRequired[LocalizedStringTypeDef],  # (1)
    RouteNumber: NotRequired[RouteNumberTypeDef],  # (2)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-braces: RouteNumberTypeDef](./type_defs.md#routenumbertypedef) 
## RouteRoadTypeDef

```python
# RouteRoadTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteRoadTypeDef


def get_value() -> RouteRoadTypeDef:
    return {
        "RoadName": ...,
    }


# RouteRoadTypeDef definition

class RouteRoadTypeDef(TypedDict):
    RoadName: List[LocalizedStringTypeDef],  # (1)
    RouteNumber: List[RouteNumberTypeDef],  # (2)
    Towards: List[LocalizedStringTypeDef],  # (1)
    Type: NotRequired[RouteRoadTypeType],  # (4)
```

1. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
2. See [:material-code-braces: RouteNumberTypeDef](./type_defs.md#routenumbertypedef) 
3. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
4. See [:material-code-brackets: RouteRoadTypeType](./literals.md#routeroadtypetype) 
## RouteSignpostLabelTypeDef

```python
# RouteSignpostLabelTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteSignpostLabelTypeDef


def get_value() -> RouteSignpostLabelTypeDef:
    return {
        "RouteNumber": ...,
    }


# RouteSignpostLabelTypeDef definition

class RouteSignpostLabelTypeDef(TypedDict):
    RouteNumber: NotRequired[RouteNumberTypeDef],  # (1)
    Text: NotRequired[LocalizedStringTypeDef],  # (2)
```

1. See [:material-code-braces: RouteNumberTypeDef](./type_defs.md#routenumbertypedef) 
2. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
## RouteMatrixBoundaryGeometryOutputTypeDef

```python
# RouteMatrixBoundaryGeometryOutputTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixBoundaryGeometryOutputTypeDef


def get_value() -> RouteMatrixBoundaryGeometryOutputTypeDef:
    return {
        "AutoCircle": ...,
    }


# RouteMatrixBoundaryGeometryOutputTypeDef definition

class RouteMatrixBoundaryGeometryOutputTypeDef(TypedDict):
    AutoCircle: NotRequired[RouteMatrixAutoCircleTypeDef],  # (1)
    Circle: NotRequired[CircleOutputTypeDef],  # (2)
    BoundingBox: NotRequired[List[float]],
    Polygon: NotRequired[List[List[List[float]]]],
```

1. See [:material-code-braces: RouteMatrixAutoCircleTypeDef](./type_defs.md#routematrixautocircletypedef) 
2. See [:material-code-braces: CircleOutputTypeDef](./type_defs.md#circleoutputtypedef) 
## RouteMatrixBoundaryGeometryTypeDef

```python
# RouteMatrixBoundaryGeometryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixBoundaryGeometryTypeDef


def get_value() -> RouteMatrixBoundaryGeometryTypeDef:
    return {
        "AutoCircle": ...,
    }


# RouteMatrixBoundaryGeometryTypeDef definition

class RouteMatrixBoundaryGeometryTypeDef(TypedDict):
    AutoCircle: NotRequired[RouteMatrixAutoCircleTypeDef],  # (1)
    Circle: NotRequired[CircleTypeDef],  # (2)
    BoundingBox: NotRequired[Sequence[float]],
    Polygon: NotRequired[Sequence[Sequence[Sequence[float]]]],
```

1. See [:material-code-braces: RouteMatrixAutoCircleTypeDef](./type_defs.md#routematrixautocircletypedef) 
2. See [:material-code-braces: CircleTypeDef](./type_defs.md#circletypedef) 
## RouteMatrixAvoidanceAreaTypeDef

```python
# RouteMatrixAvoidanceAreaTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixAvoidanceAreaTypeDef


def get_value() -> RouteMatrixAvoidanceAreaTypeDef:
    return {
        "Geometry": ...,
    }


# RouteMatrixAvoidanceAreaTypeDef definition

class RouteMatrixAvoidanceAreaTypeDef(TypedDict):
    Geometry: RouteMatrixAvoidanceAreaGeometryTypeDef,  # (1)
```

1. See [:material-code-braces: RouteMatrixAvoidanceAreaGeometryTypeDef](./type_defs.md#routematrixavoidanceareageometrytypedef) 
## RouteMatrixCarOptionsTypeDef

```python
# RouteMatrixCarOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixCarOptionsTypeDef


def get_value() -> RouteMatrixCarOptionsTypeDef:
    return {
        "LicensePlate": ...,
    }


# RouteMatrixCarOptionsTypeDef definition

class RouteMatrixCarOptionsTypeDef(TypedDict):
    LicensePlate: NotRequired[RouteMatrixVehicleLicensePlateTypeDef],  # (1)
    MaxSpeed: NotRequired[float],
    Occupancy: NotRequired[int],
```

1. See [:material-code-braces: RouteMatrixVehicleLicensePlateTypeDef](./type_defs.md#routematrixvehiclelicenseplatetypedef) 
## RouteMatrixScooterOptionsTypeDef

```python
# RouteMatrixScooterOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixScooterOptionsTypeDef


def get_value() -> RouteMatrixScooterOptionsTypeDef:
    return {
        "LicensePlate": ...,
    }


# RouteMatrixScooterOptionsTypeDef definition

class RouteMatrixScooterOptionsTypeDef(TypedDict):
    LicensePlate: NotRequired[RouteMatrixVehicleLicensePlateTypeDef],  # (1)
    MaxSpeed: NotRequired[float],
    Occupancy: NotRequired[int],
```

1. See [:material-code-braces: RouteMatrixVehicleLicensePlateTypeDef](./type_defs.md#routematrixvehiclelicenseplatetypedef) 
## RouteMatrixDestinationOptionsTypeDef

```python
# RouteMatrixDestinationOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixDestinationOptionsTypeDef


def get_value() -> RouteMatrixDestinationOptionsTypeDef:
    return {
        "AvoidActionsForDistance": ...,
    }


# RouteMatrixDestinationOptionsTypeDef definition

class RouteMatrixDestinationOptionsTypeDef(TypedDict):
    AvoidActionsForDistance: NotRequired[int],
    Heading: NotRequired[float],
    Matching: NotRequired[RouteMatrixMatchingOptionsTypeDef],  # (1)
    SideOfStreet: NotRequired[RouteMatrixSideOfStreetOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: RouteMatrixMatchingOptionsTypeDef](./type_defs.md#routematrixmatchingoptionstypedef) 
2. See [:material-code-braces: RouteMatrixSideOfStreetOptionsTypeDef](./type_defs.md#routematrixsideofstreetoptionstypedef) 
## RouteMatrixOriginOptionsTypeDef

```python
# RouteMatrixOriginOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixOriginOptionsTypeDef


def get_value() -> RouteMatrixOriginOptionsTypeDef:
    return {
        "AvoidActionsForDistance": ...,
    }


# RouteMatrixOriginOptionsTypeDef definition

class RouteMatrixOriginOptionsTypeDef(TypedDict):
    AvoidActionsForDistance: NotRequired[int],
    Heading: NotRequired[float],
    Matching: NotRequired[RouteMatrixMatchingOptionsTypeDef],  # (1)
    SideOfStreet: NotRequired[RouteMatrixSideOfStreetOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: RouteMatrixMatchingOptionsTypeDef](./type_defs.md#routematrixmatchingoptionstypedef) 
2. See [:material-code-braces: RouteMatrixSideOfStreetOptionsTypeDef](./type_defs.md#routematrixsideofstreetoptionstypedef) 
## RouteMatrixTruckOptionsTypeDef

```python
# RouteMatrixTruckOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixTruckOptionsTypeDef


def get_value() -> RouteMatrixTruckOptionsTypeDef:
    return {
        "AxleCount": ...,
    }


# RouteMatrixTruckOptionsTypeDef definition

class RouteMatrixTruckOptionsTypeDef(TypedDict):
    AxleCount: NotRequired[int],
    GrossWeight: NotRequired[int],
    HazardousCargos: NotRequired[Sequence[RouteMatrixHazardousCargoTypeType]],  # (1)
    Height: NotRequired[int],
    KpraLength: NotRequired[int],
    Length: NotRequired[int],
    LicensePlate: NotRequired[RouteMatrixVehicleLicensePlateTypeDef],  # (2)
    MaxSpeed: NotRequired[float],
    Occupancy: NotRequired[int],
    PayloadCapacity: NotRequired[int],
    Trailer: NotRequired[RouteMatrixTrailerOptionsTypeDef],  # (3)
    TruckType: NotRequired[RouteMatrixTruckTypeType],  # (4)
    TunnelRestrictionCode: NotRequired[str],
    WeightPerAxle: NotRequired[int],
    WeightPerAxleGroup: NotRequired[WeightPerAxleGroupTypeDef],  # (5)
    Width: NotRequired[int],
```

1. See [:material-code-brackets: RouteMatrixHazardousCargoTypeType](./literals.md#routematrixhazardouscargotypetype) 
2. See [:material-code-braces: RouteMatrixVehicleLicensePlateTypeDef](./type_defs.md#routematrixvehiclelicenseplatetypedef) 
3. See [:material-code-braces: RouteMatrixTrailerOptionsTypeDef](./type_defs.md#routematrixtraileroptionstypedef) 
4. See [:material-code-brackets: RouteMatrixTruckTypeType](./literals.md#routematrixtrucktypetype) 
5. See [:material-code-braces: WeightPerAxleGroupTypeDef](./type_defs.md#weightperaxlegrouptypedef) 
## RoutePassThroughWaypointTypeDef

```python
# RoutePassThroughWaypointTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePassThroughWaypointTypeDef


def get_value() -> RoutePassThroughWaypointTypeDef:
    return {
        "GeometryOffset": ...,
    }


# RoutePassThroughWaypointTypeDef definition

class RoutePassThroughWaypointTypeDef(TypedDict):
    Place: RoutePassThroughPlaceTypeDef,  # (1)
    GeometryOffset: NotRequired[int],
```

1. See [:material-code-braces: RoutePassThroughPlaceTypeDef](./type_defs.md#routepassthroughplacetypedef) 
## RoutePedestrianArrivalTypeDef

```python
# RoutePedestrianArrivalTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePedestrianArrivalTypeDef


def get_value() -> RoutePedestrianArrivalTypeDef:
    return {
        "Place": ...,
    }


# RoutePedestrianArrivalTypeDef definition

class RoutePedestrianArrivalTypeDef(TypedDict):
    Place: RoutePedestrianPlaceTypeDef,  # (1)
    Time: NotRequired[str],
```

1. See [:material-code-braces: RoutePedestrianPlaceTypeDef](./type_defs.md#routepedestrianplacetypedef) 
## RoutePedestrianDepartureTypeDef

```python
# RoutePedestrianDepartureTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePedestrianDepartureTypeDef


def get_value() -> RoutePedestrianDepartureTypeDef:
    return {
        "Place": ...,
    }


# RoutePedestrianDepartureTypeDef definition

class RoutePedestrianDepartureTypeDef(TypedDict):
    Place: RoutePedestrianPlaceTypeDef,  # (1)
    Time: NotRequired[str],
```

1. See [:material-code-braces: RoutePedestrianPlaceTypeDef](./type_defs.md#routepedestrianplacetypedef) 
## RoutePedestrianSpanTypeDef

```python
# RoutePedestrianSpanTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePedestrianSpanTypeDef


def get_value() -> RoutePedestrianSpanTypeDef:
    return {
        "BestCaseDuration": ...,
    }


# RoutePedestrianSpanTypeDef definition

class RoutePedestrianSpanTypeDef(TypedDict):
    BestCaseDuration: NotRequired[int],
    Country: NotRequired[str],
    Distance: NotRequired[int],
    Duration: NotRequired[int],
    DynamicSpeed: NotRequired[RouteSpanDynamicSpeedDetailsTypeDef],  # (1)
    FunctionalClassification: NotRequired[int],
    GeometryOffset: NotRequired[int],
    Incidents: NotRequired[List[int]],
    Names: NotRequired[List[LocalizedStringTypeDef]],  # (2)
    PedestrianAccess: NotRequired[List[RouteSpanPedestrianAccessAttributeType]],  # (3)
    Region: NotRequired[str],
    RoadAttributes: NotRequired[List[RouteSpanRoadAttributeType]],  # (4)
    RouteNumbers: NotRequired[List[RouteNumberTypeDef]],  # (5)
    SpeedLimit: NotRequired[RouteSpanSpeedLimitDetailsTypeDef],  # (6)
    TypicalDuration: NotRequired[int],
```

1. See [:material-code-braces: RouteSpanDynamicSpeedDetailsTypeDef](./type_defs.md#routespandynamicspeeddetailstypedef) 
2. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
3. See [:material-code-brackets: RouteSpanPedestrianAccessAttributeType](./literals.md#routespanpedestrianaccessattributetype) 
4. See [:material-code-brackets: RouteSpanRoadAttributeType](./literals.md#routespanroadattributetype) 
5. See [:material-code-braces: RouteNumberTypeDef](./type_defs.md#routenumbertypedef) 
6. See [:material-code-braces: RouteSpanSpeedLimitDetailsTypeDef](./type_defs.md#routespanspeedlimitdetailstypedef) 
## RouteVehicleSpanTypeDef

```python
# RouteVehicleSpanTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleSpanTypeDef


def get_value() -> RouteVehicleSpanTypeDef:
    return {
        "BestCaseDuration": ...,
    }


# RouteVehicleSpanTypeDef definition

class RouteVehicleSpanTypeDef(TypedDict):
    BestCaseDuration: NotRequired[int],
    CarAccess: NotRequired[List[RouteSpanCarAccessAttributeType]],  # (1)
    Country: NotRequired[str],
    Distance: NotRequired[int],
    Duration: NotRequired[int],
    DynamicSpeed: NotRequired[RouteSpanDynamicSpeedDetailsTypeDef],  # (2)
    FunctionalClassification: NotRequired[int],
    Gate: NotRequired[RouteSpanGateAttributeType],  # (3)
    GeometryOffset: NotRequired[int],
    Incidents: NotRequired[List[int]],
    Names: NotRequired[List[LocalizedStringTypeDef]],  # (4)
    Notices: NotRequired[List[int]],
    RailwayCrossing: NotRequired[RouteSpanRailwayCrossingAttributeType],  # (5)
    Region: NotRequired[str],
    RoadAttributes: NotRequired[List[RouteSpanRoadAttributeType]],  # (6)
    RouteNumbers: NotRequired[List[RouteNumberTypeDef]],  # (7)
    ScooterAccess: NotRequired[List[RouteSpanScooterAccessAttributeType]],  # (8)
    SpeedLimit: NotRequired[RouteSpanSpeedLimitDetailsTypeDef],  # (9)
    TollSystems: NotRequired[List[int]],
    TruckAccess: NotRequired[List[RouteSpanTruckAccessAttributeType]],  # (10)
    TruckRoadTypes: NotRequired[List[int]],
    TypicalDuration: NotRequired[int],
    Zones: NotRequired[List[int]],
```

1. See [:material-code-brackets: RouteSpanCarAccessAttributeType](./literals.md#routespancaraccessattributetype) 
2. See [:material-code-braces: RouteSpanDynamicSpeedDetailsTypeDef](./type_defs.md#routespandynamicspeeddetailstypedef) 
3. See [:material-code-brackets: RouteSpanGateAttributeType](./literals.md#routespangateattributetype) 
4. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
5. See [:material-code-brackets: RouteSpanRailwayCrossingAttributeType](./literals.md#routespanrailwaycrossingattributetype) 
6. See [:material-code-brackets: RouteSpanRoadAttributeType](./literals.md#routespanroadattributetype) 
7. See [:material-code-braces: RouteNumberTypeDef](./type_defs.md#routenumbertypedef) 
8. See [:material-code-brackets: RouteSpanScooterAccessAttributeType](./literals.md#routespanscooteraccessattributetype) 
9. See [:material-code-braces: RouteSpanSpeedLimitDetailsTypeDef](./type_defs.md#routespanspeedlimitdetailstypedef) 
10. See [:material-code-brackets: RouteSpanTruckAccessAttributeType](./literals.md#routespantruckaccessattributetype) 
## RoutePedestrianSummaryTypeDef

```python
# RoutePedestrianSummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePedestrianSummaryTypeDef


def get_value() -> RoutePedestrianSummaryTypeDef:
    return {
        "Overview": ...,
    }


# RoutePedestrianSummaryTypeDef definition

class RoutePedestrianSummaryTypeDef(TypedDict):
    Overview: NotRequired[RoutePedestrianOverviewSummaryTypeDef],  # (1)
    TravelOnly: NotRequired[RoutePedestrianTravelOnlySummaryTypeDef],  # (2)
```

1. See [:material-code-braces: RoutePedestrianOverviewSummaryTypeDef](./type_defs.md#routepedestrianoverviewsummarytypedef) 
2. See [:material-code-braces: RoutePedestrianTravelOnlySummaryTypeDef](./type_defs.md#routepedestriantravelonlysummarytypedef) 
## RouteTollPassTypeDef

```python
# RouteTollPassTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTollPassTypeDef


def get_value() -> RouteTollPassTypeDef:
    return {
        "IncludesReturnTrip": ...,
    }


# RouteTollPassTypeDef definition

class RouteTollPassTypeDef(TypedDict):
    IncludesReturnTrip: NotRequired[bool],
    SeniorPass: NotRequired[bool],
    TransferCount: NotRequired[int],
    TripCount: NotRequired[int],
    ValidityPeriod: NotRequired[RouteTollPassValidityPeriodTypeDef],  # (1)
```

1. See [:material-code-braces: RouteTollPassValidityPeriodTypeDef](./type_defs.md#routetollpassvalidityperiodtypedef) 
## RouteTollPriceSummaryTypeDef

```python
# RouteTollPriceSummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTollPriceSummaryTypeDef


def get_value() -> RouteTollPriceSummaryTypeDef:
    return {
        "Currency": ...,
    }


# RouteTollPriceSummaryTypeDef definition

class RouteTollPriceSummaryTypeDef(TypedDict):
    Currency: str,
    Estimate: bool,
    Range: bool,
    Value: float,
    RangeValue: NotRequired[RouteTollPriceValueRangeTypeDef],  # (1)
```

1. See [:material-code-braces: RouteTollPriceValueRangeTypeDef](./type_defs.md#routetollpricevaluerangetypedef) 
## RouteTollPriceTypeDef

```python
# RouteTollPriceTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTollPriceTypeDef


def get_value() -> RouteTollPriceTypeDef:
    return {
        "Currency": ...,
    }


# RouteTollPriceTypeDef definition

class RouteTollPriceTypeDef(TypedDict):
    Currency: str,
    Estimate: bool,
    Range: bool,
    Value: float,
    PerDuration: NotRequired[int],
    RangeValue: NotRequired[RouteTollPriceValueRangeTypeDef],  # (1)
```

1. See [:material-code-braces: RouteTollPriceValueRangeTypeDef](./type_defs.md#routetollpricevaluerangetypedef) 
## RouteTruckOptionsTypeDef

```python
# RouteTruckOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTruckOptionsTypeDef


def get_value() -> RouteTruckOptionsTypeDef:
    return {
        "AxleCount": ...,
    }


# RouteTruckOptionsTypeDef definition

class RouteTruckOptionsTypeDef(TypedDict):
    AxleCount: NotRequired[int],
    EngineType: NotRequired[RouteEngineTypeType],  # (1)
    GrossWeight: NotRequired[int],
    HazardousCargos: NotRequired[Sequence[RouteHazardousCargoTypeType]],  # (2)
    Height: NotRequired[int],
    HeightAboveFirstAxle: NotRequired[int],
    KpraLength: NotRequired[int],
    Length: NotRequired[int],
    LicensePlate: NotRequired[RouteVehicleLicensePlateTypeDef],  # (3)
    MaxSpeed: NotRequired[float],
    Occupancy: NotRequired[int],
    PayloadCapacity: NotRequired[int],
    TireCount: NotRequired[int],
    Trailer: NotRequired[RouteTrailerOptionsTypeDef],  # (4)
    TruckType: NotRequired[RouteTruckTypeType],  # (5)
    TunnelRestrictionCode: NotRequired[str],
    WeightPerAxle: NotRequired[int],
    WeightPerAxleGroup: NotRequired[WeightPerAxleGroupTypeDef],  # (6)
    Width: NotRequired[int],
```

1. See [:material-code-brackets: RouteEngineTypeType](./literals.md#routeenginetypetype) 
2. See [:material-code-brackets: RouteHazardousCargoTypeType](./literals.md#routehazardouscargotypetype) 
3. See [:material-code-braces: RouteVehicleLicensePlateTypeDef](./type_defs.md#routevehiclelicenseplatetypedef) 
4. See [:material-code-braces: RouteTrailerOptionsTypeDef](./type_defs.md#routetraileroptionstypedef) 
5. See [:material-code-brackets: RouteTruckTypeType](./literals.md#routetrucktypetype) 
6. See [:material-code-braces: WeightPerAxleGroupTypeDef](./type_defs.md#weightperaxlegrouptypedef) 
## RouteVehicleArrivalTypeDef

```python
# RouteVehicleArrivalTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleArrivalTypeDef


def get_value() -> RouteVehicleArrivalTypeDef:
    return {
        "Place": ...,
    }


# RouteVehicleArrivalTypeDef definition

class RouteVehicleArrivalTypeDef(TypedDict):
    Place: RouteVehiclePlaceTypeDef,  # (1)
    Time: NotRequired[str],
```

1. See [:material-code-braces: RouteVehiclePlaceTypeDef](./type_defs.md#routevehicleplacetypedef) 
## RouteVehicleDepartureTypeDef

```python
# RouteVehicleDepartureTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleDepartureTypeDef


def get_value() -> RouteVehicleDepartureTypeDef:
    return {
        "Place": ...,
    }


# RouteVehicleDepartureTypeDef definition

class RouteVehicleDepartureTypeDef(TypedDict):
    Place: RouteVehiclePlaceTypeDef,  # (1)
    Time: NotRequired[str],
```

1. See [:material-code-braces: RouteVehiclePlaceTypeDef](./type_defs.md#routevehicleplacetypedef) 
## RouteVehicleSummaryTypeDef

```python
# RouteVehicleSummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleSummaryTypeDef


def get_value() -> RouteVehicleSummaryTypeDef:
    return {
        "Overview": ...,
    }


# RouteVehicleSummaryTypeDef definition

class RouteVehicleSummaryTypeDef(TypedDict):
    Overview: NotRequired[RouteVehicleOverviewSummaryTypeDef],  # (1)
    TravelOnly: NotRequired[RouteVehicleTravelOnlySummaryTypeDef],  # (2)
```

1. See [:material-code-braces: RouteVehicleOverviewSummaryTypeDef](./type_defs.md#routevehicleoverviewsummarytypedef) 
2. See [:material-code-braces: RouteVehicleTravelOnlySummaryTypeDef](./type_defs.md#routevehicletravelonlysummarytypedef) 
## RouteViolatedConstraintsTypeDef

```python
# RouteViolatedConstraintsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteViolatedConstraintsTypeDef


def get_value() -> RouteViolatedConstraintsTypeDef:
    return {
        "AllHazardsRestricted": ...,
    }


# RouteViolatedConstraintsTypeDef definition

class RouteViolatedConstraintsTypeDef(TypedDict):
    HazardousCargos: List[RouteHazardousCargoTypeType],  # (2)
    AllHazardsRestricted: NotRequired[bool],
    AxleCount: NotRequired[RouteNoticeDetailRangeTypeDef],  # (1)
    MaxHeight: NotRequired[int],
    MaxKpraLength: NotRequired[int],
    MaxLength: NotRequired[int],
    MaxPayloadCapacity: NotRequired[int],
    MaxWeight: NotRequired[RouteWeightConstraintTypeDef],  # (3)
    MaxWeightPerAxle: NotRequired[int],
    MaxWeightPerAxleGroup: NotRequired[WeightPerAxleGroupTypeDef],  # (4)
    MaxWidth: NotRequired[int],
    Occupancy: NotRequired[RouteNoticeDetailRangeTypeDef],  # (1)
    RestrictedTimes: NotRequired[str],
    TimeDependent: NotRequired[bool],
    TrailerCount: NotRequired[RouteNoticeDetailRangeTypeDef],  # (1)
    TravelMode: NotRequired[bool],
    TruckRoadType: NotRequired[str],
    TruckType: NotRequired[RouteTruckTypeType],  # (7)
    TunnelRestrictionCode: NotRequired[str],
```

1. See [:material-code-braces: RouteNoticeDetailRangeTypeDef](./type_defs.md#routenoticedetailrangetypedef) 
2. See [:material-code-brackets: RouteHazardousCargoTypeType](./literals.md#routehazardouscargotypetype) 
3. See [:material-code-braces: RouteWeightConstraintTypeDef](./type_defs.md#routeweightconstrainttypedef) 
4. See [:material-code-braces: WeightPerAxleGroupTypeDef](./type_defs.md#weightperaxlegrouptypedef) 
5. See [:material-code-braces: RouteNoticeDetailRangeTypeDef](./type_defs.md#routenoticedetailrangetypedef) 
6. See [:material-code-braces: RouteNoticeDetailRangeTypeDef](./type_defs.md#routenoticedetailrangetypedef) 
7. See [:material-code-brackets: RouteTruckTypeType](./literals.md#routetrucktypetype) 
## WaypointOptimizationAccessHoursTypeDef

```python
# WaypointOptimizationAccessHoursTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationAccessHoursTypeDef


def get_value() -> WaypointOptimizationAccessHoursTypeDef:
    return {
        "From": ...,
    }


# WaypointOptimizationAccessHoursTypeDef definition

class WaypointOptimizationAccessHoursTypeDef(TypedDict):
    From: WaypointOptimizationAccessHoursEntryTypeDef,  # (1)
    To: WaypointOptimizationAccessHoursEntryTypeDef,  # (1)
```

1. See [:material-code-braces: WaypointOptimizationAccessHoursEntryTypeDef](./type_defs.md#waypointoptimizationaccesshoursentrytypedef) 
2. See [:material-code-braces: WaypointOptimizationAccessHoursEntryTypeDef](./type_defs.md#waypointoptimizationaccesshoursentrytypedef) 
## WaypointOptimizationAvoidanceAreaTypeDef

```python
# WaypointOptimizationAvoidanceAreaTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationAvoidanceAreaTypeDef


def get_value() -> WaypointOptimizationAvoidanceAreaTypeDef:
    return {
        "Geometry": ...,
    }


# WaypointOptimizationAvoidanceAreaTypeDef definition

class WaypointOptimizationAvoidanceAreaTypeDef(TypedDict):
    Geometry: WaypointOptimizationAvoidanceAreaGeometryTypeDef,  # (1)
```

1. See [:material-code-braces: WaypointOptimizationAvoidanceAreaGeometryTypeDef](./type_defs.md#waypointoptimizationavoidanceareageometrytypedef) 
## WaypointOptimizationClusteringOptionsTypeDef

```python
# WaypointOptimizationClusteringOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationClusteringOptionsTypeDef


def get_value() -> WaypointOptimizationClusteringOptionsTypeDef:
    return {
        "Algorithm": ...,
    }


# WaypointOptimizationClusteringOptionsTypeDef definition

class WaypointOptimizationClusteringOptionsTypeDef(TypedDict):
    Algorithm: WaypointOptimizationClusteringAlgorithmType,  # (1)
    DrivingDistanceOptions: NotRequired[WaypointOptimizationDrivingDistanceOptionsTypeDef],  # (2)
```

1. See [:material-code-brackets: WaypointOptimizationClusteringAlgorithmType](./literals.md#waypointoptimizationclusteringalgorithmtype) 
2. See [:material-code-braces: WaypointOptimizationDrivingDistanceOptionsTypeDef](./type_defs.md#waypointoptimizationdrivingdistanceoptionstypedef) 
## WaypointOptimizationImpedingWaypointTypeDef

```python
# WaypointOptimizationImpedingWaypointTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationImpedingWaypointTypeDef


def get_value() -> WaypointOptimizationImpedingWaypointTypeDef:
    return {
        "FailedConstraints": ...,
    }


# WaypointOptimizationImpedingWaypointTypeDef definition

class WaypointOptimizationImpedingWaypointTypeDef(TypedDict):
    FailedConstraints: List[WaypointOptimizationFailedConstraintTypeDef],  # (1)
    Id: str,
    Position: List[float],
```

1. See [:material-code-braces: WaypointOptimizationFailedConstraintTypeDef](./type_defs.md#waypointoptimizationfailedconstrainttypedef) 
## WaypointOptimizationRestCyclesTypeDef

```python
# WaypointOptimizationRestCyclesTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationRestCyclesTypeDef


def get_value() -> WaypointOptimizationRestCyclesTypeDef:
    return {
        "LongCycle": ...,
    }


# WaypointOptimizationRestCyclesTypeDef definition

class WaypointOptimizationRestCyclesTypeDef(TypedDict):
    LongCycle: WaypointOptimizationRestCycleDurationsTypeDef,  # (1)
    ShortCycle: WaypointOptimizationRestCycleDurationsTypeDef,  # (1)
```

1. See [:material-code-braces: WaypointOptimizationRestCycleDurationsTypeDef](./type_defs.md#waypointoptimizationrestcycledurationstypedef) 
2. See [:material-code-braces: WaypointOptimizationRestCycleDurationsTypeDef](./type_defs.md#waypointoptimizationrestcycledurationstypedef) 
## WaypointOptimizationTruckOptionsTypeDef

```python
# WaypointOptimizationTruckOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationTruckOptionsTypeDef


def get_value() -> WaypointOptimizationTruckOptionsTypeDef:
    return {
        "GrossWeight": ...,
    }


# WaypointOptimizationTruckOptionsTypeDef definition

class WaypointOptimizationTruckOptionsTypeDef(TypedDict):
    GrossWeight: NotRequired[int],
    HazardousCargos: NotRequired[Sequence[WaypointOptimizationHazardousCargoTypeType]],  # (1)
    Height: NotRequired[int],
    Length: NotRequired[int],
    Trailer: NotRequired[WaypointOptimizationTrailerOptionsTypeDef],  # (2)
    TruckType: NotRequired[WaypointOptimizationTruckTypeType],  # (3)
    TunnelRestrictionCode: NotRequired[str],
    WeightPerAxle: NotRequired[int],
    Width: NotRequired[int],
```

1. See [:material-code-brackets: WaypointOptimizationHazardousCargoTypeType](./literals.md#waypointoptimizationhazardouscargotypetype) 
2. See [:material-code-braces: WaypointOptimizationTrailerOptionsTypeDef](./type_defs.md#waypointoptimizationtraileroptionstypedef) 
3. See [:material-code-brackets: WaypointOptimizationTruckTypeType](./literals.md#waypointoptimizationtrucktypetype) 
## IsolineAvoidanceAreaTypeDef

```python
# IsolineAvoidanceAreaTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineAvoidanceAreaTypeDef


def get_value() -> IsolineAvoidanceAreaTypeDef:
    return {
        "Except": ...,
    }


# IsolineAvoidanceAreaTypeDef definition

class IsolineAvoidanceAreaTypeDef(TypedDict):
    Geometry: IsolineAvoidanceAreaGeometryTypeDef,  # (2)
    Except: NotRequired[Sequence[IsolineAvoidanceAreaGeometryTypeDef]],  # (1)
```

1. See [:material-code-braces: IsolineAvoidanceAreaGeometryTypeDef](./type_defs.md#isolineavoidanceareageometrytypedef) 
2. See [:material-code-braces: IsolineAvoidanceAreaGeometryTypeDef](./type_defs.md#isolineavoidanceareageometrytypedef) 
## RouteAvoidanceAreaTypeDef

```python
# RouteAvoidanceAreaTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteAvoidanceAreaTypeDef


def get_value() -> RouteAvoidanceAreaTypeDef:
    return {
        "Except": ...,
    }


# RouteAvoidanceAreaTypeDef definition

class RouteAvoidanceAreaTypeDef(TypedDict):
    Geometry: RouteAvoidanceAreaGeometryTypeDef,  # (2)
    Except: NotRequired[Sequence[RouteAvoidanceAreaGeometryTypeDef]],  # (1)
```

1. See [:material-code-braces: RouteAvoidanceAreaGeometryTypeDef](./type_defs.md#routeavoidanceareageometrytypedef) 
2. See [:material-code-braces: RouteAvoidanceAreaGeometryTypeDef](./type_defs.md#routeavoidanceareageometrytypedef) 
## IsolineTypeDef

```python
# IsolineTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineTypeDef


def get_value() -> IsolineTypeDef:
    return {
        "Connections": ...,
    }


# IsolineTypeDef definition

class IsolineTypeDef(TypedDict):
    Connections: List[IsolineConnectionTypeDef],  # (1)
    Geometries: List[IsolineShapeGeometryTypeDef],  # (2)
    DistanceThreshold: NotRequired[int],
    TimeThreshold: NotRequired[int],
```

1. See [:material-code-braces: IsolineConnectionTypeDef](./type_defs.md#isolineconnectiontypedef) 
2. See [:material-code-braces: IsolineShapeGeometryTypeDef](./type_defs.md#isolineshapegeometrytypedef) 
## IsolineTravelModeOptionsTypeDef

```python
# IsolineTravelModeOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineTravelModeOptionsTypeDef


def get_value() -> IsolineTravelModeOptionsTypeDef:
    return {
        "Car": ...,
    }


# IsolineTravelModeOptionsTypeDef definition

class IsolineTravelModeOptionsTypeDef(TypedDict):
    Car: NotRequired[IsolineCarOptionsTypeDef],  # (1)
    Scooter: NotRequired[IsolineScooterOptionsTypeDef],  # (2)
    Truck: NotRequired[IsolineTruckOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: IsolineCarOptionsTypeDef](./type_defs.md#isolinecaroptionstypedef) 
2. See [:material-code-braces: IsolineScooterOptionsTypeDef](./type_defs.md#isolinescooteroptionstypedef) 
3. See [:material-code-braces: IsolineTruckOptionsTypeDef](./type_defs.md#isolinetruckoptionstypedef) 
## RoadSnapTravelModeOptionsTypeDef

```python
# RoadSnapTravelModeOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoadSnapTravelModeOptionsTypeDef


def get_value() -> RoadSnapTravelModeOptionsTypeDef:
    return {
        "Truck": ...,
    }


# RoadSnapTravelModeOptionsTypeDef definition

class RoadSnapTravelModeOptionsTypeDef(TypedDict):
    Truck: NotRequired[RoadSnapTruckOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: RoadSnapTruckOptionsTypeDef](./type_defs.md#roadsnaptruckoptionstypedef) 
## RouteSignpostTypeDef

```python
# RouteSignpostTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteSignpostTypeDef


def get_value() -> RouteSignpostTypeDef:
    return {
        "Labels": ...,
    }


# RouteSignpostTypeDef definition

class RouteSignpostTypeDef(TypedDict):
    Labels: List[RouteSignpostLabelTypeDef],  # (1)
```

1. See [:material-code-braces: RouteSignpostLabelTypeDef](./type_defs.md#routesignpostlabeltypedef) 
## RouteMatrixBoundaryOutputTypeDef

```python
# RouteMatrixBoundaryOutputTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixBoundaryOutputTypeDef


def get_value() -> RouteMatrixBoundaryOutputTypeDef:
    return {
        "Geometry": ...,
    }


# RouteMatrixBoundaryOutputTypeDef definition

class RouteMatrixBoundaryOutputTypeDef(TypedDict):
    Geometry: NotRequired[RouteMatrixBoundaryGeometryOutputTypeDef],  # (1)
    Unbounded: NotRequired[bool],
```

1. See [:material-code-braces: RouteMatrixBoundaryGeometryOutputTypeDef](./type_defs.md#routematrixboundarygeometryoutputtypedef) 
## RouteMatrixBoundaryTypeDef

```python
# RouteMatrixBoundaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixBoundaryTypeDef


def get_value() -> RouteMatrixBoundaryTypeDef:
    return {
        "Geometry": ...,
    }


# RouteMatrixBoundaryTypeDef definition

class RouteMatrixBoundaryTypeDef(TypedDict):
    Geometry: NotRequired[RouteMatrixBoundaryGeometryTypeDef],  # (1)
    Unbounded: NotRequired[bool],
```

1. See [:material-code-braces: RouteMatrixBoundaryGeometryTypeDef](./type_defs.md#routematrixboundarygeometrytypedef) 
## RouteMatrixAvoidanceOptionsTypeDef

```python
# RouteMatrixAvoidanceOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixAvoidanceOptionsTypeDef


def get_value() -> RouteMatrixAvoidanceOptionsTypeDef:
    return {
        "Areas": ...,
    }


# RouteMatrixAvoidanceOptionsTypeDef definition

class RouteMatrixAvoidanceOptionsTypeDef(TypedDict):
    Areas: NotRequired[Sequence[RouteMatrixAvoidanceAreaTypeDef]],  # (1)
    CarShuttleTrains: NotRequired[bool],
    ControlledAccessHighways: NotRequired[bool],
    DirtRoads: NotRequired[bool],
    Ferries: NotRequired[bool],
    TollRoads: NotRequired[bool],
    TollTransponders: NotRequired[bool],
    TruckRoadTypes: NotRequired[Sequence[str]],
    Tunnels: NotRequired[bool],
    UTurns: NotRequired[bool],
    ZoneCategories: NotRequired[Sequence[RouteMatrixAvoidanceZoneCategoryTypeDef]],  # (2)
```

1. See [:material-code-braces: RouteMatrixAvoidanceAreaTypeDef](./type_defs.md#routematrixavoidanceareatypedef) 
2. See [:material-code-braces: RouteMatrixAvoidanceZoneCategoryTypeDef](./type_defs.md#routematrixavoidancezonecategorytypedef) 
## RouteMatrixDestinationTypeDef

```python
# RouteMatrixDestinationTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixDestinationTypeDef


def get_value() -> RouteMatrixDestinationTypeDef:
    return {
        "Options": ...,
    }


# RouteMatrixDestinationTypeDef definition

class RouteMatrixDestinationTypeDef(TypedDict):
    Position: Sequence[float],
    Options: NotRequired[RouteMatrixDestinationOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: RouteMatrixDestinationOptionsTypeDef](./type_defs.md#routematrixdestinationoptionstypedef) 
## RouteMatrixOriginTypeDef

```python
# RouteMatrixOriginTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixOriginTypeDef


def get_value() -> RouteMatrixOriginTypeDef:
    return {
        "Options": ...,
    }


# RouteMatrixOriginTypeDef definition

class RouteMatrixOriginTypeDef(TypedDict):
    Position: Sequence[float],
    Options: NotRequired[RouteMatrixOriginOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: RouteMatrixOriginOptionsTypeDef](./type_defs.md#routematrixoriginoptionstypedef) 
## RouteMatrixTravelModeOptionsTypeDef

```python
# RouteMatrixTravelModeOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteMatrixTravelModeOptionsTypeDef


def get_value() -> RouteMatrixTravelModeOptionsTypeDef:
    return {
        "Car": ...,
    }


# RouteMatrixTravelModeOptionsTypeDef definition

class RouteMatrixTravelModeOptionsTypeDef(TypedDict):
    Car: NotRequired[RouteMatrixCarOptionsTypeDef],  # (1)
    Scooter: NotRequired[RouteMatrixScooterOptionsTypeDef],  # (2)
    Truck: NotRequired[RouteMatrixTruckOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: RouteMatrixCarOptionsTypeDef](./type_defs.md#routematrixcaroptionstypedef) 
2. See [:material-code-braces: RouteMatrixScooterOptionsTypeDef](./type_defs.md#routematrixscooteroptionstypedef) 
3. See [:material-code-braces: RouteMatrixTruckOptionsTypeDef](./type_defs.md#routematrixtruckoptionstypedef) 
## RouteFerryLegDetailsTypeDef

```python
# RouteFerryLegDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteFerryLegDetailsTypeDef


def get_value() -> RouteFerryLegDetailsTypeDef:
    return {
        "AfterTravelSteps": ...,
    }


# RouteFerryLegDetailsTypeDef definition

class RouteFerryLegDetailsTypeDef(TypedDict):
    AfterTravelSteps: List[RouteFerryAfterTravelStepTypeDef],  # (1)
    Arrival: RouteFerryArrivalTypeDef,  # (2)
    BeforeTravelSteps: List[RouteFerryBeforeTravelStepTypeDef],  # (3)
    Departure: RouteFerryDepartureTypeDef,  # (4)
    Notices: List[RouteFerryNoticeTypeDef],  # (5)
    PassThroughWaypoints: List[RoutePassThroughWaypointTypeDef],  # (6)
    Spans: List[RouteFerrySpanTypeDef],  # (7)
    TravelSteps: List[RouteFerryTravelStepTypeDef],  # (9)
    RouteName: NotRequired[str],
    Summary: NotRequired[RouteFerrySummaryTypeDef],  # (8)
```

1. See [:material-code-braces: RouteFerryAfterTravelStepTypeDef](./type_defs.md#routeferryaftertravelsteptypedef) 
2. See [:material-code-braces: RouteFerryArrivalTypeDef](./type_defs.md#routeferryarrivaltypedef) 
3. See [:material-code-braces: RouteFerryBeforeTravelStepTypeDef](./type_defs.md#routeferrybeforetravelsteptypedef) 
4. See [:material-code-braces: RouteFerryDepartureTypeDef](./type_defs.md#routeferrydeparturetypedef) 
5. See [:material-code-braces: RouteFerryNoticeTypeDef](./type_defs.md#routeferrynoticetypedef) 
6. See [:material-code-braces: RoutePassThroughWaypointTypeDef](./type_defs.md#routepassthroughwaypointtypedef) 
7. See [:material-code-braces: RouteFerrySpanTypeDef](./type_defs.md#routeferryspantypedef) 
8. See [:material-code-braces: RouteFerrySummaryTypeDef](./type_defs.md#routeferrysummarytypedef) 
9. See [:material-code-braces: RouteFerryTravelStepTypeDef](./type_defs.md#routeferrytravelsteptypedef) 
## RouteTollSummaryTypeDef

```python
# RouteTollSummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTollSummaryTypeDef


def get_value() -> RouteTollSummaryTypeDef:
    return {
        "Total": ...,
    }


# RouteTollSummaryTypeDef definition

class RouteTollSummaryTypeDef(TypedDict):
    Total: NotRequired[RouteTollPriceSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: RouteTollPriceSummaryTypeDef](./type_defs.md#routetollpricesummarytypedef) 
## RouteTollRateTypeDef

```python
# RouteTollRateTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTollRateTypeDef


def get_value() -> RouteTollRateTypeDef:
    return {
        "ApplicableTimes": ...,
    }


# RouteTollRateTypeDef definition

class RouteTollRateTypeDef(TypedDict):
    Id: str,
    LocalPrice: RouteTollPriceTypeDef,  # (1)
    Name: str,
    PaymentMethods: List[RouteTollPaymentMethodType],  # (4)
    Transponders: List[RouteTransponderTypeDef],  # (5)
    ApplicableTimes: NotRequired[str],
    ConvertedPrice: NotRequired[RouteTollPriceTypeDef],  # (1)
    Pass: NotRequired[RouteTollPassTypeDef],  # (3)
```

1. See [:material-code-braces: RouteTollPriceTypeDef](./type_defs.md#routetollpricetypedef) 
2. See [:material-code-braces: RouteTollPriceTypeDef](./type_defs.md#routetollpricetypedef) 
3. See [:material-code-braces: RouteTollPassTypeDef](./type_defs.md#routetollpasstypedef) 
4. See [:material-code-brackets: RouteTollPaymentMethodType](./literals.md#routetollpaymentmethodtype) 
5. See [:material-code-braces: RouteTransponderTypeDef](./type_defs.md#routetranspondertypedef) 
## RouteTravelModeOptionsTypeDef

```python
# RouteTravelModeOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTravelModeOptionsTypeDef


def get_value() -> RouteTravelModeOptionsTypeDef:
    return {
        "Car": ...,
    }


# RouteTravelModeOptionsTypeDef definition

class RouteTravelModeOptionsTypeDef(TypedDict):
    Car: NotRequired[RouteCarOptionsTypeDef],  # (1)
    Pedestrian: NotRequired[RoutePedestrianOptionsTypeDef],  # (2)
    Scooter: NotRequired[RouteScooterOptionsTypeDef],  # (3)
    Truck: NotRequired[RouteTruckOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: RouteCarOptionsTypeDef](./type_defs.md#routecaroptionstypedef) 
2. See [:material-code-braces: RoutePedestrianOptionsTypeDef](./type_defs.md#routepedestrianoptionstypedef) 
3. See [:material-code-braces: RouteScooterOptionsTypeDef](./type_defs.md#routescooteroptionstypedef) 
4. See [:material-code-braces: RouteTruckOptionsTypeDef](./type_defs.md#routetruckoptionstypedef) 
## RouteVehicleNoticeDetailTypeDef

```python
# RouteVehicleNoticeDetailTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleNoticeDetailTypeDef


def get_value() -> RouteVehicleNoticeDetailTypeDef:
    return {
        "Title": ...,
    }


# RouteVehicleNoticeDetailTypeDef definition

class RouteVehicleNoticeDetailTypeDef(TypedDict):
    Title: NotRequired[str],
    ViolatedConstraints: NotRequired[RouteViolatedConstraintsTypeDef],  # (1)
```

1. See [:material-code-braces: RouteViolatedConstraintsTypeDef](./type_defs.md#routeviolatedconstraintstypedef) 
## WaypointOptimizationDestinationOptionsTypeDef

```python
# WaypointOptimizationDestinationOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationDestinationOptionsTypeDef


def get_value() -> WaypointOptimizationDestinationOptionsTypeDef:
    return {
        "AccessHours": ...,
    }


# WaypointOptimizationDestinationOptionsTypeDef definition

class WaypointOptimizationDestinationOptionsTypeDef(TypedDict):
    AccessHours: NotRequired[WaypointOptimizationAccessHoursTypeDef],  # (1)
    AppointmentTime: NotRequired[str],
    Heading: NotRequired[float],
    Id: NotRequired[str],
    ServiceDuration: NotRequired[int],
    SideOfStreet: NotRequired[WaypointOptimizationSideOfStreetOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: WaypointOptimizationAccessHoursTypeDef](./type_defs.md#waypointoptimizationaccesshourstypedef) 
2. See [:material-code-braces: WaypointOptimizationSideOfStreetOptionsTypeDef](./type_defs.md#waypointoptimizationsideofstreetoptionstypedef) 
## WaypointOptimizationWaypointTypeDef

```python
# WaypointOptimizationWaypointTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationWaypointTypeDef


def get_value() -> WaypointOptimizationWaypointTypeDef:
    return {
        "AccessHours": ...,
    }


# WaypointOptimizationWaypointTypeDef definition

class WaypointOptimizationWaypointTypeDef(TypedDict):
    Position: Sequence[float],
    AccessHours: NotRequired[WaypointOptimizationAccessHoursTypeDef],  # (1)
    AppointmentTime: NotRequired[str],
    Before: NotRequired[Sequence[int]],
    Heading: NotRequired[float],
    Id: NotRequired[str],
    ServiceDuration: NotRequired[int],
    SideOfStreet: NotRequired[WaypointOptimizationSideOfStreetOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: WaypointOptimizationAccessHoursTypeDef](./type_defs.md#waypointoptimizationaccesshourstypedef) 
2. See [:material-code-braces: WaypointOptimizationSideOfStreetOptionsTypeDef](./type_defs.md#waypointoptimizationsideofstreetoptionstypedef) 
## WaypointOptimizationAvoidanceOptionsTypeDef

```python
# WaypointOptimizationAvoidanceOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationAvoidanceOptionsTypeDef


def get_value() -> WaypointOptimizationAvoidanceOptionsTypeDef:
    return {
        "Areas": ...,
    }


# WaypointOptimizationAvoidanceOptionsTypeDef definition

class WaypointOptimizationAvoidanceOptionsTypeDef(TypedDict):
    Areas: NotRequired[Sequence[WaypointOptimizationAvoidanceAreaTypeDef]],  # (1)
    CarShuttleTrains: NotRequired[bool],
    ControlledAccessHighways: NotRequired[bool],
    DirtRoads: NotRequired[bool],
    Ferries: NotRequired[bool],
    TollRoads: NotRequired[bool],
    Tunnels: NotRequired[bool],
    UTurns: NotRequired[bool],
```

1. See [:material-code-braces: WaypointOptimizationAvoidanceAreaTypeDef](./type_defs.md#waypointoptimizationavoidanceareatypedef) 
## OptimizeWaypointsResponseTypeDef

```python
# OptimizeWaypointsResponseTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import OptimizeWaypointsResponseTypeDef


def get_value() -> OptimizeWaypointsResponseTypeDef:
    return {
        "Connections": ...,
    }


# OptimizeWaypointsResponseTypeDef definition

class OptimizeWaypointsResponseTypeDef(TypedDict):
    Connections: List[WaypointOptimizationConnectionTypeDef],  # (1)
    Distance: int,
    Duration: int,
    ImpedingWaypoints: List[WaypointOptimizationImpedingWaypointTypeDef],  # (2)
    OptimizedWaypoints: List[WaypointOptimizationOptimizedWaypointTypeDef],  # (3)
    PricingBucket: str,
    TimeBreakdown: WaypointOptimizationTimeBreakdownTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: WaypointOptimizationConnectionTypeDef](./type_defs.md#waypointoptimizationconnectiontypedef) 
2. See [:material-code-braces: WaypointOptimizationImpedingWaypointTypeDef](./type_defs.md#waypointoptimizationimpedingwaypointtypedef) 
3. See [:material-code-braces: WaypointOptimizationOptimizedWaypointTypeDef](./type_defs.md#waypointoptimizationoptimizedwaypointtypedef) 
4. See [:material-code-braces: WaypointOptimizationTimeBreakdownTypeDef](./type_defs.md#waypointoptimizationtimebreakdowntypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WaypointOptimizationDriverOptionsTypeDef

```python
# WaypointOptimizationDriverOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationDriverOptionsTypeDef


def get_value() -> WaypointOptimizationDriverOptionsTypeDef:
    return {
        "RestCycles": ...,
    }


# WaypointOptimizationDriverOptionsTypeDef definition

class WaypointOptimizationDriverOptionsTypeDef(TypedDict):
    RestCycles: NotRequired[WaypointOptimizationRestCyclesTypeDef],  # (1)
    RestProfile: NotRequired[WaypointOptimizationRestProfileTypeDef],  # (2)
    TreatServiceTimeAs: NotRequired[WaypointOptimizationServiceTimeTreatmentType],  # (3)
```

1. See [:material-code-braces: WaypointOptimizationRestCyclesTypeDef](./type_defs.md#waypointoptimizationrestcyclestypedef) 
2. See [:material-code-braces: WaypointOptimizationRestProfileTypeDef](./type_defs.md#waypointoptimizationrestprofiletypedef) 
3. See [:material-code-brackets: WaypointOptimizationServiceTimeTreatmentType](./literals.md#waypointoptimizationservicetimetreatmenttype) 
## WaypointOptimizationTravelModeOptionsTypeDef

```python
# WaypointOptimizationTravelModeOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import WaypointOptimizationTravelModeOptionsTypeDef


def get_value() -> WaypointOptimizationTravelModeOptionsTypeDef:
    return {
        "Pedestrian": ...,
    }


# WaypointOptimizationTravelModeOptionsTypeDef definition

class WaypointOptimizationTravelModeOptionsTypeDef(TypedDict):
    Pedestrian: NotRequired[WaypointOptimizationPedestrianOptionsTypeDef],  # (1)
    Truck: NotRequired[WaypointOptimizationTruckOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: WaypointOptimizationPedestrianOptionsTypeDef](./type_defs.md#waypointoptimizationpedestrianoptionstypedef) 
2. See [:material-code-braces: WaypointOptimizationTruckOptionsTypeDef](./type_defs.md#waypointoptimizationtruckoptionstypedef) 
## IsolineAvoidanceOptionsTypeDef

```python
# IsolineAvoidanceOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import IsolineAvoidanceOptionsTypeDef


def get_value() -> IsolineAvoidanceOptionsTypeDef:
    return {
        "Areas": ...,
    }


# IsolineAvoidanceOptionsTypeDef definition

class IsolineAvoidanceOptionsTypeDef(TypedDict):
    Areas: NotRequired[Sequence[IsolineAvoidanceAreaTypeDef]],  # (1)
    CarShuttleTrains: NotRequired[bool],
    ControlledAccessHighways: NotRequired[bool],
    DirtRoads: NotRequired[bool],
    Ferries: NotRequired[bool],
    SeasonalClosure: NotRequired[bool],
    TollRoads: NotRequired[bool],
    TollTransponders: NotRequired[bool],
    TruckRoadTypes: NotRequired[Sequence[str]],
    Tunnels: NotRequired[bool],
    UTurns: NotRequired[bool],
    ZoneCategories: NotRequired[Sequence[IsolineAvoidanceZoneCategoryTypeDef]],  # (2)
```

1. See [:material-code-braces: IsolineAvoidanceAreaTypeDef](./type_defs.md#isolineavoidanceareatypedef) 
2. See [:material-code-braces: IsolineAvoidanceZoneCategoryTypeDef](./type_defs.md#isolineavoidancezonecategorytypedef) 
## RouteAvoidanceOptionsTypeDef

```python
# RouteAvoidanceOptionsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteAvoidanceOptionsTypeDef


def get_value() -> RouteAvoidanceOptionsTypeDef:
    return {
        "Areas": ...,
    }


# RouteAvoidanceOptionsTypeDef definition

class RouteAvoidanceOptionsTypeDef(TypedDict):
    Areas: NotRequired[Sequence[RouteAvoidanceAreaTypeDef]],  # (1)
    CarShuttleTrains: NotRequired[bool],
    ControlledAccessHighways: NotRequired[bool],
    DirtRoads: NotRequired[bool],
    Ferries: NotRequired[bool],
    SeasonalClosure: NotRequired[bool],
    TollRoads: NotRequired[bool],
    TollTransponders: NotRequired[bool],
    TruckRoadTypes: NotRequired[Sequence[str]],
    Tunnels: NotRequired[bool],
    UTurns: NotRequired[bool],
    ZoneCategories: NotRequired[Sequence[RouteAvoidanceZoneCategoryTypeDef]],  # (2)
```

1. See [:material-code-braces: RouteAvoidanceAreaTypeDef](./type_defs.md#routeavoidanceareatypedef) 
2. See [:material-code-braces: RouteAvoidanceZoneCategoryTypeDef](./type_defs.md#routeavoidancezonecategorytypedef) 
## CalculateIsolinesResponseTypeDef

```python
# CalculateIsolinesResponseTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import CalculateIsolinesResponseTypeDef


def get_value() -> CalculateIsolinesResponseTypeDef:
    return {
        "ArrivalTime": ...,
    }


# CalculateIsolinesResponseTypeDef definition

class CalculateIsolinesResponseTypeDef(TypedDict):
    ArrivalTime: str,
    DepartureTime: str,
    IsolineGeometryFormat: GeometryFormatType,  # (1)
    Isolines: List[IsolineTypeDef],  # (2)
    PricingBucket: str,
    SnappedDestination: List[float],
    SnappedOrigin: List[float],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: GeometryFormatType](./literals.md#geometryformattype) 
2. See [:material-code-braces: IsolineTypeDef](./type_defs.md#isolinetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SnapToRoadsRequestTypeDef

```python
# SnapToRoadsRequestTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import SnapToRoadsRequestTypeDef


def get_value() -> SnapToRoadsRequestTypeDef:
    return {
        "TracePoints": ...,
    }


# SnapToRoadsRequestTypeDef definition

class SnapToRoadsRequestTypeDef(TypedDict):
    TracePoints: Sequence[RoadSnapTracePointTypeDef],  # (1)
    Key: NotRequired[str],
    SnappedGeometryFormat: NotRequired[GeometryFormatType],  # (2)
    SnapRadius: NotRequired[int],
    TravelMode: NotRequired[RoadSnapTravelModeType],  # (3)
    TravelModeOptions: NotRequired[RoadSnapTravelModeOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: RoadSnapTracePointTypeDef](./type_defs.md#roadsnaptracepointtypedef) 
2. See [:material-code-brackets: GeometryFormatType](./literals.md#geometryformattype) 
3. See [:material-code-brackets: RoadSnapTravelModeType](./literals.md#roadsnaptravelmodetype) 
4. See [:material-code-braces: RoadSnapTravelModeOptionsTypeDef](./type_defs.md#roadsnaptravelmodeoptionstypedef) 
## RoutePedestrianTravelStepTypeDef

```python
# RoutePedestrianTravelStepTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePedestrianTravelStepTypeDef


def get_value() -> RoutePedestrianTravelStepTypeDef:
    return {
        "ContinueStepDetails": ...,
    }


# RoutePedestrianTravelStepTypeDef definition

class RoutePedestrianTravelStepTypeDef(TypedDict):
    Duration: int,
    Type: RoutePedestrianTravelStepTypeType,  # (11)
    ContinueStepDetails: NotRequired[RouteContinueStepDetailsTypeDef],  # (1)
    CurrentRoad: NotRequired[RouteRoadTypeDef],  # (2)
    Distance: NotRequired[int],
    ExitNumber: NotRequired[List[LocalizedStringTypeDef]],  # (3)
    GeometryOffset: NotRequired[int],
    Instruction: NotRequired[str],
    KeepStepDetails: NotRequired[RouteKeepStepDetailsTypeDef],  # (4)
    NextRoad: NotRequired[RouteRoadTypeDef],  # (2)
    RoundaboutEnterStepDetails: NotRequired[RouteRoundaboutEnterStepDetailsTypeDef],  # (6)
    RoundaboutExitStepDetails: NotRequired[RouteRoundaboutExitStepDetailsTypeDef],  # (7)
    RoundaboutPassStepDetails: NotRequired[RouteRoundaboutPassStepDetailsTypeDef],  # (8)
    Signpost: NotRequired[RouteSignpostTypeDef],  # (9)
    TurnStepDetails: NotRequired[RouteTurnStepDetailsTypeDef],  # (10)
```

1. See [:material-code-braces: RouteContinueStepDetailsTypeDef](./type_defs.md#routecontinuestepdetailstypedef) 
2. See [:material-code-braces: RouteRoadTypeDef](./type_defs.md#routeroadtypedef) 
3. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
4. See [:material-code-braces: RouteKeepStepDetailsTypeDef](./type_defs.md#routekeepstepdetailstypedef) 
5. See [:material-code-braces: RouteRoadTypeDef](./type_defs.md#routeroadtypedef) 
6. See [:material-code-braces: RouteRoundaboutEnterStepDetailsTypeDef](./type_defs.md#routeroundaboutenterstepdetailstypedef) 
7. See [:material-code-braces: RouteRoundaboutExitStepDetailsTypeDef](./type_defs.md#routeroundaboutexitstepdetailstypedef) 
8. See [:material-code-braces: RouteRoundaboutPassStepDetailsTypeDef](./type_defs.md#routeroundaboutpassstepdetailstypedef) 
9. See [:material-code-braces: RouteSignpostTypeDef](./type_defs.md#routesignposttypedef) 
10. See [:material-code-braces: RouteTurnStepDetailsTypeDef](./type_defs.md#routeturnstepdetailstypedef) 
11. See [:material-code-brackets: RoutePedestrianTravelStepTypeType](./literals.md#routepedestriantravelsteptypetype) 
## RouteVehicleTravelStepTypeDef

```python
# RouteVehicleTravelStepTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleTravelStepTypeDef


def get_value() -> RouteVehicleTravelStepTypeDef:
    return {
        "ContinueHighwayStepDetails": ...,
    }


# RouteVehicleTravelStepTypeDef definition

class RouteVehicleTravelStepTypeDef(TypedDict):
    Duration: int,
    Type: RouteVehicleTravelStepTypeType,  # (15)
    ContinueHighwayStepDetails: NotRequired[RouteContinueHighwayStepDetailsTypeDef],  # (1)
    ContinueStepDetails: NotRequired[RouteContinueStepDetailsTypeDef],  # (2)
    CurrentRoad: NotRequired[RouteRoadTypeDef],  # (3)
    Distance: NotRequired[int],
    EnterHighwayStepDetails: NotRequired[RouteEnterHighwayStepDetailsTypeDef],  # (4)
    ExitNumber: NotRequired[List[LocalizedStringTypeDef]],  # (5)
    ExitStepDetails: NotRequired[RouteExitStepDetailsTypeDef],  # (6)
    GeometryOffset: NotRequired[int],
    Instruction: NotRequired[str],
    KeepStepDetails: NotRequired[RouteKeepStepDetailsTypeDef],  # (7)
    NextRoad: NotRequired[RouteRoadTypeDef],  # (3)
    RampStepDetails: NotRequired[RouteRampStepDetailsTypeDef],  # (9)
    RoundaboutEnterStepDetails: NotRequired[RouteRoundaboutEnterStepDetailsTypeDef],  # (10)
    RoundaboutExitStepDetails: NotRequired[RouteRoundaboutExitStepDetailsTypeDef],  # (11)
    RoundaboutPassStepDetails: NotRequired[RouteRoundaboutPassStepDetailsTypeDef],  # (12)
    Signpost: NotRequired[RouteSignpostTypeDef],  # (13)
    TurnStepDetails: NotRequired[RouteTurnStepDetailsTypeDef],  # (14)
    UTurnStepDetails: NotRequired[RouteUTurnStepDetailsTypeDef],  # (16)
```

1. See [:material-code-braces: RouteContinueHighwayStepDetailsTypeDef](./type_defs.md#routecontinuehighwaystepdetailstypedef) 
2. See [:material-code-braces: RouteContinueStepDetailsTypeDef](./type_defs.md#routecontinuestepdetailstypedef) 
3. See [:material-code-braces: RouteRoadTypeDef](./type_defs.md#routeroadtypedef) 
4. See [:material-code-braces: RouteEnterHighwayStepDetailsTypeDef](./type_defs.md#routeenterhighwaystepdetailstypedef) 
5. See [:material-code-braces: LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef) 
6. See [:material-code-braces: RouteExitStepDetailsTypeDef](./type_defs.md#routeexitstepdetailstypedef) 
7. See [:material-code-braces: RouteKeepStepDetailsTypeDef](./type_defs.md#routekeepstepdetailstypedef) 
8. See [:material-code-braces: RouteRoadTypeDef](./type_defs.md#routeroadtypedef) 
9. See [:material-code-braces: RouteRampStepDetailsTypeDef](./type_defs.md#routerampstepdetailstypedef) 
10. See [:material-code-braces: RouteRoundaboutEnterStepDetailsTypeDef](./type_defs.md#routeroundaboutenterstepdetailstypedef) 
11. See [:material-code-braces: RouteRoundaboutExitStepDetailsTypeDef](./type_defs.md#routeroundaboutexitstepdetailstypedef) 
12. See [:material-code-braces: RouteRoundaboutPassStepDetailsTypeDef](./type_defs.md#routeroundaboutpassstepdetailstypedef) 
13. See [:material-code-braces: RouteSignpostTypeDef](./type_defs.md#routesignposttypedef) 
14. See [:material-code-braces: RouteTurnStepDetailsTypeDef](./type_defs.md#routeturnstepdetailstypedef) 
15. See [:material-code-brackets: RouteVehicleTravelStepTypeType](./literals.md#routevehicletravelsteptypetype) 
16. See [:material-code-braces: RouteUTurnStepDetailsTypeDef](./type_defs.md#routeuturnstepdetailstypedef) 
## CalculateRouteMatrixResponseTypeDef

```python
# CalculateRouteMatrixResponseTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import CalculateRouteMatrixResponseTypeDef


def get_value() -> CalculateRouteMatrixResponseTypeDef:
    return {
        "ErrorCount": ...,
    }


# CalculateRouteMatrixResponseTypeDef definition

class CalculateRouteMatrixResponseTypeDef(TypedDict):
    ErrorCount: int,
    PricingBucket: str,
    RouteMatrix: List[List[RouteMatrixEntryTypeDef]],  # (1)
    RoutingBoundary: RouteMatrixBoundaryOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RouteMatrixEntryTypeDef](./type_defs.md#routematrixentrytypedef) 
2. See [:material-code-braces: RouteMatrixBoundaryOutputTypeDef](./type_defs.md#routematrixboundaryoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RouteSummaryTypeDef

```python
# RouteSummaryTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteSummaryTypeDef


def get_value() -> RouteSummaryTypeDef:
    return {
        "Distance": ...,
    }


# RouteSummaryTypeDef definition

class RouteSummaryTypeDef(TypedDict):
    Distance: NotRequired[int],
    Duration: NotRequired[int],
    Tolls: NotRequired[RouteTollSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: RouteTollSummaryTypeDef](./type_defs.md#routetollsummarytypedef) 
## RouteTollTypeDef

```python
# RouteTollTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTollTypeDef


def get_value() -> RouteTollTypeDef:
    return {
        "Country": ...,
    }


# RouteTollTypeDef definition

class RouteTollTypeDef(TypedDict):
    PaymentSites: List[RouteTollPaymentSiteTypeDef],  # (1)
    Rates: List[RouteTollRateTypeDef],  # (2)
    Systems: List[int],
    Country: NotRequired[str],
```

1. See [:material-code-braces: RouteTollPaymentSiteTypeDef](./type_defs.md#routetollpaymentsitetypedef) 
2. See [:material-code-braces: RouteTollRateTypeDef](./type_defs.md#routetollratetypedef) 
## RouteVehicleNoticeTypeDef

```python
# RouteVehicleNoticeTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleNoticeTypeDef


def get_value() -> RouteVehicleNoticeTypeDef:
    return {
        "Code": ...,
    }


# RouteVehicleNoticeTypeDef definition

class RouteVehicleNoticeTypeDef(TypedDict):
    Code: RouteVehicleNoticeCodeType,  # (1)
    Details: List[RouteVehicleNoticeDetailTypeDef],  # (2)
    Impact: NotRequired[RouteNoticeImpactType],  # (3)
```

1. See [:material-code-brackets: RouteVehicleNoticeCodeType](./literals.md#routevehiclenoticecodetype) 
2. See [:material-code-braces: RouteVehicleNoticeDetailTypeDef](./type_defs.md#routevehiclenoticedetailtypedef) 
3. See [:material-code-brackets: RouteNoticeImpactType](./literals.md#routenoticeimpacttype) 
## OptimizeWaypointsRequestTypeDef

```python
# OptimizeWaypointsRequestTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import OptimizeWaypointsRequestTypeDef


def get_value() -> OptimizeWaypointsRequestTypeDef:
    return {
        "Origin": ...,
    }


# OptimizeWaypointsRequestTypeDef definition

class OptimizeWaypointsRequestTypeDef(TypedDict):
    Origin: Sequence[float],
    Avoid: NotRequired[WaypointOptimizationAvoidanceOptionsTypeDef],  # (1)
    Clustering: NotRequired[WaypointOptimizationClusteringOptionsTypeDef],  # (2)
    DepartureTime: NotRequired[str],
    Destination: NotRequired[Sequence[float]],
    DestinationOptions: NotRequired[WaypointOptimizationDestinationOptionsTypeDef],  # (3)
    Driver: NotRequired[WaypointOptimizationDriverOptionsTypeDef],  # (4)
    Exclude: NotRequired[WaypointOptimizationExclusionOptionsTypeDef],  # (5)
    Key: NotRequired[str],
    OptimizeSequencingFor: NotRequired[WaypointOptimizationSequencingObjectiveType],  # (6)
    OriginOptions: NotRequired[WaypointOptimizationOriginOptionsTypeDef],  # (7)
    Traffic: NotRequired[WaypointOptimizationTrafficOptionsTypeDef],  # (8)
    TravelMode: NotRequired[WaypointOptimizationTravelModeType],  # (9)
    TravelModeOptions: NotRequired[WaypointOptimizationTravelModeOptionsTypeDef],  # (10)
    Waypoints: NotRequired[Sequence[WaypointOptimizationWaypointTypeDef]],  # (11)
```

1. See [:material-code-braces: WaypointOptimizationAvoidanceOptionsTypeDef](./type_defs.md#waypointoptimizationavoidanceoptionstypedef) 
2. See [:material-code-braces: WaypointOptimizationClusteringOptionsTypeDef](./type_defs.md#waypointoptimizationclusteringoptionstypedef) 
3. See [:material-code-braces: WaypointOptimizationDestinationOptionsTypeDef](./type_defs.md#waypointoptimizationdestinationoptionstypedef) 
4. See [:material-code-braces: WaypointOptimizationDriverOptionsTypeDef](./type_defs.md#waypointoptimizationdriveroptionstypedef) 
5. See [:material-code-braces: WaypointOptimizationExclusionOptionsTypeDef](./type_defs.md#waypointoptimizationexclusionoptionstypedef) 
6. See [:material-code-brackets: WaypointOptimizationSequencingObjectiveType](./literals.md#waypointoptimizationsequencingobjectivetype) 
7. See [:material-code-braces: WaypointOptimizationOriginOptionsTypeDef](./type_defs.md#waypointoptimizationoriginoptionstypedef) 
8. See [:material-code-braces: WaypointOptimizationTrafficOptionsTypeDef](./type_defs.md#waypointoptimizationtrafficoptionstypedef) 
9. See [:material-code-brackets: WaypointOptimizationTravelModeType](./literals.md#waypointoptimizationtravelmodetype) 
10. See [:material-code-braces: WaypointOptimizationTravelModeOptionsTypeDef](./type_defs.md#waypointoptimizationtravelmodeoptionstypedef) 
11. See [:material-code-braces: WaypointOptimizationWaypointTypeDef](./type_defs.md#waypointoptimizationwaypointtypedef) 
## CalculateIsolinesRequestTypeDef

```python
# CalculateIsolinesRequestTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import CalculateIsolinesRequestTypeDef


def get_value() -> CalculateIsolinesRequestTypeDef:
    return {
        "Thresholds": ...,
    }


# CalculateIsolinesRequestTypeDef definition

class CalculateIsolinesRequestTypeDef(TypedDict):
    Thresholds: IsolineThresholdsTypeDef,  # (1)
    Allow: NotRequired[IsolineAllowOptionsTypeDef],  # (2)
    ArrivalTime: NotRequired[str],
    Avoid: NotRequired[IsolineAvoidanceOptionsTypeDef],  # (3)
    DepartNow: NotRequired[bool],
    DepartureTime: NotRequired[str],
    Destination: NotRequired[Sequence[float]],
    DestinationOptions: NotRequired[IsolineDestinationOptionsTypeDef],  # (4)
    IsolineGeometryFormat: NotRequired[GeometryFormatType],  # (5)
    IsolineGranularity: NotRequired[IsolineGranularityOptionsTypeDef],  # (6)
    Key: NotRequired[str],
    OptimizeIsolineFor: NotRequired[IsolineOptimizationObjectiveType],  # (7)
    OptimizeRoutingFor: NotRequired[RoutingObjectiveType],  # (8)
    Origin: NotRequired[Sequence[float]],
    OriginOptions: NotRequired[IsolineOriginOptionsTypeDef],  # (9)
    Traffic: NotRequired[IsolineTrafficOptionsTypeDef],  # (10)
    TravelMode: NotRequired[IsolineTravelModeType],  # (11)
    TravelModeOptions: NotRequired[IsolineTravelModeOptionsTypeDef],  # (12)
```

1. See [:material-code-braces: IsolineThresholdsTypeDef](./type_defs.md#isolinethresholdstypedef) 
2. See [:material-code-braces: IsolineAllowOptionsTypeDef](./type_defs.md#isolineallowoptionstypedef) 
3. See [:material-code-braces: IsolineAvoidanceOptionsTypeDef](./type_defs.md#isolineavoidanceoptionstypedef) 
4. See [:material-code-braces: IsolineDestinationOptionsTypeDef](./type_defs.md#isolinedestinationoptionstypedef) 
5. See [:material-code-brackets: GeometryFormatType](./literals.md#geometryformattype) 
6. See [:material-code-braces: IsolineGranularityOptionsTypeDef](./type_defs.md#isolinegranularityoptionstypedef) 
7. See [:material-code-brackets: IsolineOptimizationObjectiveType](./literals.md#isolineoptimizationobjectivetype) 
8. See [:material-code-brackets: RoutingObjectiveType](./literals.md#routingobjectivetype) 
9. See [:material-code-braces: IsolineOriginOptionsTypeDef](./type_defs.md#isolineoriginoptionstypedef) 
10. See [:material-code-braces: IsolineTrafficOptionsTypeDef](./type_defs.md#isolinetrafficoptionstypedef) 
11. See [:material-code-brackets: IsolineTravelModeType](./literals.md#isolinetravelmodetype) 
12. See [:material-code-braces: IsolineTravelModeOptionsTypeDef](./type_defs.md#isolinetravelmodeoptionstypedef) 
## CalculateRoutesRequestTypeDef

```python
# CalculateRoutesRequestTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import CalculateRoutesRequestTypeDef


def get_value() -> CalculateRoutesRequestTypeDef:
    return {
        "Destination": ...,
    }


# CalculateRoutesRequestTypeDef definition

class CalculateRoutesRequestTypeDef(TypedDict):
    Destination: Sequence[float],
    Origin: Sequence[float],
    Allow: NotRequired[RouteAllowOptionsTypeDef],  # (1)
    ArrivalTime: NotRequired[str],
    Avoid: NotRequired[RouteAvoidanceOptionsTypeDef],  # (2)
    DepartNow: NotRequired[bool],
    DepartureTime: NotRequired[str],
    DestinationOptions: NotRequired[RouteDestinationOptionsTypeDef],  # (3)
    Driver: NotRequired[RouteDriverOptionsTypeDef],  # (4)
    Exclude: NotRequired[RouteExclusionOptionsTypeDef],  # (5)
    InstructionsMeasurementSystem: NotRequired[MeasurementSystemType],  # (6)
    Key: NotRequired[str],
    Languages: NotRequired[Sequence[str]],
    LegAdditionalFeatures: NotRequired[Sequence[RouteLegAdditionalFeatureType]],  # (7)
    LegGeometryFormat: NotRequired[GeometryFormatType],  # (8)
    MaxAlternatives: NotRequired[int],
    OptimizeRoutingFor: NotRequired[RoutingObjectiveType],  # (9)
    OriginOptions: NotRequired[RouteOriginOptionsTypeDef],  # (10)
    SpanAdditionalFeatures: NotRequired[Sequence[RouteSpanAdditionalFeatureType]],  # (11)
    Tolls: NotRequired[RouteTollOptionsTypeDef],  # (12)
    Traffic: NotRequired[RouteTrafficOptionsTypeDef],  # (13)
    TravelMode: NotRequired[RouteTravelModeType],  # (14)
    TravelModeOptions: NotRequired[RouteTravelModeOptionsTypeDef],  # (15)
    TravelStepType: NotRequired[RouteTravelStepTypeType],  # (16)
    Waypoints: NotRequired[Sequence[RouteWaypointTypeDef]],  # (17)
```

1. See [:material-code-braces: RouteAllowOptionsTypeDef](./type_defs.md#routeallowoptionstypedef) 
2. See [:material-code-braces: RouteAvoidanceOptionsTypeDef](./type_defs.md#routeavoidanceoptionstypedef) 
3. See [:material-code-braces: RouteDestinationOptionsTypeDef](./type_defs.md#routedestinationoptionstypedef) 
4. See [:material-code-braces: RouteDriverOptionsTypeDef](./type_defs.md#routedriveroptionstypedef) 
5. See [:material-code-braces: RouteExclusionOptionsTypeDef](./type_defs.md#routeexclusionoptionstypedef) 
6. See [:material-code-brackets: MeasurementSystemType](./literals.md#measurementsystemtype) 
7. See [:material-code-brackets: RouteLegAdditionalFeatureType](./literals.md#routelegadditionalfeaturetype) 
8. See [:material-code-brackets: GeometryFormatType](./literals.md#geometryformattype) 
9. See [:material-code-brackets: RoutingObjectiveType](./literals.md#routingobjectivetype) 
10. See [:material-code-braces: RouteOriginOptionsTypeDef](./type_defs.md#routeoriginoptionstypedef) 
11. See [:material-code-brackets: RouteSpanAdditionalFeatureType](./literals.md#routespanadditionalfeaturetype) 
12. See [:material-code-braces: RouteTollOptionsTypeDef](./type_defs.md#routetolloptionstypedef) 
13. See [:material-code-braces: RouteTrafficOptionsTypeDef](./type_defs.md#routetrafficoptionstypedef) 
14. See [:material-code-brackets: RouteTravelModeType](./literals.md#routetravelmodetype) 
15. See [:material-code-braces: RouteTravelModeOptionsTypeDef](./type_defs.md#routetravelmodeoptionstypedef) 
16. See [:material-code-brackets: RouteTravelStepTypeType](./literals.md#routetravelsteptypetype) 
17. See [:material-code-braces: RouteWaypointTypeDef](./type_defs.md#routewaypointtypedef) 
## RoutePedestrianLegDetailsTypeDef

```python
# RoutePedestrianLegDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RoutePedestrianLegDetailsTypeDef


def get_value() -> RoutePedestrianLegDetailsTypeDef:
    return {
        "Arrival": ...,
    }


# RoutePedestrianLegDetailsTypeDef definition

class RoutePedestrianLegDetailsTypeDef(TypedDict):
    Arrival: RoutePedestrianArrivalTypeDef,  # (1)
    Departure: RoutePedestrianDepartureTypeDef,  # (2)
    Notices: List[RoutePedestrianNoticeTypeDef],  # (3)
    PassThroughWaypoints: List[RoutePassThroughWaypointTypeDef],  # (4)
    Spans: List[RoutePedestrianSpanTypeDef],  # (5)
    TravelSteps: List[RoutePedestrianTravelStepTypeDef],  # (7)
    Summary: NotRequired[RoutePedestrianSummaryTypeDef],  # (6)
```

1. See [:material-code-braces: RoutePedestrianArrivalTypeDef](./type_defs.md#routepedestrianarrivaltypedef) 
2. See [:material-code-braces: RoutePedestrianDepartureTypeDef](./type_defs.md#routepedestriandeparturetypedef) 
3. See [:material-code-braces: RoutePedestrianNoticeTypeDef](./type_defs.md#routepedestriannoticetypedef) 
4. See [:material-code-braces: RoutePassThroughWaypointTypeDef](./type_defs.md#routepassthroughwaypointtypedef) 
5. See [:material-code-braces: RoutePedestrianSpanTypeDef](./type_defs.md#routepedestrianspantypedef) 
6. See [:material-code-braces: RoutePedestrianSummaryTypeDef](./type_defs.md#routepedestriansummarytypedef) 
7. See [:material-code-braces: RoutePedestrianTravelStepTypeDef](./type_defs.md#routepedestriantravelsteptypedef) 
## CalculateRouteMatrixRequestTypeDef

```python
# CalculateRouteMatrixRequestTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import CalculateRouteMatrixRequestTypeDef


def get_value() -> CalculateRouteMatrixRequestTypeDef:
    return {
        "Destinations": ...,
    }


# CalculateRouteMatrixRequestTypeDef definition

class CalculateRouteMatrixRequestTypeDef(TypedDict):
    Destinations: Sequence[RouteMatrixDestinationTypeDef],  # (1)
    Origins: Sequence[RouteMatrixOriginTypeDef],  # (2)
    RoutingBoundary: RouteMatrixBoundaryUnionTypeDef,  # (3)
    Allow: NotRequired[RouteMatrixAllowOptionsTypeDef],  # (4)
    Avoid: NotRequired[RouteMatrixAvoidanceOptionsTypeDef],  # (5)
    DepartNow: NotRequired[bool],
    DepartureTime: NotRequired[str],
    Exclude: NotRequired[RouteMatrixExclusionOptionsTypeDef],  # (6)
    Key: NotRequired[str],
    OptimizeRoutingFor: NotRequired[RoutingObjectiveType],  # (7)
    Traffic: NotRequired[RouteMatrixTrafficOptionsTypeDef],  # (8)
    TravelMode: NotRequired[RouteMatrixTravelModeType],  # (9)
    TravelModeOptions: NotRequired[RouteMatrixTravelModeOptionsTypeDef],  # (10)
```

1. See [:material-code-braces: RouteMatrixDestinationTypeDef](./type_defs.md#routematrixdestinationtypedef) 
2. See [:material-code-braces: RouteMatrixOriginTypeDef](./type_defs.md#routematrixorigintypedef) 
3. See [:material-code-braces: RouteMatrixBoundaryTypeDef](./type_defs.md#routematrixboundarytypedef) [:material-code-braces: RouteMatrixBoundaryOutputTypeDef](./type_defs.md#routematrixboundaryoutputtypedef) 
4. See [:material-code-braces: RouteMatrixAllowOptionsTypeDef](./type_defs.md#routematrixallowoptionstypedef) 
5. See [:material-code-braces: RouteMatrixAvoidanceOptionsTypeDef](./type_defs.md#routematrixavoidanceoptionstypedef) 
6. See [:material-code-braces: RouteMatrixExclusionOptionsTypeDef](./type_defs.md#routematrixexclusionoptionstypedef) 
7. See [:material-code-brackets: RoutingObjectiveType](./literals.md#routingobjectivetype) 
8. See [:material-code-braces: RouteMatrixTrafficOptionsTypeDef](./type_defs.md#routematrixtrafficoptionstypedef) 
9. See [:material-code-brackets: RouteMatrixTravelModeType](./literals.md#routematrixtravelmodetype) 
10. See [:material-code-braces: RouteMatrixTravelModeOptionsTypeDef](./type_defs.md#routematrixtravelmodeoptionstypedef) 
## RouteVehicleLegDetailsTypeDef

```python
# RouteVehicleLegDetailsTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteVehicleLegDetailsTypeDef


def get_value() -> RouteVehicleLegDetailsTypeDef:
    return {
        "Arrival": ...,
    }


# RouteVehicleLegDetailsTypeDef definition

class RouteVehicleLegDetailsTypeDef(TypedDict):
    Arrival: RouteVehicleArrivalTypeDef,  # (1)
    Departure: RouteVehicleDepartureTypeDef,  # (2)
    Incidents: List[RouteVehicleIncidentTypeDef],  # (3)
    Notices: List[RouteVehicleNoticeTypeDef],  # (4)
    PassThroughWaypoints: List[RoutePassThroughWaypointTypeDef],  # (5)
    Spans: List[RouteVehicleSpanTypeDef],  # (6)
    Tolls: List[RouteTollTypeDef],  # (8)
    TollSystems: List[RouteTollSystemTypeDef],  # (9)
    TravelSteps: List[RouteVehicleTravelStepTypeDef],  # (10)
    TruckRoadTypes: List[str],
    Zones: List[RouteZoneTypeDef],  # (11)
    Summary: NotRequired[RouteVehicleSummaryTypeDef],  # (7)
```

1. See [:material-code-braces: RouteVehicleArrivalTypeDef](./type_defs.md#routevehiclearrivaltypedef) 
2. See [:material-code-braces: RouteVehicleDepartureTypeDef](./type_defs.md#routevehicledeparturetypedef) 
3. See [:material-code-braces: RouteVehicleIncidentTypeDef](./type_defs.md#routevehicleincidenttypedef) 
4. See [:material-code-braces: RouteVehicleNoticeTypeDef](./type_defs.md#routevehiclenoticetypedef) 
5. See [:material-code-braces: RoutePassThroughWaypointTypeDef](./type_defs.md#routepassthroughwaypointtypedef) 
6. See [:material-code-braces: RouteVehicleSpanTypeDef](./type_defs.md#routevehiclespantypedef) 
7. See [:material-code-braces: RouteVehicleSummaryTypeDef](./type_defs.md#routevehiclesummarytypedef) 
8. See [:material-code-braces: RouteTollTypeDef](./type_defs.md#routetolltypedef) 
9. See [:material-code-braces: RouteTollSystemTypeDef](./type_defs.md#routetollsystemtypedef) 
10. See [:material-code-braces: RouteVehicleTravelStepTypeDef](./type_defs.md#routevehicletravelsteptypedef) 
11. See [:material-code-braces: RouteZoneTypeDef](./type_defs.md#routezonetypedef) 
## RouteLegTypeDef

```python
# RouteLegTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteLegTypeDef


def get_value() -> RouteLegTypeDef:
    return {
        "FerryLegDetails": ...,
    }


# RouteLegTypeDef definition

class RouteLegTypeDef(TypedDict):
    Geometry: RouteLegGeometryTypeDef,  # (2)
    TravelMode: RouteLegTravelModeType,  # (4)
    Type: RouteLegTypeType,  # (5)
    FerryLegDetails: NotRequired[RouteFerryLegDetailsTypeDef],  # (1)
    Language: NotRequired[str],
    PedestrianLegDetails: NotRequired[RoutePedestrianLegDetailsTypeDef],  # (3)
    VehicleLegDetails: NotRequired[RouteVehicleLegDetailsTypeDef],  # (6)
```

1. See [:material-code-braces: RouteFerryLegDetailsTypeDef](./type_defs.md#routeferrylegdetailstypedef) 
2. See [:material-code-braces: RouteLegGeometryTypeDef](./type_defs.md#routeleggeometrytypedef) 
3. See [:material-code-braces: RoutePedestrianLegDetailsTypeDef](./type_defs.md#routepedestrianlegdetailstypedef) 
4. See [:material-code-brackets: RouteLegTravelModeType](./literals.md#routelegtravelmodetype) 
5. See [:material-code-brackets: RouteLegTypeType](./literals.md#routelegtypetype) 
6. See [:material-code-braces: RouteVehicleLegDetailsTypeDef](./type_defs.md#routevehiclelegdetailstypedef) 
## RouteTypeDef

```python
# RouteTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import RouteTypeDef


def get_value() -> RouteTypeDef:
    return {
        "Legs": ...,
    }


# RouteTypeDef definition

class RouteTypeDef(TypedDict):
    Legs: List[RouteLegTypeDef],  # (1)
    MajorRoadLabels: List[RouteMajorRoadLabelTypeDef],  # (2)
    Summary: NotRequired[RouteSummaryTypeDef],  # (3)
```

1. See [:material-code-braces: RouteLegTypeDef](./type_defs.md#routelegtypedef) 
2. See [:material-code-braces: RouteMajorRoadLabelTypeDef](./type_defs.md#routemajorroadlabeltypedef) 
3. See [:material-code-braces: RouteSummaryTypeDef](./type_defs.md#routesummarytypedef) 
## CalculateRoutesResponseTypeDef

```python
# CalculateRoutesResponseTypeDef TypedDict usage example

from types_aiobotocore_geo_routes.type_defs import CalculateRoutesResponseTypeDef


def get_value() -> CalculateRoutesResponseTypeDef:
    return {
        "LegGeometryFormat": ...,
    }


# CalculateRoutesResponseTypeDef definition

class CalculateRoutesResponseTypeDef(TypedDict):
    LegGeometryFormat: GeometryFormatType,  # (1)
    Notices: List[RouteResponseNoticeTypeDef],  # (2)
    PricingBucket: str,
    Routes: List[RouteTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: GeometryFormatType](./literals.md#geometryformattype) 
2. See [:material-code-braces: RouteResponseNoticeTypeDef](./type_defs.md#routeresponsenoticetypedef) 
3. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
