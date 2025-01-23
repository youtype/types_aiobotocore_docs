# Type definitions

> [Index](../README.md) > [ControlTower](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#controltower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).



## BaselineOperationTypeDef

```python
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
# BaselineSummaryTypeDef definition

class BaselineSummaryTypeDef(TypedDict):
    arn: str,
    name: str,
    description: NotRequired[str],
```

## ControlOperationFilterTypeDef

```python
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
## CreateLandingZoneInputRequestTypeDef

```python
# CreateLandingZoneInputRequestTypeDef definition

class CreateLandingZoneInputRequestTypeDef(TypedDict):
    manifest: Mapping[str, Any],
    version: str,
    tags: NotRequired[Mapping[str, str]],
```

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

## DeleteLandingZoneInputRequestTypeDef

```python
# DeleteLandingZoneInputRequestTypeDef definition

class DeleteLandingZoneInputRequestTypeDef(TypedDict):
    landingZoneIdentifier: str,
```

## DisableBaselineInputRequestTypeDef

```python
# DisableBaselineInputRequestTypeDef definition

class DisableBaselineInputRequestTypeDef(TypedDict):
    enabledBaselineIdentifier: str,
```

## DisableControlInputRequestTypeDef

```python
# DisableControlInputRequestTypeDef definition

class DisableControlInputRequestTypeDef(TypedDict):
    controlIdentifier: str,
    targetIdentifier: str,
```

## DriftStatusSummaryTypeDef

```python
# DriftStatusSummaryTypeDef definition

class DriftStatusSummaryTypeDef(TypedDict):
    driftStatus: NotRequired[DriftStatusType],  # (1)
```

1. See [:material-code-brackets: DriftStatusType](./literals.md#driftstatustype) 
## EnabledBaselineParameterTypeDef

```python
# EnabledBaselineParameterTypeDef definition

class EnabledBaselineParameterTypeDef(TypedDict):
    key: str,
    value: Mapping[str, Any],
```

## EnabledControlParameterTypeDef

```python
# EnabledControlParameterTypeDef definition

class EnabledControlParameterTypeDef(TypedDict):
    key: str,
    value: Mapping[str, Any],
```

## EnabledBaselineParameterSummaryTypeDef

```python
# EnabledBaselineParameterSummaryTypeDef definition

class EnabledBaselineParameterSummaryTypeDef(TypedDict):
    key: str,
    value: Dict[str, Any],
```

## EnablementStatusSummaryTypeDef

```python
# EnablementStatusSummaryTypeDef definition

class EnablementStatusSummaryTypeDef(TypedDict):
    lastOperationIdentifier: NotRequired[str],
    status: NotRequired[EnablementStatusType],  # (1)
```

1. See [:material-code-brackets: EnablementStatusType](./literals.md#enablementstatustype) 
## EnabledBaselineFilterTypeDef

```python
# EnabledBaselineFilterTypeDef definition

class EnabledBaselineFilterTypeDef(TypedDict):
    baselineIdentifiers: NotRequired[Sequence[str]],
    parentIdentifiers: NotRequired[Sequence[str]],
    targetIdentifiers: NotRequired[Sequence[str]],
```

## EnabledControlParameterSummaryTypeDef

```python
# EnabledControlParameterSummaryTypeDef definition

class EnabledControlParameterSummaryTypeDef(TypedDict):
    key: str,
    value: Dict[str, Any],
```

## RegionTypeDef

```python
# RegionTypeDef definition

class RegionTypeDef(TypedDict):
    name: NotRequired[str],
```

## EnabledControlFilterTypeDef

```python
# EnabledControlFilterTypeDef definition

class EnabledControlFilterTypeDef(TypedDict):
    controlIdentifiers: NotRequired[Sequence[str]],
    driftStatuses: NotRequired[Sequence[DriftStatusType]],  # (1)
    statuses: NotRequired[Sequence[EnablementStatusType]],  # (2)
```

1. See [:material-code-brackets: DriftStatusType](./literals.md#driftstatustype) 
2. See [:material-code-brackets: EnablementStatusType](./literals.md#enablementstatustype) 
## GetBaselineInputRequestTypeDef

```python
# GetBaselineInputRequestTypeDef definition

class GetBaselineInputRequestTypeDef(TypedDict):
    baselineIdentifier: str,
```

## GetBaselineOperationInputRequestTypeDef

```python
# GetBaselineOperationInputRequestTypeDef definition

class GetBaselineOperationInputRequestTypeDef(TypedDict):
    operationIdentifier: str,
```

## GetControlOperationInputRequestTypeDef

```python
# GetControlOperationInputRequestTypeDef definition

class GetControlOperationInputRequestTypeDef(TypedDict):
    operationIdentifier: str,
```

## GetEnabledBaselineInputRequestTypeDef

```python
# GetEnabledBaselineInputRequestTypeDef definition

class GetEnabledBaselineInputRequestTypeDef(TypedDict):
    enabledBaselineIdentifier: str,
```

## GetEnabledControlInputRequestTypeDef

```python
# GetEnabledControlInputRequestTypeDef definition

class GetEnabledControlInputRequestTypeDef(TypedDict):
    enabledControlIdentifier: str,
```

## GetLandingZoneInputRequestTypeDef

```python
# GetLandingZoneInputRequestTypeDef definition

class GetLandingZoneInputRequestTypeDef(TypedDict):
    landingZoneIdentifier: str,
```

## GetLandingZoneOperationInputRequestTypeDef

```python
# GetLandingZoneOperationInputRequestTypeDef definition

class GetLandingZoneOperationInputRequestTypeDef(TypedDict):
    operationIdentifier: str,
```

## LandingZoneOperationDetailTypeDef

```python
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
# LandingZoneDriftStatusSummaryTypeDef definition

class LandingZoneDriftStatusSummaryTypeDef(TypedDict):
    status: NotRequired[LandingZoneDriftStatusType],  # (1)
```

1. See [:material-code-brackets: LandingZoneDriftStatusType](./literals.md#landingzonedriftstatustype) 
## LandingZoneOperationFilterTypeDef

```python
# LandingZoneOperationFilterTypeDef definition

class LandingZoneOperationFilterTypeDef(TypedDict):
    statuses: NotRequired[Sequence[LandingZoneOperationStatusType]],  # (1)
    types: NotRequired[Sequence[LandingZoneOperationTypeType]],  # (2)
```

1. See [:material-code-brackets: LandingZoneOperationStatusType](./literals.md#landingzoneoperationstatustype) 
2. See [:material-code-brackets: LandingZoneOperationTypeType](./literals.md#landingzoneoperationtypetype) 
## LandingZoneOperationSummaryTypeDef

```python
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
# LandingZoneSummaryTypeDef definition

class LandingZoneSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListBaselinesInputRequestTypeDef

```python
# ListBaselinesInputRequestTypeDef definition

class ListBaselinesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListLandingZonesInputRequestTypeDef

```python
# ListLandingZonesInputRequestTypeDef definition

class ListLandingZonesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ResetEnabledBaselineInputRequestTypeDef

```python
# ResetEnabledBaselineInputRequestTypeDef definition

class ResetEnabledBaselineInputRequestTypeDef(TypedDict):
    enabledBaselineIdentifier: str,
```

## ResetEnabledControlInputRequestTypeDef

```python
# ResetEnabledControlInputRequestTypeDef definition

class ResetEnabledControlInputRequestTypeDef(TypedDict):
    enabledControlIdentifier: str,
```

## ResetLandingZoneInputRequestTypeDef

```python
# ResetLandingZoneInputRequestTypeDef definition

class ResetLandingZoneInputRequestTypeDef(TypedDict):
    landingZoneIdentifier: str,
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateLandingZoneInputRequestTypeDef

```python
# UpdateLandingZoneInputRequestTypeDef definition

class UpdateLandingZoneInputRequestTypeDef(TypedDict):
    landingZoneIdentifier: str,
    manifest: Mapping[str, Any],
    version: str,
```

## ListControlOperationsInputRequestTypeDef

```python
# ListControlOperationsInputRequestTypeDef definition

class ListControlOperationsInputRequestTypeDef(TypedDict):
    filter: NotRequired[ControlOperationFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ControlOperationFilterTypeDef](./type_defs.md#controloperationfiltertypedef) 
## CreateLandingZoneOutputTypeDef

```python
# CreateLandingZoneOutputTypeDef definition

class CreateLandingZoneOutputTypeDef(TypedDict):
    arn: str,
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteLandingZoneOutputTypeDef

```python
# DeleteLandingZoneOutputTypeDef definition

class DeleteLandingZoneOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableBaselineOutputTypeDef

```python
# DisableBaselineOutputTypeDef definition

class DisableBaselineOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableControlOutputTypeDef

```python
# DisableControlOutputTypeDef definition

class DisableControlOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableBaselineOutputTypeDef

```python
# EnableBaselineOutputTypeDef definition

class EnableBaselineOutputTypeDef(TypedDict):
    arn: str,
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableControlOutputTypeDef

```python
# EnableControlOutputTypeDef definition

class EnableControlOutputTypeDef(TypedDict):
    arn: str,
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBaselineOperationOutputTypeDef

```python
# GetBaselineOperationOutputTypeDef definition

class GetBaselineOperationOutputTypeDef(TypedDict):
    baselineOperation: BaselineOperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BaselineOperationTypeDef](./type_defs.md#baselineoperationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBaselineOutputTypeDef

```python
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
# GetControlOperationOutputTypeDef definition

class GetControlOperationOutputTypeDef(TypedDict):
    controlOperation: ControlOperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ControlOperationTypeDef](./type_defs.md#controloperationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBaselinesOutputTypeDef

```python
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
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetEnabledBaselineOutputTypeDef

```python
# ResetEnabledBaselineOutputTypeDef definition

class ResetEnabledBaselineOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetEnabledControlOutputTypeDef

```python
# ResetEnabledControlOutputTypeDef definition

class ResetEnabledControlOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetLandingZoneOutputTypeDef

```python
# ResetLandingZoneOutputTypeDef definition

class ResetLandingZoneOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnabledBaselineOutputTypeDef

```python
# UpdateEnabledBaselineOutputTypeDef definition

class UpdateEnabledBaselineOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnabledControlOutputTypeDef

```python
# UpdateEnabledControlOutputTypeDef definition

class UpdateEnabledControlOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLandingZoneOutputTypeDef

```python
# UpdateLandingZoneOutputTypeDef definition

class UpdateLandingZoneOutputTypeDef(TypedDict):
    operationIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableBaselineInputRequestTypeDef

```python
# EnableBaselineInputRequestTypeDef definition

class EnableBaselineInputRequestTypeDef(TypedDict):
    baselineIdentifier: str,
    baselineVersion: str,
    targetIdentifier: str,
    parameters: NotRequired[Sequence[EnabledBaselineParameterTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: EnabledBaselineParameterTypeDef](./type_defs.md#enabledbaselineparametertypedef) 
## UpdateEnabledBaselineInputRequestTypeDef

```python
# UpdateEnabledBaselineInputRequestTypeDef definition

class UpdateEnabledBaselineInputRequestTypeDef(TypedDict):
    baselineVersion: str,
    enabledBaselineIdentifier: str,
    parameters: NotRequired[Sequence[EnabledBaselineParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: EnabledBaselineParameterTypeDef](./type_defs.md#enabledbaselineparametertypedef) 
## EnableControlInputRequestTypeDef

```python
# EnableControlInputRequestTypeDef definition

class EnableControlInputRequestTypeDef(TypedDict):
    controlIdentifier: str,
    targetIdentifier: str,
    parameters: NotRequired[Sequence[EnabledControlParameterTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: EnabledControlParameterTypeDef](./type_defs.md#enabledcontrolparametertypedef) 
## UpdateEnabledControlInputRequestTypeDef

```python
# UpdateEnabledControlInputRequestTypeDef definition

class UpdateEnabledControlInputRequestTypeDef(TypedDict):
    enabledControlIdentifier: str,
    parameters: Sequence[EnabledControlParameterTypeDef],  # (1)
```

1. See [:material-code-braces: EnabledControlParameterTypeDef](./type_defs.md#enabledcontrolparametertypedef) 
## EnabledBaselineDetailsTypeDef

```python
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
## ListEnabledBaselinesInputRequestTypeDef

```python
# ListEnabledBaselinesInputRequestTypeDef definition

class ListEnabledBaselinesInputRequestTypeDef(TypedDict):
    filter: NotRequired[EnabledBaselineFilterTypeDef],  # (1)
    includeChildren: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnabledBaselineFilterTypeDef](./type_defs.md#enabledbaselinefiltertypedef) 
## EnabledControlDetailsTypeDef

```python
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
## ListEnabledControlsInputRequestTypeDef

```python
# ListEnabledControlsInputRequestTypeDef definition

class ListEnabledControlsInputRequestTypeDef(TypedDict):
    filter: NotRequired[EnabledControlFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    targetIdentifier: NotRequired[str],
```

1. See [:material-code-braces: EnabledControlFilterTypeDef](./type_defs.md#enabledcontrolfiltertypedef) 
## GetLandingZoneOperationOutputTypeDef

```python
# GetLandingZoneOperationOutputTypeDef definition

class GetLandingZoneOperationOutputTypeDef(TypedDict):
    operationDetails: LandingZoneOperationDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LandingZoneOperationDetailTypeDef](./type_defs.md#landingzoneoperationdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LandingZoneDetailTypeDef

```python
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
## ListLandingZoneOperationsInputRequestTypeDef

```python
# ListLandingZoneOperationsInputRequestTypeDef definition

class ListLandingZoneOperationsInputRequestTypeDef(TypedDict):
    filter: NotRequired[LandingZoneOperationFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LandingZoneOperationFilterTypeDef](./type_defs.md#landingzoneoperationfiltertypedef) 
## ListLandingZoneOperationsOutputTypeDef

```python
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
# ListBaselinesInputPaginateTypeDef definition

class ListBaselinesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListControlOperationsInputPaginateTypeDef

```python
# ListControlOperationsInputPaginateTypeDef definition

class ListControlOperationsInputPaginateTypeDef(TypedDict):
    filter: NotRequired[ControlOperationFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ControlOperationFilterTypeDef](./type_defs.md#controloperationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnabledBaselinesInputPaginateTypeDef

```python
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
# ListLandingZoneOperationsInputPaginateTypeDef definition

class ListLandingZoneOperationsInputPaginateTypeDef(TypedDict):
    filter: NotRequired[LandingZoneOperationFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: LandingZoneOperationFilterTypeDef](./type_defs.md#landingzoneoperationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLandingZonesInputPaginateTypeDef

```python
# ListLandingZonesInputPaginateTypeDef definition

class ListLandingZonesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetEnabledBaselineOutputTypeDef

```python
# GetEnabledBaselineOutputTypeDef definition

class GetEnabledBaselineOutputTypeDef(TypedDict):
    enabledBaselineDetails: EnabledBaselineDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnabledBaselineDetailsTypeDef](./type_defs.md#enabledbaselinedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnabledBaselinesOutputTypeDef

```python
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
# GetEnabledControlOutputTypeDef definition

class GetEnabledControlOutputTypeDef(TypedDict):
    enabledControlDetails: EnabledControlDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnabledControlDetailsTypeDef](./type_defs.md#enabledcontroldetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLandingZoneOutputTypeDef

```python
# GetLandingZoneOutputTypeDef definition

class GetLandingZoneOutputTypeDef(TypedDict):
    landingZone: LandingZoneDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LandingZoneDetailTypeDef](./type_defs.md#landingzonedetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
