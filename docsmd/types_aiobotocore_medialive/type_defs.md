# Type definitions

> [Index](../README.md) > [MediaLive](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MediaLive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
    type annotations stubs module [types-aiobotocore-medialive](https://pypi.org/project/types-aiobotocore-medialive/).



## AacSettingsTypeDef

```python
# AacSettingsTypeDef definition

class AacSettingsTypeDef(TypedDict):
    Bitrate: NotRequired[float],
    CodingMode: NotRequired[AacCodingModeType],  # (1)
    InputType: NotRequired[AacInputTypeType],  # (2)
    Profile: NotRequired[AacProfileType],  # (3)
    RateControlMode: NotRequired[AacRateControlModeType],  # (4)
    RawFormat: NotRequired[AacRawFormatType],  # (5)
    SampleRate: NotRequired[float],
    Spec: NotRequired[AacSpecType],  # (6)
    VbrQuality: NotRequired[AacVbrQualityType],  # (7)
```

1. See [:material-code-brackets: AacCodingModeType](./literals.md#aaccodingmodetype) 
2. See [:material-code-brackets: AacInputTypeType](./literals.md#aacinputtypetype) 
3. See [:material-code-brackets: AacProfileType](./literals.md#aacprofiletype) 
4. See [:material-code-brackets: AacRateControlModeType](./literals.md#aacratecontrolmodetype) 
5. See [:material-code-brackets: AacRawFormatType](./literals.md#aacrawformattype) 
6. See [:material-code-brackets: AacSpecType](./literals.md#aacspectype) 
7. See [:material-code-brackets: AacVbrQualityType](./literals.md#aacvbrqualitytype) 
## Ac3SettingsTypeDef

```python
# Ac3SettingsTypeDef definition

class Ac3SettingsTypeDef(TypedDict):
    Bitrate: NotRequired[float],
    BitstreamMode: NotRequired[Ac3BitstreamModeType],  # (1)
    CodingMode: NotRequired[Ac3CodingModeType],  # (2)
    Dialnorm: NotRequired[int],
    DrcProfile: NotRequired[Ac3DrcProfileType],  # (3)
    LfeFilter: NotRequired[Ac3LfeFilterType],  # (4)
    MetadataControl: NotRequired[Ac3MetadataControlType],  # (5)
```

1. See [:material-code-brackets: Ac3BitstreamModeType](./literals.md#ac3bitstreammodetype) 
2. See [:material-code-brackets: Ac3CodingModeType](./literals.md#ac3codingmodetype) 
3. See [:material-code-brackets: Ac3DrcProfileType](./literals.md#ac3drcprofiletype) 
4. See [:material-code-brackets: Ac3LfeFilterType](./literals.md#ac3lfefiltertype) 
5. See [:material-code-brackets: Ac3MetadataControlType](./literals.md#ac3metadatacontroltype) 
## AcceptInputDeviceTransferRequestRequestTypeDef

```python
# AcceptInputDeviceTransferRequestRequestTypeDef definition

class AcceptInputDeviceTransferRequestRequestTypeDef(TypedDict):
    InputDeviceId: str,
```

## AccountConfigurationTypeDef

```python
# AccountConfigurationTypeDef definition

class AccountConfigurationTypeDef(TypedDict):
    KmsKeyId: NotRequired[str],
```

## AncillarySourceSettingsTypeDef

```python
# AncillarySourceSettingsTypeDef definition

class AncillarySourceSettingsTypeDef(TypedDict):
    SourceAncillaryChannelNumber: NotRequired[int],
```

## ArchiveS3SettingsTypeDef

```python
# ArchiveS3SettingsTypeDef definition

class ArchiveS3SettingsTypeDef(TypedDict):
    CannedAcl: NotRequired[S3CannedAclType],  # (1)
```

1. See [:material-code-brackets: S3CannedAclType](./literals.md#s3cannedacltype) 
## OutputLocationRefTypeDef

```python
# OutputLocationRefTypeDef definition

class OutputLocationRefTypeDef(TypedDict):
    DestinationRefId: NotRequired[str],
```

## InputChannelLevelTypeDef

```python
# InputChannelLevelTypeDef definition

class InputChannelLevelTypeDef(TypedDict):
    Gain: int,
    InputChannel: int,
```

## Eac3AtmosSettingsTypeDef

```python
# Eac3AtmosSettingsTypeDef definition

class Eac3AtmosSettingsTypeDef(TypedDict):
    Bitrate: NotRequired[float],
    CodingMode: NotRequired[Eac3AtmosCodingModeType],  # (1)
    Dialnorm: NotRequired[int],
    DrcLine: NotRequired[Eac3AtmosDrcLineType],  # (2)
    DrcRf: NotRequired[Eac3AtmosDrcRfType],  # (3)
    HeightTrim: NotRequired[float],
    SurroundTrim: NotRequired[float],
```

1. See [:material-code-brackets: Eac3AtmosCodingModeType](./literals.md#eac3atmoscodingmodetype) 
2. See [:material-code-brackets: Eac3AtmosDrcLineType](./literals.md#eac3atmosdrclinetype) 
3. See [:material-code-brackets: Eac3AtmosDrcRfType](./literals.md#eac3atmosdrcrftype) 
## Eac3SettingsTypeDef

```python
# Eac3SettingsTypeDef definition

class Eac3SettingsTypeDef(TypedDict):
    AttenuationControl: NotRequired[Eac3AttenuationControlType],  # (1)
    Bitrate: NotRequired[float],
    BitstreamMode: NotRequired[Eac3BitstreamModeType],  # (2)
    CodingMode: NotRequired[Eac3CodingModeType],  # (3)
    DcFilter: NotRequired[Eac3DcFilterType],  # (4)
    Dialnorm: NotRequired[int],
    DrcLine: NotRequired[Eac3DrcLineType],  # (5)
    DrcRf: NotRequired[Eac3DrcRfType],  # (6)
    LfeControl: NotRequired[Eac3LfeControlType],  # (7)
    LfeFilter: NotRequired[Eac3LfeFilterType],  # (8)
    LoRoCenterMixLevel: NotRequired[float],
    LoRoSurroundMixLevel: NotRequired[float],
    LtRtCenterMixLevel: NotRequired[float],
    LtRtSurroundMixLevel: NotRequired[float],
    MetadataControl: NotRequired[Eac3MetadataControlType],  # (9)
    PassthroughControl: NotRequired[Eac3PassthroughControlType],  # (10)
    PhaseControl: NotRequired[Eac3PhaseControlType],  # (11)
    StereoDownmix: NotRequired[Eac3StereoDownmixType],  # (12)
    SurroundExMode: NotRequired[Eac3SurroundExModeType],  # (13)
    SurroundMode: NotRequired[Eac3SurroundModeType],  # (14)
```

1. See [:material-code-brackets: Eac3AttenuationControlType](./literals.md#eac3attenuationcontroltype) 
2. See [:material-code-brackets: Eac3BitstreamModeType](./literals.md#eac3bitstreammodetype) 
3. See [:material-code-brackets: Eac3CodingModeType](./literals.md#eac3codingmodetype) 
4. See [:material-code-brackets: Eac3DcFilterType](./literals.md#eac3dcfiltertype) 
5. See [:material-code-brackets: Eac3DrcLineType](./literals.md#eac3drclinetype) 
6. See [:material-code-brackets: Eac3DrcRfType](./literals.md#eac3drcrftype) 
7. See [:material-code-brackets: Eac3LfeControlType](./literals.md#eac3lfecontroltype) 
8. See [:material-code-brackets: Eac3LfeFilterType](./literals.md#eac3lfefiltertype) 
9. See [:material-code-brackets: Eac3MetadataControlType](./literals.md#eac3metadatacontroltype) 
10. See [:material-code-brackets: Eac3PassthroughControlType](./literals.md#eac3passthroughcontroltype) 
11. See [:material-code-brackets: Eac3PhaseControlType](./literals.md#eac3phasecontroltype) 
12. See [:material-code-brackets: Eac3StereoDownmixType](./literals.md#eac3stereodownmixtype) 
13. See [:material-code-brackets: Eac3SurroundExModeType](./literals.md#eac3surroundexmodetype) 
14. See [:material-code-brackets: Eac3SurroundModeType](./literals.md#eac3surroundmodetype) 
## Mp2SettingsTypeDef

```python
# Mp2SettingsTypeDef definition

class Mp2SettingsTypeDef(TypedDict):
    Bitrate: NotRequired[float],
    CodingMode: NotRequired[Mp2CodingModeType],  # (1)
    SampleRate: NotRequired[float],
```

1. See [:material-code-brackets: Mp2CodingModeType](./literals.md#mp2codingmodetype) 
## WavSettingsTypeDef

```python
# WavSettingsTypeDef definition

class WavSettingsTypeDef(TypedDict):
    BitDepth: NotRequired[float],
    CodingMode: NotRequired[WavCodingModeType],  # (1)
    SampleRate: NotRequired[float],
```

1. See [:material-code-brackets: WavCodingModeType](./literals.md#wavcodingmodetype) 
## AudioNormalizationSettingsTypeDef

```python
# AudioNormalizationSettingsTypeDef definition

class AudioNormalizationSettingsTypeDef(TypedDict):
    Algorithm: NotRequired[AudioNormalizationAlgorithmType],  # (1)
    AlgorithmControl: NotRequired[AudioNormalizationAlgorithmControlType],  # (2)
    TargetLkfs: NotRequired[float],
```

1. See [:material-code-brackets: AudioNormalizationAlgorithmType](./literals.md#audionormalizationalgorithmtype) 
2. See [:material-code-brackets: AudioNormalizationAlgorithmControlType](./literals.md#audionormalizationalgorithmcontroltype) 
## AudioDolbyEDecodeTypeDef

```python
# AudioDolbyEDecodeTypeDef definition

class AudioDolbyEDecodeTypeDef(TypedDict):
    ProgramSelection: DolbyEProgramSelectionType,  # (1)
```

1. See [:material-code-brackets: DolbyEProgramSelectionType](./literals.md#dolbyeprogramselectiontype) 
## AudioHlsRenditionSelectionTypeDef

```python
# AudioHlsRenditionSelectionTypeDef definition

class AudioHlsRenditionSelectionTypeDef(TypedDict):
    GroupId: str,
    Name: str,
```

## AudioLanguageSelectionTypeDef

```python
# AudioLanguageSelectionTypeDef definition

class AudioLanguageSelectionTypeDef(TypedDict):
    LanguageCode: str,
    LanguageSelectionPolicy: NotRequired[AudioLanguageSelectionPolicyType],  # (1)
```

1. See [:material-code-brackets: AudioLanguageSelectionPolicyType](./literals.md#audiolanguageselectionpolicytype) 
## InputLocationTypeDef

```python
# InputLocationTypeDef definition

class InputLocationTypeDef(TypedDict):
    Uri: str,
    PasswordParam: NotRequired[str],
    Username: NotRequired[str],
```

## AudioPidSelectionTypeDef

```python
# AudioPidSelectionTypeDef definition

class AudioPidSelectionTypeDef(TypedDict):
    Pid: int,
```

## AudioSilenceFailoverSettingsTypeDef

```python
# AudioSilenceFailoverSettingsTypeDef definition

class AudioSilenceFailoverSettingsTypeDef(TypedDict):
    AudioSelectorName: str,
    AudioSilenceThresholdMsec: NotRequired[int],
```

## AudioTrackTypeDef

```python
# AudioTrackTypeDef definition

class AudioTrackTypeDef(TypedDict):
    Track: int,
```

## EsamTypeDef

```python
# EsamTypeDef definition

class EsamTypeDef(TypedDict):
    AcquisitionPointId: str,
    PoisEndpoint: str,
    AdAvailOffset: NotRequired[int],
    PasswordParam: NotRequired[str],
    Username: NotRequired[str],
    ZoneIdentity: NotRequired[str],
```

## Scte35SpliceInsertTypeDef

```python
# Scte35SpliceInsertTypeDef definition

class Scte35SpliceInsertTypeDef(TypedDict):
    AdAvailOffset: NotRequired[int],
    NoRegionalBlackoutFlag: NotRequired[Scte35SpliceInsertNoRegionalBlackoutBehaviorType],  # (1)
    WebDeliveryAllowedFlag: NotRequired[Scte35SpliceInsertWebDeliveryAllowedBehaviorType],  # (2)
```

1. See [:material-code-brackets: Scte35SpliceInsertNoRegionalBlackoutBehaviorType](./literals.md#scte35spliceinsertnoregionalblackoutbehaviortype) 
2. See [:material-code-brackets: Scte35SpliceInsertWebDeliveryAllowedBehaviorType](./literals.md#scte35spliceinsertwebdeliveryallowedbehaviortype) 
## Scte35TimeSignalAposTypeDef

```python
# Scte35TimeSignalAposTypeDef definition

class Scte35TimeSignalAposTypeDef(TypedDict):
    AdAvailOffset: NotRequired[int],
    NoRegionalBlackoutFlag: NotRequired[Scte35AposNoRegionalBlackoutBehaviorType],  # (1)
    WebDeliveryAllowedFlag: NotRequired[Scte35AposWebDeliveryAllowedBehaviorType],  # (2)
```

1. See [:material-code-brackets: Scte35AposNoRegionalBlackoutBehaviorType](./literals.md#scte35aposnoregionalblackoutbehaviortype) 
2. See [:material-code-brackets: Scte35AposWebDeliveryAllowedBehaviorType](./literals.md#scte35aposwebdeliveryallowedbehaviortype) 
## BatchDeleteRequestRequestTypeDef

```python
# BatchDeleteRequestRequestTypeDef definition

class BatchDeleteRequestRequestTypeDef(TypedDict):
    ChannelIds: NotRequired[Sequence[str]],
    InputIds: NotRequired[Sequence[str]],
    InputSecurityGroupIds: NotRequired[Sequence[str]],
    MultiplexIds: NotRequired[Sequence[str]],
```

## BatchFailedResultModelTypeDef

```python
# BatchFailedResultModelTypeDef definition

class BatchFailedResultModelTypeDef(TypedDict):
    Arn: NotRequired[str],
    Code: NotRequired[str],
    Id: NotRequired[str],
    Message: NotRequired[str],
```

## BatchSuccessfulResultModelTypeDef

```python
# BatchSuccessfulResultModelTypeDef definition

class BatchSuccessfulResultModelTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    State: NotRequired[str],
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

## BatchScheduleActionDeleteRequestTypeDef

```python
# BatchScheduleActionDeleteRequestTypeDef definition

class BatchScheduleActionDeleteRequestTypeDef(TypedDict):
    ActionNames: Sequence[str],
```

## BatchStartRequestRequestTypeDef

```python
# BatchStartRequestRequestTypeDef definition

class BatchStartRequestRequestTypeDef(TypedDict):
    ChannelIds: NotRequired[Sequence[str]],
    MultiplexIds: NotRequired[Sequence[str]],
```

## BatchStopRequestRequestTypeDef

```python
# BatchStopRequestRequestTypeDef definition

class BatchStopRequestRequestTypeDef(TypedDict):
    ChannelIds: NotRequired[Sequence[str]],
    MultiplexIds: NotRequired[Sequence[str]],
```

## CancelInputDeviceTransferRequestRequestTypeDef

```python
# CancelInputDeviceTransferRequestRequestTypeDef definition

class CancelInputDeviceTransferRequestRequestTypeDef(TypedDict):
    InputDeviceId: str,
```

## EbuTtDDestinationSettingsTypeDef

```python
# EbuTtDDestinationSettingsTypeDef definition

class EbuTtDDestinationSettingsTypeDef(TypedDict):
    CopyrightHolder: NotRequired[str],
    FillLineGap: NotRequired[EbuTtDFillLineGapControlType],  # (1)
    FontFamily: NotRequired[str],
    StyleControl: NotRequired[EbuTtDDestinationStyleControlType],  # (2)
```

1. See [:material-code-brackets: EbuTtDFillLineGapControlType](./literals.md#ebuttdfilllinegapcontroltype) 
2. See [:material-code-brackets: EbuTtDDestinationStyleControlType](./literals.md#ebuttddestinationstylecontroltype) 
## TtmlDestinationSettingsTypeDef

```python
# TtmlDestinationSettingsTypeDef definition

class TtmlDestinationSettingsTypeDef(TypedDict):
    StyleControl: NotRequired[TtmlDestinationStyleControlType],  # (1)
```

1. See [:material-code-brackets: TtmlDestinationStyleControlType](./literals.md#ttmldestinationstylecontroltype) 
## WebvttDestinationSettingsTypeDef

```python
# WebvttDestinationSettingsTypeDef definition

class WebvttDestinationSettingsTypeDef(TypedDict):
    StyleControl: NotRequired[WebvttDestinationStyleControlType],  # (1)
```

1. See [:material-code-brackets: WebvttDestinationStyleControlType](./literals.md#webvttdestinationstylecontroltype) 
## CaptionLanguageMappingTypeDef

```python
# CaptionLanguageMappingTypeDef definition

class CaptionLanguageMappingTypeDef(TypedDict):
    CaptionChannel: int,
    LanguageCode: str,
    LanguageDescription: str,
```

## CaptionRectangleTypeDef

```python
# CaptionRectangleTypeDef definition

class CaptionRectangleTypeDef(TypedDict):
    Height: float,
    LeftOffset: float,
    TopOffset: float,
    Width: float,
```

## DvbSubSourceSettingsTypeDef

```python
# DvbSubSourceSettingsTypeDef definition

class DvbSubSourceSettingsTypeDef(TypedDict):
    OcrLanguage: NotRequired[DvbSubOcrLanguageType],  # (1)
    Pid: NotRequired[int],
```

1. See [:material-code-brackets: DvbSubOcrLanguageType](./literals.md#dvbsubocrlanguagetype) 
## EmbeddedSourceSettingsTypeDef

```python
# EmbeddedSourceSettingsTypeDef definition

class EmbeddedSourceSettingsTypeDef(TypedDict):
    Convert608To708: NotRequired[EmbeddedConvert608To708Type],  # (1)
    Scte20Detection: NotRequired[EmbeddedScte20DetectionType],  # (2)
    Source608ChannelNumber: NotRequired[int],
    Source608TrackNumber: NotRequired[int],
```

1. See [:material-code-brackets: EmbeddedConvert608To708Type](./literals.md#embeddedconvert608to708type) 
2. See [:material-code-brackets: EmbeddedScte20DetectionType](./literals.md#embeddedscte20detectiontype) 
## Scte20SourceSettingsTypeDef

```python
# Scte20SourceSettingsTypeDef definition

class Scte20SourceSettingsTypeDef(TypedDict):
    Convert608To708: NotRequired[Scte20Convert608To708Type],  # (1)
    Source608ChannelNumber: NotRequired[int],
```

1. See [:material-code-brackets: Scte20Convert608To708Type](./literals.md#scte20convert608to708type) 
## Scte27SourceSettingsTypeDef

```python
# Scte27SourceSettingsTypeDef definition

class Scte27SourceSettingsTypeDef(TypedDict):
    OcrLanguage: NotRequired[Scte27OcrLanguageType],  # (1)
    Pid: NotRequired[int],
```

1. See [:material-code-brackets: Scte27OcrLanguageType](./literals.md#scte27ocrlanguagetype) 
## CdiInputSpecificationTypeDef

```python
# CdiInputSpecificationTypeDef definition

class CdiInputSpecificationTypeDef(TypedDict):
    Resolution: NotRequired[CdiInputResolutionType],  # (1)
```

1. See [:material-code-brackets: CdiInputResolutionType](./literals.md#cdiinputresolutiontype) 
## ChannelEgressEndpointTypeDef

```python
# ChannelEgressEndpointTypeDef definition

class ChannelEgressEndpointTypeDef(TypedDict):
    SourceIp: NotRequired[str],
```

## InputSpecificationTypeDef

```python
# InputSpecificationTypeDef definition

class InputSpecificationTypeDef(TypedDict):
    Codec: NotRequired[InputCodecType],  # (1)
    MaximumBitrate: NotRequired[InputMaximumBitrateType],  # (2)
    Resolution: NotRequired[InputResolutionType],  # (3)
```

1. See [:material-code-brackets: InputCodecType](./literals.md#inputcodectype) 
2. See [:material-code-brackets: InputMaximumBitrateType](./literals.md#inputmaximumbitratetype) 
3. See [:material-code-brackets: InputResolutionType](./literals.md#inputresolutiontype) 
## MaintenanceStatusTypeDef

```python
# MaintenanceStatusTypeDef definition

class MaintenanceStatusTypeDef(TypedDict):
    MaintenanceDay: NotRequired[MaintenanceDayType],  # (1)
    MaintenanceDeadline: NotRequired[str],
    MaintenanceScheduledDate: NotRequired[str],
    MaintenanceStartTime: NotRequired[str],
```

1. See [:material-code-brackets: MaintenanceDayType](./literals.md#maintenancedaytype) 
## VpcOutputSettingsDescriptionTypeDef

```python
# VpcOutputSettingsDescriptionTypeDef definition

class VpcOutputSettingsDescriptionTypeDef(TypedDict):
    AvailabilityZones: NotRequired[List[str]],
    NetworkInterfaceIds: NotRequired[List[str]],
    SecurityGroupIds: NotRequired[List[str]],
    SubnetIds: NotRequired[List[str]],
```

## PipelineDetailTypeDef

```python
# PipelineDetailTypeDef definition

class PipelineDetailTypeDef(TypedDict):
    ActiveInputAttachmentName: NotRequired[str],
    ActiveInputSwitchActionName: NotRequired[str],
    ActiveMotionGraphicsActionName: NotRequired[str],
    ActiveMotionGraphicsUri: NotRequired[str],
    PipelineId: NotRequired[str],
```

## ClaimDeviceRequestRequestTypeDef

```python
# ClaimDeviceRequestRequestTypeDef definition

class ClaimDeviceRequestRequestTypeDef(TypedDict):
    Id: NotRequired[str],
```

## MaintenanceCreateSettingsTypeDef

```python
# MaintenanceCreateSettingsTypeDef definition

class MaintenanceCreateSettingsTypeDef(TypedDict):
    MaintenanceDay: NotRequired[MaintenanceDayType],  # (1)
    MaintenanceStartTime: NotRequired[str],
```

1. See [:material-code-brackets: MaintenanceDayType](./literals.md#maintenancedaytype) 
## VpcOutputSettingsTypeDef

```python
# VpcOutputSettingsTypeDef definition

class VpcOutputSettingsTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    PublicAddressAllocationIds: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
```

## InputDestinationRequestTypeDef

```python
# InputDestinationRequestTypeDef definition

class InputDestinationRequestTypeDef(TypedDict):
    StreamName: NotRequired[str],
```

## InputDeviceSettingsTypeDef

```python
# InputDeviceSettingsTypeDef definition

class InputDeviceSettingsTypeDef(TypedDict):
    Id: NotRequired[str],
```

## InputSourceRequestTypeDef

```python
# InputSourceRequestTypeDef definition

class InputSourceRequestTypeDef(TypedDict):
    PasswordParam: NotRequired[str],
    Url: NotRequired[str],
    Username: NotRequired[str],
```

## InputVpcRequestTypeDef

```python
# InputVpcRequestTypeDef definition

class InputVpcRequestTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
```

## MediaConnectFlowRequestTypeDef

```python
# MediaConnectFlowRequestTypeDef definition

class MediaConnectFlowRequestTypeDef(TypedDict):
    FlowArn: NotRequired[str],
```

## InputWhitelistRuleCidrTypeDef

```python
# InputWhitelistRuleCidrTypeDef definition

class InputWhitelistRuleCidrTypeDef(TypedDict):
    Cidr: NotRequired[str],
```

## MultiplexSettingsTypeDef

```python
# MultiplexSettingsTypeDef definition

class MultiplexSettingsTypeDef(TypedDict):
    TransportStreamBitrate: int,
    TransportStreamId: int,
    MaximumVideoBufferDelayMilliseconds: NotRequired[int],
    TransportStreamReservedBitrate: NotRequired[int],
```

## CreatePartnerInputRequestRequestTypeDef

```python
# CreatePartnerInputRequestRequestTypeDef definition

class CreatePartnerInputRequestRequestTypeDef(TypedDict):
    InputId: str,
    RequestId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## CreateTagsRequestRequestTypeDef

```python
# CreateTagsRequestRequestTypeDef definition

class CreateTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: NotRequired[Mapping[str, str]],
```

## DeleteChannelRequestRequestTypeDef

```python
# DeleteChannelRequestRequestTypeDef definition

class DeleteChannelRequestRequestTypeDef(TypedDict):
    ChannelId: str,
```

## DeleteInputRequestRequestTypeDef

```python
# DeleteInputRequestRequestTypeDef definition

class DeleteInputRequestRequestTypeDef(TypedDict):
    InputId: str,
```

## DeleteInputSecurityGroupRequestRequestTypeDef

```python
# DeleteInputSecurityGroupRequestRequestTypeDef definition

class DeleteInputSecurityGroupRequestRequestTypeDef(TypedDict):
    InputSecurityGroupId: str,
```

## DeleteMultiplexProgramRequestRequestTypeDef

```python
# DeleteMultiplexProgramRequestRequestTypeDef definition

class DeleteMultiplexProgramRequestRequestTypeDef(TypedDict):
    MultiplexId: str,
    ProgramName: str,
```

## MultiplexProgramPacketIdentifiersMapTypeDef

```python
# MultiplexProgramPacketIdentifiersMapTypeDef definition

class MultiplexProgramPacketIdentifiersMapTypeDef(TypedDict):
    AudioPids: NotRequired[List[int]],
    DvbSubPids: NotRequired[List[int]],
    DvbTeletextPid: NotRequired[int],
    EtvPlatformPid: NotRequired[int],
    EtvSignalPid: NotRequired[int],
    KlvDataPids: NotRequired[List[int]],
    PcrPid: NotRequired[int],
    PmtPid: NotRequired[int],
    PrivateMetadataPid: NotRequired[int],
    Scte27Pids: NotRequired[List[int]],
    Scte35Pid: NotRequired[int],
    TimedMetadataPid: NotRequired[int],
    VideoPid: NotRequired[int],
```

## MultiplexProgramPipelineDetailTypeDef

```python
# MultiplexProgramPipelineDetailTypeDef definition

class MultiplexProgramPipelineDetailTypeDef(TypedDict):
    ActiveChannelPipeline: NotRequired[str],
    PipelineId: NotRequired[str],
```

## DeleteMultiplexRequestRequestTypeDef

```python
# DeleteMultiplexRequestRequestTypeDef definition

class DeleteMultiplexRequestRequestTypeDef(TypedDict):
    MultiplexId: str,
```

## DeleteReservationRequestRequestTypeDef

```python
# DeleteReservationRequestRequestTypeDef definition

class DeleteReservationRequestRequestTypeDef(TypedDict):
    ReservationId: str,
```

## RenewalSettingsTypeDef

```python
# RenewalSettingsTypeDef definition

class RenewalSettingsTypeDef(TypedDict):
    AutomaticRenewal: NotRequired[ReservationAutomaticRenewalType],  # (1)
    RenewalCount: NotRequired[int],
```

1. See [:material-code-brackets: ReservationAutomaticRenewalType](./literals.md#reservationautomaticrenewaltype) 
## ReservationResourceSpecificationTypeDef

```python
# ReservationResourceSpecificationTypeDef definition

class ReservationResourceSpecificationTypeDef(TypedDict):
    ChannelClass: NotRequired[ChannelClassType],  # (1)
    Codec: NotRequired[ReservationCodecType],  # (2)
    MaximumBitrate: NotRequired[ReservationMaximumBitrateType],  # (3)
    MaximumFramerate: NotRequired[ReservationMaximumFramerateType],  # (4)
    Resolution: NotRequired[ReservationResolutionType],  # (5)
    ResourceType: NotRequired[ReservationResourceTypeType],  # (6)
    SpecialFeature: NotRequired[ReservationSpecialFeatureType],  # (7)
    VideoQuality: NotRequired[ReservationVideoQualityType],  # (8)
```

1. See [:material-code-brackets: ChannelClassType](./literals.md#channelclasstype) 
2. See [:material-code-brackets: ReservationCodecType](./literals.md#reservationcodectype) 
3. See [:material-code-brackets: ReservationMaximumBitrateType](./literals.md#reservationmaximumbitratetype) 
4. See [:material-code-brackets: ReservationMaximumFramerateType](./literals.md#reservationmaximumframeratetype) 
5. See [:material-code-brackets: ReservationResolutionType](./literals.md#reservationresolutiontype) 
6. See [:material-code-brackets: ReservationResourceTypeType](./literals.md#reservationresourcetypetype) 
7. See [:material-code-brackets: ReservationSpecialFeatureType](./literals.md#reservationspecialfeaturetype) 
8. See [:material-code-brackets: ReservationVideoQualityType](./literals.md#reservationvideoqualitytype) 
## DeleteScheduleRequestRequestTypeDef

```python
# DeleteScheduleRequestRequestTypeDef definition

class DeleteScheduleRequestRequestTypeDef(TypedDict):
    ChannelId: str,
```

## DeleteTagsRequestRequestTypeDef

```python
# DeleteTagsRequestRequestTypeDef definition

class DeleteTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeChannelRequestRequestTypeDef

```python
# DescribeChannelRequestRequestTypeDef definition

class DescribeChannelRequestRequestTypeDef(TypedDict):
    ChannelId: str,
```

## DescribeInputDeviceRequestRequestTypeDef

```python
# DescribeInputDeviceRequestRequestTypeDef definition

class DescribeInputDeviceRequestRequestTypeDef(TypedDict):
    InputDeviceId: str,
```

## InputDeviceHdSettingsTypeDef

```python
# InputDeviceHdSettingsTypeDef definition

class InputDeviceHdSettingsTypeDef(TypedDict):
    ActiveInput: NotRequired[InputDeviceActiveInputType],  # (1)
    ConfiguredInput: NotRequired[InputDeviceConfiguredInputType],  # (2)
    DeviceState: NotRequired[InputDeviceStateType],  # (3)
    Framerate: NotRequired[float],
    Height: NotRequired[int],
    MaxBitrate: NotRequired[int],
    ScanType: NotRequired[InputDeviceScanTypeType],  # (4)
    Width: NotRequired[int],
    LatencyMs: NotRequired[int],
```

1. See [:material-code-brackets: InputDeviceActiveInputType](./literals.md#inputdeviceactiveinputtype) 
2. See [:material-code-brackets: InputDeviceConfiguredInputType](./literals.md#inputdeviceconfiguredinputtype) 
3. See [:material-code-brackets: InputDeviceStateType](./literals.md#inputdevicestatetype) 
4. See [:material-code-brackets: InputDeviceScanTypeType](./literals.md#inputdevicescantypetype) 
## InputDeviceNetworkSettingsTypeDef

```python
# InputDeviceNetworkSettingsTypeDef definition

class InputDeviceNetworkSettingsTypeDef(TypedDict):
    DnsAddresses: NotRequired[List[str]],
    Gateway: NotRequired[str],
    IpAddress: NotRequired[str],
    IpScheme: NotRequired[InputDeviceIpSchemeType],  # (1)
    SubnetMask: NotRequired[str],
```

1. See [:material-code-brackets: InputDeviceIpSchemeType](./literals.md#inputdeviceipschemetype) 
## InputDeviceUhdSettingsTypeDef

```python
# InputDeviceUhdSettingsTypeDef definition

class InputDeviceUhdSettingsTypeDef(TypedDict):
    ActiveInput: NotRequired[InputDeviceActiveInputType],  # (1)
    ConfiguredInput: NotRequired[InputDeviceConfiguredInputType],  # (2)
    DeviceState: NotRequired[InputDeviceStateType],  # (3)
    Framerate: NotRequired[float],
    Height: NotRequired[int],
    MaxBitrate: NotRequired[int],
    ScanType: NotRequired[InputDeviceScanTypeType],  # (4)
    Width: NotRequired[int],
    LatencyMs: NotRequired[int],
```

1. See [:material-code-brackets: InputDeviceActiveInputType](./literals.md#inputdeviceactiveinputtype) 
2. See [:material-code-brackets: InputDeviceConfiguredInputType](./literals.md#inputdeviceconfiguredinputtype) 
3. See [:material-code-brackets: InputDeviceStateType](./literals.md#inputdevicestatetype) 
4. See [:material-code-brackets: InputDeviceScanTypeType](./literals.md#inputdevicescantypetype) 
## DescribeInputDeviceThumbnailRequestRequestTypeDef

```python
# DescribeInputDeviceThumbnailRequestRequestTypeDef definition

class DescribeInputDeviceThumbnailRequestRequestTypeDef(TypedDict):
    InputDeviceId: str,
    Accept: AcceptHeaderType,  # (1)
```

1. See [:material-code-brackets: AcceptHeaderType](./literals.md#acceptheadertype) 
## DescribeInputRequestRequestTypeDef

```python
# DescribeInputRequestRequestTypeDef definition

class DescribeInputRequestRequestTypeDef(TypedDict):
    InputId: str,
```

## InputSourceTypeDef

```python
# InputSourceTypeDef definition

class InputSourceTypeDef(TypedDict):
    PasswordParam: NotRequired[str],
    Url: NotRequired[str],
    Username: NotRequired[str],
```

## MediaConnectFlowTypeDef

```python
# MediaConnectFlowTypeDef definition

class MediaConnectFlowTypeDef(TypedDict):
    FlowArn: NotRequired[str],
```

## DescribeInputSecurityGroupRequestRequestTypeDef

```python
# DescribeInputSecurityGroupRequestRequestTypeDef definition

class DescribeInputSecurityGroupRequestRequestTypeDef(TypedDict):
    InputSecurityGroupId: str,
```

## InputWhitelistRuleTypeDef

```python
# InputWhitelistRuleTypeDef definition

class InputWhitelistRuleTypeDef(TypedDict):
    Cidr: NotRequired[str],
```

## DescribeMultiplexProgramRequestRequestTypeDef

```python
# DescribeMultiplexProgramRequestRequestTypeDef definition

class DescribeMultiplexProgramRequestRequestTypeDef(TypedDict):
    MultiplexId: str,
    ProgramName: str,
```

## DescribeMultiplexRequestRequestTypeDef

```python
# DescribeMultiplexRequestRequestTypeDef definition

class DescribeMultiplexRequestRequestTypeDef(TypedDict):
    MultiplexId: str,
```

## DescribeOfferingRequestRequestTypeDef

```python
# DescribeOfferingRequestRequestTypeDef definition

class DescribeOfferingRequestRequestTypeDef(TypedDict):
    OfferingId: str,
```

## DescribeReservationRequestRequestTypeDef

```python
# DescribeReservationRequestRequestTypeDef definition

class DescribeReservationRequestRequestTypeDef(TypedDict):
    ReservationId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeScheduleRequestRequestTypeDef

```python
# DescribeScheduleRequestRequestTypeDef definition

class DescribeScheduleRequestRequestTypeDef(TypedDict):
    ChannelId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeThumbnailsRequestRequestTypeDef

```python
# DescribeThumbnailsRequestRequestTypeDef definition

class DescribeThumbnailsRequestRequestTypeDef(TypedDict):
    ChannelId: str,
    PipelineId: str,
    ThumbnailType: str,
```

## DvbNitSettingsTypeDef

```python
# DvbNitSettingsTypeDef definition

class DvbNitSettingsTypeDef(TypedDict):
    NetworkId: int,
    NetworkName: str,
    RepInterval: NotRequired[int],
```

## DvbSdtSettingsTypeDef

```python
# DvbSdtSettingsTypeDef definition

class DvbSdtSettingsTypeDef(TypedDict):
    OutputSdt: NotRequired[DvbSdtOutputSdtType],  # (1)
    RepInterval: NotRequired[int],
    ServiceName: NotRequired[str],
    ServiceProviderName: NotRequired[str],
```

1. See [:material-code-brackets: DvbSdtOutputSdtType](./literals.md#dvbsdtoutputsdttype) 
## DvbTdtSettingsTypeDef

```python
# DvbTdtSettingsTypeDef definition

class DvbTdtSettingsTypeDef(TypedDict):
    RepInterval: NotRequired[int],
```

## FeatureActivationsTypeDef

```python
# FeatureActivationsTypeDef definition

class FeatureActivationsTypeDef(TypedDict):
    InputPrepareScheduleActions: NotRequired[FeatureActivationsInputPrepareScheduleActionsType],  # (1)
```

1. See [:material-code-brackets: FeatureActivationsInputPrepareScheduleActionsType](./literals.md#featureactivationsinputpreparescheduleactionstype) 
## NielsenConfigurationTypeDef

```python
# NielsenConfigurationTypeDef definition

class NielsenConfigurationTypeDef(TypedDict):
    DistributorId: NotRequired[str],
    NielsenPcmToId3Tagging: NotRequired[NielsenPcmToId3TaggingStateType],  # (1)
```

1. See [:material-code-brackets: NielsenPcmToId3TaggingStateType](./literals.md#nielsenpcmtoid3taggingstatetype) 
## ThumbnailConfigurationTypeDef

```python
# ThumbnailConfigurationTypeDef definition

class ThumbnailConfigurationTypeDef(TypedDict):
    State: ThumbnailStateType,  # (1)
```

1. See [:material-code-brackets: ThumbnailStateType](./literals.md#thumbnailstatetype) 
## TimecodeConfigTypeDef

```python
# TimecodeConfigTypeDef definition

class TimecodeConfigTypeDef(TypedDict):
    Source: TimecodeConfigSourceType,  # (1)
    SyncThreshold: NotRequired[int],
```

1. See [:material-code-brackets: TimecodeConfigSourceType](./literals.md#timecodeconfigsourcetype) 
## InputLossFailoverSettingsTypeDef

```python
# InputLossFailoverSettingsTypeDef definition

class InputLossFailoverSettingsTypeDef(TypedDict):
    InputLossThresholdMsec: NotRequired[int],
```

## VideoBlackFailoverSettingsTypeDef

```python
# VideoBlackFailoverSettingsTypeDef definition

class VideoBlackFailoverSettingsTypeDef(TypedDict):
    BlackDetectThreshold: NotRequired[float],
    VideoBlackThresholdMsec: NotRequired[int],
```

## FecOutputSettingsTypeDef

```python
# FecOutputSettingsTypeDef definition

class FecOutputSettingsTypeDef(TypedDict):
    ColumnDepth: NotRequired[int],
    IncludeFec: NotRequired[FecOutputIncludeFecType],  # (1)
    RowLength: NotRequired[int],
```

1. See [:material-code-brackets: FecOutputIncludeFecType](./literals.md#fecoutputincludefectype) 
## FixedModeScheduleActionStartSettingsTypeDef

```python
# FixedModeScheduleActionStartSettingsTypeDef definition

class FixedModeScheduleActionStartSettingsTypeDef(TypedDict):
    Time: str,
```

## Fmp4HlsSettingsTypeDef

```python
# Fmp4HlsSettingsTypeDef definition

class Fmp4HlsSettingsTypeDef(TypedDict):
    AudioRenditionSets: NotRequired[str],
    NielsenId3Behavior: NotRequired[Fmp4NielsenId3BehaviorType],  # (1)
    TimedMetadataBehavior: NotRequired[Fmp4TimedMetadataBehaviorType],  # (2)
```

1. See [:material-code-brackets: Fmp4NielsenId3BehaviorType](./literals.md#fmp4nielsenid3behaviortype) 
2. See [:material-code-brackets: Fmp4TimedMetadataBehaviorType](./literals.md#fmp4timedmetadatabehaviortype) 
## FollowModeScheduleActionStartSettingsTypeDef

```python
# FollowModeScheduleActionStartSettingsTypeDef definition

class FollowModeScheduleActionStartSettingsTypeDef(TypedDict):
    FollowPoint: FollowPointType,  # (1)
    ReferenceActionName: str,
```

1. See [:material-code-brackets: FollowPointType](./literals.md#followpointtype) 
## FrameCaptureS3SettingsTypeDef

```python
# FrameCaptureS3SettingsTypeDef definition

class FrameCaptureS3SettingsTypeDef(TypedDict):
    CannedAcl: NotRequired[S3CannedAclType],  # (1)
```

1. See [:material-code-brackets: S3CannedAclType](./literals.md#s3cannedacltype) 
## FrameCaptureOutputSettingsTypeDef

```python
# FrameCaptureOutputSettingsTypeDef definition

class FrameCaptureOutputSettingsTypeDef(TypedDict):
    NameModifier: NotRequired[str],
```

## TimecodeBurninSettingsTypeDef

```python
# TimecodeBurninSettingsTypeDef definition

class TimecodeBurninSettingsTypeDef(TypedDict):
    FontSize: TimecodeBurninFontSizeType,  # (1)
    Position: TimecodeBurninPositionType,  # (2)
    Prefix: NotRequired[str],
```

1. See [:material-code-brackets: TimecodeBurninFontSizeType](./literals.md#timecodeburninfontsizetype) 
2. See [:material-code-brackets: TimecodeBurninPositionType](./literals.md#timecodeburninpositiontype) 
## H264ColorSpaceSettingsTypeDef

```python
# H264ColorSpaceSettingsTypeDef definition

class H264ColorSpaceSettingsTypeDef(TypedDict):
    ColorSpacePassthroughSettings: NotRequired[Mapping[str, Any]],
    Rec601Settings: NotRequired[Mapping[str, Any]],
    Rec709Settings: NotRequired[Mapping[str, Any]],
```

## TemporalFilterSettingsTypeDef

```python
# TemporalFilterSettingsTypeDef definition

class TemporalFilterSettingsTypeDef(TypedDict):
    PostFilterSharpening: NotRequired[TemporalFilterPostFilterSharpeningType],  # (1)
    Strength: NotRequired[TemporalFilterStrengthType],  # (2)
```

1. See [:material-code-brackets: TemporalFilterPostFilterSharpeningType](./literals.md#temporalfilterpostfiltersharpeningtype) 
2. See [:material-code-brackets: TemporalFilterStrengthType](./literals.md#temporalfilterstrengthtype) 
## Hdr10SettingsTypeDef

```python
# Hdr10SettingsTypeDef definition

class Hdr10SettingsTypeDef(TypedDict):
    MaxCll: NotRequired[int],
    MaxFall: NotRequired[int],
```

## HlsAkamaiSettingsTypeDef

```python
# HlsAkamaiSettingsTypeDef definition

class HlsAkamaiSettingsTypeDef(TypedDict):
    ConnectionRetryInterval: NotRequired[int],
    FilecacheDuration: NotRequired[int],
    HttpTransferMode: NotRequired[HlsAkamaiHttpTransferModeType],  # (1)
    NumRetries: NotRequired[int],
    RestartDelay: NotRequired[int],
    Salt: NotRequired[str],
    Token: NotRequired[str],
```

1. See [:material-code-brackets: HlsAkamaiHttpTransferModeType](./literals.md#hlsakamaihttptransfermodetype) 
## HlsBasicPutSettingsTypeDef

```python
# HlsBasicPutSettingsTypeDef definition

class HlsBasicPutSettingsTypeDef(TypedDict):
    ConnectionRetryInterval: NotRequired[int],
    FilecacheDuration: NotRequired[int],
    NumRetries: NotRequired[int],
    RestartDelay: NotRequired[int],
```

## HlsMediaStoreSettingsTypeDef

```python
# HlsMediaStoreSettingsTypeDef definition

class HlsMediaStoreSettingsTypeDef(TypedDict):
    ConnectionRetryInterval: NotRequired[int],
    FilecacheDuration: NotRequired[int],
    MediaStoreStorageClass: NotRequired[HlsMediaStoreStorageClassType],  # (1)
    NumRetries: NotRequired[int],
    RestartDelay: NotRequired[int],
```

1. See [:material-code-brackets: HlsMediaStoreStorageClassType](./literals.md#hlsmediastorestorageclasstype) 
## HlsS3SettingsTypeDef

```python
# HlsS3SettingsTypeDef definition

class HlsS3SettingsTypeDef(TypedDict):
    CannedAcl: NotRequired[S3CannedAclType],  # (1)
```

1. See [:material-code-brackets: S3CannedAclType](./literals.md#s3cannedacltype) 
## HlsWebdavSettingsTypeDef

```python
# HlsWebdavSettingsTypeDef definition

class HlsWebdavSettingsTypeDef(TypedDict):
    ConnectionRetryInterval: NotRequired[int],
    FilecacheDuration: NotRequired[int],
    HttpTransferMode: NotRequired[HlsWebdavHttpTransferModeType],  # (1)
    NumRetries: NotRequired[int],
    RestartDelay: NotRequired[int],
```

1. See [:material-code-brackets: HlsWebdavHttpTransferModeType](./literals.md#hlswebdavhttptransfermodetype) 
## HlsId3SegmentTaggingScheduleActionSettingsTypeDef

```python
# HlsId3SegmentTaggingScheduleActionSettingsTypeDef definition

class HlsId3SegmentTaggingScheduleActionSettingsTypeDef(TypedDict):
    Tag: NotRequired[str],
    Id3: NotRequired[str],
```

## HlsInputSettingsTypeDef

```python
# HlsInputSettingsTypeDef definition

class HlsInputSettingsTypeDef(TypedDict):
    Bandwidth: NotRequired[int],
    BufferSegments: NotRequired[int],
    Retries: NotRequired[int],
    RetryInterval: NotRequired[int],
    Scte35Source: NotRequired[HlsScte35SourceTypeType],  # (1)
```

1. See [:material-code-brackets: HlsScte35SourceTypeType](./literals.md#hlsscte35sourcetypetype) 
## HlsTimedMetadataScheduleActionSettingsTypeDef

```python
# HlsTimedMetadataScheduleActionSettingsTypeDef definition

class HlsTimedMetadataScheduleActionSettingsTypeDef(TypedDict):
    Id3: str,
```

## StartTimecodeTypeDef

```python
# StartTimecodeTypeDef definition

class StartTimecodeTypeDef(TypedDict):
    Timecode: NotRequired[str],
```

## StopTimecodeTypeDef

```python
# StopTimecodeTypeDef definition

class StopTimecodeTypeDef(TypedDict):
    LastFrameClippingBehavior: NotRequired[LastFrameClippingBehaviorType],  # (1)
    Timecode: NotRequired[str],
```

1. See [:material-code-brackets: LastFrameClippingBehaviorType](./literals.md#lastframeclippingbehaviortype) 
## InputDestinationVpcTypeDef

```python
# InputDestinationVpcTypeDef definition

class InputDestinationVpcTypeDef(TypedDict):
    AvailabilityZone: NotRequired[str],
    NetworkInterfaceId: NotRequired[str],
```

## InputDeviceConfigurableSettingsTypeDef

```python
# InputDeviceConfigurableSettingsTypeDef definition

class InputDeviceConfigurableSettingsTypeDef(TypedDict):
    ConfiguredInput: NotRequired[InputDeviceConfiguredInputType],  # (1)
    MaxBitrate: NotRequired[int],
    LatencyMs: NotRequired[int],
```

1. See [:material-code-brackets: InputDeviceConfiguredInputType](./literals.md#inputdeviceconfiguredinputtype) 
## InputDeviceRequestTypeDef

```python
# InputDeviceRequestTypeDef definition

class InputDeviceRequestTypeDef(TypedDict):
    Id: NotRequired[str],
```

## ListChannelsRequestRequestTypeDef

```python
# ListChannelsRequestRequestTypeDef definition

class ListChannelsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListInputDeviceTransfersRequestRequestTypeDef

```python
# ListInputDeviceTransfersRequestRequestTypeDef definition

class ListInputDeviceTransfersRequestRequestTypeDef(TypedDict):
    TransferType: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## TransferringInputDeviceSummaryTypeDef

```python
# TransferringInputDeviceSummaryTypeDef definition

class TransferringInputDeviceSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Message: NotRequired[str],
    TargetCustomerId: NotRequired[str],
    TransferType: NotRequired[InputDeviceTransferTypeType],  # (1)
```

1. See [:material-code-brackets: InputDeviceTransferTypeType](./literals.md#inputdevicetransfertypetype) 
## ListInputDevicesRequestRequestTypeDef

```python
# ListInputDevicesRequestRequestTypeDef definition

class ListInputDevicesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListInputSecurityGroupsRequestRequestTypeDef

```python
# ListInputSecurityGroupsRequestRequestTypeDef definition

class ListInputSecurityGroupsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListInputsRequestRequestTypeDef

```python
# ListInputsRequestRequestTypeDef definition

class ListInputsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListMultiplexProgramsRequestRequestTypeDef

```python
# ListMultiplexProgramsRequestRequestTypeDef definition

class ListMultiplexProgramsRequestRequestTypeDef(TypedDict):
    MultiplexId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## MultiplexProgramSummaryTypeDef

```python
# MultiplexProgramSummaryTypeDef definition

class MultiplexProgramSummaryTypeDef(TypedDict):
    ChannelId: NotRequired[str],
    ProgramName: NotRequired[str],
```

## ListMultiplexesRequestRequestTypeDef

```python
# ListMultiplexesRequestRequestTypeDef definition

class ListMultiplexesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListOfferingsRequestRequestTypeDef

```python
# ListOfferingsRequestRequestTypeDef definition

class ListOfferingsRequestRequestTypeDef(TypedDict):
    ChannelClass: NotRequired[str],
    ChannelConfiguration: NotRequired[str],
    Codec: NotRequired[str],
    Duration: NotRequired[str],
    MaxResults: NotRequired[int],
    MaximumBitrate: NotRequired[str],
    MaximumFramerate: NotRequired[str],
    NextToken: NotRequired[str],
    Resolution: NotRequired[str],
    ResourceType: NotRequired[str],
    SpecialFeature: NotRequired[str],
    VideoQuality: NotRequired[str],
```

## ListReservationsRequestRequestTypeDef

```python
# ListReservationsRequestRequestTypeDef definition

class ListReservationsRequestRequestTypeDef(TypedDict):
    ChannelClass: NotRequired[str],
    Codec: NotRequired[str],
    MaxResults: NotRequired[int],
    MaximumBitrate: NotRequired[str],
    MaximumFramerate: NotRequired[str],
    NextToken: NotRequired[str],
    Resolution: NotRequired[str],
    ResourceType: NotRequired[str],
    SpecialFeature: NotRequired[str],
    VideoQuality: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## M3u8SettingsTypeDef

```python
# M3u8SettingsTypeDef definition

class M3u8SettingsTypeDef(TypedDict):
    AudioFramesPerPes: NotRequired[int],
    AudioPids: NotRequired[str],
    EcmPid: NotRequired[str],
    NielsenId3Behavior: NotRequired[M3u8NielsenId3BehaviorType],  # (1)
    PatInterval: NotRequired[int],
    PcrControl: NotRequired[M3u8PcrControlType],  # (2)
    PcrPeriod: NotRequired[int],
    PcrPid: NotRequired[str],
    PmtInterval: NotRequired[int],
    PmtPid: NotRequired[str],
    ProgramNum: NotRequired[int],
    Scte35Behavior: NotRequired[M3u8Scte35BehaviorType],  # (3)
    Scte35Pid: NotRequired[str],
    TimedMetadataBehavior: NotRequired[M3u8TimedMetadataBehaviorType],  # (4)
    TimedMetadataPid: NotRequired[str],
    TransportStreamId: NotRequired[int],
    VideoPid: NotRequired[str],
```

1. See [:material-code-brackets: M3u8NielsenId3BehaviorType](./literals.md#m3u8nielsenid3behaviortype) 
2. See [:material-code-brackets: M3u8PcrControlType](./literals.md#m3u8pcrcontroltype) 
3. See [:material-code-brackets: M3u8Scte35BehaviorType](./literals.md#m3u8scte35behaviortype) 
4. See [:material-code-brackets: M3u8TimedMetadataBehaviorType](./literals.md#m3u8timedmetadatabehaviortype) 
## MaintenanceUpdateSettingsTypeDef

```python
# MaintenanceUpdateSettingsTypeDef definition

class MaintenanceUpdateSettingsTypeDef(TypedDict):
    MaintenanceDay: NotRequired[MaintenanceDayType],  # (1)
    MaintenanceScheduledDate: NotRequired[str],
    MaintenanceStartTime: NotRequired[str],
```

1. See [:material-code-brackets: MaintenanceDayType](./literals.md#maintenancedaytype) 
## MediaPackageOutputDestinationSettingsTypeDef

```python
# MediaPackageOutputDestinationSettingsTypeDef definition

class MediaPackageOutputDestinationSettingsTypeDef(TypedDict):
    ChannelId: NotRequired[str],
```

## MotionGraphicsActivateScheduleActionSettingsTypeDef

```python
# MotionGraphicsActivateScheduleActionSettingsTypeDef definition

class MotionGraphicsActivateScheduleActionSettingsTypeDef(TypedDict):
    Duration: NotRequired[int],
    PasswordParam: NotRequired[str],
    Url: NotRequired[str],
    Username: NotRequired[str],
```

## MotionGraphicsSettingsTypeDef

```python
# MotionGraphicsSettingsTypeDef definition

class MotionGraphicsSettingsTypeDef(TypedDict):
    HtmlMotionGraphicsSettings: NotRequired[Mapping[str, Any]],
```

## MsSmoothOutputSettingsTypeDef

```python
# MsSmoothOutputSettingsTypeDef definition

class MsSmoothOutputSettingsTypeDef(TypedDict):
    H265PackagingType: NotRequired[MsSmoothH265PackagingTypeType],  # (1)
    NameModifier: NotRequired[str],
```

1. See [:material-code-brackets: MsSmoothH265PackagingTypeType](./literals.md#mssmoothh265packagingtypetype) 
## MultiplexMediaConnectOutputDestinationSettingsTypeDef

```python
# MultiplexMediaConnectOutputDestinationSettingsTypeDef definition

class MultiplexMediaConnectOutputDestinationSettingsTypeDef(TypedDict):
    EntitlementArn: NotRequired[str],
```

## MultiplexProgramChannelDestinationSettingsTypeDef

```python
# MultiplexProgramChannelDestinationSettingsTypeDef definition

class MultiplexProgramChannelDestinationSettingsTypeDef(TypedDict):
    MultiplexId: NotRequired[str],
    ProgramName: NotRequired[str],
```

## MultiplexProgramServiceDescriptorTypeDef

```python
# MultiplexProgramServiceDescriptorTypeDef definition

class MultiplexProgramServiceDescriptorTypeDef(TypedDict):
    ProviderName: str,
    ServiceName: str,
```

## MultiplexSettingsSummaryTypeDef

```python
# MultiplexSettingsSummaryTypeDef definition

class MultiplexSettingsSummaryTypeDef(TypedDict):
    TransportStreamBitrate: NotRequired[int],
```

## MultiplexStatmuxVideoSettingsTypeDef

```python
# MultiplexStatmuxVideoSettingsTypeDef definition

class MultiplexStatmuxVideoSettingsTypeDef(TypedDict):
    MaximumBitrate: NotRequired[int],
    MinimumBitrate: NotRequired[int],
    Priority: NotRequired[int],
```

## NielsenCBETTypeDef

```python
# NielsenCBETTypeDef definition

class NielsenCBETTypeDef(TypedDict):
    CbetCheckDigitString: str,
    CbetStepaside: NielsenWatermarksCbetStepasideType,  # (1)
    Csid: str,
```

1. See [:material-code-brackets: NielsenWatermarksCbetStepasideType](./literals.md#nielsenwatermarkscbetstepasidetype) 
## NielsenNaesIiNwTypeDef

```python
# NielsenNaesIiNwTypeDef definition

class NielsenNaesIiNwTypeDef(TypedDict):
    CheckDigitString: str,
    Sid: float,
    Timezone: NotRequired[NielsenWatermarkTimezonesType],  # (1)
```

1. See [:material-code-brackets: NielsenWatermarkTimezonesType](./literals.md#nielsenwatermarktimezonestype) 
## OutputDestinationSettingsTypeDef

```python
# OutputDestinationSettingsTypeDef definition

class OutputDestinationSettingsTypeDef(TypedDict):
    PasswordParam: NotRequired[str],
    StreamName: NotRequired[str],
    Url: NotRequired[str],
    Username: NotRequired[str],
```

## RtmpGroupSettingsTypeDef

```python
# RtmpGroupSettingsTypeDef definition

class RtmpGroupSettingsTypeDef(TypedDict):
    AdMarkers: NotRequired[Sequence[RtmpAdMarkersType]],  # (1)
    AuthenticationScheme: NotRequired[AuthenticationSchemeType],  # (2)
    CacheFullBehavior: NotRequired[RtmpCacheFullBehaviorType],  # (3)
    CacheLength: NotRequired[int],
    CaptionData: NotRequired[RtmpCaptionDataType],  # (4)
    InputLossAction: NotRequired[InputLossActionForRtmpOutType],  # (5)
    RestartDelay: NotRequired[int],
```

1. See [:material-code-brackets: RtmpAdMarkersType](./literals.md#rtmpadmarkerstype) 
2. See [:material-code-brackets: AuthenticationSchemeType](./literals.md#authenticationschemetype) 
3. See [:material-code-brackets: RtmpCacheFullBehaviorType](./literals.md#rtmpcachefullbehaviortype) 
4. See [:material-code-brackets: RtmpCaptionDataType](./literals.md#rtmpcaptiondatatype) 
5. See [:material-code-brackets: InputLossActionForRtmpOutType](./literals.md#inputlossactionforrtmpouttype) 
## UdpGroupSettingsTypeDef

```python
# UdpGroupSettingsTypeDef definition

class UdpGroupSettingsTypeDef(TypedDict):
    InputLossAction: NotRequired[InputLossActionForUdpOutType],  # (1)
    TimedMetadataId3Frame: NotRequired[UdpTimedMetadataId3FrameType],  # (2)
    TimedMetadataId3Period: NotRequired[int],
```

1. See [:material-code-brackets: InputLossActionForUdpOutType](./literals.md#inputlossactionforudpouttype) 
2. See [:material-code-brackets: UdpTimedMetadataId3FrameType](./literals.md#udptimedmetadataid3frametype) 
## PipelinePauseStateSettingsTypeDef

```python
# PipelinePauseStateSettingsTypeDef definition

class PipelinePauseStateSettingsTypeDef(TypedDict):
    PipelineId: PipelineIdType,  # (1)
```

1. See [:material-code-brackets: PipelineIdType](./literals.md#pipelineidtype) 
## RebootInputDeviceRequestRequestTypeDef

```python
# RebootInputDeviceRequestRequestTypeDef definition

class RebootInputDeviceRequestRequestTypeDef(TypedDict):
    InputDeviceId: str,
    Force: NotRequired[RebootInputDeviceForceType],  # (1)
```

1. See [:material-code-brackets: RebootInputDeviceForceType](./literals.md#rebootinputdeviceforcetype) 
## RejectInputDeviceTransferRequestRequestTypeDef

```python
# RejectInputDeviceTransferRequestRequestTypeDef definition

class RejectInputDeviceTransferRequestRequestTypeDef(TypedDict):
    InputDeviceId: str,
```

## Scte35InputScheduleActionSettingsTypeDef

```python
# Scte35InputScheduleActionSettingsTypeDef definition

class Scte35InputScheduleActionSettingsTypeDef(TypedDict):
    Mode: Scte35InputModeType,  # (1)
    InputAttachmentNameReference: NotRequired[str],
```

1. See [:material-code-brackets: Scte35InputModeType](./literals.md#scte35inputmodetype) 
## Scte35ReturnToNetworkScheduleActionSettingsTypeDef

```python
# Scte35ReturnToNetworkScheduleActionSettingsTypeDef definition

class Scte35ReturnToNetworkScheduleActionSettingsTypeDef(TypedDict):
    SpliceEventId: int,
```

## Scte35SpliceInsertScheduleActionSettingsTypeDef

```python
# Scte35SpliceInsertScheduleActionSettingsTypeDef definition

class Scte35SpliceInsertScheduleActionSettingsTypeDef(TypedDict):
    SpliceEventId: int,
    Duration: NotRequired[int],
```

## StaticImageDeactivateScheduleActionSettingsTypeDef

```python
# StaticImageDeactivateScheduleActionSettingsTypeDef definition

class StaticImageDeactivateScheduleActionSettingsTypeDef(TypedDict):
    FadeOut: NotRequired[int],
    Layer: NotRequired[int],
```

## Scte35DeliveryRestrictionsTypeDef

```python
# Scte35DeliveryRestrictionsTypeDef definition

class Scte35DeliveryRestrictionsTypeDef(TypedDict):
    ArchiveAllowedFlag: Scte35ArchiveAllowedFlagType,  # (1)
    DeviceRestrictions: Scte35DeviceRestrictionsType,  # (2)
    NoRegionalBlackoutFlag: Scte35NoRegionalBlackoutFlagType,  # (3)
    WebDeliveryAllowedFlag: Scte35WebDeliveryAllowedFlagType,  # (4)
```

1. See [:material-code-brackets: Scte35ArchiveAllowedFlagType](./literals.md#scte35archiveallowedflagtype) 
2. See [:material-code-brackets: Scte35DeviceRestrictionsType](./literals.md#scte35devicerestrictionstype) 
3. See [:material-code-brackets: Scte35NoRegionalBlackoutFlagType](./literals.md#scte35noregionalblackoutflagtype) 
4. See [:material-code-brackets: Scte35WebDeliveryAllowedFlagType](./literals.md#scte35webdeliveryallowedflagtype) 
## StartChannelRequestRequestTypeDef

```python
# StartChannelRequestRequestTypeDef definition

class StartChannelRequestRequestTypeDef(TypedDict):
    ChannelId: str,
```

## StartInputDeviceMaintenanceWindowRequestRequestTypeDef

```python
# StartInputDeviceMaintenanceWindowRequestRequestTypeDef definition

class StartInputDeviceMaintenanceWindowRequestRequestTypeDef(TypedDict):
    InputDeviceId: str,
```

## StartMultiplexRequestRequestTypeDef

```python
# StartMultiplexRequestRequestTypeDef definition

class StartMultiplexRequestRequestTypeDef(TypedDict):
    MultiplexId: str,
```

## StopChannelRequestRequestTypeDef

```python
# StopChannelRequestRequestTypeDef definition

class StopChannelRequestRequestTypeDef(TypedDict):
    ChannelId: str,
```

## StopMultiplexRequestRequestTypeDef

```python
# StopMultiplexRequestRequestTypeDef definition

class StopMultiplexRequestRequestTypeDef(TypedDict):
    MultiplexId: str,
```

## ThumbnailTypeDef

```python
# ThumbnailTypeDef definition

class ThumbnailTypeDef(TypedDict):
    Body: NotRequired[str],
    ContentType: NotRequired[str],
    ThumbnailType: NotRequired[ThumbnailTypeType],  # (1)
    TimeStamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ThumbnailTypeType](./literals.md#thumbnailtypetype) 
## TransferInputDeviceRequestRequestTypeDef

```python
# TransferInputDeviceRequestRequestTypeDef definition

class TransferInputDeviceRequestRequestTypeDef(TypedDict):
    InputDeviceId: str,
    TargetCustomerId: NotRequired[str],
    TargetRegion: NotRequired[str],
    TransferMessage: NotRequired[str],
```

## VideoSelectorPidTypeDef

```python
# VideoSelectorPidTypeDef definition

class VideoSelectorPidTypeDef(TypedDict):
    Pid: NotRequired[int],
```

## VideoSelectorProgramIdTypeDef

```python
# VideoSelectorProgramIdTypeDef definition

class VideoSelectorProgramIdTypeDef(TypedDict):
    ProgramId: NotRequired[int],
```

## UpdateAccountConfigurationRequestRequestTypeDef

```python
# UpdateAccountConfigurationRequestRequestTypeDef definition

class UpdateAccountConfigurationRequestRequestTypeDef(TypedDict):
    AccountConfiguration: NotRequired[AccountConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AccountConfigurationTypeDef](./type_defs.md#accountconfigurationtypedef) 
## ArchiveCdnSettingsTypeDef

```python
# ArchiveCdnSettingsTypeDef definition

class ArchiveCdnSettingsTypeDef(TypedDict):
    ArchiveS3Settings: NotRequired[ArchiveS3SettingsTypeDef],  # (1)
```

1. See [:material-code-braces: ArchiveS3SettingsTypeDef](./type_defs.md#archives3settingstypedef) 
## MediaPackageGroupSettingsTypeDef

```python
# MediaPackageGroupSettingsTypeDef definition

class MediaPackageGroupSettingsTypeDef(TypedDict):
    Destination: OutputLocationRefTypeDef,  # (1)
```

1. See [:material-code-braces: OutputLocationRefTypeDef](./type_defs.md#outputlocationreftypedef) 
## MsSmoothGroupSettingsTypeDef

```python
# MsSmoothGroupSettingsTypeDef definition

class MsSmoothGroupSettingsTypeDef(TypedDict):
    Destination: OutputLocationRefTypeDef,  # (3)
    AcquisitionPointId: NotRequired[str],
    AudioOnlyTimecodeControl: NotRequired[SmoothGroupAudioOnlyTimecodeControlType],  # (1)
    CertificateMode: NotRequired[SmoothGroupCertificateModeType],  # (2)
    ConnectionRetryInterval: NotRequired[int],
    EventId: NotRequired[str],
    EventIdMode: NotRequired[SmoothGroupEventIdModeType],  # (4)
    EventStopBehavior: NotRequired[SmoothGroupEventStopBehaviorType],  # (5)
    FilecacheDuration: NotRequired[int],
    FragmentLength: NotRequired[int],
    InputLossAction: NotRequired[InputLossActionForMsSmoothOutType],  # (6)
    NumRetries: NotRequired[int],
    RestartDelay: NotRequired[int],
    SegmentationMode: NotRequired[SmoothGroupSegmentationModeType],  # (7)
    SendDelayMs: NotRequired[int],
    SparseTrackType: NotRequired[SmoothGroupSparseTrackTypeType],  # (8)
    StreamManifestBehavior: NotRequired[SmoothGroupStreamManifestBehaviorType],  # (9)
    TimestampOffset: NotRequired[str],
    TimestampOffsetMode: NotRequired[SmoothGroupTimestampOffsetModeType],  # (10)
```

1. See [:material-code-brackets: SmoothGroupAudioOnlyTimecodeControlType](./literals.md#smoothgroupaudioonlytimecodecontroltype) 
2. See [:material-code-brackets: SmoothGroupCertificateModeType](./literals.md#smoothgroupcertificatemodetype) 
3. See [:material-code-braces: OutputLocationRefTypeDef](./type_defs.md#outputlocationreftypedef) 
4. See [:material-code-brackets: SmoothGroupEventIdModeType](./literals.md#smoothgroupeventidmodetype) 
5. See [:material-code-brackets: SmoothGroupEventStopBehaviorType](./literals.md#smoothgroupeventstopbehaviortype) 
6. See [:material-code-brackets: InputLossActionForMsSmoothOutType](./literals.md#inputlossactionformssmoothouttype) 
7. See [:material-code-brackets: SmoothGroupSegmentationModeType](./literals.md#smoothgroupsegmentationmodetype) 
8. See [:material-code-brackets: SmoothGroupSparseTrackTypeType](./literals.md#smoothgroupsparsetracktypetype) 
9. See [:material-code-brackets: SmoothGroupStreamManifestBehaviorType](./literals.md#smoothgroupstreammanifestbehaviortype) 
10. See [:material-code-brackets: SmoothGroupTimestampOffsetModeType](./literals.md#smoothgrouptimestampoffsetmodetype) 
## MultiplexOutputSettingsTypeDef

```python
# MultiplexOutputSettingsTypeDef definition

class MultiplexOutputSettingsTypeDef(TypedDict):
    Destination: OutputLocationRefTypeDef,  # (1)
```

1. See [:material-code-braces: OutputLocationRefTypeDef](./type_defs.md#outputlocationreftypedef) 
## RtmpOutputSettingsTypeDef

```python
# RtmpOutputSettingsTypeDef definition

class RtmpOutputSettingsTypeDef(TypedDict):
    Destination: OutputLocationRefTypeDef,  # (2)
    CertificateMode: NotRequired[RtmpOutputCertificateModeType],  # (1)
    ConnectionRetryInterval: NotRequired[int],
    NumRetries: NotRequired[int],
```

1. See [:material-code-brackets: RtmpOutputCertificateModeType](./literals.md#rtmpoutputcertificatemodetype) 
2. See [:material-code-braces: OutputLocationRefTypeDef](./type_defs.md#outputlocationreftypedef) 
## AudioChannelMappingTypeDef

```python
# AudioChannelMappingTypeDef definition

class AudioChannelMappingTypeDef(TypedDict):
    InputChannelLevels: Sequence[InputChannelLevelTypeDef],  # (1)
    OutputChannel: int,
```

1. See [:material-code-braces: InputChannelLevelTypeDef](./type_defs.md#inputchannelleveltypedef) 
## AudioCodecSettingsTypeDef

```python
# AudioCodecSettingsTypeDef definition

class AudioCodecSettingsTypeDef(TypedDict):
    AacSettings: NotRequired[AacSettingsTypeDef],  # (1)
    Ac3Settings: NotRequired[Ac3SettingsTypeDef],  # (2)
    Eac3AtmosSettings: NotRequired[Eac3AtmosSettingsTypeDef],  # (3)
    Eac3Settings: NotRequired[Eac3SettingsTypeDef],  # (4)
    Mp2Settings: NotRequired[Mp2SettingsTypeDef],  # (5)
    PassThroughSettings: NotRequired[Mapping[str, Any]],
    WavSettings: NotRequired[WavSettingsTypeDef],  # (6)
```

1. See [:material-code-braces: AacSettingsTypeDef](./type_defs.md#aacsettingstypedef) 
2. See [:material-code-braces: Ac3SettingsTypeDef](./type_defs.md#ac3settingstypedef) 
3. See [:material-code-braces: Eac3AtmosSettingsTypeDef](./type_defs.md#eac3atmossettingstypedef) 
4. See [:material-code-braces: Eac3SettingsTypeDef](./type_defs.md#eac3settingstypedef) 
5. See [:material-code-braces: Mp2SettingsTypeDef](./type_defs.md#mp2settingstypedef) 
6. See [:material-code-braces: WavSettingsTypeDef](./type_defs.md#wavsettingstypedef) 
## AudioOnlyHlsSettingsTypeDef

```python
# AudioOnlyHlsSettingsTypeDef definition

class AudioOnlyHlsSettingsTypeDef(TypedDict):
    AudioGroupId: NotRequired[str],
    AudioOnlyImage: NotRequired[InputLocationTypeDef],  # (1)
    AudioTrackType: NotRequired[AudioOnlyHlsTrackTypeType],  # (2)
    SegmentType: NotRequired[AudioOnlyHlsSegmentTypeType],  # (3)
```

1. See [:material-code-braces: InputLocationTypeDef](./type_defs.md#inputlocationtypedef) 
2. See [:material-code-brackets: AudioOnlyHlsTrackTypeType](./literals.md#audioonlyhlstracktypetype) 
3. See [:material-code-brackets: AudioOnlyHlsSegmentTypeType](./literals.md#audioonlyhlssegmenttypetype) 
## AvailBlankingTypeDef

```python
# AvailBlankingTypeDef definition

class AvailBlankingTypeDef(TypedDict):
    AvailBlankingImage: NotRequired[InputLocationTypeDef],  # (1)
    State: NotRequired[AvailBlankingStateType],  # (2)
```

1. See [:material-code-braces: InputLocationTypeDef](./type_defs.md#inputlocationtypedef) 
2. See [:material-code-brackets: AvailBlankingStateType](./literals.md#availblankingstatetype) 
## BlackoutSlateTypeDef

```python
# BlackoutSlateTypeDef definition

class BlackoutSlateTypeDef(TypedDict):
    BlackoutSlateImage: NotRequired[InputLocationTypeDef],  # (1)
    NetworkEndBlackout: NotRequired[BlackoutSlateNetworkEndBlackoutType],  # (2)
    NetworkEndBlackoutImage: NotRequired[InputLocationTypeDef],  # (1)
    NetworkId: NotRequired[str],
    State: NotRequired[BlackoutSlateStateType],  # (4)
```

1. See [:material-code-braces: InputLocationTypeDef](./type_defs.md#inputlocationtypedef) 
2. See [:material-code-brackets: BlackoutSlateNetworkEndBlackoutType](./literals.md#blackoutslatenetworkendblackouttype) 
3. See [:material-code-braces: InputLocationTypeDef](./type_defs.md#inputlocationtypedef) 
4. See [:material-code-brackets: BlackoutSlateStateType](./literals.md#blackoutslatestatetype) 
## BurnInDestinationSettingsTypeDef

```python
# BurnInDestinationSettingsTypeDef definition

class BurnInDestinationSettingsTypeDef(TypedDict):
    Alignment: NotRequired[BurnInAlignmentType],  # (1)
    BackgroundColor: NotRequired[BurnInBackgroundColorType],  # (2)
    BackgroundOpacity: NotRequired[int],
    Font: NotRequired[InputLocationTypeDef],  # (3)
    FontColor: NotRequired[BurnInFontColorType],  # (4)
    FontOpacity: NotRequired[int],
    FontResolution: NotRequired[int],
    FontSize: NotRequired[str],
    OutlineColor: NotRequired[BurnInOutlineColorType],  # (5)
    OutlineSize: NotRequired[int],
    ShadowColor: NotRequired[BurnInShadowColorType],  # (6)
    ShadowOpacity: NotRequired[int],
    ShadowXOffset: NotRequired[int],
    ShadowYOffset: NotRequired[int],
    TeletextGridControl: NotRequired[BurnInTeletextGridControlType],  # (7)
    XPosition: NotRequired[int],
    YPosition: NotRequired[int],
```

1. See [:material-code-brackets: BurnInAlignmentType](./literals.md#burninalignmenttype) 
2. See [:material-code-brackets: BurnInBackgroundColorType](./literals.md#burninbackgroundcolortype) 
3. See [:material-code-braces: InputLocationTypeDef](./type_defs.md#inputlocationtypedef) 
4. See [:material-code-brackets: BurnInFontColorType](./literals.md#burninfontcolortype) 
5. See [:material-code-brackets: BurnInOutlineColorType](./literals.md#burninoutlinecolortype) 
6. See [:material-code-brackets: BurnInShadowColorType](./literals.md#burninshadowcolortype) 
7. See [:material-code-brackets: BurnInTeletextGridControlType](./literals.md#burninteletextgridcontroltype) 
## DvbSubDestinationSettingsTypeDef

```python
# DvbSubDestinationSettingsTypeDef definition

class DvbSubDestinationSettingsTypeDef(TypedDict):
    Alignment: NotRequired[DvbSubDestinationAlignmentType],  # (1)
    BackgroundColor: NotRequired[DvbSubDestinationBackgroundColorType],  # (2)
    BackgroundOpacity: NotRequired[int],
    Font: NotRequired[InputLocationTypeDef],  # (3)
    FontColor: NotRequired[DvbSubDestinationFontColorType],  # (4)
    FontOpacity: NotRequired[int],
    FontResolution: NotRequired[int],
    FontSize: NotRequired[str],
    OutlineColor: NotRequired[DvbSubDestinationOutlineColorType],  # (5)
    OutlineSize: NotRequired[int],
    ShadowColor: NotRequired[DvbSubDestinationShadowColorType],  # (6)
    ShadowOpacity: NotRequired[int],
    ShadowXOffset: NotRequired[int],
    ShadowYOffset: NotRequired[int],
    TeletextGridControl: NotRequired[DvbSubDestinationTeletextGridControlType],  # (7)
    XPosition: NotRequired[int],
    YPosition: NotRequired[int],
```

1. See [:material-code-brackets: DvbSubDestinationAlignmentType](./literals.md#dvbsubdestinationalignmenttype) 
2. See [:material-code-brackets: DvbSubDestinationBackgroundColorType](./literals.md#dvbsubdestinationbackgroundcolortype) 
3. See [:material-code-braces: InputLocationTypeDef](./type_defs.md#inputlocationtypedef) 
4. See [:material-code-brackets: DvbSubDestinationFontColorType](./literals.md#dvbsubdestinationfontcolortype) 
5. See [:material-code-brackets: DvbSubDestinationOutlineColorType](./literals.md#dvbsubdestinationoutlinecolortype) 
6. See [:material-code-brackets: DvbSubDestinationShadowColorType](./literals.md#dvbsubdestinationshadowcolortype) 
7. See [:material-code-brackets: DvbSubDestinationTeletextGridControlType](./literals.md#dvbsubdestinationteletextgridcontroltype) 
## InputLossBehaviorTypeDef

```python
# InputLossBehaviorTypeDef definition

class InputLossBehaviorTypeDef(TypedDict):
    BlackFrameMsec: NotRequired[int],
    InputLossImageColor: NotRequired[str],
    InputLossImageSlate: NotRequired[InputLocationTypeDef],  # (1)
    InputLossImageType: NotRequired[InputLossImageTypeType],  # (2)
    RepeatFrameMsec: NotRequired[int],
```

1. See [:material-code-braces: InputLocationTypeDef](./type_defs.md#inputlocationtypedef) 
2. See [:material-code-brackets: InputLossImageTypeType](./literals.md#inputlossimagetypetype) 
## StaticImageActivateScheduleActionSettingsTypeDef

```python
# StaticImageActivateScheduleActionSettingsTypeDef definition

class StaticImageActivateScheduleActionSettingsTypeDef(TypedDict):
    Image: InputLocationTypeDef,  # (1)
    Duration: NotRequired[int],
    FadeIn: NotRequired[int],
    FadeOut: NotRequired[int],
    Height: NotRequired[int],
    ImageX: NotRequired[int],
    ImageY: NotRequired[int],
    Layer: NotRequired[int],
    Opacity: NotRequired[int],
    Width: NotRequired[int],
```

1. See [:material-code-braces: InputLocationTypeDef](./type_defs.md#inputlocationtypedef) 
## StaticKeySettingsTypeDef

```python
# StaticKeySettingsTypeDef definition

class StaticKeySettingsTypeDef(TypedDict):
    StaticKeyValue: str,
    KeyProviderServer: NotRequired[InputLocationTypeDef],  # (1)
```

1. See [:material-code-braces: InputLocationTypeDef](./type_defs.md#inputlocationtypedef) 
## AudioTrackSelectionTypeDef

```python
# AudioTrackSelectionTypeDef definition

class AudioTrackSelectionTypeDef(TypedDict):
    Tracks: Sequence[AudioTrackTypeDef],  # (1)
    DolbyEDecode: NotRequired[AudioDolbyEDecodeTypeDef],  # (2)
```

1. See [:material-code-braces: AudioTrackTypeDef](./type_defs.md#audiotracktypedef) 
2. See [:material-code-braces: AudioDolbyEDecodeTypeDef](./type_defs.md#audiodolbyedecodetypedef) 
## AvailSettingsTypeDef

```python
# AvailSettingsTypeDef definition

class AvailSettingsTypeDef(TypedDict):
    Esam: NotRequired[EsamTypeDef],  # (1)
    Scte35SpliceInsert: NotRequired[Scte35SpliceInsertTypeDef],  # (2)
    Scte35TimeSignalApos: NotRequired[Scte35TimeSignalAposTypeDef],  # (3)
```

1. See [:material-code-braces: EsamTypeDef](./type_defs.md#esamtypedef) 
2. See [:material-code-braces: Scte35SpliceInsertTypeDef](./type_defs.md#scte35spliceinserttypedef) 
3. See [:material-code-braces: Scte35TimeSignalAposTypeDef](./type_defs.md#scte35timesignalapostypedef) 
## BatchDeleteResponseTypeDef

```python
# BatchDeleteResponseTypeDef definition

class BatchDeleteResponseTypeDef(TypedDict):
    Failed: List[BatchFailedResultModelTypeDef],  # (1)
    Successful: List[BatchSuccessfulResultModelTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchFailedResultModelTypeDef](./type_defs.md#batchfailedresultmodeltypedef) 
2. See [:material-code-braces: BatchSuccessfulResultModelTypeDef](./type_defs.md#batchsuccessfulresultmodeltypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchStartResponseTypeDef

```python
# BatchStartResponseTypeDef definition

class BatchStartResponseTypeDef(TypedDict):
    Failed: List[BatchFailedResultModelTypeDef],  # (1)
    Successful: List[BatchSuccessfulResultModelTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchFailedResultModelTypeDef](./type_defs.md#batchfailedresultmodeltypedef) 
2. See [:material-code-braces: BatchSuccessfulResultModelTypeDef](./type_defs.md#batchsuccessfulresultmodeltypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchStopResponseTypeDef

```python
# BatchStopResponseTypeDef definition

class BatchStopResponseTypeDef(TypedDict):
    Failed: List[BatchFailedResultModelTypeDef],  # (1)
    Successful: List[BatchSuccessfulResultModelTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchFailedResultModelTypeDef](./type_defs.md#batchfailedresultmodeltypedef) 
2. See [:material-code-braces: BatchSuccessfulResultModelTypeDef](./type_defs.md#batchsuccessfulresultmodeltypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountConfigurationResponseTypeDef

```python
# DescribeAccountConfigurationResponseTypeDef definition

class DescribeAccountConfigurationResponseTypeDef(TypedDict):
    AccountConfiguration: AccountConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountConfigurationTypeDef](./type_defs.md#accountconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInputDeviceThumbnailResponseTypeDef

```python
# DescribeInputDeviceThumbnailResponseTypeDef definition

class DescribeInputDeviceThumbnailResponseTypeDef(TypedDict):
    Body: StreamingBody,
    ContentType: ContentTypeType,  # (1)
    ContentLength: int,
    ETag: str,
    LastModified: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ContentTypeType](./literals.md#contenttypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountConfigurationResponseTypeDef

```python
# UpdateAccountConfigurationResponseTypeDef definition

class UpdateAccountConfigurationResponseTypeDef(TypedDict):
    AccountConfiguration: AccountConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountConfigurationTypeDef](./type_defs.md#accountconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TeletextSourceSettingsTypeDef

```python
# TeletextSourceSettingsTypeDef definition

class TeletextSourceSettingsTypeDef(TypedDict):
    OutputRectangle: NotRequired[CaptionRectangleTypeDef],  # (1)
    PageNumber: NotRequired[str],
```

1. See [:material-code-braces: CaptionRectangleTypeDef](./type_defs.md#captionrectangletypedef) 
## CreateInputRequestRequestTypeDef

```python
# CreateInputRequestRequestTypeDef definition

class CreateInputRequestRequestTypeDef(TypedDict):
    Destinations: NotRequired[Sequence[InputDestinationRequestTypeDef]],  # (1)
    InputDevices: NotRequired[Sequence[InputDeviceSettingsTypeDef]],  # (2)
    InputSecurityGroups: NotRequired[Sequence[str]],
    MediaConnectFlows: NotRequired[Sequence[MediaConnectFlowRequestTypeDef]],  # (3)
    Name: NotRequired[str],
    RequestId: NotRequired[str],
    RoleArn: NotRequired[str],
    Sources: NotRequired[Sequence[InputSourceRequestTypeDef]],  # (4)
    Tags: NotRequired[Mapping[str, str]],
    Type: NotRequired[InputTypeType],  # (5)
    Vpc: NotRequired[InputVpcRequestTypeDef],  # (6)
```

1. See [:material-code-braces: InputDestinationRequestTypeDef](./type_defs.md#inputdestinationrequesttypedef) 
2. See [:material-code-braces: InputDeviceSettingsTypeDef](./type_defs.md#inputdevicesettingstypedef) 
3. See [:material-code-braces: MediaConnectFlowRequestTypeDef](./type_defs.md#mediaconnectflowrequesttypedef) 
4. See [:material-code-braces: InputSourceRequestTypeDef](./type_defs.md#inputsourcerequesttypedef) 
5. See [:material-code-brackets: InputTypeType](./literals.md#inputtypetype) 
6. See [:material-code-braces: InputVpcRequestTypeDef](./type_defs.md#inputvpcrequesttypedef) 
## CreateInputSecurityGroupRequestRequestTypeDef

```python
# CreateInputSecurityGroupRequestRequestTypeDef definition

class CreateInputSecurityGroupRequestRequestTypeDef(TypedDict):
    Tags: NotRequired[Mapping[str, str]],
    WhitelistRules: NotRequired[Sequence[InputWhitelistRuleCidrTypeDef]],  # (1)
```

1. See [:material-code-braces: InputWhitelistRuleCidrTypeDef](./type_defs.md#inputwhitelistrulecidrtypedef) 
## UpdateInputSecurityGroupRequestRequestTypeDef

```python
# UpdateInputSecurityGroupRequestRequestTypeDef definition

class UpdateInputSecurityGroupRequestRequestTypeDef(TypedDict):
    InputSecurityGroupId: str,
    Tags: NotRequired[Mapping[str, str]],
    WhitelistRules: NotRequired[Sequence[InputWhitelistRuleCidrTypeDef]],  # (1)
```

1. See [:material-code-braces: InputWhitelistRuleCidrTypeDef](./type_defs.md#inputwhitelistrulecidrtypedef) 
## CreateMultiplexRequestRequestTypeDef

```python
# CreateMultiplexRequestRequestTypeDef definition

class CreateMultiplexRequestRequestTypeDef(TypedDict):
    AvailabilityZones: Sequence[str],
    MultiplexSettings: MultiplexSettingsTypeDef,  # (1)
    Name: str,
    RequestId: str,
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MultiplexSettingsTypeDef](./type_defs.md#multiplexsettingstypedef) 
## UpdateMultiplexRequestRequestTypeDef

```python
# UpdateMultiplexRequestRequestTypeDef definition

class UpdateMultiplexRequestRequestTypeDef(TypedDict):
    MultiplexId: str,
    MultiplexSettings: NotRequired[MultiplexSettingsTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: MultiplexSettingsTypeDef](./type_defs.md#multiplexsettingstypedef) 
## PurchaseOfferingRequestRequestTypeDef

```python
# PurchaseOfferingRequestRequestTypeDef definition

class PurchaseOfferingRequestRequestTypeDef(TypedDict):
    Count: int,
    OfferingId: str,
    Name: NotRequired[str],
    RenewalSettings: NotRequired[RenewalSettingsTypeDef],  # (1)
    RequestId: NotRequired[str],
    Start: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: RenewalSettingsTypeDef](./type_defs.md#renewalsettingstypedef) 
## UpdateReservationRequestRequestTypeDef

```python
# UpdateReservationRequestRequestTypeDef definition

class UpdateReservationRequestRequestTypeDef(TypedDict):
    ReservationId: str,
    Name: NotRequired[str],
    RenewalSettings: NotRequired[RenewalSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: RenewalSettingsTypeDef](./type_defs.md#renewalsettingstypedef) 
## DeleteReservationResponseTypeDef

```python
# DeleteReservationResponseTypeDef definition

class DeleteReservationResponseTypeDef(TypedDict):
    Arn: str,
    Count: int,
    CurrencyCode: str,
    Duration: int,
    DurationUnits: OfferingDurationUnitsType,  # (1)
    End: str,
    FixedPrice: float,
    Name: str,
    OfferingDescription: str,
    OfferingId: str,
    OfferingType: OfferingTypeType,  # (2)
    Region: str,
    RenewalSettings: RenewalSettingsTypeDef,  # (3)
    ReservationId: str,
    ResourceSpecification: ReservationResourceSpecificationTypeDef,  # (4)
    Start: str,
    State: ReservationStateType,  # (5)
    Tags: Dict[str, str],
    UsagePrice: float,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: OfferingDurationUnitsType](./literals.md#offeringdurationunitstype) 
2. See [:material-code-brackets: OfferingTypeType](./literals.md#offeringtypetype) 
3. See [:material-code-braces: RenewalSettingsTypeDef](./type_defs.md#renewalsettingstypedef) 
4. See [:material-code-braces: ReservationResourceSpecificationTypeDef](./type_defs.md#reservationresourcespecificationtypedef) 
5. See [:material-code-brackets: ReservationStateType](./literals.md#reservationstatetype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOfferingResponseTypeDef

```python
# DescribeOfferingResponseTypeDef definition

class DescribeOfferingResponseTypeDef(TypedDict):
    Arn: str,
    CurrencyCode: str,
    Duration: int,
    DurationUnits: OfferingDurationUnitsType,  # (1)
    FixedPrice: float,
    OfferingDescription: str,
    OfferingId: str,
    OfferingType: OfferingTypeType,  # (2)
    Region: str,
    ResourceSpecification: ReservationResourceSpecificationTypeDef,  # (3)
    UsagePrice: float,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: OfferingDurationUnitsType](./literals.md#offeringdurationunitstype) 
2. See [:material-code-brackets: OfferingTypeType](./literals.md#offeringtypetype) 
3. See [:material-code-braces: ReservationResourceSpecificationTypeDef](./type_defs.md#reservationresourcespecificationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReservationResponseTypeDef

```python
# DescribeReservationResponseTypeDef definition

class DescribeReservationResponseTypeDef(TypedDict):
    Arn: str,
    Count: int,
    CurrencyCode: str,
    Duration: int,
    DurationUnits: OfferingDurationUnitsType,  # (1)
    End: str,
    FixedPrice: float,
    Name: str,
    OfferingDescription: str,
    OfferingId: str,
    OfferingType: OfferingTypeType,  # (2)
    Region: str,
    RenewalSettings: RenewalSettingsTypeDef,  # (3)
    ReservationId: str,
    ResourceSpecification: ReservationResourceSpecificationTypeDef,  # (4)
    Start: str,
    State: ReservationStateType,  # (5)
    Tags: Dict[str, str],
    UsagePrice: float,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: OfferingDurationUnitsType](./literals.md#offeringdurationunitstype) 
2. See [:material-code-brackets: OfferingTypeType](./literals.md#offeringtypetype) 
3. See [:material-code-braces: RenewalSettingsTypeDef](./type_defs.md#renewalsettingstypedef) 
4. See [:material-code-braces: ReservationResourceSpecificationTypeDef](./type_defs.md#reservationresourcespecificationtypedef) 
5. See [:material-code-brackets: ReservationStateType](./literals.md#reservationstatetype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OfferingTypeDef

```python
# OfferingTypeDef definition

class OfferingTypeDef(TypedDict):
    Arn: NotRequired[str],
    CurrencyCode: NotRequired[str],
    Duration: NotRequired[int],
    DurationUnits: NotRequired[OfferingDurationUnitsType],  # (1)
    FixedPrice: NotRequired[float],
    OfferingDescription: NotRequired[str],
    OfferingId: NotRequired[str],
    OfferingType: NotRequired[OfferingTypeType],  # (2)
    Region: NotRequired[str],
    ResourceSpecification: NotRequired[ReservationResourceSpecificationTypeDef],  # (3)
    UsagePrice: NotRequired[float],
```

1. See [:material-code-brackets: OfferingDurationUnitsType](./literals.md#offeringdurationunitstype) 
2. See [:material-code-brackets: OfferingTypeType](./literals.md#offeringtypetype) 
3. See [:material-code-braces: ReservationResourceSpecificationTypeDef](./type_defs.md#reservationresourcespecificationtypedef) 
## ReservationTypeDef

```python
# ReservationTypeDef definition

class ReservationTypeDef(TypedDict):
    Arn: NotRequired[str],
    Count: NotRequired[int],
    CurrencyCode: NotRequired[str],
    Duration: NotRequired[int],
    DurationUnits: NotRequired[OfferingDurationUnitsType],  # (1)
    End: NotRequired[str],
    FixedPrice: NotRequired[float],
    Name: NotRequired[str],
    OfferingDescription: NotRequired[str],
    OfferingId: NotRequired[str],
    OfferingType: NotRequired[OfferingTypeType],  # (2)
    Region: NotRequired[str],
    RenewalSettings: NotRequired[RenewalSettingsTypeDef],  # (3)
    ReservationId: NotRequired[str],
    ResourceSpecification: NotRequired[ReservationResourceSpecificationTypeDef],  # (4)
    Start: NotRequired[str],
    State: NotRequired[ReservationStateType],  # (5)
    Tags: NotRequired[Dict[str, str]],
    UsagePrice: NotRequired[float],
```

1. See [:material-code-brackets: OfferingDurationUnitsType](./literals.md#offeringdurationunitstype) 
2. See [:material-code-brackets: OfferingTypeType](./literals.md#offeringtypetype) 
3. See [:material-code-braces: RenewalSettingsTypeDef](./type_defs.md#renewalsettingstypedef) 
4. See [:material-code-braces: ReservationResourceSpecificationTypeDef](./type_defs.md#reservationresourcespecificationtypedef) 
5. See [:material-code-brackets: ReservationStateType](./literals.md#reservationstatetype) 
## DescribeChannelRequestChannelCreatedWaitTypeDef

```python
# DescribeChannelRequestChannelCreatedWaitTypeDef definition

class DescribeChannelRequestChannelCreatedWaitTypeDef(TypedDict):
    ChannelId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeChannelRequestChannelDeletedWaitTypeDef

```python
# DescribeChannelRequestChannelDeletedWaitTypeDef definition

class DescribeChannelRequestChannelDeletedWaitTypeDef(TypedDict):
    ChannelId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeChannelRequestChannelRunningWaitTypeDef

```python
# DescribeChannelRequestChannelRunningWaitTypeDef definition

class DescribeChannelRequestChannelRunningWaitTypeDef(TypedDict):
    ChannelId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeChannelRequestChannelStoppedWaitTypeDef

```python
# DescribeChannelRequestChannelStoppedWaitTypeDef definition

class DescribeChannelRequestChannelStoppedWaitTypeDef(TypedDict):
    ChannelId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInputRequestInputAttachedWaitTypeDef

```python
# DescribeInputRequestInputAttachedWaitTypeDef definition

class DescribeInputRequestInputAttachedWaitTypeDef(TypedDict):
    InputId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInputRequestInputDeletedWaitTypeDef

```python
# DescribeInputRequestInputDeletedWaitTypeDef definition

class DescribeInputRequestInputDeletedWaitTypeDef(TypedDict):
    InputId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInputRequestInputDetachedWaitTypeDef

```python
# DescribeInputRequestInputDetachedWaitTypeDef definition

class DescribeInputRequestInputDetachedWaitTypeDef(TypedDict):
    InputId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeMultiplexRequestMultiplexCreatedWaitTypeDef

```python
# DescribeMultiplexRequestMultiplexCreatedWaitTypeDef definition

class DescribeMultiplexRequestMultiplexCreatedWaitTypeDef(TypedDict):
    MultiplexId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeMultiplexRequestMultiplexDeletedWaitTypeDef

```python
# DescribeMultiplexRequestMultiplexDeletedWaitTypeDef definition

class DescribeMultiplexRequestMultiplexDeletedWaitTypeDef(TypedDict):
    MultiplexId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeMultiplexRequestMultiplexRunningWaitTypeDef

```python
# DescribeMultiplexRequestMultiplexRunningWaitTypeDef definition

class DescribeMultiplexRequestMultiplexRunningWaitTypeDef(TypedDict):
    MultiplexId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeMultiplexRequestMultiplexStoppedWaitTypeDef

```python
# DescribeMultiplexRequestMultiplexStoppedWaitTypeDef definition

class DescribeMultiplexRequestMultiplexStoppedWaitTypeDef(TypedDict):
    MultiplexId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeInputDeviceResponseTypeDef

```python
# DescribeInputDeviceResponseTypeDef definition

class DescribeInputDeviceResponseTypeDef(TypedDict):
    Arn: str,
    ConnectionState: InputDeviceConnectionStateType,  # (1)
    DeviceSettingsSyncState: DeviceSettingsSyncStateType,  # (2)
    DeviceUpdateStatus: DeviceUpdateStatusType,  # (3)
    HdDeviceSettings: InputDeviceHdSettingsTypeDef,  # (4)
    Id: str,
    MacAddress: str,
    Name: str,
    NetworkSettings: InputDeviceNetworkSettingsTypeDef,  # (5)
    SerialNumber: str,
    Type: InputDeviceTypeType,  # (6)
    UhdDeviceSettings: InputDeviceUhdSettingsTypeDef,  # (7)
    Tags: Dict[str, str],
    AvailabilityZone: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: InputDeviceConnectionStateType](./literals.md#inputdeviceconnectionstatetype) 
2. See [:material-code-brackets: DeviceSettingsSyncStateType](./literals.md#devicesettingssyncstatetype) 
3. See [:material-code-brackets: DeviceUpdateStatusType](./literals.md#deviceupdatestatustype) 
4. See [:material-code-braces: InputDeviceHdSettingsTypeDef](./type_defs.md#inputdevicehdsettingstypedef) 
5. See [:material-code-braces: InputDeviceNetworkSettingsTypeDef](./type_defs.md#inputdevicenetworksettingstypedef) 
6. See [:material-code-brackets: InputDeviceTypeType](./literals.md#inputdevicetypetype) 
7. See [:material-code-braces: InputDeviceUhdSettingsTypeDef](./type_defs.md#inputdeviceuhdsettingstypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InputDeviceSummaryTypeDef

```python
# InputDeviceSummaryTypeDef definition

class InputDeviceSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    ConnectionState: NotRequired[InputDeviceConnectionStateType],  # (1)
    DeviceSettingsSyncState: NotRequired[DeviceSettingsSyncStateType],  # (2)
    DeviceUpdateStatus: NotRequired[DeviceUpdateStatusType],  # (3)
    HdDeviceSettings: NotRequired[InputDeviceHdSettingsTypeDef],  # (4)
    Id: NotRequired[str],
    MacAddress: NotRequired[str],
    Name: NotRequired[str],
    NetworkSettings: NotRequired[InputDeviceNetworkSettingsTypeDef],  # (5)
    SerialNumber: NotRequired[str],
    Type: NotRequired[InputDeviceTypeType],  # (6)
    UhdDeviceSettings: NotRequired[InputDeviceUhdSettingsTypeDef],  # (7)
    Tags: NotRequired[Dict[str, str]],
    AvailabilityZone: NotRequired[str],
```

1. See [:material-code-brackets: InputDeviceConnectionStateType](./literals.md#inputdeviceconnectionstatetype) 
2. See [:material-code-brackets: DeviceSettingsSyncStateType](./literals.md#devicesettingssyncstatetype) 
3. See [:material-code-brackets: DeviceUpdateStatusType](./literals.md#deviceupdatestatustype) 
4. See [:material-code-braces: InputDeviceHdSettingsTypeDef](./type_defs.md#inputdevicehdsettingstypedef) 
5. See [:material-code-braces: InputDeviceNetworkSettingsTypeDef](./type_defs.md#inputdevicenetworksettingstypedef) 
6. See [:material-code-brackets: InputDeviceTypeType](./literals.md#inputdevicetypetype) 
7. See [:material-code-braces: InputDeviceUhdSettingsTypeDef](./type_defs.md#inputdeviceuhdsettingstypedef) 
## UpdateInputDeviceResponseTypeDef

```python
# UpdateInputDeviceResponseTypeDef definition

class UpdateInputDeviceResponseTypeDef(TypedDict):
    Arn: str,
    ConnectionState: InputDeviceConnectionStateType,  # (1)
    DeviceSettingsSyncState: DeviceSettingsSyncStateType,  # (2)
    DeviceUpdateStatus: DeviceUpdateStatusType,  # (3)
    HdDeviceSettings: InputDeviceHdSettingsTypeDef,  # (4)
    Id: str,
    MacAddress: str,
    Name: str,
    NetworkSettings: InputDeviceNetworkSettingsTypeDef,  # (5)
    SerialNumber: str,
    Type: InputDeviceTypeType,  # (6)
    UhdDeviceSettings: InputDeviceUhdSettingsTypeDef,  # (7)
    Tags: Dict[str, str],
    AvailabilityZone: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: InputDeviceConnectionStateType](./literals.md#inputdeviceconnectionstatetype) 
2. See [:material-code-brackets: DeviceSettingsSyncStateType](./literals.md#devicesettingssyncstatetype) 
3. See [:material-code-brackets: DeviceUpdateStatusType](./literals.md#deviceupdatestatustype) 
4. See [:material-code-braces: InputDeviceHdSettingsTypeDef](./type_defs.md#inputdevicehdsettingstypedef) 
5. See [:material-code-braces: InputDeviceNetworkSettingsTypeDef](./type_defs.md#inputdevicenetworksettingstypedef) 
6. See [:material-code-brackets: InputDeviceTypeType](./literals.md#inputdevicetypetype) 
7. See [:material-code-braces: InputDeviceUhdSettingsTypeDef](./type_defs.md#inputdeviceuhdsettingstypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInputSecurityGroupResponseTypeDef

```python
# DescribeInputSecurityGroupResponseTypeDef definition

class DescribeInputSecurityGroupResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Inputs: List[str],
    State: InputSecurityGroupStateType,  # (1)
    Tags: Dict[str, str],
    WhitelistRules: List[InputWhitelistRuleTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: InputSecurityGroupStateType](./literals.md#inputsecuritygroupstatetype) 
2. See [:material-code-braces: InputWhitelistRuleTypeDef](./type_defs.md#inputwhitelistruletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InputSecurityGroupTypeDef

```python
# InputSecurityGroupTypeDef definition

class InputSecurityGroupTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Inputs: NotRequired[List[str]],
    State: NotRequired[InputSecurityGroupStateType],  # (1)
    Tags: NotRequired[Dict[str, str]],
    WhitelistRules: NotRequired[List[InputWhitelistRuleTypeDef]],  # (2)
```

1. See [:material-code-brackets: InputSecurityGroupStateType](./literals.md#inputsecuritygroupstatetype) 
2. See [:material-code-braces: InputWhitelistRuleTypeDef](./type_defs.md#inputwhitelistruletypedef) 
## DescribeScheduleRequestDescribeSchedulePaginateTypeDef

```python
# DescribeScheduleRequestDescribeSchedulePaginateTypeDef definition

class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(TypedDict):
    ChannelId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListChannelsRequestListChannelsPaginateTypeDef

```python
# ListChannelsRequestListChannelsPaginateTypeDef definition

class ListChannelsRequestListChannelsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef

```python
# ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef definition

class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(TypedDict):
    TransferType: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInputDevicesRequestListInputDevicesPaginateTypeDef

```python
# ListInputDevicesRequestListInputDevicesPaginateTypeDef definition

class ListInputDevicesRequestListInputDevicesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef

```python
# ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef definition

class ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInputsRequestListInputsPaginateTypeDef

```python
# ListInputsRequestListInputsPaginateTypeDef definition

class ListInputsRequestListInputsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef

```python
# ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef definition

class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(TypedDict):
    MultiplexId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMultiplexesRequestListMultiplexesPaginateTypeDef

```python
# ListMultiplexesRequestListMultiplexesPaginateTypeDef definition

class ListMultiplexesRequestListMultiplexesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOfferingsRequestListOfferingsPaginateTypeDef

```python
# ListOfferingsRequestListOfferingsPaginateTypeDef definition

class ListOfferingsRequestListOfferingsPaginateTypeDef(TypedDict):
    ChannelClass: NotRequired[str],
    ChannelConfiguration: NotRequired[str],
    Codec: NotRequired[str],
    Duration: NotRequired[str],
    MaximumBitrate: NotRequired[str],
    MaximumFramerate: NotRequired[str],
    Resolution: NotRequired[str],
    ResourceType: NotRequired[str],
    SpecialFeature: NotRequired[str],
    VideoQuality: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReservationsRequestListReservationsPaginateTypeDef

```python
# ListReservationsRequestListReservationsPaginateTypeDef definition

class ListReservationsRequestListReservationsPaginateTypeDef(TypedDict):
    ChannelClass: NotRequired[str],
    Codec: NotRequired[str],
    MaximumBitrate: NotRequired[str],
    MaximumFramerate: NotRequired[str],
    Resolution: NotRequired[str],
    ResourceType: NotRequired[str],
    SpecialFeature: NotRequired[str],
    VideoQuality: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## M2tsSettingsTypeDef

```python
# M2tsSettingsTypeDef definition

class M2tsSettingsTypeDef(TypedDict):
    AbsentInputAudioBehavior: NotRequired[M2tsAbsentInputAudioBehaviorType],  # (1)
    Arib: NotRequired[M2tsAribType],  # (2)
    AribCaptionsPid: NotRequired[str],
    AribCaptionsPidControl: NotRequired[M2tsAribCaptionsPidControlType],  # (3)
    AudioBufferModel: NotRequired[M2tsAudioBufferModelType],  # (4)
    AudioFramesPerPes: NotRequired[int],
    AudioPids: NotRequired[str],
    AudioStreamType: NotRequired[M2tsAudioStreamTypeType],  # (5)
    Bitrate: NotRequired[int],
    BufferModel: NotRequired[M2tsBufferModelType],  # (6)
    CcDescriptor: NotRequired[M2tsCcDescriptorType],  # (7)
    DvbNitSettings: NotRequired[DvbNitSettingsTypeDef],  # (8)
    DvbSdtSettings: NotRequired[DvbSdtSettingsTypeDef],  # (9)
    DvbSubPids: NotRequired[str],
    DvbTdtSettings: NotRequired[DvbTdtSettingsTypeDef],  # (10)
    DvbTeletextPid: NotRequired[str],
    Ebif: NotRequired[M2tsEbifControlType],  # (11)
    EbpAudioInterval: NotRequired[M2tsAudioIntervalType],  # (12)
    EbpLookaheadMs: NotRequired[int],
    EbpPlacement: NotRequired[M2tsEbpPlacementType],  # (13)
    EcmPid: NotRequired[str],
    EsRateInPes: NotRequired[M2tsEsRateInPesType],  # (14)
    EtvPlatformPid: NotRequired[str],
    EtvSignalPid: NotRequired[str],
    FragmentTime: NotRequired[float],
    Klv: NotRequired[M2tsKlvType],  # (15)
    KlvDataPids: NotRequired[str],
    NielsenId3Behavior: NotRequired[M2tsNielsenId3BehaviorType],  # (16)
    NullPacketBitrate: NotRequired[float],
    PatInterval: NotRequired[int],
    PcrControl: NotRequired[M2tsPcrControlType],  # (17)
    PcrPeriod: NotRequired[int],
    PcrPid: NotRequired[str],
    PmtInterval: NotRequired[int],
    PmtPid: NotRequired[str],
    ProgramNum: NotRequired[int],
    RateMode: NotRequired[M2tsRateModeType],  # (18)
    Scte27Pids: NotRequired[str],
    Scte35Control: NotRequired[M2tsScte35ControlType],  # (19)
    Scte35Pid: NotRequired[str],
    SegmentationMarkers: NotRequired[M2tsSegmentationMarkersType],  # (20)
    SegmentationStyle: NotRequired[M2tsSegmentationStyleType],  # (21)
    SegmentationTime: NotRequired[float],
    TimedMetadataBehavior: NotRequired[M2tsTimedMetadataBehaviorType],  # (22)
    TimedMetadataPid: NotRequired[str],
    TransportStreamId: NotRequired[int],
    VideoPid: NotRequired[str],
    Scte35PrerollPullupMilliseconds: NotRequired[float],
```

1. See [:material-code-brackets: M2tsAbsentInputAudioBehaviorType](./literals.md#m2tsabsentinputaudiobehaviortype) 
2. See [:material-code-brackets: M2tsAribType](./literals.md#m2tsaribtype) 
3. See [:material-code-brackets: M2tsAribCaptionsPidControlType](./literals.md#m2tsaribcaptionspidcontroltype) 
4. See [:material-code-brackets: M2tsAudioBufferModelType](./literals.md#m2tsaudiobuffermodeltype) 
5. See [:material-code-brackets: M2tsAudioStreamTypeType](./literals.md#m2tsaudiostreamtypetype) 
6. See [:material-code-brackets: M2tsBufferModelType](./literals.md#m2tsbuffermodeltype) 
7. See [:material-code-brackets: M2tsCcDescriptorType](./literals.md#m2tsccdescriptortype) 
8. See [:material-code-braces: DvbNitSettingsTypeDef](./type_defs.md#dvbnitsettingstypedef) 
9. See [:material-code-braces: DvbSdtSettingsTypeDef](./type_defs.md#dvbsdtsettingstypedef) 
10. See [:material-code-braces: DvbTdtSettingsTypeDef](./type_defs.md#dvbtdtsettingstypedef) 
11. See [:material-code-brackets: M2tsEbifControlType](./literals.md#m2tsebifcontroltype) 
12. See [:material-code-brackets: M2tsAudioIntervalType](./literals.md#m2tsaudiointervaltype) 
13. See [:material-code-brackets: M2tsEbpPlacementType](./literals.md#m2tsebpplacementtype) 
14. See [:material-code-brackets: M2tsEsRateInPesType](./literals.md#m2tsesrateinpestype) 
15. See [:material-code-brackets: M2tsKlvType](./literals.md#m2tsklvtype) 
16. See [:material-code-brackets: M2tsNielsenId3BehaviorType](./literals.md#m2tsnielsenid3behaviortype) 
17. See [:material-code-brackets: M2tsPcrControlType](./literals.md#m2tspcrcontroltype) 
18. See [:material-code-brackets: M2tsRateModeType](./literals.md#m2tsratemodetype) 
19. See [:material-code-brackets: M2tsScte35ControlType](./literals.md#m2tsscte35controltype) 
20. See [:material-code-brackets: M2tsSegmentationMarkersType](./literals.md#m2tssegmentationmarkerstype) 
21. See [:material-code-brackets: M2tsSegmentationStyleType](./literals.md#m2tssegmentationstyletype) 
22. See [:material-code-brackets: M2tsTimedMetadataBehaviorType](./literals.md#m2tstimedmetadatabehaviortype) 
## FailoverConditionSettingsTypeDef

```python
# FailoverConditionSettingsTypeDef definition

class FailoverConditionSettingsTypeDef(TypedDict):
    AudioSilenceSettings: NotRequired[AudioSilenceFailoverSettingsTypeDef],  # (1)
    InputLossSettings: NotRequired[InputLossFailoverSettingsTypeDef],  # (2)
    VideoBlackSettings: NotRequired[VideoBlackFailoverSettingsTypeDef],  # (3)
```

1. See [:material-code-braces: AudioSilenceFailoverSettingsTypeDef](./type_defs.md#audiosilencefailoversettingstypedef) 
2. See [:material-code-braces: InputLossFailoverSettingsTypeDef](./type_defs.md#inputlossfailoversettingstypedef) 
3. See [:material-code-braces: VideoBlackFailoverSettingsTypeDef](./type_defs.md#videoblackfailoversettingstypedef) 
## ScheduleActionStartSettingsTypeDef

```python
# ScheduleActionStartSettingsTypeDef definition

class ScheduleActionStartSettingsTypeDef(TypedDict):
    FixedModeScheduleActionStartSettings: NotRequired[FixedModeScheduleActionStartSettingsTypeDef],  # (1)
    FollowModeScheduleActionStartSettings: NotRequired[FollowModeScheduleActionStartSettingsTypeDef],  # (2)
    ImmediateModeScheduleActionStartSettings: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: FixedModeScheduleActionStartSettingsTypeDef](./type_defs.md#fixedmodescheduleactionstartsettingstypedef) 
2. See [:material-code-braces: FollowModeScheduleActionStartSettingsTypeDef](./type_defs.md#followmodescheduleactionstartsettingstypedef) 
## FrameCaptureCdnSettingsTypeDef

```python
# FrameCaptureCdnSettingsTypeDef definition

class FrameCaptureCdnSettingsTypeDef(TypedDict):
    FrameCaptureS3Settings: NotRequired[FrameCaptureS3SettingsTypeDef],  # (1)
```

1. See [:material-code-braces: FrameCaptureS3SettingsTypeDef](./type_defs.md#framecaptures3settingstypedef) 
## FrameCaptureSettingsTypeDef

```python
# FrameCaptureSettingsTypeDef definition

class FrameCaptureSettingsTypeDef(TypedDict):
    CaptureInterval: NotRequired[int],
    CaptureIntervalUnits: NotRequired[FrameCaptureIntervalUnitType],  # (1)
    TimecodeBurninSettings: NotRequired[TimecodeBurninSettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: FrameCaptureIntervalUnitType](./literals.md#framecaptureintervalunittype) 
2. See [:material-code-braces: TimecodeBurninSettingsTypeDef](./type_defs.md#timecodeburninsettingstypedef) 
## H264FilterSettingsTypeDef

```python
# H264FilterSettingsTypeDef definition

class H264FilterSettingsTypeDef(TypedDict):
    TemporalFilterSettings: NotRequired[TemporalFilterSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: TemporalFilterSettingsTypeDef](./type_defs.md#temporalfiltersettingstypedef) 
## H265FilterSettingsTypeDef

```python
# H265FilterSettingsTypeDef definition

class H265FilterSettingsTypeDef(TypedDict):
    TemporalFilterSettings: NotRequired[TemporalFilterSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: TemporalFilterSettingsTypeDef](./type_defs.md#temporalfiltersettingstypedef) 
## Mpeg2FilterSettingsTypeDef

```python
# Mpeg2FilterSettingsTypeDef definition

class Mpeg2FilterSettingsTypeDef(TypedDict):
    TemporalFilterSettings: NotRequired[TemporalFilterSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: TemporalFilterSettingsTypeDef](./type_defs.md#temporalfiltersettingstypedef) 
## H265ColorSpaceSettingsTypeDef

```python
# H265ColorSpaceSettingsTypeDef definition

class H265ColorSpaceSettingsTypeDef(TypedDict):
    ColorSpacePassthroughSettings: NotRequired[Mapping[str, Any]],
    DolbyVision81Settings: NotRequired[Mapping[str, Any]],
    Hdr10Settings: NotRequired[Hdr10SettingsTypeDef],  # (1)
    Rec601Settings: NotRequired[Mapping[str, Any]],
    Rec709Settings: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: Hdr10SettingsTypeDef](./type_defs.md#hdr10settingstypedef) 
## VideoSelectorColorSpaceSettingsTypeDef

```python
# VideoSelectorColorSpaceSettingsTypeDef definition

class VideoSelectorColorSpaceSettingsTypeDef(TypedDict):
    Hdr10Settings: NotRequired[Hdr10SettingsTypeDef],  # (1)
```

1. See [:material-code-braces: Hdr10SettingsTypeDef](./type_defs.md#hdr10settingstypedef) 
## HlsCdnSettingsTypeDef

```python
# HlsCdnSettingsTypeDef definition

class HlsCdnSettingsTypeDef(TypedDict):
    HlsAkamaiSettings: NotRequired[HlsAkamaiSettingsTypeDef],  # (1)
    HlsBasicPutSettings: NotRequired[HlsBasicPutSettingsTypeDef],  # (2)
    HlsMediaStoreSettings: NotRequired[HlsMediaStoreSettingsTypeDef],  # (3)
    HlsS3Settings: NotRequired[HlsS3SettingsTypeDef],  # (4)
    HlsWebdavSettings: NotRequired[HlsWebdavSettingsTypeDef],  # (5)
```

1. See [:material-code-braces: HlsAkamaiSettingsTypeDef](./type_defs.md#hlsakamaisettingstypedef) 
2. See [:material-code-braces: HlsBasicPutSettingsTypeDef](./type_defs.md#hlsbasicputsettingstypedef) 
3. See [:material-code-braces: HlsMediaStoreSettingsTypeDef](./type_defs.md#hlsmediastoresettingstypedef) 
4. See [:material-code-braces: HlsS3SettingsTypeDef](./type_defs.md#hlss3settingstypedef) 
5. See [:material-code-braces: HlsWebdavSettingsTypeDef](./type_defs.md#hlswebdavsettingstypedef) 
## NetworkInputSettingsTypeDef

```python
# NetworkInputSettingsTypeDef definition

class NetworkInputSettingsTypeDef(TypedDict):
    HlsInputSettings: NotRequired[HlsInputSettingsTypeDef],  # (1)
    ServerValidation: NotRequired[NetworkInputServerValidationType],  # (2)
```

1. See [:material-code-braces: HlsInputSettingsTypeDef](./type_defs.md#hlsinputsettingstypedef) 
2. See [:material-code-brackets: NetworkInputServerValidationType](./literals.md#networkinputservervalidationtype) 
## InputClippingSettingsTypeDef

```python
# InputClippingSettingsTypeDef definition

class InputClippingSettingsTypeDef(TypedDict):
    InputTimecodeSource: InputTimecodeSourceType,  # (1)
    StartTimecode: NotRequired[StartTimecodeTypeDef],  # (2)
    StopTimecode: NotRequired[StopTimecodeTypeDef],  # (3)
```

1. See [:material-code-brackets: InputTimecodeSourceType](./literals.md#inputtimecodesourcetype) 
2. See [:material-code-braces: StartTimecodeTypeDef](./type_defs.md#starttimecodetypedef) 
3. See [:material-code-braces: StopTimecodeTypeDef](./type_defs.md#stoptimecodetypedef) 
## InputDestinationTypeDef

```python
# InputDestinationTypeDef definition

class InputDestinationTypeDef(TypedDict):
    Ip: NotRequired[str],
    Port: NotRequired[str],
    Url: NotRequired[str],
    Vpc: NotRequired[InputDestinationVpcTypeDef],  # (1)
```

1. See [:material-code-braces: InputDestinationVpcTypeDef](./type_defs.md#inputdestinationvpctypedef) 
## UpdateInputDeviceRequestRequestTypeDef

```python
# UpdateInputDeviceRequestRequestTypeDef definition

class UpdateInputDeviceRequestRequestTypeDef(TypedDict):
    InputDeviceId: str,
    HdDeviceSettings: NotRequired[InputDeviceConfigurableSettingsTypeDef],  # (1)
    Name: NotRequired[str],
    UhdDeviceSettings: NotRequired[InputDeviceConfigurableSettingsTypeDef],  # (1)
    AvailabilityZone: NotRequired[str],
```

1. See [:material-code-braces: InputDeviceConfigurableSettingsTypeDef](./type_defs.md#inputdeviceconfigurablesettingstypedef) 
2. See [:material-code-braces: InputDeviceConfigurableSettingsTypeDef](./type_defs.md#inputdeviceconfigurablesettingstypedef) 
## UpdateInputRequestRequestTypeDef

```python
# UpdateInputRequestRequestTypeDef definition

class UpdateInputRequestRequestTypeDef(TypedDict):
    InputId: str,
    Destinations: NotRequired[Sequence[InputDestinationRequestTypeDef]],  # (1)
    InputDevices: NotRequired[Sequence[InputDeviceRequestTypeDef]],  # (2)
    InputSecurityGroups: NotRequired[Sequence[str]],
    MediaConnectFlows: NotRequired[Sequence[MediaConnectFlowRequestTypeDef]],  # (3)
    Name: NotRequired[str],
    RoleArn: NotRequired[str],
    Sources: NotRequired[Sequence[InputSourceRequestTypeDef]],  # (4)
```

1. See [:material-code-braces: InputDestinationRequestTypeDef](./type_defs.md#inputdestinationrequesttypedef) 
2. See [:material-code-braces: InputDeviceRequestTypeDef](./type_defs.md#inputdevicerequesttypedef) 
3. See [:material-code-braces: MediaConnectFlowRequestTypeDef](./type_defs.md#mediaconnectflowrequesttypedef) 
4. See [:material-code-braces: InputSourceRequestTypeDef](./type_defs.md#inputsourcerequesttypedef) 
## ListInputDeviceTransfersResponseTypeDef

```python
# ListInputDeviceTransfersResponseTypeDef definition

class ListInputDeviceTransfersResponseTypeDef(TypedDict):
    InputDeviceTransfers: List[TransferringInputDeviceSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TransferringInputDeviceSummaryTypeDef](./type_defs.md#transferringinputdevicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMultiplexProgramsResponseTypeDef

```python
# ListMultiplexProgramsResponseTypeDef definition

class ListMultiplexProgramsResponseTypeDef(TypedDict):
    MultiplexPrograms: List[MultiplexProgramSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MultiplexProgramSummaryTypeDef](./type_defs.md#multiplexprogramsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StandardHlsSettingsTypeDef

```python
# StandardHlsSettingsTypeDef definition

class StandardHlsSettingsTypeDef(TypedDict):
    M3u8Settings: M3u8SettingsTypeDef,  # (1)
    AudioRenditionSets: NotRequired[str],
```

1. See [:material-code-braces: M3u8SettingsTypeDef](./type_defs.md#m3u8settingstypedef) 
## MotionGraphicsConfigurationTypeDef

```python
# MotionGraphicsConfigurationTypeDef definition

class MotionGraphicsConfigurationTypeDef(TypedDict):
    MotionGraphicsSettings: MotionGraphicsSettingsTypeDef,  # (2)
    MotionGraphicsInsertion: NotRequired[MotionGraphicsInsertionType],  # (1)
```

1. See [:material-code-brackets: MotionGraphicsInsertionType](./literals.md#motiongraphicsinsertiontype) 
2. See [:material-code-braces: MotionGraphicsSettingsTypeDef](./type_defs.md#motiongraphicssettingstypedef) 
## MultiplexOutputDestinationTypeDef

```python
# MultiplexOutputDestinationTypeDef definition

class MultiplexOutputDestinationTypeDef(TypedDict):
    MediaConnectSettings: NotRequired[MultiplexMediaConnectOutputDestinationSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: MultiplexMediaConnectOutputDestinationSettingsTypeDef](./type_defs.md#multiplexmediaconnectoutputdestinationsettingstypedef) 
## MultiplexSummaryTypeDef

```python
# MultiplexSummaryTypeDef definition

class MultiplexSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    AvailabilityZones: NotRequired[List[str]],
    Id: NotRequired[str],
    MultiplexSettings: NotRequired[MultiplexSettingsSummaryTypeDef],  # (1)
    Name: NotRequired[str],
    PipelinesRunningCount: NotRequired[int],
    ProgramCount: NotRequired[int],
    State: NotRequired[MultiplexStateType],  # (2)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: MultiplexSettingsSummaryTypeDef](./type_defs.md#multiplexsettingssummarytypedef) 
2. See [:material-code-brackets: MultiplexStateType](./literals.md#multiplexstatetype) 
## MultiplexVideoSettingsTypeDef

```python
# MultiplexVideoSettingsTypeDef definition

class MultiplexVideoSettingsTypeDef(TypedDict):
    ConstantBitrate: NotRequired[int],
    StatmuxSettings: NotRequired[MultiplexStatmuxVideoSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: MultiplexStatmuxVideoSettingsTypeDef](./type_defs.md#multiplexstatmuxvideosettingstypedef) 
## NielsenWatermarksSettingsTypeDef

```python
# NielsenWatermarksSettingsTypeDef definition

class NielsenWatermarksSettingsTypeDef(TypedDict):
    NielsenCbetSettings: NotRequired[NielsenCBETTypeDef],  # (1)
    NielsenDistributionType: NotRequired[NielsenWatermarksDistributionTypesType],  # (2)
    NielsenNaesIiNwSettings: NotRequired[NielsenNaesIiNwTypeDef],  # (3)
```

1. See [:material-code-braces: NielsenCBETTypeDef](./type_defs.md#nielsencbettypedef) 
2. See [:material-code-brackets: NielsenWatermarksDistributionTypesType](./literals.md#nielsenwatermarksdistributiontypestype) 
3. See [:material-code-braces: NielsenNaesIiNwTypeDef](./type_defs.md#nielsennaesiinwtypedef) 
## OutputDestinationTypeDef

```python
# OutputDestinationTypeDef definition

class OutputDestinationTypeDef(TypedDict):
    Id: NotRequired[str],
    MediaPackageSettings: NotRequired[Sequence[MediaPackageOutputDestinationSettingsTypeDef]],  # (1)
    MultiplexSettings: NotRequired[MultiplexProgramChannelDestinationSettingsTypeDef],  # (2)
    Settings: NotRequired[Sequence[OutputDestinationSettingsTypeDef]],  # (3)
```

1. See [:material-code-braces: MediaPackageOutputDestinationSettingsTypeDef](./type_defs.md#mediapackageoutputdestinationsettingstypedef) 
2. See [:material-code-braces: MultiplexProgramChannelDestinationSettingsTypeDef](./type_defs.md#multiplexprogramchanneldestinationsettingstypedef) 
3. See [:material-code-braces: OutputDestinationSettingsTypeDef](./type_defs.md#outputdestinationsettingstypedef) 
## PauseStateScheduleActionSettingsTypeDef

```python
# PauseStateScheduleActionSettingsTypeDef definition

class PauseStateScheduleActionSettingsTypeDef(TypedDict):
    Pipelines: NotRequired[Sequence[PipelinePauseStateSettingsTypeDef]],  # (1)
```

1. See [:material-code-braces: PipelinePauseStateSettingsTypeDef](./type_defs.md#pipelinepausestatesettingstypedef) 
## Scte35SegmentationDescriptorTypeDef

```python
# Scte35SegmentationDescriptorTypeDef definition

class Scte35SegmentationDescriptorTypeDef(TypedDict):
    SegmentationCancelIndicator: Scte35SegmentationCancelIndicatorType,  # (2)
    SegmentationEventId: int,
    DeliveryRestrictions: NotRequired[Scte35DeliveryRestrictionsTypeDef],  # (1)
    SegmentNum: NotRequired[int],
    SegmentationDuration: NotRequired[int],
    SegmentationTypeId: NotRequired[int],
    SegmentationUpid: NotRequired[str],
    SegmentationUpidType: NotRequired[int],
    SegmentsExpected: NotRequired[int],
    SubSegmentNum: NotRequired[int],
    SubSegmentsExpected: NotRequired[int],
```

1. See [:material-code-braces: Scte35DeliveryRestrictionsTypeDef](./type_defs.md#scte35deliveryrestrictionstypedef) 
2. See [:material-code-brackets: Scte35SegmentationCancelIndicatorType](./literals.md#scte35segmentationcancelindicatortype) 
## ThumbnailDetailTypeDef

```python
# ThumbnailDetailTypeDef definition

class ThumbnailDetailTypeDef(TypedDict):
    PipelineId: NotRequired[str],
    Thumbnails: NotRequired[List[ThumbnailTypeDef]],  # (1)
```

1. See [:material-code-braces: ThumbnailTypeDef](./type_defs.md#thumbnailtypedef) 
## VideoSelectorSettingsTypeDef

```python
# VideoSelectorSettingsTypeDef definition

class VideoSelectorSettingsTypeDef(TypedDict):
    VideoSelectorPid: NotRequired[VideoSelectorPidTypeDef],  # (1)
    VideoSelectorProgramId: NotRequired[VideoSelectorProgramIdTypeDef],  # (2)
```

1. See [:material-code-braces: VideoSelectorPidTypeDef](./type_defs.md#videoselectorpidtypedef) 
2. See [:material-code-braces: VideoSelectorProgramIdTypeDef](./type_defs.md#videoselectorprogramidtypedef) 
## ArchiveGroupSettingsTypeDef

```python
# ArchiveGroupSettingsTypeDef definition

class ArchiveGroupSettingsTypeDef(TypedDict):
    Destination: OutputLocationRefTypeDef,  # (2)
    ArchiveCdnSettings: NotRequired[ArchiveCdnSettingsTypeDef],  # (1)
    RolloverInterval: NotRequired[int],
```

1. See [:material-code-braces: ArchiveCdnSettingsTypeDef](./type_defs.md#archivecdnsettingstypedef) 
2. See [:material-code-braces: OutputLocationRefTypeDef](./type_defs.md#outputlocationreftypedef) 
## RemixSettingsTypeDef

```python
# RemixSettingsTypeDef definition

class RemixSettingsTypeDef(TypedDict):
    ChannelMappings: Sequence[AudioChannelMappingTypeDef],  # (1)
    ChannelsIn: NotRequired[int],
    ChannelsOut: NotRequired[int],
```

1. See [:material-code-braces: AudioChannelMappingTypeDef](./type_defs.md#audiochannelmappingtypedef) 
## CaptionDestinationSettingsTypeDef

```python
# CaptionDestinationSettingsTypeDef definition

class CaptionDestinationSettingsTypeDef(TypedDict):
    AribDestinationSettings: NotRequired[Mapping[str, Any]],
    BurnInDestinationSettings: NotRequired[BurnInDestinationSettingsTypeDef],  # (1)
    DvbSubDestinationSettings: NotRequired[DvbSubDestinationSettingsTypeDef],  # (2)
    EbuTtDDestinationSettings: NotRequired[EbuTtDDestinationSettingsTypeDef],  # (3)
    EmbeddedDestinationSettings: NotRequired[Mapping[str, Any]],
    EmbeddedPlusScte20DestinationSettings: NotRequired[Mapping[str, Any]],
    RtmpCaptionInfoDestinationSettings: NotRequired[Mapping[str, Any]],
    Scte20PlusEmbeddedDestinationSettings: NotRequired[Mapping[str, Any]],
    Scte27DestinationSettings: NotRequired[Mapping[str, Any]],
    SmpteTtDestinationSettings: NotRequired[Mapping[str, Any]],
    TeletextDestinationSettings: NotRequired[Mapping[str, Any]],
    TtmlDestinationSettings: NotRequired[TtmlDestinationSettingsTypeDef],  # (4)
    WebvttDestinationSettings: NotRequired[WebvttDestinationSettingsTypeDef],  # (5)
```

1. See [:material-code-braces: BurnInDestinationSettingsTypeDef](./type_defs.md#burnindestinationsettingstypedef) 
2. See [:material-code-braces: DvbSubDestinationSettingsTypeDef](./type_defs.md#dvbsubdestinationsettingstypedef) 
3. See [:material-code-braces: EbuTtDDestinationSettingsTypeDef](./type_defs.md#ebuttddestinationsettingstypedef) 
4. See [:material-code-braces: TtmlDestinationSettingsTypeDef](./type_defs.md#ttmldestinationsettingstypedef) 
5. See [:material-code-braces: WebvttDestinationSettingsTypeDef](./type_defs.md#webvttdestinationsettingstypedef) 
## GlobalConfigurationTypeDef

```python
# GlobalConfigurationTypeDef definition

class GlobalConfigurationTypeDef(TypedDict):
    InitialAudioGain: NotRequired[int],
    InputEndAction: NotRequired[GlobalConfigurationInputEndActionType],  # (1)
    InputLossBehavior: NotRequired[InputLossBehaviorTypeDef],  # (2)
    OutputLockingMode: NotRequired[GlobalConfigurationOutputLockingModeType],  # (3)
    OutputTimingSource: NotRequired[GlobalConfigurationOutputTimingSourceType],  # (4)
    SupportLowFramerateInputs: NotRequired[GlobalConfigurationLowFramerateInputsType],  # (5)
```

1. See [:material-code-brackets: GlobalConfigurationInputEndActionType](./literals.md#globalconfigurationinputendactiontype) 
2. See [:material-code-braces: InputLossBehaviorTypeDef](./type_defs.md#inputlossbehaviortypedef) 
3. See [:material-code-brackets: GlobalConfigurationOutputLockingModeType](./literals.md#globalconfigurationoutputlockingmodetype) 
4. See [:material-code-brackets: GlobalConfigurationOutputTimingSourceType](./literals.md#globalconfigurationoutputtimingsourcetype) 
5. See [:material-code-brackets: GlobalConfigurationLowFramerateInputsType](./literals.md#globalconfigurationlowframerateinputstype) 
## KeyProviderSettingsTypeDef

```python
# KeyProviderSettingsTypeDef definition

class KeyProviderSettingsTypeDef(TypedDict):
    StaticKeySettings: NotRequired[StaticKeySettingsTypeDef],  # (1)
```

1. See [:material-code-braces: StaticKeySettingsTypeDef](./type_defs.md#statickeysettingstypedef) 
## AudioSelectorSettingsTypeDef

```python
# AudioSelectorSettingsTypeDef definition

class AudioSelectorSettingsTypeDef(TypedDict):
    AudioHlsRenditionSelection: NotRequired[AudioHlsRenditionSelectionTypeDef],  # (1)
    AudioLanguageSelection: NotRequired[AudioLanguageSelectionTypeDef],  # (2)
    AudioPidSelection: NotRequired[AudioPidSelectionTypeDef],  # (3)
    AudioTrackSelection: NotRequired[AudioTrackSelectionTypeDef],  # (4)
```

1. See [:material-code-braces: AudioHlsRenditionSelectionTypeDef](./type_defs.md#audiohlsrenditionselectiontypedef) 
2. See [:material-code-braces: AudioLanguageSelectionTypeDef](./type_defs.md#audiolanguageselectiontypedef) 
3. See [:material-code-braces: AudioPidSelectionTypeDef](./type_defs.md#audiopidselectiontypedef) 
4. See [:material-code-braces: AudioTrackSelectionTypeDef](./type_defs.md#audiotrackselectiontypedef) 
## AvailConfigurationTypeDef

```python
# AvailConfigurationTypeDef definition

class AvailConfigurationTypeDef(TypedDict):
    AvailSettings: NotRequired[AvailSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: AvailSettingsTypeDef](./type_defs.md#availsettingstypedef) 
## CaptionSelectorSettingsTypeDef

```python
# CaptionSelectorSettingsTypeDef definition

class CaptionSelectorSettingsTypeDef(TypedDict):
    AncillarySourceSettings: NotRequired[AncillarySourceSettingsTypeDef],  # (1)
    AribSourceSettings: NotRequired[Mapping[str, Any]],
    DvbSubSourceSettings: NotRequired[DvbSubSourceSettingsTypeDef],  # (2)
    EmbeddedSourceSettings: NotRequired[EmbeddedSourceSettingsTypeDef],  # (3)
    Scte20SourceSettings: NotRequired[Scte20SourceSettingsTypeDef],  # (4)
    Scte27SourceSettings: NotRequired[Scte27SourceSettingsTypeDef],  # (5)
    TeletextSourceSettings: NotRequired[TeletextSourceSettingsTypeDef],  # (6)
```

1. See [:material-code-braces: AncillarySourceSettingsTypeDef](./type_defs.md#ancillarysourcesettingstypedef) 
2. See [:material-code-braces: DvbSubSourceSettingsTypeDef](./type_defs.md#dvbsubsourcesettingstypedef) 
3. See [:material-code-braces: EmbeddedSourceSettingsTypeDef](./type_defs.md#embeddedsourcesettingstypedef) 
4. See [:material-code-braces: Scte20SourceSettingsTypeDef](./type_defs.md#scte20sourcesettingstypedef) 
5. See [:material-code-braces: Scte27SourceSettingsTypeDef](./type_defs.md#scte27sourcesettingstypedef) 
6. See [:material-code-braces: TeletextSourceSettingsTypeDef](./type_defs.md#teletextsourcesettingstypedef) 
## ListOfferingsResponseTypeDef

```python
# ListOfferingsResponseTypeDef definition

class ListOfferingsResponseTypeDef(TypedDict):
    NextToken: str,
    Offerings: List[OfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OfferingTypeDef](./type_defs.md#offeringtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReservationsResponseTypeDef

```python
# ListReservationsResponseTypeDef definition

class ListReservationsResponseTypeDef(TypedDict):
    NextToken: str,
    Reservations: List[ReservationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservationTypeDef](./type_defs.md#reservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PurchaseOfferingResponseTypeDef

```python
# PurchaseOfferingResponseTypeDef definition

class PurchaseOfferingResponseTypeDef(TypedDict):
    Reservation: ReservationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservationTypeDef](./type_defs.md#reservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReservationResponseTypeDef

```python
# UpdateReservationResponseTypeDef definition

class UpdateReservationResponseTypeDef(TypedDict):
    Reservation: ReservationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservationTypeDef](./type_defs.md#reservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInputDevicesResponseTypeDef

```python
# ListInputDevicesResponseTypeDef definition

class ListInputDevicesResponseTypeDef(TypedDict):
    InputDevices: List[InputDeviceSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputDeviceSummaryTypeDef](./type_defs.md#inputdevicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInputSecurityGroupResponseTypeDef

```python
# CreateInputSecurityGroupResponseTypeDef definition

class CreateInputSecurityGroupResponseTypeDef(TypedDict):
    SecurityGroup: InputSecurityGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputSecurityGroupTypeDef](./type_defs.md#inputsecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInputSecurityGroupsResponseTypeDef

```python
# ListInputSecurityGroupsResponseTypeDef definition

class ListInputSecurityGroupsResponseTypeDef(TypedDict):
    InputSecurityGroups: List[InputSecurityGroupTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputSecurityGroupTypeDef](./type_defs.md#inputsecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInputSecurityGroupResponseTypeDef

```python
# UpdateInputSecurityGroupResponseTypeDef definition

class UpdateInputSecurityGroupResponseTypeDef(TypedDict):
    SecurityGroup: InputSecurityGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputSecurityGroupTypeDef](./type_defs.md#inputsecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ArchiveContainerSettingsTypeDef

```python
# ArchiveContainerSettingsTypeDef definition

class ArchiveContainerSettingsTypeDef(TypedDict):
    M2tsSettings: NotRequired[M2tsSettingsTypeDef],  # (1)
    RawSettings: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: M2tsSettingsTypeDef](./type_defs.md#m2tssettingstypedef) 
## UdpContainerSettingsTypeDef

```python
# UdpContainerSettingsTypeDef definition

class UdpContainerSettingsTypeDef(TypedDict):
    M2tsSettings: NotRequired[M2tsSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: M2tsSettingsTypeDef](./type_defs.md#m2tssettingstypedef) 
## FailoverConditionTypeDef

```python
# FailoverConditionTypeDef definition

class FailoverConditionTypeDef(TypedDict):
    FailoverConditionSettings: NotRequired[FailoverConditionSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: FailoverConditionSettingsTypeDef](./type_defs.md#failoverconditionsettingstypedef) 
## FrameCaptureGroupSettingsTypeDef

```python
# FrameCaptureGroupSettingsTypeDef definition

class FrameCaptureGroupSettingsTypeDef(TypedDict):
    Destination: OutputLocationRefTypeDef,  # (1)
    FrameCaptureCdnSettings: NotRequired[FrameCaptureCdnSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: OutputLocationRefTypeDef](./type_defs.md#outputlocationreftypedef) 
2. See [:material-code-braces: FrameCaptureCdnSettingsTypeDef](./type_defs.md#framecapturecdnsettingstypedef) 
## H264SettingsTypeDef

```python
# H264SettingsTypeDef definition

class H264SettingsTypeDef(TypedDict):
    AdaptiveQuantization: NotRequired[H264AdaptiveQuantizationType],  # (1)
    AfdSignaling: NotRequired[AfdSignalingType],  # (2)
    Bitrate: NotRequired[int],
    BufFillPct: NotRequired[int],
    BufSize: NotRequired[int],
    ColorMetadata: NotRequired[H264ColorMetadataType],  # (3)
    ColorSpaceSettings: NotRequired[H264ColorSpaceSettingsTypeDef],  # (4)
    EntropyEncoding: NotRequired[H264EntropyEncodingType],  # (5)
    FilterSettings: NotRequired[H264FilterSettingsTypeDef],  # (6)
    FixedAfd: NotRequired[FixedAfdType],  # (7)
    FlickerAq: NotRequired[H264FlickerAqType],  # (8)
    ForceFieldPictures: NotRequired[H264ForceFieldPicturesType],  # (9)
    FramerateControl: NotRequired[H264FramerateControlType],  # (10)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    GopBReference: NotRequired[H264GopBReferenceType],  # (11)
    GopClosedCadence: NotRequired[int],
    GopNumBFrames: NotRequired[int],
    GopSize: NotRequired[float],
    GopSizeUnits: NotRequired[H264GopSizeUnitsType],  # (12)
    Level: NotRequired[H264LevelType],  # (13)
    LookAheadRateControl: NotRequired[H264LookAheadRateControlType],  # (14)
    MaxBitrate: NotRequired[int],
    MinIInterval: NotRequired[int],
    NumRefFrames: NotRequired[int],
    ParControl: NotRequired[H264ParControlType],  # (15)
    ParDenominator: NotRequired[int],
    ParNumerator: NotRequired[int],
    Profile: NotRequired[H264ProfileType],  # (16)
    QualityLevel: NotRequired[H264QualityLevelType],  # (17)
    QvbrQualityLevel: NotRequired[int],
    RateControlMode: NotRequired[H264RateControlModeType],  # (18)
    ScanType: NotRequired[H264ScanTypeType],  # (19)
    SceneChangeDetect: NotRequired[H264SceneChangeDetectType],  # (20)
    Slices: NotRequired[int],
    Softness: NotRequired[int],
    SpatialAq: NotRequired[H264SpatialAqType],  # (21)
    SubgopLength: NotRequired[H264SubGopLengthType],  # (22)
    Syntax: NotRequired[H264SyntaxType],  # (23)
    TemporalAq: NotRequired[H264TemporalAqType],  # (24)
    TimecodeInsertion: NotRequired[H264TimecodeInsertionBehaviorType],  # (25)
    TimecodeBurninSettings: NotRequired[TimecodeBurninSettingsTypeDef],  # (26)
```

1. See [:material-code-brackets: H264AdaptiveQuantizationType](./literals.md#h264adaptivequantizationtype) 
2. See [:material-code-brackets: AfdSignalingType](./literals.md#afdsignalingtype) 
3. See [:material-code-brackets: H264ColorMetadataType](./literals.md#h264colormetadatatype) 
4. See [:material-code-braces: H264ColorSpaceSettingsTypeDef](./type_defs.md#h264colorspacesettingstypedef) 
5. See [:material-code-brackets: H264EntropyEncodingType](./literals.md#h264entropyencodingtype) 
6. See [:material-code-braces: H264FilterSettingsTypeDef](./type_defs.md#h264filtersettingstypedef) 
7. See [:material-code-brackets: FixedAfdType](./literals.md#fixedafdtype) 
8. See [:material-code-brackets: H264FlickerAqType](./literals.md#h264flickeraqtype) 
9. See [:material-code-brackets: H264ForceFieldPicturesType](./literals.md#h264forcefieldpicturestype) 
10. See [:material-code-brackets: H264FramerateControlType](./literals.md#h264frameratecontroltype) 
11. See [:material-code-brackets: H264GopBReferenceType](./literals.md#h264gopbreferencetype) 
12. See [:material-code-brackets: H264GopSizeUnitsType](./literals.md#h264gopsizeunitstype) 
13. See [:material-code-brackets: H264LevelType](./literals.md#h264leveltype) 
14. See [:material-code-brackets: H264LookAheadRateControlType](./literals.md#h264lookaheadratecontroltype) 
15. See [:material-code-brackets: H264ParControlType](./literals.md#h264parcontroltype) 
16. See [:material-code-brackets: H264ProfileType](./literals.md#h264profiletype) 
17. See [:material-code-brackets: H264QualityLevelType](./literals.md#h264qualityleveltype) 
18. See [:material-code-brackets: H264RateControlModeType](./literals.md#h264ratecontrolmodetype) 
19. See [:material-code-brackets: H264ScanTypeType](./literals.md#h264scantypetype) 
20. See [:material-code-brackets: H264SceneChangeDetectType](./literals.md#h264scenechangedetecttype) 
21. See [:material-code-brackets: H264SpatialAqType](./literals.md#h264spatialaqtype) 
22. See [:material-code-brackets: H264SubGopLengthType](./literals.md#h264subgoplengthtype) 
23. See [:material-code-brackets: H264SyntaxType](./literals.md#h264syntaxtype) 
24. See [:material-code-brackets: H264TemporalAqType](./literals.md#h264temporalaqtype) 
25. See [:material-code-brackets: H264TimecodeInsertionBehaviorType](./literals.md#h264timecodeinsertionbehaviortype) 
26. See [:material-code-braces: TimecodeBurninSettingsTypeDef](./type_defs.md#timecodeburninsettingstypedef) 
## Mpeg2SettingsTypeDef

```python
# Mpeg2SettingsTypeDef definition

class Mpeg2SettingsTypeDef(TypedDict):
    FramerateDenominator: int,
    FramerateNumerator: int,
    AdaptiveQuantization: NotRequired[Mpeg2AdaptiveQuantizationType],  # (1)
    AfdSignaling: NotRequired[AfdSignalingType],  # (2)
    ColorMetadata: NotRequired[Mpeg2ColorMetadataType],  # (3)
    ColorSpace: NotRequired[Mpeg2ColorSpaceType],  # (4)
    DisplayAspectRatio: NotRequired[Mpeg2DisplayRatioType],  # (5)
    FilterSettings: NotRequired[Mpeg2FilterSettingsTypeDef],  # (6)
    FixedAfd: NotRequired[FixedAfdType],  # (7)
    GopClosedCadence: NotRequired[int],
    GopNumBFrames: NotRequired[int],
    GopSize: NotRequired[float],
    GopSizeUnits: NotRequired[Mpeg2GopSizeUnitsType],  # (8)
    ScanType: NotRequired[Mpeg2ScanTypeType],  # (9)
    SubgopLength: NotRequired[Mpeg2SubGopLengthType],  # (10)
    TimecodeInsertion: NotRequired[Mpeg2TimecodeInsertionBehaviorType],  # (11)
    TimecodeBurninSettings: NotRequired[TimecodeBurninSettingsTypeDef],  # (12)
```

1. See [:material-code-brackets: Mpeg2AdaptiveQuantizationType](./literals.md#mpeg2adaptivequantizationtype) 
2. See [:material-code-brackets: AfdSignalingType](./literals.md#afdsignalingtype) 
3. See [:material-code-brackets: Mpeg2ColorMetadataType](./literals.md#mpeg2colormetadatatype) 
4. See [:material-code-brackets: Mpeg2ColorSpaceType](./literals.md#mpeg2colorspacetype) 
5. See [:material-code-brackets: Mpeg2DisplayRatioType](./literals.md#mpeg2displayratiotype) 
6. See [:material-code-braces: Mpeg2FilterSettingsTypeDef](./type_defs.md#mpeg2filtersettingstypedef) 
7. See [:material-code-brackets: FixedAfdType](./literals.md#fixedafdtype) 
8. See [:material-code-brackets: Mpeg2GopSizeUnitsType](./literals.md#mpeg2gopsizeunitstype) 
9. See [:material-code-brackets: Mpeg2ScanTypeType](./literals.md#mpeg2scantypetype) 
10. See [:material-code-brackets: Mpeg2SubGopLengthType](./literals.md#mpeg2subgoplengthtype) 
11. See [:material-code-brackets: Mpeg2TimecodeInsertionBehaviorType](./literals.md#mpeg2timecodeinsertionbehaviortype) 
12. See [:material-code-braces: TimecodeBurninSettingsTypeDef](./type_defs.md#timecodeburninsettingstypedef) 
## H265SettingsTypeDef

```python
# H265SettingsTypeDef definition

class H265SettingsTypeDef(TypedDict):
    FramerateDenominator: int,
    FramerateNumerator: int,
    AdaptiveQuantization: NotRequired[H265AdaptiveQuantizationType],  # (1)
    AfdSignaling: NotRequired[AfdSignalingType],  # (2)
    AlternativeTransferFunction: NotRequired[H265AlternativeTransferFunctionType],  # (3)
    Bitrate: NotRequired[int],
    BufSize: NotRequired[int],
    ColorMetadata: NotRequired[H265ColorMetadataType],  # (4)
    ColorSpaceSettings: NotRequired[H265ColorSpaceSettingsTypeDef],  # (5)
    FilterSettings: NotRequired[H265FilterSettingsTypeDef],  # (6)
    FixedAfd: NotRequired[FixedAfdType],  # (7)
    FlickerAq: NotRequired[H265FlickerAqType],  # (8)
    GopClosedCadence: NotRequired[int],
    GopSize: NotRequired[float],
    GopSizeUnits: NotRequired[H265GopSizeUnitsType],  # (9)
    Level: NotRequired[H265LevelType],  # (10)
    LookAheadRateControl: NotRequired[H265LookAheadRateControlType],  # (11)
    MaxBitrate: NotRequired[int],
    MinIInterval: NotRequired[int],
    ParDenominator: NotRequired[int],
    ParNumerator: NotRequired[int],
    Profile: NotRequired[H265ProfileType],  # (12)
    QvbrQualityLevel: NotRequired[int],
    RateControlMode: NotRequired[H265RateControlModeType],  # (13)
    ScanType: NotRequired[H265ScanTypeType],  # (14)
    SceneChangeDetect: NotRequired[H265SceneChangeDetectType],  # (15)
    Slices: NotRequired[int],
    Tier: NotRequired[H265TierType],  # (16)
    TimecodeInsertion: NotRequired[H265TimecodeInsertionBehaviorType],  # (17)
    TimecodeBurninSettings: NotRequired[TimecodeBurninSettingsTypeDef],  # (18)
```

1. See [:material-code-brackets: H265AdaptiveQuantizationType](./literals.md#h265adaptivequantizationtype) 
2. See [:material-code-brackets: AfdSignalingType](./literals.md#afdsignalingtype) 
3. See [:material-code-brackets: H265AlternativeTransferFunctionType](./literals.md#h265alternativetransferfunctiontype) 
4. See [:material-code-brackets: H265ColorMetadataType](./literals.md#h265colormetadatatype) 
5. See [:material-code-braces: H265ColorSpaceSettingsTypeDef](./type_defs.md#h265colorspacesettingstypedef) 
6. See [:material-code-braces: H265FilterSettingsTypeDef](./type_defs.md#h265filtersettingstypedef) 
7. See [:material-code-brackets: FixedAfdType](./literals.md#fixedafdtype) 
8. See [:material-code-brackets: H265FlickerAqType](./literals.md#h265flickeraqtype) 
9. See [:material-code-brackets: H265GopSizeUnitsType](./literals.md#h265gopsizeunitstype) 
10. See [:material-code-brackets: H265LevelType](./literals.md#h265leveltype) 
11. See [:material-code-brackets: H265LookAheadRateControlType](./literals.md#h265lookaheadratecontroltype) 
12. See [:material-code-brackets: H265ProfileType](./literals.md#h265profiletype) 
13. See [:material-code-brackets: H265RateControlModeType](./literals.md#h265ratecontrolmodetype) 
14. See [:material-code-brackets: H265ScanTypeType](./literals.md#h265scantypetype) 
15. See [:material-code-brackets: H265SceneChangeDetectType](./literals.md#h265scenechangedetecttype) 
16. See [:material-code-brackets: H265TierType](./literals.md#h265tiertype) 
17. See [:material-code-brackets: H265TimecodeInsertionBehaviorType](./literals.md#h265timecodeinsertionbehaviortype) 
18. See [:material-code-braces: TimecodeBurninSettingsTypeDef](./type_defs.md#timecodeburninsettingstypedef) 
## InputPrepareScheduleActionSettingsTypeDef

```python
# InputPrepareScheduleActionSettingsTypeDef definition

class InputPrepareScheduleActionSettingsTypeDef(TypedDict):
    InputAttachmentNameReference: NotRequired[str],
    InputClippingSettings: NotRequired[InputClippingSettingsTypeDef],  # (1)
    UrlPath: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: InputClippingSettingsTypeDef](./type_defs.md#inputclippingsettingstypedef) 
## InputSwitchScheduleActionSettingsTypeDef

```python
# InputSwitchScheduleActionSettingsTypeDef definition

class InputSwitchScheduleActionSettingsTypeDef(TypedDict):
    InputAttachmentNameReference: str,
    InputClippingSettings: NotRequired[InputClippingSettingsTypeDef],  # (1)
    UrlPath: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: InputClippingSettingsTypeDef](./type_defs.md#inputclippingsettingstypedef) 
## DescribeInputResponseTypeDef

```python
# DescribeInputResponseTypeDef definition

class DescribeInputResponseTypeDef(TypedDict):
    Arn: str,
    AttachedChannels: List[str],
    Destinations: List[InputDestinationTypeDef],  # (1)
    Id: str,
    InputClass: InputClassType,  # (2)
    InputDevices: List[InputDeviceSettingsTypeDef],  # (3)
    InputPartnerIds: List[str],
    InputSourceType: InputSourceTypeType,  # (4)
    MediaConnectFlows: List[MediaConnectFlowTypeDef],  # (5)
    Name: str,
    RoleArn: str,
    SecurityGroups: List[str],
    Sources: List[InputSourceTypeDef],  # (6)
    State: InputStateType,  # (7)
    Tags: Dict[str, str],
    Type: InputTypeType,  # (8)
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-braces: InputDestinationTypeDef](./type_defs.md#inputdestinationtypedef) 
2. See [:material-code-brackets: InputClassType](./literals.md#inputclasstype) 
3. See [:material-code-braces: InputDeviceSettingsTypeDef](./type_defs.md#inputdevicesettingstypedef) 
4. See [:material-code-brackets: InputSourceTypeType](./literals.md#inputsourcetypetype) 
5. See [:material-code-braces: MediaConnectFlowTypeDef](./type_defs.md#mediaconnectflowtypedef) 
6. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
7. See [:material-code-brackets: InputStateType](./literals.md#inputstatetype) 
8. See [:material-code-brackets: InputTypeType](./literals.md#inputtypetype) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InputTypeDef

```python
# InputTypeDef definition

class InputTypeDef(TypedDict):
    Arn: NotRequired[str],
    AttachedChannels: NotRequired[List[str]],
    Destinations: NotRequired[List[InputDestinationTypeDef]],  # (1)
    Id: NotRequired[str],
    InputClass: NotRequired[InputClassType],  # (2)
    InputDevices: NotRequired[List[InputDeviceSettingsTypeDef]],  # (3)
    InputPartnerIds: NotRequired[List[str]],
    InputSourceType: NotRequired[InputSourceTypeType],  # (4)
    MediaConnectFlows: NotRequired[List[MediaConnectFlowTypeDef]],  # (5)
    Name: NotRequired[str],
    RoleArn: NotRequired[str],
    SecurityGroups: NotRequired[List[str]],
    Sources: NotRequired[List[InputSourceTypeDef]],  # (6)
    State: NotRequired[InputStateType],  # (7)
    Tags: NotRequired[Dict[str, str]],
    Type: NotRequired[InputTypeType],  # (8)
```

1. See [:material-code-braces: InputDestinationTypeDef](./type_defs.md#inputdestinationtypedef) 
2. See [:material-code-brackets: InputClassType](./literals.md#inputclasstype) 
3. See [:material-code-braces: InputDeviceSettingsTypeDef](./type_defs.md#inputdevicesettingstypedef) 
4. See [:material-code-brackets: InputSourceTypeType](./literals.md#inputsourcetypetype) 
5. See [:material-code-braces: MediaConnectFlowTypeDef](./type_defs.md#mediaconnectflowtypedef) 
6. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
7. See [:material-code-brackets: InputStateType](./literals.md#inputstatetype) 
8. See [:material-code-brackets: InputTypeType](./literals.md#inputtypetype) 
## HlsSettingsTypeDef

```python
# HlsSettingsTypeDef definition

class HlsSettingsTypeDef(TypedDict):
    AudioOnlyHlsSettings: NotRequired[AudioOnlyHlsSettingsTypeDef],  # (1)
    Fmp4HlsSettings: NotRequired[Fmp4HlsSettingsTypeDef],  # (2)
    FrameCaptureHlsSettings: NotRequired[Mapping[str, Any]],
    StandardHlsSettings: NotRequired[StandardHlsSettingsTypeDef],  # (3)
```

1. See [:material-code-braces: AudioOnlyHlsSettingsTypeDef](./type_defs.md#audioonlyhlssettingstypedef) 
2. See [:material-code-braces: Fmp4HlsSettingsTypeDef](./type_defs.md#fmp4hlssettingstypedef) 
3. See [:material-code-braces: StandardHlsSettingsTypeDef](./type_defs.md#standardhlssettingstypedef) 
## DeleteMultiplexResponseTypeDef

```python
# DeleteMultiplexResponseTypeDef definition

class DeleteMultiplexResponseTypeDef(TypedDict):
    Arn: str,
    AvailabilityZones: List[str],
    Destinations: List[MultiplexOutputDestinationTypeDef],  # (1)
    Id: str,
    MultiplexSettings: MultiplexSettingsTypeDef,  # (2)
    Name: str,
    PipelinesRunningCount: int,
    ProgramCount: int,
    State: MultiplexStateType,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: MultiplexOutputDestinationTypeDef](./type_defs.md#multiplexoutputdestinationtypedef) 
2. See [:material-code-braces: MultiplexSettingsTypeDef](./type_defs.md#multiplexsettingstypedef) 
3. See [:material-code-brackets: MultiplexStateType](./literals.md#multiplexstatetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMultiplexResponseTypeDef

```python
# DescribeMultiplexResponseTypeDef definition

class DescribeMultiplexResponseTypeDef(TypedDict):
    Arn: str,
    AvailabilityZones: List[str],
    Destinations: List[MultiplexOutputDestinationTypeDef],  # (1)
    Id: str,
    MultiplexSettings: MultiplexSettingsTypeDef,  # (2)
    Name: str,
    PipelinesRunningCount: int,
    ProgramCount: int,
    State: MultiplexStateType,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: MultiplexOutputDestinationTypeDef](./type_defs.md#multiplexoutputdestinationtypedef) 
2. See [:material-code-braces: MultiplexSettingsTypeDef](./type_defs.md#multiplexsettingstypedef) 
3. See [:material-code-brackets: MultiplexStateType](./literals.md#multiplexstatetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MultiplexTypeDef

```python
# MultiplexTypeDef definition

class MultiplexTypeDef(TypedDict):
    Arn: NotRequired[str],
    AvailabilityZones: NotRequired[List[str]],
    Destinations: NotRequired[List[MultiplexOutputDestinationTypeDef]],  # (1)
    Id: NotRequired[str],
    MultiplexSettings: NotRequired[MultiplexSettingsTypeDef],  # (2)
    Name: NotRequired[str],
    PipelinesRunningCount: NotRequired[int],
    ProgramCount: NotRequired[int],
    State: NotRequired[MultiplexStateType],  # (3)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: MultiplexOutputDestinationTypeDef](./type_defs.md#multiplexoutputdestinationtypedef) 
2. See [:material-code-braces: MultiplexSettingsTypeDef](./type_defs.md#multiplexsettingstypedef) 
3. See [:material-code-brackets: MultiplexStateType](./literals.md#multiplexstatetype) 
## StartMultiplexResponseTypeDef

```python
# StartMultiplexResponseTypeDef definition

class StartMultiplexResponseTypeDef(TypedDict):
    Arn: str,
    AvailabilityZones: List[str],
    Destinations: List[MultiplexOutputDestinationTypeDef],  # (1)
    Id: str,
    MultiplexSettings: MultiplexSettingsTypeDef,  # (2)
    Name: str,
    PipelinesRunningCount: int,
    ProgramCount: int,
    State: MultiplexStateType,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: MultiplexOutputDestinationTypeDef](./type_defs.md#multiplexoutputdestinationtypedef) 
2. See [:material-code-braces: MultiplexSettingsTypeDef](./type_defs.md#multiplexsettingstypedef) 
3. See [:material-code-brackets: MultiplexStateType](./literals.md#multiplexstatetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopMultiplexResponseTypeDef

```python
# StopMultiplexResponseTypeDef definition

class StopMultiplexResponseTypeDef(TypedDict):
    Arn: str,
    AvailabilityZones: List[str],
    Destinations: List[MultiplexOutputDestinationTypeDef],  # (1)
    Id: str,
    MultiplexSettings: MultiplexSettingsTypeDef,  # (2)
    Name: str,
    PipelinesRunningCount: int,
    ProgramCount: int,
    State: MultiplexStateType,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: MultiplexOutputDestinationTypeDef](./type_defs.md#multiplexoutputdestinationtypedef) 
2. See [:material-code-braces: MultiplexSettingsTypeDef](./type_defs.md#multiplexsettingstypedef) 
3. See [:material-code-brackets: MultiplexStateType](./literals.md#multiplexstatetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMultiplexesResponseTypeDef

```python
# ListMultiplexesResponseTypeDef definition

class ListMultiplexesResponseTypeDef(TypedDict):
    Multiplexes: List[MultiplexSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MultiplexSummaryTypeDef](./type_defs.md#multiplexsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MultiplexProgramSettingsTypeDef

```python
# MultiplexProgramSettingsTypeDef definition

class MultiplexProgramSettingsTypeDef(TypedDict):
    ProgramNumber: int,
    PreferredChannelPipeline: NotRequired[PreferredChannelPipelineType],  # (1)
    ServiceDescriptor: NotRequired[MultiplexProgramServiceDescriptorTypeDef],  # (2)
    VideoSettings: NotRequired[MultiplexVideoSettingsTypeDef],  # (3)
```

1. See [:material-code-brackets: PreferredChannelPipelineType](./literals.md#preferredchannelpipelinetype) 
2. See [:material-code-braces: MultiplexProgramServiceDescriptorTypeDef](./type_defs.md#multiplexprogramservicedescriptortypedef) 
3. See [:material-code-braces: MultiplexVideoSettingsTypeDef](./type_defs.md#multiplexvideosettingstypedef) 
## AudioWatermarkSettingsTypeDef

```python
# AudioWatermarkSettingsTypeDef definition

class AudioWatermarkSettingsTypeDef(TypedDict):
    NielsenWatermarksSettings: NotRequired[NielsenWatermarksSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: NielsenWatermarksSettingsTypeDef](./type_defs.md#nielsenwatermarkssettingstypedef) 
## UpdateChannelClassRequestRequestTypeDef

```python
# UpdateChannelClassRequestRequestTypeDef definition

class UpdateChannelClassRequestRequestTypeDef(TypedDict):
    ChannelClass: ChannelClassType,  # (1)
    ChannelId: str,
    Destinations: NotRequired[Sequence[OutputDestinationTypeDef]],  # (2)
```

1. See [:material-code-brackets: ChannelClassType](./literals.md#channelclasstype) 
2. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) 
## Scte35DescriptorSettingsTypeDef

```python
# Scte35DescriptorSettingsTypeDef definition

class Scte35DescriptorSettingsTypeDef(TypedDict):
    SegmentationDescriptorScte35DescriptorSettings: Scte35SegmentationDescriptorTypeDef,  # (1)
```

1. See [:material-code-braces: Scte35SegmentationDescriptorTypeDef](./type_defs.md#scte35segmentationdescriptortypedef) 
## DescribeThumbnailsResponseTypeDef

```python
# DescribeThumbnailsResponseTypeDef definition

class DescribeThumbnailsResponseTypeDef(TypedDict):
    ThumbnailDetails: List[ThumbnailDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThumbnailDetailTypeDef](./type_defs.md#thumbnaildetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VideoSelectorTypeDef

```python
# VideoSelectorTypeDef definition

class VideoSelectorTypeDef(TypedDict):
    ColorSpace: NotRequired[VideoSelectorColorSpaceType],  # (1)
    ColorSpaceSettings: NotRequired[VideoSelectorColorSpaceSettingsTypeDef],  # (2)
    ColorSpaceUsage: NotRequired[VideoSelectorColorSpaceUsageType],  # (3)
    SelectorSettings: NotRequired[VideoSelectorSettingsTypeDef],  # (4)
```

1. See [:material-code-brackets: VideoSelectorColorSpaceType](./literals.md#videoselectorcolorspacetype) 
2. See [:material-code-braces: VideoSelectorColorSpaceSettingsTypeDef](./type_defs.md#videoselectorcolorspacesettingstypedef) 
3. See [:material-code-brackets: VideoSelectorColorSpaceUsageType](./literals.md#videoselectorcolorspaceusagetype) 
4. See [:material-code-braces: VideoSelectorSettingsTypeDef](./type_defs.md#videoselectorsettingstypedef) 
## CaptionDescriptionTypeDef

```python
# CaptionDescriptionTypeDef definition

class CaptionDescriptionTypeDef(TypedDict):
    CaptionSelectorName: str,
    Name: str,
    Accessibility: NotRequired[AccessibilityTypeType],  # (1)
    DestinationSettings: NotRequired[CaptionDestinationSettingsTypeDef],  # (2)
    LanguageCode: NotRequired[str],
    LanguageDescription: NotRequired[str],
```

1. See [:material-code-brackets: AccessibilityTypeType](./literals.md#accessibilitytypetype) 
2. See [:material-code-braces: CaptionDestinationSettingsTypeDef](./type_defs.md#captiondestinationsettingstypedef) 
## HlsGroupSettingsTypeDef

```python
# HlsGroupSettingsTypeDef definition

class HlsGroupSettingsTypeDef(TypedDict):
    Destination: OutputLocationRefTypeDef,  # (6)
    AdMarkers: NotRequired[Sequence[HlsAdMarkersType]],  # (1)
    BaseUrlContent: NotRequired[str],
    BaseUrlContent1: NotRequired[str],
    BaseUrlManifest: NotRequired[str],
    BaseUrlManifest1: NotRequired[str],
    CaptionLanguageMappings: NotRequired[Sequence[CaptionLanguageMappingTypeDef]],  # (2)
    CaptionLanguageSetting: NotRequired[HlsCaptionLanguageSettingType],  # (3)
    ClientCache: NotRequired[HlsClientCacheType],  # (4)
    CodecSpecification: NotRequired[HlsCodecSpecificationType],  # (5)
    ConstantIv: NotRequired[str],
    DirectoryStructure: NotRequired[HlsDirectoryStructureType],  # (7)
    DiscontinuityTags: NotRequired[HlsDiscontinuityTagsType],  # (8)
    EncryptionType: NotRequired[HlsEncryptionTypeType],  # (9)
    HlsCdnSettings: NotRequired[HlsCdnSettingsTypeDef],  # (10)
    HlsId3SegmentTagging: NotRequired[HlsId3SegmentTaggingStateType],  # (11)
    IFrameOnlyPlaylists: NotRequired[IFrameOnlyPlaylistTypeType],  # (12)
    IncompleteSegmentBehavior: NotRequired[HlsIncompleteSegmentBehaviorType],  # (13)
    IndexNSegments: NotRequired[int],
    InputLossAction: NotRequired[InputLossActionForHlsOutType],  # (14)
    IvInManifest: NotRequired[HlsIvInManifestType],  # (15)
    IvSource: NotRequired[HlsIvSourceType],  # (16)
    KeepSegments: NotRequired[int],
    KeyFormat: NotRequired[str],
    KeyFormatVersions: NotRequired[str],
    KeyProviderSettings: NotRequired[KeyProviderSettingsTypeDef],  # (17)
    ManifestCompression: NotRequired[HlsManifestCompressionType],  # (18)
    ManifestDurationFormat: NotRequired[HlsManifestDurationFormatType],  # (19)
    MinSegmentLength: NotRequired[int],
    Mode: NotRequired[HlsModeType],  # (20)
    OutputSelection: NotRequired[HlsOutputSelectionType],  # (21)
    ProgramDateTime: NotRequired[HlsProgramDateTimeType],  # (22)
    ProgramDateTimeClock: NotRequired[HlsProgramDateTimeClockType],  # (23)
    ProgramDateTimePeriod: NotRequired[int],
    RedundantManifest: NotRequired[HlsRedundantManifestType],  # (24)
    SegmentLength: NotRequired[int],
    SegmentationMode: NotRequired[HlsSegmentationModeType],  # (25)
    SegmentsPerSubdirectory: NotRequired[int],
    StreamInfResolution: NotRequired[HlsStreamInfResolutionType],  # (26)
    TimedMetadataId3Frame: NotRequired[HlsTimedMetadataId3FrameType],  # (27)
    TimedMetadataId3Period: NotRequired[int],
    TimestampDeltaMilliseconds: NotRequired[int],
    TsFileMode: NotRequired[HlsTsFileModeType],  # (28)
```

1. See [:material-code-brackets: HlsAdMarkersType](./literals.md#hlsadmarkerstype) 
2. See [:material-code-braces: CaptionLanguageMappingTypeDef](./type_defs.md#captionlanguagemappingtypedef) 
3. See [:material-code-brackets: HlsCaptionLanguageSettingType](./literals.md#hlscaptionlanguagesettingtype) 
4. See [:material-code-brackets: HlsClientCacheType](./literals.md#hlsclientcachetype) 
5. See [:material-code-brackets: HlsCodecSpecificationType](./literals.md#hlscodecspecificationtype) 
6. See [:material-code-braces: OutputLocationRefTypeDef](./type_defs.md#outputlocationreftypedef) 
7. See [:material-code-brackets: HlsDirectoryStructureType](./literals.md#hlsdirectorystructuretype) 
8. See [:material-code-brackets: HlsDiscontinuityTagsType](./literals.md#hlsdiscontinuitytagstype) 
9. See [:material-code-brackets: HlsEncryptionTypeType](./literals.md#hlsencryptiontypetype) 
10. See [:material-code-braces: HlsCdnSettingsTypeDef](./type_defs.md#hlscdnsettingstypedef) 
11. See [:material-code-brackets: HlsId3SegmentTaggingStateType](./literals.md#hlsid3segmenttaggingstatetype) 
12. See [:material-code-brackets: IFrameOnlyPlaylistTypeType](./literals.md#iframeonlyplaylisttypetype) 
13. See [:material-code-brackets: HlsIncompleteSegmentBehaviorType](./literals.md#hlsincompletesegmentbehaviortype) 
14. See [:material-code-brackets: InputLossActionForHlsOutType](./literals.md#inputlossactionforhlsouttype) 
15. See [:material-code-brackets: HlsIvInManifestType](./literals.md#hlsivinmanifesttype) 
16. See [:material-code-brackets: HlsIvSourceType](./literals.md#hlsivsourcetype) 
17. See [:material-code-braces: KeyProviderSettingsTypeDef](./type_defs.md#keyprovidersettingstypedef) 
18. See [:material-code-brackets: HlsManifestCompressionType](./literals.md#hlsmanifestcompressiontype) 
19. See [:material-code-brackets: HlsManifestDurationFormatType](./literals.md#hlsmanifestdurationformattype) 
20. See [:material-code-brackets: HlsModeType](./literals.md#hlsmodetype) 
21. See [:material-code-brackets: HlsOutputSelectionType](./literals.md#hlsoutputselectiontype) 
22. See [:material-code-brackets: HlsProgramDateTimeType](./literals.md#hlsprogramdatetimetype) 
23. See [:material-code-brackets: HlsProgramDateTimeClockType](./literals.md#hlsprogramdatetimeclocktype) 
24. See [:material-code-brackets: HlsRedundantManifestType](./literals.md#hlsredundantmanifesttype) 
25. See [:material-code-brackets: HlsSegmentationModeType](./literals.md#hlssegmentationmodetype) 
26. See [:material-code-brackets: HlsStreamInfResolutionType](./literals.md#hlsstreaminfresolutiontype) 
27. See [:material-code-brackets: HlsTimedMetadataId3FrameType](./literals.md#hlstimedmetadataid3frametype) 
28. See [:material-code-brackets: HlsTsFileModeType](./literals.md#hlstsfilemodetype) 
## AudioSelectorTypeDef

```python
# AudioSelectorTypeDef definition

class AudioSelectorTypeDef(TypedDict):
    Name: str,
    SelectorSettings: NotRequired[AudioSelectorSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: AudioSelectorSettingsTypeDef](./type_defs.md#audioselectorsettingstypedef) 
## CaptionSelectorTypeDef

```python
# CaptionSelectorTypeDef definition

class CaptionSelectorTypeDef(TypedDict):
    Name: str,
    LanguageCode: NotRequired[str],
    SelectorSettings: NotRequired[CaptionSelectorSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: CaptionSelectorSettingsTypeDef](./type_defs.md#captionselectorsettingstypedef) 
## ArchiveOutputSettingsTypeDef

```python
# ArchiveOutputSettingsTypeDef definition

class ArchiveOutputSettingsTypeDef(TypedDict):
    ContainerSettings: ArchiveContainerSettingsTypeDef,  # (1)
    Extension: NotRequired[str],
    NameModifier: NotRequired[str],
```

1. See [:material-code-braces: ArchiveContainerSettingsTypeDef](./type_defs.md#archivecontainersettingstypedef) 
## UdpOutputSettingsTypeDef

```python
# UdpOutputSettingsTypeDef definition

class UdpOutputSettingsTypeDef(TypedDict):
    ContainerSettings: UdpContainerSettingsTypeDef,  # (1)
    Destination: OutputLocationRefTypeDef,  # (2)
    BufferMsec: NotRequired[int],
    FecOutputSettings: NotRequired[FecOutputSettingsTypeDef],  # (3)
```

1. See [:material-code-braces: UdpContainerSettingsTypeDef](./type_defs.md#udpcontainersettingstypedef) 
2. See [:material-code-braces: OutputLocationRefTypeDef](./type_defs.md#outputlocationreftypedef) 
3. See [:material-code-braces: FecOutputSettingsTypeDef](./type_defs.md#fecoutputsettingstypedef) 
## AutomaticInputFailoverSettingsTypeDef

```python
# AutomaticInputFailoverSettingsTypeDef definition

class AutomaticInputFailoverSettingsTypeDef(TypedDict):
    SecondaryInputId: str,
    ErrorClearTimeMsec: NotRequired[int],
    FailoverConditions: NotRequired[Sequence[FailoverConditionTypeDef]],  # (1)
    InputPreference: NotRequired[InputPreferenceType],  # (2)
```

1. See [:material-code-braces: FailoverConditionTypeDef](./type_defs.md#failoverconditiontypedef) 
2. See [:material-code-brackets: InputPreferenceType](./literals.md#inputpreferencetype) 
## VideoCodecSettingsTypeDef

```python
# VideoCodecSettingsTypeDef definition

class VideoCodecSettingsTypeDef(TypedDict):
    FrameCaptureSettings: NotRequired[FrameCaptureSettingsTypeDef],  # (1)
    H264Settings: NotRequired[H264SettingsTypeDef],  # (2)
    H265Settings: NotRequired[H265SettingsTypeDef],  # (3)
    Mpeg2Settings: NotRequired[Mpeg2SettingsTypeDef],  # (4)
```

1. See [:material-code-braces: FrameCaptureSettingsTypeDef](./type_defs.md#framecapturesettingstypedef) 
2. See [:material-code-braces: H264SettingsTypeDef](./type_defs.md#h264settingstypedef) 
3. See [:material-code-braces: H265SettingsTypeDef](./type_defs.md#h265settingstypedef) 
4. See [:material-code-braces: Mpeg2SettingsTypeDef](./type_defs.md#mpeg2settingstypedef) 
## CreateInputResponseTypeDef

```python
# CreateInputResponseTypeDef definition

class CreateInputResponseTypeDef(TypedDict):
    Input: InputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePartnerInputResponseTypeDef

```python
# CreatePartnerInputResponseTypeDef definition

class CreatePartnerInputResponseTypeDef(TypedDict):
    Input: InputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInputsResponseTypeDef

```python
# ListInputsResponseTypeDef definition

class ListInputsResponseTypeDef(TypedDict):
    Inputs: List[InputTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInputResponseTypeDef

```python
# UpdateInputResponseTypeDef definition

class UpdateInputResponseTypeDef(TypedDict):
    Input: InputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HlsOutputSettingsTypeDef

```python
# HlsOutputSettingsTypeDef definition

class HlsOutputSettingsTypeDef(TypedDict):
    HlsSettings: HlsSettingsTypeDef,  # (2)
    H265PackagingType: NotRequired[HlsH265PackagingTypeType],  # (1)
    NameModifier: NotRequired[str],
    SegmentModifier: NotRequired[str],
```

1. See [:material-code-brackets: HlsH265PackagingTypeType](./literals.md#hlsh265packagingtypetype) 
2. See [:material-code-braces: HlsSettingsTypeDef](./type_defs.md#hlssettingstypedef) 
## CreateMultiplexResponseTypeDef

```python
# CreateMultiplexResponseTypeDef definition

class CreateMultiplexResponseTypeDef(TypedDict):
    Multiplex: MultiplexTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MultiplexTypeDef](./type_defs.md#multiplextypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMultiplexResponseTypeDef

```python
# UpdateMultiplexResponseTypeDef definition

class UpdateMultiplexResponseTypeDef(TypedDict):
    Multiplex: MultiplexTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MultiplexTypeDef](./type_defs.md#multiplextypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMultiplexProgramRequestRequestTypeDef

```python
# CreateMultiplexProgramRequestRequestTypeDef definition

class CreateMultiplexProgramRequestRequestTypeDef(TypedDict):
    MultiplexId: str,
    MultiplexProgramSettings: MultiplexProgramSettingsTypeDef,  # (1)
    ProgramName: str,
    RequestId: str,
```

1. See [:material-code-braces: MultiplexProgramSettingsTypeDef](./type_defs.md#multiplexprogramsettingstypedef) 
## DeleteMultiplexProgramResponseTypeDef

```python
# DeleteMultiplexProgramResponseTypeDef definition

class DeleteMultiplexProgramResponseTypeDef(TypedDict):
    ChannelId: str,
    MultiplexProgramSettings: MultiplexProgramSettingsTypeDef,  # (1)
    PacketIdentifiersMap: MultiplexProgramPacketIdentifiersMapTypeDef,  # (2)
    PipelineDetails: List[MultiplexProgramPipelineDetailTypeDef],  # (3)
    ProgramName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: MultiplexProgramSettingsTypeDef](./type_defs.md#multiplexprogramsettingstypedef) 
2. See [:material-code-braces: MultiplexProgramPacketIdentifiersMapTypeDef](./type_defs.md#multiplexprogrampacketidentifiersmaptypedef) 
3. See [:material-code-braces: MultiplexProgramPipelineDetailTypeDef](./type_defs.md#multiplexprogrampipelinedetailtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMultiplexProgramResponseTypeDef

```python
# DescribeMultiplexProgramResponseTypeDef definition

class DescribeMultiplexProgramResponseTypeDef(TypedDict):
    ChannelId: str,
    MultiplexProgramSettings: MultiplexProgramSettingsTypeDef,  # (1)
    PacketIdentifiersMap: MultiplexProgramPacketIdentifiersMapTypeDef,  # (2)
    PipelineDetails: List[MultiplexProgramPipelineDetailTypeDef],  # (3)
    ProgramName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: MultiplexProgramSettingsTypeDef](./type_defs.md#multiplexprogramsettingstypedef) 
2. See [:material-code-braces: MultiplexProgramPacketIdentifiersMapTypeDef](./type_defs.md#multiplexprogrampacketidentifiersmaptypedef) 
3. See [:material-code-braces: MultiplexProgramPipelineDetailTypeDef](./type_defs.md#multiplexprogrampipelinedetailtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MultiplexProgramTypeDef

```python
# MultiplexProgramTypeDef definition

class MultiplexProgramTypeDef(TypedDict):
    ChannelId: NotRequired[str],
    MultiplexProgramSettings: NotRequired[MultiplexProgramSettingsTypeDef],  # (1)
    PacketIdentifiersMap: NotRequired[MultiplexProgramPacketIdentifiersMapTypeDef],  # (2)
    PipelineDetails: NotRequired[List[MultiplexProgramPipelineDetailTypeDef]],  # (3)
    ProgramName: NotRequired[str],
```

1. See [:material-code-braces: MultiplexProgramSettingsTypeDef](./type_defs.md#multiplexprogramsettingstypedef) 
2. See [:material-code-braces: MultiplexProgramPacketIdentifiersMapTypeDef](./type_defs.md#multiplexprogrampacketidentifiersmaptypedef) 
3. See [:material-code-braces: MultiplexProgramPipelineDetailTypeDef](./type_defs.md#multiplexprogrampipelinedetailtypedef) 
## UpdateMultiplexProgramRequestRequestTypeDef

```python
# UpdateMultiplexProgramRequestRequestTypeDef definition

class UpdateMultiplexProgramRequestRequestTypeDef(TypedDict):
    MultiplexId: str,
    ProgramName: str,
    MultiplexProgramSettings: NotRequired[MultiplexProgramSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: MultiplexProgramSettingsTypeDef](./type_defs.md#multiplexprogramsettingstypedef) 
## AudioDescriptionTypeDef

```python
# AudioDescriptionTypeDef definition

class AudioDescriptionTypeDef(TypedDict):
    AudioSelectorName: str,
    Name: str,
    AudioNormalizationSettings: NotRequired[AudioNormalizationSettingsTypeDef],  # (1)
    AudioType: NotRequired[AudioTypeType],  # (2)
    AudioTypeControl: NotRequired[AudioDescriptionAudioTypeControlType],  # (3)
    AudioWatermarkingSettings: NotRequired[AudioWatermarkSettingsTypeDef],  # (4)
    CodecSettings: NotRequired[AudioCodecSettingsTypeDef],  # (5)
    LanguageCode: NotRequired[str],
    LanguageCodeControl: NotRequired[AudioDescriptionLanguageCodeControlType],  # (6)
    RemixSettings: NotRequired[RemixSettingsTypeDef],  # (7)
    StreamName: NotRequired[str],
```

1. See [:material-code-braces: AudioNormalizationSettingsTypeDef](./type_defs.md#audionormalizationsettingstypedef) 
2. See [:material-code-brackets: AudioTypeType](./literals.md#audiotypetype) 
3. See [:material-code-brackets: AudioDescriptionAudioTypeControlType](./literals.md#audiodescriptionaudiotypecontroltype) 
4. See [:material-code-braces: AudioWatermarkSettingsTypeDef](./type_defs.md#audiowatermarksettingstypedef) 
5. See [:material-code-braces: AudioCodecSettingsTypeDef](./type_defs.md#audiocodecsettingstypedef) 
6. See [:material-code-brackets: AudioDescriptionLanguageCodeControlType](./literals.md#audiodescriptionlanguagecodecontroltype) 
7. See [:material-code-braces: RemixSettingsTypeDef](./type_defs.md#remixsettingstypedef) 
## Scte35DescriptorTypeDef

```python
# Scte35DescriptorTypeDef definition

class Scte35DescriptorTypeDef(TypedDict):
    Scte35DescriptorSettings: Scte35DescriptorSettingsTypeDef,  # (1)
```

1. See [:material-code-braces: Scte35DescriptorSettingsTypeDef](./type_defs.md#scte35descriptorsettingstypedef) 
## OutputGroupSettingsTypeDef

```python
# OutputGroupSettingsTypeDef definition

class OutputGroupSettingsTypeDef(TypedDict):
    ArchiveGroupSettings: NotRequired[ArchiveGroupSettingsTypeDef],  # (1)
    FrameCaptureGroupSettings: NotRequired[FrameCaptureGroupSettingsTypeDef],  # (2)
    HlsGroupSettings: NotRequired[HlsGroupSettingsTypeDef],  # (3)
    MediaPackageGroupSettings: NotRequired[MediaPackageGroupSettingsTypeDef],  # (4)
    MsSmoothGroupSettings: NotRequired[MsSmoothGroupSettingsTypeDef],  # (5)
    MultiplexGroupSettings: NotRequired[Mapping[str, Any]],
    RtmpGroupSettings: NotRequired[RtmpGroupSettingsTypeDef],  # (6)
    UdpGroupSettings: NotRequired[UdpGroupSettingsTypeDef],  # (7)
```

1. See [:material-code-braces: ArchiveGroupSettingsTypeDef](./type_defs.md#archivegroupsettingstypedef) 
2. See [:material-code-braces: FrameCaptureGroupSettingsTypeDef](./type_defs.md#framecapturegroupsettingstypedef) 
3. See [:material-code-braces: HlsGroupSettingsTypeDef](./type_defs.md#hlsgroupsettingstypedef) 
4. See [:material-code-braces: MediaPackageGroupSettingsTypeDef](./type_defs.md#mediapackagegroupsettingstypedef) 
5. See [:material-code-braces: MsSmoothGroupSettingsTypeDef](./type_defs.md#mssmoothgroupsettingstypedef) 
6. See [:material-code-braces: RtmpGroupSettingsTypeDef](./type_defs.md#rtmpgroupsettingstypedef) 
7. See [:material-code-braces: UdpGroupSettingsTypeDef](./type_defs.md#udpgroupsettingstypedef) 
## InputSettingsTypeDef

```python
# InputSettingsTypeDef definition

class InputSettingsTypeDef(TypedDict):
    AudioSelectors: NotRequired[Sequence[AudioSelectorTypeDef]],  # (1)
    CaptionSelectors: NotRequired[Sequence[CaptionSelectorTypeDef]],  # (2)
    DeblockFilter: NotRequired[InputDeblockFilterType],  # (3)
    DenoiseFilter: NotRequired[InputDenoiseFilterType],  # (4)
    FilterStrength: NotRequired[int],
    InputFilter: NotRequired[InputFilterType],  # (5)
    NetworkInputSettings: NotRequired[NetworkInputSettingsTypeDef],  # (6)
    Scte35Pid: NotRequired[int],
    Smpte2038DataPreference: NotRequired[Smpte2038DataPreferenceType],  # (7)
    SourceEndBehavior: NotRequired[InputSourceEndBehaviorType],  # (8)
    VideoSelector: NotRequired[VideoSelectorTypeDef],  # (9)
```

1. See [:material-code-braces: AudioSelectorTypeDef](./type_defs.md#audioselectortypedef) 
2. See [:material-code-braces: CaptionSelectorTypeDef](./type_defs.md#captionselectortypedef) 
3. See [:material-code-brackets: InputDeblockFilterType](./literals.md#inputdeblockfiltertype) 
4. See [:material-code-brackets: InputDenoiseFilterType](./literals.md#inputdenoisefiltertype) 
5. See [:material-code-brackets: InputFilterType](./literals.md#inputfiltertype) 
6. See [:material-code-braces: NetworkInputSettingsTypeDef](./type_defs.md#networkinputsettingstypedef) 
7. See [:material-code-brackets: Smpte2038DataPreferenceType](./literals.md#smpte2038datapreferencetype) 
8. See [:material-code-brackets: InputSourceEndBehaviorType](./literals.md#inputsourceendbehaviortype) 
9. See [:material-code-braces: VideoSelectorTypeDef](./type_defs.md#videoselectortypedef) 
## VideoDescriptionTypeDef

```python
# VideoDescriptionTypeDef definition

class VideoDescriptionTypeDef(TypedDict):
    Name: str,
    CodecSettings: NotRequired[VideoCodecSettingsTypeDef],  # (1)
    Height: NotRequired[int],
    RespondToAfd: NotRequired[VideoDescriptionRespondToAfdType],  # (2)
    ScalingBehavior: NotRequired[VideoDescriptionScalingBehaviorType],  # (3)
    Sharpness: NotRequired[int],
    Width: NotRequired[int],
```

1. See [:material-code-braces: VideoCodecSettingsTypeDef](./type_defs.md#videocodecsettingstypedef) 
2. See [:material-code-brackets: VideoDescriptionRespondToAfdType](./literals.md#videodescriptionrespondtoafdtype) 
3. See [:material-code-brackets: VideoDescriptionScalingBehaviorType](./literals.md#videodescriptionscalingbehaviortype) 
## OutputSettingsTypeDef

```python
# OutputSettingsTypeDef definition

class OutputSettingsTypeDef(TypedDict):
    ArchiveOutputSettings: NotRequired[ArchiveOutputSettingsTypeDef],  # (1)
    FrameCaptureOutputSettings: NotRequired[FrameCaptureOutputSettingsTypeDef],  # (2)
    HlsOutputSettings: NotRequired[HlsOutputSettingsTypeDef],  # (3)
    MediaPackageOutputSettings: NotRequired[Mapping[str, Any]],
    MsSmoothOutputSettings: NotRequired[MsSmoothOutputSettingsTypeDef],  # (4)
    MultiplexOutputSettings: NotRequired[MultiplexOutputSettingsTypeDef],  # (5)
    RtmpOutputSettings: NotRequired[RtmpOutputSettingsTypeDef],  # (6)
    UdpOutputSettings: NotRequired[UdpOutputSettingsTypeDef],  # (7)
```

1. See [:material-code-braces: ArchiveOutputSettingsTypeDef](./type_defs.md#archiveoutputsettingstypedef) 
2. See [:material-code-braces: FrameCaptureOutputSettingsTypeDef](./type_defs.md#framecaptureoutputsettingstypedef) 
3. See [:material-code-braces: HlsOutputSettingsTypeDef](./type_defs.md#hlsoutputsettingstypedef) 
4. See [:material-code-braces: MsSmoothOutputSettingsTypeDef](./type_defs.md#mssmoothoutputsettingstypedef) 
5. See [:material-code-braces: MultiplexOutputSettingsTypeDef](./type_defs.md#multiplexoutputsettingstypedef) 
6. See [:material-code-braces: RtmpOutputSettingsTypeDef](./type_defs.md#rtmpoutputsettingstypedef) 
7. See [:material-code-braces: UdpOutputSettingsTypeDef](./type_defs.md#udpoutputsettingstypedef) 
## CreateMultiplexProgramResponseTypeDef

```python
# CreateMultiplexProgramResponseTypeDef definition

class CreateMultiplexProgramResponseTypeDef(TypedDict):
    MultiplexProgram: MultiplexProgramTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MultiplexProgramTypeDef](./type_defs.md#multiplexprogramtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMultiplexProgramResponseTypeDef

```python
# UpdateMultiplexProgramResponseTypeDef definition

class UpdateMultiplexProgramResponseTypeDef(TypedDict):
    MultiplexProgram: MultiplexProgramTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MultiplexProgramTypeDef](./type_defs.md#multiplexprogramtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## Scte35TimeSignalScheduleActionSettingsTypeDef

```python
# Scte35TimeSignalScheduleActionSettingsTypeDef definition

class Scte35TimeSignalScheduleActionSettingsTypeDef(TypedDict):
    Scte35Descriptors: Sequence[Scte35DescriptorTypeDef],  # (1)
```

1. See [:material-code-braces: Scte35DescriptorTypeDef](./type_defs.md#scte35descriptortypedef) 
## InputAttachmentTypeDef

```python
# InputAttachmentTypeDef definition

class InputAttachmentTypeDef(TypedDict):
    AutomaticInputFailoverSettings: NotRequired[AutomaticInputFailoverSettingsTypeDef],  # (1)
    InputAttachmentName: NotRequired[str],
    InputId: NotRequired[str],
    InputSettings: NotRequired[InputSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: AutomaticInputFailoverSettingsTypeDef](./type_defs.md#automaticinputfailoversettingstypedef) 
2. See [:material-code-braces: InputSettingsTypeDef](./type_defs.md#inputsettingstypedef) 
## OutputTypeDef

```python
# OutputTypeDef definition

class OutputTypeDef(TypedDict):
    OutputSettings: OutputSettingsTypeDef,  # (1)
    AudioDescriptionNames: NotRequired[Sequence[str]],
    CaptionDescriptionNames: NotRequired[Sequence[str]],
    OutputName: NotRequired[str],
    VideoDescriptionName: NotRequired[str],
```

1. See [:material-code-braces: OutputSettingsTypeDef](./type_defs.md#outputsettingstypedef) 
## ScheduleActionSettingsTypeDef

```python
# ScheduleActionSettingsTypeDef definition

class ScheduleActionSettingsTypeDef(TypedDict):
    HlsId3SegmentTaggingSettings: NotRequired[HlsId3SegmentTaggingScheduleActionSettingsTypeDef],  # (1)
    HlsTimedMetadataSettings: NotRequired[HlsTimedMetadataScheduleActionSettingsTypeDef],  # (2)
    InputPrepareSettings: NotRequired[InputPrepareScheduleActionSettingsTypeDef],  # (3)
    InputSwitchSettings: NotRequired[InputSwitchScheduleActionSettingsTypeDef],  # (4)
    MotionGraphicsImageActivateSettings: NotRequired[MotionGraphicsActivateScheduleActionSettingsTypeDef],  # (5)
    MotionGraphicsImageDeactivateSettings: NotRequired[Mapping[str, Any]],
    PauseStateSettings: NotRequired[PauseStateScheduleActionSettingsTypeDef],  # (6)
    Scte35InputSettings: NotRequired[Scte35InputScheduleActionSettingsTypeDef],  # (7)
    Scte35ReturnToNetworkSettings: NotRequired[Scte35ReturnToNetworkScheduleActionSettingsTypeDef],  # (8)
    Scte35SpliceInsertSettings: NotRequired[Scte35SpliceInsertScheduleActionSettingsTypeDef],  # (9)
    Scte35TimeSignalSettings: NotRequired[Scte35TimeSignalScheduleActionSettingsTypeDef],  # (10)
    StaticImageActivateSettings: NotRequired[StaticImageActivateScheduleActionSettingsTypeDef],  # (11)
    StaticImageDeactivateSettings: NotRequired[StaticImageDeactivateScheduleActionSettingsTypeDef],  # (12)
```

1. See [:material-code-braces: HlsId3SegmentTaggingScheduleActionSettingsTypeDef](./type_defs.md#hlsid3segmenttaggingscheduleactionsettingstypedef) 
2. See [:material-code-braces: HlsTimedMetadataScheduleActionSettingsTypeDef](./type_defs.md#hlstimedmetadatascheduleactionsettingstypedef) 
3. See [:material-code-braces: InputPrepareScheduleActionSettingsTypeDef](./type_defs.md#inputpreparescheduleactionsettingstypedef) 
4. See [:material-code-braces: InputSwitchScheduleActionSettingsTypeDef](./type_defs.md#inputswitchscheduleactionsettingstypedef) 
5. See [:material-code-braces: MotionGraphicsActivateScheduleActionSettingsTypeDef](./type_defs.md#motiongraphicsactivatescheduleactionsettingstypedef) 
6. See [:material-code-braces: PauseStateScheduleActionSettingsTypeDef](./type_defs.md#pausestatescheduleactionsettingstypedef) 
7. See [:material-code-braces: Scte35InputScheduleActionSettingsTypeDef](./type_defs.md#scte35inputscheduleactionsettingstypedef) 
8. See [:material-code-braces: Scte35ReturnToNetworkScheduleActionSettingsTypeDef](./type_defs.md#scte35returntonetworkscheduleactionsettingstypedef) 
9. See [:material-code-braces: Scte35SpliceInsertScheduleActionSettingsTypeDef](./type_defs.md#scte35spliceinsertscheduleactionsettingstypedef) 
10. See [:material-code-braces: Scte35TimeSignalScheduleActionSettingsTypeDef](./type_defs.md#scte35timesignalscheduleactionsettingstypedef) 
11. See [:material-code-braces: StaticImageActivateScheduleActionSettingsTypeDef](./type_defs.md#staticimageactivatescheduleactionsettingstypedef) 
12. See [:material-code-braces: StaticImageDeactivateScheduleActionSettingsTypeDef](./type_defs.md#staticimagedeactivatescheduleactionsettingstypedef) 
## ChannelSummaryTypeDef

```python
# ChannelSummaryTypeDef definition

class ChannelSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CdiInputSpecification: NotRequired[CdiInputSpecificationTypeDef],  # (1)
    ChannelClass: NotRequired[ChannelClassType],  # (2)
    Destinations: NotRequired[List[OutputDestinationTypeDef]],  # (3)
    EgressEndpoints: NotRequired[List[ChannelEgressEndpointTypeDef]],  # (4)
    Id: NotRequired[str],
    InputAttachments: NotRequired[List[InputAttachmentTypeDef]],  # (5)
    InputSpecification: NotRequired[InputSpecificationTypeDef],  # (6)
    LogLevel: NotRequired[LogLevelType],  # (7)
    Maintenance: NotRequired[MaintenanceStatusTypeDef],  # (8)
    Name: NotRequired[str],
    PipelinesRunningCount: NotRequired[int],
    RoleArn: NotRequired[str],
    State: NotRequired[ChannelStateType],  # (9)
    Tags: NotRequired[Dict[str, str]],
    Vpc: NotRequired[VpcOutputSettingsDescriptionTypeDef],  # (10)
```

1. See [:material-code-braces: CdiInputSpecificationTypeDef](./type_defs.md#cdiinputspecificationtypedef) 
2. See [:material-code-brackets: ChannelClassType](./literals.md#channelclasstype) 
3. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) 
4. See [:material-code-braces: ChannelEgressEndpointTypeDef](./type_defs.md#channelegressendpointtypedef) 
5. See [:material-code-braces: InputAttachmentTypeDef](./type_defs.md#inputattachmenttypedef) 
6. See [:material-code-braces: InputSpecificationTypeDef](./type_defs.md#inputspecificationtypedef) 
7. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
8. See [:material-code-braces: MaintenanceStatusTypeDef](./type_defs.md#maintenancestatustypedef) 
9. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
10. See [:material-code-braces: VpcOutputSettingsDescriptionTypeDef](./type_defs.md#vpcoutputsettingsdescriptiontypedef) 
## OutputGroupTypeDef

```python
# OutputGroupTypeDef definition

class OutputGroupTypeDef(TypedDict):
    OutputGroupSettings: OutputGroupSettingsTypeDef,  # (1)
    Outputs: Sequence[OutputTypeDef],  # (2)
    Name: NotRequired[str],
```

1. See [:material-code-braces: OutputGroupSettingsTypeDef](./type_defs.md#outputgroupsettingstypedef) 
2. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
## ScheduleActionTypeDef

```python
# ScheduleActionTypeDef definition

class ScheduleActionTypeDef(TypedDict):
    ActionName: str,
    ScheduleActionSettings: ScheduleActionSettingsTypeDef,  # (1)
    ScheduleActionStartSettings: ScheduleActionStartSettingsTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduleActionSettingsTypeDef](./type_defs.md#scheduleactionsettingstypedef) 
2. See [:material-code-braces: ScheduleActionStartSettingsTypeDef](./type_defs.md#scheduleactionstartsettingstypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    Channels: List[ChannelSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelSummaryTypeDef](./type_defs.md#channelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EncoderSettingsTypeDef

```python
# EncoderSettingsTypeDef definition

class EncoderSettingsTypeDef(TypedDict):
    AudioDescriptions: Sequence[AudioDescriptionTypeDef],  # (1)
    OutputGroups: Sequence[OutputGroupTypeDef],  # (10)
    TimecodeConfig: TimecodeConfigTypeDef,  # (11)
    VideoDescriptions: Sequence[VideoDescriptionTypeDef],  # (12)
    AvailBlanking: NotRequired[AvailBlankingTypeDef],  # (2)
    AvailConfiguration: NotRequired[AvailConfigurationTypeDef],  # (3)
    BlackoutSlate: NotRequired[BlackoutSlateTypeDef],  # (4)
    CaptionDescriptions: NotRequired[Sequence[CaptionDescriptionTypeDef]],  # (5)
    FeatureActivations: NotRequired[FeatureActivationsTypeDef],  # (6)
    GlobalConfiguration: NotRequired[GlobalConfigurationTypeDef],  # (7)
    MotionGraphicsConfiguration: NotRequired[MotionGraphicsConfigurationTypeDef],  # (8)
    NielsenConfiguration: NotRequired[NielsenConfigurationTypeDef],  # (9)
    ThumbnailConfiguration: NotRequired[ThumbnailConfigurationTypeDef],  # (13)
```

1. See [:material-code-braces: AudioDescriptionTypeDef](./type_defs.md#audiodescriptiontypedef) 
2. See [:material-code-braces: AvailBlankingTypeDef](./type_defs.md#availblankingtypedef) 
3. See [:material-code-braces: AvailConfigurationTypeDef](./type_defs.md#availconfigurationtypedef) 
4. See [:material-code-braces: BlackoutSlateTypeDef](./type_defs.md#blackoutslatetypedef) 
5. See [:material-code-braces: CaptionDescriptionTypeDef](./type_defs.md#captiondescriptiontypedef) 
6. See [:material-code-braces: FeatureActivationsTypeDef](./type_defs.md#featureactivationstypedef) 
7. See [:material-code-braces: GlobalConfigurationTypeDef](./type_defs.md#globalconfigurationtypedef) 
8. See [:material-code-braces: MotionGraphicsConfigurationTypeDef](./type_defs.md#motiongraphicsconfigurationtypedef) 
9. See [:material-code-braces: NielsenConfigurationTypeDef](./type_defs.md#nielsenconfigurationtypedef) 
10. See [:material-code-braces: OutputGroupTypeDef](./type_defs.md#outputgrouptypedef) 
11. See [:material-code-braces: TimecodeConfigTypeDef](./type_defs.md#timecodeconfigtypedef) 
12. See [:material-code-braces: VideoDescriptionTypeDef](./type_defs.md#videodescriptiontypedef) 
13. See [:material-code-braces: ThumbnailConfigurationTypeDef](./type_defs.md#thumbnailconfigurationtypedef) 
## BatchScheduleActionCreateRequestTypeDef

```python
# BatchScheduleActionCreateRequestTypeDef definition

class BatchScheduleActionCreateRequestTypeDef(TypedDict):
    ScheduleActions: Sequence[ScheduleActionTypeDef],  # (1)
```

1. See [:material-code-braces: ScheduleActionTypeDef](./type_defs.md#scheduleactiontypedef) 
## BatchScheduleActionCreateResultTypeDef

```python
# BatchScheduleActionCreateResultTypeDef definition

class BatchScheduleActionCreateResultTypeDef(TypedDict):
    ScheduleActions: List[ScheduleActionTypeDef],  # (1)
```

1. See [:material-code-braces: ScheduleActionTypeDef](./type_defs.md#scheduleactiontypedef) 
## BatchScheduleActionDeleteResultTypeDef

```python
# BatchScheduleActionDeleteResultTypeDef definition

class BatchScheduleActionDeleteResultTypeDef(TypedDict):
    ScheduleActions: List[ScheduleActionTypeDef],  # (1)
```

1. See [:material-code-braces: ScheduleActionTypeDef](./type_defs.md#scheduleactiontypedef) 
## DescribeScheduleResponseTypeDef

```python
# DescribeScheduleResponseTypeDef definition

class DescribeScheduleResponseTypeDef(TypedDict):
    NextToken: str,
    ScheduleActions: List[ScheduleActionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduleActionTypeDef](./type_defs.md#scheduleactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChannelTypeDef

```python
# ChannelTypeDef definition

class ChannelTypeDef(TypedDict):
    Arn: NotRequired[str],
    CdiInputSpecification: NotRequired[CdiInputSpecificationTypeDef],  # (1)
    ChannelClass: NotRequired[ChannelClassType],  # (2)
    Destinations: NotRequired[List[OutputDestinationTypeDef]],  # (3)
    EgressEndpoints: NotRequired[List[ChannelEgressEndpointTypeDef]],  # (4)
    EncoderSettings: NotRequired[EncoderSettingsTypeDef],  # (5)
    Id: NotRequired[str],
    InputAttachments: NotRequired[List[InputAttachmentTypeDef]],  # (6)
    InputSpecification: NotRequired[InputSpecificationTypeDef],  # (7)
    LogLevel: NotRequired[LogLevelType],  # (8)
    Maintenance: NotRequired[MaintenanceStatusTypeDef],  # (9)
    Name: NotRequired[str],
    PipelineDetails: NotRequired[List[PipelineDetailTypeDef]],  # (10)
    PipelinesRunningCount: NotRequired[int],
    RoleArn: NotRequired[str],
    State: NotRequired[ChannelStateType],  # (11)
    Tags: NotRequired[Dict[str, str]],
    Vpc: NotRequired[VpcOutputSettingsDescriptionTypeDef],  # (12)
```

1. See [:material-code-braces: CdiInputSpecificationTypeDef](./type_defs.md#cdiinputspecificationtypedef) 
2. See [:material-code-brackets: ChannelClassType](./literals.md#channelclasstype) 
3. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) 
4. See [:material-code-braces: ChannelEgressEndpointTypeDef](./type_defs.md#channelegressendpointtypedef) 
5. See [:material-code-braces: EncoderSettingsTypeDef](./type_defs.md#encodersettingstypedef) 
6. See [:material-code-braces: InputAttachmentTypeDef](./type_defs.md#inputattachmenttypedef) 
7. See [:material-code-braces: InputSpecificationTypeDef](./type_defs.md#inputspecificationtypedef) 
8. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
9. See [:material-code-braces: MaintenanceStatusTypeDef](./type_defs.md#maintenancestatustypedef) 
10. See [:material-code-braces: PipelineDetailTypeDef](./type_defs.md#pipelinedetailtypedef) 
11. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
12. See [:material-code-braces: VpcOutputSettingsDescriptionTypeDef](./type_defs.md#vpcoutputsettingsdescriptiontypedef) 
## CreateChannelRequestRequestTypeDef

```python
# CreateChannelRequestRequestTypeDef definition

class CreateChannelRequestRequestTypeDef(TypedDict):
    CdiInputSpecification: NotRequired[CdiInputSpecificationTypeDef],  # (1)
    ChannelClass: NotRequired[ChannelClassType],  # (2)
    Destinations: NotRequired[Sequence[OutputDestinationTypeDef]],  # (3)
    EncoderSettings: NotRequired[EncoderSettingsTypeDef],  # (4)
    InputAttachments: NotRequired[Sequence[InputAttachmentTypeDef]],  # (5)
    InputSpecification: NotRequired[InputSpecificationTypeDef],  # (6)
    LogLevel: NotRequired[LogLevelType],  # (7)
    Maintenance: NotRequired[MaintenanceCreateSettingsTypeDef],  # (8)
    Name: NotRequired[str],
    RequestId: NotRequired[str],
    Reserved: NotRequired[str],
    RoleArn: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    Vpc: NotRequired[VpcOutputSettingsTypeDef],  # (9)
```

1. See [:material-code-braces: CdiInputSpecificationTypeDef](./type_defs.md#cdiinputspecificationtypedef) 
2. See [:material-code-brackets: ChannelClassType](./literals.md#channelclasstype) 
3. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) 
4. See [:material-code-braces: EncoderSettingsTypeDef](./type_defs.md#encodersettingstypedef) 
5. See [:material-code-braces: InputAttachmentTypeDef](./type_defs.md#inputattachmenttypedef) 
6. See [:material-code-braces: InputSpecificationTypeDef](./type_defs.md#inputspecificationtypedef) 
7. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
8. See [:material-code-braces: MaintenanceCreateSettingsTypeDef](./type_defs.md#maintenancecreatesettingstypedef) 
9. See [:material-code-braces: VpcOutputSettingsTypeDef](./type_defs.md#vpcoutputsettingstypedef) 
## DeleteChannelResponseTypeDef

```python
# DeleteChannelResponseTypeDef definition

class DeleteChannelResponseTypeDef(TypedDict):
    Arn: str,
    CdiInputSpecification: CdiInputSpecificationTypeDef,  # (1)
    ChannelClass: ChannelClassType,  # (2)
    Destinations: List[OutputDestinationTypeDef],  # (3)
    EgressEndpoints: List[ChannelEgressEndpointTypeDef],  # (4)
    EncoderSettings: EncoderSettingsTypeDef,  # (5)
    Id: str,
    InputAttachments: List[InputAttachmentTypeDef],  # (6)
    InputSpecification: InputSpecificationTypeDef,  # (7)
    LogLevel: LogLevelType,  # (8)
    Maintenance: MaintenanceStatusTypeDef,  # (9)
    Name: str,
    PipelineDetails: List[PipelineDetailTypeDef],  # (10)
    PipelinesRunningCount: int,
    RoleArn: str,
    State: ChannelStateType,  # (11)
    Tags: Dict[str, str],
    Vpc: VpcOutputSettingsDescriptionTypeDef,  # (12)
    ResponseMetadata: ResponseMetadataTypeDef,  # (13)
```

1. See [:material-code-braces: CdiInputSpecificationTypeDef](./type_defs.md#cdiinputspecificationtypedef) 
2. See [:material-code-brackets: ChannelClassType](./literals.md#channelclasstype) 
3. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) 
4. See [:material-code-braces: ChannelEgressEndpointTypeDef](./type_defs.md#channelegressendpointtypedef) 
5. See [:material-code-braces: EncoderSettingsTypeDef](./type_defs.md#encodersettingstypedef) 
6. See [:material-code-braces: InputAttachmentTypeDef](./type_defs.md#inputattachmenttypedef) 
7. See [:material-code-braces: InputSpecificationTypeDef](./type_defs.md#inputspecificationtypedef) 
8. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
9. See [:material-code-braces: MaintenanceStatusTypeDef](./type_defs.md#maintenancestatustypedef) 
10. See [:material-code-braces: PipelineDetailTypeDef](./type_defs.md#pipelinedetailtypedef) 
11. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
12. See [:material-code-braces: VpcOutputSettingsDescriptionTypeDef](./type_defs.md#vpcoutputsettingsdescriptiontypedef) 
13. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelResponseTypeDef

```python
# DescribeChannelResponseTypeDef definition

class DescribeChannelResponseTypeDef(TypedDict):
    Arn: str,
    CdiInputSpecification: CdiInputSpecificationTypeDef,  # (1)
    ChannelClass: ChannelClassType,  # (2)
    Destinations: List[OutputDestinationTypeDef],  # (3)
    EgressEndpoints: List[ChannelEgressEndpointTypeDef],  # (4)
    EncoderSettings: EncoderSettingsTypeDef,  # (5)
    Id: str,
    InputAttachments: List[InputAttachmentTypeDef],  # (6)
    InputSpecification: InputSpecificationTypeDef,  # (7)
    LogLevel: LogLevelType,  # (8)
    Maintenance: MaintenanceStatusTypeDef,  # (9)
    Name: str,
    PipelineDetails: List[PipelineDetailTypeDef],  # (10)
    PipelinesRunningCount: int,
    RoleArn: str,
    State: ChannelStateType,  # (11)
    Tags: Dict[str, str],
    Vpc: VpcOutputSettingsDescriptionTypeDef,  # (12)
    ResponseMetadata: ResponseMetadataTypeDef,  # (13)
```

1. See [:material-code-braces: CdiInputSpecificationTypeDef](./type_defs.md#cdiinputspecificationtypedef) 
2. See [:material-code-brackets: ChannelClassType](./literals.md#channelclasstype) 
3. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) 
4. See [:material-code-braces: ChannelEgressEndpointTypeDef](./type_defs.md#channelegressendpointtypedef) 
5. See [:material-code-braces: EncoderSettingsTypeDef](./type_defs.md#encodersettingstypedef) 
6. See [:material-code-braces: InputAttachmentTypeDef](./type_defs.md#inputattachmenttypedef) 
7. See [:material-code-braces: InputSpecificationTypeDef](./type_defs.md#inputspecificationtypedef) 
8. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
9. See [:material-code-braces: MaintenanceStatusTypeDef](./type_defs.md#maintenancestatustypedef) 
10. See [:material-code-braces: PipelineDetailTypeDef](./type_defs.md#pipelinedetailtypedef) 
11. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
12. See [:material-code-braces: VpcOutputSettingsDescriptionTypeDef](./type_defs.md#vpcoutputsettingsdescriptiontypedef) 
13. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartChannelResponseTypeDef

```python
# StartChannelResponseTypeDef definition

class StartChannelResponseTypeDef(TypedDict):
    Arn: str,
    CdiInputSpecification: CdiInputSpecificationTypeDef,  # (1)
    ChannelClass: ChannelClassType,  # (2)
    Destinations: List[OutputDestinationTypeDef],  # (3)
    EgressEndpoints: List[ChannelEgressEndpointTypeDef],  # (4)
    EncoderSettings: EncoderSettingsTypeDef,  # (5)
    Id: str,
    InputAttachments: List[InputAttachmentTypeDef],  # (6)
    InputSpecification: InputSpecificationTypeDef,  # (7)
    LogLevel: LogLevelType,  # (8)
    Maintenance: MaintenanceStatusTypeDef,  # (9)
    Name: str,
    PipelineDetails: List[PipelineDetailTypeDef],  # (10)
    PipelinesRunningCount: int,
    RoleArn: str,
    State: ChannelStateType,  # (11)
    Tags: Dict[str, str],
    Vpc: VpcOutputSettingsDescriptionTypeDef,  # (12)
    ResponseMetadata: ResponseMetadataTypeDef,  # (13)
```

1. See [:material-code-braces: CdiInputSpecificationTypeDef](./type_defs.md#cdiinputspecificationtypedef) 
2. See [:material-code-brackets: ChannelClassType](./literals.md#channelclasstype) 
3. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) 
4. See [:material-code-braces: ChannelEgressEndpointTypeDef](./type_defs.md#channelegressendpointtypedef) 
5. See [:material-code-braces: EncoderSettingsTypeDef](./type_defs.md#encodersettingstypedef) 
6. See [:material-code-braces: InputAttachmentTypeDef](./type_defs.md#inputattachmenttypedef) 
7. See [:material-code-braces: InputSpecificationTypeDef](./type_defs.md#inputspecificationtypedef) 
8. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
9. See [:material-code-braces: MaintenanceStatusTypeDef](./type_defs.md#maintenancestatustypedef) 
10. See [:material-code-braces: PipelineDetailTypeDef](./type_defs.md#pipelinedetailtypedef) 
11. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
12. See [:material-code-braces: VpcOutputSettingsDescriptionTypeDef](./type_defs.md#vpcoutputsettingsdescriptiontypedef) 
13. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopChannelResponseTypeDef

```python
# StopChannelResponseTypeDef definition

class StopChannelResponseTypeDef(TypedDict):
    Arn: str,
    CdiInputSpecification: CdiInputSpecificationTypeDef,  # (1)
    ChannelClass: ChannelClassType,  # (2)
    Destinations: List[OutputDestinationTypeDef],  # (3)
    EgressEndpoints: List[ChannelEgressEndpointTypeDef],  # (4)
    EncoderSettings: EncoderSettingsTypeDef,  # (5)
    Id: str,
    InputAttachments: List[InputAttachmentTypeDef],  # (6)
    InputSpecification: InputSpecificationTypeDef,  # (7)
    LogLevel: LogLevelType,  # (8)
    Maintenance: MaintenanceStatusTypeDef,  # (9)
    Name: str,
    PipelineDetails: List[PipelineDetailTypeDef],  # (10)
    PipelinesRunningCount: int,
    RoleArn: str,
    State: ChannelStateType,  # (11)
    Tags: Dict[str, str],
    Vpc: VpcOutputSettingsDescriptionTypeDef,  # (12)
    ResponseMetadata: ResponseMetadataTypeDef,  # (13)
```

1. See [:material-code-braces: CdiInputSpecificationTypeDef](./type_defs.md#cdiinputspecificationtypedef) 
2. See [:material-code-brackets: ChannelClassType](./literals.md#channelclasstype) 
3. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) 
4. See [:material-code-braces: ChannelEgressEndpointTypeDef](./type_defs.md#channelegressendpointtypedef) 
5. See [:material-code-braces: EncoderSettingsTypeDef](./type_defs.md#encodersettingstypedef) 
6. See [:material-code-braces: InputAttachmentTypeDef](./type_defs.md#inputattachmenttypedef) 
7. See [:material-code-braces: InputSpecificationTypeDef](./type_defs.md#inputspecificationtypedef) 
8. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
9. See [:material-code-braces: MaintenanceStatusTypeDef](./type_defs.md#maintenancestatustypedef) 
10. See [:material-code-braces: PipelineDetailTypeDef](./type_defs.md#pipelinedetailtypedef) 
11. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
12. See [:material-code-braces: VpcOutputSettingsDescriptionTypeDef](./type_defs.md#vpcoutputsettingsdescriptiontypedef) 
13. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelRequestRequestTypeDef

```python
# UpdateChannelRequestRequestTypeDef definition

class UpdateChannelRequestRequestTypeDef(TypedDict):
    ChannelId: str,
    CdiInputSpecification: NotRequired[CdiInputSpecificationTypeDef],  # (1)
    Destinations: NotRequired[Sequence[OutputDestinationTypeDef]],  # (2)
    EncoderSettings: NotRequired[EncoderSettingsTypeDef],  # (3)
    InputAttachments: NotRequired[Sequence[InputAttachmentTypeDef]],  # (4)
    InputSpecification: NotRequired[InputSpecificationTypeDef],  # (5)
    LogLevel: NotRequired[LogLevelType],  # (6)
    Maintenance: NotRequired[MaintenanceUpdateSettingsTypeDef],  # (7)
    Name: NotRequired[str],
    RoleArn: NotRequired[str],
```

1. See [:material-code-braces: CdiInputSpecificationTypeDef](./type_defs.md#cdiinputspecificationtypedef) 
2. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) 
3. See [:material-code-braces: EncoderSettingsTypeDef](./type_defs.md#encodersettingstypedef) 
4. See [:material-code-braces: InputAttachmentTypeDef](./type_defs.md#inputattachmenttypedef) 
5. See [:material-code-braces: InputSpecificationTypeDef](./type_defs.md#inputspecificationtypedef) 
6. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
7. See [:material-code-braces: MaintenanceUpdateSettingsTypeDef](./type_defs.md#maintenanceupdatesettingstypedef) 
## BatchUpdateScheduleRequestRequestTypeDef

```python
# BatchUpdateScheduleRequestRequestTypeDef definition

class BatchUpdateScheduleRequestRequestTypeDef(TypedDict):
    ChannelId: str,
    Creates: NotRequired[BatchScheduleActionCreateRequestTypeDef],  # (1)
    Deletes: NotRequired[BatchScheduleActionDeleteRequestTypeDef],  # (2)
```

1. See [:material-code-braces: BatchScheduleActionCreateRequestTypeDef](./type_defs.md#batchscheduleactioncreaterequesttypedef) 
2. See [:material-code-braces: BatchScheduleActionDeleteRequestTypeDef](./type_defs.md#batchscheduleactiondeleterequesttypedef) 
## BatchUpdateScheduleResponseTypeDef

```python
# BatchUpdateScheduleResponseTypeDef definition

class BatchUpdateScheduleResponseTypeDef(TypedDict):
    Creates: BatchScheduleActionCreateResultTypeDef,  # (1)
    Deletes: BatchScheduleActionDeleteResultTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchScheduleActionCreateResultTypeDef](./type_defs.md#batchscheduleactioncreateresulttypedef) 
2. See [:material-code-braces: BatchScheduleActionDeleteResultTypeDef](./type_defs.md#batchscheduleactiondeleteresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelResponseTypeDef

```python
# CreateChannelResponseTypeDef definition

class CreateChannelResponseTypeDef(TypedDict):
    Channel: ChannelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelClassResponseTypeDef

```python
# UpdateChannelClassResponseTypeDef definition

class UpdateChannelClassResponseTypeDef(TypedDict):
    Channel: ChannelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelResponseTypeDef

```python
# UpdateChannelResponseTypeDef definition

class UpdateChannelResponseTypeDef(TypedDict):
    Channel: ChannelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
