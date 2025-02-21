# Type definitions

> [Index](../README.md) > [ControlTower](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#controltower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).



## BaselineOperationTypeDef

```python
# BaselineOperationTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import BaselineOperationTypeDef


def get_value() -> BaselineOperationTypeDef:
    return {
        "endTime": ...,
    }


# BaselineOperationTypeDef definition

class BaselineOperationTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    operationIdentifier: NotRequired[str],
    operationType: NotRequired[BaselineOperationTypeType],  # (1)
    startTime: NotRequired[datetime],
    status: NotRequired[BaselineOperationStatusType],  # (2)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: BaselineOperationTypeType](./literals.md#baselineoperationtypetype) 
2. See [:material-code-brackets: BaselineOperationStatusType](./literals.md#baselineoperationstatustype) 
## BaselineSummaryTypeDef

```python
# BaselineSummaryTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import BaselineSummaryTypeDef


def get_value() -> BaselineSummaryTypeDef:
    return {
        "arn": ...,
    }


# BaselineSummaryTypeDef definition

class BaselineSummaryTypeDef(TypedDict):
    arn: str,
    name: str,
    description: NotRequired[str],
```

## ControlOperationFilterTypeDef

```python
# ControlOperationFilterTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ControlOperationFilterTypeDef


def get_value() -> ControlOperationFilterTypeDef:
    return {
        "controlIdentifiers": ...,
    }


# ControlOperationFilterTypeDef definition

class ControlOperationFilterTypeDef(TypedDict):
    controlIdentifiers: NotRequired[Sequence[str]],
    controlOperationTypes: NotRequired[Sequence[ControlOperationTypeType]],  # (1)
    enabledControlIdentifiers: NotRequired[Sequence[str]],
    statuses: NotRequired[Sequence[ControlOperationStatusType]],  # (2)
    targetIdentifiers: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ControlOperationTypeType](./literals.md#controloperationtypetype) 
2. See [:material-code-brackets: ControlOperationStatusType](./literals.md#controloperationstatustype) 
## ControlOperationSummaryTypeDef

```python
# ControlOperationSummaryTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ControlOperationSummaryTypeDef


def get_value() -> ControlOperationSummaryTypeDef:
    return {
        "controlIdentifier": ...,
    }


# ControlOperationSummaryTypeDef definition

class ControlOperationSummaryTypeDef(TypedDict):
    controlIdentifier: NotRequired[str],
    enabledControlIdentifier: NotRequired[str],
    endTime: NotRequired[datetime],
    operationIdentifier: NotRequired[str],
    operationType: NotRequired[ControlOperationTypeType],  # (1)
    startTime: NotRequired[datetime],
    status: NotRequired[ControlOperationStatusType],  # (2)
    statusMessage: NotRequired[str],
    targetIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: ControlOperationTypeType](./literals.md#controloperationtypetype) 
2. See [:material-code-brackets: ControlOperationStatusType](./literals.md#controloperationstatustype) 
## ControlOperationTypeDef

```python
# ControlOperationTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ControlOperationTypeDef


def get_value() -> ControlOperationTypeDef:
    return {
        "controlIdentifier": ...,
    }


# ControlOperationTypeDef definition

class ControlOperationTypeDef(TypedDict):
    controlIdentifier: NotRequired[str],
    enabledControlIdentifier: NotRequired[str],
    endTime: NotRequired[datetime],
    operationIdentifier: NotRequired[str],
    operationType: NotRequired[ControlOperationTypeType],  # (1)
    startTime: NotRequired[datetime],
    status: NotRequired[ControlOperationStatusType],  # (2)
    statusMessage: NotRequired[str],
    targetIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: ControlOperationTypeType](./literals.md#controloperationtypetype) 
2. See [:material-code-brackets: ControlOperationStatusType](./literals.md#controloperationstatustype) 
## CreateLandingZoneInputTypeDef

```python
# CreateLandingZoneInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import CreateLandingZoneInputTypeDef


def get_value() -> CreateLandingZoneInputTypeDef:
    return {
        "manifest": ...,
    }


# CreateLandingZoneInputTypeDef definition

class CreateLandingZoneInputTypeDef(TypedDict):
    manifest: Mapping[str, Any],
    version: str,
    tags: NotRequired[Mapping[str, str]],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ResponseMetadataTypeDef


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

## DeleteLandingZoneInputTypeDef

```python
# DeleteLandingZoneInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import DeleteLandingZoneInputTypeDef


def get_value() -> DeleteLandingZoneInputTypeDef:
    return {
        "landingZoneIdentifier": ...,
    }


# DeleteLandingZoneInputTypeDef definition

class DeleteLandingZoneInputTypeDef(TypedDict):
    landingZoneIdentifier: str,
```

## DisableBaselineInputTypeDef

```python
# DisableBaselineInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import DisableBaselineInputTypeDef


def get_value() -> DisableBaselineInputTypeDef:
    return {
        "enabledBaselineIdentifier": ...,
    }


# DisableBaselineInputTypeDef definition

class DisableBaselineInputTypeDef(TypedDict):
    enabledBaselineIdentifier: str,
```

## DisableControlInputTypeDef

```python
# DisableControlInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import DisableControlInputTypeDef


def get_value() -> DisableControlInputTypeDef:
    return {
        "controlIdentifier": ...,
    }


# DisableControlInputTypeDef definition

class DisableControlInputTypeDef(TypedDict):
    controlIdentifier: str,
    targetIdentifier: str,
```

## DriftStatusSummaryTypeDef

```python
# DriftStatusSummaryTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import DriftStatusSummaryTypeDef


def get_value() -> DriftStatusSummaryTypeDef:
    return {
        "driftStatus": ...,
    }


# DriftStatusSummaryTypeDef definition

class DriftStatusSummaryTypeDef(TypedDict):
    driftStatus: NotRequired[DriftStatusType],  # (1)
```

1. See [:material-code-brackets: DriftStatusType](./literals.md#driftstatustype) 
## EnabledBaselineParameterTypeDef

```python
# EnabledBaselineParameterTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnabledBaselineParameterTypeDef


def get_value() -> EnabledBaselineParameterTypeDef:
    return {
        "key": ...,
    }


# EnabledBaselineParameterTypeDef definition

class EnabledBaselineParameterTypeDef(TypedDict):
    key: str,
    value: Mapping[str, Any],
```

## EnabledControlParameterTypeDef

```python
# EnabledControlParameterTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnabledControlParameterTypeDef


def get_value() -> EnabledControlParameterTypeDef:
    return {
        "key": ...,
    }


# EnabledControlParameterTypeDef definition

class EnabledControlParameterTypeDef(TypedDict):
    key: str,
    value: Mapping[str, Any],
```

## EnabledBaselineParameterSummaryTypeDef

```python
# EnabledBaselineParameterSummaryTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnabledBaselineParameterSummaryTypeDef


def get_value() -> EnabledBaselineParameterSummaryTypeDef:
    return {
        "key": ...,
    }


# EnabledBaselineParameterSummaryTypeDef definition

class EnabledBaselineParameterSummaryTypeDef(TypedDict):
    key: str,
    value: Dict[str, Any],
```

## EnablementStatusSummaryTypeDef

```python
# EnablementStatusSummaryTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnablementStatusSummaryTypeDef


def get_value() -> EnablementStatusSummaryTypeDef:
    return {
        "lastOperationIdentifier": ...,
    }


# EnablementStatusSummaryTypeDef definition

class EnablementStatusSummaryTypeDef(TypedDict):
    lastOperationIdentifier: NotRequired[str],
    status: NotRequired[EnablementStatusType],  # (1)
```

1. See [:material-code-brackets: EnablementStatusType](./literals.md#enablementstatustype) 
## EnabledBaselineFilterTypeDef

```python
# EnabledBaselineFilterTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnabledBaselineFilterTypeDef


def get_value() -> EnabledBaselineFilterTypeDef:
    return {
        "baselineIdentifiers": ...,
    }


# EnabledBaselineFilterTypeDef definition

class EnabledBaselineFilterTypeDef(TypedDict):
    baselineIdentifiers: NotRequired[Sequence[str]],
    parentIdentifiers: NotRequired[Sequence[str]],
    targetIdentifiers: NotRequired[Sequence[str]],
```

## EnabledControlParameterSummaryTypeDef

```python
# EnabledControlParameterSummaryTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnabledControlParameterSummaryTypeDef


def get_value() -> EnabledControlParameterSummaryTypeDef:
    return {
        "key": ...,
    }


# EnabledControlParameterSummaryTypeDef definition

class EnabledControlParameterSummaryTypeDef(TypedDict):
    key: str,
    value: Dict[str, Any],
```

## RegionTypeDef

```python
# RegionTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import RegionTypeDef


def get_value() -> RegionTypeDef:
    return {
        "name": ...,
    }


# RegionTypeDef definition

class RegionTypeDef(TypedDict):
    name: NotRequired[str],
```

## EnabledControlFilterTypeDef

```python
# EnabledControlFilterTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnabledControlFilterTypeDef


def get_value() -> EnabledControlFilterTypeDef:
    return {
        "controlIdentifiers": ...,
    }


# EnabledControlFilterTypeDef definition

class EnabledControlFilterTypeDef(TypedDict):
    controlIdentifiers: NotRequired[Sequence[str]],
    driftStatuses: NotRequired[Sequence[DriftStatusType]],  # (1)
    statuses: NotRequired[Sequence[EnablementStatusType]],  # (2)
```

1. See [:material-code-brackets: DriftStatusType](./literals.md#driftstatustype) 
2. See [:material-code-brackets: EnablementStatusType](./literals.md#enablementstatustype) 
## GetBaselineInputTypeDef

```python
# GetBaselineInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetBaselineInputTypeDef


def get_value() -> GetBaselineInputTypeDef:
    return {
        "baselineIdentifier": ...,
    }


# GetBaselineInputTypeDef definition

class GetBaselineInputTypeDef(TypedDict):
    baselineIdentifier: str,
```

## GetBaselineOperationInputTypeDef

```python
# GetBaselineOperationInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetBaselineOperationInputTypeDef


def get_value() -> GetBaselineOperationInputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# GetBaselineOperationInputTypeDef definition

class GetBaselineOperationInputTypeDef(TypedDict):
    operationIdentifier: str,
```

## GetControlOperationInputTypeDef

```python
# GetControlOperationInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetControlOperationInputTypeDef


def get_value() -> GetControlOperationInputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# GetControlOperationInputTypeDef definition

class GetControlOperationInputTypeDef(TypedDict):
    operationIdentifier: str,
```

## GetEnabledBaselineInputTypeDef

```python
# GetEnabledBaselineInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetEnabledBaselineInputTypeDef


def get_value() -> GetEnabledBaselineInputTypeDef:
    return {
        "enabledBaselineIdentifier": ...,
    }


# GetEnabledBaselineInputTypeDef definition

class GetEnabledBaselineInputTypeDef(TypedDict):
    enabledBaselineIdentifier: str,
```

## GetEnabledControlInputTypeDef

```python
# GetEnabledControlInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetEnabledControlInputTypeDef


def get_value() -> GetEnabledControlInputTypeDef:
    return {
        "enabledControlIdentifier": ...,
    }


# GetEnabledControlInputTypeDef definition

class GetEnabledControlInputTypeDef(TypedDict):
    enabledControlIdentifier: str,
```

## GetLandingZoneInputTypeDef

```python
# GetLandingZoneInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetLandingZoneInputTypeDef


def get_value() -> GetLandingZoneInputTypeDef:
    return {
        "landingZoneIdentifier": ...,
    }


# GetLandingZoneInputTypeDef definition

class GetLandingZoneInputTypeDef(TypedDict):
    landingZoneIdentifier: str,
```

## GetLandingZoneOperationInputTypeDef

```python
# GetLandingZoneOperationInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetLandingZoneOperationInputTypeDef


def get_value() -> GetLandingZoneOperationInputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# GetLandingZoneOperationInputTypeDef definition

class GetLandingZoneOperationInputTypeDef(TypedDict):
    operationIdentifier: str,
```

## LandingZoneOperationDetailTypeDef

```python
# LandingZoneOperationDetailTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import LandingZoneOperationDetailTypeDef


def get_value() -> LandingZoneOperationDetailTypeDef:
    return {
        "endTime": ...,
    }


# LandingZoneOperationDetailTypeDef definition

class LandingZoneOperationDetailTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    operationIdentifier: NotRequired[str],
    operationType: NotRequired[LandingZoneOperationTypeType],  # (1)
    startTime: NotRequired[datetime],
    status: NotRequired[LandingZoneOperationStatusType],  # (2)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: LandingZoneOperationTypeType](./literals.md#landingzoneoperationtypetype) 
2. See [:material-code-brackets: LandingZoneOperationStatusType](./literals.md#landingzoneoperationstatustype) 
## LandingZoneDriftStatusSummaryTypeDef

```python
# LandingZoneDriftStatusSummaryTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import LandingZoneDriftStatusSummaryTypeDef


def get_value() -> LandingZoneDriftStatusSummaryTypeDef:
    return {
        "status": ...,
    }


# LandingZoneDriftStatusSummaryTypeDef definition

class LandingZoneDriftStatusSummaryTypeDef(TypedDict):
    status: NotRequired[LandingZoneDriftStatusType],  # (1)
```

1. See [:material-code-brackets: LandingZoneDriftStatusType](./literals.md#landingzonedriftstatustype) 
## LandingZoneOperationFilterTypeDef

```python
# LandingZoneOperationFilterTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import LandingZoneOperationFilterTypeDef


def get_value() -> LandingZoneOperationFilterTypeDef:
    return {
        "statuses": ...,
    }


# LandingZoneOperationFilterTypeDef definition

class LandingZoneOperationFilterTypeDef(TypedDict):
    statuses: NotRequired[Sequence[LandingZoneOperationStatusType]],  # (1)
    types: NotRequired[Sequence[LandingZoneOperationTypeType]],  # (2)
```

1. See [:material-code-brackets: LandingZoneOperationStatusType](./literals.md#landingzoneoperationstatustype) 
2. See [:material-code-brackets: LandingZoneOperationTypeType](./literals.md#landingzoneoperationtypetype) 
## LandingZoneOperationSummaryTypeDef

```python
# LandingZoneOperationSummaryTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import LandingZoneOperationSummaryTypeDef


def get_value() -> LandingZoneOperationSummaryTypeDef:
    return {
        "operationIdentifier": ...,
    }


# LandingZoneOperationSummaryTypeDef definition

class LandingZoneOperationSummaryTypeDef(TypedDict):
    operationIdentifier: NotRequired[str],
    operationType: NotRequired[LandingZoneOperationTypeType],  # (1)
    status: NotRequired[LandingZoneOperationStatusType],  # (2)
```

1. See [:material-code-brackets: LandingZoneOperationTypeType](./literals.md#landingzoneoperationtypetype) 
2. See [:material-code-brackets: LandingZoneOperationStatusType](./literals.md#landingzoneoperationstatustype) 
## LandingZoneSummaryTypeDef

```python
# LandingZoneSummaryTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import LandingZoneSummaryTypeDef


def get_value() -> LandingZoneSummaryTypeDef:
    return {
        "arn": ...,
    }


# LandingZoneSummaryTypeDef definition

class LandingZoneSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import PaginatorConfigTypeDef


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

## ListBaselinesInputTypeDef

```python
# ListBaselinesInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListBaselinesInputTypeDef


def get_value() -> ListBaselinesInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListBaselinesInputTypeDef definition

class ListBaselinesInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListLandingZonesInputTypeDef

```python
# ListLandingZonesInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListLandingZonesInputTypeDef


def get_value() -> ListLandingZonesInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListLandingZonesInputTypeDef definition

class ListLandingZonesInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    resourceArn: str,
```

## ResetEnabledBaselineInputTypeDef

```python
# ResetEnabledBaselineInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ResetEnabledBaselineInputTypeDef


def get_value() -> ResetEnabledBaselineInputTypeDef:
    return {
        "enabledBaselineIdentifier": ...,
    }


# ResetEnabledBaselineInputTypeDef definition

class ResetEnabledBaselineInputTypeDef(TypedDict):
    enabledBaselineIdentifier: str,
```

## ResetEnabledControlInputTypeDef

```python
# ResetEnabledControlInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ResetEnabledControlInputTypeDef


def get_value() -> ResetEnabledControlInputTypeDef:
    return {
        "enabledControlIdentifier": ...,
    }


# ResetEnabledControlInputTypeDef definition

class ResetEnabledControlInputTypeDef(TypedDict):
    enabledControlIdentifier: str,
```

## ResetLandingZoneInputTypeDef

```python
# ResetLandingZoneInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ResetLandingZoneInputTypeDef


def get_value() -> ResetLandingZoneInputTypeDef:
    return {
        "landingZoneIdentifier": ...,
    }


# ResetLandingZoneInputTypeDef definition

class ResetLandingZoneInputTypeDef(TypedDict):
    landingZoneIdentifier: str,
```

## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import TagResourceInputTypeDef


def get_value() -> TagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceInputTypeDef definition

class TagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputTypeDef

```python
# UntagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateLandingZoneInputTypeDef

```python
# UpdateLandingZoneInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import UpdateLandingZoneInputTypeDef


def get_value() -> UpdateLandingZoneInputTypeDef:
    return {
        "landingZoneIdentifier": ...,
    }


# UpdateLandingZoneInputTypeDef definition

class UpdateLandingZoneInputTypeDef(TypedDict):
    landingZoneIdentifier: str,
    manifest: Mapping[str, Any],
    version: str,
```

## ListControlOperationsInputTypeDef

```python
# ListControlOperationsInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListControlOperationsInputTypeDef


def get_value() -> ListControlOperationsInputTypeDef:
    return {
        "filter": ...,
    }


# ListControlOperationsInputTypeDef definition

class ListControlOperationsInputTypeDef(TypedDict):
    filter: NotRequired[ControlOperationFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ControlOperationFilterTypeDef](./type_defs.md#controloperationfiltertypedef) 
## CreateLandingZoneOutputTypeDef

```python
# CreateLandingZoneOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import CreateLandingZoneOutputTypeDef


def get_value() -> CreateLandingZoneOutputTypeDef:
    return {
        "arn": ...,
    }


# CreateLandingZoneOutputTypeDef definition

class CreateLandingZoneOutputTypeDef(TypedDict):
    arn: str,
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteLandingZoneOutputTypeDef

```python
# DeleteLandingZoneOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import DeleteLandingZoneOutputTypeDef


def get_value() -> DeleteLandingZoneOutputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# DeleteLandingZoneOutputTypeDef definition

class DeleteLandingZoneOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableBaselineOutputTypeDef

```python
# DisableBaselineOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import DisableBaselineOutputTypeDef


def get_value() -> DisableBaselineOutputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# DisableBaselineOutputTypeDef definition

class DisableBaselineOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableControlOutputTypeDef

```python
# DisableControlOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import DisableControlOutputTypeDef


def get_value() -> DisableControlOutputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# DisableControlOutputTypeDef definition

class DisableControlOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableBaselineOutputTypeDef

```python
# EnableBaselineOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnableBaselineOutputTypeDef


def get_value() -> EnableBaselineOutputTypeDef:
    return {
        "arn": ...,
    }


# EnableBaselineOutputTypeDef definition

class EnableBaselineOutputTypeDef(TypedDict):
    arn: str,
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableControlOutputTypeDef

```python
# EnableControlOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnableControlOutputTypeDef


def get_value() -> EnableControlOutputTypeDef:
    return {
        "arn": ...,
    }


# EnableControlOutputTypeDef definition

class EnableControlOutputTypeDef(TypedDict):
    arn: str,
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBaselineOperationOutputTypeDef

```python
# GetBaselineOperationOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetBaselineOperationOutputTypeDef


def get_value() -> GetBaselineOperationOutputTypeDef:
    return {
        "baselineOperation": ...,
    }


# GetBaselineOperationOutputTypeDef definition

class GetBaselineOperationOutputTypeDef(TypedDict):
    baselineOperation: BaselineOperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BaselineOperationTypeDef](./type_defs.md#baselineoperationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBaselineOutputTypeDef

```python
# GetBaselineOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetBaselineOutputTypeDef


def get_value() -> GetBaselineOutputTypeDef:
    return {
        "arn": ...,
    }


# GetBaselineOutputTypeDef definition

class GetBaselineOutputTypeDef(TypedDict):
    arn: str,
    description: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetControlOperationOutputTypeDef

```python
# GetControlOperationOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetControlOperationOutputTypeDef


def get_value() -> GetControlOperationOutputTypeDef:
    return {
        "controlOperation": ...,
    }


# GetControlOperationOutputTypeDef definition

class GetControlOperationOutputTypeDef(TypedDict):
    controlOperation: ControlOperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ControlOperationTypeDef](./type_defs.md#controloperationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBaselinesOutputTypeDef

```python
# ListBaselinesOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListBaselinesOutputTypeDef


def get_value() -> ListBaselinesOutputTypeDef:
    return {
        "baselines": ...,
    }


# ListBaselinesOutputTypeDef definition

class ListBaselinesOutputTypeDef(TypedDict):
    baselines: List[BaselineSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BaselineSummaryTypeDef](./type_defs.md#baselinesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListControlOperationsOutputTypeDef

```python
# ListControlOperationsOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListControlOperationsOutputTypeDef


def get_value() -> ListControlOperationsOutputTypeDef:
    return {
        "controlOperations": ...,
    }


# ListControlOperationsOutputTypeDef definition

class ListControlOperationsOutputTypeDef(TypedDict):
    controlOperations: List[ControlOperationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ControlOperationSummaryTypeDef](./type_defs.md#controloperationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListTagsForResourceOutputTypeDef


def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetEnabledBaselineOutputTypeDef

```python
# ResetEnabledBaselineOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ResetEnabledBaselineOutputTypeDef


def get_value() -> ResetEnabledBaselineOutputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# ResetEnabledBaselineOutputTypeDef definition

class ResetEnabledBaselineOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetEnabledControlOutputTypeDef

```python
# ResetEnabledControlOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ResetEnabledControlOutputTypeDef


def get_value() -> ResetEnabledControlOutputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# ResetEnabledControlOutputTypeDef definition

class ResetEnabledControlOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetLandingZoneOutputTypeDef

```python
# ResetLandingZoneOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ResetLandingZoneOutputTypeDef


def get_value() -> ResetLandingZoneOutputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# ResetLandingZoneOutputTypeDef definition

class ResetLandingZoneOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnabledBaselineOutputTypeDef

```python
# UpdateEnabledBaselineOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import UpdateEnabledBaselineOutputTypeDef


def get_value() -> UpdateEnabledBaselineOutputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# UpdateEnabledBaselineOutputTypeDef definition

class UpdateEnabledBaselineOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnabledControlOutputTypeDef

```python
# UpdateEnabledControlOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import UpdateEnabledControlOutputTypeDef


def get_value() -> UpdateEnabledControlOutputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# UpdateEnabledControlOutputTypeDef definition

class UpdateEnabledControlOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLandingZoneOutputTypeDef

```python
# UpdateLandingZoneOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import UpdateLandingZoneOutputTypeDef


def get_value() -> UpdateLandingZoneOutputTypeDef:
    return {
        "operationIdentifier": ...,
    }


# UpdateLandingZoneOutputTypeDef definition

class UpdateLandingZoneOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableBaselineInputTypeDef

```python
# EnableBaselineInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnableBaselineInputTypeDef


def get_value() -> EnableBaselineInputTypeDef:
    return {
        "baselineIdentifier": ...,
    }


# EnableBaselineInputTypeDef definition

class EnableBaselineInputTypeDef(TypedDict):
    baselineIdentifier: str,
    baselineVersion: str,
    targetIdentifier: str,
    parameters: NotRequired[Sequence[EnabledBaselineParameterTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: EnabledBaselineParameterTypeDef](./type_defs.md#enabledbaselineparametertypedef) 
## UpdateEnabledBaselineInputTypeDef

```python
# UpdateEnabledBaselineInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import UpdateEnabledBaselineInputTypeDef


def get_value() -> UpdateEnabledBaselineInputTypeDef:
    return {
        "baselineVersion": ...,
    }


# UpdateEnabledBaselineInputTypeDef definition

class UpdateEnabledBaselineInputTypeDef(TypedDict):
    baselineVersion: str,
    enabledBaselineIdentifier: str,
    parameters: NotRequired[Sequence[EnabledBaselineParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: EnabledBaselineParameterTypeDef](./type_defs.md#enabledbaselineparametertypedef) 
## EnableControlInputTypeDef

```python
# EnableControlInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnableControlInputTypeDef


def get_value() -> EnableControlInputTypeDef:
    return {
        "controlIdentifier": ...,
    }


# EnableControlInputTypeDef definition

class EnableControlInputTypeDef(TypedDict):
    controlIdentifier: str,
    targetIdentifier: str,
    parameters: NotRequired[Sequence[EnabledControlParameterTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: EnabledControlParameterTypeDef](./type_defs.md#enabledcontrolparametertypedef) 
## UpdateEnabledControlInputTypeDef

```python
# UpdateEnabledControlInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import UpdateEnabledControlInputTypeDef


def get_value() -> UpdateEnabledControlInputTypeDef:
    return {
        "enabledControlIdentifier": ...,
    }


# UpdateEnabledControlInputTypeDef definition

class UpdateEnabledControlInputTypeDef(TypedDict):
    enabledControlIdentifier: str,
    parameters: Sequence[EnabledControlParameterTypeDef],  # (1)
```

1. See [:material-code-braces: EnabledControlParameterTypeDef](./type_defs.md#enabledcontrolparametertypedef) 
## EnabledBaselineDetailsTypeDef

```python
# EnabledBaselineDetailsTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnabledBaselineDetailsTypeDef


def get_value() -> EnabledBaselineDetailsTypeDef:
    return {
        "arn": ...,
    }


# EnabledBaselineDetailsTypeDef definition

class EnabledBaselineDetailsTypeDef(TypedDict):
    arn: str,
    baselineIdentifier: str,
    statusSummary: EnablementStatusSummaryTypeDef,  # (2)
    targetIdentifier: str,
    baselineVersion: NotRequired[str],
    parameters: NotRequired[List[EnabledBaselineParameterSummaryTypeDef]],  # (1)
    parentIdentifier: NotRequired[str],
```

1. See [:material-code-braces: EnabledBaselineParameterSummaryTypeDef](./type_defs.md#enabledbaselineparametersummarytypedef) 
2. See [:material-code-braces: EnablementStatusSummaryTypeDef](./type_defs.md#enablementstatussummarytypedef) 
## EnabledBaselineSummaryTypeDef

```python
# EnabledBaselineSummaryTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnabledBaselineSummaryTypeDef


def get_value() -> EnabledBaselineSummaryTypeDef:
    return {
        "arn": ...,
    }


# EnabledBaselineSummaryTypeDef definition

class EnabledBaselineSummaryTypeDef(TypedDict):
    arn: str,
    baselineIdentifier: str,
    statusSummary: EnablementStatusSummaryTypeDef,  # (1)
    targetIdentifier: str,
    baselineVersion: NotRequired[str],
    parentIdentifier: NotRequired[str],
```

1. See [:material-code-braces: EnablementStatusSummaryTypeDef](./type_defs.md#enablementstatussummarytypedef) 
## EnabledControlSummaryTypeDef

```python
# EnabledControlSummaryTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnabledControlSummaryTypeDef


def get_value() -> EnabledControlSummaryTypeDef:
    return {
        "arn": ...,
    }


# EnabledControlSummaryTypeDef definition

class EnabledControlSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    controlIdentifier: NotRequired[str],
    driftStatusSummary: NotRequired[DriftStatusSummaryTypeDef],  # (1)
    statusSummary: NotRequired[EnablementStatusSummaryTypeDef],  # (2)
    targetIdentifier: NotRequired[str],
```

1. See [:material-code-braces: DriftStatusSummaryTypeDef](./type_defs.md#driftstatussummarytypedef) 
2. See [:material-code-braces: EnablementStatusSummaryTypeDef](./type_defs.md#enablementstatussummarytypedef) 
## ListEnabledBaselinesInputTypeDef

```python
# ListEnabledBaselinesInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListEnabledBaselinesInputTypeDef


def get_value() -> ListEnabledBaselinesInputTypeDef:
    return {
        "filter": ...,
    }


# ListEnabledBaselinesInputTypeDef definition

class ListEnabledBaselinesInputTypeDef(TypedDict):
    filter: NotRequired[EnabledBaselineFilterTypeDef],  # (1)
    includeChildren: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnabledBaselineFilterTypeDef](./type_defs.md#enabledbaselinefiltertypedef) 
## EnabledControlDetailsTypeDef

```python
# EnabledControlDetailsTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import EnabledControlDetailsTypeDef


def get_value() -> EnabledControlDetailsTypeDef:
    return {
        "arn": ...,
    }


# EnabledControlDetailsTypeDef definition

class EnabledControlDetailsTypeDef(TypedDict):
    arn: NotRequired[str],
    controlIdentifier: NotRequired[str],
    driftStatusSummary: NotRequired[DriftStatusSummaryTypeDef],  # (1)
    parameters: NotRequired[List[EnabledControlParameterSummaryTypeDef]],  # (2)
    statusSummary: NotRequired[EnablementStatusSummaryTypeDef],  # (3)
    targetIdentifier: NotRequired[str],
    targetRegions: NotRequired[List[RegionTypeDef]],  # (4)
```

1. See [:material-code-braces: DriftStatusSummaryTypeDef](./type_defs.md#driftstatussummarytypedef) 
2. See [:material-code-braces: EnabledControlParameterSummaryTypeDef](./type_defs.md#enabledcontrolparametersummarytypedef) 
3. See [:material-code-braces: EnablementStatusSummaryTypeDef](./type_defs.md#enablementstatussummarytypedef) 
4. See [:material-code-braces: RegionTypeDef](./type_defs.md#regiontypedef) 
## ListEnabledControlsInputTypeDef

```python
# ListEnabledControlsInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListEnabledControlsInputTypeDef


def get_value() -> ListEnabledControlsInputTypeDef:
    return {
        "filter": ...,
    }


# ListEnabledControlsInputTypeDef definition

class ListEnabledControlsInputTypeDef(TypedDict):
    filter: NotRequired[EnabledControlFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    targetIdentifier: NotRequired[str],
```

1. See [:material-code-braces: EnabledControlFilterTypeDef](./type_defs.md#enabledcontrolfiltertypedef) 
## GetLandingZoneOperationOutputTypeDef

```python
# GetLandingZoneOperationOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetLandingZoneOperationOutputTypeDef


def get_value() -> GetLandingZoneOperationOutputTypeDef:
    return {
        "operationDetails": ...,
    }


# GetLandingZoneOperationOutputTypeDef definition

class GetLandingZoneOperationOutputTypeDef(TypedDict):
    operationDetails: LandingZoneOperationDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LandingZoneOperationDetailTypeDef](./type_defs.md#landingzoneoperationdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LandingZoneDetailTypeDef

```python
# LandingZoneDetailTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import LandingZoneDetailTypeDef


def get_value() -> LandingZoneDetailTypeDef:
    return {
        "arn": ...,
    }


# LandingZoneDetailTypeDef definition

class LandingZoneDetailTypeDef(TypedDict):
    manifest: Dict[str, Any],
    version: str,
    arn: NotRequired[str],
    driftStatus: NotRequired[LandingZoneDriftStatusSummaryTypeDef],  # (1)
    latestAvailableVersion: NotRequired[str],
    status: NotRequired[LandingZoneStatusType],  # (2)
```

1. See [:material-code-braces: LandingZoneDriftStatusSummaryTypeDef](./type_defs.md#landingzonedriftstatussummarytypedef) 
2. See [:material-code-brackets: LandingZoneStatusType](./literals.md#landingzonestatustype) 
## ListLandingZoneOperationsInputTypeDef

```python
# ListLandingZoneOperationsInputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListLandingZoneOperationsInputTypeDef


def get_value() -> ListLandingZoneOperationsInputTypeDef:
    return {
        "filter": ...,
    }


# ListLandingZoneOperationsInputTypeDef definition

class ListLandingZoneOperationsInputTypeDef(TypedDict):
    filter: NotRequired[LandingZoneOperationFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LandingZoneOperationFilterTypeDef](./type_defs.md#landingzoneoperationfiltertypedef) 
## ListLandingZoneOperationsOutputTypeDef

```python
# ListLandingZoneOperationsOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListLandingZoneOperationsOutputTypeDef


def get_value() -> ListLandingZoneOperationsOutputTypeDef:
    return {
        "landingZoneOperations": ...,
    }


# ListLandingZoneOperationsOutputTypeDef definition

class ListLandingZoneOperationsOutputTypeDef(TypedDict):
    landingZoneOperations: List[LandingZoneOperationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LandingZoneOperationSummaryTypeDef](./type_defs.md#landingzoneoperationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLandingZonesOutputTypeDef

```python
# ListLandingZonesOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListLandingZonesOutputTypeDef


def get_value() -> ListLandingZonesOutputTypeDef:
    return {
        "landingZones": ...,
    }


# ListLandingZonesOutputTypeDef definition

class ListLandingZonesOutputTypeDef(TypedDict):
    landingZones: List[LandingZoneSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LandingZoneSummaryTypeDef](./type_defs.md#landingzonesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBaselinesInputPaginateTypeDef

```python
# ListBaselinesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListBaselinesInputPaginateTypeDef


def get_value() -> ListBaselinesInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListBaselinesInputPaginateTypeDef definition

class ListBaselinesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListControlOperationsInputPaginateTypeDef

```python
# ListControlOperationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListControlOperationsInputPaginateTypeDef


def get_value() -> ListControlOperationsInputPaginateTypeDef:
    return {
        "filter": ...,
    }


# ListControlOperationsInputPaginateTypeDef definition

class ListControlOperationsInputPaginateTypeDef(TypedDict):
    filter: NotRequired[ControlOperationFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ControlOperationFilterTypeDef](./type_defs.md#controloperationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnabledBaselinesInputPaginateTypeDef

```python
# ListEnabledBaselinesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListEnabledBaselinesInputPaginateTypeDef


def get_value() -> ListEnabledBaselinesInputPaginateTypeDef:
    return {
        "filter": ...,
    }


# ListEnabledBaselinesInputPaginateTypeDef definition

class ListEnabledBaselinesInputPaginateTypeDef(TypedDict):
    filter: NotRequired[EnabledBaselineFilterTypeDef],  # (1)
    includeChildren: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EnabledBaselineFilterTypeDef](./type_defs.md#enabledbaselinefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnabledControlsInputPaginateTypeDef

```python
# ListEnabledControlsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListEnabledControlsInputPaginateTypeDef


def get_value() -> ListEnabledControlsInputPaginateTypeDef:
    return {
        "filter": ...,
    }


# ListEnabledControlsInputPaginateTypeDef definition

class ListEnabledControlsInputPaginateTypeDef(TypedDict):
    filter: NotRequired[EnabledControlFilterTypeDef],  # (1)
    targetIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EnabledControlFilterTypeDef](./type_defs.md#enabledcontrolfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLandingZoneOperationsInputPaginateTypeDef

```python
# ListLandingZoneOperationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListLandingZoneOperationsInputPaginateTypeDef


def get_value() -> ListLandingZoneOperationsInputPaginateTypeDef:
    return {
        "filter": ...,
    }


# ListLandingZoneOperationsInputPaginateTypeDef definition

class ListLandingZoneOperationsInputPaginateTypeDef(TypedDict):
    filter: NotRequired[LandingZoneOperationFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: LandingZoneOperationFilterTypeDef](./type_defs.md#landingzoneoperationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLandingZonesInputPaginateTypeDef

```python
# ListLandingZonesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListLandingZonesInputPaginateTypeDef


def get_value() -> ListLandingZonesInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListLandingZonesInputPaginateTypeDef definition

class ListLandingZonesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetEnabledBaselineOutputTypeDef

```python
# GetEnabledBaselineOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetEnabledBaselineOutputTypeDef


def get_value() -> GetEnabledBaselineOutputTypeDef:
    return {
        "enabledBaselineDetails": ...,
    }


# GetEnabledBaselineOutputTypeDef definition

class GetEnabledBaselineOutputTypeDef(TypedDict):
    enabledBaselineDetails: EnabledBaselineDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnabledBaselineDetailsTypeDef](./type_defs.md#enabledbaselinedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnabledBaselinesOutputTypeDef

```python
# ListEnabledBaselinesOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListEnabledBaselinesOutputTypeDef


def get_value() -> ListEnabledBaselinesOutputTypeDef:
    return {
        "enabledBaselines": ...,
    }


# ListEnabledBaselinesOutputTypeDef definition

class ListEnabledBaselinesOutputTypeDef(TypedDict):
    enabledBaselines: List[EnabledBaselineSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnabledBaselineSummaryTypeDef](./type_defs.md#enabledbaselinesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnabledControlsOutputTypeDef

```python
# ListEnabledControlsOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import ListEnabledControlsOutputTypeDef


def get_value() -> ListEnabledControlsOutputTypeDef:
    return {
        "enabledControls": ...,
    }


# ListEnabledControlsOutputTypeDef definition

class ListEnabledControlsOutputTypeDef(TypedDict):
    enabledControls: List[EnabledControlSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnabledControlSummaryTypeDef](./type_defs.md#enabledcontrolsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnabledControlOutputTypeDef

```python
# GetEnabledControlOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetEnabledControlOutputTypeDef


def get_value() -> GetEnabledControlOutputTypeDef:
    return {
        "enabledControlDetails": ...,
    }


# GetEnabledControlOutputTypeDef definition

class GetEnabledControlOutputTypeDef(TypedDict):
    enabledControlDetails: EnabledControlDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnabledControlDetailsTypeDef](./type_defs.md#enabledcontroldetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLandingZoneOutputTypeDef

```python
# GetLandingZoneOutputTypeDef TypedDict usage example

from types_aiobotocore_controltower.type_defs import GetLandingZoneOutputTypeDef


def get_value() -> GetLandingZoneOutputTypeDef:
    return {
        "landingZone": ...,
    }


# GetLandingZoneOutputTypeDef definition

class GetLandingZoneOutputTypeDef(TypedDict):
    landingZone: LandingZoneDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LandingZoneDetailTypeDef](./type_defs.md#landingzonedetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
