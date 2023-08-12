# Type definitions

> [Index](../README.md) > [MediaConvert](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MediaConvert](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
    type annotations stubs module [types-aiobotocore-mediaconvert](https://pypi.org/project/types-aiobotocore-mediaconvert/).



## AacSettingsTypeDef

```python
# AacSettingsTypeDef definition

class AacSettingsTypeDef(TypedDict):
    AudioDescriptionBroadcasterMix: NotRequired[AacAudioDescriptionBroadcasterMixType],  # (1)
    Bitrate: NotRequired[int],
    CodecProfile: NotRequired[AacCodecProfileType],  # (2)
    CodingMode: NotRequired[AacCodingModeType],  # (3)
    RateControlMode: NotRequired[AacRateControlModeType],  # (4)
    RawFormat: NotRequired[AacRawFormatType],  # (5)
    SampleRate: NotRequired[int],
    Specification: NotRequired[AacSpecificationType],  # (6)
    VbrQuality: NotRequired[AacVbrQualityType],  # (7)
```

1. See [:material-code-brackets: AacAudioDescriptionBroadcasterMixType](./literals.md#aacaudiodescriptionbroadcastermixtype) 
2. See [:material-code-brackets: AacCodecProfileType](./literals.md#aaccodecprofiletype) 
3. See [:material-code-brackets: AacCodingModeType](./literals.md#aaccodingmodetype) 
4. See [:material-code-brackets: AacRateControlModeType](./literals.md#aacratecontrolmodetype) 
5. See [:material-code-brackets: AacRawFormatType](./literals.md#aacrawformattype) 
6. See [:material-code-brackets: AacSpecificationType](./literals.md#aacspecificationtype) 
7. See [:material-code-brackets: AacVbrQualityType](./literals.md#aacvbrqualitytype) 
## Ac3SettingsTypeDef

```python
# Ac3SettingsTypeDef definition

class Ac3SettingsTypeDef(TypedDict):
    Bitrate: NotRequired[int],
    BitstreamMode: NotRequired[Ac3BitstreamModeType],  # (1)
    CodingMode: NotRequired[Ac3CodingModeType],  # (2)
    Dialnorm: NotRequired[int],
    DynamicRangeCompressionLine: NotRequired[Ac3DynamicRangeCompressionLineType],  # (3)
    DynamicRangeCompressionProfile: NotRequired[Ac3DynamicRangeCompressionProfileType],  # (4)
    DynamicRangeCompressionRf: NotRequired[Ac3DynamicRangeCompressionRfType],  # (5)
    LfeFilter: NotRequired[Ac3LfeFilterType],  # (6)
    MetadataControl: NotRequired[Ac3MetadataControlType],  # (7)
    SampleRate: NotRequired[int],
```

1. See [:material-code-brackets: Ac3BitstreamModeType](./literals.md#ac3bitstreammodetype) 
2. See [:material-code-brackets: Ac3CodingModeType](./literals.md#ac3codingmodetype) 
3. See [:material-code-brackets: Ac3DynamicRangeCompressionLineType](./literals.md#ac3dynamicrangecompressionlinetype) 
4. See [:material-code-brackets: Ac3DynamicRangeCompressionProfileType](./literals.md#ac3dynamicrangecompressionprofiletype) 
5. See [:material-code-brackets: Ac3DynamicRangeCompressionRfType](./literals.md#ac3dynamicrangecompressionrftype) 
6. See [:material-code-brackets: Ac3LfeFilterType](./literals.md#ac3lfefiltertype) 
7. See [:material-code-brackets: Ac3MetadataControlType](./literals.md#ac3metadatacontroltype) 
## AccelerationSettingsTypeDef

```python
# AccelerationSettingsTypeDef definition

class AccelerationSettingsTypeDef(TypedDict):
    Mode: AccelerationModeType,  # (1)
```

1. See [:material-code-brackets: AccelerationModeType](./literals.md#accelerationmodetype) 
## AdvancedInputFilterSettingsTypeDef

```python
# AdvancedInputFilterSettingsTypeDef definition

class AdvancedInputFilterSettingsTypeDef(TypedDict):
    AddTexture: NotRequired[AdvancedInputFilterAddTextureType],  # (1)
    Sharpening: NotRequired[AdvancedInputFilterSharpenType],  # (2)
```

1. See [:material-code-brackets: AdvancedInputFilterAddTextureType](./literals.md#advancedinputfilteraddtexturetype) 
2. See [:material-code-brackets: AdvancedInputFilterSharpenType](./literals.md#advancedinputfiltersharpentype) 
## AiffSettingsTypeDef

```python
# AiffSettingsTypeDef definition

class AiffSettingsTypeDef(TypedDict):
    BitDepth: NotRequired[int],
    Channels: NotRequired[int],
    SampleRate: NotRequired[int],
```

## AllowedRenditionSizeTypeDef

```python
# AllowedRenditionSizeTypeDef definition

class AllowedRenditionSizeTypeDef(TypedDict):
    Height: NotRequired[int],
    Required: NotRequired[RequiredFlagType],  # (1)
    Width: NotRequired[int],
```

1. See [:material-code-brackets: RequiredFlagType](./literals.md#requiredflagtype) 
## AncillarySourceSettingsTypeDef

```python
# AncillarySourceSettingsTypeDef definition

class AncillarySourceSettingsTypeDef(TypedDict):
    Convert608To708: NotRequired[AncillaryConvert608To708Type],  # (1)
    SourceAncillaryChannelNumber: NotRequired[int],
    TerminateCaptions: NotRequired[AncillaryTerminateCaptionsType],  # (2)
```

1. See [:material-code-brackets: AncillaryConvert608To708Type](./literals.md#ancillaryconvert608to708type) 
2. See [:material-code-brackets: AncillaryTerminateCaptionsType](./literals.md#ancillaryterminatecaptionstype) 
## AssociateCertificateRequestRequestTypeDef

```python
# AssociateCertificateRequestRequestTypeDef definition

class AssociateCertificateRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## AudioChannelTaggingSettingsTypeDef

```python
# AudioChannelTaggingSettingsTypeDef definition

class AudioChannelTaggingSettingsTypeDef(TypedDict):
    ChannelTag: NotRequired[AudioChannelTagType],  # (1)
```

1. See [:material-code-brackets: AudioChannelTagType](./literals.md#audiochanneltagtype) 
## Eac3AtmosSettingsTypeDef

```python
# Eac3AtmosSettingsTypeDef definition

class Eac3AtmosSettingsTypeDef(TypedDict):
    Bitrate: NotRequired[int],
    BitstreamMode: NotRequired[Eac3AtmosBitstreamModeType],  # (1)
    CodingMode: NotRequired[Eac3AtmosCodingModeType],  # (2)
    DialogueIntelligence: NotRequired[Eac3AtmosDialogueIntelligenceType],  # (3)
    DownmixControl: NotRequired[Eac3AtmosDownmixControlType],  # (4)
    DynamicRangeCompressionLine: NotRequired[Eac3AtmosDynamicRangeCompressionLineType],  # (5)
    DynamicRangeCompressionRf: NotRequired[Eac3AtmosDynamicRangeCompressionRfType],  # (6)
    DynamicRangeControl: NotRequired[Eac3AtmosDynamicRangeControlType],  # (7)
    LoRoCenterMixLevel: NotRequired[float],
    LoRoSurroundMixLevel: NotRequired[float],
    LtRtCenterMixLevel: NotRequired[float],
    LtRtSurroundMixLevel: NotRequired[float],
    MeteringMode: NotRequired[Eac3AtmosMeteringModeType],  # (8)
    SampleRate: NotRequired[int],
    SpeechThreshold: NotRequired[int],
    StereoDownmix: NotRequired[Eac3AtmosStereoDownmixType],  # (9)
    SurroundExMode: NotRequired[Eac3AtmosSurroundExModeType],  # (10)
```

1. See [:material-code-brackets: Eac3AtmosBitstreamModeType](./literals.md#eac3atmosbitstreammodetype) 
2. See [:material-code-brackets: Eac3AtmosCodingModeType](./literals.md#eac3atmoscodingmodetype) 
3. See [:material-code-brackets: Eac3AtmosDialogueIntelligenceType](./literals.md#eac3atmosdialogueintelligencetype) 
4. See [:material-code-brackets: Eac3AtmosDownmixControlType](./literals.md#eac3atmosdownmixcontroltype) 
5. See [:material-code-brackets: Eac3AtmosDynamicRangeCompressionLineType](./literals.md#eac3atmosdynamicrangecompressionlinetype) 
6. See [:material-code-brackets: Eac3AtmosDynamicRangeCompressionRfType](./literals.md#eac3atmosdynamicrangecompressionrftype) 
7. See [:material-code-brackets: Eac3AtmosDynamicRangeControlType](./literals.md#eac3atmosdynamicrangecontroltype) 
8. See [:material-code-brackets: Eac3AtmosMeteringModeType](./literals.md#eac3atmosmeteringmodetype) 
9. See [:material-code-brackets: Eac3AtmosStereoDownmixType](./literals.md#eac3atmosstereodownmixtype) 
10. See [:material-code-brackets: Eac3AtmosSurroundExModeType](./literals.md#eac3atmossurroundexmodetype) 
## Eac3SettingsTypeDef

```python
# Eac3SettingsTypeDef definition

class Eac3SettingsTypeDef(TypedDict):
    AttenuationControl: NotRequired[Eac3AttenuationControlType],  # (1)
    Bitrate: NotRequired[int],
    BitstreamMode: NotRequired[Eac3BitstreamModeType],  # (2)
    CodingMode: NotRequired[Eac3CodingModeType],  # (3)
    DcFilter: NotRequired[Eac3DcFilterType],  # (4)
    Dialnorm: NotRequired[int],
    DynamicRangeCompressionLine: NotRequired[Eac3DynamicRangeCompressionLineType],  # (5)
    DynamicRangeCompressionRf: NotRequired[Eac3DynamicRangeCompressionRfType],  # (6)
    LfeControl: NotRequired[Eac3LfeControlType],  # (7)
    LfeFilter: NotRequired[Eac3LfeFilterType],  # (8)
    LoRoCenterMixLevel: NotRequired[float],
    LoRoSurroundMixLevel: NotRequired[float],
    LtRtCenterMixLevel: NotRequired[float],
    LtRtSurroundMixLevel: NotRequired[float],
    MetadataControl: NotRequired[Eac3MetadataControlType],  # (9)
    PassthroughControl: NotRequired[Eac3PassthroughControlType],  # (10)
    PhaseControl: NotRequired[Eac3PhaseControlType],  # (11)
    SampleRate: NotRequired[int],
    StereoDownmix: NotRequired[Eac3StereoDownmixType],  # (12)
    SurroundExMode: NotRequired[Eac3SurroundExModeType],  # (13)
    SurroundMode: NotRequired[Eac3SurroundModeType],  # (14)
```

1. See [:material-code-brackets: Eac3AttenuationControlType](./literals.md#eac3attenuationcontroltype) 
2. See [:material-code-brackets: Eac3BitstreamModeType](./literals.md#eac3bitstreammodetype) 
3. See [:material-code-brackets: Eac3CodingModeType](./literals.md#eac3codingmodetype) 
4. See [:material-code-brackets: Eac3DcFilterType](./literals.md#eac3dcfiltertype) 
5. See [:material-code-brackets: Eac3DynamicRangeCompressionLineType](./literals.md#eac3dynamicrangecompressionlinetype) 
6. See [:material-code-brackets: Eac3DynamicRangeCompressionRfType](./literals.md#eac3dynamicrangecompressionrftype) 
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
    Bitrate: NotRequired[int],
    Channels: NotRequired[int],
    SampleRate: NotRequired[int],
```

## Mp3SettingsTypeDef

```python
# Mp3SettingsTypeDef definition

class Mp3SettingsTypeDef(TypedDict):
    Bitrate: NotRequired[int],
    Channels: NotRequired[int],
    RateControlMode: NotRequired[Mp3RateControlModeType],  # (1)
    SampleRate: NotRequired[int],
    VbrQuality: NotRequired[int],
```

1. See [:material-code-brackets: Mp3RateControlModeType](./literals.md#mp3ratecontrolmodetype) 
## OpusSettingsTypeDef

```python
# OpusSettingsTypeDef definition

class OpusSettingsTypeDef(TypedDict):
    Bitrate: NotRequired[int],
    Channels: NotRequired[int],
    SampleRate: NotRequired[int],
```

## VorbisSettingsTypeDef

```python
# VorbisSettingsTypeDef definition

class VorbisSettingsTypeDef(TypedDict):
    Channels: NotRequired[int],
    SampleRate: NotRequired[int],
    VbrQuality: NotRequired[int],
```

## WavSettingsTypeDef

```python
# WavSettingsTypeDef definition

class WavSettingsTypeDef(TypedDict):
    BitDepth: NotRequired[int],
    Channels: NotRequired[int],
    Format: NotRequired[WavFormatType],  # (1)
    SampleRate: NotRequired[int],
```

1. See [:material-code-brackets: WavFormatType](./literals.md#wavformattype) 
## AudioNormalizationSettingsTypeDef

```python
# AudioNormalizationSettingsTypeDef definition

class AudioNormalizationSettingsTypeDef(TypedDict):
    Algorithm: NotRequired[AudioNormalizationAlgorithmType],  # (1)
    AlgorithmControl: NotRequired[AudioNormalizationAlgorithmControlType],  # (2)
    CorrectionGateLevel: NotRequired[int],
    LoudnessLogging: NotRequired[AudioNormalizationLoudnessLoggingType],  # (3)
    PeakCalculation: NotRequired[AudioNormalizationPeakCalculationType],  # (4)
    TargetLkfs: NotRequired[float],
    TruePeakLimiterThreshold: NotRequired[float],
```

1. See [:material-code-brackets: AudioNormalizationAlgorithmType](./literals.md#audionormalizationalgorithmtype) 
2. See [:material-code-brackets: AudioNormalizationAlgorithmControlType](./literals.md#audionormalizationalgorithmcontroltype) 
3. See [:material-code-brackets: AudioNormalizationLoudnessLoggingType](./literals.md#audionormalizationloudnessloggingtype) 
4. See [:material-code-brackets: AudioNormalizationPeakCalculationType](./literals.md#audionormalizationpeakcalculationtype) 
## AudioSelectorGroupTypeDef

```python
# AudioSelectorGroupTypeDef definition

class AudioSelectorGroupTypeDef(TypedDict):
    AudioSelectorNames: NotRequired[Sequence[str]],
```

## HlsRenditionGroupSettingsTypeDef

```python
# HlsRenditionGroupSettingsTypeDef definition

class HlsRenditionGroupSettingsTypeDef(TypedDict):
    RenditionGroupId: NotRequired[str],
    RenditionLanguageCode: NotRequired[LanguageCodeType],  # (1)
    RenditionName: NotRequired[str],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## ForceIncludeRenditionSizeTypeDef

```python
# ForceIncludeRenditionSizeTypeDef definition

class ForceIncludeRenditionSizeTypeDef(TypedDict):
    Height: NotRequired[int],
    Width: NotRequired[int],
```

## MinBottomRenditionSizeTypeDef

```python
# MinBottomRenditionSizeTypeDef definition

class MinBottomRenditionSizeTypeDef(TypedDict):
    Height: NotRequired[int],
    Width: NotRequired[int],
```

## MinTopRenditionSizeTypeDef

```python
# MinTopRenditionSizeTypeDef definition

class MinTopRenditionSizeTypeDef(TypedDict):
    Height: NotRequired[int],
    Width: NotRequired[int],
```

## Av1QvbrSettingsTypeDef

```python
# Av1QvbrSettingsTypeDef definition

class Av1QvbrSettingsTypeDef(TypedDict):
    QvbrQualityLevel: NotRequired[int],
    QvbrQualityLevelFineTune: NotRequired[float],
```

## AvailBlankingTypeDef

```python
# AvailBlankingTypeDef definition

class AvailBlankingTypeDef(TypedDict):
    AvailBlankingImage: NotRequired[str],
```

## AvcIntraUhdSettingsTypeDef

```python
# AvcIntraUhdSettingsTypeDef definition

class AvcIntraUhdSettingsTypeDef(TypedDict):
    QualityTuningLevel: NotRequired[AvcIntraUhdQualityTuningLevelType],  # (1)
```

1. See [:material-code-brackets: AvcIntraUhdQualityTuningLevelType](./literals.md#avcintrauhdqualitytuningleveltype) 
## BandwidthReductionFilterTypeDef

```python
# BandwidthReductionFilterTypeDef definition

class BandwidthReductionFilterTypeDef(TypedDict):
    Sharpening: NotRequired[BandwidthReductionFilterSharpeningType],  # (1)
    Strength: NotRequired[BandwidthReductionFilterStrengthType],  # (2)
```

1. See [:material-code-brackets: BandwidthReductionFilterSharpeningType](./literals.md#bandwidthreductionfiltersharpeningtype) 
2. See [:material-code-brackets: BandwidthReductionFilterStrengthType](./literals.md#bandwidthreductionfilterstrengthtype) 
## BurninDestinationSettingsTypeDef

```python
# BurninDestinationSettingsTypeDef definition

class BurninDestinationSettingsTypeDef(TypedDict):
    Alignment: NotRequired[BurninSubtitleAlignmentType],  # (1)
    ApplyFontColor: NotRequired[BurninSubtitleApplyFontColorType],  # (2)
    BackgroundColor: NotRequired[BurninSubtitleBackgroundColorType],  # (3)
    BackgroundOpacity: NotRequired[int],
    FallbackFont: NotRequired[BurninSubtitleFallbackFontType],  # (4)
    FontColor: NotRequired[BurninSubtitleFontColorType],  # (5)
    FontOpacity: NotRequired[int],
    FontResolution: NotRequired[int],
    FontScript: NotRequired[FontScriptType],  # (6)
    FontSize: NotRequired[int],
    HexFontColor: NotRequired[str],
    OutlineColor: NotRequired[BurninSubtitleOutlineColorType],  # (7)
    OutlineSize: NotRequired[int],
    ShadowColor: NotRequired[BurninSubtitleShadowColorType],  # (8)
    ShadowOpacity: NotRequired[int],
    ShadowXOffset: NotRequired[int],
    ShadowYOffset: NotRequired[int],
    StylePassthrough: NotRequired[BurnInSubtitleStylePassthroughType],  # (9)
    TeletextSpacing: NotRequired[BurninSubtitleTeletextSpacingType],  # (10)
    XPosition: NotRequired[int],
    YPosition: NotRequired[int],
```

1. See [:material-code-brackets: BurninSubtitleAlignmentType](./literals.md#burninsubtitlealignmenttype) 
2. See [:material-code-brackets: BurninSubtitleApplyFontColorType](./literals.md#burninsubtitleapplyfontcolortype) 
3. See [:material-code-brackets: BurninSubtitleBackgroundColorType](./literals.md#burninsubtitlebackgroundcolortype) 
4. See [:material-code-brackets: BurninSubtitleFallbackFontType](./literals.md#burninsubtitlefallbackfonttype) 
5. See [:material-code-brackets: BurninSubtitleFontColorType](./literals.md#burninsubtitlefontcolortype) 
6. See [:material-code-brackets: FontScriptType](./literals.md#fontscripttype) 
7. See [:material-code-brackets: BurninSubtitleOutlineColorType](./literals.md#burninsubtitleoutlinecolortype) 
8. See [:material-code-brackets: BurninSubtitleShadowColorType](./literals.md#burninsubtitleshadowcolortype) 
9. See [:material-code-brackets: BurnInSubtitleStylePassthroughType](./literals.md#burninsubtitlestylepassthroughtype) 
10. See [:material-code-brackets: BurninSubtitleTeletextSpacingType](./literals.md#burninsubtitleteletextspacingtype) 
## CancelJobRequestRequestTypeDef

```python
# CancelJobRequestRequestTypeDef definition

class CancelJobRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DvbSubDestinationSettingsTypeDef

```python
# DvbSubDestinationSettingsTypeDef definition

class DvbSubDestinationSettingsTypeDef(TypedDict):
    Alignment: NotRequired[DvbSubtitleAlignmentType],  # (1)
    ApplyFontColor: NotRequired[DvbSubtitleApplyFontColorType],  # (2)
    BackgroundColor: NotRequired[DvbSubtitleBackgroundColorType],  # (3)
    BackgroundOpacity: NotRequired[int],
    DdsHandling: NotRequired[DvbddsHandlingType],  # (4)
    DdsXCoordinate: NotRequired[int],
    DdsYCoordinate: NotRequired[int],
    FallbackFont: NotRequired[DvbSubSubtitleFallbackFontType],  # (5)
    FontColor: NotRequired[DvbSubtitleFontColorType],  # (6)
    FontOpacity: NotRequired[int],
    FontResolution: NotRequired[int],
    FontScript: NotRequired[FontScriptType],  # (7)
    FontSize: NotRequired[int],
    Height: NotRequired[int],
    HexFontColor: NotRequired[str],
    OutlineColor: NotRequired[DvbSubtitleOutlineColorType],  # (8)
    OutlineSize: NotRequired[int],
    ShadowColor: NotRequired[DvbSubtitleShadowColorType],  # (9)
    ShadowOpacity: NotRequired[int],
    ShadowXOffset: NotRequired[int],
    ShadowYOffset: NotRequired[int],
    StylePassthrough: NotRequired[DvbSubtitleStylePassthroughType],  # (10)
    SubtitlingType: NotRequired[DvbSubtitlingTypeType],  # (11)
    TeletextSpacing: NotRequired[DvbSubtitleTeletextSpacingType],  # (12)
    Width: NotRequired[int],
    XPosition: NotRequired[int],
    YPosition: NotRequired[int],
```

1. See [:material-code-brackets: DvbSubtitleAlignmentType](./literals.md#dvbsubtitlealignmenttype) 
2. See [:material-code-brackets: DvbSubtitleApplyFontColorType](./literals.md#dvbsubtitleapplyfontcolortype) 
3. See [:material-code-brackets: DvbSubtitleBackgroundColorType](./literals.md#dvbsubtitlebackgroundcolortype) 
4. See [:material-code-brackets: DvbddsHandlingType](./literals.md#dvbddshandlingtype) 
5. See [:material-code-brackets: DvbSubSubtitleFallbackFontType](./literals.md#dvbsubsubtitlefallbackfonttype) 
6. See [:material-code-brackets: DvbSubtitleFontColorType](./literals.md#dvbsubtitlefontcolortype) 
7. See [:material-code-brackets: FontScriptType](./literals.md#fontscripttype) 
8. See [:material-code-brackets: DvbSubtitleOutlineColorType](./literals.md#dvbsubtitleoutlinecolortype) 
9. See [:material-code-brackets: DvbSubtitleShadowColorType](./literals.md#dvbsubtitleshadowcolortype) 
10. See [:material-code-brackets: DvbSubtitleStylePassthroughType](./literals.md#dvbsubtitlestylepassthroughtype) 
11. See [:material-code-brackets: DvbSubtitlingTypeType](./literals.md#dvbsubtitlingtypetype) 
12. See [:material-code-brackets: DvbSubtitleTeletextSpacingType](./literals.md#dvbsubtitleteletextspacingtype) 
## EmbeddedDestinationSettingsTypeDef

```python
# EmbeddedDestinationSettingsTypeDef definition

class EmbeddedDestinationSettingsTypeDef(TypedDict):
    Destination608ChannelNumber: NotRequired[int],
    Destination708ServiceNumber: NotRequired[int],
```

## ImscDestinationSettingsTypeDef

```python
# ImscDestinationSettingsTypeDef definition

class ImscDestinationSettingsTypeDef(TypedDict):
    Accessibility: NotRequired[ImscAccessibilitySubsType],  # (1)
    StylePassthrough: NotRequired[ImscStylePassthroughType],  # (2)
```

1. See [:material-code-brackets: ImscAccessibilitySubsType](./literals.md#imscaccessibilitysubstype) 
2. See [:material-code-brackets: ImscStylePassthroughType](./literals.md#imscstylepassthroughtype) 
## SccDestinationSettingsTypeDef

```python
# SccDestinationSettingsTypeDef definition

class SccDestinationSettingsTypeDef(TypedDict):
    Framerate: NotRequired[SccDestinationFramerateType],  # (1)
```

1. See [:material-code-brackets: SccDestinationFramerateType](./literals.md#sccdestinationframeratetype) 
## SrtDestinationSettingsTypeDef

```python
# SrtDestinationSettingsTypeDef definition

class SrtDestinationSettingsTypeDef(TypedDict):
    StylePassthrough: NotRequired[SrtStylePassthroughType],  # (1)
```

1. See [:material-code-brackets: SrtStylePassthroughType](./literals.md#srtstylepassthroughtype) 
## TeletextDestinationSettingsTypeDef

```python
# TeletextDestinationSettingsTypeDef definition

class TeletextDestinationSettingsTypeDef(TypedDict):
    PageNumber: NotRequired[str],
    PageTypes: NotRequired[Sequence[TeletextPageTypeType]],  # (1)
```

1. See [:material-code-brackets: TeletextPageTypeType](./literals.md#teletextpagetypetype) 
## TtmlDestinationSettingsTypeDef

```python
# TtmlDestinationSettingsTypeDef definition

class TtmlDestinationSettingsTypeDef(TypedDict):
    StylePassthrough: NotRequired[TtmlStylePassthroughType],  # (1)
```

1. See [:material-code-brackets: TtmlStylePassthroughType](./literals.md#ttmlstylepassthroughtype) 
## WebvttDestinationSettingsTypeDef

```python
# WebvttDestinationSettingsTypeDef definition

class WebvttDestinationSettingsTypeDef(TypedDict):
    Accessibility: NotRequired[WebvttAccessibilitySubsType],  # (1)
    StylePassthrough: NotRequired[WebvttStylePassthroughType],  # (2)
```

1. See [:material-code-brackets: WebvttAccessibilitySubsType](./literals.md#webvttaccessibilitysubstype) 
2. See [:material-code-brackets: WebvttStylePassthroughType](./literals.md#webvttstylepassthroughtype) 
## CaptionSourceFramerateTypeDef

```python
# CaptionSourceFramerateTypeDef definition

class CaptionSourceFramerateTypeDef(TypedDict):
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
```

## DvbSubSourceSettingsTypeDef

```python
# DvbSubSourceSettingsTypeDef definition

class DvbSubSourceSettingsTypeDef(TypedDict):
    Pid: NotRequired[int],
```

## EmbeddedSourceSettingsTypeDef

```python
# EmbeddedSourceSettingsTypeDef definition

class EmbeddedSourceSettingsTypeDef(TypedDict):
    Convert608To708: NotRequired[EmbeddedConvert608To708Type],  # (1)
    Source608ChannelNumber: NotRequired[int],
    Source608TrackNumber: NotRequired[int],
    TerminateCaptions: NotRequired[EmbeddedTerminateCaptionsType],  # (2)
```

1. See [:material-code-brackets: EmbeddedConvert608To708Type](./literals.md#embeddedconvert608to708type) 
2. See [:material-code-brackets: EmbeddedTerminateCaptionsType](./literals.md#embeddedterminatecaptionstype) 
## TeletextSourceSettingsTypeDef

```python
# TeletextSourceSettingsTypeDef definition

class TeletextSourceSettingsTypeDef(TypedDict):
    PageNumber: NotRequired[str],
```

## TrackSourceSettingsTypeDef

```python
# TrackSourceSettingsTypeDef definition

class TrackSourceSettingsTypeDef(TypedDict):
    TrackNumber: NotRequired[int],
```

## WebvttHlsSourceSettingsTypeDef

```python
# WebvttHlsSourceSettingsTypeDef definition

class WebvttHlsSourceSettingsTypeDef(TypedDict):
    RenditionGroupId: NotRequired[str],
    RenditionLanguageCode: NotRequired[LanguageCodeType],  # (1)
    RenditionName: NotRequired[str],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## OutputChannelMappingTypeDef

```python
# OutputChannelMappingTypeDef definition

class OutputChannelMappingTypeDef(TypedDict):
    InputChannels: NotRequired[Sequence[int]],
    InputChannelsFineTune: NotRequired[Sequence[float]],
```

## ClipLimitsTypeDef

```python
# ClipLimitsTypeDef definition

class ClipLimitsTypeDef(TypedDict):
    MaximumRGBTolerance: NotRequired[int],
    MaximumYUV: NotRequired[int],
    MinimumRGBTolerance: NotRequired[int],
    MinimumYUV: NotRequired[int],
```

## CmafAdditionalManifestTypeDef

```python
# CmafAdditionalManifestTypeDef definition

class CmafAdditionalManifestTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[Sequence[str]],
```

## SpekeKeyProviderCmafTypeDef

```python
# SpekeKeyProviderCmafTypeDef definition

class SpekeKeyProviderCmafTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    DashSignaledSystemIds: NotRequired[Sequence[str]],
    HlsSignaledSystemIds: NotRequired[Sequence[str]],
    ResourceId: NotRequired[str],
    Url: NotRequired[str],
```

## StaticKeyProviderTypeDef

```python
# StaticKeyProviderTypeDef definition

class StaticKeyProviderTypeDef(TypedDict):
    KeyFormat: NotRequired[str],
    KeyFormatVersions: NotRequired[str],
    StaticKeyValue: NotRequired[str],
    Url: NotRequired[str],
```

## CmafImageBasedTrickPlaySettingsTypeDef

```python
# CmafImageBasedTrickPlaySettingsTypeDef definition

class CmafImageBasedTrickPlaySettingsTypeDef(TypedDict):
    IntervalCadence: NotRequired[CmafIntervalCadenceType],  # (1)
    ThumbnailHeight: NotRequired[int],
    ThumbnailInterval: NotRequired[float],
    ThumbnailWidth: NotRequired[int],
    TileHeight: NotRequired[int],
    TileWidth: NotRequired[int],
```

1. See [:material-code-brackets: CmafIntervalCadenceType](./literals.md#cmafintervalcadencetype) 
## CmfcSettingsTypeDef

```python
# CmfcSettingsTypeDef definition

class CmfcSettingsTypeDef(TypedDict):
    AudioDuration: NotRequired[CmfcAudioDurationType],  # (1)
    AudioGroupId: NotRequired[str],
    AudioRenditionSets: NotRequired[str],
    AudioTrackType: NotRequired[CmfcAudioTrackTypeType],  # (2)
    DescriptiveVideoServiceFlag: NotRequired[CmfcDescriptiveVideoServiceFlagType],  # (3)
    IFrameOnlyManifest: NotRequired[CmfcIFrameOnlyManifestType],  # (4)
    KlvMetadata: NotRequired[CmfcKlvMetadataType],  # (5)
    ManifestMetadataSignaling: NotRequired[CmfcManifestMetadataSignalingType],  # (6)
    Scte35Esam: NotRequired[CmfcScte35EsamType],  # (7)
    Scte35Source: NotRequired[CmfcScte35SourceType],  # (8)
    TimedMetadata: NotRequired[CmfcTimedMetadataType],  # (9)
    TimedMetadataBoxVersion: NotRequired[CmfcTimedMetadataBoxVersionType],  # (10)
    TimedMetadataSchemeIdUri: NotRequired[str],
    TimedMetadataValue: NotRequired[str],
```

1. See [:material-code-brackets: CmfcAudioDurationType](./literals.md#cmfcaudiodurationtype) 
2. See [:material-code-brackets: CmfcAudioTrackTypeType](./literals.md#cmfcaudiotracktypetype) 
3. See [:material-code-brackets: CmfcDescriptiveVideoServiceFlagType](./literals.md#cmfcdescriptivevideoserviceflagtype) 
4. See [:material-code-brackets: CmfcIFrameOnlyManifestType](./literals.md#cmfciframeonlymanifesttype) 
5. See [:material-code-brackets: CmfcKlvMetadataType](./literals.md#cmfcklvmetadatatype) 
6. See [:material-code-brackets: CmfcManifestMetadataSignalingType](./literals.md#cmfcmanifestmetadatasignalingtype) 
7. See [:material-code-brackets: CmfcScte35EsamType](./literals.md#cmfcscte35esamtype) 
8. See [:material-code-brackets: CmfcScte35SourceType](./literals.md#cmfcscte35sourcetype) 
9. See [:material-code-brackets: CmfcTimedMetadataType](./literals.md#cmfctimedmetadatatype) 
10. See [:material-code-brackets: CmfcTimedMetadataBoxVersionType](./literals.md#cmfctimedmetadataboxversiontype) 
## Hdr10MetadataTypeDef

```python
# Hdr10MetadataTypeDef definition

class Hdr10MetadataTypeDef(TypedDict):
    BluePrimaryX: NotRequired[int],
    BluePrimaryY: NotRequired[int],
    GreenPrimaryX: NotRequired[int],
    GreenPrimaryY: NotRequired[int],
    MaxContentLightLevel: NotRequired[int],
    MaxFrameAverageLightLevel: NotRequired[int],
    MaxLuminance: NotRequired[int],
    MinLuminance: NotRequired[int],
    RedPrimaryX: NotRequired[int],
    RedPrimaryY: NotRequired[int],
    WhitePointX: NotRequired[int],
    WhitePointY: NotRequired[int],
```

## F4vSettingsTypeDef

```python
# F4vSettingsTypeDef definition

class F4vSettingsTypeDef(TypedDict):
    MoovPlacement: NotRequired[F4vMoovPlacementType],  # (1)
```

1. See [:material-code-brackets: F4vMoovPlacementType](./literals.md#f4vmoovplacementtype) 
## M3u8SettingsTypeDef

```python
# M3u8SettingsTypeDef definition

class M3u8SettingsTypeDef(TypedDict):
    AudioDuration: NotRequired[M3u8AudioDurationType],  # (1)
    AudioFramesPerPes: NotRequired[int],
    AudioPids: NotRequired[Sequence[int]],
    DataPTSControl: NotRequired[M3u8DataPtsControlType],  # (2)
    MaxPcrInterval: NotRequired[int],
    NielsenId3: NotRequired[M3u8NielsenId3Type],  # (3)
    PatInterval: NotRequired[int],
    PcrControl: NotRequired[M3u8PcrControlType],  # (4)
    PcrPid: NotRequired[int],
    PmtInterval: NotRequired[int],
    PmtPid: NotRequired[int],
    PrivateMetadataPid: NotRequired[int],
    ProgramNumber: NotRequired[int],
    Scte35Pid: NotRequired[int],
    Scte35Source: NotRequired[M3u8Scte35SourceType],  # (5)
    TimedMetadata: NotRequired[TimedMetadataType],  # (6)
    TimedMetadataPid: NotRequired[int],
    TransportStreamId: NotRequired[int],
    VideoPid: NotRequired[int],
```

1. See [:material-code-brackets: M3u8AudioDurationType](./literals.md#m3u8audiodurationtype) 
2. See [:material-code-brackets: M3u8DataPtsControlType](./literals.md#m3u8dataptscontroltype) 
3. See [:material-code-brackets: M3u8NielsenId3Type](./literals.md#m3u8nielsenid3type) 
4. See [:material-code-brackets: M3u8PcrControlType](./literals.md#m3u8pcrcontroltype) 
5. See [:material-code-brackets: M3u8Scte35SourceType](./literals.md#m3u8scte35sourcetype) 
6. See [:material-code-brackets: TimedMetadataType](./literals.md#timedmetadatatype) 
## MovSettingsTypeDef

```python
# MovSettingsTypeDef definition

class MovSettingsTypeDef(TypedDict):
    ClapAtom: NotRequired[MovClapAtomType],  # (1)
    CslgAtom: NotRequired[MovCslgAtomType],  # (2)
    Mpeg2FourCCControl: NotRequired[MovMpeg2FourCCControlType],  # (3)
    PaddingControl: NotRequired[MovPaddingControlType],  # (4)
    Reference: NotRequired[MovReferenceType],  # (5)
```

1. See [:material-code-brackets: MovClapAtomType](./literals.md#movclapatomtype) 
2. See [:material-code-brackets: MovCslgAtomType](./literals.md#movcslgatomtype) 
3. See [:material-code-brackets: MovMpeg2FourCCControlType](./literals.md#movmpeg2fourcccontroltype) 
4. See [:material-code-brackets: MovPaddingControlType](./literals.md#movpaddingcontroltype) 
5. See [:material-code-brackets: MovReferenceType](./literals.md#movreferencetype) 
## Mp4SettingsTypeDef

```python
# Mp4SettingsTypeDef definition

class Mp4SettingsTypeDef(TypedDict):
    AudioDuration: NotRequired[CmfcAudioDurationType],  # (1)
    CslgAtom: NotRequired[Mp4CslgAtomType],  # (2)
    CttsVersion: NotRequired[int],
    FreeSpaceBox: NotRequired[Mp4FreeSpaceBoxType],  # (3)
    MoovPlacement: NotRequired[Mp4MoovPlacementType],  # (4)
    Mp4MajorBrand: NotRequired[str],
```

1. See [:material-code-brackets: CmfcAudioDurationType](./literals.md#cmfcaudiodurationtype) 
2. See [:material-code-brackets: Mp4CslgAtomType](./literals.md#mp4cslgatomtype) 
3. See [:material-code-brackets: Mp4FreeSpaceBoxType](./literals.md#mp4freespaceboxtype) 
4. See [:material-code-brackets: Mp4MoovPlacementType](./literals.md#mp4moovplacementtype) 
## MpdSettingsTypeDef

```python
# MpdSettingsTypeDef definition

class MpdSettingsTypeDef(TypedDict):
    AccessibilityCaptionHints: NotRequired[MpdAccessibilityCaptionHintsType],  # (1)
    AudioDuration: NotRequired[MpdAudioDurationType],  # (2)
    CaptionContainerType: NotRequired[MpdCaptionContainerTypeType],  # (3)
    KlvMetadata: NotRequired[MpdKlvMetadataType],  # (4)
    ManifestMetadataSignaling: NotRequired[MpdManifestMetadataSignalingType],  # (5)
    Scte35Esam: NotRequired[MpdScte35EsamType],  # (6)
    Scte35Source: NotRequired[MpdScte35SourceType],  # (7)
    TimedMetadata: NotRequired[MpdTimedMetadataType],  # (8)
    TimedMetadataBoxVersion: NotRequired[MpdTimedMetadataBoxVersionType],  # (9)
    TimedMetadataSchemeIdUri: NotRequired[str],
    TimedMetadataValue: NotRequired[str],
```

1. See [:material-code-brackets: MpdAccessibilityCaptionHintsType](./literals.md#mpdaccessibilitycaptionhintstype) 
2. See [:material-code-brackets: MpdAudioDurationType](./literals.md#mpdaudiodurationtype) 
3. See [:material-code-brackets: MpdCaptionContainerTypeType](./literals.md#mpdcaptioncontainertypetype) 
4. See [:material-code-brackets: MpdKlvMetadataType](./literals.md#mpdklvmetadatatype) 
5. See [:material-code-brackets: MpdManifestMetadataSignalingType](./literals.md#mpdmanifestmetadatasignalingtype) 
6. See [:material-code-brackets: MpdScte35EsamType](./literals.md#mpdscte35esamtype) 
7. See [:material-code-brackets: MpdScte35SourceType](./literals.md#mpdscte35sourcetype) 
8. See [:material-code-brackets: MpdTimedMetadataType](./literals.md#mpdtimedmetadatatype) 
9. See [:material-code-brackets: MpdTimedMetadataBoxVersionType](./literals.md#mpdtimedmetadataboxversiontype) 
## HopDestinationTypeDef

```python
# HopDestinationTypeDef definition

class HopDestinationTypeDef(TypedDict):
    Priority: NotRequired[int],
    Queue: NotRequired[str],
    WaitMinutes: NotRequired[int],
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

## ReservationPlanSettingsTypeDef

```python
# ReservationPlanSettingsTypeDef definition

class ReservationPlanSettingsTypeDef(TypedDict):
    Commitment: CommitmentType,  # (1)
    RenewalType: RenewalTypeType,  # (2)
    ReservedSlots: int,
```

1. See [:material-code-brackets: CommitmentType](./literals.md#commitmenttype) 
2. See [:material-code-brackets: RenewalTypeType](./literals.md#renewaltypetype) 
## DashAdditionalManifestTypeDef

```python
# DashAdditionalManifestTypeDef definition

class DashAdditionalManifestTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[Sequence[str]],
```

## SpekeKeyProviderTypeDef

```python
# SpekeKeyProviderTypeDef definition

class SpekeKeyProviderTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    ResourceId: NotRequired[str],
    SystemIds: NotRequired[Sequence[str]],
    Url: NotRequired[str],
```

## DashIsoImageBasedTrickPlaySettingsTypeDef

```python
# DashIsoImageBasedTrickPlaySettingsTypeDef definition

class DashIsoImageBasedTrickPlaySettingsTypeDef(TypedDict):
    IntervalCadence: NotRequired[DashIsoIntervalCadenceType],  # (1)
    ThumbnailHeight: NotRequired[int],
    ThumbnailInterval: NotRequired[float],
    ThumbnailWidth: NotRequired[int],
    TileHeight: NotRequired[int],
    TileWidth: NotRequired[int],
```

1. See [:material-code-brackets: DashIsoIntervalCadenceType](./literals.md#dashisointervalcadencetype) 
## DeinterlacerTypeDef

```python
# DeinterlacerTypeDef definition

class DeinterlacerTypeDef(TypedDict):
    Algorithm: NotRequired[DeinterlaceAlgorithmType],  # (1)
    Control: NotRequired[DeinterlacerControlType],  # (2)
    Mode: NotRequired[DeinterlacerModeType],  # (3)
```

1. See [:material-code-brackets: DeinterlaceAlgorithmType](./literals.md#deinterlacealgorithmtype) 
2. See [:material-code-brackets: DeinterlacerControlType](./literals.md#deinterlacercontroltype) 
3. See [:material-code-brackets: DeinterlacerModeType](./literals.md#deinterlacermodetype) 
## DeleteJobTemplateRequestRequestTypeDef

```python
# DeleteJobTemplateRequestRequestTypeDef definition

class DeleteJobTemplateRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeletePresetRequestRequestTypeDef

```python
# DeletePresetRequestRequestTypeDef definition

class DeletePresetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteQueueRequestRequestTypeDef

```python
# DeleteQueueRequestRequestTypeDef definition

class DeleteQueueRequestRequestTypeDef(TypedDict):
    Name: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeEndpointsRequestRequestTypeDef

```python
# DescribeEndpointsRequestRequestTypeDef definition

class DescribeEndpointsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    Mode: NotRequired[DescribeEndpointsModeType],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: DescribeEndpointsModeType](./literals.md#describeendpointsmodetype) 
## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Url: NotRequired[str],
```

## DisassociateCertificateRequestRequestTypeDef

```python
# DisassociateCertificateRequestRequestTypeDef definition

class DisassociateCertificateRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## DolbyVisionLevel6MetadataTypeDef

```python
# DolbyVisionLevel6MetadataTypeDef definition

class DolbyVisionLevel6MetadataTypeDef(TypedDict):
    MaxCll: NotRequired[int],
    MaxFall: NotRequired[int],
```

## DvbNitSettingsTypeDef

```python
# DvbNitSettingsTypeDef definition

class DvbNitSettingsTypeDef(TypedDict):
    NetworkId: NotRequired[int],
    NetworkName: NotRequired[str],
    NitInterval: NotRequired[int],
```

## DvbSdtSettingsTypeDef

```python
# DvbSdtSettingsTypeDef definition

class DvbSdtSettingsTypeDef(TypedDict):
    OutputSdt: NotRequired[OutputSdtType],  # (1)
    SdtInterval: NotRequired[int],
    ServiceName: NotRequired[str],
    ServiceProviderName: NotRequired[str],
```

1. See [:material-code-brackets: OutputSdtType](./literals.md#outputsdttype) 
## DvbTdtSettingsTypeDef

```python
# DvbTdtSettingsTypeDef definition

class DvbTdtSettingsTypeDef(TypedDict):
    TdtInterval: NotRequired[int],
```

## EsamManifestConfirmConditionNotificationTypeDef

```python
# EsamManifestConfirmConditionNotificationTypeDef definition

class EsamManifestConfirmConditionNotificationTypeDef(TypedDict):
    MccXml: NotRequired[str],
```

## EsamSignalProcessingNotificationTypeDef

```python
# EsamSignalProcessingNotificationTypeDef definition

class EsamSignalProcessingNotificationTypeDef(TypedDict):
    SccXml: NotRequired[str],
```

## ExtendedDataServicesTypeDef

```python
# ExtendedDataServicesTypeDef definition

class ExtendedDataServicesTypeDef(TypedDict):
    CopyProtectionAction: NotRequired[CopyProtectionActionType],  # (1)
    VchipAction: NotRequired[VchipActionType],  # (2)
```

1. See [:material-code-brackets: CopyProtectionActionType](./literals.md#copyprotectionactiontype) 
2. See [:material-code-brackets: VchipActionType](./literals.md#vchipactiontype) 
## FrameCaptureSettingsTypeDef

```python
# FrameCaptureSettingsTypeDef definition

class FrameCaptureSettingsTypeDef(TypedDict):
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    MaxCaptures: NotRequired[int],
    Quality: NotRequired[int],
```

## GetJobRequestRequestTypeDef

```python
# GetJobRequestRequestTypeDef definition

class GetJobRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetJobTemplateRequestRequestTypeDef

```python
# GetJobTemplateRequestRequestTypeDef definition

class GetJobTemplateRequestRequestTypeDef(TypedDict):
    Name: str,
```

## PolicyTypeDef

```python
# PolicyTypeDef definition

class PolicyTypeDef(TypedDict):
    HttpInputs: NotRequired[InputPolicyType],  # (1)
    HttpsInputs: NotRequired[InputPolicyType],  # (1)
    S3Inputs: NotRequired[InputPolicyType],  # (1)
```

1. See [:material-code-brackets: InputPolicyType](./literals.md#inputpolicytype) 
2. See [:material-code-brackets: InputPolicyType](./literals.md#inputpolicytype) 
3. See [:material-code-brackets: InputPolicyType](./literals.md#inputpolicytype) 
## GetPresetRequestRequestTypeDef

```python
# GetPresetRequestRequestTypeDef definition

class GetPresetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetQueueRequestRequestTypeDef

```python
# GetQueueRequestRequestTypeDef definition

class GetQueueRequestRequestTypeDef(TypedDict):
    Name: str,
```

## H264QvbrSettingsTypeDef

```python
# H264QvbrSettingsTypeDef definition

class H264QvbrSettingsTypeDef(TypedDict):
    MaxAverageBitrate: NotRequired[int],
    QvbrQualityLevel: NotRequired[int],
    QvbrQualityLevelFineTune: NotRequired[float],
```

## H265QvbrSettingsTypeDef

```python
# H265QvbrSettingsTypeDef definition

class H265QvbrSettingsTypeDef(TypedDict):
    MaxAverageBitrate: NotRequired[int],
    QvbrQualityLevel: NotRequired[int],
    QvbrQualityLevelFineTune: NotRequired[float],
```

## Hdr10PlusTypeDef

```python
# Hdr10PlusTypeDef definition

class Hdr10PlusTypeDef(TypedDict):
    MasteringMonitorNits: NotRequired[int],
    TargetMonitorNits: NotRequired[int],
```

## HlsAdditionalManifestTypeDef

```python
# HlsAdditionalManifestTypeDef definition

class HlsAdditionalManifestTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[Sequence[str]],
```

## HlsCaptionLanguageMappingTypeDef

```python
# HlsCaptionLanguageMappingTypeDef definition

class HlsCaptionLanguageMappingTypeDef(TypedDict):
    CaptionChannel: NotRequired[int],
    CustomLanguageCode: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    LanguageDescription: NotRequired[str],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## HlsImageBasedTrickPlaySettingsTypeDef

```python
# HlsImageBasedTrickPlaySettingsTypeDef definition

class HlsImageBasedTrickPlaySettingsTypeDef(TypedDict):
    IntervalCadence: NotRequired[HlsIntervalCadenceType],  # (1)
    ThumbnailHeight: NotRequired[int],
    ThumbnailInterval: NotRequired[float],
    ThumbnailWidth: NotRequired[int],
    TileHeight: NotRequired[int],
    TileWidth: NotRequired[int],
```

1. See [:material-code-brackets: HlsIntervalCadenceType](./literals.md#hlsintervalcadencetype) 
## HlsSettingsTypeDef

```python
# HlsSettingsTypeDef definition

class HlsSettingsTypeDef(TypedDict):
    AudioGroupId: NotRequired[str],
    AudioOnlyContainer: NotRequired[HlsAudioOnlyContainerType],  # (1)
    AudioRenditionSets: NotRequired[str],
    AudioTrackType: NotRequired[HlsAudioTrackTypeType],  # (2)
    DescriptiveVideoServiceFlag: NotRequired[HlsDescriptiveVideoServiceFlagType],  # (3)
    IFrameOnlyManifest: NotRequired[HlsIFrameOnlyManifestType],  # (4)
    SegmentModifier: NotRequired[str],
```

1. See [:material-code-brackets: HlsAudioOnlyContainerType](./literals.md#hlsaudioonlycontainertype) 
2. See [:material-code-brackets: HlsAudioTrackTypeType](./literals.md#hlsaudiotracktypetype) 
3. See [:material-code-brackets: HlsDescriptiveVideoServiceFlagType](./literals.md#hlsdescriptivevideoserviceflagtype) 
4. See [:material-code-brackets: HlsIFrameOnlyManifestType](./literals.md#hlsiframeonlymanifesttype) 
## Id3InsertionTypeDef

```python
# Id3InsertionTypeDef definition

class Id3InsertionTypeDef(TypedDict):
    Id3: NotRequired[str],
    Timecode: NotRequired[str],
```

## InsertableImageTypeDef

```python
# InsertableImageTypeDef definition

class InsertableImageTypeDef(TypedDict):
    Duration: NotRequired[int],
    FadeIn: NotRequired[int],
    FadeOut: NotRequired[int],
    Height: NotRequired[int],
    ImageInserterInput: NotRequired[str],
    ImageX: NotRequired[int],
    ImageY: NotRequired[int],
    Layer: NotRequired[int],
    Opacity: NotRequired[int],
    StartTime: NotRequired[str],
    Width: NotRequired[int],
```

## InputClippingTypeDef

```python
# InputClippingTypeDef definition

class InputClippingTypeDef(TypedDict):
    EndTimecode: NotRequired[str],
    StartTimecode: NotRequired[str],
```

## InputDecryptionSettingsTypeDef

```python
# InputDecryptionSettingsTypeDef definition

class InputDecryptionSettingsTypeDef(TypedDict):
    DecryptionMode: NotRequired[DecryptionModeType],  # (1)
    EncryptedDecryptionKey: NotRequired[str],
    InitializationVector: NotRequired[str],
    KmsKeyRegion: NotRequired[str],
```

1. See [:material-code-brackets: DecryptionModeType](./literals.md#decryptionmodetype) 
## RectangleTypeDef

```python
# RectangleTypeDef definition

class RectangleTypeDef(TypedDict):
    Height: NotRequired[int],
    Width: NotRequired[int],
    X: NotRequired[int],
    Y: NotRequired[int],
```

## InputVideoGeneratorTypeDef

```python
# InputVideoGeneratorTypeDef definition

class InputVideoGeneratorTypeDef(TypedDict):
    Duration: NotRequired[int],
```

## JobMessagesTypeDef

```python
# JobMessagesTypeDef definition

class JobMessagesTypeDef(TypedDict):
    Info: NotRequired[List[str]],
    Warning: NotRequired[List[str]],
```

## KantarWatermarkSettingsTypeDef

```python
# KantarWatermarkSettingsTypeDef definition

class KantarWatermarkSettingsTypeDef(TypedDict):
    ChannelName: NotRequired[str],
    ContentReference: NotRequired[str],
    CredentialsSecretName: NotRequired[str],
    FileOffset: NotRequired[float],
    KantarLicenseId: NotRequired[int],
    KantarServerUrl: NotRequired[str],
    LogDestination: NotRequired[str],
    Metadata3: NotRequired[str],
    Metadata4: NotRequired[str],
    Metadata5: NotRequired[str],
    Metadata6: NotRequired[str],
    Metadata7: NotRequired[str],
    Metadata8: NotRequired[str],
```

## NielsenConfigurationTypeDef

```python
# NielsenConfigurationTypeDef definition

class NielsenConfigurationTypeDef(TypedDict):
    BreakoutCode: NotRequired[int],
    DistributorId: NotRequired[str],
```

## NielsenNonLinearWatermarkSettingsTypeDef

```python
# NielsenNonLinearWatermarkSettingsTypeDef definition

class NielsenNonLinearWatermarkSettingsTypeDef(TypedDict):
    ActiveWatermarkProcess: NotRequired[NielsenActiveWatermarkProcessTypeType],  # (1)
    AdiFilename: NotRequired[str],
    AssetId: NotRequired[str],
    AssetName: NotRequired[str],
    CbetSourceId: NotRequired[str],
    EpisodeId: NotRequired[str],
    MetadataDestination: NotRequired[str],
    SourceId: NotRequired[int],
    SourceWatermarkStatus: NotRequired[NielsenSourceWatermarkStatusTypeType],  # (2)
    TicServerUrl: NotRequired[str],
    UniqueTicPerAudioTrack: NotRequired[NielsenUniqueTicPerAudioTrackTypeType],  # (3)
```

1. See [:material-code-brackets: NielsenActiveWatermarkProcessTypeType](./literals.md#nielsenactivewatermarkprocesstypetype) 
2. See [:material-code-brackets: NielsenSourceWatermarkStatusTypeType](./literals.md#nielsensourcewatermarkstatustypetype) 
3. See [:material-code-brackets: NielsenUniqueTicPerAudioTrackTypeType](./literals.md#nielsenuniqueticperaudiotracktypetype) 
## TimecodeConfigTypeDef

```python
# TimecodeConfigTypeDef definition

class TimecodeConfigTypeDef(TypedDict):
    Anchor: NotRequired[str],
    Source: NotRequired[TimecodeSourceType],  # (1)
    Start: NotRequired[str],
    TimestampOffset: NotRequired[str],
```

1. See [:material-code-brackets: TimecodeSourceType](./literals.md#timecodesourcetype) 
## QueueTransitionTypeDef

```python
# QueueTransitionTypeDef definition

class QueueTransitionTypeDef(TypedDict):
    DestinationQueue: NotRequired[str],
    SourceQueue: NotRequired[str],
    Timestamp: NotRequired[datetime],
```

## TimingTypeDef

```python
# TimingTypeDef definition

class TimingTypeDef(TypedDict):
    FinishTime: NotRequired[datetime],
    StartTime: NotRequired[datetime],
    SubmitTime: NotRequired[datetime],
```

## WarningGroupTypeDef

```python
# WarningGroupTypeDef definition

class WarningGroupTypeDef(TypedDict):
    Code: int,
    Count: int,
```

## ListJobTemplatesRequestRequestTypeDef

```python
# ListJobTemplatesRequestRequestTypeDef definition

class ListJobTemplatesRequestRequestTypeDef(TypedDict):
    Category: NotRequired[str],
    ListBy: NotRequired[JobTemplateListByType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Order: NotRequired[OrderType],  # (2)
```

1. See [:material-code-brackets: JobTemplateListByType](./literals.md#jobtemplatelistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## ListJobsRequestRequestTypeDef

```python
# ListJobsRequestRequestTypeDef definition

class ListJobsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Order: NotRequired[OrderType],  # (1)
    Queue: NotRequired[str],
    Status: NotRequired[JobStatusType],  # (2)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## ListPresetsRequestRequestTypeDef

```python
# ListPresetsRequestRequestTypeDef definition

class ListPresetsRequestRequestTypeDef(TypedDict):
    Category: NotRequired[str],
    ListBy: NotRequired[PresetListByType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Order: NotRequired[OrderType],  # (2)
```

1. See [:material-code-brackets: PresetListByType](./literals.md#presetlistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## ListQueuesRequestRequestTypeDef

```python
# ListQueuesRequestRequestTypeDef definition

class ListQueuesRequestRequestTypeDef(TypedDict):
    ListBy: NotRequired[QueueListByType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Order: NotRequired[OrderType],  # (2)
```

1. See [:material-code-brackets: QueueListByType](./literals.md#queuelistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## ResourceTagsTypeDef

```python
# ResourceTagsTypeDef definition

class ResourceTagsTypeDef(TypedDict):
    Arn: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

## M2tsScte35EsamTypeDef

```python
# M2tsScte35EsamTypeDef definition

class M2tsScte35EsamTypeDef(TypedDict):
    Scte35EsamPid: NotRequired[int],
```

## MotionImageInsertionFramerateTypeDef

```python
# MotionImageInsertionFramerateTypeDef definition

class MotionImageInsertionFramerateTypeDef(TypedDict):
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
```

## MotionImageInsertionOffsetTypeDef

```python
# MotionImageInsertionOffsetTypeDef definition

class MotionImageInsertionOffsetTypeDef(TypedDict):
    ImageX: NotRequired[int],
    ImageY: NotRequired[int],
```

## Mpeg2SettingsTypeDef

```python
# Mpeg2SettingsTypeDef definition

class Mpeg2SettingsTypeDef(TypedDict):
    AdaptiveQuantization: NotRequired[Mpeg2AdaptiveQuantizationType],  # (1)
    Bitrate: NotRequired[int],
    CodecLevel: NotRequired[Mpeg2CodecLevelType],  # (2)
    CodecProfile: NotRequired[Mpeg2CodecProfileType],  # (3)
    DynamicSubGop: NotRequired[Mpeg2DynamicSubGopType],  # (4)
    FramerateControl: NotRequired[Mpeg2FramerateControlType],  # (5)
    FramerateConversionAlgorithm: NotRequired[Mpeg2FramerateConversionAlgorithmType],  # (6)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    GopClosedCadence: NotRequired[int],
    GopSize: NotRequired[float],
    GopSizeUnits: NotRequired[Mpeg2GopSizeUnitsType],  # (7)
    HrdBufferFinalFillPercentage: NotRequired[int],
    HrdBufferInitialFillPercentage: NotRequired[int],
    HrdBufferSize: NotRequired[int],
    InterlaceMode: NotRequired[Mpeg2InterlaceModeType],  # (8)
    IntraDcPrecision: NotRequired[Mpeg2IntraDcPrecisionType],  # (9)
    MaxBitrate: NotRequired[int],
    MinIInterval: NotRequired[int],
    NumberBFramesBetweenReferenceFrames: NotRequired[int],
    ParControl: NotRequired[Mpeg2ParControlType],  # (10)
    ParDenominator: NotRequired[int],
    ParNumerator: NotRequired[int],
    QualityTuningLevel: NotRequired[Mpeg2QualityTuningLevelType],  # (11)
    RateControlMode: NotRequired[Mpeg2RateControlModeType],  # (12)
    ScanTypeConversionMode: NotRequired[Mpeg2ScanTypeConversionModeType],  # (13)
    SceneChangeDetect: NotRequired[Mpeg2SceneChangeDetectType],  # (14)
    SlowPal: NotRequired[Mpeg2SlowPalType],  # (15)
    Softness: NotRequired[int],
    SpatialAdaptiveQuantization: NotRequired[Mpeg2SpatialAdaptiveQuantizationType],  # (16)
    Syntax: NotRequired[Mpeg2SyntaxType],  # (17)
    Telecine: NotRequired[Mpeg2TelecineType],  # (18)
    TemporalAdaptiveQuantization: NotRequired[Mpeg2TemporalAdaptiveQuantizationType],  # (19)
```

1. See [:material-code-brackets: Mpeg2AdaptiveQuantizationType](./literals.md#mpeg2adaptivequantizationtype) 
2. See [:material-code-brackets: Mpeg2CodecLevelType](./literals.md#mpeg2codecleveltype) 
3. See [:material-code-brackets: Mpeg2CodecProfileType](./literals.md#mpeg2codecprofiletype) 
4. See [:material-code-brackets: Mpeg2DynamicSubGopType](./literals.md#mpeg2dynamicsubgoptype) 
5. See [:material-code-brackets: Mpeg2FramerateControlType](./literals.md#mpeg2frameratecontroltype) 
6. See [:material-code-brackets: Mpeg2FramerateConversionAlgorithmType](./literals.md#mpeg2framerateconversionalgorithmtype) 
7. See [:material-code-brackets: Mpeg2GopSizeUnitsType](./literals.md#mpeg2gopsizeunitstype) 
8. See [:material-code-brackets: Mpeg2InterlaceModeType](./literals.md#mpeg2interlacemodetype) 
9. See [:material-code-brackets: Mpeg2IntraDcPrecisionType](./literals.md#mpeg2intradcprecisiontype) 
10. See [:material-code-brackets: Mpeg2ParControlType](./literals.md#mpeg2parcontroltype) 
11. See [:material-code-brackets: Mpeg2QualityTuningLevelType](./literals.md#mpeg2qualitytuningleveltype) 
12. See [:material-code-brackets: Mpeg2RateControlModeType](./literals.md#mpeg2ratecontrolmodetype) 
13. See [:material-code-brackets: Mpeg2ScanTypeConversionModeType](./literals.md#mpeg2scantypeconversionmodetype) 
14. See [:material-code-brackets: Mpeg2SceneChangeDetectType](./literals.md#mpeg2scenechangedetecttype) 
15. See [:material-code-brackets: Mpeg2SlowPalType](./literals.md#mpeg2slowpaltype) 
16. See [:material-code-brackets: Mpeg2SpatialAdaptiveQuantizationType](./literals.md#mpeg2spatialadaptivequantizationtype) 
17. See [:material-code-brackets: Mpeg2SyntaxType](./literals.md#mpeg2syntaxtype) 
18. See [:material-code-brackets: Mpeg2TelecineType](./literals.md#mpeg2telecinetype) 
19. See [:material-code-brackets: Mpeg2TemporalAdaptiveQuantizationType](./literals.md#mpeg2temporaladaptivequantizationtype) 
## MsSmoothAdditionalManifestTypeDef

```python
# MsSmoothAdditionalManifestTypeDef definition

class MsSmoothAdditionalManifestTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[Sequence[str]],
```

## MxfXavcProfileSettingsTypeDef

```python
# MxfXavcProfileSettingsTypeDef definition

class MxfXavcProfileSettingsTypeDef(TypedDict):
    DurationMode: NotRequired[MxfXavcDurationModeType],  # (1)
    MaxAncDataSize: NotRequired[int],
```

1. See [:material-code-brackets: MxfXavcDurationModeType](./literals.md#mxfxavcdurationmodetype) 
## NexGuardFileMarkerSettingsTypeDef

```python
# NexGuardFileMarkerSettingsTypeDef definition

class NexGuardFileMarkerSettingsTypeDef(TypedDict):
    License: NotRequired[str],
    Payload: NotRequired[int],
    Preset: NotRequired[str],
    Strength: NotRequired[WatermarkingStrengthType],  # (1)
```

1. See [:material-code-brackets: WatermarkingStrengthType](./literals.md#watermarkingstrengthtype) 
## NoiseReducerFilterSettingsTypeDef

```python
# NoiseReducerFilterSettingsTypeDef definition

class NoiseReducerFilterSettingsTypeDef(TypedDict):
    Strength: NotRequired[int],
```

## NoiseReducerSpatialFilterSettingsTypeDef

```python
# NoiseReducerSpatialFilterSettingsTypeDef definition

class NoiseReducerSpatialFilterSettingsTypeDef(TypedDict):
    PostFilterSharpenStrength: NotRequired[int],
    Speed: NotRequired[int],
    Strength: NotRequired[int],
```

## NoiseReducerTemporalFilterSettingsTypeDef

```python
# NoiseReducerTemporalFilterSettingsTypeDef definition

class NoiseReducerTemporalFilterSettingsTypeDef(TypedDict):
    AggressiveMode: NotRequired[int],
    PostTemporalSharpening: NotRequired[NoiseFilterPostTemporalSharpeningType],  # (1)
    PostTemporalSharpeningStrength: NotRequired[NoiseFilterPostTemporalSharpeningStrengthType],  # (2)
    Speed: NotRequired[int],
    Strength: NotRequired[int],
```

1. See [:material-code-brackets: NoiseFilterPostTemporalSharpeningType](./literals.md#noisefilterposttemporalsharpeningtype) 
2. See [:material-code-brackets: NoiseFilterPostTemporalSharpeningStrengthType](./literals.md#noisefilterposttemporalsharpeningstrengthtype) 
## VideoDetailTypeDef

```python
# VideoDetailTypeDef definition

class VideoDetailTypeDef(TypedDict):
    HeightInPx: NotRequired[int],
    WidthInPx: NotRequired[int],
```

## ProresSettingsTypeDef

```python
# ProresSettingsTypeDef definition

class ProresSettingsTypeDef(TypedDict):
    ChromaSampling: NotRequired[ProresChromaSamplingType],  # (1)
    CodecProfile: NotRequired[ProresCodecProfileType],  # (2)
    FramerateControl: NotRequired[ProresFramerateControlType],  # (3)
    FramerateConversionAlgorithm: NotRequired[ProresFramerateConversionAlgorithmType],  # (4)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    InterlaceMode: NotRequired[ProresInterlaceModeType],  # (5)
    ParControl: NotRequired[ProresParControlType],  # (6)
    ParDenominator: NotRequired[int],
    ParNumerator: NotRequired[int],
    ScanTypeConversionMode: NotRequired[ProresScanTypeConversionModeType],  # (7)
    SlowPal: NotRequired[ProresSlowPalType],  # (8)
    Telecine: NotRequired[ProresTelecineType],  # (9)
```

1. See [:material-code-brackets: ProresChromaSamplingType](./literals.md#proreschromasamplingtype) 
2. See [:material-code-brackets: ProresCodecProfileType](./literals.md#prorescodecprofiletype) 
3. See [:material-code-brackets: ProresFramerateControlType](./literals.md#proresframeratecontroltype) 
4. See [:material-code-brackets: ProresFramerateConversionAlgorithmType](./literals.md#proresframerateconversionalgorithmtype) 
5. See [:material-code-brackets: ProresInterlaceModeType](./literals.md#proresinterlacemodetype) 
6. See [:material-code-brackets: ProresParControlType](./literals.md#proresparcontroltype) 
7. See [:material-code-brackets: ProresScanTypeConversionModeType](./literals.md#proresscantypeconversionmodetype) 
8. See [:material-code-brackets: ProresSlowPalType](./literals.md#proresslowpaltype) 
9. See [:material-code-brackets: ProresTelecineType](./literals.md#prorestelecinetype) 
## ReservationPlanTypeDef

```python
# ReservationPlanTypeDef definition

class ReservationPlanTypeDef(TypedDict):
    Commitment: NotRequired[CommitmentType],  # (1)
    ExpiresAt: NotRequired[datetime],
    PurchasedAt: NotRequired[datetime],
    RenewalType: NotRequired[RenewalTypeType],  # (2)
    ReservedSlots: NotRequired[int],
    Status: NotRequired[ReservationPlanStatusType],  # (3)
```

1. See [:material-code-brackets: CommitmentType](./literals.md#commitmenttype) 
2. See [:material-code-brackets: RenewalTypeType](./literals.md#renewaltypetype) 
3. See [:material-code-brackets: ReservationPlanStatusType](./literals.md#reservationplanstatustype) 
## S3DestinationAccessControlTypeDef

```python
# S3DestinationAccessControlTypeDef definition

class S3DestinationAccessControlTypeDef(TypedDict):
    CannedAcl: NotRequired[S3ObjectCannedAclType],  # (1)
```

1. See [:material-code-brackets: S3ObjectCannedAclType](./literals.md#s3objectcannedacltype) 
## S3EncryptionSettingsTypeDef

```python
# S3EncryptionSettingsTypeDef definition

class S3EncryptionSettingsTypeDef(TypedDict):
    EncryptionType: NotRequired[S3ServerSideEncryptionTypeType],  # (1)
    KmsEncryptionContext: NotRequired[str],
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: S3ServerSideEncryptionTypeType](./literals.md#s3serversideencryptiontypetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    Arn: str,
    Tags: Mapping[str, str],
```

## TimecodeBurninTypeDef

```python
# TimecodeBurninTypeDef definition

class TimecodeBurninTypeDef(TypedDict):
    FontSize: NotRequired[int],
    Position: NotRequired[TimecodeBurninPositionType],  # (1)
    Prefix: NotRequired[str],
```

1. See [:material-code-brackets: TimecodeBurninPositionType](./literals.md#timecodeburninpositiontype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    Arn: str,
    TagKeys: NotRequired[Sequence[str]],
```

## Vc3SettingsTypeDef

```python
# Vc3SettingsTypeDef definition

class Vc3SettingsTypeDef(TypedDict):
    FramerateControl: NotRequired[Vc3FramerateControlType],  # (1)
    FramerateConversionAlgorithm: NotRequired[Vc3FramerateConversionAlgorithmType],  # (2)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    InterlaceMode: NotRequired[Vc3InterlaceModeType],  # (3)
    ScanTypeConversionMode: NotRequired[Vc3ScanTypeConversionModeType],  # (4)
    SlowPal: NotRequired[Vc3SlowPalType],  # (5)
    Telecine: NotRequired[Vc3TelecineType],  # (6)
    Vc3Class: NotRequired[Vc3ClassType],  # (7)
```

1. See [:material-code-brackets: Vc3FramerateControlType](./literals.md#vc3frameratecontroltype) 
2. See [:material-code-brackets: Vc3FramerateConversionAlgorithmType](./literals.md#vc3framerateconversionalgorithmtype) 
3. See [:material-code-brackets: Vc3InterlaceModeType](./literals.md#vc3interlacemodetype) 
4. See [:material-code-brackets: Vc3ScanTypeConversionModeType](./literals.md#vc3scantypeconversionmodetype) 
5. See [:material-code-brackets: Vc3SlowPalType](./literals.md#vc3slowpaltype) 
6. See [:material-code-brackets: Vc3TelecineType](./literals.md#vc3telecinetype) 
7. See [:material-code-brackets: Vc3ClassType](./literals.md#vc3classtype) 
## Vp8SettingsTypeDef

```python
# Vp8SettingsTypeDef definition

class Vp8SettingsTypeDef(TypedDict):
    Bitrate: NotRequired[int],
    FramerateControl: NotRequired[Vp8FramerateControlType],  # (1)
    FramerateConversionAlgorithm: NotRequired[Vp8FramerateConversionAlgorithmType],  # (2)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    GopSize: NotRequired[float],
    HrdBufferSize: NotRequired[int],
    MaxBitrate: NotRequired[int],
    ParControl: NotRequired[Vp8ParControlType],  # (3)
    ParDenominator: NotRequired[int],
    ParNumerator: NotRequired[int],
    QualityTuningLevel: NotRequired[Vp8QualityTuningLevelType],  # (4)
    RateControlMode: NotRequired[Vp8RateControlModeType],  # (5)
```

1. See [:material-code-brackets: Vp8FramerateControlType](./literals.md#vp8frameratecontroltype) 
2. See [:material-code-brackets: Vp8FramerateConversionAlgorithmType](./literals.md#vp8framerateconversionalgorithmtype) 
3. See [:material-code-brackets: Vp8ParControlType](./literals.md#vp8parcontroltype) 
4. See [:material-code-brackets: Vp8QualityTuningLevelType](./literals.md#vp8qualitytuningleveltype) 
5. See [:material-code-brackets: Vp8RateControlModeType](./literals.md#vp8ratecontrolmodetype) 
## Vp9SettingsTypeDef

```python
# Vp9SettingsTypeDef definition

class Vp9SettingsTypeDef(TypedDict):
    Bitrate: NotRequired[int],
    FramerateControl: NotRequired[Vp9FramerateControlType],  # (1)
    FramerateConversionAlgorithm: NotRequired[Vp9FramerateConversionAlgorithmType],  # (2)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    GopSize: NotRequired[float],
    HrdBufferSize: NotRequired[int],
    MaxBitrate: NotRequired[int],
    ParControl: NotRequired[Vp9ParControlType],  # (3)
    ParDenominator: NotRequired[int],
    ParNumerator: NotRequired[int],
    QualityTuningLevel: NotRequired[Vp9QualityTuningLevelType],  # (4)
    RateControlMode: NotRequired[Vp9RateControlModeType],  # (5)
```

1. See [:material-code-brackets: Vp9FramerateControlType](./literals.md#vp9frameratecontroltype) 
2. See [:material-code-brackets: Vp9FramerateConversionAlgorithmType](./literals.md#vp9framerateconversionalgorithmtype) 
3. See [:material-code-brackets: Vp9ParControlType](./literals.md#vp9parcontroltype) 
4. See [:material-code-brackets: Vp9QualityTuningLevelType](./literals.md#vp9qualitytuningleveltype) 
5. See [:material-code-brackets: Vp9RateControlModeType](./literals.md#vp9ratecontrolmodetype) 
## Xavc4kIntraCbgProfileSettingsTypeDef

```python
# Xavc4kIntraCbgProfileSettingsTypeDef definition

class Xavc4kIntraCbgProfileSettingsTypeDef(TypedDict):
    XavcClass: NotRequired[Xavc4kIntraCbgProfileClassType],  # (1)
```

1. See [:material-code-brackets: Xavc4kIntraCbgProfileClassType](./literals.md#xavc4kintracbgprofileclasstype) 
## Xavc4kIntraVbrProfileSettingsTypeDef

```python
# Xavc4kIntraVbrProfileSettingsTypeDef definition

class Xavc4kIntraVbrProfileSettingsTypeDef(TypedDict):
    XavcClass: NotRequired[Xavc4kIntraVbrProfileClassType],  # (1)
```

1. See [:material-code-brackets: Xavc4kIntraVbrProfileClassType](./literals.md#xavc4kintravbrprofileclasstype) 
## Xavc4kProfileSettingsTypeDef

```python
# Xavc4kProfileSettingsTypeDef definition

class Xavc4kProfileSettingsTypeDef(TypedDict):
    BitrateClass: NotRequired[Xavc4kProfileBitrateClassType],  # (1)
    CodecProfile: NotRequired[Xavc4kProfileCodecProfileType],  # (2)
    FlickerAdaptiveQuantization: NotRequired[XavcFlickerAdaptiveQuantizationType],  # (3)
    GopBReference: NotRequired[XavcGopBReferenceType],  # (4)
    GopClosedCadence: NotRequired[int],
    HrdBufferSize: NotRequired[int],
    QualityTuningLevel: NotRequired[Xavc4kProfileQualityTuningLevelType],  # (5)
    Slices: NotRequired[int],
```

1. See [:material-code-brackets: Xavc4kProfileBitrateClassType](./literals.md#xavc4kprofilebitrateclasstype) 
2. See [:material-code-brackets: Xavc4kProfileCodecProfileType](./literals.md#xavc4kprofilecodecprofiletype) 
3. See [:material-code-brackets: XavcFlickerAdaptiveQuantizationType](./literals.md#xavcflickeradaptivequantizationtype) 
4. See [:material-code-brackets: XavcGopBReferenceType](./literals.md#xavcgopbreferencetype) 
5. See [:material-code-brackets: Xavc4kProfileQualityTuningLevelType](./literals.md#xavc4kprofilequalitytuningleveltype) 
## XavcHdIntraCbgProfileSettingsTypeDef

```python
# XavcHdIntraCbgProfileSettingsTypeDef definition

class XavcHdIntraCbgProfileSettingsTypeDef(TypedDict):
    XavcClass: NotRequired[XavcHdIntraCbgProfileClassType],  # (1)
```

1. See [:material-code-brackets: XavcHdIntraCbgProfileClassType](./literals.md#xavchdintracbgprofileclasstype) 
## XavcHdProfileSettingsTypeDef

```python
# XavcHdProfileSettingsTypeDef definition

class XavcHdProfileSettingsTypeDef(TypedDict):
    BitrateClass: NotRequired[XavcHdProfileBitrateClassType],  # (1)
    FlickerAdaptiveQuantization: NotRequired[XavcFlickerAdaptiveQuantizationType],  # (2)
    GopBReference: NotRequired[XavcGopBReferenceType],  # (3)
    GopClosedCadence: NotRequired[int],
    HrdBufferSize: NotRequired[int],
    InterlaceMode: NotRequired[XavcInterlaceModeType],  # (4)
    QualityTuningLevel: NotRequired[XavcHdProfileQualityTuningLevelType],  # (5)
    Slices: NotRequired[int],
    Telecine: NotRequired[XavcHdProfileTelecineType],  # (6)
```

1. See [:material-code-brackets: XavcHdProfileBitrateClassType](./literals.md#xavchdprofilebitrateclasstype) 
2. See [:material-code-brackets: XavcFlickerAdaptiveQuantizationType](./literals.md#xavcflickeradaptivequantizationtype) 
3. See [:material-code-brackets: XavcGopBReferenceType](./literals.md#xavcgopbreferencetype) 
4. See [:material-code-brackets: XavcInterlaceModeType](./literals.md#xavcinterlacemodetype) 
5. See [:material-code-brackets: XavcHdProfileQualityTuningLevelType](./literals.md#xavchdprofilequalitytuningleveltype) 
6. See [:material-code-brackets: XavcHdProfileTelecineType](./literals.md#xavchdprofiletelecinetype) 
## AudioCodecSettingsTypeDef

```python
# AudioCodecSettingsTypeDef definition

class AudioCodecSettingsTypeDef(TypedDict):
    AacSettings: NotRequired[AacSettingsTypeDef],  # (1)
    Ac3Settings: NotRequired[Ac3SettingsTypeDef],  # (2)
    AiffSettings: NotRequired[AiffSettingsTypeDef],  # (3)
    Codec: NotRequired[AudioCodecType],  # (4)
    Eac3AtmosSettings: NotRequired[Eac3AtmosSettingsTypeDef],  # (5)
    Eac3Settings: NotRequired[Eac3SettingsTypeDef],  # (6)
    Mp2Settings: NotRequired[Mp2SettingsTypeDef],  # (7)
    Mp3Settings: NotRequired[Mp3SettingsTypeDef],  # (8)
    OpusSettings: NotRequired[OpusSettingsTypeDef],  # (9)
    VorbisSettings: NotRequired[VorbisSettingsTypeDef],  # (10)
    WavSettings: NotRequired[WavSettingsTypeDef],  # (11)
```

1. See [:material-code-braces: AacSettingsTypeDef](./type_defs.md#aacsettingstypedef) 
2. See [:material-code-braces: Ac3SettingsTypeDef](./type_defs.md#ac3settingstypedef) 
3. See [:material-code-braces: AiffSettingsTypeDef](./type_defs.md#aiffsettingstypedef) 
4. See [:material-code-brackets: AudioCodecType](./literals.md#audiocodectype) 
5. See [:material-code-braces: Eac3AtmosSettingsTypeDef](./type_defs.md#eac3atmossettingstypedef) 
6. See [:material-code-braces: Eac3SettingsTypeDef](./type_defs.md#eac3settingstypedef) 
7. See [:material-code-braces: Mp2SettingsTypeDef](./type_defs.md#mp2settingstypedef) 
8. See [:material-code-braces: Mp3SettingsTypeDef](./type_defs.md#mp3settingstypedef) 
9. See [:material-code-braces: OpusSettingsTypeDef](./type_defs.md#opussettingstypedef) 
10. See [:material-code-braces: VorbisSettingsTypeDef](./type_defs.md#vorbissettingstypedef) 
11. See [:material-code-braces: WavSettingsTypeDef](./type_defs.md#wavsettingstypedef) 
## AutomatedAbrRuleTypeDef

```python
# AutomatedAbrRuleTypeDef definition

class AutomatedAbrRuleTypeDef(TypedDict):
    AllowedRenditions: NotRequired[Sequence[AllowedRenditionSizeTypeDef]],  # (1)
    ForceIncludeRenditions: NotRequired[Sequence[ForceIncludeRenditionSizeTypeDef]],  # (2)
    MinBottomRenditionSize: NotRequired[MinBottomRenditionSizeTypeDef],  # (3)
    MinTopRenditionSize: NotRequired[MinTopRenditionSizeTypeDef],  # (4)
    Type: NotRequired[RuleTypeType],  # (5)
```

1. See [:material-code-braces: AllowedRenditionSizeTypeDef](./type_defs.md#allowedrenditionsizetypedef) 
2. See [:material-code-braces: ForceIncludeRenditionSizeTypeDef](./type_defs.md#forceincluderenditionsizetypedef) 
3. See [:material-code-braces: MinBottomRenditionSizeTypeDef](./type_defs.md#minbottomrenditionsizetypedef) 
4. See [:material-code-braces: MinTopRenditionSizeTypeDef](./type_defs.md#mintoprenditionsizetypedef) 
5. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
## Av1SettingsTypeDef

```python
# Av1SettingsTypeDef definition

class Av1SettingsTypeDef(TypedDict):
    AdaptiveQuantization: NotRequired[Av1AdaptiveQuantizationType],  # (1)
    BitDepth: NotRequired[Av1BitDepthType],  # (2)
    FramerateControl: NotRequired[Av1FramerateControlType],  # (3)
    FramerateConversionAlgorithm: NotRequired[Av1FramerateConversionAlgorithmType],  # (4)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    GopSize: NotRequired[float],
    MaxBitrate: NotRequired[int],
    NumberBFramesBetweenReferenceFrames: NotRequired[int],
    QvbrSettings: NotRequired[Av1QvbrSettingsTypeDef],  # (5)
    RateControlMode: NotRequired[Av1RateControlModeType],  # (6)
    Slices: NotRequired[int],
    SpatialAdaptiveQuantization: NotRequired[Av1SpatialAdaptiveQuantizationType],  # (7)
```

1. See [:material-code-brackets: Av1AdaptiveQuantizationType](./literals.md#av1adaptivequantizationtype) 
2. See [:material-code-brackets: Av1BitDepthType](./literals.md#av1bitdepthtype) 
3. See [:material-code-brackets: Av1FramerateControlType](./literals.md#av1frameratecontroltype) 
4. See [:material-code-brackets: Av1FramerateConversionAlgorithmType](./literals.md#av1framerateconversionalgorithmtype) 
5. See [:material-code-braces: Av1QvbrSettingsTypeDef](./type_defs.md#av1qvbrsettingstypedef) 
6. See [:material-code-brackets: Av1RateControlModeType](./literals.md#av1ratecontrolmodetype) 
7. See [:material-code-brackets: Av1SpatialAdaptiveQuantizationType](./literals.md#av1spatialadaptivequantizationtype) 
## AvcIntraSettingsTypeDef

```python
# AvcIntraSettingsTypeDef definition

class AvcIntraSettingsTypeDef(TypedDict):
    AvcIntraClass: NotRequired[AvcIntraClassType],  # (1)
    AvcIntraUhdSettings: NotRequired[AvcIntraUhdSettingsTypeDef],  # (2)
    FramerateControl: NotRequired[AvcIntraFramerateControlType],  # (3)
    FramerateConversionAlgorithm: NotRequired[AvcIntraFramerateConversionAlgorithmType],  # (4)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    InterlaceMode: NotRequired[AvcIntraInterlaceModeType],  # (5)
    ScanTypeConversionMode: NotRequired[AvcIntraScanTypeConversionModeType],  # (6)
    SlowPal: NotRequired[AvcIntraSlowPalType],  # (7)
    Telecine: NotRequired[AvcIntraTelecineType],  # (8)
```

1. See [:material-code-brackets: AvcIntraClassType](./literals.md#avcintraclasstype) 
2. See [:material-code-braces: AvcIntraUhdSettingsTypeDef](./type_defs.md#avcintrauhdsettingstypedef) 
3. See [:material-code-brackets: AvcIntraFramerateControlType](./literals.md#avcintraframeratecontroltype) 
4. See [:material-code-brackets: AvcIntraFramerateConversionAlgorithmType](./literals.md#avcintraframerateconversionalgorithmtype) 
5. See [:material-code-brackets: AvcIntraInterlaceModeType](./literals.md#avcintrainterlacemodetype) 
6. See [:material-code-brackets: AvcIntraScanTypeConversionModeType](./literals.md#avcintrascantypeconversionmodetype) 
7. See [:material-code-brackets: AvcIntraSlowPalType](./literals.md#avcintraslowpaltype) 
8. See [:material-code-brackets: AvcIntraTelecineType](./literals.md#avcintratelecinetype) 
## CaptionDestinationSettingsTypeDef

```python
# CaptionDestinationSettingsTypeDef definition

class CaptionDestinationSettingsTypeDef(TypedDict):
    BurninDestinationSettings: NotRequired[BurninDestinationSettingsTypeDef],  # (1)
    DestinationType: NotRequired[CaptionDestinationTypeType],  # (2)
    DvbSubDestinationSettings: NotRequired[DvbSubDestinationSettingsTypeDef],  # (3)
    EmbeddedDestinationSettings: NotRequired[EmbeddedDestinationSettingsTypeDef],  # (4)
    ImscDestinationSettings: NotRequired[ImscDestinationSettingsTypeDef],  # (5)
    SccDestinationSettings: NotRequired[SccDestinationSettingsTypeDef],  # (6)
    SrtDestinationSettings: NotRequired[SrtDestinationSettingsTypeDef],  # (7)
    TeletextDestinationSettings: NotRequired[TeletextDestinationSettingsTypeDef],  # (8)
    TtmlDestinationSettings: NotRequired[TtmlDestinationSettingsTypeDef],  # (9)
    WebvttDestinationSettings: NotRequired[WebvttDestinationSettingsTypeDef],  # (10)
```

1. See [:material-code-braces: BurninDestinationSettingsTypeDef](./type_defs.md#burnindestinationsettingstypedef) 
2. See [:material-code-brackets: CaptionDestinationTypeType](./literals.md#captiondestinationtypetype) 
3. See [:material-code-braces: DvbSubDestinationSettingsTypeDef](./type_defs.md#dvbsubdestinationsettingstypedef) 
4. See [:material-code-braces: EmbeddedDestinationSettingsTypeDef](./type_defs.md#embeddeddestinationsettingstypedef) 
5. See [:material-code-braces: ImscDestinationSettingsTypeDef](./type_defs.md#imscdestinationsettingstypedef) 
6. See [:material-code-braces: SccDestinationSettingsTypeDef](./type_defs.md#sccdestinationsettingstypedef) 
7. See [:material-code-braces: SrtDestinationSettingsTypeDef](./type_defs.md#srtdestinationsettingstypedef) 
8. See [:material-code-braces: TeletextDestinationSettingsTypeDef](./type_defs.md#teletextdestinationsettingstypedef) 
9. See [:material-code-braces: TtmlDestinationSettingsTypeDef](./type_defs.md#ttmldestinationsettingstypedef) 
10. See [:material-code-braces: WebvttDestinationSettingsTypeDef](./type_defs.md#webvttdestinationsettingstypedef) 
## FileSourceSettingsTypeDef

```python
# FileSourceSettingsTypeDef definition

class FileSourceSettingsTypeDef(TypedDict):
    Convert608To708: NotRequired[FileSourceConvert608To708Type],  # (1)
    ConvertPaintToPop: NotRequired[CaptionSourceConvertPaintOnToPopOnType],  # (2)
    Framerate: NotRequired[CaptionSourceFramerateTypeDef],  # (3)
    SourceFile: NotRequired[str],
    TimeDelta: NotRequired[int],
    TimeDeltaUnits: NotRequired[FileSourceTimeDeltaUnitsType],  # (4)
```

1. See [:material-code-brackets: FileSourceConvert608To708Type](./literals.md#filesourceconvert608to708type) 
2. See [:material-code-brackets: CaptionSourceConvertPaintOnToPopOnType](./literals.md#captionsourceconvertpaintontopopontype) 
3. See [:material-code-braces: CaptionSourceFramerateTypeDef](./type_defs.md#captionsourceframeratetypedef) 
4. See [:material-code-brackets: FileSourceTimeDeltaUnitsType](./literals.md#filesourcetimedeltaunitstype) 
## ChannelMappingTypeDef

```python
# ChannelMappingTypeDef definition

class ChannelMappingTypeDef(TypedDict):
    OutputChannels: NotRequired[Sequence[OutputChannelMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: OutputChannelMappingTypeDef](./type_defs.md#outputchannelmappingtypedef) 
## CmafEncryptionSettingsTypeDef

```python
# CmafEncryptionSettingsTypeDef definition

class CmafEncryptionSettingsTypeDef(TypedDict):
    ConstantInitializationVector: NotRequired[str],
    EncryptionMethod: NotRequired[CmafEncryptionTypeType],  # (1)
    InitializationVectorInManifest: NotRequired[CmafInitializationVectorInManifestType],  # (2)
    SpekeKeyProvider: NotRequired[SpekeKeyProviderCmafTypeDef],  # (3)
    StaticKeyProvider: NotRequired[StaticKeyProviderTypeDef],  # (4)
    Type: NotRequired[CmafKeyProviderTypeType],  # (5)
```

1. See [:material-code-brackets: CmafEncryptionTypeType](./literals.md#cmafencryptiontypetype) 
2. See [:material-code-brackets: CmafInitializationVectorInManifestType](./literals.md#cmafinitializationvectorinmanifesttype) 
3. See [:material-code-braces: SpekeKeyProviderCmafTypeDef](./type_defs.md#spekekeyprovidercmaftypedef) 
4. See [:material-code-braces: StaticKeyProviderTypeDef](./type_defs.md#statickeyprovidertypedef) 
5. See [:material-code-brackets: CmafKeyProviderTypeType](./literals.md#cmafkeyprovidertypetype) 
## ColorCorrectorTypeDef

```python
# ColorCorrectorTypeDef definition

class ColorCorrectorTypeDef(TypedDict):
    Brightness: NotRequired[int],
    ClipLimits: NotRequired[ClipLimitsTypeDef],  # (1)
    ColorSpaceConversion: NotRequired[ColorSpaceConversionType],  # (2)
    Contrast: NotRequired[int],
    Hdr10Metadata: NotRequired[Hdr10MetadataTypeDef],  # (3)
    HdrToSdrToneMapper: NotRequired[HDRToSDRToneMapperType],  # (4)
    Hue: NotRequired[int],
    SampleRangeConversion: NotRequired[SampleRangeConversionType],  # (5)
    Saturation: NotRequired[int],
    SdrReferenceWhiteLevel: NotRequired[int],
```

1. See [:material-code-braces: ClipLimitsTypeDef](./type_defs.md#cliplimitstypedef) 
2. See [:material-code-brackets: ColorSpaceConversionType](./literals.md#colorspaceconversiontype) 
3. See [:material-code-braces: Hdr10MetadataTypeDef](./type_defs.md#hdr10metadatatypedef) 
4. See [:material-code-brackets: HDRToSDRToneMapperType](./literals.md#hdrtosdrtonemappertype) 
5. See [:material-code-brackets: SampleRangeConversionType](./literals.md#samplerangeconversiontype) 
## VideoSelectorTypeDef

```python
# VideoSelectorTypeDef definition

class VideoSelectorTypeDef(TypedDict):
    AlphaBehavior: NotRequired[AlphaBehaviorType],  # (1)
    ColorSpace: NotRequired[ColorSpaceType],  # (2)
    ColorSpaceUsage: NotRequired[ColorSpaceUsageType],  # (3)
    EmbeddedTimecodeOverride: NotRequired[EmbeddedTimecodeOverrideType],  # (4)
    Hdr10Metadata: NotRequired[Hdr10MetadataTypeDef],  # (5)
    PadVideo: NotRequired[PadVideoType],  # (6)
    Pid: NotRequired[int],
    ProgramNumber: NotRequired[int],
    Rotate: NotRequired[InputRotateType],  # (7)
    SampleRange: NotRequired[InputSampleRangeType],  # (8)
```

1. See [:material-code-brackets: AlphaBehaviorType](./literals.md#alphabehaviortype) 
2. See [:material-code-brackets: ColorSpaceType](./literals.md#colorspacetype) 
3. See [:material-code-brackets: ColorSpaceUsageType](./literals.md#colorspaceusagetype) 
4. See [:material-code-brackets: EmbeddedTimecodeOverrideType](./literals.md#embeddedtimecodeoverridetype) 
5. See [:material-code-braces: Hdr10MetadataTypeDef](./type_defs.md#hdr10metadatatypedef) 
6. See [:material-code-brackets: PadVideoType](./literals.md#padvideotype) 
7. See [:material-code-brackets: InputRotateType](./literals.md#inputrotatetype) 
8. See [:material-code-brackets: InputSampleRangeType](./literals.md#inputsamplerangetype) 
## CreateQueueRequestRequestTypeDef

```python
# CreateQueueRequestRequestTypeDef definition

class CreateQueueRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    ReservationPlanSettings: NotRequired[ReservationPlanSettingsTypeDef],  # (2)
    Status: NotRequired[QueueStatusType],  # (3)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: ReservationPlanSettingsTypeDef](./type_defs.md#reservationplansettingstypedef) 
3. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
## UpdateQueueRequestRequestTypeDef

```python
# UpdateQueueRequestRequestTypeDef definition

class UpdateQueueRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    ReservationPlanSettings: NotRequired[ReservationPlanSettingsTypeDef],  # (1)
    Status: NotRequired[QueueStatusType],  # (2)
```

1. See [:material-code-braces: ReservationPlanSettingsTypeDef](./type_defs.md#reservationplansettingstypedef) 
2. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
## DashIsoEncryptionSettingsTypeDef

```python
# DashIsoEncryptionSettingsTypeDef definition

class DashIsoEncryptionSettingsTypeDef(TypedDict):
    PlaybackDeviceCompatibility: NotRequired[DashIsoPlaybackDeviceCompatibilityType],  # (1)
    SpekeKeyProvider: NotRequired[SpekeKeyProviderTypeDef],  # (2)
```

1. See [:material-code-brackets: DashIsoPlaybackDeviceCompatibilityType](./literals.md#dashisoplaybackdevicecompatibilitytype) 
2. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) 
## HlsEncryptionSettingsTypeDef

```python
# HlsEncryptionSettingsTypeDef definition

class HlsEncryptionSettingsTypeDef(TypedDict):
    ConstantInitializationVector: NotRequired[str],
    EncryptionMethod: NotRequired[HlsEncryptionTypeType],  # (1)
    InitializationVectorInManifest: NotRequired[HlsInitializationVectorInManifestType],  # (2)
    OfflineEncrypted: NotRequired[HlsOfflineEncryptedType],  # (3)
    SpekeKeyProvider: NotRequired[SpekeKeyProviderTypeDef],  # (4)
    StaticKeyProvider: NotRequired[StaticKeyProviderTypeDef],  # (5)
    Type: NotRequired[HlsKeyProviderTypeType],  # (6)
```

1. See [:material-code-brackets: HlsEncryptionTypeType](./literals.md#hlsencryptiontypetype) 
2. See [:material-code-brackets: HlsInitializationVectorInManifestType](./literals.md#hlsinitializationvectorinmanifesttype) 
3. See [:material-code-brackets: HlsOfflineEncryptedType](./literals.md#hlsofflineencryptedtype) 
4. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) 
5. See [:material-code-braces: StaticKeyProviderTypeDef](./type_defs.md#statickeyprovidertypedef) 
6. See [:material-code-brackets: HlsKeyProviderTypeType](./literals.md#hlskeyprovidertypetype) 
## MsSmoothEncryptionSettingsTypeDef

```python
# MsSmoothEncryptionSettingsTypeDef definition

class MsSmoothEncryptionSettingsTypeDef(TypedDict):
    SpekeKeyProvider: NotRequired[SpekeKeyProviderTypeDef],  # (1)
```

1. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) 
## DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef

```python
# DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef definition

class DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef(TypedDict):
    Mode: NotRequired[DescribeEndpointsModeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DescribeEndpointsModeType](./literals.md#describeendpointsmodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobTemplatesRequestListJobTemplatesPaginateTypeDef

```python
# ListJobTemplatesRequestListJobTemplatesPaginateTypeDef definition

class ListJobTemplatesRequestListJobTemplatesPaginateTypeDef(TypedDict):
    Category: NotRequired[str],
    ListBy: NotRequired[JobTemplateListByType],  # (1)
    Order: NotRequired[OrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: JobTemplateListByType](./literals.md#jobtemplatelistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestListJobsPaginateTypeDef

```python
# ListJobsRequestListJobsPaginateTypeDef definition

class ListJobsRequestListJobsPaginateTypeDef(TypedDict):
    Order: NotRequired[OrderType],  # (1)
    Queue: NotRequired[str],
    Status: NotRequired[JobStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPresetsRequestListPresetsPaginateTypeDef

```python
# ListPresetsRequestListPresetsPaginateTypeDef definition

class ListPresetsRequestListPresetsPaginateTypeDef(TypedDict):
    Category: NotRequired[str],
    ListBy: NotRequired[PresetListByType],  # (1)
    Order: NotRequired[OrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PresetListByType](./literals.md#presetlistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueuesRequestListQueuesPaginateTypeDef

```python
# ListQueuesRequestListQueuesPaginateTypeDef definition

class ListQueuesRequestListQueuesPaginateTypeDef(TypedDict):
    ListBy: NotRequired[QueueListByType],  # (1)
    Order: NotRequired[OrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: QueueListByType](./literals.md#queuelistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEndpointsResponseTypeDef

```python
# DescribeEndpointsResponseTypeDef definition

class DescribeEndpointsResponseTypeDef(TypedDict):
    Endpoints: List[EndpointTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DolbyVisionTypeDef

```python
# DolbyVisionTypeDef definition

class DolbyVisionTypeDef(TypedDict):
    L6Metadata: NotRequired[DolbyVisionLevel6MetadataTypeDef],  # (1)
    L6Mode: NotRequired[DolbyVisionLevel6ModeType],  # (2)
    Mapping: NotRequired[DolbyVisionMappingType],  # (3)
    Profile: NotRequired[DolbyVisionProfileType],  # (4)
```

1. See [:material-code-braces: DolbyVisionLevel6MetadataTypeDef](./type_defs.md#dolbyvisionlevel6metadatatypedef) 
2. See [:material-code-brackets: DolbyVisionLevel6ModeType](./literals.md#dolbyvisionlevel6modetype) 
3. See [:material-code-brackets: DolbyVisionMappingType](./literals.md#dolbyvisionmappingtype) 
4. See [:material-code-brackets: DolbyVisionProfileType](./literals.md#dolbyvisionprofiletype) 
## EsamSettingsTypeDef

```python
# EsamSettingsTypeDef definition

class EsamSettingsTypeDef(TypedDict):
    ManifestConfirmConditionNotification: NotRequired[EsamManifestConfirmConditionNotificationTypeDef],  # (1)
    ResponseSignalPreroll: NotRequired[int],
    SignalProcessingNotification: NotRequired[EsamSignalProcessingNotificationTypeDef],  # (2)
```

1. See [:material-code-braces: EsamManifestConfirmConditionNotificationTypeDef](./type_defs.md#esammanifestconfirmconditionnotificationtypedef) 
2. See [:material-code-braces: EsamSignalProcessingNotificationTypeDef](./type_defs.md#esamsignalprocessingnotificationtypedef) 
## GetPolicyResponseTypeDef

```python
# GetPolicyResponseTypeDef definition

class GetPolicyResponseTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutPolicyRequestRequestTypeDef

```python
# PutPolicyRequestRequestTypeDef definition

class PutPolicyRequestRequestTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
## PutPolicyResponseTypeDef

```python
# PutPolicyResponseTypeDef definition

class PutPolicyResponseTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## H264SettingsTypeDef

```python
# H264SettingsTypeDef definition

class H264SettingsTypeDef(TypedDict):
    AdaptiveQuantization: NotRequired[H264AdaptiveQuantizationType],  # (1)
    BandwidthReductionFilter: NotRequired[BandwidthReductionFilterTypeDef],  # (2)
    Bitrate: NotRequired[int],
    CodecLevel: NotRequired[H264CodecLevelType],  # (3)
    CodecProfile: NotRequired[H264CodecProfileType],  # (4)
    DynamicSubGop: NotRequired[H264DynamicSubGopType],  # (5)
    EntropyEncoding: NotRequired[H264EntropyEncodingType],  # (6)
    FieldEncoding: NotRequired[H264FieldEncodingType],  # (7)
    FlickerAdaptiveQuantization: NotRequired[H264FlickerAdaptiveQuantizationType],  # (8)
    FramerateControl: NotRequired[H264FramerateControlType],  # (9)
    FramerateConversionAlgorithm: NotRequired[H264FramerateConversionAlgorithmType],  # (10)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    GopBReference: NotRequired[H264GopBReferenceType],  # (11)
    GopClosedCadence: NotRequired[int],
    GopSize: NotRequired[float],
    GopSizeUnits: NotRequired[H264GopSizeUnitsType],  # (12)
    HrdBufferFinalFillPercentage: NotRequired[int],
    HrdBufferInitialFillPercentage: NotRequired[int],
    HrdBufferSize: NotRequired[int],
    InterlaceMode: NotRequired[H264InterlaceModeType],  # (13)
    MaxBitrate: NotRequired[int],
    MinIInterval: NotRequired[int],
    NumberBFramesBetweenReferenceFrames: NotRequired[int],
    NumberReferenceFrames: NotRequired[int],
    ParControl: NotRequired[H264ParControlType],  # (14)
    ParDenominator: NotRequired[int],
    ParNumerator: NotRequired[int],
    QualityTuningLevel: NotRequired[H264QualityTuningLevelType],  # (15)
    QvbrSettings: NotRequired[H264QvbrSettingsTypeDef],  # (16)
    RateControlMode: NotRequired[H264RateControlModeType],  # (17)
    RepeatPps: NotRequired[H264RepeatPpsType],  # (18)
    ScanTypeConversionMode: NotRequired[H264ScanTypeConversionModeType],  # (19)
    SceneChangeDetect: NotRequired[H264SceneChangeDetectType],  # (20)
    Slices: NotRequired[int],
    SlowPal: NotRequired[H264SlowPalType],  # (21)
    Softness: NotRequired[int],
    SpatialAdaptiveQuantization: NotRequired[H264SpatialAdaptiveQuantizationType],  # (22)
    Syntax: NotRequired[H264SyntaxType],  # (23)
    Telecine: NotRequired[H264TelecineType],  # (24)
    TemporalAdaptiveQuantization: NotRequired[H264TemporalAdaptiveQuantizationType],  # (25)
    UnregisteredSeiTimecode: NotRequired[H264UnregisteredSeiTimecodeType],  # (26)
```

1. See [:material-code-brackets: H264AdaptiveQuantizationType](./literals.md#h264adaptivequantizationtype) 
2. See [:material-code-braces: BandwidthReductionFilterTypeDef](./type_defs.md#bandwidthreductionfiltertypedef) 
3. See [:material-code-brackets: H264CodecLevelType](./literals.md#h264codecleveltype) 
4. See [:material-code-brackets: H264CodecProfileType](./literals.md#h264codecprofiletype) 
5. See [:material-code-brackets: H264DynamicSubGopType](./literals.md#h264dynamicsubgoptype) 
6. See [:material-code-brackets: H264EntropyEncodingType](./literals.md#h264entropyencodingtype) 
7. See [:material-code-brackets: H264FieldEncodingType](./literals.md#h264fieldencodingtype) 
8. See [:material-code-brackets: H264FlickerAdaptiveQuantizationType](./literals.md#h264flickeradaptivequantizationtype) 
9. See [:material-code-brackets: H264FramerateControlType](./literals.md#h264frameratecontroltype) 
10. See [:material-code-brackets: H264FramerateConversionAlgorithmType](./literals.md#h264framerateconversionalgorithmtype) 
11. See [:material-code-brackets: H264GopBReferenceType](./literals.md#h264gopbreferencetype) 
12. See [:material-code-brackets: H264GopSizeUnitsType](./literals.md#h264gopsizeunitstype) 
13. See [:material-code-brackets: H264InterlaceModeType](./literals.md#h264interlacemodetype) 
14. See [:material-code-brackets: H264ParControlType](./literals.md#h264parcontroltype) 
15. See [:material-code-brackets: H264QualityTuningLevelType](./literals.md#h264qualitytuningleveltype) 
16. See [:material-code-braces: H264QvbrSettingsTypeDef](./type_defs.md#h264qvbrsettingstypedef) 
17. See [:material-code-brackets: H264RateControlModeType](./literals.md#h264ratecontrolmodetype) 
18. See [:material-code-brackets: H264RepeatPpsType](./literals.md#h264repeatppstype) 
19. See [:material-code-brackets: H264ScanTypeConversionModeType](./literals.md#h264scantypeconversionmodetype) 
20. See [:material-code-brackets: H264SceneChangeDetectType](./literals.md#h264scenechangedetecttype) 
21. See [:material-code-brackets: H264SlowPalType](./literals.md#h264slowpaltype) 
22. See [:material-code-brackets: H264SpatialAdaptiveQuantizationType](./literals.md#h264spatialadaptivequantizationtype) 
23. See [:material-code-brackets: H264SyntaxType](./literals.md#h264syntaxtype) 
24. See [:material-code-brackets: H264TelecineType](./literals.md#h264telecinetype) 
25. See [:material-code-brackets: H264TemporalAdaptiveQuantizationType](./literals.md#h264temporaladaptivequantizationtype) 
26. See [:material-code-brackets: H264UnregisteredSeiTimecodeType](./literals.md#h264unregisteredseitimecodetype) 
## H265SettingsTypeDef

```python
# H265SettingsTypeDef definition

class H265SettingsTypeDef(TypedDict):
    AdaptiveQuantization: NotRequired[H265AdaptiveQuantizationType],  # (1)
    AlternateTransferFunctionSei: NotRequired[H265AlternateTransferFunctionSeiType],  # (2)
    BandwidthReductionFilter: NotRequired[BandwidthReductionFilterTypeDef],  # (3)
    Bitrate: NotRequired[int],
    CodecLevel: NotRequired[H265CodecLevelType],  # (4)
    CodecProfile: NotRequired[H265CodecProfileType],  # (5)
    DynamicSubGop: NotRequired[H265DynamicSubGopType],  # (6)
    FlickerAdaptiveQuantization: NotRequired[H265FlickerAdaptiveQuantizationType],  # (7)
    FramerateControl: NotRequired[H265FramerateControlType],  # (8)
    FramerateConversionAlgorithm: NotRequired[H265FramerateConversionAlgorithmType],  # (9)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    GopBReference: NotRequired[H265GopBReferenceType],  # (10)
    GopClosedCadence: NotRequired[int],
    GopSize: NotRequired[float],
    GopSizeUnits: NotRequired[H265GopSizeUnitsType],  # (11)
    HrdBufferFinalFillPercentage: NotRequired[int],
    HrdBufferInitialFillPercentage: NotRequired[int],
    HrdBufferSize: NotRequired[int],
    InterlaceMode: NotRequired[H265InterlaceModeType],  # (12)
    MaxBitrate: NotRequired[int],
    MinIInterval: NotRequired[int],
    NumberBFramesBetweenReferenceFrames: NotRequired[int],
    NumberReferenceFrames: NotRequired[int],
    ParControl: NotRequired[H265ParControlType],  # (13)
    ParDenominator: NotRequired[int],
    ParNumerator: NotRequired[int],
    QualityTuningLevel: NotRequired[H265QualityTuningLevelType],  # (14)
    QvbrSettings: NotRequired[H265QvbrSettingsTypeDef],  # (15)
    RateControlMode: NotRequired[H265RateControlModeType],  # (16)
    SampleAdaptiveOffsetFilterMode: NotRequired[H265SampleAdaptiveOffsetFilterModeType],  # (17)
    ScanTypeConversionMode: NotRequired[H265ScanTypeConversionModeType],  # (18)
    SceneChangeDetect: NotRequired[H265SceneChangeDetectType],  # (19)
    Slices: NotRequired[int],
    SlowPal: NotRequired[H265SlowPalType],  # (20)
    SpatialAdaptiveQuantization: NotRequired[H265SpatialAdaptiveQuantizationType],  # (21)
    Telecine: NotRequired[H265TelecineType],  # (22)
    TemporalAdaptiveQuantization: NotRequired[H265TemporalAdaptiveQuantizationType],  # (23)
    TemporalIds: NotRequired[H265TemporalIdsType],  # (24)
    Tiles: NotRequired[H265TilesType],  # (25)
    UnregisteredSeiTimecode: NotRequired[H265UnregisteredSeiTimecodeType],  # (26)
    WriteMp4PackagingType: NotRequired[H265WriteMp4PackagingTypeType],  # (27)
```

1. See [:material-code-brackets: H265AdaptiveQuantizationType](./literals.md#h265adaptivequantizationtype) 
2. See [:material-code-brackets: H265AlternateTransferFunctionSeiType](./literals.md#h265alternatetransferfunctionseitype) 
3. See [:material-code-braces: BandwidthReductionFilterTypeDef](./type_defs.md#bandwidthreductionfiltertypedef) 
4. See [:material-code-brackets: H265CodecLevelType](./literals.md#h265codecleveltype) 
5. See [:material-code-brackets: H265CodecProfileType](./literals.md#h265codecprofiletype) 
6. See [:material-code-brackets: H265DynamicSubGopType](./literals.md#h265dynamicsubgoptype) 
7. See [:material-code-brackets: H265FlickerAdaptiveQuantizationType](./literals.md#h265flickeradaptivequantizationtype) 
8. See [:material-code-brackets: H265FramerateControlType](./literals.md#h265frameratecontroltype) 
9. See [:material-code-brackets: H265FramerateConversionAlgorithmType](./literals.md#h265framerateconversionalgorithmtype) 
10. See [:material-code-brackets: H265GopBReferenceType](./literals.md#h265gopbreferencetype) 
11. See [:material-code-brackets: H265GopSizeUnitsType](./literals.md#h265gopsizeunitstype) 
12. See [:material-code-brackets: H265InterlaceModeType](./literals.md#h265interlacemodetype) 
13. See [:material-code-brackets: H265ParControlType](./literals.md#h265parcontroltype) 
14. See [:material-code-brackets: H265QualityTuningLevelType](./literals.md#h265qualitytuningleveltype) 
15. See [:material-code-braces: H265QvbrSettingsTypeDef](./type_defs.md#h265qvbrsettingstypedef) 
16. See [:material-code-brackets: H265RateControlModeType](./literals.md#h265ratecontrolmodetype) 
17. See [:material-code-brackets: H265SampleAdaptiveOffsetFilterModeType](./literals.md#h265sampleadaptiveoffsetfiltermodetype) 
18. See [:material-code-brackets: H265ScanTypeConversionModeType](./literals.md#h265scantypeconversionmodetype) 
19. See [:material-code-brackets: H265SceneChangeDetectType](./literals.md#h265scenechangedetecttype) 
20. See [:material-code-brackets: H265SlowPalType](./literals.md#h265slowpaltype) 
21. See [:material-code-brackets: H265SpatialAdaptiveQuantizationType](./literals.md#h265spatialadaptivequantizationtype) 
22. See [:material-code-brackets: H265TelecineType](./literals.md#h265telecinetype) 
23. See [:material-code-brackets: H265TemporalAdaptiveQuantizationType](./literals.md#h265temporaladaptivequantizationtype) 
24. See [:material-code-brackets: H265TemporalIdsType](./literals.md#h265temporalidstype) 
25. See [:material-code-brackets: H265TilesType](./literals.md#h265tilestype) 
26. See [:material-code-brackets: H265UnregisteredSeiTimecodeType](./literals.md#h265unregisteredseitimecodetype) 
27. See [:material-code-brackets: H265WriteMp4PackagingTypeType](./literals.md#h265writemp4packagingtypetype) 
## OutputSettingsTypeDef

```python
# OutputSettingsTypeDef definition

class OutputSettingsTypeDef(TypedDict):
    HlsSettings: NotRequired[HlsSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: HlsSettingsTypeDef](./type_defs.md#hlssettingstypedef) 
## TimedMetadataInsertionTypeDef

```python
# TimedMetadataInsertionTypeDef definition

class TimedMetadataInsertionTypeDef(TypedDict):
    Id3Insertions: NotRequired[Sequence[Id3InsertionTypeDef]],  # (1)
```

1. See [:material-code-braces: Id3InsertionTypeDef](./type_defs.md#id3insertiontypedef) 
## ImageInserterTypeDef

```python
# ImageInserterTypeDef definition

class ImageInserterTypeDef(TypedDict):
    InsertableImages: NotRequired[Sequence[InsertableImageTypeDef]],  # (1)
    SdrReferenceWhiteLevel: NotRequired[int],
```

1. See [:material-code-braces: InsertableImageTypeDef](./type_defs.md#insertableimagetypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    ResourceTags: ResourceTagsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagsTypeDef](./type_defs.md#resourcetagstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## M2tsSettingsTypeDef

```python
# M2tsSettingsTypeDef definition

class M2tsSettingsTypeDef(TypedDict):
    AudioBufferModel: NotRequired[M2tsAudioBufferModelType],  # (1)
    AudioDuration: NotRequired[M2tsAudioDurationType],  # (2)
    AudioFramesPerPes: NotRequired[int],
    AudioPids: NotRequired[Sequence[int]],
    Bitrate: NotRequired[int],
    BufferModel: NotRequired[M2tsBufferModelType],  # (3)
    DataPTSControl: NotRequired[M2tsDataPtsControlType],  # (4)
    DvbNitSettings: NotRequired[DvbNitSettingsTypeDef],  # (5)
    DvbSdtSettings: NotRequired[DvbSdtSettingsTypeDef],  # (6)
    DvbSubPids: NotRequired[Sequence[int]],
    DvbTdtSettings: NotRequired[DvbTdtSettingsTypeDef],  # (7)
    DvbTeletextPid: NotRequired[int],
    EbpAudioInterval: NotRequired[M2tsEbpAudioIntervalType],  # (8)
    EbpPlacement: NotRequired[M2tsEbpPlacementType],  # (9)
    EsRateInPes: NotRequired[M2tsEsRateInPesType],  # (10)
    ForceTsVideoEbpOrder: NotRequired[M2tsForceTsVideoEbpOrderType],  # (11)
    FragmentTime: NotRequired[float],
    KlvMetadata: NotRequired[M2tsKlvMetadataType],  # (12)
    MaxPcrInterval: NotRequired[int],
    MinEbpInterval: NotRequired[int],
    NielsenId3: NotRequired[M2tsNielsenId3Type],  # (13)
    NullPacketBitrate: NotRequired[float],
    PatInterval: NotRequired[int],
    PcrControl: NotRequired[M2tsPcrControlType],  # (14)
    PcrPid: NotRequired[int],
    PmtInterval: NotRequired[int],
    PmtPid: NotRequired[int],
    PrivateMetadataPid: NotRequired[int],
    ProgramNumber: NotRequired[int],
    RateMode: NotRequired[M2tsRateModeType],  # (15)
    Scte35Esam: NotRequired[M2tsScte35EsamTypeDef],  # (16)
    Scte35Pid: NotRequired[int],
    Scte35Source: NotRequired[M2tsScte35SourceType],  # (17)
    SegmentationMarkers: NotRequired[M2tsSegmentationMarkersType],  # (18)
    SegmentationStyle: NotRequired[M2tsSegmentationStyleType],  # (19)
    SegmentationTime: NotRequired[float],
    TimedMetadataPid: NotRequired[int],
    TransportStreamId: NotRequired[int],
    VideoPid: NotRequired[int],
```

1. See [:material-code-brackets: M2tsAudioBufferModelType](./literals.md#m2tsaudiobuffermodeltype) 
2. See [:material-code-brackets: M2tsAudioDurationType](./literals.md#m2tsaudiodurationtype) 
3. See [:material-code-brackets: M2tsBufferModelType](./literals.md#m2tsbuffermodeltype) 
4. See [:material-code-brackets: M2tsDataPtsControlType](./literals.md#m2tsdataptscontroltype) 
5. See [:material-code-braces: DvbNitSettingsTypeDef](./type_defs.md#dvbnitsettingstypedef) 
6. See [:material-code-braces: DvbSdtSettingsTypeDef](./type_defs.md#dvbsdtsettingstypedef) 
7. See [:material-code-braces: DvbTdtSettingsTypeDef](./type_defs.md#dvbtdtsettingstypedef) 
8. See [:material-code-brackets: M2tsEbpAudioIntervalType](./literals.md#m2tsebpaudiointervaltype) 
9. See [:material-code-brackets: M2tsEbpPlacementType](./literals.md#m2tsebpplacementtype) 
10. See [:material-code-brackets: M2tsEsRateInPesType](./literals.md#m2tsesrateinpestype) 
11. See [:material-code-brackets: M2tsForceTsVideoEbpOrderType](./literals.md#m2tsforcetsvideoebpordertype) 
12. See [:material-code-brackets: M2tsKlvMetadataType](./literals.md#m2tsklvmetadatatype) 
13. See [:material-code-brackets: M2tsNielsenId3Type](./literals.md#m2tsnielsenid3type) 
14. See [:material-code-brackets: M2tsPcrControlType](./literals.md#m2tspcrcontroltype) 
15. See [:material-code-brackets: M2tsRateModeType](./literals.md#m2tsratemodetype) 
16. See [:material-code-braces: M2tsScte35EsamTypeDef](./type_defs.md#m2tsscte35esamtypedef) 
17. See [:material-code-brackets: M2tsScte35SourceType](./literals.md#m2tsscte35sourcetype) 
18. See [:material-code-brackets: M2tsSegmentationMarkersType](./literals.md#m2tssegmentationmarkerstype) 
19. See [:material-code-brackets: M2tsSegmentationStyleType](./literals.md#m2tssegmentationstyletype) 
## MotionImageInserterTypeDef

```python
# MotionImageInserterTypeDef definition

class MotionImageInserterTypeDef(TypedDict):
    Framerate: NotRequired[MotionImageInsertionFramerateTypeDef],  # (1)
    Input: NotRequired[str],
    InsertionMode: NotRequired[MotionImageInsertionModeType],  # (2)
    Offset: NotRequired[MotionImageInsertionOffsetTypeDef],  # (3)
    Playback: NotRequired[MotionImagePlaybackType],  # (4)
    StartTime: NotRequired[str],
```

1. See [:material-code-braces: MotionImageInsertionFramerateTypeDef](./type_defs.md#motionimageinsertionframeratetypedef) 
2. See [:material-code-brackets: MotionImageInsertionModeType](./literals.md#motionimageinsertionmodetype) 
3. See [:material-code-braces: MotionImageInsertionOffsetTypeDef](./type_defs.md#motionimageinsertionoffsettypedef) 
4. See [:material-code-brackets: MotionImagePlaybackType](./literals.md#motionimageplaybacktype) 
## MxfSettingsTypeDef

```python
# MxfSettingsTypeDef definition

class MxfSettingsTypeDef(TypedDict):
    AfdSignaling: NotRequired[MxfAfdSignalingType],  # (1)
    Profile: NotRequired[MxfProfileType],  # (2)
    XavcProfileSettings: NotRequired[MxfXavcProfileSettingsTypeDef],  # (3)
```

1. See [:material-code-brackets: MxfAfdSignalingType](./literals.md#mxfafdsignalingtype) 
2. See [:material-code-brackets: MxfProfileType](./literals.md#mxfprofiletype) 
3. See [:material-code-braces: MxfXavcProfileSettingsTypeDef](./type_defs.md#mxfxavcprofilesettingstypedef) 
## PartnerWatermarkingTypeDef

```python
# PartnerWatermarkingTypeDef definition

class PartnerWatermarkingTypeDef(TypedDict):
    NexguardFileMarkerSettings: NotRequired[NexGuardFileMarkerSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: NexGuardFileMarkerSettingsTypeDef](./type_defs.md#nexguardfilemarkersettingstypedef) 
## NoiseReducerTypeDef

```python
# NoiseReducerTypeDef definition

class NoiseReducerTypeDef(TypedDict):
    Filter: NotRequired[NoiseReducerFilterType],  # (1)
    FilterSettings: NotRequired[NoiseReducerFilterSettingsTypeDef],  # (2)
    SpatialFilterSettings: NotRequired[NoiseReducerSpatialFilterSettingsTypeDef],  # (3)
    TemporalFilterSettings: NotRequired[NoiseReducerTemporalFilterSettingsTypeDef],  # (4)
```

1. See [:material-code-brackets: NoiseReducerFilterType](./literals.md#noisereducerfiltertype) 
2. See [:material-code-braces: NoiseReducerFilterSettingsTypeDef](./type_defs.md#noisereducerfiltersettingstypedef) 
3. See [:material-code-braces: NoiseReducerSpatialFilterSettingsTypeDef](./type_defs.md#noisereducerspatialfiltersettingstypedef) 
4. See [:material-code-braces: NoiseReducerTemporalFilterSettingsTypeDef](./type_defs.md#noisereducertemporalfiltersettingstypedef) 
## OutputDetailTypeDef

```python
# OutputDetailTypeDef definition

class OutputDetailTypeDef(TypedDict):
    DurationInMs: NotRequired[int],
    VideoDetails: NotRequired[VideoDetailTypeDef],  # (1)
```

1. See [:material-code-braces: VideoDetailTypeDef](./type_defs.md#videodetailtypedef) 
## QueueTypeDef

```python
# QueueTypeDef definition

class QueueTypeDef(TypedDict):
    Name: str,
    Arn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Description: NotRequired[str],
    LastUpdated: NotRequired[datetime],
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    ProgressingJobsCount: NotRequired[int],
    ReservationPlan: NotRequired[ReservationPlanTypeDef],  # (2)
    Status: NotRequired[QueueStatusType],  # (3)
    SubmittedJobsCount: NotRequired[int],
    Type: NotRequired[TypeType],  # (4)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: ReservationPlanTypeDef](./type_defs.md#reservationplantypedef) 
3. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
4. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## S3DestinationSettingsTypeDef

```python
# S3DestinationSettingsTypeDef definition

class S3DestinationSettingsTypeDef(TypedDict):
    AccessControl: NotRequired[S3DestinationAccessControlTypeDef],  # (1)
    Encryption: NotRequired[S3EncryptionSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: S3DestinationAccessControlTypeDef](./type_defs.md#s3destinationaccesscontroltypedef) 
2. See [:material-code-braces: S3EncryptionSettingsTypeDef](./type_defs.md#s3encryptionsettingstypedef) 
## XavcSettingsTypeDef

```python
# XavcSettingsTypeDef definition

class XavcSettingsTypeDef(TypedDict):
    AdaptiveQuantization: NotRequired[XavcAdaptiveQuantizationType],  # (1)
    EntropyEncoding: NotRequired[XavcEntropyEncodingType],  # (2)
    FramerateControl: NotRequired[XavcFramerateControlType],  # (3)
    FramerateConversionAlgorithm: NotRequired[XavcFramerateConversionAlgorithmType],  # (4)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    Profile: NotRequired[XavcProfileType],  # (5)
    SlowPal: NotRequired[XavcSlowPalType],  # (6)
    Softness: NotRequired[int],
    SpatialAdaptiveQuantization: NotRequired[XavcSpatialAdaptiveQuantizationType],  # (7)
    TemporalAdaptiveQuantization: NotRequired[XavcTemporalAdaptiveQuantizationType],  # (8)
    Xavc4kIntraCbgProfileSettings: NotRequired[Xavc4kIntraCbgProfileSettingsTypeDef],  # (9)
    Xavc4kIntraVbrProfileSettings: NotRequired[Xavc4kIntraVbrProfileSettingsTypeDef],  # (10)
    Xavc4kProfileSettings: NotRequired[Xavc4kProfileSettingsTypeDef],  # (11)
    XavcHdIntraCbgProfileSettings: NotRequired[XavcHdIntraCbgProfileSettingsTypeDef],  # (12)
    XavcHdProfileSettings: NotRequired[XavcHdProfileSettingsTypeDef],  # (13)
```

1. See [:material-code-brackets: XavcAdaptiveQuantizationType](./literals.md#xavcadaptivequantizationtype) 
2. See [:material-code-brackets: XavcEntropyEncodingType](./literals.md#xavcentropyencodingtype) 
3. See [:material-code-brackets: XavcFramerateControlType](./literals.md#xavcframeratecontroltype) 
4. See [:material-code-brackets: XavcFramerateConversionAlgorithmType](./literals.md#xavcframerateconversionalgorithmtype) 
5. See [:material-code-brackets: XavcProfileType](./literals.md#xavcprofiletype) 
6. See [:material-code-brackets: XavcSlowPalType](./literals.md#xavcslowpaltype) 
7. See [:material-code-brackets: XavcSpatialAdaptiveQuantizationType](./literals.md#xavcspatialadaptivequantizationtype) 
8. See [:material-code-brackets: XavcTemporalAdaptiveQuantizationType](./literals.md#xavctemporaladaptivequantizationtype) 
9. See [:material-code-braces: Xavc4kIntraCbgProfileSettingsTypeDef](./type_defs.md#xavc4kintracbgprofilesettingstypedef) 
10. See [:material-code-braces: Xavc4kIntraVbrProfileSettingsTypeDef](./type_defs.md#xavc4kintravbrprofilesettingstypedef) 
11. See [:material-code-braces: Xavc4kProfileSettingsTypeDef](./type_defs.md#xavc4kprofilesettingstypedef) 
12. See [:material-code-braces: XavcHdIntraCbgProfileSettingsTypeDef](./type_defs.md#xavchdintracbgprofilesettingstypedef) 
13. See [:material-code-braces: XavcHdProfileSettingsTypeDef](./type_defs.md#xavchdprofilesettingstypedef) 
## AutomatedAbrSettingsTypeDef

```python
# AutomatedAbrSettingsTypeDef definition

class AutomatedAbrSettingsTypeDef(TypedDict):
    MaxAbrBitrate: NotRequired[int],
    MaxRenditions: NotRequired[int],
    MinAbrBitrate: NotRequired[int],
    Rules: NotRequired[Sequence[AutomatedAbrRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: AutomatedAbrRuleTypeDef](./type_defs.md#automatedabrruletypedef) 
## CaptionDescriptionPresetTypeDef

```python
# CaptionDescriptionPresetTypeDef definition

class CaptionDescriptionPresetTypeDef(TypedDict):
    CustomLanguageCode: NotRequired[str],
    DestinationSettings: NotRequired[CaptionDestinationSettingsTypeDef],  # (1)
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    LanguageDescription: NotRequired[str],
```

1. See [:material-code-braces: CaptionDestinationSettingsTypeDef](./type_defs.md#captiondestinationsettingstypedef) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## CaptionDescriptionTypeDef

```python
# CaptionDescriptionTypeDef definition

class CaptionDescriptionTypeDef(TypedDict):
    CaptionSelectorName: NotRequired[str],
    CustomLanguageCode: NotRequired[str],
    DestinationSettings: NotRequired[CaptionDestinationSettingsTypeDef],  # (1)
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    LanguageDescription: NotRequired[str],
```

1. See [:material-code-braces: CaptionDestinationSettingsTypeDef](./type_defs.md#captiondestinationsettingstypedef) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## CaptionSourceSettingsTypeDef

```python
# CaptionSourceSettingsTypeDef definition

class CaptionSourceSettingsTypeDef(TypedDict):
    AncillarySourceSettings: NotRequired[AncillarySourceSettingsTypeDef],  # (1)
    DvbSubSourceSettings: NotRequired[DvbSubSourceSettingsTypeDef],  # (2)
    EmbeddedSourceSettings: NotRequired[EmbeddedSourceSettingsTypeDef],  # (3)
    FileSourceSettings: NotRequired[FileSourceSettingsTypeDef],  # (4)
    SourceType: NotRequired[CaptionSourceTypeType],  # (5)
    TeletextSourceSettings: NotRequired[TeletextSourceSettingsTypeDef],  # (6)
    TrackSourceSettings: NotRequired[TrackSourceSettingsTypeDef],  # (7)
    WebvttHlsSourceSettings: NotRequired[WebvttHlsSourceSettingsTypeDef],  # (8)
```

1. See [:material-code-braces: AncillarySourceSettingsTypeDef](./type_defs.md#ancillarysourcesettingstypedef) 
2. See [:material-code-braces: DvbSubSourceSettingsTypeDef](./type_defs.md#dvbsubsourcesettingstypedef) 
3. See [:material-code-braces: EmbeddedSourceSettingsTypeDef](./type_defs.md#embeddedsourcesettingstypedef) 
4. See [:material-code-braces: FileSourceSettingsTypeDef](./type_defs.md#filesourcesettingstypedef) 
5. See [:material-code-brackets: CaptionSourceTypeType](./literals.md#captionsourcetypetype) 
6. See [:material-code-braces: TeletextSourceSettingsTypeDef](./type_defs.md#teletextsourcesettingstypedef) 
7. See [:material-code-braces: TrackSourceSettingsTypeDef](./type_defs.md#tracksourcesettingstypedef) 
8. See [:material-code-braces: WebvttHlsSourceSettingsTypeDef](./type_defs.md#webvtthlssourcesettingstypedef) 
## RemixSettingsTypeDef

```python
# RemixSettingsTypeDef definition

class RemixSettingsTypeDef(TypedDict):
    ChannelMapping: NotRequired[ChannelMappingTypeDef],  # (1)
    ChannelsIn: NotRequired[int],
    ChannelsOut: NotRequired[int],
```

1. See [:material-code-braces: ChannelMappingTypeDef](./type_defs.md#channelmappingtypedef) 
## ContainerSettingsTypeDef

```python
# ContainerSettingsTypeDef definition

class ContainerSettingsTypeDef(TypedDict):
    CmfcSettings: NotRequired[CmfcSettingsTypeDef],  # (1)
    Container: NotRequired[ContainerTypeType],  # (2)
    F4vSettings: NotRequired[F4vSettingsTypeDef],  # (3)
    M2tsSettings: NotRequired[M2tsSettingsTypeDef],  # (4)
    M3u8Settings: NotRequired[M3u8SettingsTypeDef],  # (5)
    MovSettings: NotRequired[MovSettingsTypeDef],  # (6)
    Mp4Settings: NotRequired[Mp4SettingsTypeDef],  # (7)
    MpdSettings: NotRequired[MpdSettingsTypeDef],  # (8)
    MxfSettings: NotRequired[MxfSettingsTypeDef],  # (9)
```

1. See [:material-code-braces: CmfcSettingsTypeDef](./type_defs.md#cmfcsettingstypedef) 
2. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
3. See [:material-code-braces: F4vSettingsTypeDef](./type_defs.md#f4vsettingstypedef) 
4. See [:material-code-braces: M2tsSettingsTypeDef](./type_defs.md#m2tssettingstypedef) 
5. See [:material-code-braces: M3u8SettingsTypeDef](./type_defs.md#m3u8settingstypedef) 
6. See [:material-code-braces: MovSettingsTypeDef](./type_defs.md#movsettingstypedef) 
7. See [:material-code-braces: Mp4SettingsTypeDef](./type_defs.md#mp4settingstypedef) 
8. See [:material-code-braces: MpdSettingsTypeDef](./type_defs.md#mpdsettingstypedef) 
9. See [:material-code-braces: MxfSettingsTypeDef](./type_defs.md#mxfsettingstypedef) 
## VideoPreprocessorTypeDef

```python
# VideoPreprocessorTypeDef definition

class VideoPreprocessorTypeDef(TypedDict):
    ColorCorrector: NotRequired[ColorCorrectorTypeDef],  # (1)
    Deinterlacer: NotRequired[DeinterlacerTypeDef],  # (2)
    DolbyVision: NotRequired[DolbyVisionTypeDef],  # (3)
    Hdr10Plus: NotRequired[Hdr10PlusTypeDef],  # (4)
    ImageInserter: NotRequired[ImageInserterTypeDef],  # (5)
    NoiseReducer: NotRequired[NoiseReducerTypeDef],  # (6)
    PartnerWatermarking: NotRequired[PartnerWatermarkingTypeDef],  # (7)
    TimecodeBurnin: NotRequired[TimecodeBurninTypeDef],  # (8)
```

1. See [:material-code-braces: ColorCorrectorTypeDef](./type_defs.md#colorcorrectortypedef) 
2. See [:material-code-braces: DeinterlacerTypeDef](./type_defs.md#deinterlacertypedef) 
3. See [:material-code-braces: DolbyVisionTypeDef](./type_defs.md#dolbyvisiontypedef) 
4. See [:material-code-braces: Hdr10PlusTypeDef](./type_defs.md#hdr10plustypedef) 
5. See [:material-code-braces: ImageInserterTypeDef](./type_defs.md#imageinsertertypedef) 
6. See [:material-code-braces: NoiseReducerTypeDef](./type_defs.md#noisereducertypedef) 
7. See [:material-code-braces: PartnerWatermarkingTypeDef](./type_defs.md#partnerwatermarkingtypedef) 
8. See [:material-code-braces: TimecodeBurninTypeDef](./type_defs.md#timecodeburnintypedef) 
## OutputGroupDetailTypeDef

```python
# OutputGroupDetailTypeDef definition

class OutputGroupDetailTypeDef(TypedDict):
    OutputDetails: NotRequired[List[OutputDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: OutputDetailTypeDef](./type_defs.md#outputdetailtypedef) 
## CreateQueueResponseTypeDef

```python
# CreateQueueResponseTypeDef definition

class CreateQueueResponseTypeDef(TypedDict):
    Queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueueResponseTypeDef

```python
# GetQueueResponseTypeDef definition

class GetQueueResponseTypeDef(TypedDict):
    Queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueuesResponseTypeDef

```python
# ListQueuesResponseTypeDef definition

class ListQueuesResponseTypeDef(TypedDict):
    NextToken: str,
    Queues: List[QueueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQueueResponseTypeDef

```python
# UpdateQueueResponseTypeDef definition

class UpdateQueueResponseTypeDef(TypedDict):
    Queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationSettingsTypeDef

```python
# DestinationSettingsTypeDef definition

class DestinationSettingsTypeDef(TypedDict):
    S3Settings: NotRequired[S3DestinationSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: S3DestinationSettingsTypeDef](./type_defs.md#s3destinationsettingstypedef) 
## VideoCodecSettingsTypeDef

```python
# VideoCodecSettingsTypeDef definition

class VideoCodecSettingsTypeDef(TypedDict):
    Av1Settings: NotRequired[Av1SettingsTypeDef],  # (1)
    AvcIntraSettings: NotRequired[AvcIntraSettingsTypeDef],  # (2)
    Codec: NotRequired[VideoCodecType],  # (3)
    FrameCaptureSettings: NotRequired[FrameCaptureSettingsTypeDef],  # (4)
    H264Settings: NotRequired[H264SettingsTypeDef],  # (5)
    H265Settings: NotRequired[H265SettingsTypeDef],  # (6)
    Mpeg2Settings: NotRequired[Mpeg2SettingsTypeDef],  # (7)
    ProresSettings: NotRequired[ProresSettingsTypeDef],  # (8)
    Vc3Settings: NotRequired[Vc3SettingsTypeDef],  # (9)
    Vp8Settings: NotRequired[Vp8SettingsTypeDef],  # (10)
    Vp9Settings: NotRequired[Vp9SettingsTypeDef],  # (11)
    XavcSettings: NotRequired[XavcSettingsTypeDef],  # (12)
```

1. See [:material-code-braces: Av1SettingsTypeDef](./type_defs.md#av1settingstypedef) 
2. See [:material-code-braces: AvcIntraSettingsTypeDef](./type_defs.md#avcintrasettingstypedef) 
3. See [:material-code-brackets: VideoCodecType](./literals.md#videocodectype) 
4. See [:material-code-braces: FrameCaptureSettingsTypeDef](./type_defs.md#framecapturesettingstypedef) 
5. See [:material-code-braces: H264SettingsTypeDef](./type_defs.md#h264settingstypedef) 
6. See [:material-code-braces: H265SettingsTypeDef](./type_defs.md#h265settingstypedef) 
7. See [:material-code-braces: Mpeg2SettingsTypeDef](./type_defs.md#mpeg2settingstypedef) 
8. See [:material-code-braces: ProresSettingsTypeDef](./type_defs.md#proressettingstypedef) 
9. See [:material-code-braces: Vc3SettingsTypeDef](./type_defs.md#vc3settingstypedef) 
10. See [:material-code-braces: Vp8SettingsTypeDef](./type_defs.md#vp8settingstypedef) 
11. See [:material-code-braces: Vp9SettingsTypeDef](./type_defs.md#vp9settingstypedef) 
12. See [:material-code-braces: XavcSettingsTypeDef](./type_defs.md#xavcsettingstypedef) 
## AutomatedEncodingSettingsTypeDef

```python
# AutomatedEncodingSettingsTypeDef definition

class AutomatedEncodingSettingsTypeDef(TypedDict):
    AbrSettings: NotRequired[AutomatedAbrSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: AutomatedAbrSettingsTypeDef](./type_defs.md#automatedabrsettingstypedef) 
## CaptionSelectorTypeDef

```python
# CaptionSelectorTypeDef definition

class CaptionSelectorTypeDef(TypedDict):
    CustomLanguageCode: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    SourceSettings: NotRequired[CaptionSourceSettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: CaptionSourceSettingsTypeDef](./type_defs.md#captionsourcesettingstypedef) 
## AudioDescriptionTypeDef

```python
# AudioDescriptionTypeDef definition

class AudioDescriptionTypeDef(TypedDict):
    AudioChannelTaggingSettings: NotRequired[AudioChannelTaggingSettingsTypeDef],  # (1)
    AudioNormalizationSettings: NotRequired[AudioNormalizationSettingsTypeDef],  # (2)
    AudioSourceName: NotRequired[str],
    AudioType: NotRequired[int],
    AudioTypeControl: NotRequired[AudioTypeControlType],  # (3)
    CodecSettings: NotRequired[AudioCodecSettingsTypeDef],  # (4)
    CustomLanguageCode: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (5)
    LanguageCodeControl: NotRequired[AudioLanguageCodeControlType],  # (6)
    RemixSettings: NotRequired[RemixSettingsTypeDef],  # (7)
    StreamName: NotRequired[str],
```

1. See [:material-code-braces: AudioChannelTaggingSettingsTypeDef](./type_defs.md#audiochanneltaggingsettingstypedef) 
2. See [:material-code-braces: AudioNormalizationSettingsTypeDef](./type_defs.md#audionormalizationsettingstypedef) 
3. See [:material-code-brackets: AudioTypeControlType](./literals.md#audiotypecontroltype) 
4. See [:material-code-braces: AudioCodecSettingsTypeDef](./type_defs.md#audiocodecsettingstypedef) 
5. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
6. See [:material-code-brackets: AudioLanguageCodeControlType](./literals.md#audiolanguagecodecontroltype) 
7. See [:material-code-braces: RemixSettingsTypeDef](./type_defs.md#remixsettingstypedef) 
## AudioSelectorTypeDef

```python
# AudioSelectorTypeDef definition

class AudioSelectorTypeDef(TypedDict):
    AudioDurationCorrection: NotRequired[AudioDurationCorrectionType],  # (1)
    CustomLanguageCode: NotRequired[str],
    DefaultSelection: NotRequired[AudioDefaultSelectionType],  # (2)
    ExternalAudioFileInput: NotRequired[str],
    HlsRenditionGroupSettings: NotRequired[HlsRenditionGroupSettingsTypeDef],  # (3)
    LanguageCode: NotRequired[LanguageCodeType],  # (4)
    Offset: NotRequired[int],
    Pids: NotRequired[Sequence[int]],
    ProgramSelection: NotRequired[int],
    RemixSettings: NotRequired[RemixSettingsTypeDef],  # (5)
    SelectorType: NotRequired[AudioSelectorTypeType],  # (6)
    Tracks: NotRequired[Sequence[int]],
```

1. See [:material-code-brackets: AudioDurationCorrectionType](./literals.md#audiodurationcorrectiontype) 
2. See [:material-code-brackets: AudioDefaultSelectionType](./literals.md#audiodefaultselectiontype) 
3. See [:material-code-braces: HlsRenditionGroupSettingsTypeDef](./type_defs.md#hlsrenditiongroupsettingstypedef) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-braces: RemixSettingsTypeDef](./type_defs.md#remixsettingstypedef) 
6. See [:material-code-brackets: AudioSelectorTypeType](./literals.md#audioselectortypetype) 
## CmafGroupSettingsTypeDef

```python
# CmafGroupSettingsTypeDef definition

class CmafGroupSettingsTypeDef(TypedDict):
    AdditionalManifests: NotRequired[Sequence[CmafAdditionalManifestTypeDef]],  # (1)
    BaseUrl: NotRequired[str],
    ClientCache: NotRequired[CmafClientCacheType],  # (2)
    CodecSpecification: NotRequired[CmafCodecSpecificationType],  # (3)
    DashManifestStyle: NotRequired[DashManifestStyleType],  # (4)
    Destination: NotRequired[str],
    DestinationSettings: NotRequired[DestinationSettingsTypeDef],  # (5)
    Encryption: NotRequired[CmafEncryptionSettingsTypeDef],  # (6)
    FragmentLength: NotRequired[int],
    ImageBasedTrickPlay: NotRequired[CmafImageBasedTrickPlayType],  # (7)
    ImageBasedTrickPlaySettings: NotRequired[CmafImageBasedTrickPlaySettingsTypeDef],  # (8)
    ManifestCompression: NotRequired[CmafManifestCompressionType],  # (9)
    ManifestDurationFormat: NotRequired[CmafManifestDurationFormatType],  # (10)
    MinBufferTime: NotRequired[int],
    MinFinalSegmentLength: NotRequired[float],
    MpdManifestBandwidthType: NotRequired[CmafMpdManifestBandwidthTypeType],  # (11)
    MpdProfile: NotRequired[CmafMpdProfileType],  # (12)
    PtsOffsetHandlingForBFrames: NotRequired[CmafPtsOffsetHandlingForBFramesType],  # (13)
    SegmentControl: NotRequired[CmafSegmentControlType],  # (14)
    SegmentLength: NotRequired[int],
    SegmentLengthControl: NotRequired[CmafSegmentLengthControlType],  # (15)
    StreamInfResolution: NotRequired[CmafStreamInfResolutionType],  # (16)
    TargetDurationCompatibilityMode: NotRequired[CmafTargetDurationCompatibilityModeType],  # (17)
    VideoCompositionOffsets: NotRequired[CmafVideoCompositionOffsetsType],  # (18)
    WriteDashManifest: NotRequired[CmafWriteDASHManifestType],  # (19)
    WriteHlsManifest: NotRequired[CmafWriteHLSManifestType],  # (20)
    WriteSegmentTimelineInRepresentation: NotRequired[CmafWriteSegmentTimelineInRepresentationType],  # (21)
```

1. See [:material-code-braces: CmafAdditionalManifestTypeDef](./type_defs.md#cmafadditionalmanifesttypedef) 
2. See [:material-code-brackets: CmafClientCacheType](./literals.md#cmafclientcachetype) 
3. See [:material-code-brackets: CmafCodecSpecificationType](./literals.md#cmafcodecspecificationtype) 
4. See [:material-code-brackets: DashManifestStyleType](./literals.md#dashmanifeststyletype) 
5. See [:material-code-braces: DestinationSettingsTypeDef](./type_defs.md#destinationsettingstypedef) 
6. See [:material-code-braces: CmafEncryptionSettingsTypeDef](./type_defs.md#cmafencryptionsettingstypedef) 
7. See [:material-code-brackets: CmafImageBasedTrickPlayType](./literals.md#cmafimagebasedtrickplaytype) 
8. See [:material-code-braces: CmafImageBasedTrickPlaySettingsTypeDef](./type_defs.md#cmafimagebasedtrickplaysettingstypedef) 
9. See [:material-code-brackets: CmafManifestCompressionType](./literals.md#cmafmanifestcompressiontype) 
10. See [:material-code-brackets: CmafManifestDurationFormatType](./literals.md#cmafmanifestdurationformattype) 
11. See [:material-code-brackets: CmafMpdManifestBandwidthTypeType](./literals.md#cmafmpdmanifestbandwidthtypetype) 
12. See [:material-code-brackets: CmafMpdProfileType](./literals.md#cmafmpdprofiletype) 
13. See [:material-code-brackets: CmafPtsOffsetHandlingForBFramesType](./literals.md#cmafptsoffsethandlingforbframestype) 
14. See [:material-code-brackets: CmafSegmentControlType](./literals.md#cmafsegmentcontroltype) 
15. See [:material-code-brackets: CmafSegmentLengthControlType](./literals.md#cmafsegmentlengthcontroltype) 
16. See [:material-code-brackets: CmafStreamInfResolutionType](./literals.md#cmafstreaminfresolutiontype) 
17. See [:material-code-brackets: CmafTargetDurationCompatibilityModeType](./literals.md#cmaftargetdurationcompatibilitymodetype) 
18. See [:material-code-brackets: CmafVideoCompositionOffsetsType](./literals.md#cmafvideocompositionoffsetstype) 
19. See [:material-code-brackets: CmafWriteDASHManifestType](./literals.md#cmafwritedashmanifesttype) 
20. See [:material-code-brackets: CmafWriteHLSManifestType](./literals.md#cmafwritehlsmanifesttype) 
21. See [:material-code-brackets: CmafWriteSegmentTimelineInRepresentationType](./literals.md#cmafwritesegmenttimelineinrepresentationtype) 
## DashIsoGroupSettingsTypeDef

```python
# DashIsoGroupSettingsTypeDef definition

class DashIsoGroupSettingsTypeDef(TypedDict):
    AdditionalManifests: NotRequired[Sequence[DashAdditionalManifestTypeDef]],  # (1)
    AudioChannelConfigSchemeIdUri: NotRequired[DashIsoGroupAudioChannelConfigSchemeIdUriType],  # (2)
    BaseUrl: NotRequired[str],
    DashManifestStyle: NotRequired[DashManifestStyleType],  # (3)
    Destination: NotRequired[str],
    DestinationSettings: NotRequired[DestinationSettingsTypeDef],  # (4)
    Encryption: NotRequired[DashIsoEncryptionSettingsTypeDef],  # (5)
    FragmentLength: NotRequired[int],
    HbbtvCompliance: NotRequired[DashIsoHbbtvComplianceType],  # (6)
    ImageBasedTrickPlay: NotRequired[DashIsoImageBasedTrickPlayType],  # (7)
    ImageBasedTrickPlaySettings: NotRequired[DashIsoImageBasedTrickPlaySettingsTypeDef],  # (8)
    MinBufferTime: NotRequired[int],
    MinFinalSegmentLength: NotRequired[float],
    MpdManifestBandwidthType: NotRequired[DashIsoMpdManifestBandwidthTypeType],  # (9)
    MpdProfile: NotRequired[DashIsoMpdProfileType],  # (10)
    PtsOffsetHandlingForBFrames: NotRequired[DashIsoPtsOffsetHandlingForBFramesType],  # (11)
    SegmentControl: NotRequired[DashIsoSegmentControlType],  # (12)
    SegmentLength: NotRequired[int],
    SegmentLengthControl: NotRequired[DashIsoSegmentLengthControlType],  # (13)
    VideoCompositionOffsets: NotRequired[DashIsoVideoCompositionOffsetsType],  # (14)
    WriteSegmentTimelineInRepresentation: NotRequired[DashIsoWriteSegmentTimelineInRepresentationType],  # (15)
```

1. See [:material-code-braces: DashAdditionalManifestTypeDef](./type_defs.md#dashadditionalmanifesttypedef) 
2. See [:material-code-brackets: DashIsoGroupAudioChannelConfigSchemeIdUriType](./literals.md#dashisogroupaudiochannelconfigschemeiduritype) 
3. See [:material-code-brackets: DashManifestStyleType](./literals.md#dashmanifeststyletype) 
4. See [:material-code-braces: DestinationSettingsTypeDef](./type_defs.md#destinationsettingstypedef) 
5. See [:material-code-braces: DashIsoEncryptionSettingsTypeDef](./type_defs.md#dashisoencryptionsettingstypedef) 
6. See [:material-code-brackets: DashIsoHbbtvComplianceType](./literals.md#dashisohbbtvcompliancetype) 
7. See [:material-code-brackets: DashIsoImageBasedTrickPlayType](./literals.md#dashisoimagebasedtrickplaytype) 
8. See [:material-code-braces: DashIsoImageBasedTrickPlaySettingsTypeDef](./type_defs.md#dashisoimagebasedtrickplaysettingstypedef) 
9. See [:material-code-brackets: DashIsoMpdManifestBandwidthTypeType](./literals.md#dashisompdmanifestbandwidthtypetype) 
10. See [:material-code-brackets: DashIsoMpdProfileType](./literals.md#dashisompdprofiletype) 
11. See [:material-code-brackets: DashIsoPtsOffsetHandlingForBFramesType](./literals.md#dashisoptsoffsethandlingforbframestype) 
12. See [:material-code-brackets: DashIsoSegmentControlType](./literals.md#dashisosegmentcontroltype) 
13. See [:material-code-brackets: DashIsoSegmentLengthControlType](./literals.md#dashisosegmentlengthcontroltype) 
14. See [:material-code-brackets: DashIsoVideoCompositionOffsetsType](./literals.md#dashisovideocompositionoffsetstype) 
15. See [:material-code-brackets: DashIsoWriteSegmentTimelineInRepresentationType](./literals.md#dashisowritesegmenttimelineinrepresentationtype) 
## FileGroupSettingsTypeDef

```python
# FileGroupSettingsTypeDef definition

class FileGroupSettingsTypeDef(TypedDict):
    Destination: NotRequired[str],
    DestinationSettings: NotRequired[DestinationSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: DestinationSettingsTypeDef](./type_defs.md#destinationsettingstypedef) 
## HlsGroupSettingsTypeDef

```python
# HlsGroupSettingsTypeDef definition

class HlsGroupSettingsTypeDef(TypedDict):
    AdMarkers: NotRequired[Sequence[HlsAdMarkersType]],  # (1)
    AdditionalManifests: NotRequired[Sequence[HlsAdditionalManifestTypeDef]],  # (2)
    AudioOnlyHeader: NotRequired[HlsAudioOnlyHeaderType],  # (3)
    BaseUrl: NotRequired[str],
    CaptionLanguageMappings: NotRequired[Sequence[HlsCaptionLanguageMappingTypeDef]],  # (4)
    CaptionLanguageSetting: NotRequired[HlsCaptionLanguageSettingType],  # (5)
    CaptionSegmentLengthControl: NotRequired[HlsCaptionSegmentLengthControlType],  # (6)
    ClientCache: NotRequired[HlsClientCacheType],  # (7)
    CodecSpecification: NotRequired[HlsCodecSpecificationType],  # (8)
    Destination: NotRequired[str],
    DestinationSettings: NotRequired[DestinationSettingsTypeDef],  # (9)
    DirectoryStructure: NotRequired[HlsDirectoryStructureType],  # (10)
    Encryption: NotRequired[HlsEncryptionSettingsTypeDef],  # (11)
    ImageBasedTrickPlay: NotRequired[HlsImageBasedTrickPlayType],  # (12)
    ImageBasedTrickPlaySettings: NotRequired[HlsImageBasedTrickPlaySettingsTypeDef],  # (13)
    ManifestCompression: NotRequired[HlsManifestCompressionType],  # (14)
    ManifestDurationFormat: NotRequired[HlsManifestDurationFormatType],  # (15)
    MinFinalSegmentLength: NotRequired[float],
    MinSegmentLength: NotRequired[int],
    OutputSelection: NotRequired[HlsOutputSelectionType],  # (16)
    ProgramDateTime: NotRequired[HlsProgramDateTimeType],  # (17)
    ProgramDateTimePeriod: NotRequired[int],
    ProgressiveWriteHlsManifest: NotRequired[HlsProgressiveWriteHlsManifestType],  # (18)
    SegmentControl: NotRequired[HlsSegmentControlType],  # (19)
    SegmentLength: NotRequired[int],
    SegmentLengthControl: NotRequired[HlsSegmentLengthControlType],  # (20)
    SegmentsPerSubdirectory: NotRequired[int],
    StreamInfResolution: NotRequired[HlsStreamInfResolutionType],  # (21)
    TargetDurationCompatibilityMode: NotRequired[HlsTargetDurationCompatibilityModeType],  # (22)
    TimedMetadataId3Frame: NotRequired[HlsTimedMetadataId3FrameType],  # (23)
    TimedMetadataId3Period: NotRequired[int],
    TimestampDeltaMilliseconds: NotRequired[int],
```

1. See [:material-code-brackets: HlsAdMarkersType](./literals.md#hlsadmarkerstype) 
2. See [:material-code-braces: HlsAdditionalManifestTypeDef](./type_defs.md#hlsadditionalmanifesttypedef) 
3. See [:material-code-brackets: HlsAudioOnlyHeaderType](./literals.md#hlsaudioonlyheadertype) 
4. See [:material-code-braces: HlsCaptionLanguageMappingTypeDef](./type_defs.md#hlscaptionlanguagemappingtypedef) 
5. See [:material-code-brackets: HlsCaptionLanguageSettingType](./literals.md#hlscaptionlanguagesettingtype) 
6. See [:material-code-brackets: HlsCaptionSegmentLengthControlType](./literals.md#hlscaptionsegmentlengthcontroltype) 
7. See [:material-code-brackets: HlsClientCacheType](./literals.md#hlsclientcachetype) 
8. See [:material-code-brackets: HlsCodecSpecificationType](./literals.md#hlscodecspecificationtype) 
9. See [:material-code-braces: DestinationSettingsTypeDef](./type_defs.md#destinationsettingstypedef) 
10. See [:material-code-brackets: HlsDirectoryStructureType](./literals.md#hlsdirectorystructuretype) 
11. See [:material-code-braces: HlsEncryptionSettingsTypeDef](./type_defs.md#hlsencryptionsettingstypedef) 
12. See [:material-code-brackets: HlsImageBasedTrickPlayType](./literals.md#hlsimagebasedtrickplaytype) 
13. See [:material-code-braces: HlsImageBasedTrickPlaySettingsTypeDef](./type_defs.md#hlsimagebasedtrickplaysettingstypedef) 
14. See [:material-code-brackets: HlsManifestCompressionType](./literals.md#hlsmanifestcompressiontype) 
15. See [:material-code-brackets: HlsManifestDurationFormatType](./literals.md#hlsmanifestdurationformattype) 
16. See [:material-code-brackets: HlsOutputSelectionType](./literals.md#hlsoutputselectiontype) 
17. See [:material-code-brackets: HlsProgramDateTimeType](./literals.md#hlsprogramdatetimetype) 
18. See [:material-code-brackets: HlsProgressiveWriteHlsManifestType](./literals.md#hlsprogressivewritehlsmanifesttype) 
19. See [:material-code-brackets: HlsSegmentControlType](./literals.md#hlssegmentcontroltype) 
20. See [:material-code-brackets: HlsSegmentLengthControlType](./literals.md#hlssegmentlengthcontroltype) 
21. See [:material-code-brackets: HlsStreamInfResolutionType](./literals.md#hlsstreaminfresolutiontype) 
22. See [:material-code-brackets: HlsTargetDurationCompatibilityModeType](./literals.md#hlstargetdurationcompatibilitymodetype) 
23. See [:material-code-brackets: HlsTimedMetadataId3FrameType](./literals.md#hlstimedmetadataid3frametype) 
## MsSmoothGroupSettingsTypeDef

```python
# MsSmoothGroupSettingsTypeDef definition

class MsSmoothGroupSettingsTypeDef(TypedDict):
    AdditionalManifests: NotRequired[Sequence[MsSmoothAdditionalManifestTypeDef]],  # (1)
    AudioDeduplication: NotRequired[MsSmoothAudioDeduplicationType],  # (2)
    Destination: NotRequired[str],
    DestinationSettings: NotRequired[DestinationSettingsTypeDef],  # (3)
    Encryption: NotRequired[MsSmoothEncryptionSettingsTypeDef],  # (4)
    FragmentLength: NotRequired[int],
    FragmentLengthControl: NotRequired[MsSmoothFragmentLengthControlType],  # (5)
    ManifestEncoding: NotRequired[MsSmoothManifestEncodingType],  # (6)
```

1. See [:material-code-braces: MsSmoothAdditionalManifestTypeDef](./type_defs.md#mssmoothadditionalmanifesttypedef) 
2. See [:material-code-brackets: MsSmoothAudioDeduplicationType](./literals.md#mssmoothaudiodeduplicationtype) 
3. See [:material-code-braces: DestinationSettingsTypeDef](./type_defs.md#destinationsettingstypedef) 
4. See [:material-code-braces: MsSmoothEncryptionSettingsTypeDef](./type_defs.md#mssmoothencryptionsettingstypedef) 
5. See [:material-code-brackets: MsSmoothFragmentLengthControlType](./literals.md#mssmoothfragmentlengthcontroltype) 
6. See [:material-code-brackets: MsSmoothManifestEncodingType](./literals.md#mssmoothmanifestencodingtype) 
## VideoDescriptionTypeDef

```python
# VideoDescriptionTypeDef definition

class VideoDescriptionTypeDef(TypedDict):
    AfdSignaling: NotRequired[AfdSignalingType],  # (1)
    AntiAlias: NotRequired[AntiAliasType],  # (2)
    CodecSettings: NotRequired[VideoCodecSettingsTypeDef],  # (3)
    ColorMetadata: NotRequired[ColorMetadataType],  # (4)
    Crop: NotRequired[RectangleTypeDef],  # (5)
    DropFrameTimecode: NotRequired[DropFrameTimecodeType],  # (6)
    FixedAfd: NotRequired[int],
    Height: NotRequired[int],
    Position: NotRequired[RectangleTypeDef],  # (5)
    RespondToAfd: NotRequired[RespondToAfdType],  # (8)
    ScalingBehavior: NotRequired[ScalingBehaviorType],  # (9)
    Sharpness: NotRequired[int],
    TimecodeInsertion: NotRequired[VideoTimecodeInsertionType],  # (10)
    VideoPreprocessors: NotRequired[VideoPreprocessorTypeDef],  # (11)
    Width: NotRequired[int],
```

1. See [:material-code-brackets: AfdSignalingType](./literals.md#afdsignalingtype) 
2. See [:material-code-brackets: AntiAliasType](./literals.md#antialiastype) 
3. See [:material-code-braces: VideoCodecSettingsTypeDef](./type_defs.md#videocodecsettingstypedef) 
4. See [:material-code-brackets: ColorMetadataType](./literals.md#colormetadatatype) 
5. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
6. See [:material-code-brackets: DropFrameTimecodeType](./literals.md#dropframetimecodetype) 
7. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
8. See [:material-code-brackets: RespondToAfdType](./literals.md#respondtoafdtype) 
9. See [:material-code-brackets: ScalingBehaviorType](./literals.md#scalingbehaviortype) 
10. See [:material-code-brackets: VideoTimecodeInsertionType](./literals.md#videotimecodeinsertiontype) 
11. See [:material-code-braces: VideoPreprocessorTypeDef](./type_defs.md#videopreprocessortypedef) 
## InputTemplateTypeDef

```python
# InputTemplateTypeDef definition

class InputTemplateTypeDef(TypedDict):
    AdvancedInputFilter: NotRequired[AdvancedInputFilterType],  # (1)
    AdvancedInputFilterSettings: NotRequired[AdvancedInputFilterSettingsTypeDef],  # (2)
    AudioSelectorGroups: NotRequired[Mapping[str, AudioSelectorGroupTypeDef]],  # (3)
    AudioSelectors: NotRequired[Mapping[str, AudioSelectorTypeDef]],  # (4)
    CaptionSelectors: NotRequired[Mapping[str, CaptionSelectorTypeDef]],  # (5)
    Crop: NotRequired[RectangleTypeDef],  # (6)
    DeblockFilter: NotRequired[InputDeblockFilterType],  # (7)
    DenoiseFilter: NotRequired[InputDenoiseFilterType],  # (8)
    DolbyVisionMetadataXml: NotRequired[str],
    FilterEnable: NotRequired[InputFilterEnableType],  # (9)
    FilterStrength: NotRequired[int],
    ImageInserter: NotRequired[ImageInserterTypeDef],  # (10)
    InputClippings: NotRequired[Sequence[InputClippingTypeDef]],  # (11)
    InputScanType: NotRequired[InputScanTypeType],  # (12)
    Position: NotRequired[RectangleTypeDef],  # (6)
    ProgramNumber: NotRequired[int],
    PsiControl: NotRequired[InputPsiControlType],  # (14)
    TimecodeSource: NotRequired[InputTimecodeSourceType],  # (15)
    TimecodeStart: NotRequired[str],
    VideoSelector: NotRequired[VideoSelectorTypeDef],  # (16)
```

1. See [:material-code-brackets: AdvancedInputFilterType](./literals.md#advancedinputfiltertype) 
2. See [:material-code-braces: AdvancedInputFilterSettingsTypeDef](./type_defs.md#advancedinputfiltersettingstypedef) 
3. See [:material-code-braces: AudioSelectorGroupTypeDef](./type_defs.md#audioselectorgrouptypedef) 
4. See [:material-code-braces: AudioSelectorTypeDef](./type_defs.md#audioselectortypedef) 
5. See [:material-code-braces: CaptionSelectorTypeDef](./type_defs.md#captionselectortypedef) 
6. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
7. See [:material-code-brackets: InputDeblockFilterType](./literals.md#inputdeblockfiltertype) 
8. See [:material-code-brackets: InputDenoiseFilterType](./literals.md#inputdenoisefiltertype) 
9. See [:material-code-brackets: InputFilterEnableType](./literals.md#inputfilterenabletype) 
10. See [:material-code-braces: ImageInserterTypeDef](./type_defs.md#imageinsertertypedef) 
11. See [:material-code-braces: InputClippingTypeDef](./type_defs.md#inputclippingtypedef) 
12. See [:material-code-brackets: InputScanTypeType](./literals.md#inputscantypetype) 
13. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
14. See [:material-code-brackets: InputPsiControlType](./literals.md#inputpsicontroltype) 
15. See [:material-code-brackets: InputTimecodeSourceType](./literals.md#inputtimecodesourcetype) 
16. See [:material-code-braces: VideoSelectorTypeDef](./type_defs.md#videoselectortypedef) 
## InputTypeDef

```python
# InputTypeDef definition

class InputTypeDef(TypedDict):
    AdvancedInputFilter: NotRequired[AdvancedInputFilterType],  # (1)
    AdvancedInputFilterSettings: NotRequired[AdvancedInputFilterSettingsTypeDef],  # (2)
    AudioSelectorGroups: NotRequired[Mapping[str, AudioSelectorGroupTypeDef]],  # (3)
    AudioSelectors: NotRequired[Mapping[str, AudioSelectorTypeDef]],  # (4)
    CaptionSelectors: NotRequired[Mapping[str, CaptionSelectorTypeDef]],  # (5)
    Crop: NotRequired[RectangleTypeDef],  # (6)
    DeblockFilter: NotRequired[InputDeblockFilterType],  # (7)
    DecryptionSettings: NotRequired[InputDecryptionSettingsTypeDef],  # (8)
    DenoiseFilter: NotRequired[InputDenoiseFilterType],  # (9)
    DolbyVisionMetadataXml: NotRequired[str],
    FileInput: NotRequired[str],
    FilterEnable: NotRequired[InputFilterEnableType],  # (10)
    FilterStrength: NotRequired[int],
    ImageInserter: NotRequired[ImageInserterTypeDef],  # (11)
    InputClippings: NotRequired[Sequence[InputClippingTypeDef]],  # (12)
    InputScanType: NotRequired[InputScanTypeType],  # (13)
    Position: NotRequired[RectangleTypeDef],  # (6)
    ProgramNumber: NotRequired[int],
    PsiControl: NotRequired[InputPsiControlType],  # (15)
    SupplementalImps: NotRequired[Sequence[str]],
    TimecodeSource: NotRequired[InputTimecodeSourceType],  # (16)
    TimecodeStart: NotRequired[str],
    VideoGenerator: NotRequired[InputVideoGeneratorTypeDef],  # (17)
    VideoSelector: NotRequired[VideoSelectorTypeDef],  # (18)
```

1. See [:material-code-brackets: AdvancedInputFilterType](./literals.md#advancedinputfiltertype) 
2. See [:material-code-braces: AdvancedInputFilterSettingsTypeDef](./type_defs.md#advancedinputfiltersettingstypedef) 
3. See [:material-code-braces: AudioSelectorGroupTypeDef](./type_defs.md#audioselectorgrouptypedef) 
4. See [:material-code-braces: AudioSelectorTypeDef](./type_defs.md#audioselectortypedef) 
5. See [:material-code-braces: CaptionSelectorTypeDef](./type_defs.md#captionselectortypedef) 
6. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
7. See [:material-code-brackets: InputDeblockFilterType](./literals.md#inputdeblockfiltertype) 
8. See [:material-code-braces: InputDecryptionSettingsTypeDef](./type_defs.md#inputdecryptionsettingstypedef) 
9. See [:material-code-brackets: InputDenoiseFilterType](./literals.md#inputdenoisefiltertype) 
10. See [:material-code-brackets: InputFilterEnableType](./literals.md#inputfilterenabletype) 
11. See [:material-code-braces: ImageInserterTypeDef](./type_defs.md#imageinsertertypedef) 
12. See [:material-code-braces: InputClippingTypeDef](./type_defs.md#inputclippingtypedef) 
13. See [:material-code-brackets: InputScanTypeType](./literals.md#inputscantypetype) 
14. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
15. See [:material-code-brackets: InputPsiControlType](./literals.md#inputpsicontroltype) 
16. See [:material-code-brackets: InputTimecodeSourceType](./literals.md#inputtimecodesourcetype) 
17. See [:material-code-braces: InputVideoGeneratorTypeDef](./type_defs.md#inputvideogeneratortypedef) 
18. See [:material-code-braces: VideoSelectorTypeDef](./type_defs.md#videoselectortypedef) 
## OutputGroupSettingsTypeDef

```python
# OutputGroupSettingsTypeDef definition

class OutputGroupSettingsTypeDef(TypedDict):
    CmafGroupSettings: NotRequired[CmafGroupSettingsTypeDef],  # (1)
    DashIsoGroupSettings: NotRequired[DashIsoGroupSettingsTypeDef],  # (2)
    FileGroupSettings: NotRequired[FileGroupSettingsTypeDef],  # (3)
    HlsGroupSettings: NotRequired[HlsGroupSettingsTypeDef],  # (4)
    MsSmoothGroupSettings: NotRequired[MsSmoothGroupSettingsTypeDef],  # (5)
    Type: NotRequired[OutputGroupTypeType],  # (6)
```

1. See [:material-code-braces: CmafGroupSettingsTypeDef](./type_defs.md#cmafgroupsettingstypedef) 
2. See [:material-code-braces: DashIsoGroupSettingsTypeDef](./type_defs.md#dashisogroupsettingstypedef) 
3. See [:material-code-braces: FileGroupSettingsTypeDef](./type_defs.md#filegroupsettingstypedef) 
4. See [:material-code-braces: HlsGroupSettingsTypeDef](./type_defs.md#hlsgroupsettingstypedef) 
5. See [:material-code-braces: MsSmoothGroupSettingsTypeDef](./type_defs.md#mssmoothgroupsettingstypedef) 
6. See [:material-code-brackets: OutputGroupTypeType](./literals.md#outputgrouptypetype) 
## OutputTypeDef

```python
# OutputTypeDef definition

class OutputTypeDef(TypedDict):
    AudioDescriptions: NotRequired[Sequence[AudioDescriptionTypeDef]],  # (1)
    CaptionDescriptions: NotRequired[Sequence[CaptionDescriptionTypeDef]],  # (2)
    ContainerSettings: NotRequired[ContainerSettingsTypeDef],  # (3)
    Extension: NotRequired[str],
    NameModifier: NotRequired[str],
    OutputSettings: NotRequired[OutputSettingsTypeDef],  # (4)
    Preset: NotRequired[str],
    VideoDescription: NotRequired[VideoDescriptionTypeDef],  # (5)
```

1. See [:material-code-braces: AudioDescriptionTypeDef](./type_defs.md#audiodescriptiontypedef) 
2. See [:material-code-braces: CaptionDescriptionTypeDef](./type_defs.md#captiondescriptiontypedef) 
3. See [:material-code-braces: ContainerSettingsTypeDef](./type_defs.md#containersettingstypedef) 
4. See [:material-code-braces: OutputSettingsTypeDef](./type_defs.md#outputsettingstypedef) 
5. See [:material-code-braces: VideoDescriptionTypeDef](./type_defs.md#videodescriptiontypedef) 
## PresetSettingsTypeDef

```python
# PresetSettingsTypeDef definition

class PresetSettingsTypeDef(TypedDict):
    AudioDescriptions: NotRequired[Sequence[AudioDescriptionTypeDef]],  # (1)
    CaptionDescriptions: NotRequired[Sequence[CaptionDescriptionPresetTypeDef]],  # (2)
    ContainerSettings: NotRequired[ContainerSettingsTypeDef],  # (3)
    VideoDescription: NotRequired[VideoDescriptionTypeDef],  # (4)
```

1. See [:material-code-braces: AudioDescriptionTypeDef](./type_defs.md#audiodescriptiontypedef) 
2. See [:material-code-braces: CaptionDescriptionPresetTypeDef](./type_defs.md#captiondescriptionpresettypedef) 
3. See [:material-code-braces: ContainerSettingsTypeDef](./type_defs.md#containersettingstypedef) 
4. See [:material-code-braces: VideoDescriptionTypeDef](./type_defs.md#videodescriptiontypedef) 
## OutputGroupTypeDef

```python
# OutputGroupTypeDef definition

class OutputGroupTypeDef(TypedDict):
    AutomatedEncodingSettings: NotRequired[AutomatedEncodingSettingsTypeDef],  # (1)
    CustomName: NotRequired[str],
    Name: NotRequired[str],
    OutputGroupSettings: NotRequired[OutputGroupSettingsTypeDef],  # (2)
    Outputs: NotRequired[Sequence[OutputTypeDef]],  # (3)
```

1. See [:material-code-braces: AutomatedEncodingSettingsTypeDef](./type_defs.md#automatedencodingsettingstypedef) 
2. See [:material-code-braces: OutputGroupSettingsTypeDef](./type_defs.md#outputgroupsettingstypedef) 
3. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
## CreatePresetRequestRequestTypeDef

```python
# CreatePresetRequestRequestTypeDef definition

class CreatePresetRequestRequestTypeDef(TypedDict):
    Name: str,
    Settings: PresetSettingsTypeDef,  # (1)
    Category: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: PresetSettingsTypeDef](./type_defs.md#presetsettingstypedef) 
## PresetTypeDef

```python
# PresetTypeDef definition

class PresetTypeDef(TypedDict):
    Name: str,
    Settings: PresetSettingsTypeDef,  # (1)
    Arn: NotRequired[str],
    Category: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Description: NotRequired[str],
    LastUpdated: NotRequired[datetime],
    Type: NotRequired[TypeType],  # (2)
```

1. See [:material-code-braces: PresetSettingsTypeDef](./type_defs.md#presetsettingstypedef) 
2. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## UpdatePresetRequestRequestTypeDef

```python
# UpdatePresetRequestRequestTypeDef definition

class UpdatePresetRequestRequestTypeDef(TypedDict):
    Name: str,
    Category: NotRequired[str],
    Description: NotRequired[str],
    Settings: NotRequired[PresetSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: PresetSettingsTypeDef](./type_defs.md#presetsettingstypedef) 
## JobSettingsTypeDef

```python
# JobSettingsTypeDef definition

class JobSettingsTypeDef(TypedDict):
    AdAvailOffset: NotRequired[int],
    AvailBlanking: NotRequired[AvailBlankingTypeDef],  # (1)
    Esam: NotRequired[EsamSettingsTypeDef],  # (2)
    ExtendedDataServices: NotRequired[ExtendedDataServicesTypeDef],  # (3)
    Inputs: NotRequired[Sequence[InputTypeDef]],  # (4)
    KantarWatermark: NotRequired[KantarWatermarkSettingsTypeDef],  # (5)
    MotionImageInserter: NotRequired[MotionImageInserterTypeDef],  # (6)
    NielsenConfiguration: NotRequired[NielsenConfigurationTypeDef],  # (7)
    NielsenNonLinearWatermark: NotRequired[NielsenNonLinearWatermarkSettingsTypeDef],  # (8)
    OutputGroups: NotRequired[Sequence[OutputGroupTypeDef]],  # (9)
    TimecodeConfig: NotRequired[TimecodeConfigTypeDef],  # (10)
    TimedMetadataInsertion: NotRequired[TimedMetadataInsertionTypeDef],  # (11)
```

1. See [:material-code-braces: AvailBlankingTypeDef](./type_defs.md#availblankingtypedef) 
2. See [:material-code-braces: EsamSettingsTypeDef](./type_defs.md#esamsettingstypedef) 
3. See [:material-code-braces: ExtendedDataServicesTypeDef](./type_defs.md#extendeddataservicestypedef) 
4. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
5. See [:material-code-braces: KantarWatermarkSettingsTypeDef](./type_defs.md#kantarwatermarksettingstypedef) 
6. See [:material-code-braces: MotionImageInserterTypeDef](./type_defs.md#motionimageinsertertypedef) 
7. See [:material-code-braces: NielsenConfigurationTypeDef](./type_defs.md#nielsenconfigurationtypedef) 
8. See [:material-code-braces: NielsenNonLinearWatermarkSettingsTypeDef](./type_defs.md#nielsennonlinearwatermarksettingstypedef) 
9. See [:material-code-braces: OutputGroupTypeDef](./type_defs.md#outputgrouptypedef) 
10. See [:material-code-braces: TimecodeConfigTypeDef](./type_defs.md#timecodeconfigtypedef) 
11. See [:material-code-braces: TimedMetadataInsertionTypeDef](./type_defs.md#timedmetadatainsertiontypedef) 
## JobTemplateSettingsTypeDef

```python
# JobTemplateSettingsTypeDef definition

class JobTemplateSettingsTypeDef(TypedDict):
    AdAvailOffset: NotRequired[int],
    AvailBlanking: NotRequired[AvailBlankingTypeDef],  # (1)
    Esam: NotRequired[EsamSettingsTypeDef],  # (2)
    ExtendedDataServices: NotRequired[ExtendedDataServicesTypeDef],  # (3)
    Inputs: NotRequired[Sequence[InputTemplateTypeDef]],  # (4)
    KantarWatermark: NotRequired[KantarWatermarkSettingsTypeDef],  # (5)
    MotionImageInserter: NotRequired[MotionImageInserterTypeDef],  # (6)
    NielsenConfiguration: NotRequired[NielsenConfigurationTypeDef],  # (7)
    NielsenNonLinearWatermark: NotRequired[NielsenNonLinearWatermarkSettingsTypeDef],  # (8)
    OutputGroups: NotRequired[Sequence[OutputGroupTypeDef]],  # (9)
    TimecodeConfig: NotRequired[TimecodeConfigTypeDef],  # (10)
    TimedMetadataInsertion: NotRequired[TimedMetadataInsertionTypeDef],  # (11)
```

1. See [:material-code-braces: AvailBlankingTypeDef](./type_defs.md#availblankingtypedef) 
2. See [:material-code-braces: EsamSettingsTypeDef](./type_defs.md#esamsettingstypedef) 
3. See [:material-code-braces: ExtendedDataServicesTypeDef](./type_defs.md#extendeddataservicestypedef) 
4. See [:material-code-braces: InputTemplateTypeDef](./type_defs.md#inputtemplatetypedef) 
5. See [:material-code-braces: KantarWatermarkSettingsTypeDef](./type_defs.md#kantarwatermarksettingstypedef) 
6. See [:material-code-braces: MotionImageInserterTypeDef](./type_defs.md#motionimageinsertertypedef) 
7. See [:material-code-braces: NielsenConfigurationTypeDef](./type_defs.md#nielsenconfigurationtypedef) 
8. See [:material-code-braces: NielsenNonLinearWatermarkSettingsTypeDef](./type_defs.md#nielsennonlinearwatermarksettingstypedef) 
9. See [:material-code-braces: OutputGroupTypeDef](./type_defs.md#outputgrouptypedef) 
10. See [:material-code-braces: TimecodeConfigTypeDef](./type_defs.md#timecodeconfigtypedef) 
11. See [:material-code-braces: TimedMetadataInsertionTypeDef](./type_defs.md#timedmetadatainsertiontypedef) 
## CreatePresetResponseTypeDef

```python
# CreatePresetResponseTypeDef definition

class CreatePresetResponseTypeDef(TypedDict):
    Preset: PresetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPresetResponseTypeDef

```python
# GetPresetResponseTypeDef definition

class GetPresetResponseTypeDef(TypedDict):
    Preset: PresetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPresetsResponseTypeDef

```python
# ListPresetsResponseTypeDef definition

class ListPresetsResponseTypeDef(TypedDict):
    NextToken: str,
    Presets: List[PresetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePresetResponseTypeDef

```python
# UpdatePresetResponseTypeDef definition

class UpdatePresetResponseTypeDef(TypedDict):
    Preset: PresetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobRequestRequestTypeDef

```python
# CreateJobRequestRequestTypeDef definition

class CreateJobRequestRequestTypeDef(TypedDict):
    Role: str,
    Settings: JobSettingsTypeDef,  # (1)
    AccelerationSettings: NotRequired[AccelerationSettingsTypeDef],  # (2)
    BillingTagsSource: NotRequired[BillingTagsSourceType],  # (3)
    ClientRequestToken: NotRequired[str],
    HopDestinations: NotRequired[Sequence[HopDestinationTypeDef]],  # (4)
    JobTemplate: NotRequired[str],
    Priority: NotRequired[int],
    Queue: NotRequired[str],
    SimulateReservedQueue: NotRequired[SimulateReservedQueueType],  # (5)
    StatusUpdateInterval: NotRequired[StatusUpdateIntervalType],  # (6)
    Tags: NotRequired[Mapping[str, str]],
    UserMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: JobSettingsTypeDef](./type_defs.md#jobsettingstypedef) 
2. See [:material-code-braces: AccelerationSettingsTypeDef](./type_defs.md#accelerationsettingstypedef) 
3. See [:material-code-brackets: BillingTagsSourceType](./literals.md#billingtagssourcetype) 
4. See [:material-code-braces: HopDestinationTypeDef](./type_defs.md#hopdestinationtypedef) 
5. See [:material-code-brackets: SimulateReservedQueueType](./literals.md#simulatereservedqueuetype) 
6. See [:material-code-brackets: StatusUpdateIntervalType](./literals.md#statusupdateintervaltype) 
## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    Role: str,
    Settings: JobSettingsTypeDef,  # (9)
    AccelerationSettings: NotRequired[AccelerationSettingsTypeDef],  # (1)
    AccelerationStatus: NotRequired[AccelerationStatusType],  # (2)
    Arn: NotRequired[str],
    BillingTagsSource: NotRequired[BillingTagsSourceType],  # (3)
    ClientRequestToken: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    CurrentPhase: NotRequired[JobPhaseType],  # (4)
    ErrorCode: NotRequired[int],
    ErrorMessage: NotRequired[str],
    HopDestinations: NotRequired[List[HopDestinationTypeDef]],  # (5)
    Id: NotRequired[str],
    JobPercentComplete: NotRequired[int],
    JobTemplate: NotRequired[str],
    Messages: NotRequired[JobMessagesTypeDef],  # (6)
    OutputGroupDetails: NotRequired[List[OutputGroupDetailTypeDef]],  # (7)
    Priority: NotRequired[int],
    Queue: NotRequired[str],
    QueueTransitions: NotRequired[List[QueueTransitionTypeDef]],  # (8)
    RetryCount: NotRequired[int],
    SimulateReservedQueue: NotRequired[SimulateReservedQueueType],  # (10)
    Status: NotRequired[JobStatusType],  # (11)
    StatusUpdateInterval: NotRequired[StatusUpdateIntervalType],  # (12)
    Timing: NotRequired[TimingTypeDef],  # (13)
    UserMetadata: NotRequired[Dict[str, str]],
    Warnings: NotRequired[List[WarningGroupTypeDef]],  # (14)
```

1. See [:material-code-braces: AccelerationSettingsTypeDef](./type_defs.md#accelerationsettingstypedef) 
2. See [:material-code-brackets: AccelerationStatusType](./literals.md#accelerationstatustype) 
3. See [:material-code-brackets: BillingTagsSourceType](./literals.md#billingtagssourcetype) 
4. See [:material-code-brackets: JobPhaseType](./literals.md#jobphasetype) 
5. See [:material-code-braces: HopDestinationTypeDef](./type_defs.md#hopdestinationtypedef) 
6. See [:material-code-braces: JobMessagesTypeDef](./type_defs.md#jobmessagestypedef) 
7. See [:material-code-braces: OutputGroupDetailTypeDef](./type_defs.md#outputgroupdetailtypedef) 
8. See [:material-code-braces: QueueTransitionTypeDef](./type_defs.md#queuetransitiontypedef) 
9. See [:material-code-braces: JobSettingsTypeDef](./type_defs.md#jobsettingstypedef) 
10. See [:material-code-brackets: SimulateReservedQueueType](./literals.md#simulatereservedqueuetype) 
11. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
12. See [:material-code-brackets: StatusUpdateIntervalType](./literals.md#statusupdateintervaltype) 
13. See [:material-code-braces: TimingTypeDef](./type_defs.md#timingtypedef) 
14. See [:material-code-braces: WarningGroupTypeDef](./type_defs.md#warninggrouptypedef) 
## CreateJobTemplateRequestRequestTypeDef

```python
# CreateJobTemplateRequestRequestTypeDef definition

class CreateJobTemplateRequestRequestTypeDef(TypedDict):
    Name: str,
    Settings: JobTemplateSettingsTypeDef,  # (1)
    AccelerationSettings: NotRequired[AccelerationSettingsTypeDef],  # (2)
    Category: NotRequired[str],
    Description: NotRequired[str],
    HopDestinations: NotRequired[Sequence[HopDestinationTypeDef]],  # (3)
    Priority: NotRequired[int],
    Queue: NotRequired[str],
    StatusUpdateInterval: NotRequired[StatusUpdateIntervalType],  # (4)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: JobTemplateSettingsTypeDef](./type_defs.md#jobtemplatesettingstypedef) 
2. See [:material-code-braces: AccelerationSettingsTypeDef](./type_defs.md#accelerationsettingstypedef) 
3. See [:material-code-braces: HopDestinationTypeDef](./type_defs.md#hopdestinationtypedef) 
4. See [:material-code-brackets: StatusUpdateIntervalType](./literals.md#statusupdateintervaltype) 
## JobTemplateTypeDef

```python
# JobTemplateTypeDef definition

class JobTemplateTypeDef(TypedDict):
    Name: str,
    Settings: JobTemplateSettingsTypeDef,  # (3)
    AccelerationSettings: NotRequired[AccelerationSettingsTypeDef],  # (1)
    Arn: NotRequired[str],
    Category: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Description: NotRequired[str],
    HopDestinations: NotRequired[List[HopDestinationTypeDef]],  # (2)
    LastUpdated: NotRequired[datetime],
    Priority: NotRequired[int],
    Queue: NotRequired[str],
    StatusUpdateInterval: NotRequired[StatusUpdateIntervalType],  # (4)
    Type: NotRequired[TypeType],  # (5)
```

1. See [:material-code-braces: AccelerationSettingsTypeDef](./type_defs.md#accelerationsettingstypedef) 
2. See [:material-code-braces: HopDestinationTypeDef](./type_defs.md#hopdestinationtypedef) 
3. See [:material-code-braces: JobTemplateSettingsTypeDef](./type_defs.md#jobtemplatesettingstypedef) 
4. See [:material-code-brackets: StatusUpdateIntervalType](./literals.md#statusupdateintervaltype) 
5. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## UpdateJobTemplateRequestRequestTypeDef

```python
# UpdateJobTemplateRequestRequestTypeDef definition

class UpdateJobTemplateRequestRequestTypeDef(TypedDict):
    Name: str,
    AccelerationSettings: NotRequired[AccelerationSettingsTypeDef],  # (1)
    Category: NotRequired[str],
    Description: NotRequired[str],
    HopDestinations: NotRequired[Sequence[HopDestinationTypeDef]],  # (2)
    Priority: NotRequired[int],
    Queue: NotRequired[str],
    Settings: NotRequired[JobTemplateSettingsTypeDef],  # (3)
    StatusUpdateInterval: NotRequired[StatusUpdateIntervalType],  # (4)
```

1. See [:material-code-braces: AccelerationSettingsTypeDef](./type_defs.md#accelerationsettingstypedef) 
2. See [:material-code-braces: HopDestinationTypeDef](./type_defs.md#hopdestinationtypedef) 
3. See [:material-code-braces: JobTemplateSettingsTypeDef](./type_defs.md#jobtemplatesettingstypedef) 
4. See [:material-code-brackets: StatusUpdateIntervalType](./literals.md#statusupdateintervaltype) 
## CreateJobResponseTypeDef

```python
# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    Job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobResponseTypeDef

```python
# GetJobResponseTypeDef definition

class GetJobResponseTypeDef(TypedDict):
    Job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsResponseTypeDef

```python
# ListJobsResponseTypeDef definition

class ListJobsResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobTemplateResponseTypeDef

```python
# CreateJobTemplateResponseTypeDef definition

class CreateJobTemplateResponseTypeDef(TypedDict):
    JobTemplate: JobTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTemplateTypeDef](./type_defs.md#jobtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobTemplateResponseTypeDef

```python
# GetJobTemplateResponseTypeDef definition

class GetJobTemplateResponseTypeDef(TypedDict):
    JobTemplate: JobTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTemplateTypeDef](./type_defs.md#jobtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobTemplatesResponseTypeDef

```python
# ListJobTemplatesResponseTypeDef definition

class ListJobTemplatesResponseTypeDef(TypedDict):
    JobTemplates: List[JobTemplateTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTemplateTypeDef](./type_defs.md#jobtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateJobTemplateResponseTypeDef

```python
# UpdateJobTemplateResponseTypeDef definition

class UpdateJobTemplateResponseTypeDef(TypedDict):
    JobTemplate: JobTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTemplateTypeDef](./type_defs.md#jobtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
