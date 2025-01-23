# LocationService module

> [Index](../README.md) > LocationService


!!! note ""

    Auto-generated documentation for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#locationservice)
    type annotations stubs module [types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `LocationService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `LocationService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[location]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[location]'

# standalone installation
python -m pip install types-aiobotocore-location
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-location
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LocationServiceClient

Type annotations and code completion for  `#!python session.create_client("location")` as [LocationServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client)

```python
# LocationServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.client import LocationServiceClient


session = get_session()
async with session.create_client("location") as client:
    client: LocationServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("location").get_paginator("...")`.

```python
# ForecastGeofenceEventsPaginator usage example

from types_aiobotocore_location.paginator import ForecastGeofenceEventsPaginator

def get_forecast_geofence_events_paginator() -> ForecastGeofenceEventsPaginator:
    return client.get_paginator("forecast_geofence_events"))
```

- [ForecastGeofenceEventsPaginator](./paginators.md#forecastgeofenceeventspaginator)
- [GetDevicePositionHistoryPaginator](./paginators.md#getdevicepositionhistorypaginator)
- [ListDevicePositionsPaginator](./paginators.md#listdevicepositionspaginator)
- [ListGeofenceCollectionsPaginator](./paginators.md#listgeofencecollectionspaginator)
- [ListGeofencesPaginator](./paginators.md#listgeofencespaginator)
- [ListKeysPaginator](./paginators.md#listkeyspaginator)
- [ListMapsPaginator](./paginators.md#listmapspaginator)
- [ListPlaceIndexesPaginator](./paginators.md#listplaceindexespaginator)
- [ListRouteCalculatorsPaginator](./paginators.md#listroutecalculatorspaginator)
- [ListTrackerConsumersPaginator](./paginators.md#listtrackerconsumerspaginator)
- [ListTrackersPaginator](./paginators.md#listtrackerspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BatchItemErrorCodeType usage example

from types_aiobotocore_location.literals import BatchItemErrorCodeType

def get_value() -> BatchItemErrorCodeType:
    return "AccessDeniedError"
```

- [BatchItemErrorCodeType](./literals.md#batchitemerrorcodetype)
- [DimensionUnitType](./literals.md#dimensionunittype)
- [DistanceUnitType](./literals.md#distanceunittype)
- [ForecastGeofenceEventsPaginatorName](./literals.md#forecastgeofenceeventspaginatorname)
- [ForecastedGeofenceEventTypeType](./literals.md#forecastedgeofenceeventtypetype)
- [GetDevicePositionHistoryPaginatorName](./literals.md#getdevicepositionhistorypaginatorname)
- [IntendedUseType](./literals.md#intendedusetype)
- [ListDevicePositionsPaginatorName](./literals.md#listdevicepositionspaginatorname)
- [ListGeofenceCollectionsPaginatorName](./literals.md#listgeofencecollectionspaginatorname)
- [ListGeofencesPaginatorName](./literals.md#listgeofencespaginatorname)
- [ListKeysPaginatorName](./literals.md#listkeyspaginatorname)
- [ListMapsPaginatorName](./literals.md#listmapspaginatorname)
- [ListPlaceIndexesPaginatorName](./literals.md#listplaceindexespaginatorname)
- [ListRouteCalculatorsPaginatorName](./literals.md#listroutecalculatorspaginatorname)
- [ListTrackerConsumersPaginatorName](./literals.md#listtrackerconsumerspaginatorname)
- [ListTrackersPaginatorName](./literals.md#listtrackerspaginatorname)
- [OptimizationModeType](./literals.md#optimizationmodetype)
- [PositionFilteringType](./literals.md#positionfilteringtype)
- [PricingPlanType](./literals.md#pricingplantype)
- [RouteMatrixErrorCodeType](./literals.md#routematrixerrorcodetype)
- [SpeedUnitType](./literals.md#speedunittype)
- [StatusType](./literals.md#statustype)
- [TravelModeType](./literals.md#travelmodetype)
- [VehicleWeightUnitType](./literals.md#vehicleweightunittype)
- [LocationServiceServiceName](./literals.md#locationserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ApiKeyFilterTypeDef](./type_defs.md#apikeyfiltertypedef)
- [ApiKeyRestrictionsOutputTypeDef](./type_defs.md#apikeyrestrictionsoutputtypedef)
- [ApiKeyRestrictionsTypeDef](./type_defs.md#apikeyrestrictionstypedef)
- [AssociateTrackerConsumerRequestRequestTypeDef](./type_defs.md#associatetrackerconsumerrequestrequesttypedef)
- [BatchItemErrorTypeDef](./type_defs.md#batchitemerrortypedef)
- [BatchDeleteDevicePositionHistoryRequestRequestTypeDef](./type_defs.md#batchdeletedevicepositionhistoryrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchDeleteGeofenceRequestRequestTypeDef](./type_defs.md#batchdeletegeofencerequestrequesttypedef)
- [BatchGetDevicePositionRequestRequestTypeDef](./type_defs.md#batchgetdevicepositionrequestrequesttypedef)
- [BatchPutGeofenceSuccessTypeDef](./type_defs.md#batchputgeofencesuccesstypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CalculateRouteCarModeOptionsTypeDef](./type_defs.md#calculateroutecarmodeoptionstypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [CalculateRouteMatrixSummaryTypeDef](./type_defs.md#calculateroutematrixsummarytypedef)
- [CalculateRouteSummaryTypeDef](./type_defs.md#calculateroutesummarytypedef)
- [TruckDimensionsTypeDef](./type_defs.md#truckdimensionstypedef)
- [TruckWeightTypeDef](./type_defs.md#truckweighttypedef)
- [CircleOutputTypeDef](./type_defs.md#circleoutputtypedef)
- [CircleTypeDef](./type_defs.md#circletypedef)
- [CreateGeofenceCollectionRequestRequestTypeDef](./type_defs.md#creategeofencecollectionrequestrequesttypedef)
- [MapConfigurationTypeDef](./type_defs.md#mapconfigurationtypedef)
- [DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef)
- [CreateRouteCalculatorRequestRequestTypeDef](./type_defs.md#createroutecalculatorrequestrequesttypedef)
- [CreateTrackerRequestRequestTypeDef](./type_defs.md#createtrackerrequestrequesttypedef)
- [DeleteGeofenceCollectionRequestRequestTypeDef](./type_defs.md#deletegeofencecollectionrequestrequesttypedef)
- [DeleteKeyRequestRequestTypeDef](./type_defs.md#deletekeyrequestrequesttypedef)
- [DeleteMapRequestRequestTypeDef](./type_defs.md#deletemaprequestrequesttypedef)
- [DeletePlaceIndexRequestRequestTypeDef](./type_defs.md#deleteplaceindexrequestrequesttypedef)
- [DeleteRouteCalculatorRequestRequestTypeDef](./type_defs.md#deleteroutecalculatorrequestrequesttypedef)
- [DeleteTrackerRequestRequestTypeDef](./type_defs.md#deletetrackerrequestrequesttypedef)
- [DescribeGeofenceCollectionRequestRequestTypeDef](./type_defs.md#describegeofencecollectionrequestrequesttypedef)
- [DescribeKeyRequestRequestTypeDef](./type_defs.md#describekeyrequestrequesttypedef)
- [DescribeMapRequestRequestTypeDef](./type_defs.md#describemaprequestrequesttypedef)
- [MapConfigurationOutputTypeDef](./type_defs.md#mapconfigurationoutputtypedef)
- [DescribePlaceIndexRequestRequestTypeDef](./type_defs.md#describeplaceindexrequestrequesttypedef)
- [DescribeRouteCalculatorRequestRequestTypeDef](./type_defs.md#describeroutecalculatorrequestrequesttypedef)
- [DescribeTrackerRequestRequestTypeDef](./type_defs.md#describetrackerrequestrequesttypedef)
- [PositionalAccuracyTypeDef](./type_defs.md#positionalaccuracytypedef)
- [WiFiAccessPointTypeDef](./type_defs.md#wifiaccesspointtypedef)
- [DisassociateTrackerConsumerRequestRequestTypeDef](./type_defs.md#disassociatetrackerconsumerrequestrequesttypedef)
- [ForecastGeofenceEventsDeviceStateTypeDef](./type_defs.md#forecastgeofenceeventsdevicestatetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ForecastedEventTypeDef](./type_defs.md#forecastedeventtypedef)
- [GetDevicePositionRequestRequestTypeDef](./type_defs.md#getdevicepositionrequestrequesttypedef)
- [GetGeofenceRequestRequestTypeDef](./type_defs.md#getgeofencerequestrequesttypedef)
- [GetMapGlyphsRequestRequestTypeDef](./type_defs.md#getmapglyphsrequestrequesttypedef)
- [GetMapSpritesRequestRequestTypeDef](./type_defs.md#getmapspritesrequestrequesttypedef)
- [GetMapStyleDescriptorRequestRequestTypeDef](./type_defs.md#getmapstyledescriptorrequestrequesttypedef)
- [GetMapTileRequestRequestTypeDef](./type_defs.md#getmaptilerequestrequesttypedef)
- [GetPlaceRequestRequestTypeDef](./type_defs.md#getplacerequestrequesttypedef)
- [LegGeometryTypeDef](./type_defs.md#leggeometrytypedef)
- [StepTypeDef](./type_defs.md#steptypedef)
- [TrackingFilterGeometryTypeDef](./type_defs.md#trackingfiltergeometrytypedef)
- [ListGeofenceCollectionsRequestRequestTypeDef](./type_defs.md#listgeofencecollectionsrequestrequesttypedef)
- [ListGeofenceCollectionsResponseEntryTypeDef](./type_defs.md#listgeofencecollectionsresponseentrytypedef)
- [ListGeofencesRequestRequestTypeDef](./type_defs.md#listgeofencesrequestrequesttypedef)
- [ListMapsRequestRequestTypeDef](./type_defs.md#listmapsrequestrequesttypedef)
- [ListMapsResponseEntryTypeDef](./type_defs.md#listmapsresponseentrytypedef)
- [ListPlaceIndexesRequestRequestTypeDef](./type_defs.md#listplaceindexesrequestrequesttypedef)
- [ListPlaceIndexesResponseEntryTypeDef](./type_defs.md#listplaceindexesresponseentrytypedef)
- [ListRouteCalculatorsRequestRequestTypeDef](./type_defs.md#listroutecalculatorsrequestrequesttypedef)
- [ListRouteCalculatorsResponseEntryTypeDef](./type_defs.md#listroutecalculatorsresponseentrytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTrackerConsumersRequestRequestTypeDef](./type_defs.md#listtrackerconsumersrequestrequesttypedef)
- [ListTrackersRequestRequestTypeDef](./type_defs.md#listtrackersrequestrequesttypedef)
- [ListTrackersResponseEntryTypeDef](./type_defs.md#listtrackersresponseentrytypedef)
- [LteLocalIdTypeDef](./type_defs.md#ltelocalidtypedef)
- [LteNetworkMeasurementsTypeDef](./type_defs.md#ltenetworkmeasurementstypedef)
- [MapConfigurationUpdateTypeDef](./type_defs.md#mapconfigurationupdatetypedef)
- [PlaceGeometryTypeDef](./type_defs.md#placegeometrytypedef)
- [TimeZoneTypeDef](./type_defs.md#timezonetypedef)
- [RouteMatrixEntryErrorTypeDef](./type_defs.md#routematrixentryerrortypedef)
- [SearchForSuggestionsResultTypeDef](./type_defs.md#searchforsuggestionsresulttypedef)
- [SearchPlaceIndexForPositionRequestRequestTypeDef](./type_defs.md#searchplaceindexforpositionrequestrequesttypedef)
- [SearchPlaceIndexForPositionSummaryTypeDef](./type_defs.md#searchplaceindexforpositionsummarytypedef)
- [SearchPlaceIndexForSuggestionsRequestRequestTypeDef](./type_defs.md#searchplaceindexforsuggestionsrequestrequesttypedef)
- [SearchPlaceIndexForSuggestionsSummaryTypeDef](./type_defs.md#searchplaceindexforsuggestionssummarytypedef)
- [SearchPlaceIndexForTextRequestRequestTypeDef](./type_defs.md#searchplaceindexfortextrequestrequesttypedef)
- [SearchPlaceIndexForTextSummaryTypeDef](./type_defs.md#searchplaceindexfortextsummarytypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateGeofenceCollectionRequestRequestTypeDef](./type_defs.md#updategeofencecollectionrequestrequesttypedef)
- [UpdateRouteCalculatorRequestRequestTypeDef](./type_defs.md#updateroutecalculatorrequestrequesttypedef)
- [UpdateTrackerRequestRequestTypeDef](./type_defs.md#updatetrackerrequestrequesttypedef)
- [ListKeysRequestRequestTypeDef](./type_defs.md#listkeysrequestrequesttypedef)
- [ListKeysResponseEntryTypeDef](./type_defs.md#listkeysresponseentrytypedef)
- [BatchDeleteDevicePositionHistoryErrorTypeDef](./type_defs.md#batchdeletedevicepositionhistoryerrortypedef)
- [BatchDeleteGeofenceErrorTypeDef](./type_defs.md#batchdeletegeofenceerrortypedef)
- [BatchEvaluateGeofencesErrorTypeDef](./type_defs.md#batchevaluategeofenceserrortypedef)
- [BatchGetDevicePositionErrorTypeDef](./type_defs.md#batchgetdevicepositionerrortypedef)
- [BatchPutGeofenceErrorTypeDef](./type_defs.md#batchputgeofenceerrortypedef)
- [BatchUpdateDevicePositionErrorTypeDef](./type_defs.md#batchupdatedevicepositionerrortypedef)
- [CreateGeofenceCollectionResponseTypeDef](./type_defs.md#creategeofencecollectionresponsetypedef)
- [CreateKeyResponseTypeDef](./type_defs.md#createkeyresponsetypedef)
- [CreateMapResponseTypeDef](./type_defs.md#createmapresponsetypedef)
- [CreatePlaceIndexResponseTypeDef](./type_defs.md#createplaceindexresponsetypedef)
- [CreateRouteCalculatorResponseTypeDef](./type_defs.md#createroutecalculatorresponsetypedef)
- [CreateTrackerResponseTypeDef](./type_defs.md#createtrackerresponsetypedef)
- [DescribeGeofenceCollectionResponseTypeDef](./type_defs.md#describegeofencecollectionresponsetypedef)
- [DescribeKeyResponseTypeDef](./type_defs.md#describekeyresponsetypedef)
- [DescribeRouteCalculatorResponseTypeDef](./type_defs.md#describeroutecalculatorresponsetypedef)
- [DescribeTrackerResponseTypeDef](./type_defs.md#describetrackerresponsetypedef)
- [GetMapGlyphsResponseTypeDef](./type_defs.md#getmapglyphsresponsetypedef)
- [GetMapSpritesResponseTypeDef](./type_defs.md#getmapspritesresponsetypedef)
- [GetMapStyleDescriptorResponseTypeDef](./type_defs.md#getmapstyledescriptorresponsetypedef)
- [GetMapTileResponseTypeDef](./type_defs.md#getmaptileresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListTrackerConsumersResponseTypeDef](./type_defs.md#listtrackerconsumersresponsetypedef)
- [PutGeofenceResponseTypeDef](./type_defs.md#putgeofenceresponsetypedef)
- [UpdateGeofenceCollectionResponseTypeDef](./type_defs.md#updategeofencecollectionresponsetypedef)
- [UpdateKeyResponseTypeDef](./type_defs.md#updatekeyresponsetypedef)
- [UpdateMapResponseTypeDef](./type_defs.md#updatemapresponsetypedef)
- [UpdatePlaceIndexResponseTypeDef](./type_defs.md#updateplaceindexresponsetypedef)
- [UpdateRouteCalculatorResponseTypeDef](./type_defs.md#updateroutecalculatorresponsetypedef)
- [UpdateTrackerResponseTypeDef](./type_defs.md#updatetrackerresponsetypedef)
- [CreateKeyRequestRequestTypeDef](./type_defs.md#createkeyrequestrequesttypedef)
- [GetDevicePositionHistoryRequestRequestTypeDef](./type_defs.md#getdevicepositionhistoryrequestrequesttypedef)
- [UpdateKeyRequestRequestTypeDef](./type_defs.md#updatekeyrequestrequesttypedef)
- [CalculateRouteTruckModeOptionsTypeDef](./type_defs.md#calculateroutetruckmodeoptionstypedef)
- [GeofenceGeometryOutputTypeDef](./type_defs.md#geofencegeometryoutputtypedef)
- [CircleUnionTypeDef](./type_defs.md#circleuniontypedef)
- [CreateMapRequestRequestTypeDef](./type_defs.md#createmaprequestrequesttypedef)
- [CreatePlaceIndexRequestRequestTypeDef](./type_defs.md#createplaceindexrequestrequesttypedef)
- [DescribePlaceIndexResponseTypeDef](./type_defs.md#describeplaceindexresponsetypedef)
- [UpdatePlaceIndexRequestRequestTypeDef](./type_defs.md#updateplaceindexrequestrequesttypedef)
- [DescribeMapResponseTypeDef](./type_defs.md#describemapresponsetypedef)
- [DevicePositionTypeDef](./type_defs.md#devicepositiontypedef)
- [DevicePositionUpdateTypeDef](./type_defs.md#devicepositionupdatetypedef)
- [GetDevicePositionResponseTypeDef](./type_defs.md#getdevicepositionresponsetypedef)
- [InferredStateTypeDef](./type_defs.md#inferredstatetypedef)
- [ListDevicePositionsResponseEntryTypeDef](./type_defs.md#listdevicepositionsresponseentrytypedef)
- [ForecastGeofenceEventsRequestRequestTypeDef](./type_defs.md#forecastgeofenceeventsrequestrequesttypedef)
- [ForecastGeofenceEventsRequestPaginateTypeDef](./type_defs.md#forecastgeofenceeventsrequestpaginatetypedef)
- [GetDevicePositionHistoryRequestPaginateTypeDef](./type_defs.md#getdevicepositionhistoryrequestpaginatetypedef)
- [ListGeofenceCollectionsRequestPaginateTypeDef](./type_defs.md#listgeofencecollectionsrequestpaginatetypedef)
- [ListGeofencesRequestPaginateTypeDef](./type_defs.md#listgeofencesrequestpaginatetypedef)
- [ListKeysRequestPaginateTypeDef](./type_defs.md#listkeysrequestpaginatetypedef)
- [ListMapsRequestPaginateTypeDef](./type_defs.md#listmapsrequestpaginatetypedef)
- [ListPlaceIndexesRequestPaginateTypeDef](./type_defs.md#listplaceindexesrequestpaginatetypedef)
- [ListRouteCalculatorsRequestPaginateTypeDef](./type_defs.md#listroutecalculatorsrequestpaginatetypedef)
- [ListTrackerConsumersRequestPaginateTypeDef](./type_defs.md#listtrackerconsumersrequestpaginatetypedef)
- [ListTrackersRequestPaginateTypeDef](./type_defs.md#listtrackersrequestpaginatetypedef)
- [ForecastGeofenceEventsResponseTypeDef](./type_defs.md#forecastgeofenceeventsresponsetypedef)
- [LegTypeDef](./type_defs.md#legtypedef)
- [ListDevicePositionsRequestPaginateTypeDef](./type_defs.md#listdevicepositionsrequestpaginatetypedef)
- [ListDevicePositionsRequestRequestTypeDef](./type_defs.md#listdevicepositionsrequestrequesttypedef)
- [ListGeofenceCollectionsResponseTypeDef](./type_defs.md#listgeofencecollectionsresponsetypedef)
- [ListMapsResponseTypeDef](./type_defs.md#listmapsresponsetypedef)
- [ListPlaceIndexesResponseTypeDef](./type_defs.md#listplaceindexesresponsetypedef)
- [ListRouteCalculatorsResponseTypeDef](./type_defs.md#listroutecalculatorsresponsetypedef)
- [ListTrackersResponseTypeDef](./type_defs.md#listtrackersresponsetypedef)
- [LteCellDetailsTypeDef](./type_defs.md#ltecelldetailstypedef)
- [UpdateMapRequestRequestTypeDef](./type_defs.md#updatemaprequestrequesttypedef)
- [PlaceTypeDef](./type_defs.md#placetypedef)
- [RouteMatrixEntryTypeDef](./type_defs.md#routematrixentrytypedef)
- [SearchPlaceIndexForSuggestionsResponseTypeDef](./type_defs.md#searchplaceindexforsuggestionsresponsetypedef)
- [ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef)
- [BatchDeleteDevicePositionHistoryResponseTypeDef](./type_defs.md#batchdeletedevicepositionhistoryresponsetypedef)
- [BatchDeleteGeofenceResponseTypeDef](./type_defs.md#batchdeletegeofenceresponsetypedef)
- [BatchEvaluateGeofencesResponseTypeDef](./type_defs.md#batchevaluategeofencesresponsetypedef)
- [BatchPutGeofenceResponseTypeDef](./type_defs.md#batchputgeofenceresponsetypedef)
- [BatchUpdateDevicePositionResponseTypeDef](./type_defs.md#batchupdatedevicepositionresponsetypedef)
- [CalculateRouteMatrixRequestRequestTypeDef](./type_defs.md#calculateroutematrixrequestrequesttypedef)
- [CalculateRouteRequestRequestTypeDef](./type_defs.md#calculaterouterequestrequesttypedef)
- [GetGeofenceResponseTypeDef](./type_defs.md#getgeofenceresponsetypedef)
- [ListGeofenceResponseEntryTypeDef](./type_defs.md#listgeofenceresponseentrytypedef)
- [GeofenceGeometryTypeDef](./type_defs.md#geofencegeometrytypedef)
- [BatchGetDevicePositionResponseTypeDef](./type_defs.md#batchgetdevicepositionresponsetypedef)
- [GetDevicePositionHistoryResponseTypeDef](./type_defs.md#getdevicepositionhistoryresponsetypedef)
- [BatchEvaluateGeofencesRequestRequestTypeDef](./type_defs.md#batchevaluategeofencesrequestrequesttypedef)
- [BatchUpdateDevicePositionRequestRequestTypeDef](./type_defs.md#batchupdatedevicepositionrequestrequesttypedef)
- [VerifyDevicePositionResponseTypeDef](./type_defs.md#verifydevicepositionresponsetypedef)
- [ListDevicePositionsResponseTypeDef](./type_defs.md#listdevicepositionsresponsetypedef)
- [CalculateRouteResponseTypeDef](./type_defs.md#calculaterouteresponsetypedef)
- [CellSignalsTypeDef](./type_defs.md#cellsignalstypedef)
- [GetPlaceResponseTypeDef](./type_defs.md#getplaceresponsetypedef)
- [SearchForPositionResultTypeDef](./type_defs.md#searchforpositionresulttypedef)
- [SearchForTextResultTypeDef](./type_defs.md#searchfortextresulttypedef)
- [CalculateRouteMatrixResponseTypeDef](./type_defs.md#calculateroutematrixresponsetypedef)
- [ListGeofencesResponseTypeDef](./type_defs.md#listgeofencesresponsetypedef)
- [GeofenceGeometryUnionTypeDef](./type_defs.md#geofencegeometryuniontypedef)
- [PutGeofenceRequestRequestTypeDef](./type_defs.md#putgeofencerequestrequesttypedef)
- [DeviceStateTypeDef](./type_defs.md#devicestatetypedef)
- [SearchPlaceIndexForPositionResponseTypeDef](./type_defs.md#searchplaceindexforpositionresponsetypedef)
- [SearchPlaceIndexForTextResponseTypeDef](./type_defs.md#searchplaceindexfortextresponsetypedef)
- [BatchPutGeofenceRequestEntryTypeDef](./type_defs.md#batchputgeofencerequestentrytypedef)
- [VerifyDevicePositionRequestRequestTypeDef](./type_defs.md#verifydevicepositionrequestrequesttypedef)
- [BatchPutGeofenceRequestRequestTypeDef](./type_defs.md#batchputgeofencerequestrequesttypedef)

