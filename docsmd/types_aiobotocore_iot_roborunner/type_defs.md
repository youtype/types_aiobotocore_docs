# Type definitions

> [Index](../README.md) > [IoTRoboRunner](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTRoboRunner](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
    type annotations stubs module [types-aiobotocore-iot-roborunner](https://pypi.org/project/types-aiobotocore-iot-roborunner/).



## CartesianCoordinatesTypeDef

```python
# CartesianCoordinatesTypeDef definition

class CartesianCoordinatesTypeDef(TypedDict):
    x: float,
    y: float,
    z: NotRequired[float],
```

## CreateDestinationRequestRequestTypeDef

```python
# CreateDestinationRequestRequestTypeDef definition

class CreateDestinationRequestRequestTypeDef(TypedDict):
    name: str,
    site: str,
    clientToken: NotRequired[str],
    state: NotRequired[DestinationStateType],  # (1)
    additionalFixedProperties: NotRequired[str],
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
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

## CreateSiteRequestRequestTypeDef

```python
# CreateSiteRequestRequestTypeDef definition

class CreateSiteRequestRequestTypeDef(TypedDict):
    name: str,
    countryCode: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## CreateWorkerFleetRequestRequestTypeDef

```python
# CreateWorkerFleetRequestRequestTypeDef definition

class CreateWorkerFleetRequestRequestTypeDef(TypedDict):
    name: str,
    site: str,
    clientToken: NotRequired[str],
    additionalFixedProperties: NotRequired[str],
```

## OrientationTypeDef

```python
# OrientationTypeDef definition

class OrientationTypeDef(TypedDict):
    degrees: NotRequired[float],
```

## VendorPropertiesTypeDef

```python
# VendorPropertiesTypeDef definition

class VendorPropertiesTypeDef(TypedDict):
    vendorWorkerId: str,
    vendorWorkerIpAddress: NotRequired[str],
    vendorAdditionalTransientProperties: NotRequired[str],
    vendorAdditionalFixedProperties: NotRequired[str],
```

## DeleteDestinationRequestRequestTypeDef

```python
# DeleteDestinationRequestRequestTypeDef definition

class DeleteDestinationRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteSiteRequestRequestTypeDef

```python
# DeleteSiteRequestRequestTypeDef definition

class DeleteSiteRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteWorkerFleetRequestRequestTypeDef

```python
# DeleteWorkerFleetRequestRequestTypeDef definition

class DeleteWorkerFleetRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteWorkerRequestRequestTypeDef

```python
# DeleteWorkerRequestRequestTypeDef definition

class DeleteWorkerRequestRequestTypeDef(TypedDict):
    id: str,
```

## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    site: str,
    createdAt: datetime,
    updatedAt: datetime,
    state: DestinationStateType,  # (1)
    additionalFixedProperties: NotRequired[str],
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
## GetDestinationRequestRequestTypeDef

```python
# GetDestinationRequestRequestTypeDef definition

class GetDestinationRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetSiteRequestRequestTypeDef

```python
# GetSiteRequestRequestTypeDef definition

class GetSiteRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetWorkerFleetRequestRequestTypeDef

```python
# GetWorkerFleetRequestRequestTypeDef definition

class GetWorkerFleetRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetWorkerRequestRequestTypeDef

```python
# GetWorkerRequestRequestTypeDef definition

class GetWorkerRequestRequestTypeDef(TypedDict):
    id: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDestinationsRequestRequestTypeDef

```python
# ListDestinationsRequestRequestTypeDef definition

class ListDestinationsRequestRequestTypeDef(TypedDict):
    site: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    state: NotRequired[DestinationStateType],  # (1)
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
## ListSitesRequestRequestTypeDef

```python
# ListSitesRequestRequestTypeDef definition

class ListSitesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## SiteTypeDef

```python
# SiteTypeDef definition

class SiteTypeDef(TypedDict):
    arn: str,
    name: str,
    countryCode: str,
    createdAt: datetime,
```

## ListWorkerFleetsRequestRequestTypeDef

```python
# ListWorkerFleetsRequestRequestTypeDef definition

class ListWorkerFleetsRequestRequestTypeDef(TypedDict):
    site: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## WorkerFleetTypeDef

```python
# WorkerFleetTypeDef definition

class WorkerFleetTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    site: str,
    createdAt: datetime,
    updatedAt: datetime,
    additionalFixedProperties: NotRequired[str],
```

## ListWorkersRequestRequestTypeDef

```python
# ListWorkersRequestRequestTypeDef definition

class ListWorkersRequestRequestTypeDef(TypedDict):
    site: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    fleet: NotRequired[str],
```

## UpdateDestinationRequestRequestTypeDef

```python
# UpdateDestinationRequestRequestTypeDef definition

class UpdateDestinationRequestRequestTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    state: NotRequired[DestinationStateType],  # (1)
    additionalFixedProperties: NotRequired[str],
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
## UpdateSiteRequestRequestTypeDef

```python
# UpdateSiteRequestRequestTypeDef definition

class UpdateSiteRequestRequestTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    countryCode: NotRequired[str],
    description: NotRequired[str],
```

## UpdateWorkerFleetRequestRequestTypeDef

```python
# UpdateWorkerFleetRequestRequestTypeDef definition

class UpdateWorkerFleetRequestRequestTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    additionalFixedProperties: NotRequired[str],
```

## PositionCoordinatesTypeDef

```python
# PositionCoordinatesTypeDef definition

class PositionCoordinatesTypeDef(TypedDict):
    cartesianCoordinates: NotRequired[CartesianCoordinatesTypeDef],  # (1)
```

1. See [:material-code-braces: CartesianCoordinatesTypeDef](./type_defs.md#cartesiancoordinatestypedef) 
## CreateDestinationResponseTypeDef

```python
# CreateDestinationResponseTypeDef definition

class CreateDestinationResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    createdAt: datetime,
    updatedAt: datetime,
    state: DestinationStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSiteResponseTypeDef

```python
# CreateSiteResponseTypeDef definition

class CreateSiteResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    createdAt: datetime,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkerFleetResponseTypeDef

```python
# CreateWorkerFleetResponseTypeDef definition

class CreateWorkerFleetResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    createdAt: datetime,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkerResponseTypeDef

```python
# CreateWorkerResponseTypeDef definition

class CreateWorkerResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    createdAt: datetime,
    updatedAt: datetime,
    site: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDestinationResponseTypeDef

```python
# GetDestinationResponseTypeDef definition

class GetDestinationResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    site: str,
    createdAt: datetime,
    updatedAt: datetime,
    state: DestinationStateType,  # (1)
    additionalFixedProperties: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSiteResponseTypeDef

```python
# GetSiteResponseTypeDef definition

class GetSiteResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    countryCode: str,
    description: str,
    createdAt: datetime,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkerFleetResponseTypeDef

```python
# GetWorkerFleetResponseTypeDef definition

class GetWorkerFleetResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    site: str,
    createdAt: datetime,
    updatedAt: datetime,
    additionalFixedProperties: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDestinationResponseTypeDef

```python
# UpdateDestinationResponseTypeDef definition

class UpdateDestinationResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    updatedAt: datetime,
    state: DestinationStateType,  # (1)
    additionalFixedProperties: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSiteResponseTypeDef

```python
# UpdateSiteResponseTypeDef definition

class UpdateSiteResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    countryCode: str,
    description: str,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkerFleetResponseTypeDef

```python
# UpdateWorkerFleetResponseTypeDef definition

class UpdateWorkerFleetResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    updatedAt: datetime,
    additionalFixedProperties: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDestinationsResponseTypeDef

```python
# ListDestinationsResponseTypeDef definition

class ListDestinationsResponseTypeDef(TypedDict):
    nextToken: str,
    destinations: List[DestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDestinationsRequestListDestinationsPaginateTypeDef

```python
# ListDestinationsRequestListDestinationsPaginateTypeDef definition

class ListDestinationsRequestListDestinationsPaginateTypeDef(TypedDict):
    site: str,
    state: NotRequired[DestinationStateType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSitesRequestListSitesPaginateTypeDef

```python
# ListSitesRequestListSitesPaginateTypeDef definition

class ListSitesRequestListSitesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef

```python
# ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef definition

class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(TypedDict):
    site: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkersRequestListWorkersPaginateTypeDef

```python
# ListWorkersRequestListWorkersPaginateTypeDef definition

class ListWorkersRequestListWorkersPaginateTypeDef(TypedDict):
    site: str,
    fleet: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSitesResponseTypeDef

```python
# ListSitesResponseTypeDef definition

class ListSitesResponseTypeDef(TypedDict):
    nextToken: str,
    sites: List[SiteTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SiteTypeDef](./type_defs.md#sitetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkerFleetsResponseTypeDef

```python
# ListWorkerFleetsResponseTypeDef definition

class ListWorkerFleetsResponseTypeDef(TypedDict):
    nextToken: str,
    workerFleets: List[WorkerFleetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkerFleetTypeDef](./type_defs.md#workerfleettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkerRequestRequestTypeDef

```python
# CreateWorkerRequestRequestTypeDef definition

class CreateWorkerRequestRequestTypeDef(TypedDict):
    name: str,
    fleet: str,
    clientToken: NotRequired[str],
    additionalTransientProperties: NotRequired[str],
    additionalFixedProperties: NotRequired[str],
    vendorProperties: NotRequired[VendorPropertiesTypeDef],  # (1)
    position: NotRequired[PositionCoordinatesTypeDef],  # (2)
    orientation: NotRequired[OrientationTypeDef],  # (3)
```

1. See [:material-code-braces: VendorPropertiesTypeDef](./type_defs.md#vendorpropertiestypedef) 
2. See [:material-code-braces: PositionCoordinatesTypeDef](./type_defs.md#positioncoordinatestypedef) 
3. See [:material-code-braces: OrientationTypeDef](./type_defs.md#orientationtypedef) 
## GetWorkerResponseTypeDef

```python
# GetWorkerResponseTypeDef definition

class GetWorkerResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    fleet: str,
    site: str,
    createdAt: datetime,
    updatedAt: datetime,
    name: str,
    additionalTransientProperties: str,
    additionalFixedProperties: str,
    vendorProperties: VendorPropertiesTypeDef,  # (1)
    position: PositionCoordinatesTypeDef,  # (2)
    orientation: OrientationTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: VendorPropertiesTypeDef](./type_defs.md#vendorpropertiestypedef) 
2. See [:material-code-braces: PositionCoordinatesTypeDef](./type_defs.md#positioncoordinatestypedef) 
3. See [:material-code-braces: OrientationTypeDef](./type_defs.md#orientationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkerRequestRequestTypeDef

```python
# UpdateWorkerRequestRequestTypeDef definition

class UpdateWorkerRequestRequestTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    additionalTransientProperties: NotRequired[str],
    additionalFixedProperties: NotRequired[str],
    vendorProperties: NotRequired[VendorPropertiesTypeDef],  # (1)
    position: NotRequired[PositionCoordinatesTypeDef],  # (2)
    orientation: NotRequired[OrientationTypeDef],  # (3)
```

1. See [:material-code-braces: VendorPropertiesTypeDef](./type_defs.md#vendorpropertiestypedef) 
2. See [:material-code-braces: PositionCoordinatesTypeDef](./type_defs.md#positioncoordinatestypedef) 
3. See [:material-code-braces: OrientationTypeDef](./type_defs.md#orientationtypedef) 
## UpdateWorkerResponseTypeDef

```python
# UpdateWorkerResponseTypeDef definition

class UpdateWorkerResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    fleet: str,
    updatedAt: datetime,
    name: str,
    additionalTransientProperties: str,
    additionalFixedProperties: str,
    orientation: OrientationTypeDef,  # (1)
    vendorProperties: VendorPropertiesTypeDef,  # (2)
    position: PositionCoordinatesTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: OrientationTypeDef](./type_defs.md#orientationtypedef) 
2. See [:material-code-braces: VendorPropertiesTypeDef](./type_defs.md#vendorpropertiestypedef) 
3. See [:material-code-braces: PositionCoordinatesTypeDef](./type_defs.md#positioncoordinatestypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkerTypeDef

```python
# WorkerTypeDef definition

class WorkerTypeDef(TypedDict):
    arn: str,
    id: str,
    fleet: str,
    createdAt: datetime,
    updatedAt: datetime,
    name: str,
    site: str,
    additionalTransientProperties: NotRequired[str],
    additionalFixedProperties: NotRequired[str],
    vendorProperties: NotRequired[VendorPropertiesTypeDef],  # (1)
    position: NotRequired[PositionCoordinatesTypeDef],  # (2)
    orientation: NotRequired[OrientationTypeDef],  # (3)
```

1. See [:material-code-braces: VendorPropertiesTypeDef](./type_defs.md#vendorpropertiestypedef) 
2. See [:material-code-braces: PositionCoordinatesTypeDef](./type_defs.md#positioncoordinatestypedef) 
3. See [:material-code-braces: OrientationTypeDef](./type_defs.md#orientationtypedef) 
## ListWorkersResponseTypeDef

```python
# ListWorkersResponseTypeDef definition

class ListWorkersResponseTypeDef(TypedDict):
    nextToken: str,
    workers: List[WorkerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkerTypeDef](./type_defs.md#workertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
