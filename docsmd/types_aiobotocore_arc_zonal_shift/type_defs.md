# Type definitions

> [Index](../README.md) > [ARCZonalShift](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ARCZonalShift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
    type annotations stubs module [types-aiobotocore-arc-zonal-shift](https://pypi.org/project/types-aiobotocore-arc-zonal-shift/).



## CancelZonalShiftRequestRequestTypeDef

```python
# CancelZonalShiftRequestRequestTypeDef definition

class CancelZonalShiftRequestRequestTypeDef(TypedDict):
    zonalShiftId: str,
```

## GetManagedResourceRequestRequestTypeDef

```python
# GetManagedResourceRequestRequestTypeDef definition

class GetManagedResourceRequestRequestTypeDef(TypedDict):
    resourceIdentifier: str,
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

## ZonalShiftInResourceTypeDef

```python
# ZonalShiftInResourceTypeDef definition

class ZonalShiftInResourceTypeDef(TypedDict):
    appliedStatus: AppliedStatusType,  # (1)
    awayFrom: str,
    comment: str,
    expiryTime: datetime,
    resourceIdentifier: str,
    startTime: datetime,
    zonalShiftId: str,
```

1. See [:material-code-brackets: AppliedStatusType](./literals.md#appliedstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListManagedResourcesRequestRequestTypeDef

```python
# ListManagedResourcesRequestRequestTypeDef definition

class ListManagedResourcesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ManagedResourceSummaryTypeDef

```python
# ManagedResourceSummaryTypeDef definition

class ManagedResourceSummaryTypeDef(TypedDict):
    availabilityZones: List[str],
    arn: NotRequired[str],
    name: NotRequired[str],
```

## ListZonalShiftsRequestRequestTypeDef

```python
# ListZonalShiftsRequestRequestTypeDef definition

class ListZonalShiftsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[ZonalShiftStatusType],  # (1)
```

1. See [:material-code-brackets: ZonalShiftStatusType](./literals.md#zonalshiftstatustype) 
## ZonalShiftSummaryTypeDef

```python
# ZonalShiftSummaryTypeDef definition

class ZonalShiftSummaryTypeDef(TypedDict):
    awayFrom: str,
    comment: str,
    expiryTime: datetime,
    resourceIdentifier: str,
    startTime: datetime,
    status: ZonalShiftStatusType,  # (1)
    zonalShiftId: str,
```

1. See [:material-code-brackets: ZonalShiftStatusType](./literals.md#zonalshiftstatustype) 
## StartZonalShiftRequestRequestTypeDef

```python
# StartZonalShiftRequestRequestTypeDef definition

class StartZonalShiftRequestRequestTypeDef(TypedDict):
    awayFrom: str,
    comment: str,
    expiresIn: str,
    resourceIdentifier: str,
```

## UpdateZonalShiftRequestRequestTypeDef

```python
# UpdateZonalShiftRequestRequestTypeDef definition

class UpdateZonalShiftRequestRequestTypeDef(TypedDict):
    zonalShiftId: str,
    comment: NotRequired[str],
    expiresIn: NotRequired[str],
```

## ZonalShiftTypeDef

```python
# ZonalShiftTypeDef definition

class ZonalShiftTypeDef(TypedDict):
    awayFrom: str,
    comment: str,
    expiryTime: datetime,
    resourceIdentifier: str,
    startTime: datetime,
    status: ZonalShiftStatusType,  # (1)
    zonalShiftId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ZonalShiftStatusType](./literals.md#zonalshiftstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetManagedResourceResponseTypeDef

```python
# GetManagedResourceResponseTypeDef definition

class GetManagedResourceResponseTypeDef(TypedDict):
    appliedWeights: Dict[str, float],
    arn: str,
    name: str,
    zonalShifts: List[ZonalShiftInResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ZonalShiftInResourceTypeDef](./type_defs.md#zonalshiftinresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedResourcesRequestListManagedResourcesPaginateTypeDef

```python
# ListManagedResourcesRequestListManagedResourcesPaginateTypeDef definition

class ListManagedResourcesRequestListManagedResourcesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListZonalShiftsRequestListZonalShiftsPaginateTypeDef

```python
# ListZonalShiftsRequestListZonalShiftsPaginateTypeDef definition

class ListZonalShiftsRequestListZonalShiftsPaginateTypeDef(TypedDict):
    status: NotRequired[ZonalShiftStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ZonalShiftStatusType](./literals.md#zonalshiftstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedResourcesResponseTypeDef

```python
# ListManagedResourcesResponseTypeDef definition

class ListManagedResourcesResponseTypeDef(TypedDict):
    items: List[ManagedResourceSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedResourceSummaryTypeDef](./type_defs.md#managedresourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListZonalShiftsResponseTypeDef

```python
# ListZonalShiftsResponseTypeDef definition

class ListZonalShiftsResponseTypeDef(TypedDict):
    items: List[ZonalShiftSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ZonalShiftSummaryTypeDef](./type_defs.md#zonalshiftsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
