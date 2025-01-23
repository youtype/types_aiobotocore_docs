# Type definitions

> [Index](../README.md) > [IoTWireless](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTWireless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#iotwireless)
    type annotations stubs module [types-aiobotocore-iotwireless](https://pypi.org/project/types-aiobotocore-iotwireless/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## BeaconingUnionTypeDef

```python
# BeaconingUnionTypeDef definition

BeaconingUnionTypeDef = Union[
    BeaconingTypeDef,  # (1)
    BeaconingOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BeaconingTypeDef](./type_defs.md#beaconingtypedef) 
2. See [:material-code-braces: BeaconingOutputTypeDef](./type_defs.md#beaconingoutputtypedef) 

## ParticipatingGatewaysMulticastUnionTypeDef

```python
# ParticipatingGatewaysMulticastUnionTypeDef definition

ParticipatingGatewaysMulticastUnionTypeDef = Union[
    ParticipatingGatewaysMulticastTypeDef,  # (1)
    ParticipatingGatewaysMulticastOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ParticipatingGatewaysMulticastTypeDef](./type_defs.md#participatinggatewaysmulticasttypedef) 
2. See [:material-code-braces: ParticipatingGatewaysMulticastOutputTypeDef](./type_defs.md#participatinggatewaysmulticastoutputtypedef) 

## FPortsUnionTypeDef

```python
# FPortsUnionTypeDef definition

FPortsUnionTypeDef = Union[
    FPortsTypeDef,  # (1)
    FPortsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FPortsTypeDef](./type_defs.md#fportstypedef) 
2. See [:material-code-braces: FPortsOutputTypeDef](./type_defs.md#fportsoutputtypedef) 

## FuotaTaskLogOptionUnionTypeDef

```python
# FuotaTaskLogOptionUnionTypeDef definition

FuotaTaskLogOptionUnionTypeDef = Union[
    FuotaTaskLogOptionTypeDef,  # (1)
    FuotaTaskLogOptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FuotaTaskLogOptionTypeDef](./type_defs.md#fuotatasklogoptiontypedef) 
2. See [:material-code-braces: FuotaTaskLogOptionOutputTypeDef](./type_defs.md#fuotatasklogoptionoutputtypedef) 

## ParticipatingGatewaysUnionTypeDef

```python
# ParticipatingGatewaysUnionTypeDef definition

ParticipatingGatewaysUnionTypeDef = Union[
    ParticipatingGatewaysTypeDef,  # (1)
    ParticipatingGatewaysOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ParticipatingGatewaysTypeDef](./type_defs.md#participatinggatewaystypedef) 
2. See [:material-code-braces: ParticipatingGatewaysOutputTypeDef](./type_defs.md#participatinggatewaysoutputtypedef) 

## WirelessDeviceLogOptionUnionTypeDef

```python
# WirelessDeviceLogOptionUnionTypeDef definition

WirelessDeviceLogOptionUnionTypeDef = Union[
    WirelessDeviceLogOptionTypeDef,  # (1)
    WirelessDeviceLogOptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WirelessDeviceLogOptionTypeDef](./type_defs.md#wirelessdevicelogoptiontypedef) 
2. See [:material-code-braces: WirelessDeviceLogOptionOutputTypeDef](./type_defs.md#wirelessdevicelogoptionoutputtypedef) 

## WirelessGatewayLogOptionUnionTypeDef

```python
# WirelessGatewayLogOptionUnionTypeDef definition

WirelessGatewayLogOptionUnionTypeDef = Union[
    WirelessGatewayLogOptionTypeDef,  # (1)
    WirelessGatewayLogOptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WirelessGatewayLogOptionTypeDef](./type_defs.md#wirelessgatewaylogoptiontypedef) 
2. See [:material-code-braces: WirelessGatewayLogOptionOutputTypeDef](./type_defs.md#wirelessgatewaylogoptionoutputtypedef) 

## LoRaWANSendDataToDeviceUnionTypeDef

```python
# LoRaWANSendDataToDeviceUnionTypeDef definition

LoRaWANSendDataToDeviceUnionTypeDef = Union[
    LoRaWANSendDataToDeviceTypeDef,  # (1)
    LoRaWANSendDataToDeviceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LoRaWANSendDataToDeviceTypeDef](./type_defs.md#lorawansenddatatodevicetypedef) 
2. See [:material-code-braces: LoRaWANSendDataToDeviceOutputTypeDef](./type_defs.md#lorawansenddatatodeviceoutputtypedef) 



## SessionKeysAbpV10XTypeDef

```python
# SessionKeysAbpV10XTypeDef definition

class SessionKeysAbpV10XTypeDef(TypedDict):
    NwkSKey: NotRequired[str],
    AppSKey: NotRequired[str],
```

## SessionKeysAbpV11TypeDef

```python
# SessionKeysAbpV11TypeDef definition

class SessionKeysAbpV11TypeDef(TypedDict):
    FNwkSIntKey: NotRequired[str],
    SNwkSIntKey: NotRequired[str],
    NwkSEncKey: NotRequired[str],
    AppSKey: NotRequired[str],
```

## AccuracyTypeDef

```python
# AccuracyTypeDef definition

class AccuracyTypeDef(TypedDict):
    HorizontalAccuracy: NotRequired[float],
    VerticalAccuracy: NotRequired[float],
```

## ApplicationConfigTypeDef

```python
# ApplicationConfigTypeDef definition

class ApplicationConfigTypeDef(TypedDict):
    FPort: NotRequired[int],
    Type: NotRequired[ApplicationConfigTypeType],  # (1)
    DestinationName: NotRequired[str],
```

1. See [:material-code-brackets: ApplicationConfigTypeType](./literals.md#applicationconfigtypetype) 
## SidewalkAccountInfoTypeDef

```python
# SidewalkAccountInfoTypeDef definition

class SidewalkAccountInfoTypeDef(TypedDict):
    AmazonId: NotRequired[str],
    AppServerPrivateKey: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef

```python
# AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef definition

class AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef(TypedDict):
    Id: str,
    MulticastGroupId: str,
```

## AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef

```python
# AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef definition

class AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef(TypedDict):
    Id: str,
    WirelessDeviceId: str,
```

## AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef

```python
# AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef definition

class AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef(TypedDict):
    Id: str,
    WirelessDeviceId: str,
```

## AssociateWirelessDeviceWithThingRequestRequestTypeDef

```python
# AssociateWirelessDeviceWithThingRequestRequestTypeDef definition

class AssociateWirelessDeviceWithThingRequestRequestTypeDef(TypedDict):
    Id: str,
    ThingArn: str,
```

## AssociateWirelessGatewayWithCertificateRequestRequestTypeDef

```python
# AssociateWirelessGatewayWithCertificateRequestRequestTypeDef definition

class AssociateWirelessGatewayWithCertificateRequestRequestTypeDef(TypedDict):
    Id: str,
    IotCertificateId: str,
```

## AssociateWirelessGatewayWithThingRequestRequestTypeDef

```python
# AssociateWirelessGatewayWithThingRequestRequestTypeDef definition

class AssociateWirelessGatewayWithThingRequestRequestTypeDef(TypedDict):
    Id: str,
    ThingArn: str,
```

## BeaconingOutputTypeDef

```python
# BeaconingOutputTypeDef definition

class BeaconingOutputTypeDef(TypedDict):
    DataRate: NotRequired[int],
    Frequencies: NotRequired[List[int]],
```

## BeaconingTypeDef

```python
# BeaconingTypeDef definition

class BeaconingTypeDef(TypedDict):
    DataRate: NotRequired[int],
    Frequencies: NotRequired[Sequence[int]],
```

## CancelMulticastGroupSessionRequestRequestTypeDef

```python
# CancelMulticastGroupSessionRequestRequestTypeDef definition

class CancelMulticastGroupSessionRequestRequestTypeDef(TypedDict):
    Id: str,
```

## CdmaLocalIdTypeDef

```python
# CdmaLocalIdTypeDef definition

class CdmaLocalIdTypeDef(TypedDict):
    PnOffset: int,
    CdmaChannel: int,
```

## CdmaNmrObjTypeDef

```python
# CdmaNmrObjTypeDef definition

class CdmaNmrObjTypeDef(TypedDict):
    PnOffset: int,
    CdmaChannel: int,
    PilotPower: NotRequired[int],
    BaseStationId: NotRequired[int],
```

## CertificateListTypeDef

```python
# CertificateListTypeDef definition

class CertificateListTypeDef(TypedDict):
    SigningAlg: SigningAlgType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: SigningAlgType](./literals.md#signingalgtype) 
## LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef

```python
# LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef definition

class LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef(TypedDict):
    GatewayEuiEventTopic: NotRequired[EventNotificationTopicStatusType],  # (1)
```

1. See [:material-code-brackets: EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype) 
## LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef

```python
# LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef definition

class LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef(TypedDict):
    WirelessGatewayEventTopic: NotRequired[EventNotificationTopicStatusType],  # (1)
```

1. See [:material-code-brackets: EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype) 
## LoRaWANDeviceProfileTypeDef

```python
# LoRaWANDeviceProfileTypeDef definition

class LoRaWANDeviceProfileTypeDef(TypedDict):
    SupportsClassB: NotRequired[bool],
    ClassBTimeout: NotRequired[int],
    PingSlotPeriod: NotRequired[int],
    PingSlotDr: NotRequired[int],
    PingSlotFreq: NotRequired[int],
    SupportsClassC: NotRequired[bool],
    ClassCTimeout: NotRequired[int],
    MacVersion: NotRequired[str],
    RegParamsRevision: NotRequired[str],
    RxDelay1: NotRequired[int],
    RxDrOffset1: NotRequired[int],
    RxDataRate2: NotRequired[int],
    RxFreq2: NotRequired[int],
    FactoryPresetFreqsList: NotRequired[Sequence[int]],
    MaxEirp: NotRequired[int],
    MaxDutyCycle: NotRequired[int],
    RfRegion: NotRequired[str],
    SupportsJoin: NotRequired[bool],
    Supports32BitFCnt: NotRequired[bool],
```

## LoRaWANFuotaTaskTypeDef

```python
# LoRaWANFuotaTaskTypeDef definition

class LoRaWANFuotaTaskTypeDef(TypedDict):
    RfRegion: NotRequired[SupportedRfRegionType],  # (1)
```

1. See [:material-code-brackets: SupportedRfRegionType](./literals.md#supportedrfregiontype) 
## TraceContentTypeDef

```python
# TraceContentTypeDef definition

class TraceContentTypeDef(TypedDict):
    WirelessDeviceFrameInfo: NotRequired[WirelessDeviceFrameInfoType],  # (1)
    LogLevel: NotRequired[LogLevelType],  # (2)
    MulticastFrameInfo: NotRequired[MulticastFrameInfoType],  # (3)
```

1. See [:material-code-brackets: WirelessDeviceFrameInfoType](./literals.md#wirelessdeviceframeinfotype) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
3. See [:material-code-brackets: MulticastFrameInfoType](./literals.md#multicastframeinfotype) 
## LoRaWANServiceProfileTypeDef

```python
# LoRaWANServiceProfileTypeDef definition

class LoRaWANServiceProfileTypeDef(TypedDict):
    AddGwMetadata: NotRequired[bool],
    DrMin: NotRequired[int],
    DrMax: NotRequired[int],
    PrAllowed: NotRequired[bool],
    RaAllowed: NotRequired[bool],
```

## SidewalkCreateWirelessDeviceTypeDef

```python
# SidewalkCreateWirelessDeviceTypeDef definition

class SidewalkCreateWirelessDeviceTypeDef(TypedDict):
    DeviceProfileId: NotRequired[str],
```

## CreateWirelessGatewayTaskRequestRequestTypeDef

```python
# CreateWirelessGatewayTaskRequestRequestTypeDef definition

class CreateWirelessGatewayTaskRequestRequestTypeDef(TypedDict):
    Id: str,
    WirelessGatewayTaskDefinitionId: str,
```

## DakCertificateMetadataTypeDef

```python
# DakCertificateMetadataTypeDef definition

class DakCertificateMetadataTypeDef(TypedDict):
    CertificateId: str,
    MaxAllowedSignature: NotRequired[int],
    FactorySupport: NotRequired[bool],
    ApId: NotRequired[str],
    DeviceTypeId: NotRequired[str],
```

## DeleteDestinationRequestRequestTypeDef

```python
# DeleteDestinationRequestRequestTypeDef definition

class DeleteDestinationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteDeviceProfileRequestRequestTypeDef

```python
# DeleteDeviceProfileRequestRequestTypeDef definition

class DeleteDeviceProfileRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteFuotaTaskRequestRequestTypeDef

```python
# DeleteFuotaTaskRequestRequestTypeDef definition

class DeleteFuotaTaskRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteMulticastGroupRequestRequestTypeDef

```python
# DeleteMulticastGroupRequestRequestTypeDef definition

class DeleteMulticastGroupRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef

```python
# DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef definition

class DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef(TypedDict):
    ConfigurationName: str,
```

## DeleteQueuedMessagesRequestRequestTypeDef

```python
# DeleteQueuedMessagesRequestRequestTypeDef definition

class DeleteQueuedMessagesRequestRequestTypeDef(TypedDict):
    Id: str,
    MessageId: str,
    WirelessDeviceType: NotRequired[WirelessDeviceTypeType],  # (1)
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
## DeleteServiceProfileRequestRequestTypeDef

```python
# DeleteServiceProfileRequestRequestTypeDef definition

class DeleteServiceProfileRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteWirelessDeviceImportTaskRequestRequestTypeDef

```python
# DeleteWirelessDeviceImportTaskRequestRequestTypeDef definition

class DeleteWirelessDeviceImportTaskRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteWirelessDeviceRequestRequestTypeDef

```python
# DeleteWirelessDeviceRequestRequestTypeDef definition

class DeleteWirelessDeviceRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteWirelessGatewayRequestRequestTypeDef

```python
# DeleteWirelessGatewayRequestRequestTypeDef definition

class DeleteWirelessGatewayRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef

```python
# DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef definition

class DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteWirelessGatewayTaskRequestRequestTypeDef

```python
# DeleteWirelessGatewayTaskRequestRequestTypeDef definition

class DeleteWirelessGatewayTaskRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeregisterWirelessDeviceRequestRequestTypeDef

```python
# DeregisterWirelessDeviceRequestRequestTypeDef definition

class DeregisterWirelessDeviceRequestRequestTypeDef(TypedDict):
    Identifier: str,
    WirelessDeviceType: NotRequired[WirelessDeviceTypeType],  # (1)
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
## DestinationsTypeDef

```python
# DestinationsTypeDef definition

class DestinationsTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    ExpressionType: NotRequired[ExpressionTypeType],  # (1)
    Expression: NotRequired[str],
    Description: NotRequired[str],
    RoleArn: NotRequired[str],
```

1. See [:material-code-brackets: ExpressionTypeType](./literals.md#expressiontypetype) 
## DeviceProfileTypeDef

```python
# DeviceProfileTypeDef definition

class DeviceProfileTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Id: NotRequired[str],
```

## SidewalkEventNotificationConfigurationsTypeDef

```python
# SidewalkEventNotificationConfigurationsTypeDef definition

class SidewalkEventNotificationConfigurationsTypeDef(TypedDict):
    AmazonIdEventTopic: NotRequired[EventNotificationTopicStatusType],  # (1)
```

1. See [:material-code-brackets: EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype) 
## SidewalkResourceTypeEventConfigurationTypeDef

```python
# SidewalkResourceTypeEventConfigurationTypeDef definition

class SidewalkResourceTypeEventConfigurationTypeDef(TypedDict):
    WirelessDeviceEventTopic: NotRequired[EventNotificationTopicStatusType],  # (1)
```

1. See [:material-code-brackets: EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype) 
## DimensionTypeDef

```python
# DimensionTypeDef definition

class DimensionTypeDef(TypedDict):
    name: NotRequired[DimensionNameType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: DimensionNameType](./literals.md#dimensionnametype) 
## DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef

```python
# DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef definition

class DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef(TypedDict):
    PartnerAccountId: str,
    PartnerType: PartnerTypeType,  # (1)
```

1. See [:material-code-brackets: PartnerTypeType](./literals.md#partnertypetype) 
## DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef

```python
# DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef definition

class DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef(TypedDict):
    Id: str,
    MulticastGroupId: str,
```

## DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef

```python
# DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef definition

class DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef(TypedDict):
    Id: str,
    WirelessDeviceId: str,
```

## DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef

```python
# DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef definition

class DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef(TypedDict):
    Id: str,
    WirelessDeviceId: str,
```

## DisassociateWirelessDeviceFromThingRequestRequestTypeDef

```python
# DisassociateWirelessDeviceFromThingRequestRequestTypeDef definition

class DisassociateWirelessDeviceFromThingRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef

```python
# DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef definition

class DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DisassociateWirelessGatewayFromThingRequestRequestTypeDef

```python
# DisassociateWirelessGatewayFromThingRequestRequestTypeDef definition

class DisassociateWirelessGatewayFromThingRequestRequestTypeDef(TypedDict):
    Id: str,
```

## PositioningTypeDef

```python
# PositioningTypeDef definition

class PositioningTypeDef(TypedDict):
    ClockSync: NotRequired[int],
    Stream: NotRequired[int],
    Gnss: NotRequired[int],
```

## FuotaTaskEventLogOptionTypeDef

```python
# FuotaTaskEventLogOptionTypeDef definition

class FuotaTaskEventLogOptionTypeDef(TypedDict):
    Event: FuotaTaskEventType,  # (1)
    LogLevel: LogLevelType,  # (2)
```

1. See [:material-code-brackets: FuotaTaskEventType](./literals.md#fuotataskeventtype) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## FuotaTaskTypeDef

```python
# FuotaTaskTypeDef definition

class FuotaTaskTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## GatewayListItemTypeDef

```python
# GatewayListItemTypeDef definition

class GatewayListItemTypeDef(TypedDict):
    GatewayId: str,
    DownlinkFrequency: int,
```

## GetDestinationRequestRequestTypeDef

```python
# GetDestinationRequestRequestTypeDef definition

class GetDestinationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetDeviceProfileRequestRequestTypeDef

```python
# GetDeviceProfileRequestRequestTypeDef definition

class GetDeviceProfileRequestRequestTypeDef(TypedDict):
    Id: str,
```

## LoRaWANDeviceProfileOutputTypeDef

```python
# LoRaWANDeviceProfileOutputTypeDef definition

class LoRaWANDeviceProfileOutputTypeDef(TypedDict):
    SupportsClassB: NotRequired[bool],
    ClassBTimeout: NotRequired[int],
    PingSlotPeriod: NotRequired[int],
    PingSlotDr: NotRequired[int],
    PingSlotFreq: NotRequired[int],
    SupportsClassC: NotRequired[bool],
    ClassCTimeout: NotRequired[int],
    MacVersion: NotRequired[str],
    RegParamsRevision: NotRequired[str],
    RxDelay1: NotRequired[int],
    RxDrOffset1: NotRequired[int],
    RxDataRate2: NotRequired[int],
    RxFreq2: NotRequired[int],
    FactoryPresetFreqsList: NotRequired[List[int]],
    MaxEirp: NotRequired[int],
    MaxDutyCycle: NotRequired[int],
    RfRegion: NotRequired[str],
    SupportsJoin: NotRequired[bool],
    Supports32BitFCnt: NotRequired[bool],
```

## GetFuotaTaskRequestRequestTypeDef

```python
# GetFuotaTaskRequestRequestTypeDef definition

class GetFuotaTaskRequestRequestTypeDef(TypedDict):
    Id: str,
```

## LoRaWANFuotaTaskGetInfoTypeDef

```python
# LoRaWANFuotaTaskGetInfoTypeDef definition

class LoRaWANFuotaTaskGetInfoTypeDef(TypedDict):
    RfRegion: NotRequired[str],
    StartTime: NotRequired[datetime],
```

## SummaryMetricConfigurationTypeDef

```python
# SummaryMetricConfigurationTypeDef definition

class SummaryMetricConfigurationTypeDef(TypedDict):
    Status: NotRequired[SummaryMetricConfigurationStatusType],  # (1)
```

1. See [:material-code-brackets: SummaryMetricConfigurationStatusType](./literals.md#summarymetricconfigurationstatustype) 
## GetMulticastGroupRequestRequestTypeDef

```python
# GetMulticastGroupRequestRequestTypeDef definition

class GetMulticastGroupRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetMulticastGroupSessionRequestRequestTypeDef

```python
# GetMulticastGroupSessionRequestRequestTypeDef definition

class GetMulticastGroupSessionRequestRequestTypeDef(TypedDict):
    Id: str,
```

## LoRaWANMulticastSessionOutputTypeDef

```python
# LoRaWANMulticastSessionOutputTypeDef definition

class LoRaWANMulticastSessionOutputTypeDef(TypedDict):
    DlDr: NotRequired[int],
    DlFreq: NotRequired[int],
    SessionStartTime: NotRequired[datetime],
    SessionTimeout: NotRequired[int],
    PingSlotPeriod: NotRequired[int],
```

## GetNetworkAnalyzerConfigurationRequestRequestTypeDef

```python
# GetNetworkAnalyzerConfigurationRequestRequestTypeDef definition

class GetNetworkAnalyzerConfigurationRequestRequestTypeDef(TypedDict):
    ConfigurationName: str,
```

## GetPartnerAccountRequestRequestTypeDef

```python
# GetPartnerAccountRequestRequestTypeDef definition

class GetPartnerAccountRequestRequestTypeDef(TypedDict):
    PartnerAccountId: str,
    PartnerType: PartnerTypeType,  # (1)
```

1. See [:material-code-brackets: PartnerTypeType](./literals.md#partnertypetype) 
## SidewalkAccountInfoWithFingerprintTypeDef

```python
# SidewalkAccountInfoWithFingerprintTypeDef definition

class SidewalkAccountInfoWithFingerprintTypeDef(TypedDict):
    AmazonId: NotRequired[str],
    Fingerprint: NotRequired[str],
    Arn: NotRequired[str],
```

## GetPositionConfigurationRequestRequestTypeDef

```python
# GetPositionConfigurationRequestRequestTypeDef definition

class GetPositionConfigurationRequestRequestTypeDef(TypedDict):
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
## GnssTypeDef

```python
# GnssTypeDef definition

class GnssTypeDef(TypedDict):
    Payload: str,
    CaptureTime: NotRequired[float],
    CaptureTimeAccuracy: NotRequired[float],
    AssistPosition: NotRequired[Sequence[float]],
    AssistAltitude: NotRequired[float],
    Use2DSolver: NotRequired[bool],
```

## IpTypeDef

```python
# IpTypeDef definition

class IpTypeDef(TypedDict):
    IpAddress: str,
```

## WiFiAccessPointTypeDef

```python
# WiFiAccessPointTypeDef definition

class WiFiAccessPointTypeDef(TypedDict):
    MacAddress: str,
    Rss: int,
```

## GetPositionRequestRequestTypeDef

```python
# GetPositionRequestRequestTypeDef definition

class GetPositionRequestRequestTypeDef(TypedDict):
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
## GetResourceEventConfigurationRequestRequestTypeDef

```python
# GetResourceEventConfigurationRequestRequestTypeDef definition

class GetResourceEventConfigurationRequestRequestTypeDef(TypedDict):
    Identifier: str,
    IdentifierType: IdentifierTypeType,  # (1)
    PartnerType: NotRequired[EventNotificationPartnerTypeType],  # (2)
```

1. See [:material-code-brackets: IdentifierTypeType](./literals.md#identifiertypetype) 
2. See [:material-code-brackets: EventNotificationPartnerTypeType](./literals.md#eventnotificationpartnertypetype) 
## GetResourceLogLevelRequestRequestTypeDef

```python
# GetResourceLogLevelRequestRequestTypeDef definition

class GetResourceLogLevelRequestRequestTypeDef(TypedDict):
    ResourceIdentifier: str,
    ResourceType: str,
```

## GetResourcePositionRequestRequestTypeDef

```python
# GetResourcePositionRequestRequestTypeDef definition

class GetResourcePositionRequestRequestTypeDef(TypedDict):
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
## GetServiceEndpointRequestRequestTypeDef

```python
# GetServiceEndpointRequestRequestTypeDef definition

class GetServiceEndpointRequestRequestTypeDef(TypedDict):
    ServiceType: NotRequired[WirelessGatewayServiceTypeType],  # (1)
```

1. See [:material-code-brackets: WirelessGatewayServiceTypeType](./literals.md#wirelessgatewayservicetypetype) 
## GetServiceProfileRequestRequestTypeDef

```python
# GetServiceProfileRequestRequestTypeDef definition

class GetServiceProfileRequestRequestTypeDef(TypedDict):
    Id: str,
```

## LoRaWANGetServiceProfileInfoTypeDef

```python
# LoRaWANGetServiceProfileInfoTypeDef definition

class LoRaWANGetServiceProfileInfoTypeDef(TypedDict):
    UlRate: NotRequired[int],
    UlBucketSize: NotRequired[int],
    UlRatePolicy: NotRequired[str],
    DlRate: NotRequired[int],
    DlBucketSize: NotRequired[int],
    DlRatePolicy: NotRequired[str],
    AddGwMetadata: NotRequired[bool],
    DevStatusReqFreq: NotRequired[int],
    ReportDevStatusBattery: NotRequired[bool],
    ReportDevStatusMargin: NotRequired[bool],
    DrMin: NotRequired[int],
    DrMax: NotRequired[int],
    ChannelMask: NotRequired[str],
    PrAllowed: NotRequired[bool],
    HrAllowed: NotRequired[bool],
    RaAllowed: NotRequired[bool],
    NwkGeoLoc: NotRequired[bool],
    TargetPer: NotRequired[int],
    MinGwDiversity: NotRequired[int],
```

## GetWirelessDeviceImportTaskRequestRequestTypeDef

```python
# GetWirelessDeviceImportTaskRequestRequestTypeDef definition

class GetWirelessDeviceImportTaskRequestRequestTypeDef(TypedDict):
    Id: str,
```

## SidewalkGetStartImportInfoTypeDef

```python
# SidewalkGetStartImportInfoTypeDef definition

class SidewalkGetStartImportInfoTypeDef(TypedDict):
    DeviceCreationFileList: NotRequired[List[str]],
    Role: NotRequired[str],
```

## GetWirelessDeviceRequestRequestTypeDef

```python
# GetWirelessDeviceRequestRequestTypeDef definition

class GetWirelessDeviceRequestRequestTypeDef(TypedDict):
    Identifier: str,
    IdentifierType: WirelessDeviceIdTypeType,  # (1)
```

1. See [:material-code-brackets: WirelessDeviceIdTypeType](./literals.md#wirelessdeviceidtypetype) 
## GetWirelessDeviceStatisticsRequestRequestTypeDef

```python
# GetWirelessDeviceStatisticsRequestRequestTypeDef definition

class GetWirelessDeviceStatisticsRequestRequestTypeDef(TypedDict):
    WirelessDeviceId: str,
```

## SidewalkDeviceMetadataTypeDef

```python
# SidewalkDeviceMetadataTypeDef definition

class SidewalkDeviceMetadataTypeDef(TypedDict):
    Rssi: NotRequired[int],
    BatteryLevel: NotRequired[BatteryLevelType],  # (1)
    Event: NotRequired[EventType],  # (2)
    DeviceState: NotRequired[DeviceStateType],  # (3)
```

1. See [:material-code-brackets: BatteryLevelType](./literals.md#batteryleveltype) 
2. See [:material-code-brackets: EventType](./literals.md#eventtype) 
3. See [:material-code-brackets: DeviceStateType](./literals.md#devicestatetype) 
## GetWirelessGatewayCertificateRequestRequestTypeDef

```python
# GetWirelessGatewayCertificateRequestRequestTypeDef definition

class GetWirelessGatewayCertificateRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetWirelessGatewayFirmwareInformationRequestRequestTypeDef

```python
# GetWirelessGatewayFirmwareInformationRequestRequestTypeDef definition

class GetWirelessGatewayFirmwareInformationRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetWirelessGatewayRequestRequestTypeDef

```python
# GetWirelessGatewayRequestRequestTypeDef definition

class GetWirelessGatewayRequestRequestTypeDef(TypedDict):
    Identifier: str,
    IdentifierType: WirelessGatewayIdTypeType,  # (1)
```

1. See [:material-code-brackets: WirelessGatewayIdTypeType](./literals.md#wirelessgatewayidtypetype) 
## GetWirelessGatewayStatisticsRequestRequestTypeDef

```python
# GetWirelessGatewayStatisticsRequestRequestTypeDef definition

class GetWirelessGatewayStatisticsRequestRequestTypeDef(TypedDict):
    WirelessGatewayId: str,
```

## GetWirelessGatewayTaskDefinitionRequestRequestTypeDef

```python
# GetWirelessGatewayTaskDefinitionRequestRequestTypeDef definition

class GetWirelessGatewayTaskDefinitionRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetWirelessGatewayTaskRequestRequestTypeDef

```python
# GetWirelessGatewayTaskRequestRequestTypeDef definition

class GetWirelessGatewayTaskRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GlobalIdentityTypeDef

```python
# GlobalIdentityTypeDef definition

class GlobalIdentityTypeDef(TypedDict):
    Lac: int,
    GeranCid: int,
```

## GsmLocalIdTypeDef

```python
# GsmLocalIdTypeDef definition

class GsmLocalIdTypeDef(TypedDict):
    Bsic: int,
    Bcch: int,
```

## ImportedSidewalkDeviceTypeDef

```python
# ImportedSidewalkDeviceTypeDef definition

class ImportedSidewalkDeviceTypeDef(TypedDict):
    SidewalkManufacturingSn: NotRequired[str],
    OnboardingStatus: NotRequired[OnboardStatusType],  # (1)
    OnboardingStatusReason: NotRequired[str],
    LastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: OnboardStatusType](./literals.md#onboardstatustype) 
## LoRaWANJoinEventNotificationConfigurationsTypeDef

```python
# LoRaWANJoinEventNotificationConfigurationsTypeDef definition

class LoRaWANJoinEventNotificationConfigurationsTypeDef(TypedDict):
    DevEuiEventTopic: NotRequired[EventNotificationTopicStatusType],  # (1)
```

1. See [:material-code-brackets: EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype) 
## LoRaWANJoinResourceTypeEventConfigurationTypeDef

```python
# LoRaWANJoinResourceTypeEventConfigurationTypeDef definition

class LoRaWANJoinResourceTypeEventConfigurationTypeDef(TypedDict):
    WirelessDeviceEventTopic: NotRequired[EventNotificationTopicStatusType],  # (1)
```

1. See [:material-code-brackets: EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype) 
## ListDestinationsRequestRequestTypeDef

```python
# ListDestinationsRequestRequestTypeDef definition

class ListDestinationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListDeviceProfilesRequestRequestTypeDef

```python
# ListDeviceProfilesRequestRequestTypeDef definition

class ListDeviceProfilesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    DeviceProfileType: NotRequired[DeviceProfileTypeType],  # (1)
```

1. See [:material-code-brackets: DeviceProfileTypeType](./literals.md#deviceprofiletypetype) 
## ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef

```python
# ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef definition

class ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef(TypedDict):
    Id: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Status: NotRequired[OnboardStatusType],  # (1)
```

1. See [:material-code-brackets: OnboardStatusType](./literals.md#onboardstatustype) 
## ListEventConfigurationsRequestRequestTypeDef

```python
# ListEventConfigurationsRequestRequestTypeDef definition

class ListEventConfigurationsRequestRequestTypeDef(TypedDict):
    ResourceType: EventNotificationResourceTypeType,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: EventNotificationResourceTypeType](./literals.md#eventnotificationresourcetypetype) 
## ListFuotaTasksRequestRequestTypeDef

```python
# ListFuotaTasksRequestRequestTypeDef definition

class ListFuotaTasksRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListMulticastGroupsByFuotaTaskRequestRequestTypeDef

```python
# ListMulticastGroupsByFuotaTaskRequestRequestTypeDef definition

class ListMulticastGroupsByFuotaTaskRequestRequestTypeDef(TypedDict):
    Id: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MulticastGroupByFuotaTaskTypeDef

```python
# MulticastGroupByFuotaTaskTypeDef definition

class MulticastGroupByFuotaTaskTypeDef(TypedDict):
    Id: NotRequired[str],
```

## ListMulticastGroupsRequestRequestTypeDef

```python
# ListMulticastGroupsRequestRequestTypeDef definition

class ListMulticastGroupsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MulticastGroupTypeDef

```python
# MulticastGroupTypeDef definition

class MulticastGroupTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## ListNetworkAnalyzerConfigurationsRequestRequestTypeDef

```python
# ListNetworkAnalyzerConfigurationsRequestRequestTypeDef definition

class ListNetworkAnalyzerConfigurationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## NetworkAnalyzerConfigurationsTypeDef

```python
# NetworkAnalyzerConfigurationsTypeDef definition

class NetworkAnalyzerConfigurationsTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## ListPartnerAccountsRequestRequestTypeDef

```python
# ListPartnerAccountsRequestRequestTypeDef definition

class ListPartnerAccountsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListPositionConfigurationsRequestRequestTypeDef

```python
# ListPositionConfigurationsRequestRequestTypeDef definition

class ListPositionConfigurationsRequestRequestTypeDef(TypedDict):
    ResourceType: NotRequired[PositionResourceTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
## ListQueuedMessagesRequestRequestTypeDef

```python
# ListQueuedMessagesRequestRequestTypeDef definition

class ListQueuedMessagesRequestRequestTypeDef(TypedDict):
    Id: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    WirelessDeviceType: NotRequired[WirelessDeviceTypeType],  # (1)
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
## ListServiceProfilesRequestRequestTypeDef

```python
# ListServiceProfilesRequestRequestTypeDef definition

class ListServiceProfilesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ServiceProfileTypeDef

```python
# ServiceProfileTypeDef definition

class ServiceProfileTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Id: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListWirelessDeviceImportTasksRequestRequestTypeDef

```python
# ListWirelessDeviceImportTasksRequestRequestTypeDef definition

class ListWirelessDeviceImportTasksRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListWirelessDevicesRequestRequestTypeDef

```python
# ListWirelessDevicesRequestRequestTypeDef definition

class ListWirelessDevicesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    DestinationName: NotRequired[str],
    DeviceProfileId: NotRequired[str],
    ServiceProfileId: NotRequired[str],
    WirelessDeviceType: NotRequired[WirelessDeviceTypeType],  # (1)
    FuotaTaskId: NotRequired[str],
    MulticastGroupId: NotRequired[str],
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
## ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef

```python
# ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef definition

class ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    TaskDefinitionType: NotRequired[WirelessGatewayTaskDefinitionTypeType],  # (1)
```

1. See [:material-code-brackets: WirelessGatewayTaskDefinitionTypeType](./literals.md#wirelessgatewaytaskdefinitiontypetype) 
## ListWirelessGatewaysRequestRequestTypeDef

```python
# ListWirelessGatewaysRequestRequestTypeDef definition

class ListWirelessGatewaysRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## LoRaWANGatewayMetadataTypeDef

```python
# LoRaWANGatewayMetadataTypeDef definition

class LoRaWANGatewayMetadataTypeDef(TypedDict):
    GatewayEui: NotRequired[str],
    Snr: NotRequired[float],
    Rssi: NotRequired[float],
```

## LoRaWANPublicGatewayMetadataTypeDef

```python
# LoRaWANPublicGatewayMetadataTypeDef definition

class LoRaWANPublicGatewayMetadataTypeDef(TypedDict):
    ProviderNetId: NotRequired[str],
    Id: NotRequired[str],
    Rssi: NotRequired[float],
    Snr: NotRequired[float],
    RfRegion: NotRequired[str],
    DlAllowed: NotRequired[bool],
```

## OtaaV10XTypeDef

```python
# OtaaV10XTypeDef definition

class OtaaV10XTypeDef(TypedDict):
    AppKey: NotRequired[str],
    AppEui: NotRequired[str],
    JoinEui: NotRequired[str],
    GenAppKey: NotRequired[str],
```

## OtaaV11TypeDef

```python
# OtaaV11TypeDef definition

class OtaaV11TypeDef(TypedDict):
    AppKey: NotRequired[str],
    NwkKey: NotRequired[str],
    JoinEui: NotRequired[str],
```

## LoRaWANGatewayVersionTypeDef

```python
# LoRaWANGatewayVersionTypeDef definition

class LoRaWANGatewayVersionTypeDef(TypedDict):
    PackageVersion: NotRequired[str],
    Model: NotRequired[str],
    Station: NotRequired[str],
```

## LoRaWANListDeviceTypeDef

```python
# LoRaWANListDeviceTypeDef definition

class LoRaWANListDeviceTypeDef(TypedDict):
    DevEui: NotRequired[str],
```

## ParticipatingGatewaysMulticastOutputTypeDef

```python
# ParticipatingGatewaysMulticastOutputTypeDef definition

class ParticipatingGatewaysMulticastOutputTypeDef(TypedDict):
    GatewayList: NotRequired[List[str]],
    TransmissionInterval: NotRequired[int],
```

## LoRaWANMulticastMetadataTypeDef

```python
# LoRaWANMulticastMetadataTypeDef definition

class LoRaWANMulticastMetadataTypeDef(TypedDict):
    FPort: NotRequired[int],
```

## UpdateAbpV10XTypeDef

```python
# UpdateAbpV10XTypeDef definition

class UpdateAbpV10XTypeDef(TypedDict):
    FCntStart: NotRequired[int],
```

## UpdateAbpV11TypeDef

```python
# UpdateAbpV11TypeDef definition

class UpdateAbpV11TypeDef(TypedDict):
    FCntStart: NotRequired[int],
```

## LteLocalIdTypeDef

```python
# LteLocalIdTypeDef definition

class LteLocalIdTypeDef(TypedDict):
    Pci: int,
    Earfcn: int,
```

## LteNmrObjTypeDef

```python
# LteNmrObjTypeDef definition

class LteNmrObjTypeDef(TypedDict):
    Pci: int,
    Earfcn: int,
    EutranCid: int,
    Rsrp: NotRequired[int],
    Rsrq: NotRequired[float],
```

## MetricQueryValueTypeDef

```python
# MetricQueryValueTypeDef definition

class MetricQueryValueTypeDef(TypedDict):
    Min: NotRequired[float],
    Max: NotRequired[float],
    Sum: NotRequired[float],
    Avg: NotRequired[float],
    Std: NotRequired[float],
    P90: NotRequired[float],
```

## ParticipatingGatewaysMulticastTypeDef

```python
# ParticipatingGatewaysMulticastTypeDef definition

class ParticipatingGatewaysMulticastTypeDef(TypedDict):
    GatewayList: NotRequired[Sequence[str]],
    TransmissionInterval: NotRequired[int],
```

## SemtechGnssConfigurationTypeDef

```python
# SemtechGnssConfigurationTypeDef definition

class SemtechGnssConfigurationTypeDef(TypedDict):
    Status: PositionConfigurationStatusType,  # (1)
    Fec: PositionConfigurationFecType,  # (2)
```

1. See [:material-code-brackets: PositionConfigurationStatusType](./literals.md#positionconfigurationstatustype) 
2. See [:material-code-brackets: PositionConfigurationFecType](./literals.md#positionconfigurationfectype) 
## SemtechGnssDetailTypeDef

```python
# SemtechGnssDetailTypeDef definition

class SemtechGnssDetailTypeDef(TypedDict):
    Provider: NotRequired[PositionSolverProviderType],  # (1)
    Type: NotRequired[PositionSolverTypeType],  # (2)
    Status: NotRequired[PositionConfigurationStatusType],  # (3)
    Fec: NotRequired[PositionConfigurationFecType],  # (4)
```

1. See [:material-code-brackets: PositionSolverProviderType](./literals.md#positionsolverprovidertype) 
2. See [:material-code-brackets: PositionSolverTypeType](./literals.md#positionsolvertypetype) 
3. See [:material-code-brackets: PositionConfigurationStatusType](./literals.md#positionconfigurationstatustype) 
4. See [:material-code-brackets: PositionConfigurationFecType](./literals.md#positionconfigurationfectype) 
## PutResourceLogLevelRequestRequestTypeDef

```python
# PutResourceLogLevelRequestRequestTypeDef definition

class PutResourceLogLevelRequestRequestTypeDef(TypedDict):
    ResourceIdentifier: str,
    ResourceType: str,
    LogLevel: LogLevelType,  # (1)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## ResetResourceLogLevelRequestRequestTypeDef

```python
# ResetResourceLogLevelRequestRequestTypeDef definition

class ResetResourceLogLevelRequestRequestTypeDef(TypedDict):
    ResourceIdentifier: str,
    ResourceType: str,
```

## SidewalkSendDataToDeviceTypeDef

```python
# SidewalkSendDataToDeviceTypeDef definition

class SidewalkSendDataToDeviceTypeDef(TypedDict):
    Seq: NotRequired[int],
    MessageType: NotRequired[MessageTypeType],  # (1)
    AckModeRetryDurationSecs: NotRequired[int],
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## SidewalkSingleStartImportInfoTypeDef

```python
# SidewalkSingleStartImportInfoTypeDef definition

class SidewalkSingleStartImportInfoTypeDef(TypedDict):
    SidewalkManufacturingSn: NotRequired[str],
```

## SidewalkStartImportInfoTypeDef

```python
# SidewalkStartImportInfoTypeDef definition

class SidewalkStartImportInfoTypeDef(TypedDict):
    DeviceCreationFile: NotRequired[str],
    Role: NotRequired[str],
```

## SidewalkUpdateAccountTypeDef

```python
# SidewalkUpdateAccountTypeDef definition

class SidewalkUpdateAccountTypeDef(TypedDict):
    AppServerPrivateKey: NotRequired[str],
```

## SidewalkUpdateImportInfoTypeDef

```python
# SidewalkUpdateImportInfoTypeDef definition

class SidewalkUpdateImportInfoTypeDef(TypedDict):
    DeviceCreationFile: NotRequired[str],
```

## TdscdmaLocalIdTypeDef

```python
# TdscdmaLocalIdTypeDef definition

class TdscdmaLocalIdTypeDef(TypedDict):
    Uarfcn: int,
    CellParams: int,
```

## TdscdmaNmrObjTypeDef

```python
# TdscdmaNmrObjTypeDef definition

class TdscdmaNmrObjTypeDef(TypedDict):
    Uarfcn: int,
    CellParams: int,
    UtranCid: NotRequired[int],
    Rscp: NotRequired[int],
    PathLoss: NotRequired[int],
```

## TestWirelessDeviceRequestRequestTypeDef

```python
# TestWirelessDeviceRequestRequestTypeDef definition

class TestWirelessDeviceRequestRequestTypeDef(TypedDict):
    Id: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateDestinationRequestRequestTypeDef

```python
# UpdateDestinationRequestRequestTypeDef definition

class UpdateDestinationRequestRequestTypeDef(TypedDict):
    Name: str,
    ExpressionType: NotRequired[ExpressionTypeType],  # (1)
    Expression: NotRequired[str],
    Description: NotRequired[str],
    RoleArn: NotRequired[str],
```

1. See [:material-code-brackets: ExpressionTypeType](./literals.md#expressiontypetype) 
## UpdatePositionRequestRequestTypeDef

```python
# UpdatePositionRequestRequestTypeDef definition

class UpdatePositionRequestRequestTypeDef(TypedDict):
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
    Position: Sequence[float],
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
## UpdateWirelessGatewayRequestRequestTypeDef

```python
# UpdateWirelessGatewayRequestRequestTypeDef definition

class UpdateWirelessGatewayRequestRequestTypeDef(TypedDict):
    Id: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    JoinEuiFilters: NotRequired[Sequence[Sequence[str]]],
    NetIdFilters: NotRequired[Sequence[str]],
    MaxEirp: NotRequired[float],
```

## WcdmaLocalIdTypeDef

```python
# WcdmaLocalIdTypeDef definition

class WcdmaLocalIdTypeDef(TypedDict):
    Uarfcndl: int,
    Psc: int,
```

## WcdmaNmrObjTypeDef

```python
# WcdmaNmrObjTypeDef definition

class WcdmaNmrObjTypeDef(TypedDict):
    Uarfcndl: int,
    Psc: int,
    UtranCid: int,
    Rscp: NotRequired[int],
    PathLoss: NotRequired[int],
```

## WirelessDeviceEventLogOptionTypeDef

```python
# WirelessDeviceEventLogOptionTypeDef definition

class WirelessDeviceEventLogOptionTypeDef(TypedDict):
    Event: WirelessDeviceEventType,  # (1)
    LogLevel: LogLevelType,  # (2)
```

1. See [:material-code-brackets: WirelessDeviceEventType](./literals.md#wirelessdeviceeventtype) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## WirelessGatewayEventLogOptionTypeDef

```python
# WirelessGatewayEventLogOptionTypeDef definition

class WirelessGatewayEventLogOptionTypeDef(TypedDict):
    Event: WirelessGatewayEventType,  # (1)
    LogLevel: LogLevelType,  # (2)
```

1. See [:material-code-brackets: WirelessGatewayEventType](./literals.md#wirelessgatewayeventtype) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## AbpV10XTypeDef

```python
# AbpV10XTypeDef definition

class AbpV10XTypeDef(TypedDict):
    DevAddr: NotRequired[str],
    SessionKeys: NotRequired[SessionKeysAbpV10XTypeDef],  # (1)
    FCntStart: NotRequired[int],
```

1. See [:material-code-braces: SessionKeysAbpV10XTypeDef](./type_defs.md#sessionkeysabpv10xtypedef) 
## AbpV11TypeDef

```python
# AbpV11TypeDef definition

class AbpV11TypeDef(TypedDict):
    DevAddr: NotRequired[str],
    SessionKeys: NotRequired[SessionKeysAbpV11TypeDef],  # (1)
    FCntStart: NotRequired[int],
```

1. See [:material-code-braces: SessionKeysAbpV11TypeDef](./type_defs.md#sessionkeysabpv11typedef) 
## AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef

```python
# AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef definition

class AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef(TypedDict):
    Sidewalk: SidewalkAccountInfoTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: SidewalkAccountInfoTypeDef](./type_defs.md#sidewalkaccountinfotypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDestinationRequestRequestTypeDef

```python
# CreateDestinationRequestRequestTypeDef definition

class CreateDestinationRequestRequestTypeDef(TypedDict):
    Name: str,
    ExpressionType: ExpressionTypeType,  # (1)
    Expression: str,
    RoleArn: str,
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-brackets: ExpressionTypeType](./literals.md#expressiontypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef

```python
# StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef definition

class StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef(TypedDict):
    Id: str,
    QueryString: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef

```python
# StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef definition

class StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef(TypedDict):
    Id: str,
    QueryString: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AssociateAwsAccountWithPartnerAccountResponseTypeDef

```python
# AssociateAwsAccountWithPartnerAccountResponseTypeDef definition

class AssociateAwsAccountWithPartnerAccountResponseTypeDef(TypedDict):
    Sidewalk: SidewalkAccountInfoTypeDef,  # (1)
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SidewalkAccountInfoTypeDef](./type_defs.md#sidewalkaccountinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateWirelessGatewayWithCertificateResponseTypeDef

```python
# AssociateWirelessGatewayWithCertificateResponseTypeDef definition

class AssociateWirelessGatewayWithCertificateResponseTypeDef(TypedDict):
    IotCertificateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDestinationResponseTypeDef

```python
# CreateDestinationResponseTypeDef definition

class CreateDestinationResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeviceProfileResponseTypeDef

```python
# CreateDeviceProfileResponseTypeDef definition

class CreateDeviceProfileResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFuotaTaskResponseTypeDef

```python
# CreateFuotaTaskResponseTypeDef definition

class CreateFuotaTaskResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMulticastGroupResponseTypeDef

```python
# CreateMulticastGroupResponseTypeDef definition

class CreateMulticastGroupResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNetworkAnalyzerConfigurationResponseTypeDef

```python
# CreateNetworkAnalyzerConfigurationResponseTypeDef definition

class CreateNetworkAnalyzerConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceProfileResponseTypeDef

```python
# CreateServiceProfileResponseTypeDef definition

class CreateServiceProfileResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWirelessDeviceResponseTypeDef

```python
# CreateWirelessDeviceResponseTypeDef definition

class CreateWirelessDeviceResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWirelessGatewayResponseTypeDef

```python
# CreateWirelessGatewayResponseTypeDef definition

class CreateWirelessGatewayResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWirelessGatewayTaskDefinitionResponseTypeDef

```python
# CreateWirelessGatewayTaskDefinitionResponseTypeDef definition

class CreateWirelessGatewayTaskDefinitionResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWirelessGatewayTaskResponseTypeDef

```python
# CreateWirelessGatewayTaskResponseTypeDef definition

class CreateWirelessGatewayTaskResponseTypeDef(TypedDict):
    WirelessGatewayTaskDefinitionId: str,
    Status: WirelessGatewayTaskStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: WirelessGatewayTaskStatusType](./literals.md#wirelessgatewaytaskstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDestinationResponseTypeDef

```python
# GetDestinationResponseTypeDef definition

class GetDestinationResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Expression: str,
    ExpressionType: ExpressionTypeType,  # (1)
    Description: str,
    RoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ExpressionTypeType](./literals.md#expressiontypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPositionEstimateResponseTypeDef

```python
# GetPositionEstimateResponseTypeDef definition

class GetPositionEstimateResponseTypeDef(TypedDict):
    GeoJsonPayload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPositionResponseTypeDef

```python
# GetPositionResponseTypeDef definition

class GetPositionResponseTypeDef(TypedDict):
    Position: List[float],
    Accuracy: AccuracyTypeDef,  # (1)
    SolverType: PositionSolverTypeType,  # (2)
    SolverProvider: PositionSolverProviderType,  # (3)
    SolverVersion: str,
    Timestamp: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AccuracyTypeDef](./type_defs.md#accuracytypedef) 
2. See [:material-code-brackets: PositionSolverTypeType](./literals.md#positionsolvertypetype) 
3. See [:material-code-brackets: PositionSolverProviderType](./literals.md#positionsolverprovidertype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceLogLevelResponseTypeDef

```python
# GetResourceLogLevelResponseTypeDef definition

class GetResourceLogLevelResponseTypeDef(TypedDict):
    LogLevel: LogLevelType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePositionResponseTypeDef

```python
# GetResourcePositionResponseTypeDef definition

class GetResourcePositionResponseTypeDef(TypedDict):
    GeoJsonPayload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceEndpointResponseTypeDef

```python
# GetServiceEndpointResponseTypeDef definition

class GetServiceEndpointResponseTypeDef(TypedDict):
    ServiceType: WirelessGatewayServiceTypeType,  # (1)
    ServiceEndpoint: str,
    ServerTrust: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: WirelessGatewayServiceTypeType](./literals.md#wirelessgatewayservicetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWirelessGatewayCertificateResponseTypeDef

```python
# GetWirelessGatewayCertificateResponseTypeDef definition

class GetWirelessGatewayCertificateResponseTypeDef(TypedDict):
    IotCertificateId: str,
    LoRaWANNetworkServerCertificateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWirelessGatewayStatisticsResponseTypeDef

```python
# GetWirelessGatewayStatisticsResponseTypeDef definition

class GetWirelessGatewayStatisticsResponseTypeDef(TypedDict):
    WirelessGatewayId: str,
    LastUplinkReceivedAt: str,
    ConnectionStatus: ConnectionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConnectionStatusType](./literals.md#connectionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWirelessGatewayTaskResponseTypeDef

```python
# GetWirelessGatewayTaskResponseTypeDef definition

class GetWirelessGatewayTaskResponseTypeDef(TypedDict):
    WirelessGatewayId: str,
    WirelessGatewayTaskDefinitionId: str,
    LastUplinkReceivedAt: str,
    TaskCreatedAt: str,
    Status: WirelessGatewayTaskStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: WirelessGatewayTaskStatusType](./literals.md#wirelessgatewaytaskstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendDataToMulticastGroupResponseTypeDef

```python
# SendDataToMulticastGroupResponseTypeDef definition

class SendDataToMulticastGroupResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendDataToWirelessDeviceResponseTypeDef

```python
# SendDataToWirelessDeviceResponseTypeDef definition

class SendDataToWirelessDeviceResponseTypeDef(TypedDict):
    MessageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSingleWirelessDeviceImportTaskResponseTypeDef

```python
# StartSingleWirelessDeviceImportTaskResponseTypeDef definition

class StartSingleWirelessDeviceImportTaskResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartWirelessDeviceImportTaskResponseTypeDef

```python
# StartWirelessDeviceImportTaskResponseTypeDef definition

class StartWirelessDeviceImportTaskResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestWirelessDeviceResponseTypeDef

```python
# TestWirelessDeviceResponseTypeDef definition

class TestWirelessDeviceResponseTypeDef(TypedDict):
    Result: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoRaWANGatewayOutputTypeDef

```python
# LoRaWANGatewayOutputTypeDef definition

class LoRaWANGatewayOutputTypeDef(TypedDict):
    GatewayEui: NotRequired[str],
    RfRegion: NotRequired[str],
    JoinEuiFilters: NotRequired[List[List[str]]],
    NetIdFilters: NotRequired[List[str]],
    SubBands: NotRequired[List[int]],
    Beaconing: NotRequired[BeaconingOutputTypeDef],  # (1)
    MaxEirp: NotRequired[float],
```

1. See [:material-code-braces: BeaconingOutputTypeDef](./type_defs.md#beaconingoutputtypedef) 
## UpdateResourcePositionRequestRequestTypeDef

```python
# UpdateResourcePositionRequestRequestTypeDef definition

class UpdateResourcePositionRequestRequestTypeDef(TypedDict):
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
    GeoJsonPayload: NotRequired[BlobTypeDef],
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
## CdmaObjTypeDef

```python
# CdmaObjTypeDef definition

class CdmaObjTypeDef(TypedDict):
    SystemId: int,
    NetworkId: int,
    BaseStationId: int,
    RegistrationZone: NotRequired[int],
    CdmaLocalId: NotRequired[CdmaLocalIdTypeDef],  # (1)
    PilotPower: NotRequired[int],
    BaseLat: NotRequired[float],
    BaseLng: NotRequired[float],
    CdmaNmr: NotRequired[Sequence[CdmaNmrObjTypeDef]],  # (2)
```

1. See [:material-code-braces: CdmaLocalIdTypeDef](./type_defs.md#cdmalocalidtypedef) 
2. See [:material-code-braces: CdmaNmrObjTypeDef](./type_defs.md#cdmanmrobjtypedef) 
## SidewalkDeviceTypeDef

```python
# SidewalkDeviceTypeDef definition

class SidewalkDeviceTypeDef(TypedDict):
    AmazonId: NotRequired[str],
    SidewalkId: NotRequired[str],
    SidewalkManufacturingSn: NotRequired[str],
    DeviceCertificates: NotRequired[List[CertificateListTypeDef]],  # (1)
    PrivateKeys: NotRequired[List[CertificateListTypeDef]],  # (1)
    DeviceProfileId: NotRequired[str],
    CertificateId: NotRequired[str],
    Status: NotRequired[WirelessDeviceSidewalkStatusType],  # (3)
```

1. See [:material-code-braces: CertificateListTypeDef](./type_defs.md#certificatelisttypedef) 
2. See [:material-code-braces: CertificateListTypeDef](./type_defs.md#certificatelisttypedef) 
3. See [:material-code-brackets: WirelessDeviceSidewalkStatusType](./literals.md#wirelessdevicesidewalkstatustype) 
## SidewalkListDeviceTypeDef

```python
# SidewalkListDeviceTypeDef definition

class SidewalkListDeviceTypeDef(TypedDict):
    AmazonId: NotRequired[str],
    SidewalkId: NotRequired[str],
    SidewalkManufacturingSn: NotRequired[str],
    DeviceCertificates: NotRequired[List[CertificateListTypeDef]],  # (1)
    DeviceProfileId: NotRequired[str],
    Status: NotRequired[WirelessDeviceSidewalkStatusType],  # (2)
```

1. See [:material-code-braces: CertificateListTypeDef](./type_defs.md#certificatelisttypedef) 
2. See [:material-code-brackets: WirelessDeviceSidewalkStatusType](./literals.md#wirelessdevicesidewalkstatustype) 
## ConnectionStatusEventConfigurationTypeDef

```python
# ConnectionStatusEventConfigurationTypeDef definition

class ConnectionStatusEventConfigurationTypeDef(TypedDict):
    LoRaWAN: NotRequired[LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef],  # (1)
    WirelessGatewayIdEventTopic: NotRequired[EventNotificationTopicStatusType],  # (2)
```

1. See [:material-code-braces: LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef](./type_defs.md#lorawanconnectionstatuseventnotificationconfigurationstypedef) 
2. See [:material-code-brackets: EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype) 
## ConnectionStatusResourceTypeEventConfigurationTypeDef

```python
# ConnectionStatusResourceTypeEventConfigurationTypeDef definition

class ConnectionStatusResourceTypeEventConfigurationTypeDef(TypedDict):
    LoRaWAN: NotRequired[LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef](./type_defs.md#lorawanconnectionstatusresourcetypeeventconfigurationtypedef) 
## CreateDeviceProfileRequestRequestTypeDef

```python
# CreateDeviceProfileRequestRequestTypeDef definition

class CreateDeviceProfileRequestRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANDeviceProfileTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ClientRequestToken: NotRequired[str],
    Sidewalk: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: LoRaWANDeviceProfileTypeDef](./type_defs.md#lorawandeviceprofiletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateFuotaTaskRequestRequestTypeDef

```python
# CreateFuotaTaskRequestRequestTypeDef definition

class CreateFuotaTaskRequestRequestTypeDef(TypedDict):
    FirmwareUpdateImage: str,
    FirmwareUpdateRole: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANFuotaTaskTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    RedundancyPercent: NotRequired[int],
    FragmentSizeBytes: NotRequired[int],
    FragmentIntervalMS: NotRequired[int],
    Descriptor: NotRequired[str],
```

1. See [:material-code-braces: LoRaWANFuotaTaskTypeDef](./type_defs.md#lorawanfuotatasktypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateFuotaTaskRequestRequestTypeDef

```python
# UpdateFuotaTaskRequestRequestTypeDef definition

class UpdateFuotaTaskRequestRequestTypeDef(TypedDict):
    Id: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANFuotaTaskTypeDef],  # (1)
    FirmwareUpdateImage: NotRequired[str],
    FirmwareUpdateRole: NotRequired[str],
    RedundancyPercent: NotRequired[int],
    FragmentSizeBytes: NotRequired[int],
    FragmentIntervalMS: NotRequired[int],
    Descriptor: NotRequired[str],
```

1. See [:material-code-braces: LoRaWANFuotaTaskTypeDef](./type_defs.md#lorawanfuotatasktypedef) 
## CreateNetworkAnalyzerConfigurationRequestRequestTypeDef

```python
# CreateNetworkAnalyzerConfigurationRequestRequestTypeDef definition

class CreateNetworkAnalyzerConfigurationRequestRequestTypeDef(TypedDict):
    Name: str,
    TraceContent: NotRequired[TraceContentTypeDef],  # (1)
    WirelessDevices: NotRequired[Sequence[str]],
    WirelessGateways: NotRequired[Sequence[str]],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ClientRequestToken: NotRequired[str],
    MulticastGroups: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TraceContentTypeDef](./type_defs.md#tracecontenttypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetNetworkAnalyzerConfigurationResponseTypeDef

```python
# GetNetworkAnalyzerConfigurationResponseTypeDef definition

class GetNetworkAnalyzerConfigurationResponseTypeDef(TypedDict):
    TraceContent: TraceContentTypeDef,  # (1)
    WirelessDevices: List[str],
    WirelessGateways: List[str],
    Description: str,
    Arn: str,
    Name: str,
    MulticastGroups: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TraceContentTypeDef](./type_defs.md#tracecontenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef

```python
# UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef definition

class UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef(TypedDict):
    ConfigurationName: str,
    TraceContent: NotRequired[TraceContentTypeDef],  # (1)
    WirelessDevicesToAdd: NotRequired[Sequence[str]],
    WirelessDevicesToRemove: NotRequired[Sequence[str]],
    WirelessGatewaysToAdd: NotRequired[Sequence[str]],
    WirelessGatewaysToRemove: NotRequired[Sequence[str]],
    Description: NotRequired[str],
    MulticastGroupsToAdd: NotRequired[Sequence[str]],
    MulticastGroupsToRemove: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TraceContentTypeDef](./type_defs.md#tracecontenttypedef) 
## CreateServiceProfileRequestRequestTypeDef

```python
# CreateServiceProfileRequestRequestTypeDef definition

class CreateServiceProfileRequestRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANServiceProfileTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: LoRaWANServiceProfileTypeDef](./type_defs.md#lorawanserviceprofiletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## SidewalkGetDeviceProfileTypeDef

```python
# SidewalkGetDeviceProfileTypeDef definition

class SidewalkGetDeviceProfileTypeDef(TypedDict):
    ApplicationServerPublicKey: NotRequired[str],
    QualificationStatus: NotRequired[bool],
    DakCertificateMetadata: NotRequired[List[DakCertificateMetadataTypeDef]],  # (1)
```

1. See [:material-code-braces: DakCertificateMetadataTypeDef](./type_defs.md#dakcertificatemetadatatypedef) 
## ListDestinationsResponseTypeDef

```python
# ListDestinationsResponseTypeDef definition

class ListDestinationsResponseTypeDef(TypedDict):
    DestinationList: List[DestinationsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DestinationsTypeDef](./type_defs.md#destinationstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeviceProfilesResponseTypeDef

```python
# ListDeviceProfilesResponseTypeDef definition

class ListDeviceProfilesResponseTypeDef(TypedDict):
    DeviceProfileList: List[DeviceProfileTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeviceProfileTypeDef](./type_defs.md#deviceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeviceRegistrationStateEventConfigurationTypeDef

```python
# DeviceRegistrationStateEventConfigurationTypeDef definition

class DeviceRegistrationStateEventConfigurationTypeDef(TypedDict):
    Sidewalk: NotRequired[SidewalkEventNotificationConfigurationsTypeDef],  # (1)
    WirelessDeviceIdEventTopic: NotRequired[EventNotificationTopicStatusType],  # (2)
```

1. See [:material-code-braces: SidewalkEventNotificationConfigurationsTypeDef](./type_defs.md#sidewalkeventnotificationconfigurationstypedef) 
2. See [:material-code-brackets: EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype) 
## MessageDeliveryStatusEventConfigurationTypeDef

```python
# MessageDeliveryStatusEventConfigurationTypeDef definition

class MessageDeliveryStatusEventConfigurationTypeDef(TypedDict):
    Sidewalk: NotRequired[SidewalkEventNotificationConfigurationsTypeDef],  # (1)
    WirelessDeviceIdEventTopic: NotRequired[EventNotificationTopicStatusType],  # (2)
```

1. See [:material-code-braces: SidewalkEventNotificationConfigurationsTypeDef](./type_defs.md#sidewalkeventnotificationconfigurationstypedef) 
2. See [:material-code-brackets: EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype) 
## ProximityEventConfigurationTypeDef

```python
# ProximityEventConfigurationTypeDef definition

class ProximityEventConfigurationTypeDef(TypedDict):
    Sidewalk: NotRequired[SidewalkEventNotificationConfigurationsTypeDef],  # (1)
    WirelessDeviceIdEventTopic: NotRequired[EventNotificationTopicStatusType],  # (2)
```

1. See [:material-code-braces: SidewalkEventNotificationConfigurationsTypeDef](./type_defs.md#sidewalkeventnotificationconfigurationstypedef) 
2. See [:material-code-brackets: EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype) 
## DeviceRegistrationStateResourceTypeEventConfigurationTypeDef

```python
# DeviceRegistrationStateResourceTypeEventConfigurationTypeDef definition

class DeviceRegistrationStateResourceTypeEventConfigurationTypeDef(TypedDict):
    Sidewalk: NotRequired[SidewalkResourceTypeEventConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SidewalkResourceTypeEventConfigurationTypeDef](./type_defs.md#sidewalkresourcetypeeventconfigurationtypedef) 
## MessageDeliveryStatusResourceTypeEventConfigurationTypeDef

```python
# MessageDeliveryStatusResourceTypeEventConfigurationTypeDef definition

class MessageDeliveryStatusResourceTypeEventConfigurationTypeDef(TypedDict):
    Sidewalk: NotRequired[SidewalkResourceTypeEventConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SidewalkResourceTypeEventConfigurationTypeDef](./type_defs.md#sidewalkresourcetypeeventconfigurationtypedef) 
## ProximityResourceTypeEventConfigurationTypeDef

```python
# ProximityResourceTypeEventConfigurationTypeDef definition

class ProximityResourceTypeEventConfigurationTypeDef(TypedDict):
    Sidewalk: NotRequired[SidewalkResourceTypeEventConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SidewalkResourceTypeEventConfigurationTypeDef](./type_defs.md#sidewalkresourcetypeeventconfigurationtypedef) 
## FPortsOutputTypeDef

```python
# FPortsOutputTypeDef definition

class FPortsOutputTypeDef(TypedDict):
    Fuota: NotRequired[int],
    Multicast: NotRequired[int],
    ClockSync: NotRequired[int],
    Positioning: NotRequired[PositioningTypeDef],  # (1)
    Applications: NotRequired[List[ApplicationConfigTypeDef]],  # (2)
```

1. See [:material-code-braces: PositioningTypeDef](./type_defs.md#positioningtypedef) 
2. See [:material-code-braces: ApplicationConfigTypeDef](./type_defs.md#applicationconfigtypedef) 
## FPortsTypeDef

```python
# FPortsTypeDef definition

class FPortsTypeDef(TypedDict):
    Fuota: NotRequired[int],
    Multicast: NotRequired[int],
    ClockSync: NotRequired[int],
    Positioning: NotRequired[PositioningTypeDef],  # (1)
    Applications: NotRequired[Sequence[ApplicationConfigTypeDef]],  # (2)
```

1. See [:material-code-braces: PositioningTypeDef](./type_defs.md#positioningtypedef) 
2. See [:material-code-braces: ApplicationConfigTypeDef](./type_defs.md#applicationconfigtypedef) 
## UpdateFPortsTypeDef

```python
# UpdateFPortsTypeDef definition

class UpdateFPortsTypeDef(TypedDict):
    Positioning: NotRequired[PositioningTypeDef],  # (1)
    Applications: NotRequired[Sequence[ApplicationConfigTypeDef]],  # (2)
```

1. See [:material-code-braces: PositioningTypeDef](./type_defs.md#positioningtypedef) 
2. See [:material-code-braces: ApplicationConfigTypeDef](./type_defs.md#applicationconfigtypedef) 
## FuotaTaskLogOptionOutputTypeDef

```python
# FuotaTaskLogOptionOutputTypeDef definition

class FuotaTaskLogOptionOutputTypeDef(TypedDict):
    Type: FuotaTaskTypeType,  # (1)
    LogLevel: LogLevelType,  # (2)
    Events: NotRequired[List[FuotaTaskEventLogOptionTypeDef]],  # (3)
```

1. See [:material-code-brackets: FuotaTaskTypeType](./literals.md#fuotatasktypetype) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
3. See [:material-code-braces: FuotaTaskEventLogOptionTypeDef](./type_defs.md#fuotataskeventlogoptiontypedef) 
## FuotaTaskLogOptionTypeDef

```python
# FuotaTaskLogOptionTypeDef definition

class FuotaTaskLogOptionTypeDef(TypedDict):
    Type: FuotaTaskTypeType,  # (1)
    LogLevel: LogLevelType,  # (2)
    Events: NotRequired[Sequence[FuotaTaskEventLogOptionTypeDef]],  # (3)
```

1. See [:material-code-brackets: FuotaTaskTypeType](./literals.md#fuotatasktypetype) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
3. See [:material-code-braces: FuotaTaskEventLogOptionTypeDef](./type_defs.md#fuotataskeventlogoptiontypedef) 
## ListFuotaTasksResponseTypeDef

```python
# ListFuotaTasksResponseTypeDef definition

class ListFuotaTasksResponseTypeDef(TypedDict):
    FuotaTaskList: List[FuotaTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FuotaTaskTypeDef](./type_defs.md#fuotatasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ParticipatingGatewaysOutputTypeDef

```python
# ParticipatingGatewaysOutputTypeDef definition

class ParticipatingGatewaysOutputTypeDef(TypedDict):
    DownlinkMode: DownlinkModeType,  # (1)
    GatewayList: List[GatewayListItemTypeDef],  # (2)
    TransmissionInterval: int,
```

1. See [:material-code-brackets: DownlinkModeType](./literals.md#downlinkmodetype) 
2. See [:material-code-braces: GatewayListItemTypeDef](./type_defs.md#gatewaylistitemtypedef) 
## ParticipatingGatewaysTypeDef

```python
# ParticipatingGatewaysTypeDef definition

class ParticipatingGatewaysTypeDef(TypedDict):
    DownlinkMode: DownlinkModeType,  # (1)
    GatewayList: Sequence[GatewayListItemTypeDef],  # (2)
    TransmissionInterval: int,
```

1. See [:material-code-brackets: DownlinkModeType](./literals.md#downlinkmodetype) 
2. See [:material-code-braces: GatewayListItemTypeDef](./type_defs.md#gatewaylistitemtypedef) 
## GetFuotaTaskResponseTypeDef

```python
# GetFuotaTaskResponseTypeDef definition

class GetFuotaTaskResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Status: FuotaTaskStatusType,  # (1)
    Name: str,
    Description: str,
    LoRaWAN: LoRaWANFuotaTaskGetInfoTypeDef,  # (2)
    FirmwareUpdateImage: str,
    FirmwareUpdateRole: str,
    CreatedAt: datetime,
    RedundancyPercent: int,
    FragmentSizeBytes: int,
    FragmentIntervalMS: int,
    Descriptor: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: FuotaTaskStatusType](./literals.md#fuotataskstatustype) 
2. See [:material-code-braces: LoRaWANFuotaTaskGetInfoTypeDef](./type_defs.md#lorawanfuotataskgetinfotypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMetricConfigurationResponseTypeDef

```python
# GetMetricConfigurationResponseTypeDef definition

class GetMetricConfigurationResponseTypeDef(TypedDict):
    SummaryMetric: SummaryMetricConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SummaryMetricConfigurationTypeDef](./type_defs.md#summarymetricconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMetricConfigurationRequestRequestTypeDef

```python
# UpdateMetricConfigurationRequestRequestTypeDef definition

class UpdateMetricConfigurationRequestRequestTypeDef(TypedDict):
    SummaryMetric: NotRequired[SummaryMetricConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SummaryMetricConfigurationTypeDef](./type_defs.md#summarymetricconfigurationtypedef) 
## GetMulticastGroupSessionResponseTypeDef

```python
# GetMulticastGroupSessionResponseTypeDef definition

class GetMulticastGroupSessionResponseTypeDef(TypedDict):
    LoRaWAN: LoRaWANMulticastSessionOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoRaWANMulticastSessionOutputTypeDef](./type_defs.md#lorawanmulticastsessionoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPartnerAccountResponseTypeDef

```python
# GetPartnerAccountResponseTypeDef definition

class GetPartnerAccountResponseTypeDef(TypedDict):
    Sidewalk: SidewalkAccountInfoWithFingerprintTypeDef,  # (1)
    AccountLinked: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SidewalkAccountInfoWithFingerprintTypeDef](./type_defs.md#sidewalkaccountinfowithfingerprinttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPartnerAccountsResponseTypeDef

```python
# ListPartnerAccountsResponseTypeDef definition

class ListPartnerAccountsResponseTypeDef(TypedDict):
    Sidewalk: List[SidewalkAccountInfoWithFingerprintTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SidewalkAccountInfoWithFingerprintTypeDef](./type_defs.md#sidewalkaccountinfowithfingerprinttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoRaWANMulticastSessionTypeDef

```python
# LoRaWANMulticastSessionTypeDef definition

class LoRaWANMulticastSessionTypeDef(TypedDict):
    DlDr: NotRequired[int],
    DlFreq: NotRequired[int],
    SessionStartTime: NotRequired[TimestampTypeDef],
    SessionTimeout: NotRequired[int],
    PingSlotPeriod: NotRequired[int],
```

## LoRaWANStartFuotaTaskTypeDef

```python
# LoRaWANStartFuotaTaskTypeDef definition

class LoRaWANStartFuotaTaskTypeDef(TypedDict):
    StartTime: NotRequired[TimestampTypeDef],
```

## SummaryMetricQueryTypeDef

```python
# SummaryMetricQueryTypeDef definition

class SummaryMetricQueryTypeDef(TypedDict):
    QueryId: NotRequired[str],
    MetricName: NotRequired[MetricNameType],  # (1)
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (2)
    AggregationPeriod: NotRequired[AggregationPeriodType],  # (3)
    StartTimestamp: NotRequired[TimestampTypeDef],
    EndTimestamp: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: MetricNameType](./literals.md#metricnametype) 
2. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
3. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
## GetServiceProfileResponseTypeDef

```python
# GetServiceProfileResponseTypeDef definition

class GetServiceProfileResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Id: str,
    LoRaWAN: LoRaWANGetServiceProfileInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoRaWANGetServiceProfileInfoTypeDef](./type_defs.md#lorawangetserviceprofileinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWirelessDeviceImportTaskResponseTypeDef

```python
# GetWirelessDeviceImportTaskResponseTypeDef definition

class GetWirelessDeviceImportTaskResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    DestinationName: str,
    Sidewalk: SidewalkGetStartImportInfoTypeDef,  # (1)
    CreationTime: datetime,
    Status: ImportTaskStatusType,  # (2)
    StatusReason: str,
    InitializedImportedDeviceCount: int,
    PendingImportedDeviceCount: int,
    OnboardedImportedDeviceCount: int,
    FailedImportedDeviceCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SidewalkGetStartImportInfoTypeDef](./type_defs.md#sidewalkgetstartimportinfotypedef) 
2. See [:material-code-brackets: ImportTaskStatusType](./literals.md#importtaskstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WirelessDeviceImportTaskTypeDef

```python
# WirelessDeviceImportTaskTypeDef definition

class WirelessDeviceImportTaskTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    DestinationName: NotRequired[str],
    Sidewalk: NotRequired[SidewalkGetStartImportInfoTypeDef],  # (1)
    CreationTime: NotRequired[datetime],
    Status: NotRequired[ImportTaskStatusType],  # (2)
    StatusReason: NotRequired[str],
    InitializedImportedDeviceCount: NotRequired[int],
    PendingImportedDeviceCount: NotRequired[int],
    OnboardedImportedDeviceCount: NotRequired[int],
    FailedImportedDeviceCount: NotRequired[int],
```

1. See [:material-code-braces: SidewalkGetStartImportInfoTypeDef](./type_defs.md#sidewalkgetstartimportinfotypedef) 
2. See [:material-code-brackets: ImportTaskStatusType](./literals.md#importtaskstatustype) 
## GsmNmrObjTypeDef

```python
# GsmNmrObjTypeDef definition

class GsmNmrObjTypeDef(TypedDict):
    Bsic: int,
    Bcch: int,
    RxLevel: NotRequired[int],
    GlobalIdentity: NotRequired[GlobalIdentityTypeDef],  # (1)
```

1. See [:material-code-braces: GlobalIdentityTypeDef](./type_defs.md#globalidentitytypedef) 
## ImportedWirelessDeviceTypeDef

```python
# ImportedWirelessDeviceTypeDef definition

class ImportedWirelessDeviceTypeDef(TypedDict):
    Sidewalk: NotRequired[ImportedSidewalkDeviceTypeDef],  # (1)
```

1. See [:material-code-braces: ImportedSidewalkDeviceTypeDef](./type_defs.md#importedsidewalkdevicetypedef) 
## JoinEventConfigurationTypeDef

```python
# JoinEventConfigurationTypeDef definition

class JoinEventConfigurationTypeDef(TypedDict):
    LoRaWAN: NotRequired[LoRaWANJoinEventNotificationConfigurationsTypeDef],  # (1)
    WirelessDeviceIdEventTopic: NotRequired[EventNotificationTopicStatusType],  # (2)
```

1. See [:material-code-braces: LoRaWANJoinEventNotificationConfigurationsTypeDef](./type_defs.md#lorawanjoineventnotificationconfigurationstypedef) 
2. See [:material-code-brackets: EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype) 
## JoinResourceTypeEventConfigurationTypeDef

```python
# JoinResourceTypeEventConfigurationTypeDef definition

class JoinResourceTypeEventConfigurationTypeDef(TypedDict):
    LoRaWAN: NotRequired[LoRaWANJoinResourceTypeEventConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: LoRaWANJoinResourceTypeEventConfigurationTypeDef](./type_defs.md#lorawanjoinresourcetypeeventconfigurationtypedef) 
## ListMulticastGroupsByFuotaTaskResponseTypeDef

```python
# ListMulticastGroupsByFuotaTaskResponseTypeDef definition

class ListMulticastGroupsByFuotaTaskResponseTypeDef(TypedDict):
    MulticastGroupList: List[MulticastGroupByFuotaTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MulticastGroupByFuotaTaskTypeDef](./type_defs.md#multicastgroupbyfuotatasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMulticastGroupsResponseTypeDef

```python
# ListMulticastGroupsResponseTypeDef definition

class ListMulticastGroupsResponseTypeDef(TypedDict):
    MulticastGroupList: List[MulticastGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MulticastGroupTypeDef](./type_defs.md#multicastgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNetworkAnalyzerConfigurationsResponseTypeDef

```python
# ListNetworkAnalyzerConfigurationsResponseTypeDef definition

class ListNetworkAnalyzerConfigurationsResponseTypeDef(TypedDict):
    NetworkAnalyzerConfigurationList: List[NetworkAnalyzerConfigurationsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NetworkAnalyzerConfigurationsTypeDef](./type_defs.md#networkanalyzerconfigurationstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceProfilesResponseTypeDef

```python
# ListServiceProfilesResponseTypeDef definition

class ListServiceProfilesResponseTypeDef(TypedDict):
    ServiceProfileList: List[ServiceProfileTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceProfileTypeDef](./type_defs.md#serviceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoRaWANDeviceMetadataTypeDef

```python
# LoRaWANDeviceMetadataTypeDef definition

class LoRaWANDeviceMetadataTypeDef(TypedDict):
    DevEui: NotRequired[str],
    FPort: NotRequired[int],
    DataRate: NotRequired[int],
    Frequency: NotRequired[int],
    Timestamp: NotRequired[str],
    Gateways: NotRequired[List[LoRaWANGatewayMetadataTypeDef]],  # (1)
    PublicGateways: NotRequired[List[LoRaWANPublicGatewayMetadataTypeDef]],  # (2)
```

1. See [:material-code-braces: LoRaWANGatewayMetadataTypeDef](./type_defs.md#lorawangatewaymetadatatypedef) 
2. See [:material-code-braces: LoRaWANPublicGatewayMetadataTypeDef](./type_defs.md#lorawanpublicgatewaymetadatatypedef) 
## LoRaWANGatewayCurrentVersionTypeDef

```python
# LoRaWANGatewayCurrentVersionTypeDef definition

class LoRaWANGatewayCurrentVersionTypeDef(TypedDict):
    CurrentVersion: NotRequired[LoRaWANGatewayVersionTypeDef],  # (1)
```

1. See [:material-code-braces: LoRaWANGatewayVersionTypeDef](./type_defs.md#lorawangatewayversiontypedef) 
## LoRaWANUpdateGatewayTaskCreateTypeDef

```python
# LoRaWANUpdateGatewayTaskCreateTypeDef definition

class LoRaWANUpdateGatewayTaskCreateTypeDef(TypedDict):
    UpdateSignature: NotRequired[str],
    SigKeyCrc: NotRequired[int],
    CurrentVersion: NotRequired[LoRaWANGatewayVersionTypeDef],  # (1)
    UpdateVersion: NotRequired[LoRaWANGatewayVersionTypeDef],  # (1)
```

1. See [:material-code-braces: LoRaWANGatewayVersionTypeDef](./type_defs.md#lorawangatewayversiontypedef) 
2. See [:material-code-braces: LoRaWANGatewayVersionTypeDef](./type_defs.md#lorawangatewayversiontypedef) 
## LoRaWANUpdateGatewayTaskEntryTypeDef

```python
# LoRaWANUpdateGatewayTaskEntryTypeDef definition

class LoRaWANUpdateGatewayTaskEntryTypeDef(TypedDict):
    CurrentVersion: NotRequired[LoRaWANGatewayVersionTypeDef],  # (1)
    UpdateVersion: NotRequired[LoRaWANGatewayVersionTypeDef],  # (1)
```

1. See [:material-code-braces: LoRaWANGatewayVersionTypeDef](./type_defs.md#lorawangatewayversiontypedef) 
2. See [:material-code-braces: LoRaWANGatewayVersionTypeDef](./type_defs.md#lorawangatewayversiontypedef) 
## LoRaWANMulticastGetTypeDef

```python
# LoRaWANMulticastGetTypeDef definition

class LoRaWANMulticastGetTypeDef(TypedDict):
    RfRegion: NotRequired[SupportedRfRegionType],  # (1)
    DlClass: NotRequired[DlClassType],  # (2)
    NumberOfDevicesRequested: NotRequired[int],
    NumberOfDevicesInGroup: NotRequired[int],
    ParticipatingGateways: NotRequired[ParticipatingGatewaysMulticastOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: SupportedRfRegionType](./literals.md#supportedrfregiontype) 
2. See [:material-code-brackets: DlClassType](./literals.md#dlclasstype) 
3. See [:material-code-braces: ParticipatingGatewaysMulticastOutputTypeDef](./type_defs.md#participatinggatewaysmulticastoutputtypedef) 
## MulticastWirelessMetadataTypeDef

```python
# MulticastWirelessMetadataTypeDef definition

class MulticastWirelessMetadataTypeDef(TypedDict):
    LoRaWAN: NotRequired[LoRaWANMulticastMetadataTypeDef],  # (1)
```

1. See [:material-code-braces: LoRaWANMulticastMetadataTypeDef](./type_defs.md#lorawanmulticastmetadatatypedef) 
## LteObjTypeDef

```python
# LteObjTypeDef definition

class LteObjTypeDef(TypedDict):
    Mcc: int,
    Mnc: int,
    EutranCid: int,
    Tac: NotRequired[int],
    LteLocalId: NotRequired[LteLocalIdTypeDef],  # (1)
    LteTimingAdvance: NotRequired[int],
    Rsrp: NotRequired[int],
    Rsrq: NotRequired[float],
    NrCapable: NotRequired[bool],
    LteNmr: NotRequired[Sequence[LteNmrObjTypeDef]],  # (2)
```

1. See [:material-code-braces: LteLocalIdTypeDef](./type_defs.md#ltelocalidtypedef) 
2. See [:material-code-braces: LteNmrObjTypeDef](./type_defs.md#ltenmrobjtypedef) 
## SummaryMetricQueryResultTypeDef

```python
# SummaryMetricQueryResultTypeDef definition

class SummaryMetricQueryResultTypeDef(TypedDict):
    QueryId: NotRequired[str],
    QueryStatus: NotRequired[MetricQueryStatusType],  # (1)
    Error: NotRequired[str],
    MetricName: NotRequired[MetricNameType],  # (2)
    Dimensions: NotRequired[List[DimensionTypeDef]],  # (3)
    AggregationPeriod: NotRequired[AggregationPeriodType],  # (4)
    StartTimestamp: NotRequired[datetime],
    EndTimestamp: NotRequired[datetime],
    Timestamps: NotRequired[List[datetime]],
    Values: NotRequired[List[MetricQueryValueTypeDef]],  # (5)
    Unit: NotRequired[str],
```

1. See [:material-code-brackets: MetricQueryStatusType](./literals.md#metricquerystatustype) 
2. See [:material-code-brackets: MetricNameType](./literals.md#metricnametype) 
3. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
4. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
5. See [:material-code-braces: MetricQueryValueTypeDef](./type_defs.md#metricqueryvaluetypedef) 
## PositionSolverConfigurationsTypeDef

```python
# PositionSolverConfigurationsTypeDef definition

class PositionSolverConfigurationsTypeDef(TypedDict):
    SemtechGnss: NotRequired[SemtechGnssConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SemtechGnssConfigurationTypeDef](./type_defs.md#semtechgnssconfigurationtypedef) 
## PositionSolverDetailsTypeDef

```python
# PositionSolverDetailsTypeDef definition

class PositionSolverDetailsTypeDef(TypedDict):
    SemtechGnss: NotRequired[SemtechGnssDetailTypeDef],  # (1)
```

1. See [:material-code-braces: SemtechGnssDetailTypeDef](./type_defs.md#semtechgnssdetailtypedef) 
## StartSingleWirelessDeviceImportTaskRequestRequestTypeDef

```python
# StartSingleWirelessDeviceImportTaskRequestRequestTypeDef definition

class StartSingleWirelessDeviceImportTaskRequestRequestTypeDef(TypedDict):
    DestinationName: str,
    Sidewalk: SidewalkSingleStartImportInfoTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    DeviceName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: SidewalkSingleStartImportInfoTypeDef](./type_defs.md#sidewalksinglestartimportinfotypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartWirelessDeviceImportTaskRequestRequestTypeDef

```python
# StartWirelessDeviceImportTaskRequestRequestTypeDef definition

class StartWirelessDeviceImportTaskRequestRequestTypeDef(TypedDict):
    DestinationName: str,
    Sidewalk: SidewalkStartImportInfoTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: SidewalkStartImportInfoTypeDef](./type_defs.md#sidewalkstartimportinfotypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdatePartnerAccountRequestRequestTypeDef

```python
# UpdatePartnerAccountRequestRequestTypeDef definition

class UpdatePartnerAccountRequestRequestTypeDef(TypedDict):
    Sidewalk: SidewalkUpdateAccountTypeDef,  # (1)
    PartnerAccountId: str,
    PartnerType: PartnerTypeType,  # (2)
```

1. See [:material-code-braces: SidewalkUpdateAccountTypeDef](./type_defs.md#sidewalkupdateaccounttypedef) 
2. See [:material-code-brackets: PartnerTypeType](./literals.md#partnertypetype) 
## UpdateWirelessDeviceImportTaskRequestRequestTypeDef

```python
# UpdateWirelessDeviceImportTaskRequestRequestTypeDef definition

class UpdateWirelessDeviceImportTaskRequestRequestTypeDef(TypedDict):
    Id: str,
    Sidewalk: SidewalkUpdateImportInfoTypeDef,  # (1)
```

1. See [:material-code-braces: SidewalkUpdateImportInfoTypeDef](./type_defs.md#sidewalkupdateimportinfotypedef) 
## TdscdmaObjTypeDef

```python
# TdscdmaObjTypeDef definition

class TdscdmaObjTypeDef(TypedDict):
    Mcc: int,
    Mnc: int,
    UtranCid: int,
    Lac: NotRequired[int],
    TdscdmaLocalId: NotRequired[TdscdmaLocalIdTypeDef],  # (1)
    TdscdmaTimingAdvance: NotRequired[int],
    Rscp: NotRequired[int],
    PathLoss: NotRequired[int],
    TdscdmaNmr: NotRequired[Sequence[TdscdmaNmrObjTypeDef]],  # (2)
```

1. See [:material-code-braces: TdscdmaLocalIdTypeDef](./type_defs.md#tdscdmalocalidtypedef) 
2. See [:material-code-braces: TdscdmaNmrObjTypeDef](./type_defs.md#tdscdmanmrobjtypedef) 
## WcdmaObjTypeDef

```python
# WcdmaObjTypeDef definition

class WcdmaObjTypeDef(TypedDict):
    Mcc: int,
    Mnc: int,
    UtranCid: int,
    Lac: NotRequired[int],
    WcdmaLocalId: NotRequired[WcdmaLocalIdTypeDef],  # (1)
    Rscp: NotRequired[int],
    PathLoss: NotRequired[int],
    WcdmaNmr: NotRequired[Sequence[WcdmaNmrObjTypeDef]],  # (2)
```

1. See [:material-code-braces: WcdmaLocalIdTypeDef](./type_defs.md#wcdmalocalidtypedef) 
2. See [:material-code-braces: WcdmaNmrObjTypeDef](./type_defs.md#wcdmanmrobjtypedef) 
## WirelessDeviceLogOptionOutputTypeDef

```python
# WirelessDeviceLogOptionOutputTypeDef definition

class WirelessDeviceLogOptionOutputTypeDef(TypedDict):
    Type: WirelessDeviceTypeType,  # (1)
    LogLevel: LogLevelType,  # (2)
    Events: NotRequired[List[WirelessDeviceEventLogOptionTypeDef]],  # (3)
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
3. See [:material-code-braces: WirelessDeviceEventLogOptionTypeDef](./type_defs.md#wirelessdeviceeventlogoptiontypedef) 
## WirelessDeviceLogOptionTypeDef

```python
# WirelessDeviceLogOptionTypeDef definition

class WirelessDeviceLogOptionTypeDef(TypedDict):
    Type: WirelessDeviceTypeType,  # (1)
    LogLevel: LogLevelType,  # (2)
    Events: NotRequired[Sequence[WirelessDeviceEventLogOptionTypeDef]],  # (3)
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
3. See [:material-code-braces: WirelessDeviceEventLogOptionTypeDef](./type_defs.md#wirelessdeviceeventlogoptiontypedef) 
## WirelessGatewayLogOptionOutputTypeDef

```python
# WirelessGatewayLogOptionOutputTypeDef definition

class WirelessGatewayLogOptionOutputTypeDef(TypedDict):
    Type: WirelessGatewayTypeType,  # (1)
    LogLevel: LogLevelType,  # (2)
    Events: NotRequired[List[WirelessGatewayEventLogOptionTypeDef]],  # (3)
```

1. See [:material-code-brackets: WirelessGatewayTypeType](./literals.md#wirelessgatewaytypetype) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
3. See [:material-code-braces: WirelessGatewayEventLogOptionTypeDef](./type_defs.md#wirelessgatewayeventlogoptiontypedef) 
## WirelessGatewayLogOptionTypeDef

```python
# WirelessGatewayLogOptionTypeDef definition

class WirelessGatewayLogOptionTypeDef(TypedDict):
    Type: WirelessGatewayTypeType,  # (1)
    LogLevel: LogLevelType,  # (2)
    Events: NotRequired[Sequence[WirelessGatewayEventLogOptionTypeDef]],  # (3)
```

1. See [:material-code-brackets: WirelessGatewayTypeType](./literals.md#wirelessgatewaytypetype) 
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
3. See [:material-code-braces: WirelessGatewayEventLogOptionTypeDef](./type_defs.md#wirelessgatewayeventlogoptiontypedef) 
## GetWirelessGatewayResponseTypeDef

```python
# GetWirelessGatewayResponseTypeDef definition

class GetWirelessGatewayResponseTypeDef(TypedDict):
    Name: str,
    Id: str,
    Description: str,
    LoRaWAN: LoRaWANGatewayOutputTypeDef,  # (1)
    Arn: str,
    ThingName: str,
    ThingArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoRaWANGatewayOutputTypeDef](./type_defs.md#lorawangatewayoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WirelessGatewayStatisticsTypeDef

```python
# WirelessGatewayStatisticsTypeDef definition

class WirelessGatewayStatisticsTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANGatewayOutputTypeDef],  # (1)
    LastUplinkReceivedAt: NotRequired[str],
```

1. See [:material-code-braces: LoRaWANGatewayOutputTypeDef](./type_defs.md#lorawangatewayoutputtypedef) 
## LoRaWANGatewayTypeDef

```python
# LoRaWANGatewayTypeDef definition

class LoRaWANGatewayTypeDef(TypedDict):
    GatewayEui: NotRequired[str],
    RfRegion: NotRequired[str],
    JoinEuiFilters: NotRequired[Sequence[Sequence[str]]],
    NetIdFilters: NotRequired[Sequence[str]],
    SubBands: NotRequired[Sequence[int]],
    Beaconing: NotRequired[BeaconingUnionTypeDef],  # (1)
    MaxEirp: NotRequired[float],
```

1. See [:material-code-braces: BeaconingTypeDef](./type_defs.md#beaconingtypedef) [:material-code-braces: BeaconingOutputTypeDef](./type_defs.md#beaconingoutputtypedef) 
## WirelessDeviceStatisticsTypeDef

```python
# WirelessDeviceStatisticsTypeDef definition

class WirelessDeviceStatisticsTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Type: NotRequired[WirelessDeviceTypeType],  # (1)
    Name: NotRequired[str],
    DestinationName: NotRequired[str],
    LastUplinkReceivedAt: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANListDeviceTypeDef],  # (2)
    Sidewalk: NotRequired[SidewalkListDeviceTypeDef],  # (3)
    FuotaDeviceStatus: NotRequired[FuotaDeviceStatusType],  # (4)
    MulticastDeviceStatus: NotRequired[str],
    McGroupId: NotRequired[int],
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
2. See [:material-code-braces: LoRaWANListDeviceTypeDef](./type_defs.md#lorawanlistdevicetypedef) 
3. See [:material-code-braces: SidewalkListDeviceTypeDef](./type_defs.md#sidewalklistdevicetypedef) 
4. See [:material-code-brackets: FuotaDeviceStatusType](./literals.md#fuotadevicestatustype) 
## GetDeviceProfileResponseTypeDef

```python
# GetDeviceProfileResponseTypeDef definition

class GetDeviceProfileResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Id: str,
    LoRaWAN: LoRaWANDeviceProfileOutputTypeDef,  # (1)
    Sidewalk: SidewalkGetDeviceProfileTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: LoRaWANDeviceProfileOutputTypeDef](./type_defs.md#lorawandeviceprofileoutputtypedef) 
2. See [:material-code-braces: SidewalkGetDeviceProfileTypeDef](./type_defs.md#sidewalkgetdeviceprofiletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoRaWANDeviceOutputTypeDef

```python
# LoRaWANDeviceOutputTypeDef definition

class LoRaWANDeviceOutputTypeDef(TypedDict):
    DevEui: NotRequired[str],
    DeviceProfileId: NotRequired[str],
    ServiceProfileId: NotRequired[str],
    OtaaV1_1: NotRequired[OtaaV11TypeDef],  # (1)
    OtaaV1_0_x: NotRequired[OtaaV10XTypeDef],  # (2)
    AbpV1_1: NotRequired[AbpV11TypeDef],  # (3)
    AbpV1_0_x: NotRequired[AbpV10XTypeDef],  # (4)
    FPorts: NotRequired[FPortsOutputTypeDef],  # (5)
```

1. See [:material-code-braces: OtaaV11TypeDef](./type_defs.md#otaav11typedef) 
2. See [:material-code-braces: OtaaV10XTypeDef](./type_defs.md#otaav10xtypedef) 
3. See [:material-code-braces: AbpV11TypeDef](./type_defs.md#abpv11typedef) 
4. See [:material-code-braces: AbpV10XTypeDef](./type_defs.md#abpv10xtypedef) 
5. See [:material-code-braces: FPortsOutputTypeDef](./type_defs.md#fportsoutputtypedef) 
## LoRaWANUpdateDeviceTypeDef

```python
# LoRaWANUpdateDeviceTypeDef definition

class LoRaWANUpdateDeviceTypeDef(TypedDict):
    DeviceProfileId: NotRequired[str],
    ServiceProfileId: NotRequired[str],
    AbpV1_1: NotRequired[UpdateAbpV11TypeDef],  # (1)
    AbpV1_0_x: NotRequired[UpdateAbpV10XTypeDef],  # (2)
    FPorts: NotRequired[UpdateFPortsTypeDef],  # (3)
```

1. See [:material-code-braces: UpdateAbpV11TypeDef](./type_defs.md#updateabpv11typedef) 
2. See [:material-code-braces: UpdateAbpV10XTypeDef](./type_defs.md#updateabpv10xtypedef) 
3. See [:material-code-braces: UpdateFPortsTypeDef](./type_defs.md#updatefportstypedef) 
## LoRaWANSendDataToDeviceOutputTypeDef

```python
# LoRaWANSendDataToDeviceOutputTypeDef definition

class LoRaWANSendDataToDeviceOutputTypeDef(TypedDict):
    FPort: NotRequired[int],
    ParticipatingGateways: NotRequired[ParticipatingGatewaysOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ParticipatingGatewaysOutputTypeDef](./type_defs.md#participatinggatewaysoutputtypedef) 
## StartMulticastGroupSessionRequestRequestTypeDef

```python
# StartMulticastGroupSessionRequestRequestTypeDef definition

class StartMulticastGroupSessionRequestRequestTypeDef(TypedDict):
    Id: str,
    LoRaWAN: LoRaWANMulticastSessionTypeDef,  # (1)
```

1. See [:material-code-braces: LoRaWANMulticastSessionTypeDef](./type_defs.md#lorawanmulticastsessiontypedef) 
## StartFuotaTaskRequestRequestTypeDef

```python
# StartFuotaTaskRequestRequestTypeDef definition

class StartFuotaTaskRequestRequestTypeDef(TypedDict):
    Id: str,
    LoRaWAN: NotRequired[LoRaWANStartFuotaTaskTypeDef],  # (1)
```

1. See [:material-code-braces: LoRaWANStartFuotaTaskTypeDef](./type_defs.md#lorawanstartfuotatasktypedef) 
## GetMetricsRequestRequestTypeDef

```python
# GetMetricsRequestRequestTypeDef definition

class GetMetricsRequestRequestTypeDef(TypedDict):
    SummaryMetricQueries: NotRequired[Sequence[SummaryMetricQueryTypeDef]],  # (1)
```

1. See [:material-code-braces: SummaryMetricQueryTypeDef](./type_defs.md#summarymetricquerytypedef) 
## ListWirelessDeviceImportTasksResponseTypeDef

```python
# ListWirelessDeviceImportTasksResponseTypeDef definition

class ListWirelessDeviceImportTasksResponseTypeDef(TypedDict):
    WirelessDeviceImportTaskList: List[WirelessDeviceImportTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WirelessDeviceImportTaskTypeDef](./type_defs.md#wirelessdeviceimporttasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GsmObjTypeDef

```python
# GsmObjTypeDef definition

class GsmObjTypeDef(TypedDict):
    Mcc: int,
    Mnc: int,
    Lac: int,
    GeranCid: int,
    GsmLocalId: NotRequired[GsmLocalIdTypeDef],  # (1)
    GsmTimingAdvance: NotRequired[int],
    RxLevel: NotRequired[int],
    GsmNmr: NotRequired[Sequence[GsmNmrObjTypeDef]],  # (2)
```

1. See [:material-code-braces: GsmLocalIdTypeDef](./type_defs.md#gsmlocalidtypedef) 
2. See [:material-code-braces: GsmNmrObjTypeDef](./type_defs.md#gsmnmrobjtypedef) 
## ListDevicesForWirelessDeviceImportTaskResponseTypeDef

```python
# ListDevicesForWirelessDeviceImportTaskResponseTypeDef definition

class ListDevicesForWirelessDeviceImportTaskResponseTypeDef(TypedDict):
    DestinationName: str,
    ImportedWirelessDeviceList: List[ImportedWirelessDeviceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportedWirelessDeviceTypeDef](./type_defs.md#importedwirelessdevicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventNotificationItemConfigurationsTypeDef

```python
# EventNotificationItemConfigurationsTypeDef definition

class EventNotificationItemConfigurationsTypeDef(TypedDict):
    DeviceRegistrationState: NotRequired[DeviceRegistrationStateEventConfigurationTypeDef],  # (1)
    Proximity: NotRequired[ProximityEventConfigurationTypeDef],  # (2)
    Join: NotRequired[JoinEventConfigurationTypeDef],  # (3)
    ConnectionStatus: NotRequired[ConnectionStatusEventConfigurationTypeDef],  # (4)
    MessageDeliveryStatus: NotRequired[MessageDeliveryStatusEventConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: DeviceRegistrationStateEventConfigurationTypeDef](./type_defs.md#deviceregistrationstateeventconfigurationtypedef) 
2. See [:material-code-braces: ProximityEventConfigurationTypeDef](./type_defs.md#proximityeventconfigurationtypedef) 
3. See [:material-code-braces: JoinEventConfigurationTypeDef](./type_defs.md#joineventconfigurationtypedef) 
4. See [:material-code-braces: ConnectionStatusEventConfigurationTypeDef](./type_defs.md#connectionstatuseventconfigurationtypedef) 
5. See [:material-code-braces: MessageDeliveryStatusEventConfigurationTypeDef](./type_defs.md#messagedeliverystatuseventconfigurationtypedef) 
## GetResourceEventConfigurationResponseTypeDef

```python
# GetResourceEventConfigurationResponseTypeDef definition

class GetResourceEventConfigurationResponseTypeDef(TypedDict):
    DeviceRegistrationState: DeviceRegistrationStateEventConfigurationTypeDef,  # (1)
    Proximity: ProximityEventConfigurationTypeDef,  # (2)
    Join: JoinEventConfigurationTypeDef,  # (3)
    ConnectionStatus: ConnectionStatusEventConfigurationTypeDef,  # (4)
    MessageDeliveryStatus: MessageDeliveryStatusEventConfigurationTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: DeviceRegistrationStateEventConfigurationTypeDef](./type_defs.md#deviceregistrationstateeventconfigurationtypedef) 
2. See [:material-code-braces: ProximityEventConfigurationTypeDef](./type_defs.md#proximityeventconfigurationtypedef) 
3. See [:material-code-braces: JoinEventConfigurationTypeDef](./type_defs.md#joineventconfigurationtypedef) 
4. See [:material-code-braces: ConnectionStatusEventConfigurationTypeDef](./type_defs.md#connectionstatuseventconfigurationtypedef) 
5. See [:material-code-braces: MessageDeliveryStatusEventConfigurationTypeDef](./type_defs.md#messagedeliverystatuseventconfigurationtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResourceEventConfigurationRequestRequestTypeDef

```python
# UpdateResourceEventConfigurationRequestRequestTypeDef definition

class UpdateResourceEventConfigurationRequestRequestTypeDef(TypedDict):
    Identifier: str,
    IdentifierType: IdentifierTypeType,  # (1)
    PartnerType: NotRequired[EventNotificationPartnerTypeType],  # (2)
    DeviceRegistrationState: NotRequired[DeviceRegistrationStateEventConfigurationTypeDef],  # (3)
    Proximity: NotRequired[ProximityEventConfigurationTypeDef],  # (4)
    Join: NotRequired[JoinEventConfigurationTypeDef],  # (5)
    ConnectionStatus: NotRequired[ConnectionStatusEventConfigurationTypeDef],  # (6)
    MessageDeliveryStatus: NotRequired[MessageDeliveryStatusEventConfigurationTypeDef],  # (7)
```

1. See [:material-code-brackets: IdentifierTypeType](./literals.md#identifiertypetype) 
2. See [:material-code-brackets: EventNotificationPartnerTypeType](./literals.md#eventnotificationpartnertypetype) 
3. See [:material-code-braces: DeviceRegistrationStateEventConfigurationTypeDef](./type_defs.md#deviceregistrationstateeventconfigurationtypedef) 
4. See [:material-code-braces: ProximityEventConfigurationTypeDef](./type_defs.md#proximityeventconfigurationtypedef) 
5. See [:material-code-braces: JoinEventConfigurationTypeDef](./type_defs.md#joineventconfigurationtypedef) 
6. See [:material-code-braces: ConnectionStatusEventConfigurationTypeDef](./type_defs.md#connectionstatuseventconfigurationtypedef) 
7. See [:material-code-braces: MessageDeliveryStatusEventConfigurationTypeDef](./type_defs.md#messagedeliverystatuseventconfigurationtypedef) 
## GetEventConfigurationByResourceTypesResponseTypeDef

```python
# GetEventConfigurationByResourceTypesResponseTypeDef definition

class GetEventConfigurationByResourceTypesResponseTypeDef(TypedDict):
    DeviceRegistrationState: DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,  # (1)
    Proximity: ProximityResourceTypeEventConfigurationTypeDef,  # (2)
    Join: JoinResourceTypeEventConfigurationTypeDef,  # (3)
    ConnectionStatus: ConnectionStatusResourceTypeEventConfigurationTypeDef,  # (4)
    MessageDeliveryStatus: MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: DeviceRegistrationStateResourceTypeEventConfigurationTypeDef](./type_defs.md#deviceregistrationstateresourcetypeeventconfigurationtypedef) 
2. See [:material-code-braces: ProximityResourceTypeEventConfigurationTypeDef](./type_defs.md#proximityresourcetypeeventconfigurationtypedef) 
3. See [:material-code-braces: JoinResourceTypeEventConfigurationTypeDef](./type_defs.md#joinresourcetypeeventconfigurationtypedef) 
4. See [:material-code-braces: ConnectionStatusResourceTypeEventConfigurationTypeDef](./type_defs.md#connectionstatusresourcetypeeventconfigurationtypedef) 
5. See [:material-code-braces: MessageDeliveryStatusResourceTypeEventConfigurationTypeDef](./type_defs.md#messagedeliverystatusresourcetypeeventconfigurationtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEventConfigurationByResourceTypesRequestRequestTypeDef

```python
# UpdateEventConfigurationByResourceTypesRequestRequestTypeDef definition

class UpdateEventConfigurationByResourceTypesRequestRequestTypeDef(TypedDict):
    DeviceRegistrationState: NotRequired[DeviceRegistrationStateResourceTypeEventConfigurationTypeDef],  # (1)
    Proximity: NotRequired[ProximityResourceTypeEventConfigurationTypeDef],  # (2)
    Join: NotRequired[JoinResourceTypeEventConfigurationTypeDef],  # (3)
    ConnectionStatus: NotRequired[ConnectionStatusResourceTypeEventConfigurationTypeDef],  # (4)
    MessageDeliveryStatus: NotRequired[MessageDeliveryStatusResourceTypeEventConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: DeviceRegistrationStateResourceTypeEventConfigurationTypeDef](./type_defs.md#deviceregistrationstateresourcetypeeventconfigurationtypedef) 
2. See [:material-code-braces: ProximityResourceTypeEventConfigurationTypeDef](./type_defs.md#proximityresourcetypeeventconfigurationtypedef) 
3. See [:material-code-braces: JoinResourceTypeEventConfigurationTypeDef](./type_defs.md#joinresourcetypeeventconfigurationtypedef) 
4. See [:material-code-braces: ConnectionStatusResourceTypeEventConfigurationTypeDef](./type_defs.md#connectionstatusresourcetypeeventconfigurationtypedef) 
5. See [:material-code-braces: MessageDeliveryStatusResourceTypeEventConfigurationTypeDef](./type_defs.md#messagedeliverystatusresourcetypeeventconfigurationtypedef) 
## GetWirelessDeviceStatisticsResponseTypeDef

```python
# GetWirelessDeviceStatisticsResponseTypeDef definition

class GetWirelessDeviceStatisticsResponseTypeDef(TypedDict):
    WirelessDeviceId: str,
    LastUplinkReceivedAt: str,
    LoRaWAN: LoRaWANDeviceMetadataTypeDef,  # (1)
    Sidewalk: SidewalkDeviceMetadataTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: LoRaWANDeviceMetadataTypeDef](./type_defs.md#lorawandevicemetadatatypedef) 
2. See [:material-code-braces: SidewalkDeviceMetadataTypeDef](./type_defs.md#sidewalkdevicemetadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWirelessGatewayFirmwareInformationResponseTypeDef

```python
# GetWirelessGatewayFirmwareInformationResponseTypeDef definition

class GetWirelessGatewayFirmwareInformationResponseTypeDef(TypedDict):
    LoRaWAN: LoRaWANGatewayCurrentVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoRaWANGatewayCurrentVersionTypeDef](./type_defs.md#lorawangatewaycurrentversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWirelessGatewayTaskCreateTypeDef

```python
# UpdateWirelessGatewayTaskCreateTypeDef definition

class UpdateWirelessGatewayTaskCreateTypeDef(TypedDict):
    UpdateDataSource: NotRequired[str],
    UpdateDataRole: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANUpdateGatewayTaskCreateTypeDef],  # (1)
```

1. See [:material-code-braces: LoRaWANUpdateGatewayTaskCreateTypeDef](./type_defs.md#lorawanupdategatewaytaskcreatetypedef) 
## UpdateWirelessGatewayTaskEntryTypeDef

```python
# UpdateWirelessGatewayTaskEntryTypeDef definition

class UpdateWirelessGatewayTaskEntryTypeDef(TypedDict):
    Id: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANUpdateGatewayTaskEntryTypeDef],  # (1)
    Arn: NotRequired[str],
```

1. See [:material-code-braces: LoRaWANUpdateGatewayTaskEntryTypeDef](./type_defs.md#lorawanupdategatewaytaskentrytypedef) 
## GetMulticastGroupResponseTypeDef

```python
# GetMulticastGroupResponseTypeDef definition

class GetMulticastGroupResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Name: str,
    Description: str,
    Status: str,
    LoRaWAN: LoRaWANMulticastGetTypeDef,  # (1)
    CreatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoRaWANMulticastGetTypeDef](./type_defs.md#lorawanmulticastgettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendDataToMulticastGroupRequestRequestTypeDef

```python
# SendDataToMulticastGroupRequestRequestTypeDef definition

class SendDataToMulticastGroupRequestRequestTypeDef(TypedDict):
    Id: str,
    PayloadData: str,
    WirelessMetadata: MulticastWirelessMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: MulticastWirelessMetadataTypeDef](./type_defs.md#multicastwirelessmetadatatypedef) 
## GetMetricsResponseTypeDef

```python
# GetMetricsResponseTypeDef definition

class GetMetricsResponseTypeDef(TypedDict):
    SummaryMetricQueryResults: List[SummaryMetricQueryResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SummaryMetricQueryResultTypeDef](./type_defs.md#summarymetricqueryresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoRaWANMulticastTypeDef

```python
# LoRaWANMulticastTypeDef definition

class LoRaWANMulticastTypeDef(TypedDict):
    RfRegion: NotRequired[SupportedRfRegionType],  # (1)
    DlClass: NotRequired[DlClassType],  # (2)
    ParticipatingGateways: NotRequired[ParticipatingGatewaysMulticastUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: SupportedRfRegionType](./literals.md#supportedrfregiontype) 
2. See [:material-code-brackets: DlClassType](./literals.md#dlclasstype) 
3. See [:material-code-braces: ParticipatingGatewaysMulticastTypeDef](./type_defs.md#participatinggatewaysmulticasttypedef) [:material-code-braces: ParticipatingGatewaysMulticastOutputTypeDef](./type_defs.md#participatinggatewaysmulticastoutputtypedef) 
## PutPositionConfigurationRequestRequestTypeDef

```python
# PutPositionConfigurationRequestRequestTypeDef definition

class PutPositionConfigurationRequestRequestTypeDef(TypedDict):
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
    Solvers: NotRequired[PositionSolverConfigurationsTypeDef],  # (2)
    Destination: NotRequired[str],
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
2. See [:material-code-braces: PositionSolverConfigurationsTypeDef](./type_defs.md#positionsolverconfigurationstypedef) 
## GetPositionConfigurationResponseTypeDef

```python
# GetPositionConfigurationResponseTypeDef definition

class GetPositionConfigurationResponseTypeDef(TypedDict):
    Solvers: PositionSolverDetailsTypeDef,  # (1)
    Destination: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PositionSolverDetailsTypeDef](./type_defs.md#positionsolverdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PositionConfigurationItemTypeDef

```python
# PositionConfigurationItemTypeDef definition

class PositionConfigurationItemTypeDef(TypedDict):
    ResourceIdentifier: NotRequired[str],
    ResourceType: NotRequired[PositionResourceTypeType],  # (1)
    Solvers: NotRequired[PositionSolverDetailsTypeDef],  # (2)
    Destination: NotRequired[str],
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
2. See [:material-code-braces: PositionSolverDetailsTypeDef](./type_defs.md#positionsolverdetailstypedef) 
## GetLogLevelsByResourceTypesResponseTypeDef

```python
# GetLogLevelsByResourceTypesResponseTypeDef definition

class GetLogLevelsByResourceTypesResponseTypeDef(TypedDict):
    DefaultLogLevel: LogLevelType,  # (1)
    WirelessGatewayLogOptions: List[WirelessGatewayLogOptionOutputTypeDef],  # (2)
    WirelessDeviceLogOptions: List[WirelessDeviceLogOptionOutputTypeDef],  # (3)
    FuotaTaskLogOptions: List[FuotaTaskLogOptionOutputTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
2. See [:material-code-braces: WirelessGatewayLogOptionOutputTypeDef](./type_defs.md#wirelessgatewaylogoptionoutputtypedef) 
3. See [:material-code-braces: WirelessDeviceLogOptionOutputTypeDef](./type_defs.md#wirelessdevicelogoptionoutputtypedef) 
4. See [:material-code-braces: FuotaTaskLogOptionOutputTypeDef](./type_defs.md#fuotatasklogoptionoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWirelessGatewaysResponseTypeDef

```python
# ListWirelessGatewaysResponseTypeDef definition

class ListWirelessGatewaysResponseTypeDef(TypedDict):
    WirelessGatewayList: List[WirelessGatewayStatisticsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WirelessGatewayStatisticsTypeDef](./type_defs.md#wirelessgatewaystatisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWirelessGatewayRequestRequestTypeDef

```python
# CreateWirelessGatewayRequestRequestTypeDef definition

class CreateWirelessGatewayRequestRequestTypeDef(TypedDict):
    LoRaWAN: LoRaWANGatewayTypeDef,  # (1)
    Name: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: LoRaWANGatewayTypeDef](./type_defs.md#lorawangatewaytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListWirelessDevicesResponseTypeDef

```python
# ListWirelessDevicesResponseTypeDef definition

class ListWirelessDevicesResponseTypeDef(TypedDict):
    WirelessDeviceList: List[WirelessDeviceStatisticsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WirelessDeviceStatisticsTypeDef](./type_defs.md#wirelessdevicestatisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWirelessDeviceResponseTypeDef

```python
# GetWirelessDeviceResponseTypeDef definition

class GetWirelessDeviceResponseTypeDef(TypedDict):
    Type: WirelessDeviceTypeType,  # (1)
    Name: str,
    Description: str,
    DestinationName: str,
    Id: str,
    Arn: str,
    ThingName: str,
    ThingArn: str,
    LoRaWAN: LoRaWANDeviceOutputTypeDef,  # (2)
    Sidewalk: SidewalkDeviceTypeDef,  # (3)
    Positioning: PositioningConfigStatusType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
2. See [:material-code-braces: LoRaWANDeviceOutputTypeDef](./type_defs.md#lorawandeviceoutputtypedef) 
3. See [:material-code-braces: SidewalkDeviceTypeDef](./type_defs.md#sidewalkdevicetypedef) 
4. See [:material-code-brackets: PositioningConfigStatusType](./literals.md#positioningconfigstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoRaWANDeviceTypeDef

```python
# LoRaWANDeviceTypeDef definition

class LoRaWANDeviceTypeDef(TypedDict):
    DevEui: NotRequired[str],
    DeviceProfileId: NotRequired[str],
    ServiceProfileId: NotRequired[str],
    OtaaV1_1: NotRequired[OtaaV11TypeDef],  # (1)
    OtaaV1_0_x: NotRequired[OtaaV10XTypeDef],  # (2)
    AbpV1_1: NotRequired[AbpV11TypeDef],  # (3)
    AbpV1_0_x: NotRequired[AbpV10XTypeDef],  # (4)
    FPorts: NotRequired[FPortsUnionTypeDef],  # (5)
```

1. See [:material-code-braces: OtaaV11TypeDef](./type_defs.md#otaav11typedef) 
2. See [:material-code-braces: OtaaV10XTypeDef](./type_defs.md#otaav10xtypedef) 
3. See [:material-code-braces: AbpV11TypeDef](./type_defs.md#abpv11typedef) 
4. See [:material-code-braces: AbpV10XTypeDef](./type_defs.md#abpv10xtypedef) 
5. See [:material-code-braces: FPortsTypeDef](./type_defs.md#fportstypedef) [:material-code-braces: FPortsOutputTypeDef](./type_defs.md#fportsoutputtypedef) 
## UpdateWirelessDeviceRequestRequestTypeDef

```python
# UpdateWirelessDeviceRequestRequestTypeDef definition

class UpdateWirelessDeviceRequestRequestTypeDef(TypedDict):
    Id: str,
    DestinationName: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANUpdateDeviceTypeDef],  # (1)
    Positioning: NotRequired[PositioningConfigStatusType],  # (2)
```

1. See [:material-code-braces: LoRaWANUpdateDeviceTypeDef](./type_defs.md#lorawanupdatedevicetypedef) 
2. See [:material-code-brackets: PositioningConfigStatusType](./literals.md#positioningconfigstatustype) 
## DownlinkQueueMessageTypeDef

```python
# DownlinkQueueMessageTypeDef definition

class DownlinkQueueMessageTypeDef(TypedDict):
    MessageId: NotRequired[str],
    TransmitMode: NotRequired[int],
    ReceivedAt: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANSendDataToDeviceOutputTypeDef],  # (1)
```

1. See [:material-code-braces: LoRaWANSendDataToDeviceOutputTypeDef](./type_defs.md#lorawansenddatatodeviceoutputtypedef) 
## LoRaWANSendDataToDeviceTypeDef

```python
# LoRaWANSendDataToDeviceTypeDef definition

class LoRaWANSendDataToDeviceTypeDef(TypedDict):
    FPort: NotRequired[int],
    ParticipatingGateways: NotRequired[ParticipatingGatewaysUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ParticipatingGatewaysTypeDef](./type_defs.md#participatinggatewaystypedef) [:material-code-braces: ParticipatingGatewaysOutputTypeDef](./type_defs.md#participatinggatewaysoutputtypedef) 
## CellTowersTypeDef

```python
# CellTowersTypeDef definition

class CellTowersTypeDef(TypedDict):
    Gsm: NotRequired[Sequence[GsmObjTypeDef]],  # (1)
    Wcdma: NotRequired[Sequence[WcdmaObjTypeDef]],  # (2)
    Tdscdma: NotRequired[Sequence[TdscdmaObjTypeDef]],  # (3)
    Lte: NotRequired[Sequence[LteObjTypeDef]],  # (4)
    Cdma: NotRequired[Sequence[CdmaObjTypeDef]],  # (5)
```

1. See [:material-code-braces: GsmObjTypeDef](./type_defs.md#gsmobjtypedef) 
2. See [:material-code-braces: WcdmaObjTypeDef](./type_defs.md#wcdmaobjtypedef) 
3. See [:material-code-braces: TdscdmaObjTypeDef](./type_defs.md#tdscdmaobjtypedef) 
4. See [:material-code-braces: LteObjTypeDef](./type_defs.md#lteobjtypedef) 
5. See [:material-code-braces: CdmaObjTypeDef](./type_defs.md#cdmaobjtypedef) 
## EventConfigurationItemTypeDef

```python
# EventConfigurationItemTypeDef definition

class EventConfigurationItemTypeDef(TypedDict):
    Identifier: NotRequired[str],
    IdentifierType: NotRequired[IdentifierTypeType],  # (1)
    PartnerType: NotRequired[EventNotificationPartnerTypeType],  # (2)
    Events: NotRequired[EventNotificationItemConfigurationsTypeDef],  # (3)
```

1. See [:material-code-brackets: IdentifierTypeType](./literals.md#identifiertypetype) 
2. See [:material-code-brackets: EventNotificationPartnerTypeType](./literals.md#eventnotificationpartnertypetype) 
3. See [:material-code-braces: EventNotificationItemConfigurationsTypeDef](./type_defs.md#eventnotificationitemconfigurationstypedef) 
## CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef

```python
# CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef definition

class CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef(TypedDict):
    AutoCreateTasks: bool,
    Name: NotRequired[str],
    Update: NotRequired[UpdateWirelessGatewayTaskCreateTypeDef],  # (1)
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: UpdateWirelessGatewayTaskCreateTypeDef](./type_defs.md#updatewirelessgatewaytaskcreatetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetWirelessGatewayTaskDefinitionResponseTypeDef

```python
# GetWirelessGatewayTaskDefinitionResponseTypeDef definition

class GetWirelessGatewayTaskDefinitionResponseTypeDef(TypedDict):
    AutoCreateTasks: bool,
    Name: str,
    Update: UpdateWirelessGatewayTaskCreateTypeDef,  # (1)
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateWirelessGatewayTaskCreateTypeDef](./type_defs.md#updatewirelessgatewaytaskcreatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWirelessGatewayTaskDefinitionsResponseTypeDef

```python
# ListWirelessGatewayTaskDefinitionsResponseTypeDef definition

class ListWirelessGatewayTaskDefinitionsResponseTypeDef(TypedDict):
    TaskDefinitions: List[UpdateWirelessGatewayTaskEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UpdateWirelessGatewayTaskEntryTypeDef](./type_defs.md#updatewirelessgatewaytaskentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMulticastGroupRequestRequestTypeDef

```python
# CreateMulticastGroupRequestRequestTypeDef definition

class CreateMulticastGroupRequestRequestTypeDef(TypedDict):
    LoRaWAN: LoRaWANMulticastTypeDef,  # (1)
    Name: NotRequired[str],
    Description: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: LoRaWANMulticastTypeDef](./type_defs.md#lorawanmulticasttypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateMulticastGroupRequestRequestTypeDef

```python
# UpdateMulticastGroupRequestRequestTypeDef definition

class UpdateMulticastGroupRequestRequestTypeDef(TypedDict):
    Id: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANMulticastTypeDef],  # (1)
```

1. See [:material-code-braces: LoRaWANMulticastTypeDef](./type_defs.md#lorawanmulticasttypedef) 
## ListPositionConfigurationsResponseTypeDef

```python
# ListPositionConfigurationsResponseTypeDef definition

class ListPositionConfigurationsResponseTypeDef(TypedDict):
    PositionConfigurationList: List[PositionConfigurationItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PositionConfigurationItemTypeDef](./type_defs.md#positionconfigurationitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLogLevelsByResourceTypesRequestRequestTypeDef

```python
# UpdateLogLevelsByResourceTypesRequestRequestTypeDef definition

class UpdateLogLevelsByResourceTypesRequestRequestTypeDef(TypedDict):
    DefaultLogLevel: NotRequired[LogLevelType],  # (1)
    FuotaTaskLogOptions: NotRequired[Sequence[FuotaTaskLogOptionUnionTypeDef]],  # (2)
    WirelessDeviceLogOptions: NotRequired[Sequence[WirelessDeviceLogOptionUnionTypeDef]],  # (3)
    WirelessGatewayLogOptions: NotRequired[Sequence[WirelessGatewayLogOptionUnionTypeDef]],  # (4)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
2. See [:material-code-braces: FuotaTaskLogOptionTypeDef](./type_defs.md#fuotatasklogoptiontypedef) [:material-code-braces: FuotaTaskLogOptionOutputTypeDef](./type_defs.md#fuotatasklogoptionoutputtypedef) 
3. See [:material-code-braces: WirelessDeviceLogOptionTypeDef](./type_defs.md#wirelessdevicelogoptiontypedef) [:material-code-braces: WirelessDeviceLogOptionOutputTypeDef](./type_defs.md#wirelessdevicelogoptionoutputtypedef) 
4. See [:material-code-braces: WirelessGatewayLogOptionTypeDef](./type_defs.md#wirelessgatewaylogoptiontypedef) [:material-code-braces: WirelessGatewayLogOptionOutputTypeDef](./type_defs.md#wirelessgatewaylogoptionoutputtypedef) 
## CreateWirelessDeviceRequestRequestTypeDef

```python
# CreateWirelessDeviceRequestRequestTypeDef definition

class CreateWirelessDeviceRequestRequestTypeDef(TypedDict):
    Type: WirelessDeviceTypeType,  # (1)
    DestinationName: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    LoRaWAN: NotRequired[LoRaWANDeviceTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    Positioning: NotRequired[PositioningConfigStatusType],  # (4)
    Sidewalk: NotRequired[SidewalkCreateWirelessDeviceTypeDef],  # (5)
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
2. See [:material-code-braces: LoRaWANDeviceTypeDef](./type_defs.md#lorawandevicetypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: PositioningConfigStatusType](./literals.md#positioningconfigstatustype) 
5. See [:material-code-braces: SidewalkCreateWirelessDeviceTypeDef](./type_defs.md#sidewalkcreatewirelessdevicetypedef) 
## ListQueuedMessagesResponseTypeDef

```python
# ListQueuedMessagesResponseTypeDef definition

class ListQueuedMessagesResponseTypeDef(TypedDict):
    DownlinkQueueMessagesList: List[DownlinkQueueMessageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DownlinkQueueMessageTypeDef](./type_defs.md#downlinkqueuemessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPositionEstimateRequestRequestTypeDef

```python
# GetPositionEstimateRequestRequestTypeDef definition

class GetPositionEstimateRequestRequestTypeDef(TypedDict):
    WiFiAccessPoints: NotRequired[Sequence[WiFiAccessPointTypeDef]],  # (1)
    CellTowers: NotRequired[CellTowersTypeDef],  # (2)
    Ip: NotRequired[IpTypeDef],  # (3)
    Gnss: NotRequired[GnssTypeDef],  # (4)
    Timestamp: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: WiFiAccessPointTypeDef](./type_defs.md#wifiaccesspointtypedef) 
2. See [:material-code-braces: CellTowersTypeDef](./type_defs.md#celltowerstypedef) 
3. See [:material-code-braces: IpTypeDef](./type_defs.md#iptypedef) 
4. See [:material-code-braces: GnssTypeDef](./type_defs.md#gnsstypedef) 
## ListEventConfigurationsResponseTypeDef

```python
# ListEventConfigurationsResponseTypeDef definition

class ListEventConfigurationsResponseTypeDef(TypedDict):
    EventConfigurationsList: List[EventConfigurationItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EventConfigurationItemTypeDef](./type_defs.md#eventconfigurationitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WirelessMetadataTypeDef

```python
# WirelessMetadataTypeDef definition

class WirelessMetadataTypeDef(TypedDict):
    LoRaWAN: NotRequired[LoRaWANSendDataToDeviceUnionTypeDef],  # (1)
    Sidewalk: NotRequired[SidewalkSendDataToDeviceTypeDef],  # (2)
```

1. See [:material-code-braces: LoRaWANSendDataToDeviceTypeDef](./type_defs.md#lorawansenddatatodevicetypedef) [:material-code-braces: LoRaWANSendDataToDeviceOutputTypeDef](./type_defs.md#lorawansenddatatodeviceoutputtypedef) 
2. See [:material-code-braces: SidewalkSendDataToDeviceTypeDef](./type_defs.md#sidewalksenddatatodevicetypedef) 
## SendDataToWirelessDeviceRequestRequestTypeDef

```python
# SendDataToWirelessDeviceRequestRequestTypeDef definition

class SendDataToWirelessDeviceRequestRequestTypeDef(TypedDict):
    Id: str,
    TransmitMode: int,
    PayloadData: str,
    WirelessMetadata: NotRequired[WirelessMetadataTypeDef],  # (1)
```

1. See [:material-code-braces: WirelessMetadataTypeDef](./type_defs.md#wirelessmetadatatypedef) 
