# Paginators

> [Index](../README.md) > [LocationService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#locationservice)
    type annotations stubs module [types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

## ForecastGeofenceEventsPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("forecast_geofence_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/paginator/ForecastGeofenceEvents.html#LocationService.Paginator.ForecastGeofenceEvents)

```python
# ForecastGeofenceEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ForecastGeofenceEventsPaginator

session = get_session()
async with session.create_client("location") as client:  # (1)
    paginator: ForecastGeofenceEventsPaginator = client.get_paginator("forecast_geofence_events")  # (2)
    async for item in paginator.paginate(...):
        item: ForecastGeofenceEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ForecastGeofenceEventsPaginator](./paginators.md#forecastgeofenceeventspaginator)
3. item: [:material-code-braces: ForecastGeofenceEventsResponseTypeDef](./type_defs.md#forecastgeofenceeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ForecastGeofenceEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CollectionName: str,
    DeviceState: ForecastGeofenceEventsDeviceStateTypeDef,  # (1)
    TimeHorizonMinutes: float = ...,
    DistanceUnit: DistanceUnitType = ...,  # (2)
    SpeedUnit: SpeedUnitType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ForecastGeofenceEventsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: ForecastGeofenceEventsDeviceStateTypeDef](./type_defs.md#forecastgeofenceeventsdevicestatetypedef) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-brackets: SpeedUnitType](./literals.md#speedunittype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ForecastGeofenceEventsResponseTypeDef](./type_defs.md#forecastgeofenceeventsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ForecastGeofenceEventsRequestPaginateTypeDef = {  # (1)
    "CollectionName": ...,
    "DeviceState": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ForecastGeofenceEventsRequestPaginateTypeDef](./type_defs.md#forecastgeofenceeventsrequestpaginatetypedef) 
## GetDevicePositionHistoryPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("get_device_position_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/paginator/GetDevicePositionHistory.html#LocationService.Paginator.GetDevicePositionHistory)

```python
# GetDevicePositionHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import GetDevicePositionHistoryPaginator

session = get_session()
async with session.create_client("location") as client:  # (1)
    paginator: GetDevicePositionHistoryPaginator = client.get_paginator("get_device_position_history")  # (2)
    async for item in paginator.paginate(...):
        item: GetDevicePositionHistoryResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [GetDevicePositionHistoryPaginator](./paginators.md#getdevicepositionhistorypaginator)
3. item: [:material-code-braces: GetDevicePositionHistoryResponseTypeDef](./type_defs.md#getdevicepositionhistoryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetDevicePositionHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TrackerName: str,
    DeviceId: str,
    StartTimeInclusive: TimestampTypeDef = ...,
    EndTimeExclusive: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetDevicePositionHistoryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDevicePositionHistoryResponseTypeDef](./type_defs.md#getdevicepositionhistoryresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetDevicePositionHistoryRequestPaginateTypeDef = {  # (1)
    "TrackerName": ...,
    "DeviceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDevicePositionHistoryRequestPaginateTypeDef](./type_defs.md#getdevicepositionhistoryrequestpaginatetypedef) 
## ListDevicePositionsPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_device_positions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/paginator/ListDevicePositions.html#LocationService.Paginator.ListDevicePositions)

```python
# ListDevicePositionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListDevicePositionsPaginator

session = get_session()
async with session.create_client("location") as client:  # (1)
    paginator: ListDevicePositionsPaginator = client.get_paginator("list_device_positions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevicePositionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListDevicePositionsPaginator](./paginators.md#listdevicepositionspaginator)
3. item: [:material-code-braces: ListDevicePositionsResponseTypeDef](./type_defs.md#listdevicepositionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDevicePositionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TrackerName: str,
    FilterGeometry: TrackingFilterGeometryTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDevicePositionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TrackingFilterGeometryTypeDef](./type_defs.md#trackingfiltergeometrytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDevicePositionsResponseTypeDef](./type_defs.md#listdevicepositionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDevicePositionsRequestPaginateTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicePositionsRequestPaginateTypeDef](./type_defs.md#listdevicepositionsrequestpaginatetypedef) 
## ListGeofenceCollectionsPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_geofence_collections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/paginator/ListGeofenceCollections.html#LocationService.Paginator.ListGeofenceCollections)

```python
# ListGeofenceCollectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListGeofenceCollectionsPaginator

session = get_session()
async with session.create_client("location") as client:  # (1)
    paginator: ListGeofenceCollectionsPaginator = client.get_paginator("list_geofence_collections")  # (2)
    async for item in paginator.paginate(...):
        item: ListGeofenceCollectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListGeofenceCollectionsPaginator](./paginators.md#listgeofencecollectionspaginator)
3. item: [:material-code-braces: ListGeofenceCollectionsResponseTypeDef](./type_defs.md#listgeofencecollectionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGeofenceCollectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGeofenceCollectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGeofenceCollectionsResponseTypeDef](./type_defs.md#listgeofencecollectionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGeofenceCollectionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGeofenceCollectionsRequestPaginateTypeDef](./type_defs.md#listgeofencecollectionsrequestpaginatetypedef) 
## ListGeofencesPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_geofences")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/paginator/ListGeofences.html#LocationService.Paginator.ListGeofences)

```python
# ListGeofencesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListGeofencesPaginator

session = get_session()
async with session.create_client("location") as client:  # (1)
    paginator: ListGeofencesPaginator = client.get_paginator("list_geofences")  # (2)
    async for item in paginator.paginate(...):
        item: ListGeofencesResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListGeofencesPaginator](./paginators.md#listgeofencespaginator)
3. item: [:material-code-braces: ListGeofencesResponseTypeDef](./type_defs.md#listgeofencesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGeofencesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CollectionName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGeofencesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGeofencesResponseTypeDef](./type_defs.md#listgeofencesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGeofencesRequestPaginateTypeDef = {  # (1)
    "CollectionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGeofencesRequestPaginateTypeDef](./type_defs.md#listgeofencesrequestpaginatetypedef) 
## ListKeysPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/paginator/ListKeys.html#LocationService.Paginator.ListKeys)

```python
# ListKeysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListKeysPaginator

session = get_session()
async with session.create_client("location") as client:  # (1)
    paginator: ListKeysPaginator = client.get_paginator("list_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListKeysPaginator](./paginators.md#listkeyspaginator)
3. item: [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: ApiKeyFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListKeysResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ApiKeyFilterTypeDef](./type_defs.md#apikeyfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListKeysRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeysRequestPaginateTypeDef](./type_defs.md#listkeysrequestpaginatetypedef) 
## ListMapsPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_maps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/paginator/ListMaps.html#LocationService.Paginator.ListMaps)

```python
# ListMapsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListMapsPaginator

session = get_session()
async with session.create_client("location") as client:  # (1)
    paginator: ListMapsPaginator = client.get_paginator("list_maps")  # (2)
    async for item in paginator.paginate(...):
        item: ListMapsResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListMapsPaginator](./paginators.md#listmapspaginator)
3. item: [:material-code-braces: ListMapsResponseTypeDef](./type_defs.md#listmapsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMapsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMapsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMapsResponseTypeDef](./type_defs.md#listmapsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMapsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMapsRequestPaginateTypeDef](./type_defs.md#listmapsrequestpaginatetypedef) 
## ListPlaceIndexesPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_place_indexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/paginator/ListPlaceIndexes.html#LocationService.Paginator.ListPlaceIndexes)

```python
# ListPlaceIndexesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListPlaceIndexesPaginator

session = get_session()
async with session.create_client("location") as client:  # (1)
    paginator: ListPlaceIndexesPaginator = client.get_paginator("list_place_indexes")  # (2)
    async for item in paginator.paginate(...):
        item: ListPlaceIndexesResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListPlaceIndexesPaginator](./paginators.md#listplaceindexespaginator)
3. item: [:material-code-braces: ListPlaceIndexesResponseTypeDef](./type_defs.md#listplaceindexesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPlaceIndexesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPlaceIndexesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPlaceIndexesResponseTypeDef](./type_defs.md#listplaceindexesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPlaceIndexesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPlaceIndexesRequestPaginateTypeDef](./type_defs.md#listplaceindexesrequestpaginatetypedef) 
## ListRouteCalculatorsPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_route_calculators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/paginator/ListRouteCalculators.html#LocationService.Paginator.ListRouteCalculators)

```python
# ListRouteCalculatorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListRouteCalculatorsPaginator

session = get_session()
async with session.create_client("location") as client:  # (1)
    paginator: ListRouteCalculatorsPaginator = client.get_paginator("list_route_calculators")  # (2)
    async for item in paginator.paginate(...):
        item: ListRouteCalculatorsResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListRouteCalculatorsPaginator](./paginators.md#listroutecalculatorspaginator)
3. item: [:material-code-braces: ListRouteCalculatorsResponseTypeDef](./type_defs.md#listroutecalculatorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRouteCalculatorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRouteCalculatorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRouteCalculatorsResponseTypeDef](./type_defs.md#listroutecalculatorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRouteCalculatorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRouteCalculatorsRequestPaginateTypeDef](./type_defs.md#listroutecalculatorsrequestpaginatetypedef) 
## ListTrackerConsumersPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_tracker_consumers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/paginator/ListTrackerConsumers.html#LocationService.Paginator.ListTrackerConsumers)

```python
# ListTrackerConsumersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListTrackerConsumersPaginator

session = get_session()
async with session.create_client("location") as client:  # (1)
    paginator: ListTrackerConsumersPaginator = client.get_paginator("list_tracker_consumers")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrackerConsumersResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListTrackerConsumersPaginator](./paginators.md#listtrackerconsumerspaginator)
3. item: [:material-code-braces: ListTrackerConsumersResponseTypeDef](./type_defs.md#listtrackerconsumersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTrackerConsumersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TrackerName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTrackerConsumersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrackerConsumersResponseTypeDef](./type_defs.md#listtrackerconsumersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTrackerConsumersRequestPaginateTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrackerConsumersRequestPaginateTypeDef](./type_defs.md#listtrackerconsumersrequestpaginatetypedef) 
## ListTrackersPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_trackers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location/paginator/ListTrackers.html#LocationService.Paginator.ListTrackers)

```python
# ListTrackersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListTrackersPaginator

session = get_session()
async with session.create_client("location") as client:  # (1)
    paginator: ListTrackersPaginator = client.get_paginator("list_trackers")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrackersResponseTypeDef
        print(item)  # (3)
```

1. client: [LocationServiceClient](./client.md)
2. paginator: [ListTrackersPaginator](./paginators.md#listtrackerspaginator)
3. item: [:material-code-braces: ListTrackersResponseTypeDef](./type_defs.md#listtrackersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTrackersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTrackersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrackersResponseTypeDef](./type_defs.md#listtrackersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTrackersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrackersRequestPaginateTypeDef](./type_defs.md#listtrackersrequestpaginatetypedef) 
