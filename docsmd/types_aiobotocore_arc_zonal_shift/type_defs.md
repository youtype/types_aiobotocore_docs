# Type definitions

> [Index](../README.md) > [ARCZonalShift](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ARCZonalShift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#arczonalshift)
    type annotations stubs module [types-aiobotocore-arc-zonal-shift](https://pypi.org/project/types-aiobotocore-arc-zonal-shift/).



## AutoshiftInResourceTypeDef

```python
# AutoshiftInResourceTypeDef definition

class AutoshiftInResourceTypeDef(TypedDict):
    appliedStatus: AutoshiftAppliedStatusType,  # (1)
    awayFrom: str,
    startTime: datetime,
```

1. See [:material-code-brackets: AutoshiftAppliedStatusType](./literals.md#autoshiftappliedstatustype) 
## AutoshiftSummaryTypeDef

```python
# AutoshiftSummaryTypeDef definition

class AutoshiftSummaryTypeDef(TypedDict):
    awayFrom: str,
    endTime: datetime,
    startTime: datetime,
    status: AutoshiftExecutionStatusType,  # (1)
```

1. See [:material-code-brackets: AutoshiftExecutionStatusType](./literals.md#autoshiftexecutionstatustype) 
## CancelZonalShiftRequestRequestTypeDef

```python
# CancelZonalShiftRequestRequestTypeDef definition

class CancelZonalShiftRequestRequestTypeDef(TypedDict):
    zonalShiftId: str,
```

## ControlConditionTypeDef

```python
# ControlConditionTypeDef definition

class ControlConditionTypeDef(TypedDict):
    alarmIdentifier: str,
    type: ControlConditionTypeType,  # (1)
```

1. See [:material-code-brackets: ControlConditionTypeType](./literals.md#controlconditiontypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DeletePracticeRunConfigurationRequestRequestTypeDef

```python
# DeletePracticeRunConfigurationRequestRequestTypeDef definition

class DeletePracticeRunConfigurationRequestRequestTypeDef(TypedDict):
    resourceIdentifier: str,
```

## GetManagedResourceRequestRequestTypeDef

```python
# GetManagedResourceRequestRequestTypeDef definition

class GetManagedResourceRequestRequestTypeDef(TypedDict):
    resourceIdentifier: str,
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
    practiceRunOutcome: NotRequired[PracticeRunOutcomeType],  # (2)
```

1. See [:material-code-brackets: AppliedStatusType](./literals.md#appliedstatustype) 
2. See [:material-code-brackets: PracticeRunOutcomeType](./literals.md#practicerunoutcometype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAutoshiftsRequestRequestTypeDef

```python
# ListAutoshiftsRequestRequestTypeDef definition

class ListAutoshiftsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[AutoshiftExecutionStatusType],  # (1)
```

1. See [:material-code-brackets: AutoshiftExecutionStatusType](./literals.md#autoshiftexecutionstatustype) 
## ListManagedResourcesRequestRequestTypeDef

```python
# ListManagedResourcesRequestRequestTypeDef definition

class ListManagedResourcesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListZonalShiftsRequestRequestTypeDef

```python
# ListZonalShiftsRequestRequestTypeDef definition

class ListZonalShiftsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    resourceIdentifier: NotRequired[str],
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
    status: ZonalShiftStatusType,  # (2)
    zonalShiftId: str,
    practiceRunOutcome: NotRequired[PracticeRunOutcomeType],  # (1)
```

1. See [:material-code-brackets: PracticeRunOutcomeType](./literals.md#practicerunoutcometype) 
2. See [:material-code-brackets: ZonalShiftStatusType](./literals.md#zonalshiftstatustype) 
## StartZonalShiftRequestRequestTypeDef

```python
# StartZonalShiftRequestRequestTypeDef definition

class StartZonalShiftRequestRequestTypeDef(TypedDict):
    awayFrom: str,
    comment: str,
    expiresIn: str,
    resourceIdentifier: str,
```

## UpdateAutoshiftObserverNotificationStatusRequestRequestTypeDef

```python
# UpdateAutoshiftObserverNotificationStatusRequestRequestTypeDef definition

class UpdateAutoshiftObserverNotificationStatusRequestRequestTypeDef(TypedDict):
    status: AutoshiftObserverNotificationStatusType,  # (1)
```

1. See [:material-code-brackets: AutoshiftObserverNotificationStatusType](./literals.md#autoshiftobservernotificationstatustype) 
## UpdateZonalAutoshiftConfigurationRequestRequestTypeDef

```python
# UpdateZonalAutoshiftConfigurationRequestRequestTypeDef definition

class UpdateZonalAutoshiftConfigurationRequestRequestTypeDef(TypedDict):
    resourceIdentifier: str,
    zonalAutoshiftStatus: ZonalAutoshiftStatusType,  # (1)
```

1. See [:material-code-brackets: ZonalAutoshiftStatusType](./literals.md#zonalautoshiftstatustype) 
## UpdateZonalShiftRequestRequestTypeDef

```python
# UpdateZonalShiftRequestRequestTypeDef definition

class UpdateZonalShiftRequestRequestTypeDef(TypedDict):
    zonalShiftId: str,
    comment: NotRequired[str],
    expiresIn: NotRequired[str],
```

## CreatePracticeRunConfigurationRequestRequestTypeDef

```python
# CreatePracticeRunConfigurationRequestRequestTypeDef definition

class CreatePracticeRunConfigurationRequestRequestTypeDef(TypedDict):
    outcomeAlarms: Sequence[ControlConditionTypeDef],  # (1)
    resourceIdentifier: str,
    blockedDates: NotRequired[Sequence[str]],
    blockedWindows: NotRequired[Sequence[str]],
    blockingAlarms: NotRequired[Sequence[ControlConditionTypeDef]],  # (1)
```

1. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
2. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
## PracticeRunConfigurationTypeDef

```python
# PracticeRunConfigurationTypeDef definition

class PracticeRunConfigurationTypeDef(TypedDict):
    outcomeAlarms: List[ControlConditionTypeDef],  # (1)
    blockedDates: NotRequired[List[str]],
    blockedWindows: NotRequired[List[str]],
    blockingAlarms: NotRequired[List[ControlConditionTypeDef]],  # (1)
```

1. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
2. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
## UpdatePracticeRunConfigurationRequestRequestTypeDef

```python
# UpdatePracticeRunConfigurationRequestRequestTypeDef definition

class UpdatePracticeRunConfigurationRequestRequestTypeDef(TypedDict):
    resourceIdentifier: str,
    blockedDates: NotRequired[Sequence[str]],
    blockedWindows: NotRequired[Sequence[str]],
    blockingAlarms: NotRequired[Sequence[ControlConditionTypeDef]],  # (1)
    outcomeAlarms: NotRequired[Sequence[ControlConditionTypeDef]],  # (1)
```

1. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
2. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
## DeletePracticeRunConfigurationResponseTypeDef

```python
# DeletePracticeRunConfigurationResponseTypeDef definition

class DeletePracticeRunConfigurationResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    zonalAutoshiftStatus: ZonalAutoshiftStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ZonalAutoshiftStatusType](./literals.md#zonalautoshiftstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAutoshiftObserverNotificationStatusResponseTypeDef

```python
# GetAutoshiftObserverNotificationStatusResponseTypeDef definition

class GetAutoshiftObserverNotificationStatusResponseTypeDef(TypedDict):
    status: AutoshiftObserverNotificationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AutoshiftObserverNotificationStatusType](./literals.md#autoshiftobservernotificationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAutoshiftsResponseTypeDef

```python
# ListAutoshiftsResponseTypeDef definition

class ListAutoshiftsResponseTypeDef(TypedDict):
    items: List[AutoshiftSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AutoshiftSummaryTypeDef](./type_defs.md#autoshiftsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAutoshiftObserverNotificationStatusResponseTypeDef

```python
# UpdateAutoshiftObserverNotificationStatusResponseTypeDef definition

class UpdateAutoshiftObserverNotificationStatusResponseTypeDef(TypedDict):
    status: AutoshiftObserverNotificationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AutoshiftObserverNotificationStatusType](./literals.md#autoshiftobservernotificationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateZonalAutoshiftConfigurationResponseTypeDef

```python
# UpdateZonalAutoshiftConfigurationResponseTypeDef definition

class UpdateZonalAutoshiftConfigurationResponseTypeDef(TypedDict):
    resourceIdentifier: str,
    zonalAutoshiftStatus: ZonalAutoshiftStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ZonalAutoshiftStatusType](./literals.md#zonalautoshiftstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## ManagedResourceSummaryTypeDef

```python
# ManagedResourceSummaryTypeDef definition

class ManagedResourceSummaryTypeDef(TypedDict):
    availabilityZones: List[str],
    appliedWeights: NotRequired[Dict[str, float]],
    arn: NotRequired[str],
    autoshifts: NotRequired[List[AutoshiftInResourceTypeDef]],  # (1)
    name: NotRequired[str],
    practiceRunStatus: NotRequired[ZonalAutoshiftStatusType],  # (2)
    zonalAutoshiftStatus: NotRequired[ZonalAutoshiftStatusType],  # (2)
    zonalShifts: NotRequired[List[ZonalShiftInResourceTypeDef]],  # (4)
```

1. See [:material-code-braces: AutoshiftInResourceTypeDef](./type_defs.md#autoshiftinresourcetypedef) 
2. See [:material-code-brackets: ZonalAutoshiftStatusType](./literals.md#zonalautoshiftstatustype) 
3. See [:material-code-brackets: ZonalAutoshiftStatusType](./literals.md#zonalautoshiftstatustype) 
4. See [:material-code-braces: ZonalShiftInResourceTypeDef](./type_defs.md#zonalshiftinresourcetypedef) 
## ListAutoshiftsRequestPaginateTypeDef

```python
# ListAutoshiftsRequestPaginateTypeDef definition

class ListAutoshiftsRequestPaginateTypeDef(TypedDict):
    status: NotRequired[AutoshiftExecutionStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AutoshiftExecutionStatusType](./literals.md#autoshiftexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedResourcesRequestPaginateTypeDef

```python
# ListManagedResourcesRequestPaginateTypeDef definition

class ListManagedResourcesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListZonalShiftsRequestPaginateTypeDef

```python
# ListZonalShiftsRequestPaginateTypeDef definition

class ListZonalShiftsRequestPaginateTypeDef(TypedDict):
    resourceIdentifier: NotRequired[str],
    status: NotRequired[ZonalShiftStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ZonalShiftStatusType](./literals.md#zonalshiftstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListZonalShiftsResponseTypeDef

```python
# ListZonalShiftsResponseTypeDef definition

class ListZonalShiftsResponseTypeDef(TypedDict):
    items: List[ZonalShiftSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ZonalShiftSummaryTypeDef](./type_defs.md#zonalshiftsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePracticeRunConfigurationResponseTypeDef

```python
# CreatePracticeRunConfigurationResponseTypeDef definition

class CreatePracticeRunConfigurationResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    practiceRunConfiguration: PracticeRunConfigurationTypeDef,  # (1)
    zonalAutoshiftStatus: ZonalAutoshiftStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PracticeRunConfigurationTypeDef](./type_defs.md#practicerunconfigurationtypedef) 
2. See [:material-code-brackets: ZonalAutoshiftStatusType](./literals.md#zonalautoshiftstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetManagedResourceResponseTypeDef

```python
# GetManagedResourceResponseTypeDef definition

class GetManagedResourceResponseTypeDef(TypedDict):
    appliedWeights: Dict[str, float],
    arn: str,
    autoshifts: List[AutoshiftInResourceTypeDef],  # (1)
    name: str,
    practiceRunConfiguration: PracticeRunConfigurationTypeDef,  # (2)
    zonalAutoshiftStatus: ZonalAutoshiftStatusType,  # (3)
    zonalShifts: List[ZonalShiftInResourceTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: AutoshiftInResourceTypeDef](./type_defs.md#autoshiftinresourcetypedef) 
2. See [:material-code-braces: PracticeRunConfigurationTypeDef](./type_defs.md#practicerunconfigurationtypedef) 
3. See [:material-code-brackets: ZonalAutoshiftStatusType](./literals.md#zonalautoshiftstatustype) 
4. See [:material-code-braces: ZonalShiftInResourceTypeDef](./type_defs.md#zonalshiftinresourcetypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePracticeRunConfigurationResponseTypeDef

```python
# UpdatePracticeRunConfigurationResponseTypeDef definition

class UpdatePracticeRunConfigurationResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    practiceRunConfiguration: PracticeRunConfigurationTypeDef,  # (1)
    zonalAutoshiftStatus: ZonalAutoshiftStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PracticeRunConfigurationTypeDef](./type_defs.md#practicerunconfigurationtypedef) 
2. See [:material-code-brackets: ZonalAutoshiftStatusType](./literals.md#zonalautoshiftstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedResourcesResponseTypeDef

```python
# ListManagedResourcesResponseTypeDef definition

class ListManagedResourcesResponseTypeDef(TypedDict):
    items: List[ManagedResourceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ManagedResourceSummaryTypeDef](./type_defs.md#managedresourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
