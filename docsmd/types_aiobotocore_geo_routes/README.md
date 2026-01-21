# LocationServiceRoutesV2 module

> [Index](../README.md) > LocationServiceRoutesV2


!!! note ""

    Auto-generated documentation for [LocationServiceRoutesV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-routes.html#locationserviceroutesv2)
    type annotations stubs module [types-aiobotocore-geo-routes](https://pypi.org/project/types-aiobotocore-geo-routes/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `LocationServiceRoutesV2` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `LocationServiceRoutesV2` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[geo-routes]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[geo-routes]'

# standalone installation
python -m pip install types-aiobotocore-geo-routes
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-geo-routes
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LocationServiceRoutesV2Client

Type annotations and code completion for  `#!python session.create_client("geo-routes")` as [LocationServiceRoutesV2Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-routes.html#LocationServiceRoutesV2.Client)

```python
# LocationServiceRoutesV2Client usage example

from aiobotocore.session import get_session

from types_aiobotocore_geo_routes.client import LocationServiceRoutesV2Client


session = get_session()
async with session.create_client("geo-routes") as client:
    client: LocationServiceRoutesV2Client
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DayOfWeekType usage example

from types_aiobotocore_geo_routes.literals import DayOfWeekType

def get_value() -> DayOfWeekType:
    return "Friday"
```

- [DayOfWeekType](./literals.md#dayofweektype)
- [GeometryFormatType](./literals.md#geometryformattype)
- [IsolineEngineTypeType](./literals.md#isolineenginetypetype)
- [IsolineHazardousCargoTypeType](./literals.md#isolinehazardouscargotypetype)
- [IsolineOptimizationObjectiveType](./literals.md#isolineoptimizationobjectivetype)
- [IsolineTravelModeType](./literals.md#isolinetravelmodetype)
- [IsolineTruckTypeType](./literals.md#isolinetrucktypetype)
- [IsolineZoneCategoryType](./literals.md#isolinezonecategorytype)
- [MatchingStrategyType](./literals.md#matchingstrategytype)
- [MeasurementSystemType](./literals.md#measurementsystemtype)
- [RoadSnapHazardousCargoTypeType](./literals.md#roadsnaphazardouscargotypetype)
- [RoadSnapNoticeCodeType](./literals.md#roadsnapnoticecodetype)
- [RoadSnapTravelModeType](./literals.md#roadsnaptravelmodetype)
- [RouteDirectionType](./literals.md#routedirectiontype)
- [RouteEngineTypeType](./literals.md#routeenginetypetype)
- [RouteFerryAfterTravelStepTypeType](./literals.md#routeferryaftertravelsteptypetype)
- [RouteFerryBeforeTravelStepTypeType](./literals.md#routeferrybeforetravelsteptypetype)
- [RouteFerryNoticeCodeType](./literals.md#routeferrynoticecodetype)
- [RouteFerryTravelStepTypeType](./literals.md#routeferrytravelsteptypetype)
- [RouteHazardousCargoTypeType](./literals.md#routehazardouscargotypetype)
- [RouteLegAdditionalFeatureType](./literals.md#routelegadditionalfeaturetype)
- [RouteLegTravelModeType](./literals.md#routelegtravelmodetype)
- [RouteLegTypeType](./literals.md#routelegtypetype)
- [RouteMatrixErrorCodeType](./literals.md#routematrixerrorcodetype)
- [RouteMatrixHazardousCargoTypeType](./literals.md#routematrixhazardouscargotypetype)
- [RouteMatrixTravelModeType](./literals.md#routematrixtravelmodetype)
- [RouteMatrixTruckTypeType](./literals.md#routematrixtrucktypetype)
- [RouteMatrixZoneCategoryType](./literals.md#routematrixzonecategorytype)
- [RouteNoticeImpactType](./literals.md#routenoticeimpacttype)
- [RoutePedestrianNoticeCodeType](./literals.md#routepedestriannoticecodetype)
- [RoutePedestrianTravelStepTypeType](./literals.md#routepedestriantravelsteptypetype)
- [RouteResponseNoticeCodeType](./literals.md#routeresponsenoticecodetype)
- [RouteRoadTypeType](./literals.md#routeroadtypetype)
- [RouteSideOfStreetType](./literals.md#routesideofstreettype)
- [RouteSpanAdditionalFeatureType](./literals.md#routespanadditionalfeaturetype)
- [RouteSpanCarAccessAttributeType](./literals.md#routespancaraccessattributetype)
- [RouteSpanGateAttributeType](./literals.md#routespangateattributetype)
- [RouteSpanPedestrianAccessAttributeType](./literals.md#routespanpedestrianaccessattributetype)
- [RouteSpanRailwayCrossingAttributeType](./literals.md#routespanrailwaycrossingattributetype)
- [RouteSpanRoadAttributeType](./literals.md#routespanroadattributetype)
- [RouteSpanScooterAccessAttributeType](./literals.md#routespanscooteraccessattributetype)
- [RouteSpanTruckAccessAttributeType](./literals.md#routespantruckaccessattributetype)
- [RouteSteeringDirectionType](./literals.md#routesteeringdirectiontype)
- [RouteTollPassValidityPeriodTypeType](./literals.md#routetollpassvalidityperiodtypetype)
- [RouteTollPaymentMethodType](./literals.md#routetollpaymentmethodtype)
- [RouteTollVehicleCategoryType](./literals.md#routetollvehiclecategorytype)
- [RouteTravelModeType](./literals.md#routetravelmodetype)
- [RouteTravelStepTypeType](./literals.md#routetravelsteptypetype)
- [RouteTruckTypeType](./literals.md#routetrucktypetype)
- [RouteTurnIntensityType](./literals.md#routeturnintensitytype)
- [RouteVehicleIncidentSeverityType](./literals.md#routevehicleincidentseveritytype)
- [RouteVehicleIncidentTypeType](./literals.md#routevehicleincidenttypetype)
- [RouteVehicleNoticeCodeType](./literals.md#routevehiclenoticecodetype)
- [RouteVehicleTravelStepTypeType](./literals.md#routevehicletravelsteptypetype)
- [RouteWeightConstraintTypeType](./literals.md#routeweightconstrainttypetype)
- [RouteZoneCategoryType](./literals.md#routezonecategorytype)
- [RoutingObjectiveType](./literals.md#routingobjectivetype)
- [SideOfStreetMatchingStrategyType](./literals.md#sideofstreetmatchingstrategytype)
- [TrafficUsageType](./literals.md#trafficusagetype)
- [WaypointOptimizationClusteringAlgorithmType](./literals.md#waypointoptimizationclusteringalgorithmtype)
- [WaypointOptimizationConstraintType](./literals.md#waypointoptimizationconstrainttype)
- [WaypointOptimizationHazardousCargoTypeType](./literals.md#waypointoptimizationhazardouscargotypetype)
- [WaypointOptimizationSequencingObjectiveType](./literals.md#waypointoptimizationsequencingobjectivetype)
- [WaypointOptimizationServiceTimeTreatmentType](./literals.md#waypointoptimizationservicetimetreatmenttype)
- [WaypointOptimizationTravelModeType](./literals.md#waypointoptimizationtravelmodetype)
- [WaypointOptimizationTruckTypeType](./literals.md#waypointoptimizationtrucktypetype)
- [LocationServiceRoutesV2ServiceName](./literals.md#locationserviceroutesv2servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [IsolineAllowOptionsTypeDef](./type_defs.md#isolineallowoptionstypedef)
- [IsolineGranularityOptionsTypeDef](./type_defs.md#isolinegranularityoptionstypedef)
- [IsolineThresholdsTypeDef](./type_defs.md#isolinethresholdstypedef)
- [IsolineTrafficOptionsTypeDef](./type_defs.md#isolinetrafficoptionstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [RouteMatrixAllowOptionsTypeDef](./type_defs.md#routematrixallowoptionstypedef)
- [RouteMatrixExclusionOptionsTypeDef](./type_defs.md#routematrixexclusionoptionstypedef)
- [RouteMatrixTrafficOptionsTypeDef](./type_defs.md#routematrixtrafficoptionstypedef)
- [RouteMatrixEntryTypeDef](./type_defs.md#routematrixentrytypedef)
- [RouteAllowOptionsTypeDef](./type_defs.md#routeallowoptionstypedef)
- [RouteExclusionOptionsTypeDef](./type_defs.md#routeexclusionoptionstypedef)
- [RouteTrafficOptionsTypeDef](./type_defs.md#routetrafficoptionstypedef)
- [RouteResponseNoticeTypeDef](./type_defs.md#routeresponsenoticetypedef)
- [CircleOutputTypeDef](./type_defs.md#circleoutputtypedef)
- [CircleTypeDef](./type_defs.md#circletypedef)
- [CorridorTypeDef](./type_defs.md#corridortypedef)
- [PolylineCorridorTypeDef](./type_defs.md#polylinecorridortypedef)
- [IsolineAvoidanceZoneCategoryTypeDef](./type_defs.md#isolineavoidancezonecategorytypedef)
- [IsolineVehicleLicensePlateTypeDef](./type_defs.md#isolinevehiclelicenseplatetypedef)
- [IsolineConnectionGeometryTypeDef](./type_defs.md#isolineconnectiongeometrytypedef)
- [IsolineMatchingOptionsTypeDef](./type_defs.md#isolinematchingoptionstypedef)
- [IsolineSideOfStreetOptionsTypeDef](./type_defs.md#isolinesideofstreetoptionstypedef)
- [IsolineShapeGeometryTypeDef](./type_defs.md#isolineshapegeometrytypedef)
- [IsolineTrailerOptionsTypeDef](./type_defs.md#isolinetraileroptionstypedef)
- [WeightPerAxleGroupTypeDef](./type_defs.md#weightperaxlegrouptypedef)
- [LocalizedStringTypeDef](./type_defs.md#localizedstringtypedef)
- [WaypointOptimizationExclusionOptionsTypeDef](./type_defs.md#waypointoptimizationexclusionoptionstypedef)
- [WaypointOptimizationOriginOptionsTypeDef](./type_defs.md#waypointoptimizationoriginoptionstypedef)
- [WaypointOptimizationTrafficOptionsTypeDef](./type_defs.md#waypointoptimizationtrafficoptionstypedef)
- [WaypointOptimizationConnectionTypeDef](./type_defs.md#waypointoptimizationconnectiontypedef)
- [WaypointOptimizationOptimizedWaypointTypeDef](./type_defs.md#waypointoptimizationoptimizedwaypointtypedef)
- [WaypointOptimizationTimeBreakdownTypeDef](./type_defs.md#waypointoptimizationtimebreakdowntypedef)
- [RoadSnapNoticeTypeDef](./type_defs.md#roadsnapnoticetypedef)
- [RoadSnapSnappedGeometryTypeDef](./type_defs.md#roadsnapsnappedgeometrytypedef)
- [RoadSnapSnappedTracePointTypeDef](./type_defs.md#roadsnapsnappedtracepointtypedef)
- [RoadSnapTracePointTypeDef](./type_defs.md#roadsnaptracepointtypedef)
- [RoadSnapTrailerOptionsTypeDef](./type_defs.md#roadsnaptraileroptionstypedef)
- [RouteAvoidanceZoneCategoryTypeDef](./type_defs.md#routeavoidancezonecategorytypedef)
- [RouteVehicleLicensePlateTypeDef](./type_defs.md#routevehiclelicenseplatetypedef)
- [RouteMatchingOptionsTypeDef](./type_defs.md#routematchingoptionstypedef)
- [RouteSideOfStreetOptionsTypeDef](./type_defs.md#routesideofstreetoptionstypedef)
- [RouteDriverScheduleIntervalTypeDef](./type_defs.md#routedriverscheduleintervaltypedef)
- [RouteEmissionTypeTypeDef](./type_defs.md#routeemissiontypetypedef)
- [RouteFerryAfterTravelStepTypeDef](./type_defs.md#routeferryaftertravelsteptypedef)
- [RouteFerryPlaceTypeDef](./type_defs.md#routeferryplacetypedef)
- [RouteFerryBeforeTravelStepTypeDef](./type_defs.md#routeferrybeforetravelsteptypedef)
- [RouteFerryNoticeTypeDef](./type_defs.md#routeferrynoticetypedef)
- [RouteFerryTravelStepTypeDef](./type_defs.md#routeferrytravelsteptypedef)
- [RouteFerryOverviewSummaryTypeDef](./type_defs.md#routeferryoverviewsummarytypedef)
- [RouteFerryTravelOnlySummaryTypeDef](./type_defs.md#routeferrytravelonlysummarytypedef)
- [RouteLegGeometryTypeDef](./type_defs.md#routeleggeometrytypedef)
- [RouteNumberTypeDef](./type_defs.md#routenumbertypedef)
- [RouteMatrixAutoCircleTypeDef](./type_defs.md#routematrixautocircletypedef)
- [RouteMatrixAvoidanceAreaGeometryTypeDef](./type_defs.md#routematrixavoidanceareageometrytypedef)
- [RouteMatrixAvoidanceZoneCategoryTypeDef](./type_defs.md#routematrixavoidancezonecategorytypedef)
- [RouteMatrixVehicleLicensePlateTypeDef](./type_defs.md#routematrixvehiclelicenseplatetypedef)
- [RouteMatrixMatchingOptionsTypeDef](./type_defs.md#routematrixmatchingoptionstypedef)
- [RouteMatrixSideOfStreetOptionsTypeDef](./type_defs.md#routematrixsideofstreetoptionstypedef)
- [RouteMatrixTrailerOptionsTypeDef](./type_defs.md#routematrixtraileroptionstypedef)
- [RouteNoticeDetailRangeTypeDef](./type_defs.md#routenoticedetailrangetypedef)
- [RoutePassThroughPlaceTypeDef](./type_defs.md#routepassthroughplacetypedef)
- [RoutePedestrianPlaceTypeDef](./type_defs.md#routepedestrianplacetypedef)
- [RoutePedestrianNoticeTypeDef](./type_defs.md#routepedestriannoticetypedef)
- [RoutePedestrianOptionsTypeDef](./type_defs.md#routepedestrianoptionstypedef)
- [RoutePedestrianOverviewSummaryTypeDef](./type_defs.md#routepedestrianoverviewsummarytypedef)
- [RouteSpanDynamicSpeedDetailsTypeDef](./type_defs.md#routespandynamicspeeddetailstypedef)
- [RouteSpanSpeedLimitDetailsTypeDef](./type_defs.md#routespanspeedlimitdetailstypedef)
- [RoutePedestrianTravelOnlySummaryTypeDef](./type_defs.md#routepedestriantravelonlysummarytypedef)
- [RouteTollPassValidityPeriodTypeDef](./type_defs.md#routetollpassvalidityperiodtypedef)
- [RouteTollPaymentSiteTypeDef](./type_defs.md#routetollpaymentsitetypedef)
- [RouteTollPriceValueRangeTypeDef](./type_defs.md#routetollpricevaluerangetypedef)
- [RouteTransponderTypeDef](./type_defs.md#routetranspondertypedef)
- [RouteTollSystemTypeDef](./type_defs.md#routetollsystemtypedef)
- [RouteTrailerOptionsTypeDef](./type_defs.md#routetraileroptionstypedef)
- [RouteVehiclePlaceTypeDef](./type_defs.md#routevehicleplacetypedef)
- [RouteVehicleIncidentTypeDef](./type_defs.md#routevehicleincidenttypedef)
- [RouteZoneTypeDef](./type_defs.md#routezonetypedef)
- [RouteVehicleOverviewSummaryTypeDef](./type_defs.md#routevehicleoverviewsummarytypedef)
- [RouteVehicleTravelOnlySummaryTypeDef](./type_defs.md#routevehicletravelonlysummarytypedef)
- [RouteWeightConstraintTypeDef](./type_defs.md#routeweightconstrainttypedef)
- [WaypointOptimizationAccessHoursEntryTypeDef](./type_defs.md#waypointoptimizationaccesshoursentrytypedef)
- [WaypointOptimizationAvoidanceAreaGeometryTypeDef](./type_defs.md#waypointoptimizationavoidanceareageometrytypedef)
- [WaypointOptimizationDrivingDistanceOptionsTypeDef](./type_defs.md#waypointoptimizationdrivingdistanceoptionstypedef)
- [WaypointOptimizationSideOfStreetOptionsTypeDef](./type_defs.md#waypointoptimizationsideofstreetoptionstypedef)
- [WaypointOptimizationRestProfileTypeDef](./type_defs.md#waypointoptimizationrestprofiletypedef)
- [WaypointOptimizationFailedConstraintTypeDef](./type_defs.md#waypointoptimizationfailedconstrainttypedef)
- [WaypointOptimizationPedestrianOptionsTypeDef](./type_defs.md#waypointoptimizationpedestrianoptionstypedef)
- [WaypointOptimizationRestCycleDurationsTypeDef](./type_defs.md#waypointoptimizationrestcycledurationstypedef)
- [WaypointOptimizationTrailerOptionsTypeDef](./type_defs.md#waypointoptimizationtraileroptionstypedef)
- [IsolineAvoidanceAreaGeometryTypeDef](./type_defs.md#isolineavoidanceareageometrytypedef)
- [RouteAvoidanceAreaGeometryTypeDef](./type_defs.md#routeavoidanceareageometrytypedef)
- [IsolineCarOptionsTypeDef](./type_defs.md#isolinecaroptionstypedef)
- [IsolineScooterOptionsTypeDef](./type_defs.md#isolinescooteroptionstypedef)
- [IsolineConnectionTypeDef](./type_defs.md#isolineconnectiontypedef)
- [IsolineDestinationOptionsTypeDef](./type_defs.md#isolinedestinationoptionstypedef)
- [IsolineOriginOptionsTypeDef](./type_defs.md#isolineoriginoptionstypedef)
- [IsolineTruckOptionsTypeDef](./type_defs.md#isolinetruckoptionstypedef)
- [RouteContinueHighwayStepDetailsTypeDef](./type_defs.md#routecontinuehighwaystepdetailstypedef)
- [RouteContinueStepDetailsTypeDef](./type_defs.md#routecontinuestepdetailstypedef)
- [RouteEnterHighwayStepDetailsTypeDef](./type_defs.md#routeenterhighwaystepdetailstypedef)
- [RouteExitStepDetailsTypeDef](./type_defs.md#routeexitstepdetailstypedef)
- [RouteFerrySpanTypeDef](./type_defs.md#routeferryspantypedef)
- [RouteKeepStepDetailsTypeDef](./type_defs.md#routekeepstepdetailstypedef)
- [RouteRampStepDetailsTypeDef](./type_defs.md#routerampstepdetailstypedef)
- [RouteRoundaboutEnterStepDetailsTypeDef](./type_defs.md#routeroundaboutenterstepdetailstypedef)
- [RouteRoundaboutExitStepDetailsTypeDef](./type_defs.md#routeroundaboutexitstepdetailstypedef)
- [RouteRoundaboutPassStepDetailsTypeDef](./type_defs.md#routeroundaboutpassstepdetailstypedef)
- [RouteTurnStepDetailsTypeDef](./type_defs.md#routeturnstepdetailstypedef)
- [RouteUTurnStepDetailsTypeDef](./type_defs.md#routeuturnstepdetailstypedef)
- [SnapToRoadsResponseTypeDef](./type_defs.md#snaptoroadsresponsetypedef)
- [RoadSnapTruckOptionsTypeDef](./type_defs.md#roadsnaptruckoptionstypedef)
- [RouteCarOptionsTypeDef](./type_defs.md#routecaroptionstypedef)
- [RouteScooterOptionsTypeDef](./type_defs.md#routescooteroptionstypedef)
- [RouteDestinationOptionsTypeDef](./type_defs.md#routedestinationoptionstypedef)
- [RouteOriginOptionsTypeDef](./type_defs.md#routeoriginoptionstypedef)
- [RouteWaypointTypeDef](./type_defs.md#routewaypointtypedef)
- [RouteDriverOptionsTypeDef](./type_defs.md#routedriveroptionstypedef)
- [RouteTollOptionsTypeDef](./type_defs.md#routetolloptionstypedef)
- [RouteFerryArrivalTypeDef](./type_defs.md#routeferryarrivaltypedef)
- [RouteFerryDepartureTypeDef](./type_defs.md#routeferrydeparturetypedef)
- [RouteFerrySummaryTypeDef](./type_defs.md#routeferrysummarytypedef)
- [RouteMajorRoadLabelTypeDef](./type_defs.md#routemajorroadlabeltypedef)
- [RouteRoadTypeDef](./type_defs.md#routeroadtypedef)
- [RouteSignpostLabelTypeDef](./type_defs.md#routesignpostlabeltypedef)
- [RouteMatrixBoundaryGeometryOutputTypeDef](./type_defs.md#routematrixboundarygeometryoutputtypedef)
- [RouteMatrixBoundaryGeometryTypeDef](./type_defs.md#routematrixboundarygeometrytypedef)
- [RouteMatrixAvoidanceAreaTypeDef](./type_defs.md#routematrixavoidanceareatypedef)
- [RouteMatrixCarOptionsTypeDef](./type_defs.md#routematrixcaroptionstypedef)
- [RouteMatrixScooterOptionsTypeDef](./type_defs.md#routematrixscooteroptionstypedef)
- [RouteMatrixDestinationOptionsTypeDef](./type_defs.md#routematrixdestinationoptionstypedef)
- [RouteMatrixOriginOptionsTypeDef](./type_defs.md#routematrixoriginoptionstypedef)
- [RouteMatrixTruckOptionsTypeDef](./type_defs.md#routematrixtruckoptionstypedef)
- [RoutePassThroughWaypointTypeDef](./type_defs.md#routepassthroughwaypointtypedef)
- [RoutePedestrianArrivalTypeDef](./type_defs.md#routepedestrianarrivaltypedef)
- [RoutePedestrianDepartureTypeDef](./type_defs.md#routepedestriandeparturetypedef)
- [RoutePedestrianSpanTypeDef](./type_defs.md#routepedestrianspantypedef)
- [RouteVehicleSpanTypeDef](./type_defs.md#routevehiclespantypedef)
- [RoutePedestrianSummaryTypeDef](./type_defs.md#routepedestriansummarytypedef)
- [RouteTollPassTypeDef](./type_defs.md#routetollpasstypedef)
- [RouteTollPriceSummaryTypeDef](./type_defs.md#routetollpricesummarytypedef)
- [RouteTollPriceTypeDef](./type_defs.md#routetollpricetypedef)
- [RouteTruckOptionsTypeDef](./type_defs.md#routetruckoptionstypedef)
- [RouteVehicleArrivalTypeDef](./type_defs.md#routevehiclearrivaltypedef)
- [RouteVehicleDepartureTypeDef](./type_defs.md#routevehicledeparturetypedef)
- [RouteVehicleSummaryTypeDef](./type_defs.md#routevehiclesummarytypedef)
- [RouteViolatedConstraintsTypeDef](./type_defs.md#routeviolatedconstraintstypedef)
- [WaypointOptimizationAccessHoursTypeDef](./type_defs.md#waypointoptimizationaccesshourstypedef)
- [WaypointOptimizationAvoidanceAreaTypeDef](./type_defs.md#waypointoptimizationavoidanceareatypedef)
- [WaypointOptimizationClusteringOptionsTypeDef](./type_defs.md#waypointoptimizationclusteringoptionstypedef)
- [WaypointOptimizationImpedingWaypointTypeDef](./type_defs.md#waypointoptimizationimpedingwaypointtypedef)
- [WaypointOptimizationRestCyclesTypeDef](./type_defs.md#waypointoptimizationrestcyclestypedef)
- [WaypointOptimizationTruckOptionsTypeDef](./type_defs.md#waypointoptimizationtruckoptionstypedef)
- [IsolineAvoidanceAreaTypeDef](./type_defs.md#isolineavoidanceareatypedef)
- [RouteAvoidanceAreaTypeDef](./type_defs.md#routeavoidanceareatypedef)
- [IsolineTypeDef](./type_defs.md#isolinetypedef)
- [IsolineTravelModeOptionsTypeDef](./type_defs.md#isolinetravelmodeoptionstypedef)
- [RoadSnapTravelModeOptionsTypeDef](./type_defs.md#roadsnaptravelmodeoptionstypedef)
- [RouteSignpostTypeDef](./type_defs.md#routesignposttypedef)
- [RouteMatrixBoundaryOutputTypeDef](./type_defs.md#routematrixboundaryoutputtypedef)
- [RouteMatrixBoundaryTypeDef](./type_defs.md#routematrixboundarytypedef)
- [RouteMatrixAvoidanceOptionsTypeDef](./type_defs.md#routematrixavoidanceoptionstypedef)
- [RouteMatrixDestinationTypeDef](./type_defs.md#routematrixdestinationtypedef)
- [RouteMatrixOriginTypeDef](./type_defs.md#routematrixorigintypedef)
- [RouteMatrixTravelModeOptionsTypeDef](./type_defs.md#routematrixtravelmodeoptionstypedef)
- [RouteFerryLegDetailsTypeDef](./type_defs.md#routeferrylegdetailstypedef)
- [RouteTollSummaryTypeDef](./type_defs.md#routetollsummarytypedef)
- [RouteTollRateTypeDef](./type_defs.md#routetollratetypedef)
- [RouteTravelModeOptionsTypeDef](./type_defs.md#routetravelmodeoptionstypedef)
- [RouteVehicleNoticeDetailTypeDef](./type_defs.md#routevehiclenoticedetailtypedef)
- [WaypointOptimizationDestinationOptionsTypeDef](./type_defs.md#waypointoptimizationdestinationoptionstypedef)
- [WaypointOptimizationWaypointTypeDef](./type_defs.md#waypointoptimizationwaypointtypedef)
- [WaypointOptimizationAvoidanceOptionsTypeDef](./type_defs.md#waypointoptimizationavoidanceoptionstypedef)
- [OptimizeWaypointsResponseTypeDef](./type_defs.md#optimizewaypointsresponsetypedef)
- [WaypointOptimizationDriverOptionsTypeDef](./type_defs.md#waypointoptimizationdriveroptionstypedef)
- [WaypointOptimizationTravelModeOptionsTypeDef](./type_defs.md#waypointoptimizationtravelmodeoptionstypedef)
- [IsolineAvoidanceOptionsTypeDef](./type_defs.md#isolineavoidanceoptionstypedef)
- [RouteAvoidanceOptionsTypeDef](./type_defs.md#routeavoidanceoptionstypedef)
- [CalculateIsolinesResponseTypeDef](./type_defs.md#calculateisolinesresponsetypedef)
- [SnapToRoadsRequestTypeDef](./type_defs.md#snaptoroadsrequesttypedef)
- [RoutePedestrianTravelStepTypeDef](./type_defs.md#routepedestriantravelsteptypedef)
- [RouteVehicleTravelStepTypeDef](./type_defs.md#routevehicletravelsteptypedef)
- [CalculateRouteMatrixResponseTypeDef](./type_defs.md#calculateroutematrixresponsetypedef)
- [RouteMatrixBoundaryUnionTypeDef](./type_defs.md#routematrixboundaryuniontypedef)
- [RouteSummaryTypeDef](./type_defs.md#routesummarytypedef)
- [RouteTollTypeDef](./type_defs.md#routetolltypedef)
- [RouteVehicleNoticeTypeDef](./type_defs.md#routevehiclenoticetypedef)
- [OptimizeWaypointsRequestTypeDef](./type_defs.md#optimizewaypointsrequesttypedef)
- [CalculateIsolinesRequestTypeDef](./type_defs.md#calculateisolinesrequesttypedef)
- [CalculateRoutesRequestTypeDef](./type_defs.md#calculateroutesrequesttypedef)
- [RoutePedestrianLegDetailsTypeDef](./type_defs.md#routepedestrianlegdetailstypedef)
- [CalculateRouteMatrixRequestTypeDef](./type_defs.md#calculateroutematrixrequesttypedef)
- [RouteVehicleLegDetailsTypeDef](./type_defs.md#routevehiclelegdetailstypedef)
- [RouteLegTypeDef](./type_defs.md#routelegtypedef)
- [RouteTypeDef](./type_defs.md#routetypedef)
- [CalculateRoutesResponseTypeDef](./type_defs.md#calculateroutesresponsetypedef)

