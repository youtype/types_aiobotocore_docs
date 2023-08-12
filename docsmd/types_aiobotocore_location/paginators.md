# Paginators

> [Index](../README.md) > [LocationService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
    type annotations stubs module [types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

## GetDevicePositionHistoryPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("get_device_position_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory)

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
    DeviceId: str,
    TrackerName: str,
    EndTimeExclusive: Union[datetime, str] = ...,
    StartTimeInclusive: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetDevicePositionHistoryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDevicePositionHistoryResponseTypeDef](./type_defs.md#getdevicepositionhistoryresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = {  # (1)
    "DeviceId": ...,
    "TrackerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef](./type_defs.md#getdevicepositionhistoryrequestgetdevicepositionhistorypaginatetypedef) 
## ListDevicePositionsPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_device_positions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions)

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
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDevicePositionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDevicePositionsResponseTypeDef](./type_defs.md#listdevicepositionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDevicePositionsRequestListDevicePositionsPaginateTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicePositionsRequestListDevicePositionsPaginateTypeDef](./type_defs.md#listdevicepositionsrequestlistdevicepositionspaginatetypedef) 
## ListGeofenceCollectionsPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_geofence_collections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections)

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
) -> AsyncIterator[ListGeofenceCollectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGeofenceCollectionsResponseTypeDef](./type_defs.md#listgeofencecollectionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef](./type_defs.md#listgeofencecollectionsrequestlistgeofencecollectionspaginatetypedef) 
## ListGeofencesPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_geofences")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences)

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
) -> AsyncIterator[ListGeofencesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGeofencesResponseTypeDef](./type_defs.md#listgeofencesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGeofencesRequestListGeofencesPaginateTypeDef = {  # (1)
    "CollectionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGeofencesRequestListGeofencesPaginateTypeDef](./type_defs.md#listgeofencesrequestlistgeofencespaginatetypedef) 
## ListKeysPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys)

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
) -> AsyncIterator[ListKeysResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ApiKeyFilterTypeDef](./type_defs.md#apikeyfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListKeysRequestListKeysPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeysRequestListKeysPaginateTypeDef](./type_defs.md#listkeysrequestlistkeyspaginatetypedef) 
## ListMapsPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_maps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps)

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
) -> AsyncIterator[ListMapsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMapsResponseTypeDef](./type_defs.md#listmapsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMapsRequestListMapsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMapsRequestListMapsPaginateTypeDef](./type_defs.md#listmapsrequestlistmapspaginatetypedef) 
## ListPlaceIndexesPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_place_indexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes)

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
) -> AsyncIterator[ListPlaceIndexesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPlaceIndexesResponseTypeDef](./type_defs.md#listplaceindexesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef](./type_defs.md#listplaceindexesrequestlistplaceindexespaginatetypedef) 
## ListRouteCalculatorsPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_route_calculators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators)

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
) -> AsyncIterator[ListRouteCalculatorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRouteCalculatorsResponseTypeDef](./type_defs.md#listroutecalculatorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef](./type_defs.md#listroutecalculatorsrequestlistroutecalculatorspaginatetypedef) 
## ListTrackerConsumersPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_tracker_consumers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers)

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
) -> AsyncIterator[ListTrackerConsumersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrackerConsumersResponseTypeDef](./type_defs.md#listtrackerconsumersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef](./type_defs.md#listtrackerconsumersrequestlisttrackerconsumerspaginatetypedef) 
## ListTrackersPaginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator("list_trackers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers)

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
) -> AsyncIterator[ListTrackersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrackersResponseTypeDef](./type_defs.md#listtrackersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTrackersRequestListTrackersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrackersRequestListTrackersPaginateTypeDef](./type_defs.md#listtrackersrequestlisttrackerspaginatetypedef) 
