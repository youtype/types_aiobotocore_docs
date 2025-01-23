# Type definitions

> [Index](../README.md) > [WorkSpacesThinClient](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WorkSpacesThinClient](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#workspacesthinclient)
    type annotations stubs module [types-aiobotocore-workspaces-thin-client](https://pypi.org/project/types-aiobotocore-workspaces-thin-client/).



## MaintenanceWindowTypeDef

```python
# MaintenanceWindowTypeDef definition

class MaintenanceWindowTypeDef(TypedDict):
    type: MaintenanceWindowTypeType,  # (1)
    startTimeHour: NotRequired[int],
    startTimeMinute: NotRequired[int],
    endTimeHour: NotRequired[int],
    endTimeMinute: NotRequired[int],
    daysOfTheWeek: NotRequired[Sequence[DayOfWeekType]],  # (2)
    applyTimeOf: NotRequired[ApplyTimeOfType],  # (3)
```

1. See [:material-code-brackets: MaintenanceWindowTypeType](./literals.md#maintenancewindowtypetype) 
2. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
3. See [:material-code-brackets: ApplyTimeOfType](./literals.md#applytimeoftype) 
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

## DeleteDeviceRequestRequestTypeDef

```python
# DeleteDeviceRequestRequestTypeDef definition

class DeleteDeviceRequestRequestTypeDef(TypedDict):
    id: str,
    clientToken: NotRequired[str],
```

## DeleteEnvironmentRequestRequestTypeDef

```python
# DeleteEnvironmentRequestRequestTypeDef definition

class DeleteEnvironmentRequestRequestTypeDef(TypedDict):
    id: str,
    clientToken: NotRequired[str],
```

## DeregisterDeviceRequestRequestTypeDef

```python
# DeregisterDeviceRequestRequestTypeDef definition

class DeregisterDeviceRequestRequestTypeDef(TypedDict):
    id: str,
    targetDeviceStatus: NotRequired[TargetDeviceStatusType],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: TargetDeviceStatusType](./literals.md#targetdevicestatustype) 
## DeviceSummaryTypeDef

```python
# DeviceSummaryTypeDef definition

class DeviceSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    serialNumber: NotRequired[str],
    name: NotRequired[str],
    model: NotRequired[str],
    environmentId: NotRequired[str],
    status: NotRequired[DeviceStatusType],  # (1)
    currentSoftwareSetId: NotRequired[str],
    desiredSoftwareSetId: NotRequired[str],
    pendingSoftwareSetId: NotRequired[str],
    softwareSetUpdateSchedule: NotRequired[SoftwareSetUpdateScheduleType],  # (2)
    lastConnectedAt: NotRequired[datetime],
    lastPostureAt: NotRequired[datetime],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    arn: NotRequired[str],
```

1. See [:material-code-brackets: DeviceStatusType](./literals.md#devicestatustype) 
2. See [:material-code-brackets: SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype) 
## DeviceTypeDef

```python
# DeviceTypeDef definition

class DeviceTypeDef(TypedDict):
    id: NotRequired[str],
    serialNumber: NotRequired[str],
    name: NotRequired[str],
    model: NotRequired[str],
    environmentId: NotRequired[str],
    status: NotRequired[DeviceStatusType],  # (1)
    currentSoftwareSetId: NotRequired[str],
    currentSoftwareSetVersion: NotRequired[str],
    desiredSoftwareSetId: NotRequired[str],
    pendingSoftwareSetId: NotRequired[str],
    pendingSoftwareSetVersion: NotRequired[str],
    softwareSetUpdateSchedule: NotRequired[SoftwareSetUpdateScheduleType],  # (2)
    softwareSetComplianceStatus: NotRequired[DeviceSoftwareSetComplianceStatusType],  # (3)
    softwareSetUpdateStatus: NotRequired[SoftwareSetUpdateStatusType],  # (4)
    lastConnectedAt: NotRequired[datetime],
    lastPostureAt: NotRequired[datetime],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    arn: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: DeviceStatusType](./literals.md#devicestatustype) 
2. See [:material-code-brackets: SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype) 
3. See [:material-code-brackets: DeviceSoftwareSetComplianceStatusType](./literals.md#devicesoftwaresetcompliancestatustype) 
4. See [:material-code-brackets: SoftwareSetUpdateStatusType](./literals.md#softwaresetupdatestatustype) 
## MaintenanceWindowOutputTypeDef

```python
# MaintenanceWindowOutputTypeDef definition

class MaintenanceWindowOutputTypeDef(TypedDict):
    type: MaintenanceWindowTypeType,  # (1)
    startTimeHour: NotRequired[int],
    startTimeMinute: NotRequired[int],
    endTimeHour: NotRequired[int],
    endTimeMinute: NotRequired[int],
    daysOfTheWeek: NotRequired[List[DayOfWeekType]],  # (2)
    applyTimeOf: NotRequired[ApplyTimeOfType],  # (3)
```

1. See [:material-code-brackets: MaintenanceWindowTypeType](./literals.md#maintenancewindowtypetype) 
2. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
3. See [:material-code-brackets: ApplyTimeOfType](./literals.md#applytimeoftype) 
## GetDeviceRequestRequestTypeDef

```python
# GetDeviceRequestRequestTypeDef definition

class GetDeviceRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetEnvironmentRequestRequestTypeDef

```python
# GetEnvironmentRequestRequestTypeDef definition

class GetEnvironmentRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetSoftwareSetRequestRequestTypeDef

```python
# GetSoftwareSetRequestRequestTypeDef definition

class GetSoftwareSetRequestRequestTypeDef(TypedDict):
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

## ListDevicesRequestRequestTypeDef

```python
# ListDevicesRequestRequestTypeDef definition

class ListDevicesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListEnvironmentsRequestRequestTypeDef

```python
# ListEnvironmentsRequestRequestTypeDef definition

class ListEnvironmentsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListSoftwareSetsRequestRequestTypeDef

```python
# ListSoftwareSetsRequestRequestTypeDef definition

class ListSoftwareSetsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## SoftwareSetSummaryTypeDef

```python
# SoftwareSetSummaryTypeDef definition

class SoftwareSetSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    version: NotRequired[str],
    releasedAt: NotRequired[datetime],
    supportedUntil: NotRequired[datetime],
    validationStatus: NotRequired[SoftwareSetValidationStatusType],  # (1)
    arn: NotRequired[str],
```

1. See [:material-code-brackets: SoftwareSetValidationStatusType](./literals.md#softwaresetvalidationstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## SoftwareTypeDef

```python
# SoftwareTypeDef definition

class SoftwareTypeDef(TypedDict):
    name: NotRequired[str],
    version: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateDeviceRequestRequestTypeDef

```python
# UpdateDeviceRequestRequestTypeDef definition

class UpdateDeviceRequestRequestTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    desiredSoftwareSetId: NotRequired[str],
    softwareSetUpdateSchedule: NotRequired[SoftwareSetUpdateScheduleType],  # (1)
```

1. See [:material-code-brackets: SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype) 
## UpdateSoftwareSetRequestRequestTypeDef

```python
# UpdateSoftwareSetRequestRequestTypeDef definition

class UpdateSoftwareSetRequestRequestTypeDef(TypedDict):
    id: str,
    validationStatus: SoftwareSetValidationStatusType,  # (1)
```

1. See [:material-code-brackets: SoftwareSetValidationStatusType](./literals.md#softwaresetvalidationstatustype) 
## CreateEnvironmentRequestRequestTypeDef

```python
# CreateEnvironmentRequestRequestTypeDef definition

class CreateEnvironmentRequestRequestTypeDef(TypedDict):
    desktopArn: str,
    name: NotRequired[str],
    desktopEndpoint: NotRequired[str],
    softwareSetUpdateSchedule: NotRequired[SoftwareSetUpdateScheduleType],  # (1)
    maintenanceWindow: NotRequired[MaintenanceWindowTypeDef],  # (2)
    softwareSetUpdateMode: NotRequired[SoftwareSetUpdateModeType],  # (3)
    desiredSoftwareSetId: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    deviceCreationTags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype) 
2. See [:material-code-braces: MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef) 
3. See [:material-code-brackets: SoftwareSetUpdateModeType](./literals.md#softwaresetupdatemodetype) 
## UpdateEnvironmentRequestRequestTypeDef

```python
# UpdateEnvironmentRequestRequestTypeDef definition

class UpdateEnvironmentRequestRequestTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    desktopArn: NotRequired[str],
    desktopEndpoint: NotRequired[str],
    softwareSetUpdateSchedule: NotRequired[SoftwareSetUpdateScheduleType],  # (1)
    maintenanceWindow: NotRequired[MaintenanceWindowTypeDef],  # (2)
    softwareSetUpdateMode: NotRequired[SoftwareSetUpdateModeType],  # (3)
    desiredSoftwareSetId: NotRequired[str],
    deviceCreationTags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype) 
2. See [:material-code-braces: MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef) 
3. See [:material-code-brackets: SoftwareSetUpdateModeType](./literals.md#softwaresetupdatemodetype) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDevicesResponseTypeDef

```python
# ListDevicesResponseTypeDef definition

class ListDevicesResponseTypeDef(TypedDict):
    devices: List[DeviceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceSummaryTypeDef](./type_defs.md#devicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDeviceResponseTypeDef

```python
# UpdateDeviceResponseTypeDef definition

class UpdateDeviceResponseTypeDef(TypedDict):
    device: DeviceSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceSummaryTypeDef](./type_defs.md#devicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeviceResponseTypeDef

```python
# GetDeviceResponseTypeDef definition

class GetDeviceResponseTypeDef(TypedDict):
    device: DeviceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentSummaryTypeDef

```python
# EnvironmentSummaryTypeDef definition

class EnvironmentSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    desktopArn: NotRequired[str],
    desktopEndpoint: NotRequired[str],
    desktopType: NotRequired[DesktopTypeType],  # (1)
    activationCode: NotRequired[str],
    softwareSetUpdateSchedule: NotRequired[SoftwareSetUpdateScheduleType],  # (2)
    maintenanceWindow: NotRequired[MaintenanceWindowOutputTypeDef],  # (3)
    softwareSetUpdateMode: NotRequired[SoftwareSetUpdateModeType],  # (4)
    desiredSoftwareSetId: NotRequired[str],
    pendingSoftwareSetId: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    arn: NotRequired[str],
```

1. See [:material-code-brackets: DesktopTypeType](./literals.md#desktoptypetype) 
2. See [:material-code-brackets: SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype) 
3. See [:material-code-braces: MaintenanceWindowOutputTypeDef](./type_defs.md#maintenancewindowoutputtypedef) 
4. See [:material-code-brackets: SoftwareSetUpdateModeType](./literals.md#softwaresetupdatemodetype) 
## EnvironmentTypeDef

```python
# EnvironmentTypeDef definition

class EnvironmentTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    desktopArn: NotRequired[str],
    desktopEndpoint: NotRequired[str],
    desktopType: NotRequired[DesktopTypeType],  # (1)
    activationCode: NotRequired[str],
    registeredDevicesCount: NotRequired[int],
    softwareSetUpdateSchedule: NotRequired[SoftwareSetUpdateScheduleType],  # (2)
    maintenanceWindow: NotRequired[MaintenanceWindowOutputTypeDef],  # (3)
    softwareSetUpdateMode: NotRequired[SoftwareSetUpdateModeType],  # (4)
    desiredSoftwareSetId: NotRequired[str],
    pendingSoftwareSetId: NotRequired[str],
    pendingSoftwareSetVersion: NotRequired[str],
    softwareSetComplianceStatus: NotRequired[EnvironmentSoftwareSetComplianceStatusType],  # (5)
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    arn: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    deviceCreationTags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: DesktopTypeType](./literals.md#desktoptypetype) 
2. See [:material-code-brackets: SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype) 
3. See [:material-code-braces: MaintenanceWindowOutputTypeDef](./type_defs.md#maintenancewindowoutputtypedef) 
4. See [:material-code-brackets: SoftwareSetUpdateModeType](./literals.md#softwaresetupdatemodetype) 
5. See [:material-code-brackets: EnvironmentSoftwareSetComplianceStatusType](./literals.md#environmentsoftwaresetcompliancestatustype) 
## ListDevicesRequestPaginateTypeDef

```python
# ListDevicesRequestPaginateTypeDef definition

class ListDevicesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentsRequestPaginateTypeDef

```python
# ListEnvironmentsRequestPaginateTypeDef definition

class ListEnvironmentsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSoftwareSetsRequestPaginateTypeDef

```python
# ListSoftwareSetsRequestPaginateTypeDef definition

class ListSoftwareSetsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSoftwareSetsResponseTypeDef

```python
# ListSoftwareSetsResponseTypeDef definition

class ListSoftwareSetsResponseTypeDef(TypedDict):
    softwareSets: List[SoftwareSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SoftwareSetSummaryTypeDef](./type_defs.md#softwaresetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SoftwareSetTypeDef

```python
# SoftwareSetTypeDef definition

class SoftwareSetTypeDef(TypedDict):
    id: NotRequired[str],
    version: NotRequired[str],
    releasedAt: NotRequired[datetime],
    supportedUntil: NotRequired[datetime],
    validationStatus: NotRequired[SoftwareSetValidationStatusType],  # (1)
    software: NotRequired[List[SoftwareTypeDef]],  # (2)
    arn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: SoftwareSetValidationStatusType](./literals.md#softwaresetvalidationstatustype) 
2. See [:material-code-braces: SoftwareTypeDef](./type_defs.md#softwaretypedef) 
## CreateEnvironmentResponseTypeDef

```python
# CreateEnvironmentResponseTypeDef definition

class CreateEnvironmentResponseTypeDef(TypedDict):
    environment: EnvironmentSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentSummaryTypeDef](./type_defs.md#environmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentsResponseTypeDef

```python
# ListEnvironmentsResponseTypeDef definition

class ListEnvironmentsResponseTypeDef(TypedDict):
    environments: List[EnvironmentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentSummaryTypeDef](./type_defs.md#environmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentResponseTypeDef

```python
# UpdateEnvironmentResponseTypeDef definition

class UpdateEnvironmentResponseTypeDef(TypedDict):
    environment: EnvironmentSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentSummaryTypeDef](./type_defs.md#environmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnvironmentResponseTypeDef

```python
# GetEnvironmentResponseTypeDef definition

class GetEnvironmentResponseTypeDef(TypedDict):
    environment: EnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSoftwareSetResponseTypeDef

```python
# GetSoftwareSetResponseTypeDef definition

class GetSoftwareSetResponseTypeDef(TypedDict):
    softwareSet: SoftwareSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SoftwareSetTypeDef](./type_defs.md#softwaresettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
