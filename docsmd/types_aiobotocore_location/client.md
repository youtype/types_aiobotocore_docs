# LocationServiceClient

> [Index](../README.md) > [LocationService](./README.md) > LocationServiceClient

!!! note ""

    Auto-generated documentation for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
    type annotations stubs module [types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

## LocationServiceClient

Type annotations and code completion for `#!python session.create_client("location")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client)

```python
# LocationServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_location.client import LocationServiceClient

session = get_session()
async with session.create_client("location") as client:
    client: LocationServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("location").exceptions` structure.

```python
# LocationServiceClient.exceptions usage example

async with session.create_client("location") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# LocationServiceClient usage type checking example

from types_aiobotocore_location.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_tracker\_consumer

Creates an association between a geofence collection and a tracker resource.

Type annotations and code completion for `#!python session.create_client("location").associate_tracker_consumer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.associate_tracker_consumer)

```python
# associate_tracker_consumer method definition

await def associate_tracker_consumer(
    self,
    *,
    TrackerName: str,
    ConsumerArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_tracker_consumer method usage example with argument unpacking

kwargs: AssociateTrackerConsumerRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
    "ConsumerArn": ...,
}

parent.associate_tracker_consumer(**kwargs)
```

1. See [:material-code-braces: AssociateTrackerConsumerRequestRequestTypeDef](./type_defs.md#associatetrackerconsumerrequestrequesttypedef) 

### batch\_delete\_device\_position\_history

Deletes the position history of one or more devices from a tracker resource.

Type annotations and code completion for `#!python session.create_client("location").batch_delete_device_position_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.batch_delete_device_position_history)

```python
# batch_delete_device_position_history method definition

await def batch_delete_device_position_history(
    self,
    *,
    TrackerName: str,
    DeviceIds: Sequence[str],
) -> BatchDeleteDevicePositionHistoryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteDevicePositionHistoryResponseTypeDef](./type_defs.md#batchdeletedevicepositionhistoryresponsetypedef) 


```python
# batch_delete_device_position_history method usage example with argument unpacking

kwargs: BatchDeleteDevicePositionHistoryRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
    "DeviceIds": ...,
}

parent.batch_delete_device_position_history(**kwargs)
```

1. See [:material-code-braces: BatchDeleteDevicePositionHistoryRequestRequestTypeDef](./type_defs.md#batchdeletedevicepositionhistoryrequestrequesttypedef) 

### batch\_delete\_geofence

Deletes a batch of geofences from a geofence collection.

Type annotations and code completion for `#!python session.create_client("location").batch_delete_geofence` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.batch_delete_geofence)

```python
# batch_delete_geofence method definition

await def batch_delete_geofence(
    self,
    *,
    CollectionName: str,
    GeofenceIds: Sequence[str],
) -> BatchDeleteGeofenceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteGeofenceResponseTypeDef](./type_defs.md#batchdeletegeofenceresponsetypedef) 


```python
# batch_delete_geofence method usage example with argument unpacking

kwargs: BatchDeleteGeofenceRequestRequestTypeDef = {  # (1)
    "CollectionName": ...,
    "GeofenceIds": ...,
}

parent.batch_delete_geofence(**kwargs)
```

1. See [:material-code-braces: BatchDeleteGeofenceRequestRequestTypeDef](./type_defs.md#batchdeletegeofencerequestrequesttypedef) 

### batch\_evaluate\_geofences

Evaluates device positions against the geofence geometries from a given
geofence
collection.

Type annotations and code completion for `#!python session.create_client("location").batch_evaluate_geofences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.batch_evaluate_geofences)

```python
# batch_evaluate_geofences method definition

await def batch_evaluate_geofences(
    self,
    *,
    CollectionName: str,
    DevicePositionUpdates: Sequence[DevicePositionUpdateTypeDef],  # (1)
) -> BatchEvaluateGeofencesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DevicePositionUpdateTypeDef](./type_defs.md#devicepositionupdatetypedef) 
2. See [:material-code-braces: BatchEvaluateGeofencesResponseTypeDef](./type_defs.md#batchevaluategeofencesresponsetypedef) 


```python
# batch_evaluate_geofences method usage example with argument unpacking

kwargs: BatchEvaluateGeofencesRequestRequestTypeDef = {  # (1)
    "CollectionName": ...,
    "DevicePositionUpdates": ...,
}

parent.batch_evaluate_geofences(**kwargs)
```

1. See [:material-code-braces: BatchEvaluateGeofencesRequestRequestTypeDef](./type_defs.md#batchevaluategeofencesrequestrequesttypedef) 

### batch\_get\_device\_position

Lists the latest device positions for requested devices.

Type annotations and code completion for `#!python session.create_client("location").batch_get_device_position` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.batch_get_device_position)

```python
# batch_get_device_position method definition

await def batch_get_device_position(
    self,
    *,
    TrackerName: str,
    DeviceIds: Sequence[str],
) -> BatchGetDevicePositionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetDevicePositionResponseTypeDef](./type_defs.md#batchgetdevicepositionresponsetypedef) 


```python
# batch_get_device_position method usage example with argument unpacking

kwargs: BatchGetDevicePositionRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
    "DeviceIds": ...,
}

parent.batch_get_device_position(**kwargs)
```

1. See [:material-code-braces: BatchGetDevicePositionRequestRequestTypeDef](./type_defs.md#batchgetdevicepositionrequestrequesttypedef) 

### batch\_put\_geofence

A batch request for storing geofence geometries into a given geofence
collection, or updates the geometry of an existing geofence if a geofence ID is
included in the
request.

Type annotations and code completion for `#!python session.create_client("location").batch_put_geofence` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.batch_put_geofence)

```python
# batch_put_geofence method definition

await def batch_put_geofence(
    self,
    *,
    CollectionName: str,
    Entries: Sequence[BatchPutGeofenceRequestEntryTypeDef],  # (1)
) -> BatchPutGeofenceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchPutGeofenceRequestEntryTypeDef](./type_defs.md#batchputgeofencerequestentrytypedef) 
2. See [:material-code-braces: BatchPutGeofenceResponseTypeDef](./type_defs.md#batchputgeofenceresponsetypedef) 


```python
# batch_put_geofence method usage example with argument unpacking

kwargs: BatchPutGeofenceRequestRequestTypeDef = {  # (1)
    "CollectionName": ...,
    "Entries": ...,
}

parent.batch_put_geofence(**kwargs)
```

1. See [:material-code-braces: BatchPutGeofenceRequestRequestTypeDef](./type_defs.md#batchputgeofencerequestrequesttypedef) 

### batch\_update\_device\_position

Uploads position update data for one or more devices to a tracker resource (up
to 10 devices per
batch).

Type annotations and code completion for `#!python session.create_client("location").batch_update_device_position` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.batch_update_device_position)

```python
# batch_update_device_position method definition

await def batch_update_device_position(
    self,
    *,
    TrackerName: str,
    Updates: Sequence[DevicePositionUpdateTypeDef],  # (1)
) -> BatchUpdateDevicePositionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DevicePositionUpdateTypeDef](./type_defs.md#devicepositionupdatetypedef) 
2. See [:material-code-braces: BatchUpdateDevicePositionResponseTypeDef](./type_defs.md#batchupdatedevicepositionresponsetypedef) 


```python
# batch_update_device_position method usage example with argument unpacking

kwargs: BatchUpdateDevicePositionRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
    "Updates": ...,
}

parent.batch_update_device_position(**kwargs)
```

1. See [:material-code-braces: BatchUpdateDevicePositionRequestRequestTypeDef](./type_defs.md#batchupdatedevicepositionrequestrequesttypedef) 

### calculate\_route



Type annotations and code completion for `#!python session.create_client("location").calculate_route` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.calculate_route)

```python
# calculate_route method definition

await def calculate_route(
    self,
    *,
    CalculatorName: str,
    DeparturePosition: Sequence[float],
    DestinationPosition: Sequence[float],
    WaypointPositions: Sequence[Sequence[float]] = ...,
    TravelMode: TravelModeType = ...,  # (1)
    DepartureTime: TimestampTypeDef = ...,
    DepartNow: bool = ...,
    DistanceUnit: DistanceUnitType = ...,  # (2)
    IncludeLegGeometry: bool = ...,
    CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,  # (3)
    TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,  # (4)
    ArrivalTime: TimestampTypeDef = ...,
    OptimizeFor: OptimizationModeType = ...,  # (5)
    Key: str = ...,
) -> CalculateRouteResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: TravelModeType](./literals.md#travelmodetype) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-braces: CalculateRouteCarModeOptionsTypeDef](./type_defs.md#calculateroutecarmodeoptionstypedef) 
4. See [:material-code-braces: CalculateRouteTruckModeOptionsTypeDef](./type_defs.md#calculateroutetruckmodeoptionstypedef) 
5. See [:material-code-brackets: OptimizationModeType](./literals.md#optimizationmodetype) 
6. See [:material-code-braces: CalculateRouteResponseTypeDef](./type_defs.md#calculaterouteresponsetypedef) 


```python
# calculate_route method usage example with argument unpacking

kwargs: CalculateRouteRequestRequestTypeDef = {  # (1)
    "CalculatorName": ...,
    "DeparturePosition": ...,
    "DestinationPosition": ...,
}

parent.calculate_route(**kwargs)
```

1. See [:material-code-braces: CalculateRouteRequestRequestTypeDef](./type_defs.md#calculaterouterequestrequesttypedef) 

### calculate\_route\_matrix



Type annotations and code completion for `#!python session.create_client("location").calculate_route_matrix` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.calculate_route_matrix)

```python
# calculate_route_matrix method definition

await def calculate_route_matrix(
    self,
    *,
    CalculatorName: str,
    DeparturePositions: Sequence[Sequence[float]],
    DestinationPositions: Sequence[Sequence[float]],
    TravelMode: TravelModeType = ...,  # (1)
    DepartureTime: TimestampTypeDef = ...,
    DepartNow: bool = ...,
    DistanceUnit: DistanceUnitType = ...,  # (2)
    CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,  # (3)
    TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,  # (4)
    Key: str = ...,
) -> CalculateRouteMatrixResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: TravelModeType](./literals.md#travelmodetype) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-braces: CalculateRouteCarModeOptionsTypeDef](./type_defs.md#calculateroutecarmodeoptionstypedef) 
4. See [:material-code-braces: CalculateRouteTruckModeOptionsTypeDef](./type_defs.md#calculateroutetruckmodeoptionstypedef) 
5. See [:material-code-braces: CalculateRouteMatrixResponseTypeDef](./type_defs.md#calculateroutematrixresponsetypedef) 


```python
# calculate_route_matrix method usage example with argument unpacking

kwargs: CalculateRouteMatrixRequestRequestTypeDef = {  # (1)
    "CalculatorName": ...,
    "DeparturePositions": ...,
    "DestinationPositions": ...,
}

parent.calculate_route_matrix(**kwargs)
```

1. See [:material-code-braces: CalculateRouteMatrixRequestRequestTypeDef](./type_defs.md#calculateroutematrixrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("location").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("location").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_geofence\_collection

Creates a geofence collection, which manages and stores geofences.

Type annotations and code completion for `#!python session.create_client("location").create_geofence_collection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_geofence_collection)

```python
# create_geofence_collection method definition

await def create_geofence_collection(
    self,
    *,
    CollectionName: str,
    PricingPlan: PricingPlanType = ...,  # (1)
    PricingPlanDataSource: str = ...,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
    KmsKeyId: str = ...,
) -> CreateGeofenceCollectionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: CreateGeofenceCollectionResponseTypeDef](./type_defs.md#creategeofencecollectionresponsetypedef) 


```python
# create_geofence_collection method usage example with argument unpacking

kwargs: CreateGeofenceCollectionRequestRequestTypeDef = {  # (1)
    "CollectionName": ...,
}

parent.create_geofence_collection(**kwargs)
```

1. See [:material-code-braces: CreateGeofenceCollectionRequestRequestTypeDef](./type_defs.md#creategeofencecollectionrequestrequesttypedef) 

### create\_key

Creates an API key resource in your Amazon Web Services account, which lets you
grant actions for Amazon Location resources to the API key
bearer.

Type annotations and code completion for `#!python session.create_client("location").create_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_key)

```python
# create_key method definition

await def create_key(
    self,
    *,
    KeyName: str,
    Restrictions: ApiKeyRestrictionsTypeDef,  # (1)
    Description: str = ...,
    ExpireTime: TimestampTypeDef = ...,
    NoExpiry: bool = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateKeyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ApiKeyRestrictionsTypeDef](./type_defs.md#apikeyrestrictionstypedef) 
2. See [:material-code-braces: CreateKeyResponseTypeDef](./type_defs.md#createkeyresponsetypedef) 


```python
# create_key method usage example with argument unpacking

kwargs: CreateKeyRequestRequestTypeDef = {  # (1)
    "KeyName": ...,
    "Restrictions": ...,
}

parent.create_key(**kwargs)
```

1. See [:material-code-braces: CreateKeyRequestRequestTypeDef](./type_defs.md#createkeyrequestrequesttypedef) 

### create\_map

Creates a map resource in your Amazon Web Services account, which provides map
tiles of different styles sourced from global location data
providers.

Type annotations and code completion for `#!python session.create_client("location").create_map` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_map)

```python
# create_map method definition

await def create_map(
    self,
    *,
    MapName: str,
    Configuration: MapConfigurationTypeDef,  # (1)
    PricingPlan: PricingPlanType = ...,  # (2)
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateMapResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MapConfigurationTypeDef](./type_defs.md#mapconfigurationtypedef) 
2. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
3. See [:material-code-braces: CreateMapResponseTypeDef](./type_defs.md#createmapresponsetypedef) 


```python
# create_map method usage example with argument unpacking

kwargs: CreateMapRequestRequestTypeDef = {  # (1)
    "MapName": ...,
    "Configuration": ...,
}

parent.create_map(**kwargs)
```

1. See [:material-code-braces: CreateMapRequestRequestTypeDef](./type_defs.md#createmaprequestrequesttypedef) 

### create\_place\_index

Creates a place index resource in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").create_place_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_place_index)

```python
# create_place_index method definition

await def create_place_index(
    self,
    *,
    IndexName: str,
    DataSource: str,
    PricingPlan: PricingPlanType = ...,  # (1)
    Description: str = ...,
    DataSourceConfiguration: DataSourceConfigurationTypeDef = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> CreatePlaceIndexResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
3. See [:material-code-braces: CreatePlaceIndexResponseTypeDef](./type_defs.md#createplaceindexresponsetypedef) 


```python
# create_place_index method usage example with argument unpacking

kwargs: CreatePlaceIndexRequestRequestTypeDef = {  # (1)
    "IndexName": ...,
    "DataSource": ...,
}

parent.create_place_index(**kwargs)
```

1. See [:material-code-braces: CreatePlaceIndexRequestRequestTypeDef](./type_defs.md#createplaceindexrequestrequesttypedef) 

### create\_route\_calculator

Creates a route calculator resource in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").create_route_calculator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_route_calculator)

```python
# create_route_calculator method definition

await def create_route_calculator(
    self,
    *,
    CalculatorName: str,
    DataSource: str,
    PricingPlan: PricingPlanType = ...,  # (1)
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateRouteCalculatorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: CreateRouteCalculatorResponseTypeDef](./type_defs.md#createroutecalculatorresponsetypedef) 


```python
# create_route_calculator method usage example with argument unpacking

kwargs: CreateRouteCalculatorRequestRequestTypeDef = {  # (1)
    "CalculatorName": ...,
    "DataSource": ...,
}

parent.create_route_calculator(**kwargs)
```

1. See [:material-code-braces: CreateRouteCalculatorRequestRequestTypeDef](./type_defs.md#createroutecalculatorrequestrequesttypedef) 

### create\_tracker

Creates a tracker resource in your Amazon Web Services account, which lets you
retrieve current and historical location of
devices.

Type annotations and code completion for `#!python session.create_client("location").create_tracker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_tracker)

```python
# create_tracker method definition

await def create_tracker(
    self,
    *,
    TrackerName: str,
    PricingPlan: PricingPlanType = ...,  # (1)
    KmsKeyId: str = ...,
    PricingPlanDataSource: str = ...,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
    PositionFiltering: PositionFilteringType = ...,  # (2)
    EventBridgeEnabled: bool = ...,
    KmsKeyEnableGeospatialQueries: bool = ...,
) -> CreateTrackerResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-brackets: PositionFilteringType](./literals.md#positionfilteringtype) 
3. See [:material-code-braces: CreateTrackerResponseTypeDef](./type_defs.md#createtrackerresponsetypedef) 


```python
# create_tracker method usage example with argument unpacking

kwargs: CreateTrackerRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.create_tracker(**kwargs)
```

1. See [:material-code-braces: CreateTrackerRequestRequestTypeDef](./type_defs.md#createtrackerrequestrequesttypedef) 

### delete\_geofence\_collection

Deletes a geofence collection from your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").delete_geofence_collection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.delete_geofence_collection)

```python
# delete_geofence_collection method definition

await def delete_geofence_collection(
    self,
    *,
    CollectionName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_geofence_collection method usage example with argument unpacking

kwargs: DeleteGeofenceCollectionRequestRequestTypeDef = {  # (1)
    "CollectionName": ...,
}

parent.delete_geofence_collection(**kwargs)
```

1. See [:material-code-braces: DeleteGeofenceCollectionRequestRequestTypeDef](./type_defs.md#deletegeofencecollectionrequestrequesttypedef) 

### delete\_key

Deletes the specified API key.

Type annotations and code completion for `#!python session.create_client("location").delete_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.delete_key)

```python
# delete_key method definition

await def delete_key(
    self,
    *,
    KeyName: str,
    ForceDelete: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_key method usage example with argument unpacking

kwargs: DeleteKeyRequestRequestTypeDef = {  # (1)
    "KeyName": ...,
}

parent.delete_key(**kwargs)
```

1. See [:material-code-braces: DeleteKeyRequestRequestTypeDef](./type_defs.md#deletekeyrequestrequesttypedef) 

### delete\_map

Deletes a map resource from your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").delete_map` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.delete_map)

```python
# delete_map method definition

await def delete_map(
    self,
    *,
    MapName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_map method usage example with argument unpacking

kwargs: DeleteMapRequestRequestTypeDef = {  # (1)
    "MapName": ...,
}

parent.delete_map(**kwargs)
```

1. See [:material-code-braces: DeleteMapRequestRequestTypeDef](./type_defs.md#deletemaprequestrequesttypedef) 

### delete\_place\_index

Deletes a place index resource from your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").delete_place_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.delete_place_index)

```python
# delete_place_index method definition

await def delete_place_index(
    self,
    *,
    IndexName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_place_index method usage example with argument unpacking

kwargs: DeletePlaceIndexRequestRequestTypeDef = {  # (1)
    "IndexName": ...,
}

parent.delete_place_index(**kwargs)
```

1. See [:material-code-braces: DeletePlaceIndexRequestRequestTypeDef](./type_defs.md#deleteplaceindexrequestrequesttypedef) 

### delete\_route\_calculator

Deletes a route calculator resource from your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").delete_route_calculator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.delete_route_calculator)

```python
# delete_route_calculator method definition

await def delete_route_calculator(
    self,
    *,
    CalculatorName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_route_calculator method usage example with argument unpacking

kwargs: DeleteRouteCalculatorRequestRequestTypeDef = {  # (1)
    "CalculatorName": ...,
}

parent.delete_route_calculator(**kwargs)
```

1. See [:material-code-braces: DeleteRouteCalculatorRequestRequestTypeDef](./type_defs.md#deleteroutecalculatorrequestrequesttypedef) 

### delete\_tracker

Deletes a tracker resource from your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").delete_tracker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.delete_tracker)

```python
# delete_tracker method definition

await def delete_tracker(
    self,
    *,
    TrackerName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_tracker method usage example with argument unpacking

kwargs: DeleteTrackerRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.delete_tracker(**kwargs)
```

1. See [:material-code-braces: DeleteTrackerRequestRequestTypeDef](./type_defs.md#deletetrackerrequestrequesttypedef) 

### describe\_geofence\_collection

Retrieves the geofence collection details.

Type annotations and code completion for `#!python session.create_client("location").describe_geofence_collection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.describe_geofence_collection)

```python
# describe_geofence_collection method definition

await def describe_geofence_collection(
    self,
    *,
    CollectionName: str,
) -> DescribeGeofenceCollectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGeofenceCollectionResponseTypeDef](./type_defs.md#describegeofencecollectionresponsetypedef) 


```python
# describe_geofence_collection method usage example with argument unpacking

kwargs: DescribeGeofenceCollectionRequestRequestTypeDef = {  # (1)
    "CollectionName": ...,
}

parent.describe_geofence_collection(**kwargs)
```

1. See [:material-code-braces: DescribeGeofenceCollectionRequestRequestTypeDef](./type_defs.md#describegeofencecollectionrequestrequesttypedef) 

### describe\_key

Retrieves the API key resource details.

Type annotations and code completion for `#!python session.create_client("location").describe_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.describe_key)

```python
# describe_key method definition

await def describe_key(
    self,
    *,
    KeyName: str,
) -> DescribeKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeKeyResponseTypeDef](./type_defs.md#describekeyresponsetypedef) 


```python
# describe_key method usage example with argument unpacking

kwargs: DescribeKeyRequestRequestTypeDef = {  # (1)
    "KeyName": ...,
}

parent.describe_key(**kwargs)
```

1. See [:material-code-braces: DescribeKeyRequestRequestTypeDef](./type_defs.md#describekeyrequestrequesttypedef) 

### describe\_map

Retrieves the map resource details.

Type annotations and code completion for `#!python session.create_client("location").describe_map` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.describe_map)

```python
# describe_map method definition

await def describe_map(
    self,
    *,
    MapName: str,
) -> DescribeMapResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMapResponseTypeDef](./type_defs.md#describemapresponsetypedef) 


```python
# describe_map method usage example with argument unpacking

kwargs: DescribeMapRequestRequestTypeDef = {  # (1)
    "MapName": ...,
}

parent.describe_map(**kwargs)
```

1. See [:material-code-braces: DescribeMapRequestRequestTypeDef](./type_defs.md#describemaprequestrequesttypedef) 

### describe\_place\_index

Retrieves the place index resource details.

Type annotations and code completion for `#!python session.create_client("location").describe_place_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.describe_place_index)

```python
# describe_place_index method definition

await def describe_place_index(
    self,
    *,
    IndexName: str,
) -> DescribePlaceIndexResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePlaceIndexResponseTypeDef](./type_defs.md#describeplaceindexresponsetypedef) 


```python
# describe_place_index method usage example with argument unpacking

kwargs: DescribePlaceIndexRequestRequestTypeDef = {  # (1)
    "IndexName": ...,
}

parent.describe_place_index(**kwargs)
```

1. See [:material-code-braces: DescribePlaceIndexRequestRequestTypeDef](./type_defs.md#describeplaceindexrequestrequesttypedef) 

### describe\_route\_calculator

Retrieves the route calculator resource details.

Type annotations and code completion for `#!python session.create_client("location").describe_route_calculator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.describe_route_calculator)

```python
# describe_route_calculator method definition

await def describe_route_calculator(
    self,
    *,
    CalculatorName: str,
) -> DescribeRouteCalculatorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRouteCalculatorResponseTypeDef](./type_defs.md#describeroutecalculatorresponsetypedef) 


```python
# describe_route_calculator method usage example with argument unpacking

kwargs: DescribeRouteCalculatorRequestRequestTypeDef = {  # (1)
    "CalculatorName": ...,
}

parent.describe_route_calculator(**kwargs)
```

1. See [:material-code-braces: DescribeRouteCalculatorRequestRequestTypeDef](./type_defs.md#describeroutecalculatorrequestrequesttypedef) 

### describe\_tracker

Retrieves the tracker resource details.

Type annotations and code completion for `#!python session.create_client("location").describe_tracker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.describe_tracker)

```python
# describe_tracker method definition

await def describe_tracker(
    self,
    *,
    TrackerName: str,
) -> DescribeTrackerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrackerResponseTypeDef](./type_defs.md#describetrackerresponsetypedef) 


```python
# describe_tracker method usage example with argument unpacking

kwargs: DescribeTrackerRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.describe_tracker(**kwargs)
```

1. See [:material-code-braces: DescribeTrackerRequestRequestTypeDef](./type_defs.md#describetrackerrequestrequesttypedef) 

### disassociate\_tracker\_consumer

Removes the association between a tracker resource and a geofence collection.

Type annotations and code completion for `#!python session.create_client("location").disassociate_tracker_consumer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.disassociate_tracker_consumer)

```python
# disassociate_tracker_consumer method definition

await def disassociate_tracker_consumer(
    self,
    *,
    TrackerName: str,
    ConsumerArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_tracker_consumer method usage example with argument unpacking

kwargs: DisassociateTrackerConsumerRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
    "ConsumerArn": ...,
}

parent.disassociate_tracker_consumer(**kwargs)
```

1. See [:material-code-braces: DisassociateTrackerConsumerRequestRequestTypeDef](./type_defs.md#disassociatetrackerconsumerrequestrequesttypedef) 

### forecast\_geofence\_events

Evaluates device positions against geofence geometries from a given geofence
collection.

Type annotations and code completion for `#!python session.create_client("location").forecast_geofence_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.forecast_geofence_events)

```python
# forecast_geofence_events method definition

await def forecast_geofence_events(
    self,
    *,
    CollectionName: str,
    DeviceState: ForecastGeofenceEventsDeviceStateTypeDef,  # (1)
    TimeHorizonMinutes: float = ...,
    DistanceUnit: DistanceUnitType = ...,  # (2)
    SpeedUnit: SpeedUnitType = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ForecastGeofenceEventsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ForecastGeofenceEventsDeviceStateTypeDef](./type_defs.md#forecastgeofenceeventsdevicestatetypedef) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-brackets: SpeedUnitType](./literals.md#speedunittype) 
4. See [:material-code-braces: ForecastGeofenceEventsResponseTypeDef](./type_defs.md#forecastgeofenceeventsresponsetypedef) 


```python
# forecast_geofence_events method usage example with argument unpacking

kwargs: ForecastGeofenceEventsRequestRequestTypeDef = {  # (1)
    "CollectionName": ...,
    "DeviceState": ...,
}

parent.forecast_geofence_events(**kwargs)
```

1. See [:material-code-braces: ForecastGeofenceEventsRequestRequestTypeDef](./type_defs.md#forecastgeofenceeventsrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("location").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_device\_position

Retrieves a device's most recent position according to its sample time.

Type annotations and code completion for `#!python session.create_client("location").get_device_position` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_device_position)

```python
# get_device_position method definition

await def get_device_position(
    self,
    *,
    TrackerName: str,
    DeviceId: str,
) -> GetDevicePositionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDevicePositionResponseTypeDef](./type_defs.md#getdevicepositionresponsetypedef) 


```python
# get_device_position method usage example with argument unpacking

kwargs: GetDevicePositionRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
    "DeviceId": ...,
}

parent.get_device_position(**kwargs)
```

1. See [:material-code-braces: GetDevicePositionRequestRequestTypeDef](./type_defs.md#getdevicepositionrequestrequesttypedef) 

### get\_device\_position\_history

Retrieves the device position history from a tracker resource within a
specified range of
time.

Type annotations and code completion for `#!python session.create_client("location").get_device_position_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_device_position_history)

```python
# get_device_position_history method definition

await def get_device_position_history(
    self,
    *,
    TrackerName: str,
    DeviceId: str,
    NextToken: str = ...,
    StartTimeInclusive: TimestampTypeDef = ...,
    EndTimeExclusive: TimestampTypeDef = ...,
    MaxResults: int = ...,
) -> GetDevicePositionHistoryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDevicePositionHistoryResponseTypeDef](./type_defs.md#getdevicepositionhistoryresponsetypedef) 


```python
# get_device_position_history method usage example with argument unpacking

kwargs: GetDevicePositionHistoryRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
    "DeviceId": ...,
}

parent.get_device_position_history(**kwargs)
```

1. See [:material-code-braces: GetDevicePositionHistoryRequestRequestTypeDef](./type_defs.md#getdevicepositionhistoryrequestrequesttypedef) 

### get\_geofence

Retrieves the geofence details from a geofence collection.

Type annotations and code completion for `#!python session.create_client("location").get_geofence` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_geofence)

```python
# get_geofence method definition

await def get_geofence(
    self,
    *,
    CollectionName: str,
    GeofenceId: str,
) -> GetGeofenceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGeofenceResponseTypeDef](./type_defs.md#getgeofenceresponsetypedef) 


```python
# get_geofence method usage example with argument unpacking

kwargs: GetGeofenceRequestRequestTypeDef = {  # (1)
    "CollectionName": ...,
    "GeofenceId": ...,
}

parent.get_geofence(**kwargs)
```

1. See [:material-code-braces: GetGeofenceRequestRequestTypeDef](./type_defs.md#getgeofencerequestrequesttypedef) 

### get\_map\_glyphs

Retrieves glyphs used to display labels on a map.

Type annotations and code completion for `#!python session.create_client("location").get_map_glyphs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_map_glyphs)

```python
# get_map_glyphs method definition

await def get_map_glyphs(
    self,
    *,
    MapName: str,
    FontStack: str,
    FontUnicodeRange: str,
    Key: str = ...,
) -> GetMapGlyphsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMapGlyphsResponseTypeDef](./type_defs.md#getmapglyphsresponsetypedef) 


```python
# get_map_glyphs method usage example with argument unpacking

kwargs: GetMapGlyphsRequestRequestTypeDef = {  # (1)
    "MapName": ...,
    "FontStack": ...,
    "FontUnicodeRange": ...,
}

parent.get_map_glyphs(**kwargs)
```

1. See [:material-code-braces: GetMapGlyphsRequestRequestTypeDef](./type_defs.md#getmapglyphsrequestrequesttypedef) 

### get\_map\_sprites

Retrieves the sprite sheet corresponding to a map resource.

Type annotations and code completion for `#!python session.create_client("location").get_map_sprites` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_map_sprites)

```python
# get_map_sprites method definition

await def get_map_sprites(
    self,
    *,
    MapName: str,
    FileName: str,
    Key: str = ...,
) -> GetMapSpritesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMapSpritesResponseTypeDef](./type_defs.md#getmapspritesresponsetypedef) 


```python
# get_map_sprites method usage example with argument unpacking

kwargs: GetMapSpritesRequestRequestTypeDef = {  # (1)
    "MapName": ...,
    "FileName": ...,
}

parent.get_map_sprites(**kwargs)
```

1. See [:material-code-braces: GetMapSpritesRequestRequestTypeDef](./type_defs.md#getmapspritesrequestrequesttypedef) 

### get\_map\_style\_descriptor

Retrieves the map style descriptor from a map resource.

Type annotations and code completion for `#!python session.create_client("location").get_map_style_descriptor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_map_style_descriptor)

```python
# get_map_style_descriptor method definition

await def get_map_style_descriptor(
    self,
    *,
    MapName: str,
    Key: str = ...,
) -> GetMapStyleDescriptorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMapStyleDescriptorResponseTypeDef](./type_defs.md#getmapstyledescriptorresponsetypedef) 


```python
# get_map_style_descriptor method usage example with argument unpacking

kwargs: GetMapStyleDescriptorRequestRequestTypeDef = {  # (1)
    "MapName": ...,
}

parent.get_map_style_descriptor(**kwargs)
```

1. See [:material-code-braces: GetMapStyleDescriptorRequestRequestTypeDef](./type_defs.md#getmapstyledescriptorrequestrequesttypedef) 

### get\_map\_tile

Retrieves a vector data tile from the map resource.

Type annotations and code completion for `#!python session.create_client("location").get_map_tile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_map_tile)

```python
# get_map_tile method definition

await def get_map_tile(
    self,
    *,
    MapName: str,
    Z: str,
    X: str,
    Y: str,
    Key: str = ...,
) -> GetMapTileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMapTileResponseTypeDef](./type_defs.md#getmaptileresponsetypedef) 


```python
# get_map_tile method usage example with argument unpacking

kwargs: GetMapTileRequestRequestTypeDef = {  # (1)
    "MapName": ...,
    "Z": ...,
    "X": ...,
    "Y": ...,
}

parent.get_map_tile(**kwargs)
```

1. See [:material-code-braces: GetMapTileRequestRequestTypeDef](./type_defs.md#getmaptilerequestrequesttypedef) 

### get\_place

Finds a place by its unique ID.

Type annotations and code completion for `#!python session.create_client("location").get_place` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_place)

```python
# get_place method definition

await def get_place(
    self,
    *,
    IndexName: str,
    PlaceId: str,
    Language: str = ...,
    Key: str = ...,
) -> GetPlaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPlaceResponseTypeDef](./type_defs.md#getplaceresponsetypedef) 


```python
# get_place method usage example with argument unpacking

kwargs: GetPlaceRequestRequestTypeDef = {  # (1)
    "IndexName": ...,
    "PlaceId": ...,
}

parent.get_place(**kwargs)
```

1. See [:material-code-braces: GetPlaceRequestRequestTypeDef](./type_defs.md#getplacerequestrequesttypedef) 

### list\_device\_positions

A batch request to retrieve all device positions.

Type annotations and code completion for `#!python session.create_client("location").list_device_positions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_device_positions)

```python
# list_device_positions method definition

await def list_device_positions(
    self,
    *,
    TrackerName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    FilterGeometry: TrackingFilterGeometryTypeDef = ...,  # (1)
) -> ListDevicePositionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TrackingFilterGeometryTypeDef](./type_defs.md#trackingfiltergeometrytypedef) 
2. See [:material-code-braces: ListDevicePositionsResponseTypeDef](./type_defs.md#listdevicepositionsresponsetypedef) 


```python
# list_device_positions method usage example with argument unpacking

kwargs: ListDevicePositionsRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.list_device_positions(**kwargs)
```

1. See [:material-code-braces: ListDevicePositionsRequestRequestTypeDef](./type_defs.md#listdevicepositionsrequestrequesttypedef) 

### list\_geofence\_collections

Lists geofence collections in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").list_geofence_collections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_geofence_collections)

```python
# list_geofence_collections method definition

await def list_geofence_collections(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListGeofenceCollectionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGeofenceCollectionsResponseTypeDef](./type_defs.md#listgeofencecollectionsresponsetypedef) 


```python
# list_geofence_collections method usage example with argument unpacking

kwargs: ListGeofenceCollectionsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_geofence_collections(**kwargs)
```

1. See [:material-code-braces: ListGeofenceCollectionsRequestRequestTypeDef](./type_defs.md#listgeofencecollectionsrequestrequesttypedef) 

### list\_geofences

Lists geofences stored in a given geofence collection.

Type annotations and code completion for `#!python session.create_client("location").list_geofences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_geofences)

```python
# list_geofences method definition

await def list_geofences(
    self,
    *,
    CollectionName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListGeofencesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGeofencesResponseTypeDef](./type_defs.md#listgeofencesresponsetypedef) 


```python
# list_geofences method usage example with argument unpacking

kwargs: ListGeofencesRequestRequestTypeDef = {  # (1)
    "CollectionName": ...,
}

parent.list_geofences(**kwargs)
```

1. See [:material-code-braces: ListGeofencesRequestRequestTypeDef](./type_defs.md#listgeofencesrequestrequesttypedef) 

### list\_keys

Lists API key resources in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").list_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_keys)

```python
# list_keys method definition

await def list_keys(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filter: ApiKeyFilterTypeDef = ...,  # (1)
) -> ListKeysResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ApiKeyFilterTypeDef](./type_defs.md#apikeyfiltertypedef) 
2. See [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 


```python
# list_keys method usage example with argument unpacking

kwargs: ListKeysRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_keys(**kwargs)
```

1. See [:material-code-braces: ListKeysRequestRequestTypeDef](./type_defs.md#listkeysrequestrequesttypedef) 

### list\_maps

Lists map resources in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").list_maps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_maps)

```python
# list_maps method definition

await def list_maps(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListMapsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMapsResponseTypeDef](./type_defs.md#listmapsresponsetypedef) 


```python
# list_maps method usage example with argument unpacking

kwargs: ListMapsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_maps(**kwargs)
```

1. See [:material-code-braces: ListMapsRequestRequestTypeDef](./type_defs.md#listmapsrequestrequesttypedef) 

### list\_place\_indexes

Lists place index resources in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").list_place_indexes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_place_indexes)

```python
# list_place_indexes method definition

await def list_place_indexes(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPlaceIndexesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPlaceIndexesResponseTypeDef](./type_defs.md#listplaceindexesresponsetypedef) 


```python
# list_place_indexes method usage example with argument unpacking

kwargs: ListPlaceIndexesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_place_indexes(**kwargs)
```

1. See [:material-code-braces: ListPlaceIndexesRequestRequestTypeDef](./type_defs.md#listplaceindexesrequestrequesttypedef) 

### list\_route\_calculators

Lists route calculator resources in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").list_route_calculators` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_route_calculators)

```python
# list_route_calculators method definition

await def list_route_calculators(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRouteCalculatorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRouteCalculatorsResponseTypeDef](./type_defs.md#listroutecalculatorsresponsetypedef) 


```python
# list_route_calculators method usage example with argument unpacking

kwargs: ListRouteCalculatorsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_route_calculators(**kwargs)
```

1. See [:material-code-braces: ListRouteCalculatorsRequestRequestTypeDef](./type_defs.md#listroutecalculatorsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags that are applied to the specified Amazon Location
resource.

Type annotations and code completion for `#!python session.create_client("location").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_tracker\_consumers

Lists geofence collections currently associated to the given tracker resource.

Type annotations and code completion for `#!python session.create_client("location").list_tracker_consumers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_tracker_consumers)

```python
# list_tracker_consumers method definition

await def list_tracker_consumers(
    self,
    *,
    TrackerName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTrackerConsumersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrackerConsumersResponseTypeDef](./type_defs.md#listtrackerconsumersresponsetypedef) 


```python
# list_tracker_consumers method usage example with argument unpacking

kwargs: ListTrackerConsumersRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.list_tracker_consumers(**kwargs)
```

1. See [:material-code-braces: ListTrackerConsumersRequestRequestTypeDef](./type_defs.md#listtrackerconsumersrequestrequesttypedef) 

### list\_trackers

Lists tracker resources in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("location").list_trackers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_trackers)

```python
# list_trackers method definition

await def list_trackers(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTrackersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrackersResponseTypeDef](./type_defs.md#listtrackersresponsetypedef) 


```python
# list_trackers method usage example with argument unpacking

kwargs: ListTrackersRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_trackers(**kwargs)
```

1. See [:material-code-braces: ListTrackersRequestRequestTypeDef](./type_defs.md#listtrackersrequestrequesttypedef) 

### put\_geofence

Stores a geofence geometry in a given geofence collection, or updates the
geometry of an existing geofence if a geofence ID is included in the
request.

Type annotations and code completion for `#!python session.create_client("location").put_geofence` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)

```python
# put_geofence method definition

await def put_geofence(
    self,
    *,
    CollectionName: str,
    GeofenceId: str,
    Geometry: GeofenceGeometryTypeDef,  # (1)
    GeofenceProperties: Mapping[str, str] = ...,
) -> PutGeofenceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GeofenceGeometryTypeDef](./type_defs.md#geofencegeometrytypedef) 
2. See [:material-code-braces: PutGeofenceResponseTypeDef](./type_defs.md#putgeofenceresponsetypedef) 


```python
# put_geofence method usage example with argument unpacking

kwargs: PutGeofenceRequestRequestTypeDef = {  # (1)
    "CollectionName": ...,
    "GeofenceId": ...,
    "Geometry": ...,
}

parent.put_geofence(**kwargs)
```

1. See [:material-code-braces: PutGeofenceRequestRequestTypeDef](./type_defs.md#putgeofencerequestrequesttypedef) 

### search\_place\_index\_for\_position

Reverse geocodes a given coordinate and returns a legible address.

Type annotations and code completion for `#!python session.create_client("location").search_place_index_for_position` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_position)

```python
# search_place_index_for_position method definition

await def search_place_index_for_position(
    self,
    *,
    IndexName: str,
    Position: Sequence[float],
    MaxResults: int = ...,
    Language: str = ...,
    Key: str = ...,
) -> SearchPlaceIndexForPositionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SearchPlaceIndexForPositionResponseTypeDef](./type_defs.md#searchplaceindexforpositionresponsetypedef) 


```python
# search_place_index_for_position method usage example with argument unpacking

kwargs: SearchPlaceIndexForPositionRequestRequestTypeDef = {  # (1)
    "IndexName": ...,
    "Position": ...,
}

parent.search_place_index_for_position(**kwargs)
```

1. See [:material-code-braces: SearchPlaceIndexForPositionRequestRequestTypeDef](./type_defs.md#searchplaceindexforpositionrequestrequesttypedef) 

### search\_place\_index\_for\_suggestions

Generates suggestions for addresses and points of interest based on partial or
misspelled free-form
text.

Type annotations and code completion for `#!python session.create_client("location").search_place_index_for_suggestions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_suggestions)

```python
# search_place_index_for_suggestions method definition

await def search_place_index_for_suggestions(
    self,
    *,
    IndexName: str,
    Text: str,
    BiasPosition: Sequence[float] = ...,
    FilterBBox: Sequence[float] = ...,
    FilterCountries: Sequence[str] = ...,
    MaxResults: int = ...,
    Language: str = ...,
    FilterCategories: Sequence[str] = ...,
    Key: str = ...,
) -> SearchPlaceIndexForSuggestionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SearchPlaceIndexForSuggestionsResponseTypeDef](./type_defs.md#searchplaceindexforsuggestionsresponsetypedef) 


```python
# search_place_index_for_suggestions method usage example with argument unpacking

kwargs: SearchPlaceIndexForSuggestionsRequestRequestTypeDef = {  # (1)
    "IndexName": ...,
    "Text": ...,
}

parent.search_place_index_for_suggestions(**kwargs)
```

1. See [:material-code-braces: SearchPlaceIndexForSuggestionsRequestRequestTypeDef](./type_defs.md#searchplaceindexforsuggestionsrequestrequesttypedef) 

### search\_place\_index\_for\_text

Geocodes free-form text, such as an address, name, city, or region to allow you
to search for Places or points of
interest.

Type annotations and code completion for `#!python session.create_client("location").search_place_index_for_text` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_text)

```python
# search_place_index_for_text method definition

await def search_place_index_for_text(
    self,
    *,
    IndexName: str,
    Text: str,
    BiasPosition: Sequence[float] = ...,
    FilterBBox: Sequence[float] = ...,
    FilterCountries: Sequence[str] = ...,
    MaxResults: int = ...,
    Language: str = ...,
    FilterCategories: Sequence[str] = ...,
    Key: str = ...,
) -> SearchPlaceIndexForTextResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SearchPlaceIndexForTextResponseTypeDef](./type_defs.md#searchplaceindexfortextresponsetypedef) 


```python
# search_place_index_for_text method usage example with argument unpacking

kwargs: SearchPlaceIndexForTextRequestRequestTypeDef = {  # (1)
    "IndexName": ...,
    "Text": ...,
}

parent.search_place_index_for_text(**kwargs)
```

1. See [:material-code-braces: SearchPlaceIndexForTextRequestRequestTypeDef](./type_defs.md#searchplaceindexfortextrequestrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified Amazon Location
Service
resource.

Type annotations and code completion for `#!python session.create_client("location").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes one or more tags from the specified Amazon Location resource.

Type annotations and code completion for `#!python session.create_client("location").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_geofence\_collection

Updates the specified properties of a given geofence collection.

Type annotations and code completion for `#!python session.create_client("location").update_geofence_collection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_geofence_collection)

```python
# update_geofence_collection method definition

await def update_geofence_collection(
    self,
    *,
    CollectionName: str,
    PricingPlan: PricingPlanType = ...,  # (1)
    PricingPlanDataSource: str = ...,
    Description: str = ...,
) -> UpdateGeofenceCollectionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: UpdateGeofenceCollectionResponseTypeDef](./type_defs.md#updategeofencecollectionresponsetypedef) 


```python
# update_geofence_collection method usage example with argument unpacking

kwargs: UpdateGeofenceCollectionRequestRequestTypeDef = {  # (1)
    "CollectionName": ...,
}

parent.update_geofence_collection(**kwargs)
```

1. See [:material-code-braces: UpdateGeofenceCollectionRequestRequestTypeDef](./type_defs.md#updategeofencecollectionrequestrequesttypedef) 

### update\_key

Updates the specified properties of a given API key resource.

Type annotations and code completion for `#!python session.create_client("location").update_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)

```python
# update_key method definition

await def update_key(
    self,
    *,
    KeyName: str,
    Description: str = ...,
    ExpireTime: TimestampTypeDef = ...,
    NoExpiry: bool = ...,
    ForceUpdate: bool = ...,
    Restrictions: ApiKeyRestrictionsTypeDef = ...,  # (1)
) -> UpdateKeyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ApiKeyRestrictionsTypeDef](./type_defs.md#apikeyrestrictionstypedef) 
2. See [:material-code-braces: UpdateKeyResponseTypeDef](./type_defs.md#updatekeyresponsetypedef) 


```python
# update_key method usage example with argument unpacking

kwargs: UpdateKeyRequestRequestTypeDef = {  # (1)
    "KeyName": ...,
}

parent.update_key(**kwargs)
```

1. See [:material-code-braces: UpdateKeyRequestRequestTypeDef](./type_defs.md#updatekeyrequestrequesttypedef) 

### update\_map

Updates the specified properties of a given map resource.

Type annotations and code completion for `#!python session.create_client("location").update_map` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_map)

```python
# update_map method definition

await def update_map(
    self,
    *,
    MapName: str,
    PricingPlan: PricingPlanType = ...,  # (1)
    Description: str = ...,
    ConfigurationUpdate: MapConfigurationUpdateTypeDef = ...,  # (2)
) -> UpdateMapResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: MapConfigurationUpdateTypeDef](./type_defs.md#mapconfigurationupdatetypedef) 
3. See [:material-code-braces: UpdateMapResponseTypeDef](./type_defs.md#updatemapresponsetypedef) 


```python
# update_map method usage example with argument unpacking

kwargs: UpdateMapRequestRequestTypeDef = {  # (1)
    "MapName": ...,
}

parent.update_map(**kwargs)
```

1. See [:material-code-braces: UpdateMapRequestRequestTypeDef](./type_defs.md#updatemaprequestrequesttypedef) 

### update\_place\_index

Updates the specified properties of a given place index resource.

Type annotations and code completion for `#!python session.create_client("location").update_place_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_place_index)

```python
# update_place_index method definition

await def update_place_index(
    self,
    *,
    IndexName: str,
    PricingPlan: PricingPlanType = ...,  # (1)
    Description: str = ...,
    DataSourceConfiguration: DataSourceConfigurationTypeDef = ...,  # (2)
) -> UpdatePlaceIndexResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
3. See [:material-code-braces: UpdatePlaceIndexResponseTypeDef](./type_defs.md#updateplaceindexresponsetypedef) 


```python
# update_place_index method usage example with argument unpacking

kwargs: UpdatePlaceIndexRequestRequestTypeDef = {  # (1)
    "IndexName": ...,
}

parent.update_place_index(**kwargs)
```

1. See [:material-code-braces: UpdatePlaceIndexRequestRequestTypeDef](./type_defs.md#updateplaceindexrequestrequesttypedef) 

### update\_route\_calculator

Updates the specified properties for a given route calculator resource.

Type annotations and code completion for `#!python session.create_client("location").update_route_calculator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_route_calculator)

```python
# update_route_calculator method definition

await def update_route_calculator(
    self,
    *,
    CalculatorName: str,
    PricingPlan: PricingPlanType = ...,  # (1)
    Description: str = ...,
) -> UpdateRouteCalculatorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: UpdateRouteCalculatorResponseTypeDef](./type_defs.md#updateroutecalculatorresponsetypedef) 


```python
# update_route_calculator method usage example with argument unpacking

kwargs: UpdateRouteCalculatorRequestRequestTypeDef = {  # (1)
    "CalculatorName": ...,
}

parent.update_route_calculator(**kwargs)
```

1. See [:material-code-braces: UpdateRouteCalculatorRequestRequestTypeDef](./type_defs.md#updateroutecalculatorrequestrequesttypedef) 

### update\_tracker

Updates the specified properties of a given tracker resource.

Type annotations and code completion for `#!python session.create_client("location").update_tracker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_tracker)

```python
# update_tracker method definition

await def update_tracker(
    self,
    *,
    TrackerName: str,
    PricingPlan: PricingPlanType = ...,  # (1)
    PricingPlanDataSource: str = ...,
    Description: str = ...,
    PositionFiltering: PositionFilteringType = ...,  # (2)
    EventBridgeEnabled: bool = ...,
    KmsKeyEnableGeospatialQueries: bool = ...,
) -> UpdateTrackerResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-brackets: PositionFilteringType](./literals.md#positionfilteringtype) 
3. See [:material-code-braces: UpdateTrackerResponseTypeDef](./type_defs.md#updatetrackerresponsetypedef) 


```python
# update_tracker method usage example with argument unpacking

kwargs: UpdateTrackerRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
}

parent.update_tracker(**kwargs)
```

1. See [:material-code-braces: UpdateTrackerRequestRequestTypeDef](./type_defs.md#updatetrackerrequestrequesttypedef) 

### verify\_device\_position

Verifies the integrity of the device's position by determining if it was
reported behind a proxy, and by comparing it to an inferred position estimated
based on the device's
state.

Type annotations and code completion for `#!python session.create_client("location").verify_device_position` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.verify_device_position)

```python
# verify_device_position method definition

await def verify_device_position(
    self,
    *,
    TrackerName: str,
    DeviceState: DeviceStateTypeDef,  # (1)
    DistanceUnit: DistanceUnitType = ...,  # (2)
) -> VerifyDevicePositionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DeviceStateTypeDef](./type_defs.md#devicestatetypedef) 
2. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
3. See [:material-code-braces: VerifyDevicePositionResponseTypeDef](./type_defs.md#verifydevicepositionresponsetypedef) 


```python
# verify_device_position method usage example with argument unpacking

kwargs: VerifyDevicePositionRequestRequestTypeDef = {  # (1)
    "TrackerName": ...,
    "DeviceState": ...,
}

parent.verify_device_position(**kwargs)
```

1. See [:material-code-braces: VerifyDevicePositionRequestRequestTypeDef](./type_defs.md#verifydevicepositionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("location").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "LocationServiceClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("location").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("location").get_paginator` method with overloads.

- `client.get_paginator("forecast_geofence_events")` -> [ForecastGeofenceEventsPaginator](./paginators.md#forecastgeofenceeventspaginator)
- `client.get_paginator("get_device_position_history")` -> [GetDevicePositionHistoryPaginator](./paginators.md#getdevicepositionhistorypaginator)
- `client.get_paginator("list_device_positions")` -> [ListDevicePositionsPaginator](./paginators.md#listdevicepositionspaginator)
- `client.get_paginator("list_geofence_collections")` -> [ListGeofenceCollectionsPaginator](./paginators.md#listgeofencecollectionspaginator)
- `client.get_paginator("list_geofences")` -> [ListGeofencesPaginator](./paginators.md#listgeofencespaginator)
- `client.get_paginator("list_keys")` -> [ListKeysPaginator](./paginators.md#listkeyspaginator)
- `client.get_paginator("list_maps")` -> [ListMapsPaginator](./paginators.md#listmapspaginator)
- `client.get_paginator("list_place_indexes")` -> [ListPlaceIndexesPaginator](./paginators.md#listplaceindexespaginator)
- `client.get_paginator("list_route_calculators")` -> [ListRouteCalculatorsPaginator](./paginators.md#listroutecalculatorspaginator)
- `client.get_paginator("list_tracker_consumers")` -> [ListTrackerConsumersPaginator](./paginators.md#listtrackerconsumerspaginator)
- `client.get_paginator("list_trackers")` -> [ListTrackersPaginator](./paginators.md#listtrackerspaginator)



