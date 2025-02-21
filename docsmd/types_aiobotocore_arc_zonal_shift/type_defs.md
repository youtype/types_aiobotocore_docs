# Type definitions

> [Index](../README.md) > [ARCZonalShift](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ARCZonalShift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#arczonalshift)
    type annotations stubs module [types-aiobotocore-arc-zonal-shift](https://pypi.org/project/types-aiobotocore-arc-zonal-shift/).



## AutoshiftInResourceTypeDef

```python
# AutoshiftInResourceTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import AutoshiftInResourceTypeDef


def get_value() -> AutoshiftInResourceTypeDef:
    return {
        "appliedStatus": ...,
    }


# AutoshiftInResourceTypeDef definition

class AutoshiftInResourceTypeDef(TypedDict):
    appliedStatus: AutoshiftAppliedStatusType,  # (1)
    awayFrom: str,
    startTime: datetime,
```

1. See [:material-code-brackets: AutoshiftAppliedStatusType](./literals.md#autoshiftappliedstatustype) 
## AutoshiftSummaryTypeDef

```python
# AutoshiftSummaryTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import AutoshiftSummaryTypeDef


def get_value() -> AutoshiftSummaryTypeDef:
    return {
        "awayFrom": ...,
    }


# AutoshiftSummaryTypeDef definition

class AutoshiftSummaryTypeDef(TypedDict):
    awayFrom: str,
    endTime: datetime,
    startTime: datetime,
    status: AutoshiftExecutionStatusType,  # (1)
```

1. See [:material-code-brackets: AutoshiftExecutionStatusType](./literals.md#autoshiftexecutionstatustype) 
## CancelZonalShiftRequestTypeDef

```python
# CancelZonalShiftRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import CancelZonalShiftRequestTypeDef


def get_value() -> CancelZonalShiftRequestTypeDef:
    return {
        "zonalShiftId": ...,
    }


# CancelZonalShiftRequestTypeDef definition

class CancelZonalShiftRequestTypeDef(TypedDict):
    zonalShiftId: str,
```

## ControlConditionTypeDef

```python
# ControlConditionTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ControlConditionTypeDef


def get_value() -> ControlConditionTypeDef:
    return {
        "alarmIdentifier": ...,
    }


# ControlConditionTypeDef definition

class ControlConditionTypeDef(TypedDict):
    alarmIdentifier: str,
    type: ControlConditionTypeType,  # (1)
```

1. See [:material-code-brackets: ControlConditionTypeType](./literals.md#controlconditiontypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ResponseMetadataTypeDef


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

## DeletePracticeRunConfigurationRequestTypeDef

```python
# DeletePracticeRunConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import DeletePracticeRunConfigurationRequestTypeDef


def get_value() -> DeletePracticeRunConfigurationRequestTypeDef:
    return {
        "resourceIdentifier": ...,
    }


# DeletePracticeRunConfigurationRequestTypeDef definition

class DeletePracticeRunConfigurationRequestTypeDef(TypedDict):
    resourceIdentifier: str,
```

## GetManagedResourceRequestTypeDef

```python
# GetManagedResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import GetManagedResourceRequestTypeDef


def get_value() -> GetManagedResourceRequestTypeDef:
    return {
        "resourceIdentifier": ...,
    }


# GetManagedResourceRequestTypeDef definition

class GetManagedResourceRequestTypeDef(TypedDict):
    resourceIdentifier: str,
```

## ZonalShiftInResourceTypeDef

```python
# ZonalShiftInResourceTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ZonalShiftInResourceTypeDef


def get_value() -> ZonalShiftInResourceTypeDef:
    return {
        "appliedStatus": ...,
    }


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
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAutoshiftsRequestTypeDef

```python
# ListAutoshiftsRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ListAutoshiftsRequestTypeDef


def get_value() -> ListAutoshiftsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListAutoshiftsRequestTypeDef definition

class ListAutoshiftsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[AutoshiftExecutionStatusType],  # (1)
```

1. See [:material-code-brackets: AutoshiftExecutionStatusType](./literals.md#autoshiftexecutionstatustype) 
## ListManagedResourcesRequestTypeDef

```python
# ListManagedResourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ListManagedResourcesRequestTypeDef


def get_value() -> ListManagedResourcesRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListManagedResourcesRequestTypeDef definition

class ListManagedResourcesRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListZonalShiftsRequestTypeDef

```python
# ListZonalShiftsRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ListZonalShiftsRequestTypeDef


def get_value() -> ListZonalShiftsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListZonalShiftsRequestTypeDef definition

class ListZonalShiftsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    resourceIdentifier: NotRequired[str],
    status: NotRequired[ZonalShiftStatusType],  # (1)
```

1. See [:material-code-brackets: ZonalShiftStatusType](./literals.md#zonalshiftstatustype) 
## ZonalShiftSummaryTypeDef

```python
# ZonalShiftSummaryTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ZonalShiftSummaryTypeDef


def get_value() -> ZonalShiftSummaryTypeDef:
    return {
        "awayFrom": ...,
    }


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
## StartZonalShiftRequestTypeDef

```python
# StartZonalShiftRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import StartZonalShiftRequestTypeDef


def get_value() -> StartZonalShiftRequestTypeDef:
    return {
        "awayFrom": ...,
    }


# StartZonalShiftRequestTypeDef definition

class StartZonalShiftRequestTypeDef(TypedDict):
    awayFrom: str,
    comment: str,
    expiresIn: str,
    resourceIdentifier: str,
```

## UpdateAutoshiftObserverNotificationStatusRequestTypeDef

```python
# UpdateAutoshiftObserverNotificationStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import UpdateAutoshiftObserverNotificationStatusRequestTypeDef


def get_value() -> UpdateAutoshiftObserverNotificationStatusRequestTypeDef:
    return {
        "status": ...,
    }


# UpdateAutoshiftObserverNotificationStatusRequestTypeDef definition

class UpdateAutoshiftObserverNotificationStatusRequestTypeDef(TypedDict):
    status: AutoshiftObserverNotificationStatusType,  # (1)
```

1. See [:material-code-brackets: AutoshiftObserverNotificationStatusType](./literals.md#autoshiftobservernotificationstatustype) 
## UpdateZonalAutoshiftConfigurationRequestTypeDef

```python
# UpdateZonalAutoshiftConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import UpdateZonalAutoshiftConfigurationRequestTypeDef


def get_value() -> UpdateZonalAutoshiftConfigurationRequestTypeDef:
    return {
        "resourceIdentifier": ...,
    }


# UpdateZonalAutoshiftConfigurationRequestTypeDef definition

class UpdateZonalAutoshiftConfigurationRequestTypeDef(TypedDict):
    resourceIdentifier: str,
    zonalAutoshiftStatus: ZonalAutoshiftStatusType,  # (1)
```

1. See [:material-code-brackets: ZonalAutoshiftStatusType](./literals.md#zonalautoshiftstatustype) 
## UpdateZonalShiftRequestTypeDef

```python
# UpdateZonalShiftRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import UpdateZonalShiftRequestTypeDef


def get_value() -> UpdateZonalShiftRequestTypeDef:
    return {
        "zonalShiftId": ...,
    }


# UpdateZonalShiftRequestTypeDef definition

class UpdateZonalShiftRequestTypeDef(TypedDict):
    zonalShiftId: str,
    comment: NotRequired[str],
    expiresIn: NotRequired[str],
```

## CreatePracticeRunConfigurationRequestTypeDef

```python
# CreatePracticeRunConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import CreatePracticeRunConfigurationRequestTypeDef


def get_value() -> CreatePracticeRunConfigurationRequestTypeDef:
    return {
        "outcomeAlarms": ...,
    }


# CreatePracticeRunConfigurationRequestTypeDef definition

class CreatePracticeRunConfigurationRequestTypeDef(TypedDict):
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
# PracticeRunConfigurationTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import PracticeRunConfigurationTypeDef


def get_value() -> PracticeRunConfigurationTypeDef:
    return {
        "blockedDates": ...,
    }


# PracticeRunConfigurationTypeDef definition

class PracticeRunConfigurationTypeDef(TypedDict):
    outcomeAlarms: List[ControlConditionTypeDef],  # (1)
    blockedDates: NotRequired[List[str]],
    blockedWindows: NotRequired[List[str]],
    blockingAlarms: NotRequired[List[ControlConditionTypeDef]],  # (1)
```

1. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
2. See [:material-code-braces: ControlConditionTypeDef](./type_defs.md#controlconditiontypedef) 
## UpdatePracticeRunConfigurationRequestTypeDef

```python
# UpdatePracticeRunConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import UpdatePracticeRunConfigurationRequestTypeDef


def get_value() -> UpdatePracticeRunConfigurationRequestTypeDef:
    return {
        "resourceIdentifier": ...,
    }


# UpdatePracticeRunConfigurationRequestTypeDef definition

class UpdatePracticeRunConfigurationRequestTypeDef(TypedDict):
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
# DeletePracticeRunConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import DeletePracticeRunConfigurationResponseTypeDef


def get_value() -> DeletePracticeRunConfigurationResponseTypeDef:
    return {
        "arn": ...,
    }


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
# GetAutoshiftObserverNotificationStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import GetAutoshiftObserverNotificationStatusResponseTypeDef


def get_value() -> GetAutoshiftObserverNotificationStatusResponseTypeDef:
    return {
        "status": ...,
    }


# GetAutoshiftObserverNotificationStatusResponseTypeDef definition

class GetAutoshiftObserverNotificationStatusResponseTypeDef(TypedDict):
    status: AutoshiftObserverNotificationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AutoshiftObserverNotificationStatusType](./literals.md#autoshiftobservernotificationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAutoshiftsResponseTypeDef

```python
# ListAutoshiftsResponseTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ListAutoshiftsResponseTypeDef


def get_value() -> ListAutoshiftsResponseTypeDef:
    return {
        "items": ...,
    }


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
# UpdateAutoshiftObserverNotificationStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import UpdateAutoshiftObserverNotificationStatusResponseTypeDef


def get_value() -> UpdateAutoshiftObserverNotificationStatusResponseTypeDef:
    return {
        "status": ...,
    }


# UpdateAutoshiftObserverNotificationStatusResponseTypeDef definition

class UpdateAutoshiftObserverNotificationStatusResponseTypeDef(TypedDict):
    status: AutoshiftObserverNotificationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AutoshiftObserverNotificationStatusType](./literals.md#autoshiftobservernotificationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateZonalAutoshiftConfigurationResponseTypeDef

```python
# UpdateZonalAutoshiftConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import UpdateZonalAutoshiftConfigurationResponseTypeDef


def get_value() -> UpdateZonalAutoshiftConfigurationResponseTypeDef:
    return {
        "resourceIdentifier": ...,
    }


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
# ZonalShiftTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ZonalShiftTypeDef


def get_value() -> ZonalShiftTypeDef:
    return {
        "awayFrom": ...,
    }


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
# ManagedResourceSummaryTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ManagedResourceSummaryTypeDef


def get_value() -> ManagedResourceSummaryTypeDef:
    return {
        "appliedWeights": ...,
    }


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
# ListAutoshiftsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ListAutoshiftsRequestPaginateTypeDef


def get_value() -> ListAutoshiftsRequestPaginateTypeDef:
    return {
        "status": ...,
    }


# ListAutoshiftsRequestPaginateTypeDef definition

class ListAutoshiftsRequestPaginateTypeDef(TypedDict):
    status: NotRequired[AutoshiftExecutionStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AutoshiftExecutionStatusType](./literals.md#autoshiftexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedResourcesRequestPaginateTypeDef

```python
# ListManagedResourcesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ListManagedResourcesRequestPaginateTypeDef


def get_value() -> ListManagedResourcesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListManagedResourcesRequestPaginateTypeDef definition

class ListManagedResourcesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListZonalShiftsRequestPaginateTypeDef

```python
# ListZonalShiftsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ListZonalShiftsRequestPaginateTypeDef


def get_value() -> ListZonalShiftsRequestPaginateTypeDef:
    return {
        "resourceIdentifier": ...,
    }


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
# ListZonalShiftsResponseTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ListZonalShiftsResponseTypeDef


def get_value() -> ListZonalShiftsResponseTypeDef:
    return {
        "items": ...,
    }


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
# CreatePracticeRunConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import CreatePracticeRunConfigurationResponseTypeDef


def get_value() -> CreatePracticeRunConfigurationResponseTypeDef:
    return {
        "arn": ...,
    }


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
# GetManagedResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import GetManagedResourceResponseTypeDef


def get_value() -> GetManagedResourceResponseTypeDef:
    return {
        "appliedWeights": ...,
    }


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
# UpdatePracticeRunConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import UpdatePracticeRunConfigurationResponseTypeDef


def get_value() -> UpdatePracticeRunConfigurationResponseTypeDef:
    return {
        "arn": ...,
    }


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
# ListManagedResourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_arc_zonal_shift.type_defs import ListManagedResourcesResponseTypeDef


def get_value() -> ListManagedResourcesResponseTypeDef:
    return {
        "items": ...,
    }


# ListManagedResourcesResponseTypeDef definition

class ListManagedResourcesResponseTypeDef(TypedDict):
    items: List[ManagedResourceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ManagedResourceSummaryTypeDef](./type_defs.md#managedresourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
