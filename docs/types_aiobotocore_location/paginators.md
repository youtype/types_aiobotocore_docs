<a id="paginators-for-aiobotocore-locationservice-module"></a>

# Paginators for aiobotocore LocationService module

> [Index](../README.md) > [LocationService](./README.md) > Paginators

Auto-generated documentation for
[LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
type annotations stubs module
[types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

- [Paginators for aiobotocore LocationService module](#paginators-for-aiobotocore-locationservice-module)
  - [GetDevicePositionHistoryPaginator](#getdevicepositionhistorypaginator)
  - [ListDevicePositionsPaginator](#listdevicepositionspaginator)
  - [ListGeofenceCollectionsPaginator](#listgeofencecollectionspaginator)
  - [ListGeofencesPaginator](#listgeofencespaginator)
  - [ListMapsPaginator](#listmapspaginator)
  - [ListPlaceIndexesPaginator](#listplaceindexespaginator)
  - [ListRouteCalculatorsPaginator](#listroutecalculatorspaginator)
  - [ListTrackerConsumersPaginator](#listtrackerconsumerspaginator)
  - [ListTrackersPaginator](#listtrackerspaginator)

<a id="getdevicepositionhistorypaginator"></a>

## GetDevicePositionHistoryPaginator

Type annotations for
`session.create_client("location").get_paginator("get_device_position_history")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import GetDevicePositionHistoryPaginator

session = get_session()
async with session.create_client("location") as client:
    client: LocationServiceClient
    paginator: GetDevicePositionHistoryPaginator = client.get_paginator("get_device_position_history")
```

Boto3 documentation:
[LocationService.Paginator.GetDevicePositionHistory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory)

Arguments for `GetDevicePositionHistoryPaginator.paginate` method:

- `DeviceId`: `str` *(required)*
- `TrackerName`: `str` *(required)*
- `EndTimeExclusive`: `Union`\[`datetime`, `str`\]
- `StartTimeInclusive`: `Union`\[`datetime`, `str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDevicePositionHistoryPaginator.paginate` returns
`AsyncIterator`\[[GetDevicePositionHistoryResponseTypeDef](./type_defs.md#getdevicepositionhistoryresponsetypedef)\].

<a id="listdevicepositionspaginator"></a>

## ListDevicePositionsPaginator

Type annotations for
`session.create_client("location").get_paginator("list_device_positions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListDevicePositionsPaginator

session = get_session()
async with session.create_client("location") as client:
    client: LocationServiceClient
    paginator: ListDevicePositionsPaginator = client.get_paginator("list_device_positions")
```

Boto3 documentation:
[LocationService.Paginator.ListDevicePositions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions)

Arguments for `ListDevicePositionsPaginator.paginate` method:

- `TrackerName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDevicePositionsPaginator.paginate` returns
`AsyncIterator`\[[ListDevicePositionsResponseTypeDef](./type_defs.md#listdevicepositionsresponsetypedef)\].

<a id="listgeofencecollectionspaginator"></a>

## ListGeofenceCollectionsPaginator

Type annotations for
`session.create_client("location").get_paginator("list_geofence_collections")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListGeofenceCollectionsPaginator

session = get_session()
async with session.create_client("location") as client:
    client: LocationServiceClient
    paginator: ListGeofenceCollectionsPaginator = client.get_paginator("list_geofence_collections")
```

Boto3 documentation:
[LocationService.Paginator.ListGeofenceCollections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections)

Arguments for `ListGeofenceCollectionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGeofenceCollectionsPaginator.paginate` returns
`AsyncIterator`\[[ListGeofenceCollectionsResponseTypeDef](./type_defs.md#listgeofencecollectionsresponsetypedef)\].

<a id="listgeofencespaginator"></a>

## ListGeofencesPaginator

Type annotations for
`session.create_client("location").get_paginator("list_geofences")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListGeofencesPaginator

session = get_session()
async with session.create_client("location") as client:
    client: LocationServiceClient
    paginator: ListGeofencesPaginator = client.get_paginator("list_geofences")
```

Boto3 documentation:
[LocationService.Paginator.ListGeofences](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences)

Arguments for `ListGeofencesPaginator.paginate` method:

- `CollectionName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGeofencesPaginator.paginate` returns
`AsyncIterator`\[[ListGeofencesResponseTypeDef](./type_defs.md#listgeofencesresponsetypedef)\].

<a id="listmapspaginator"></a>

## ListMapsPaginator

Type annotations for
`session.create_client("location").get_paginator("list_maps")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListMapsPaginator

session = get_session()
async with session.create_client("location") as client:
    client: LocationServiceClient
    paginator: ListMapsPaginator = client.get_paginator("list_maps")
```

Boto3 documentation:
[LocationService.Paginator.ListMaps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps)

Arguments for `ListMapsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMapsPaginator.paginate` returns
`AsyncIterator`\[[ListMapsResponseTypeDef](./type_defs.md#listmapsresponsetypedef)\].

<a id="listplaceindexespaginator"></a>

## ListPlaceIndexesPaginator

Type annotations for
`session.create_client("location").get_paginator("list_place_indexes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListPlaceIndexesPaginator

session = get_session()
async with session.create_client("location") as client:
    client: LocationServiceClient
    paginator: ListPlaceIndexesPaginator = client.get_paginator("list_place_indexes")
```

Boto3 documentation:
[LocationService.Paginator.ListPlaceIndexes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes)

Arguments for `ListPlaceIndexesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPlaceIndexesPaginator.paginate` returns
`AsyncIterator`\[[ListPlaceIndexesResponseTypeDef](./type_defs.md#listplaceindexesresponsetypedef)\].

<a id="listroutecalculatorspaginator"></a>

## ListRouteCalculatorsPaginator

Type annotations for
`session.create_client("location").get_paginator("list_route_calculators")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListRouteCalculatorsPaginator

session = get_session()
async with session.create_client("location") as client:
    client: LocationServiceClient
    paginator: ListRouteCalculatorsPaginator = client.get_paginator("list_route_calculators")
```

Boto3 documentation:
[LocationService.Paginator.ListRouteCalculators](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators)

Arguments for `ListRouteCalculatorsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRouteCalculatorsPaginator.paginate` returns
`AsyncIterator`\[[ListRouteCalculatorsResponseTypeDef](./type_defs.md#listroutecalculatorsresponsetypedef)\].

<a id="listtrackerconsumerspaginator"></a>

## ListTrackerConsumersPaginator

Type annotations for
`session.create_client("location").get_paginator("list_tracker_consumers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListTrackerConsumersPaginator

session = get_session()
async with session.create_client("location") as client:
    client: LocationServiceClient
    paginator: ListTrackerConsumersPaginator = client.get_paginator("list_tracker_consumers")
```

Boto3 documentation:
[LocationService.Paginator.ListTrackerConsumers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers)

Arguments for `ListTrackerConsumersPaginator.paginate` method:

- `TrackerName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTrackerConsumersPaginator.paginate` returns
`AsyncIterator`\[[ListTrackerConsumersResponseTypeDef](./type_defs.md#listtrackerconsumersresponsetypedef)\].

<a id="listtrackerspaginator"></a>

## ListTrackersPaginator

Type annotations for
`session.create_client("location").get_paginator("list_trackers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_location.paginator import ListTrackersPaginator

session = get_session()
async with session.create_client("location") as client:
    client: LocationServiceClient
    paginator: ListTrackersPaginator = client.get_paginator("list_trackers")
```

Boto3 documentation:
[LocationService.Paginator.ListTrackers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers)

Arguments for `ListTrackersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTrackersPaginator.paginate` returns
`AsyncIterator`\[[ListTrackersResponseTypeDef](./type_defs.md#listtrackersresponsetypedef)\].
