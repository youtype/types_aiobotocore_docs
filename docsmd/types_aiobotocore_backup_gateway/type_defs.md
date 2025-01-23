# Type definitions

> [Index](../README.md) > [BackupGateway](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [BackupGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#backupgateway)
    type annotations stubs module [types-aiobotocore-backup-gateway](https://pypi.org/project/types-aiobotocore-backup-gateway/).

## BandwidthRateLimitIntervalUnionTypeDef

```python
# BandwidthRateLimitIntervalUnionTypeDef definition

BandwidthRateLimitIntervalUnionTypeDef = Union[
    BandwidthRateLimitIntervalTypeDef,  # (1)
    BandwidthRateLimitIntervalOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BandwidthRateLimitIntervalTypeDef](./type_defs.md#bandwidthratelimitintervaltypedef) 
2. See [:material-code-braces: BandwidthRateLimitIntervalOutputTypeDef](./type_defs.md#bandwidthratelimitintervaloutputtypedef) 



## AssociateGatewayToServerInputRequestTypeDef

```python
# AssociateGatewayToServerInputRequestTypeDef definition

class AssociateGatewayToServerInputRequestTypeDef(TypedDict):
    GatewayArn: str,
    ServerArn: str,
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

## BandwidthRateLimitIntervalOutputTypeDef

```python
# BandwidthRateLimitIntervalOutputTypeDef definition

class BandwidthRateLimitIntervalOutputTypeDef(TypedDict):
    DaysOfWeek: List[int],
    EndHourOfDay: int,
    EndMinuteOfHour: int,
    StartHourOfDay: int,
    StartMinuteOfHour: int,
    AverageUploadRateLimitInBitsPerSec: NotRequired[int],
```

## BandwidthRateLimitIntervalTypeDef

```python
# BandwidthRateLimitIntervalTypeDef definition

class BandwidthRateLimitIntervalTypeDef(TypedDict):
    DaysOfWeek: Sequence[int],
    EndHourOfDay: int,
    EndMinuteOfHour: int,
    StartHourOfDay: int,
    StartMinuteOfHour: int,
    AverageUploadRateLimitInBitsPerSec: NotRequired[int],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DeleteGatewayInputRequestTypeDef

```python
# DeleteGatewayInputRequestTypeDef definition

class DeleteGatewayInputRequestTypeDef(TypedDict):
    GatewayArn: str,
```

## DeleteHypervisorInputRequestTypeDef

```python
# DeleteHypervisorInputRequestTypeDef definition

class DeleteHypervisorInputRequestTypeDef(TypedDict):
    HypervisorArn: str,
```

## DisassociateGatewayFromServerInputRequestTypeDef

```python
# DisassociateGatewayFromServerInputRequestTypeDef definition

class DisassociateGatewayFromServerInputRequestTypeDef(TypedDict):
    GatewayArn: str,
```

## MaintenanceStartTimeTypeDef

```python
# MaintenanceStartTimeTypeDef definition

class MaintenanceStartTimeTypeDef(TypedDict):
    HourOfDay: int,
    MinuteOfHour: int,
    DayOfMonth: NotRequired[int],
    DayOfWeek: NotRequired[int],
```

## GatewayTypeDef

```python
# GatewayTypeDef definition

class GatewayTypeDef(TypedDict):
    GatewayArn: NotRequired[str],
    GatewayDisplayName: NotRequired[str],
    GatewayType: NotRequired[GatewayTypeType],  # (1)
    HypervisorId: NotRequired[str],
    LastSeenTime: NotRequired[datetime],
```

1. See [:material-code-brackets: GatewayTypeType](./literals.md#gatewaytypetype) 
## GetBandwidthRateLimitScheduleInputRequestTypeDef

```python
# GetBandwidthRateLimitScheduleInputRequestTypeDef definition

class GetBandwidthRateLimitScheduleInputRequestTypeDef(TypedDict):
    GatewayArn: str,
```

## GetGatewayInputRequestTypeDef

```python
# GetGatewayInputRequestTypeDef definition

class GetGatewayInputRequestTypeDef(TypedDict):
    GatewayArn: str,
```

## GetHypervisorInputRequestTypeDef

```python
# GetHypervisorInputRequestTypeDef definition

class GetHypervisorInputRequestTypeDef(TypedDict):
    HypervisorArn: str,
```

## HypervisorDetailsTypeDef

```python
# HypervisorDetailsTypeDef definition

class HypervisorDetailsTypeDef(TypedDict):
    Host: NotRequired[str],
    HypervisorArn: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    LastSuccessfulMetadataSyncTime: NotRequired[datetime],
    LatestMetadataSyncStatus: NotRequired[SyncMetadataStatusType],  # (1)
    LatestMetadataSyncStatusMessage: NotRequired[str],
    LogGroupArn: NotRequired[str],
    Name: NotRequired[str],
    State: NotRequired[HypervisorStateType],  # (2)
```

1. See [:material-code-brackets: SyncMetadataStatusType](./literals.md#syncmetadatastatustype) 
2. See [:material-code-brackets: HypervisorStateType](./literals.md#hypervisorstatetype) 
## GetHypervisorPropertyMappingsInputRequestTypeDef

```python
# GetHypervisorPropertyMappingsInputRequestTypeDef definition

class GetHypervisorPropertyMappingsInputRequestTypeDef(TypedDict):
    HypervisorArn: str,
```

## VmwareToAwsTagMappingTypeDef

```python
# VmwareToAwsTagMappingTypeDef definition

class VmwareToAwsTagMappingTypeDef(TypedDict):
    AwsTagKey: str,
    AwsTagValue: str,
    VmwareCategory: str,
    VmwareTagName: str,
```

## GetVirtualMachineInputRequestTypeDef

```python
# GetVirtualMachineInputRequestTypeDef definition

class GetVirtualMachineInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## HypervisorTypeDef

```python
# HypervisorTypeDef definition

class HypervisorTypeDef(TypedDict):
    Host: NotRequired[str],
    HypervisorArn: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    Name: NotRequired[str],
    State: NotRequired[HypervisorStateType],  # (1)
```

1. See [:material-code-brackets: HypervisorStateType](./literals.md#hypervisorstatetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListGatewaysInputRequestTypeDef

```python
# ListGatewaysInputRequestTypeDef definition

class ListGatewaysInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListHypervisorsInputRequestTypeDef

```python
# ListHypervisorsInputRequestTypeDef definition

class ListHypervisorsInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListVirtualMachinesInputRequestTypeDef

```python
# ListVirtualMachinesInputRequestTypeDef definition

class ListVirtualMachinesInputRequestTypeDef(TypedDict):
    HypervisorArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## VirtualMachineTypeDef

```python
# VirtualMachineTypeDef definition

class VirtualMachineTypeDef(TypedDict):
    HostName: NotRequired[str],
    HypervisorId: NotRequired[str],
    LastBackupDate: NotRequired[datetime],
    Name: NotRequired[str],
    Path: NotRequired[str],
    ResourceArn: NotRequired[str],
```

## PutMaintenanceStartTimeInputRequestTypeDef

```python
# PutMaintenanceStartTimeInputRequestTypeDef definition

class PutMaintenanceStartTimeInputRequestTypeDef(TypedDict):
    GatewayArn: str,
    HourOfDay: int,
    MinuteOfHour: int,
    DayOfMonth: NotRequired[int],
    DayOfWeek: NotRequired[int],
```

## StartVirtualMachinesMetadataSyncInputRequestTypeDef

```python
# StartVirtualMachinesMetadataSyncInputRequestTypeDef definition

class StartVirtualMachinesMetadataSyncInputRequestTypeDef(TypedDict):
    HypervisorArn: str,
```

## TestHypervisorConfigurationInputRequestTypeDef

```python
# TestHypervisorConfigurationInputRequestTypeDef definition

class TestHypervisorConfigurationInputRequestTypeDef(TypedDict):
    GatewayArn: str,
    Host: str,
    Password: NotRequired[str],
    Username: NotRequired[str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateGatewayInformationInputRequestTypeDef

```python
# UpdateGatewayInformationInputRequestTypeDef definition

class UpdateGatewayInformationInputRequestTypeDef(TypedDict):
    GatewayArn: str,
    GatewayDisplayName: NotRequired[str],
```

## UpdateGatewaySoftwareNowInputRequestTypeDef

```python
# UpdateGatewaySoftwareNowInputRequestTypeDef definition

class UpdateGatewaySoftwareNowInputRequestTypeDef(TypedDict):
    GatewayArn: str,
```

## UpdateHypervisorInputRequestTypeDef

```python
# UpdateHypervisorInputRequestTypeDef definition

class UpdateHypervisorInputRequestTypeDef(TypedDict):
    HypervisorArn: str,
    Host: NotRequired[str],
    LogGroupArn: NotRequired[str],
    Name: NotRequired[str],
    Password: NotRequired[str],
    Username: NotRequired[str],
```

## VmwareTagTypeDef

```python
# VmwareTagTypeDef definition

class VmwareTagTypeDef(TypedDict):
    VmwareCategory: NotRequired[str],
    VmwareTagDescription: NotRequired[str],
    VmwareTagName: NotRequired[str],
```

## AssociateGatewayToServerOutputTypeDef

```python
# AssociateGatewayToServerOutputTypeDef definition

class AssociateGatewayToServerOutputTypeDef(TypedDict):
    GatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGatewayOutputTypeDef

```python
# CreateGatewayOutputTypeDef definition

class CreateGatewayOutputTypeDef(TypedDict):
    GatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGatewayOutputTypeDef

```python
# DeleteGatewayOutputTypeDef definition

class DeleteGatewayOutputTypeDef(TypedDict):
    GatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteHypervisorOutputTypeDef

```python
# DeleteHypervisorOutputTypeDef definition

class DeleteHypervisorOutputTypeDef(TypedDict):
    HypervisorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateGatewayFromServerOutputTypeDef

```python
# DisassociateGatewayFromServerOutputTypeDef definition

class DisassociateGatewayFromServerOutputTypeDef(TypedDict):
    GatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportHypervisorConfigurationOutputTypeDef

```python
# ImportHypervisorConfigurationOutputTypeDef definition

class ImportHypervisorConfigurationOutputTypeDef(TypedDict):
    HypervisorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutBandwidthRateLimitScheduleOutputTypeDef

```python
# PutBandwidthRateLimitScheduleOutputTypeDef definition

class PutBandwidthRateLimitScheduleOutputTypeDef(TypedDict):
    GatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutHypervisorPropertyMappingsOutputTypeDef

```python
# PutHypervisorPropertyMappingsOutputTypeDef definition

class PutHypervisorPropertyMappingsOutputTypeDef(TypedDict):
    HypervisorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutMaintenanceStartTimeOutputTypeDef

```python
# PutMaintenanceStartTimeOutputTypeDef definition

class PutMaintenanceStartTimeOutputTypeDef(TypedDict):
    GatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartVirtualMachinesMetadataSyncOutputTypeDef

```python
# StartVirtualMachinesMetadataSyncOutputTypeDef definition

class StartVirtualMachinesMetadataSyncOutputTypeDef(TypedDict):
    HypervisorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceOutputTypeDef

```python
# TagResourceOutputTypeDef definition

class TagResourceOutputTypeDef(TypedDict):
    ResourceARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UntagResourceOutputTypeDef

```python
# UntagResourceOutputTypeDef definition

class UntagResourceOutputTypeDef(TypedDict):
    ResourceARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGatewayInformationOutputTypeDef

```python
# UpdateGatewayInformationOutputTypeDef definition

class UpdateGatewayInformationOutputTypeDef(TypedDict):
    GatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGatewaySoftwareNowOutputTypeDef

```python
# UpdateGatewaySoftwareNowOutputTypeDef definition

class UpdateGatewaySoftwareNowOutputTypeDef(TypedDict):
    GatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateHypervisorOutputTypeDef

```python
# UpdateHypervisorOutputTypeDef definition

class UpdateHypervisorOutputTypeDef(TypedDict):
    HypervisorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBandwidthRateLimitScheduleOutputTypeDef

```python
# GetBandwidthRateLimitScheduleOutputTypeDef definition

class GetBandwidthRateLimitScheduleOutputTypeDef(TypedDict):
    BandwidthRateLimitIntervals: List[BandwidthRateLimitIntervalOutputTypeDef],  # (1)
    GatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BandwidthRateLimitIntervalOutputTypeDef](./type_defs.md#bandwidthratelimitintervaloutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGatewayInputRequestTypeDef

```python
# CreateGatewayInputRequestTypeDef definition

class CreateGatewayInputRequestTypeDef(TypedDict):
    ActivationKey: str,
    GatewayDisplayName: str,
    GatewayType: GatewayTypeType,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: GatewayTypeType](./literals.md#gatewaytypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ImportHypervisorConfigurationInputRequestTypeDef

```python
# ImportHypervisorConfigurationInputRequestTypeDef definition

class ImportHypervisorConfigurationInputRequestTypeDef(TypedDict):
    Host: str,
    Name: str,
    KmsKeyArn: NotRequired[str],
    Password: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    Username: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    ResourceArn: str,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GatewayDetailsTypeDef

```python
# GatewayDetailsTypeDef definition

class GatewayDetailsTypeDef(TypedDict):
    GatewayArn: NotRequired[str],
    GatewayDisplayName: NotRequired[str],
    GatewayType: NotRequired[GatewayTypeType],  # (1)
    HypervisorId: NotRequired[str],
    LastSeenTime: NotRequired[datetime],
    MaintenanceStartTime: NotRequired[MaintenanceStartTimeTypeDef],  # (2)
    NextUpdateAvailabilityTime: NotRequired[datetime],
    VpcEndpoint: NotRequired[str],
```

1. See [:material-code-brackets: GatewayTypeType](./literals.md#gatewaytypetype) 
2. See [:material-code-braces: MaintenanceStartTimeTypeDef](./type_defs.md#maintenancestarttimetypedef) 
## ListGatewaysOutputTypeDef

```python
# ListGatewaysOutputTypeDef definition

class ListGatewaysOutputTypeDef(TypedDict):
    Gateways: List[GatewayTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GatewayTypeDef](./type_defs.md#gatewaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetHypervisorOutputTypeDef

```python
# GetHypervisorOutputTypeDef definition

class GetHypervisorOutputTypeDef(TypedDict):
    Hypervisor: HypervisorDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HypervisorDetailsTypeDef](./type_defs.md#hypervisordetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetHypervisorPropertyMappingsOutputTypeDef

```python
# GetHypervisorPropertyMappingsOutputTypeDef definition

class GetHypervisorPropertyMappingsOutputTypeDef(TypedDict):
    HypervisorArn: str,
    IamRoleArn: str,
    VmwareToAwsTagMappings: List[VmwareToAwsTagMappingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VmwareToAwsTagMappingTypeDef](./type_defs.md#vmwaretoawstagmappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutHypervisorPropertyMappingsInputRequestTypeDef

```python
# PutHypervisorPropertyMappingsInputRequestTypeDef definition

class PutHypervisorPropertyMappingsInputRequestTypeDef(TypedDict):
    HypervisorArn: str,
    IamRoleArn: str,
    VmwareToAwsTagMappings: Sequence[VmwareToAwsTagMappingTypeDef],  # (1)
```

1. See [:material-code-braces: VmwareToAwsTagMappingTypeDef](./type_defs.md#vmwaretoawstagmappingtypedef) 
## ListHypervisorsOutputTypeDef

```python
# ListHypervisorsOutputTypeDef definition

class ListHypervisorsOutputTypeDef(TypedDict):
    Hypervisors: List[HypervisorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HypervisorTypeDef](./type_defs.md#hypervisortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGatewaysInputPaginateTypeDef

```python
# ListGatewaysInputPaginateTypeDef definition

class ListGatewaysInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHypervisorsInputPaginateTypeDef

```python
# ListHypervisorsInputPaginateTypeDef definition

class ListHypervisorsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVirtualMachinesInputPaginateTypeDef

```python
# ListVirtualMachinesInputPaginateTypeDef definition

class ListVirtualMachinesInputPaginateTypeDef(TypedDict):
    HypervisorArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVirtualMachinesOutputTypeDef

```python
# ListVirtualMachinesOutputTypeDef definition

class ListVirtualMachinesOutputTypeDef(TypedDict):
    VirtualMachines: List[VirtualMachineTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VirtualMachineTypeDef](./type_defs.md#virtualmachinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VirtualMachineDetailsTypeDef

```python
# VirtualMachineDetailsTypeDef definition

class VirtualMachineDetailsTypeDef(TypedDict):
    HostName: NotRequired[str],
    HypervisorId: NotRequired[str],
    LastBackupDate: NotRequired[datetime],
    Name: NotRequired[str],
    Path: NotRequired[str],
    ResourceArn: NotRequired[str],
    VmwareTags: NotRequired[List[VmwareTagTypeDef]],  # (1)
```

1. See [:material-code-braces: VmwareTagTypeDef](./type_defs.md#vmwaretagtypedef) 
## PutBandwidthRateLimitScheduleInputRequestTypeDef

```python
# PutBandwidthRateLimitScheduleInputRequestTypeDef definition

class PutBandwidthRateLimitScheduleInputRequestTypeDef(TypedDict):
    BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef],  # (1)
    GatewayArn: str,
```

1. See [:material-code-braces: BandwidthRateLimitIntervalTypeDef](./type_defs.md#bandwidthratelimitintervaltypedef) [:material-code-braces: BandwidthRateLimitIntervalOutputTypeDef](./type_defs.md#bandwidthratelimitintervaloutputtypedef) 
## GetGatewayOutputTypeDef

```python
# GetGatewayOutputTypeDef definition

class GetGatewayOutputTypeDef(TypedDict):
    Gateway: GatewayDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayDetailsTypeDef](./type_defs.md#gatewaydetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVirtualMachineOutputTypeDef

```python
# GetVirtualMachineOutputTypeDef definition

class GetVirtualMachineOutputTypeDef(TypedDict):
    VirtualMachine: VirtualMachineDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualMachineDetailsTypeDef](./type_defs.md#virtualmachinedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
