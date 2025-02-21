# Type definitions

> [Index](../README.md) > [MediaConvert](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MediaConvert](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#mediaconvert)
    type annotations stubs module [types-aiobotocore-mediaconvert](https://pypi.org/project/types-aiobotocore-mediaconvert/).

## PresetSettingsUnionTypeDef

```python
# PresetSettingsUnionTypeDef Union usage example

from types_aiobotocore_mediaconvert.type_defs import PresetSettingsUnionTypeDef


def get_value() -> PresetSettingsUnionTypeDef:
    return ...


# PresetSettingsUnionTypeDef definition

PresetSettingsUnionTypeDef = Union[
    PresetSettingsTypeDef,  # (1)
    PresetSettingsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PresetSettingsTypeDef](./type_defs.md#presetsettingstypedef) 
2. See [:material-code-braces: PresetSettingsOutputTypeDef](./type_defs.md#presetsettingsoutputtypedef) 

## JobSettingsUnionTypeDef

```python
# JobSettingsUnionTypeDef Union usage example

from types_aiobotocore_mediaconvert.type_defs import JobSettingsUnionTypeDef


def get_value() -> JobSettingsUnionTypeDef:
    return ...


# JobSettingsUnionTypeDef definition

JobSettingsUnionTypeDef = Union[
    JobSettingsTypeDef,  # (1)
    JobSettingsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JobSettingsTypeDef](./type_defs.md#jobsettingstypedef) 
2. See [:material-code-braces: JobSettingsOutputTypeDef](./type_defs.md#jobsettingsoutputtypedef) 

## JobTemplateSettingsUnionTypeDef

```python
# JobTemplateSettingsUnionTypeDef Union usage example

from types_aiobotocore_mediaconvert.type_defs import JobTemplateSettingsUnionTypeDef


def get_value() -> JobTemplateSettingsUnionTypeDef:
    return ...


# JobTemplateSettingsUnionTypeDef definition

JobTemplateSettingsUnionTypeDef = Union[
    JobTemplateSettingsTypeDef,  # (1)
    JobTemplateSettingsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JobTemplateSettingsTypeDef](./type_defs.md#jobtemplatesettingstypedef) 
2. See [:material-code-braces: JobTemplateSettingsOutputTypeDef](./type_defs.md#jobtemplatesettingsoutputtypedef) 



## AacSettingsTypeDef

```python
# AacSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AacSettingsTypeDef


def get_value() -> AacSettingsTypeDef:
    return {
        "AudioDescriptionBroadcasterMix": ...,
    }


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
# Ac3SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Ac3SettingsTypeDef


def get_value() -> Ac3SettingsTypeDef:
    return {
        "Bitrate": ...,
    }


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
# AccelerationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AccelerationSettingsTypeDef


def get_value() -> AccelerationSettingsTypeDef:
    return {
        "Mode": ...,
    }


# AccelerationSettingsTypeDef definition

class AccelerationSettingsTypeDef(TypedDict):
    Mode: AccelerationModeType,  # (1)
```

1. See [:material-code-brackets: AccelerationModeType](./literals.md#accelerationmodetype) 
## AdvancedInputFilterSettingsTypeDef

```python
# AdvancedInputFilterSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AdvancedInputFilterSettingsTypeDef


def get_value() -> AdvancedInputFilterSettingsTypeDef:
    return {
        "AddTexture": ...,
    }


# AdvancedInputFilterSettingsTypeDef definition

class AdvancedInputFilterSettingsTypeDef(TypedDict):
    AddTexture: NotRequired[AdvancedInputFilterAddTextureType],  # (1)
    Sharpening: NotRequired[AdvancedInputFilterSharpenType],  # (2)
```

1. See [:material-code-brackets: AdvancedInputFilterAddTextureType](./literals.md#advancedinputfilteraddtexturetype) 
2. See [:material-code-brackets: AdvancedInputFilterSharpenType](./literals.md#advancedinputfiltersharpentype) 
## AiffSettingsTypeDef

```python
# AiffSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AiffSettingsTypeDef


def get_value() -> AiffSettingsTypeDef:
    return {
        "BitDepth": ...,
    }


# AiffSettingsTypeDef definition

class AiffSettingsTypeDef(TypedDict):
    BitDepth: NotRequired[int],
    Channels: NotRequired[int],
    SampleRate: NotRequired[int],
```

## AllowedRenditionSizeTypeDef

```python
# AllowedRenditionSizeTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AllowedRenditionSizeTypeDef


def get_value() -> AllowedRenditionSizeTypeDef:
    return {
        "Height": ...,
    }


# AllowedRenditionSizeTypeDef definition

class AllowedRenditionSizeTypeDef(TypedDict):
    Height: NotRequired[int],
    Required: NotRequired[RequiredFlagType],  # (1)
    Width: NotRequired[int],
```

1. See [:material-code-brackets: RequiredFlagType](./literals.md#requiredflagtype) 
## AncillarySourceSettingsTypeDef

```python
# AncillarySourceSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AncillarySourceSettingsTypeDef


def get_value() -> AncillarySourceSettingsTypeDef:
    return {
        "Convert608To708": ...,
    }


# AncillarySourceSettingsTypeDef definition

class AncillarySourceSettingsTypeDef(TypedDict):
    Convert608To708: NotRequired[AncillaryConvert608To708Type],  # (1)
    SourceAncillaryChannelNumber: NotRequired[int],
    TerminateCaptions: NotRequired[AncillaryTerminateCaptionsType],  # (2)
```

1. See [:material-code-brackets: AncillaryConvert608To708Type](./literals.md#ancillaryconvert608to708type) 
2. See [:material-code-brackets: AncillaryTerminateCaptionsType](./literals.md#ancillaryterminatecaptionstype) 
## AssociateCertificateRequestTypeDef

```python
# AssociateCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AssociateCertificateRequestTypeDef


def get_value() -> AssociateCertificateRequestTypeDef:
    return {
        "Arn": ...,
    }


# AssociateCertificateRequestTypeDef definition

class AssociateCertificateRequestTypeDef(TypedDict):
    Arn: str,
```

## AudioChannelTaggingSettingsOutputTypeDef

```python
# AudioChannelTaggingSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AudioChannelTaggingSettingsOutputTypeDef


def get_value() -> AudioChannelTaggingSettingsOutputTypeDef:
    return {
        "ChannelTag": ...,
    }


# AudioChannelTaggingSettingsOutputTypeDef definition

class AudioChannelTaggingSettingsOutputTypeDef(TypedDict):
    ChannelTag: NotRequired[AudioChannelTagType],  # (1)
    ChannelTags: NotRequired[List[AudioChannelTagType]],  # (2)
```

1. See [:material-code-brackets: AudioChannelTagType](./literals.md#audiochanneltagtype) 
2. See [:material-code-brackets: AudioChannelTagType](./literals.md#audiochanneltagtype) 
## AudioChannelTaggingSettingsTypeDef

```python
# AudioChannelTaggingSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AudioChannelTaggingSettingsTypeDef


def get_value() -> AudioChannelTaggingSettingsTypeDef:
    return {
        "ChannelTag": ...,
    }


# AudioChannelTaggingSettingsTypeDef definition

class AudioChannelTaggingSettingsTypeDef(TypedDict):
    ChannelTag: NotRequired[AudioChannelTagType],  # (1)
    ChannelTags: NotRequired[Sequence[AudioChannelTagType]],  # (2)
```

1. See [:material-code-brackets: AudioChannelTagType](./literals.md#audiochanneltagtype) 
2. See [:material-code-brackets: AudioChannelTagType](./literals.md#audiochanneltagtype) 
## Eac3AtmosSettingsTypeDef

```python
# Eac3AtmosSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Eac3AtmosSettingsTypeDef


def get_value() -> Eac3AtmosSettingsTypeDef:
    return {
        "Bitrate": ...,
    }


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
# Eac3SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Eac3SettingsTypeDef


def get_value() -> Eac3SettingsTypeDef:
    return {
        "AttenuationControl": ...,
    }


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
## FlacSettingsTypeDef

```python
# FlacSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import FlacSettingsTypeDef


def get_value() -> FlacSettingsTypeDef:
    return {
        "BitDepth": ...,
    }


# FlacSettingsTypeDef definition

class FlacSettingsTypeDef(TypedDict):
    BitDepth: NotRequired[int],
    Channels: NotRequired[int],
    SampleRate: NotRequired[int],
```

## Mp2SettingsTypeDef

```python
# Mp2SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Mp2SettingsTypeDef


def get_value() -> Mp2SettingsTypeDef:
    return {
        "Bitrate": ...,
    }


# Mp2SettingsTypeDef definition

class Mp2SettingsTypeDef(TypedDict):
    Bitrate: NotRequired[int],
    Channels: NotRequired[int],
    SampleRate: NotRequired[int],
```

## Mp3SettingsTypeDef

```python
# Mp3SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Mp3SettingsTypeDef


def get_value() -> Mp3SettingsTypeDef:
    return {
        "Bitrate": ...,
    }


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
# OpusSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import OpusSettingsTypeDef


def get_value() -> OpusSettingsTypeDef:
    return {
        "Bitrate": ...,
    }


# OpusSettingsTypeDef definition

class OpusSettingsTypeDef(TypedDict):
    Bitrate: NotRequired[int],
    Channels: NotRequired[int],
    SampleRate: NotRequired[int],
```

## VorbisSettingsTypeDef

```python
# VorbisSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VorbisSettingsTypeDef


def get_value() -> VorbisSettingsTypeDef:
    return {
        "Channels": ...,
    }


# VorbisSettingsTypeDef definition

class VorbisSettingsTypeDef(TypedDict):
    Channels: NotRequired[int],
    SampleRate: NotRequired[int],
    VbrQuality: NotRequired[int],
```

## WavSettingsTypeDef

```python
# WavSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import WavSettingsTypeDef


def get_value() -> WavSettingsTypeDef:
    return {
        "BitDepth": ...,
    }


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
# AudioNormalizationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AudioNormalizationSettingsTypeDef


def get_value() -> AudioNormalizationSettingsTypeDef:
    return {
        "Algorithm": ...,
    }


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
## AudioSelectorGroupOutputTypeDef

```python
# AudioSelectorGroupOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AudioSelectorGroupOutputTypeDef


def get_value() -> AudioSelectorGroupOutputTypeDef:
    return {
        "AudioSelectorNames": ...,
    }


# AudioSelectorGroupOutputTypeDef definition

class AudioSelectorGroupOutputTypeDef(TypedDict):
    AudioSelectorNames: NotRequired[List[str]],
```

## AudioSelectorGroupTypeDef

```python
# AudioSelectorGroupTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AudioSelectorGroupTypeDef


def get_value() -> AudioSelectorGroupTypeDef:
    return {
        "AudioSelectorNames": ...,
    }


# AudioSelectorGroupTypeDef definition

class AudioSelectorGroupTypeDef(TypedDict):
    AudioSelectorNames: NotRequired[Sequence[str]],
```

## HlsRenditionGroupSettingsTypeDef

```python
# HlsRenditionGroupSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import HlsRenditionGroupSettingsTypeDef


def get_value() -> HlsRenditionGroupSettingsTypeDef:
    return {
        "RenditionGroupId": ...,
    }


# HlsRenditionGroupSettingsTypeDef definition

class HlsRenditionGroupSettingsTypeDef(TypedDict):
    RenditionGroupId: NotRequired[str],
    RenditionLanguageCode: NotRequired[LanguageCodeType],  # (1)
    RenditionName: NotRequired[str],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## ForceIncludeRenditionSizeTypeDef

```python
# ForceIncludeRenditionSizeTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ForceIncludeRenditionSizeTypeDef


def get_value() -> ForceIncludeRenditionSizeTypeDef:
    return {
        "Height": ...,
    }


# ForceIncludeRenditionSizeTypeDef definition

class ForceIncludeRenditionSizeTypeDef(TypedDict):
    Height: NotRequired[int],
    Width: NotRequired[int],
```

## MinBottomRenditionSizeTypeDef

```python
# MinBottomRenditionSizeTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MinBottomRenditionSizeTypeDef


def get_value() -> MinBottomRenditionSizeTypeDef:
    return {
        "Height": ...,
    }


# MinBottomRenditionSizeTypeDef definition

class MinBottomRenditionSizeTypeDef(TypedDict):
    Height: NotRequired[int],
    Width: NotRequired[int],
```

## MinTopRenditionSizeTypeDef

```python
# MinTopRenditionSizeTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MinTopRenditionSizeTypeDef


def get_value() -> MinTopRenditionSizeTypeDef:
    return {
        "Height": ...,
    }


# MinTopRenditionSizeTypeDef definition

class MinTopRenditionSizeTypeDef(TypedDict):
    Height: NotRequired[int],
    Width: NotRequired[int],
```

## Av1QvbrSettingsTypeDef

```python
# Av1QvbrSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Av1QvbrSettingsTypeDef


def get_value() -> Av1QvbrSettingsTypeDef:
    return {
        "QvbrQualityLevel": ...,
    }


# Av1QvbrSettingsTypeDef definition

class Av1QvbrSettingsTypeDef(TypedDict):
    QvbrQualityLevel: NotRequired[int],
    QvbrQualityLevelFineTune: NotRequired[float],
```

## AvailBlankingTypeDef

```python
# AvailBlankingTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AvailBlankingTypeDef


def get_value() -> AvailBlankingTypeDef:
    return {
        "AvailBlankingImage": ...,
    }


# AvailBlankingTypeDef definition

class AvailBlankingTypeDef(TypedDict):
    AvailBlankingImage: NotRequired[str],
```

## AvcIntraUhdSettingsTypeDef

```python
# AvcIntraUhdSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AvcIntraUhdSettingsTypeDef


def get_value() -> AvcIntraUhdSettingsTypeDef:
    return {
        "QualityTuningLevel": ...,
    }


# AvcIntraUhdSettingsTypeDef definition

class AvcIntraUhdSettingsTypeDef(TypedDict):
    QualityTuningLevel: NotRequired[AvcIntraUhdQualityTuningLevelType],  # (1)
```

1. See [:material-code-brackets: AvcIntraUhdQualityTuningLevelType](./literals.md#avcintrauhdqualitytuningleveltype) 
## BandwidthReductionFilterTypeDef

```python
# BandwidthReductionFilterTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import BandwidthReductionFilterTypeDef


def get_value() -> BandwidthReductionFilterTypeDef:
    return {
        "Sharpening": ...,
    }


# BandwidthReductionFilterTypeDef definition

class BandwidthReductionFilterTypeDef(TypedDict):
    Sharpening: NotRequired[BandwidthReductionFilterSharpeningType],  # (1)
    Strength: NotRequired[BandwidthReductionFilterStrengthType],  # (2)
```

1. See [:material-code-brackets: BandwidthReductionFilterSharpeningType](./literals.md#bandwidthreductionfiltersharpeningtype) 
2. See [:material-code-brackets: BandwidthReductionFilterStrengthType](./literals.md#bandwidthreductionfilterstrengthtype) 
## BurninDestinationSettingsTypeDef

```python
# BurninDestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import BurninDestinationSettingsTypeDef


def get_value() -> BurninDestinationSettingsTypeDef:
    return {
        "Alignment": ...,
    }


# BurninDestinationSettingsTypeDef definition

class BurninDestinationSettingsTypeDef(TypedDict):
    Alignment: NotRequired[BurninSubtitleAlignmentType],  # (1)
    ApplyFontColor: NotRequired[BurninSubtitleApplyFontColorType],  # (2)
    BackgroundColor: NotRequired[BurninSubtitleBackgroundColorType],  # (3)
    BackgroundOpacity: NotRequired[int],
    FallbackFont: NotRequired[BurninSubtitleFallbackFontType],  # (4)
    FontColor: NotRequired[BurninSubtitleFontColorType],  # (5)
    FontFileBold: NotRequired[str],
    FontFileBoldItalic: NotRequired[str],
    FontFileItalic: NotRequired[str],
    FontFileRegular: NotRequired[str],
    FontOpacity: NotRequired[int],
    FontResolution: NotRequired[int],
    FontScript: NotRequired[FontScriptType],  # (6)
    FontSize: NotRequired[int],
    HexFontColor: NotRequired[str],
    OutlineColor: NotRequired[BurninSubtitleOutlineColorType],  # (7)
    OutlineSize: NotRequired[int],
    RemoveRubyReserveAttributes: NotRequired[RemoveRubyReserveAttributesType],  # (8)
    ShadowColor: NotRequired[BurninSubtitleShadowColorType],  # (9)
    ShadowOpacity: NotRequired[int],
    ShadowXOffset: NotRequired[int],
    ShadowYOffset: NotRequired[int],
    StylePassthrough: NotRequired[BurnInSubtitleStylePassthroughType],  # (10)
    TeletextSpacing: NotRequired[BurninSubtitleTeletextSpacingType],  # (11)
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
8. See [:material-code-brackets: RemoveRubyReserveAttributesType](./literals.md#removerubyreserveattributestype) 
9. See [:material-code-brackets: BurninSubtitleShadowColorType](./literals.md#burninsubtitleshadowcolortype) 
10. See [:material-code-brackets: BurnInSubtitleStylePassthroughType](./literals.md#burninsubtitlestylepassthroughtype) 
11. See [:material-code-brackets: BurninSubtitleTeletextSpacingType](./literals.md#burninsubtitleteletextspacingtype) 
## CancelJobRequestTypeDef

```python
# CancelJobRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CancelJobRequestTypeDef


def get_value() -> CancelJobRequestTypeDef:
    return {
        "Id": ...,
    }


# CancelJobRequestTypeDef definition

class CancelJobRequestTypeDef(TypedDict):
    Id: str,
```

## DvbSubDestinationSettingsTypeDef

```python
# DvbSubDestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DvbSubDestinationSettingsTypeDef


def get_value() -> DvbSubDestinationSettingsTypeDef:
    return {
        "Alignment": ...,
    }


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
    FontFileBold: NotRequired[str],
    FontFileBoldItalic: NotRequired[str],
    FontFileItalic: NotRequired[str],
    FontFileRegular: NotRequired[str],
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
# EmbeddedDestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import EmbeddedDestinationSettingsTypeDef


def get_value() -> EmbeddedDestinationSettingsTypeDef:
    return {
        "Destination608ChannelNumber": ...,
    }


# EmbeddedDestinationSettingsTypeDef definition

class EmbeddedDestinationSettingsTypeDef(TypedDict):
    Destination608ChannelNumber: NotRequired[int],
    Destination708ServiceNumber: NotRequired[int],
```

## ImscDestinationSettingsTypeDef

```python
# ImscDestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ImscDestinationSettingsTypeDef


def get_value() -> ImscDestinationSettingsTypeDef:
    return {
        "Accessibility": ...,
    }


# ImscDestinationSettingsTypeDef definition

class ImscDestinationSettingsTypeDef(TypedDict):
    Accessibility: NotRequired[ImscAccessibilitySubsType],  # (1)
    StylePassthrough: NotRequired[ImscStylePassthroughType],  # (2)
```

1. See [:material-code-brackets: ImscAccessibilitySubsType](./literals.md#imscaccessibilitysubstype) 
2. See [:material-code-brackets: ImscStylePassthroughType](./literals.md#imscstylepassthroughtype) 
## SccDestinationSettingsTypeDef

```python
# SccDestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import SccDestinationSettingsTypeDef


def get_value() -> SccDestinationSettingsTypeDef:
    return {
        "Framerate": ...,
    }


# SccDestinationSettingsTypeDef definition

class SccDestinationSettingsTypeDef(TypedDict):
    Framerate: NotRequired[SccDestinationFramerateType],  # (1)
```

1. See [:material-code-brackets: SccDestinationFramerateType](./literals.md#sccdestinationframeratetype) 
## SrtDestinationSettingsTypeDef

```python
# SrtDestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import SrtDestinationSettingsTypeDef


def get_value() -> SrtDestinationSettingsTypeDef:
    return {
        "StylePassthrough": ...,
    }


# SrtDestinationSettingsTypeDef definition

class SrtDestinationSettingsTypeDef(TypedDict):
    StylePassthrough: NotRequired[SrtStylePassthroughType],  # (1)
```

1. See [:material-code-brackets: SrtStylePassthroughType](./literals.md#srtstylepassthroughtype) 
## TeletextDestinationSettingsOutputTypeDef

```python
# TeletextDestinationSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import TeletextDestinationSettingsOutputTypeDef


def get_value() -> TeletextDestinationSettingsOutputTypeDef:
    return {
        "PageNumber": ...,
    }


# TeletextDestinationSettingsOutputTypeDef definition

class TeletextDestinationSettingsOutputTypeDef(TypedDict):
    PageNumber: NotRequired[str],
    PageTypes: NotRequired[List[TeletextPageTypeType]],  # (1)
```

1. See [:material-code-brackets: TeletextPageTypeType](./literals.md#teletextpagetypetype) 
## TtmlDestinationSettingsTypeDef

```python
# TtmlDestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import TtmlDestinationSettingsTypeDef


def get_value() -> TtmlDestinationSettingsTypeDef:
    return {
        "StylePassthrough": ...,
    }


# TtmlDestinationSettingsTypeDef definition

class TtmlDestinationSettingsTypeDef(TypedDict):
    StylePassthrough: NotRequired[TtmlStylePassthroughType],  # (1)
```

1. See [:material-code-brackets: TtmlStylePassthroughType](./literals.md#ttmlstylepassthroughtype) 
## WebvttDestinationSettingsTypeDef

```python
# WebvttDestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import WebvttDestinationSettingsTypeDef


def get_value() -> WebvttDestinationSettingsTypeDef:
    return {
        "Accessibility": ...,
    }


# WebvttDestinationSettingsTypeDef definition

class WebvttDestinationSettingsTypeDef(TypedDict):
    Accessibility: NotRequired[WebvttAccessibilitySubsType],  # (1)
    StylePassthrough: NotRequired[WebvttStylePassthroughType],  # (2)
```

1. See [:material-code-brackets: WebvttAccessibilitySubsType](./literals.md#webvttaccessibilitysubstype) 
2. See [:material-code-brackets: WebvttStylePassthroughType](./literals.md#webvttstylepassthroughtype) 
## TeletextDestinationSettingsTypeDef

```python
# TeletextDestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import TeletextDestinationSettingsTypeDef


def get_value() -> TeletextDestinationSettingsTypeDef:
    return {
        "PageNumber": ...,
    }


# TeletextDestinationSettingsTypeDef definition

class TeletextDestinationSettingsTypeDef(TypedDict):
    PageNumber: NotRequired[str],
    PageTypes: NotRequired[Sequence[TeletextPageTypeType]],  # (1)
```

1. See [:material-code-brackets: TeletextPageTypeType](./literals.md#teletextpagetypetype) 
## CaptionSourceFramerateTypeDef

```python
# CaptionSourceFramerateTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CaptionSourceFramerateTypeDef


def get_value() -> CaptionSourceFramerateTypeDef:
    return {
        "FramerateDenominator": ...,
    }


# CaptionSourceFramerateTypeDef definition

class CaptionSourceFramerateTypeDef(TypedDict):
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
```

## DvbSubSourceSettingsTypeDef

```python
# DvbSubSourceSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DvbSubSourceSettingsTypeDef


def get_value() -> DvbSubSourceSettingsTypeDef:
    return {
        "Pid": ...,
    }


# DvbSubSourceSettingsTypeDef definition

class DvbSubSourceSettingsTypeDef(TypedDict):
    Pid: NotRequired[int],
```

## EmbeddedSourceSettingsTypeDef

```python
# EmbeddedSourceSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import EmbeddedSourceSettingsTypeDef


def get_value() -> EmbeddedSourceSettingsTypeDef:
    return {
        "Convert608To708": ...,
    }


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
# TeletextSourceSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import TeletextSourceSettingsTypeDef


def get_value() -> TeletextSourceSettingsTypeDef:
    return {
        "PageNumber": ...,
    }


# TeletextSourceSettingsTypeDef definition

class TeletextSourceSettingsTypeDef(TypedDict):
    PageNumber: NotRequired[str],
```

## TrackSourceSettingsTypeDef

```python
# TrackSourceSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import TrackSourceSettingsTypeDef


def get_value() -> TrackSourceSettingsTypeDef:
    return {
        "TrackNumber": ...,
    }


# TrackSourceSettingsTypeDef definition

class TrackSourceSettingsTypeDef(TypedDict):
    TrackNumber: NotRequired[int],
```

## WebvttHlsSourceSettingsTypeDef

```python
# WebvttHlsSourceSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import WebvttHlsSourceSettingsTypeDef


def get_value() -> WebvttHlsSourceSettingsTypeDef:
    return {
        "RenditionGroupId": ...,
    }


# WebvttHlsSourceSettingsTypeDef definition

class WebvttHlsSourceSettingsTypeDef(TypedDict):
    RenditionGroupId: NotRequired[str],
    RenditionLanguageCode: NotRequired[LanguageCodeType],  # (1)
    RenditionName: NotRequired[str],
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## OutputChannelMappingOutputTypeDef

```python
# OutputChannelMappingOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import OutputChannelMappingOutputTypeDef


def get_value() -> OutputChannelMappingOutputTypeDef:
    return {
        "InputChannels": ...,
    }


# OutputChannelMappingOutputTypeDef definition

class OutputChannelMappingOutputTypeDef(TypedDict):
    InputChannels: NotRequired[List[int]],
    InputChannelsFineTune: NotRequired[List[float]],
```

## OutputChannelMappingTypeDef

```python
# OutputChannelMappingTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import OutputChannelMappingTypeDef


def get_value() -> OutputChannelMappingTypeDef:
    return {
        "InputChannels": ...,
    }


# OutputChannelMappingTypeDef definition

class OutputChannelMappingTypeDef(TypedDict):
    InputChannels: NotRequired[Sequence[int]],
    InputChannelsFineTune: NotRequired[Sequence[float]],
```

## ClipLimitsTypeDef

```python
# ClipLimitsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ClipLimitsTypeDef


def get_value() -> ClipLimitsTypeDef:
    return {
        "MaximumRGBTolerance": ...,
    }


# ClipLimitsTypeDef definition

class ClipLimitsTypeDef(TypedDict):
    MaximumRGBTolerance: NotRequired[int],
    MaximumYUV: NotRequired[int],
    MinimumRGBTolerance: NotRequired[int],
    MinimumYUV: NotRequired[int],
```

## CmafAdditionalManifestOutputTypeDef

```python
# CmafAdditionalManifestOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CmafAdditionalManifestOutputTypeDef


def get_value() -> CmafAdditionalManifestOutputTypeDef:
    return {
        "ManifestNameModifier": ...,
    }


# CmafAdditionalManifestOutputTypeDef definition

class CmafAdditionalManifestOutputTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[List[str]],
```

## CmafAdditionalManifestTypeDef

```python
# CmafAdditionalManifestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CmafAdditionalManifestTypeDef


def get_value() -> CmafAdditionalManifestTypeDef:
    return {
        "ManifestNameModifier": ...,
    }


# CmafAdditionalManifestTypeDef definition

class CmafAdditionalManifestTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[Sequence[str]],
```

## StaticKeyProviderTypeDef

```python
# StaticKeyProviderTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import StaticKeyProviderTypeDef


def get_value() -> StaticKeyProviderTypeDef:
    return {
        "KeyFormat": ...,
    }


# StaticKeyProviderTypeDef definition

class StaticKeyProviderTypeDef(TypedDict):
    KeyFormat: NotRequired[str],
    KeyFormatVersions: NotRequired[str],
    StaticKeyValue: NotRequired[str],
    Url: NotRequired[str],
```

## CmafImageBasedTrickPlaySettingsTypeDef

```python
# CmafImageBasedTrickPlaySettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CmafImageBasedTrickPlaySettingsTypeDef


def get_value() -> CmafImageBasedTrickPlaySettingsTypeDef:
    return {
        "IntervalCadence": ...,
    }


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
# CmfcSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CmfcSettingsTypeDef


def get_value() -> CmfcSettingsTypeDef:
    return {
        "AudioDuration": ...,
    }


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
## ColorConversion3DLUTSettingTypeDef

```python
# ColorConversion3DLUTSettingTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ColorConversion3DLUTSettingTypeDef


def get_value() -> ColorConversion3DLUTSettingTypeDef:
    return {
        "FileInput": ...,
    }


# ColorConversion3DLUTSettingTypeDef definition

class ColorConversion3DLUTSettingTypeDef(TypedDict):
    FileInput: NotRequired[str],
    InputColorSpace: NotRequired[ColorSpaceType],  # (1)
    InputMasteringLuminance: NotRequired[int],
    OutputColorSpace: NotRequired[ColorSpaceType],  # (1)
    OutputMasteringLuminance: NotRequired[int],
```

1. See [:material-code-brackets: ColorSpaceType](./literals.md#colorspacetype) 
2. See [:material-code-brackets: ColorSpaceType](./literals.md#colorspacetype) 
## Hdr10MetadataTypeDef

```python
# Hdr10MetadataTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Hdr10MetadataTypeDef


def get_value() -> Hdr10MetadataTypeDef:
    return {
        "BluePrimaryX": ...,
    }


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
# F4vSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import F4vSettingsTypeDef


def get_value() -> F4vSettingsTypeDef:
    return {
        "MoovPlacement": ...,
    }


# F4vSettingsTypeDef definition

class F4vSettingsTypeDef(TypedDict):
    MoovPlacement: NotRequired[F4vMoovPlacementType],  # (1)
```

1. See [:material-code-brackets: F4vMoovPlacementType](./literals.md#f4vmoovplacementtype) 
## M3u8SettingsOutputTypeDef

```python
# M3u8SettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import M3u8SettingsOutputTypeDef


def get_value() -> M3u8SettingsOutputTypeDef:
    return {
        "AudioDuration": ...,
    }


# M3u8SettingsOutputTypeDef definition

class M3u8SettingsOutputTypeDef(TypedDict):
    AudioDuration: NotRequired[M3u8AudioDurationType],  # (1)
    AudioFramesPerPes: NotRequired[int],
    AudioPids: NotRequired[List[int]],
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
    PtsOffset: NotRequired[int],
    PtsOffsetMode: NotRequired[TsPtsOffsetType],  # (5)
    Scte35Pid: NotRequired[int],
    Scte35Source: NotRequired[M3u8Scte35SourceType],  # (6)
    TimedMetadata: NotRequired[TimedMetadataType],  # (7)
    TimedMetadataPid: NotRequired[int],
    TransportStreamId: NotRequired[int],
    VideoPid: NotRequired[int],
```

1. See [:material-code-brackets: M3u8AudioDurationType](./literals.md#m3u8audiodurationtype) 
2. See [:material-code-brackets: M3u8DataPtsControlType](./literals.md#m3u8dataptscontroltype) 
3. See [:material-code-brackets: M3u8NielsenId3Type](./literals.md#m3u8nielsenid3type) 
4. See [:material-code-brackets: M3u8PcrControlType](./literals.md#m3u8pcrcontroltype) 
5. See [:material-code-brackets: TsPtsOffsetType](./literals.md#tsptsoffsettype) 
6. See [:material-code-brackets: M3u8Scte35SourceType](./literals.md#m3u8scte35sourcetype) 
7. See [:material-code-brackets: TimedMetadataType](./literals.md#timedmetadatatype) 
## MovSettingsTypeDef

```python
# MovSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MovSettingsTypeDef


def get_value() -> MovSettingsTypeDef:
    return {
        "ClapAtom": ...,
    }


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
# Mp4SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Mp4SettingsTypeDef


def get_value() -> Mp4SettingsTypeDef:
    return {
        "AudioDuration": ...,
    }


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
# MpdSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MpdSettingsTypeDef


def get_value() -> MpdSettingsTypeDef:
    return {
        "AccessibilityCaptionHints": ...,
    }


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
## M3u8SettingsTypeDef

```python
# M3u8SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import M3u8SettingsTypeDef


def get_value() -> M3u8SettingsTypeDef:
    return {
        "AudioDuration": ...,
    }


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
    PtsOffset: NotRequired[int],
    PtsOffsetMode: NotRequired[TsPtsOffsetType],  # (5)
    Scte35Pid: NotRequired[int],
    Scte35Source: NotRequired[M3u8Scte35SourceType],  # (6)
    TimedMetadata: NotRequired[TimedMetadataType],  # (7)
    TimedMetadataPid: NotRequired[int],
    TransportStreamId: NotRequired[int],
    VideoPid: NotRequired[int],
```

1. See [:material-code-brackets: M3u8AudioDurationType](./literals.md#m3u8audiodurationtype) 
2. See [:material-code-brackets: M3u8DataPtsControlType](./literals.md#m3u8dataptscontroltype) 
3. See [:material-code-brackets: M3u8NielsenId3Type](./literals.md#m3u8nielsenid3type) 
4. See [:material-code-brackets: M3u8PcrControlType](./literals.md#m3u8pcrcontroltype) 
5. See [:material-code-brackets: TsPtsOffsetType](./literals.md#tsptsoffsettype) 
6. See [:material-code-brackets: M3u8Scte35SourceType](./literals.md#m3u8scte35sourcetype) 
7. See [:material-code-brackets: TimedMetadataType](./literals.md#timedmetadatatype) 
## HopDestinationTypeDef

```python
# HopDestinationTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import HopDestinationTypeDef


def get_value() -> HopDestinationTypeDef:
    return {
        "Priority": ...,
    }


# HopDestinationTypeDef definition

class HopDestinationTypeDef(TypedDict):
    Priority: NotRequired[int],
    Queue: NotRequired[str],
    WaitMinutes: NotRequired[int],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ResponseMetadataTypeDef


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

## ReservationPlanSettingsTypeDef

```python
# ReservationPlanSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ReservationPlanSettingsTypeDef


def get_value() -> ReservationPlanSettingsTypeDef:
    return {
        "Commitment": ...,
    }


# ReservationPlanSettingsTypeDef definition

class ReservationPlanSettingsTypeDef(TypedDict):
    Commitment: CommitmentType,  # (1)
    RenewalType: RenewalTypeType,  # (2)
    ReservedSlots: int,
```

1. See [:material-code-brackets: CommitmentType](./literals.md#commitmenttype) 
2. See [:material-code-brackets: RenewalTypeType](./literals.md#renewaltypetype) 
## DashAdditionalManifestOutputTypeDef

```python
# DashAdditionalManifestOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DashAdditionalManifestOutputTypeDef


def get_value() -> DashAdditionalManifestOutputTypeDef:
    return {
        "ManifestNameModifier": ...,
    }


# DashAdditionalManifestOutputTypeDef definition

class DashAdditionalManifestOutputTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[List[str]],
```

## DashAdditionalManifestTypeDef

```python
# DashAdditionalManifestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DashAdditionalManifestTypeDef


def get_value() -> DashAdditionalManifestTypeDef:
    return {
        "ManifestNameModifier": ...,
    }


# DashAdditionalManifestTypeDef definition

class DashAdditionalManifestTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[Sequence[str]],
```

## DashIsoImageBasedTrickPlaySettingsTypeDef

```python
# DashIsoImageBasedTrickPlaySettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DashIsoImageBasedTrickPlaySettingsTypeDef


def get_value() -> DashIsoImageBasedTrickPlaySettingsTypeDef:
    return {
        "IntervalCadence": ...,
    }


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
# DeinterlacerTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DeinterlacerTypeDef


def get_value() -> DeinterlacerTypeDef:
    return {
        "Algorithm": ...,
    }


# DeinterlacerTypeDef definition

class DeinterlacerTypeDef(TypedDict):
    Algorithm: NotRequired[DeinterlaceAlgorithmType],  # (1)
    Control: NotRequired[DeinterlacerControlType],  # (2)
    Mode: NotRequired[DeinterlacerModeType],  # (3)
```

1. See [:material-code-brackets: DeinterlaceAlgorithmType](./literals.md#deinterlacealgorithmtype) 
2. See [:material-code-brackets: DeinterlacerControlType](./literals.md#deinterlacercontroltype) 
3. See [:material-code-brackets: DeinterlacerModeType](./literals.md#deinterlacermodetype) 
## DeleteJobTemplateRequestTypeDef

```python
# DeleteJobTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DeleteJobTemplateRequestTypeDef


def get_value() -> DeleteJobTemplateRequestTypeDef:
    return {
        "Name": ...,
    }


# DeleteJobTemplateRequestTypeDef definition

class DeleteJobTemplateRequestTypeDef(TypedDict):
    Name: str,
```

## DeletePresetRequestTypeDef

```python
# DeletePresetRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DeletePresetRequestTypeDef


def get_value() -> DeletePresetRequestTypeDef:
    return {
        "Name": ...,
    }


# DeletePresetRequestTypeDef definition

class DeletePresetRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteQueueRequestTypeDef

```python
# DeleteQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DeleteQueueRequestTypeDef


def get_value() -> DeleteQueueRequestTypeDef:
    return {
        "Name": ...,
    }


# DeleteQueueRequestTypeDef definition

class DeleteQueueRequestTypeDef(TypedDict):
    Name: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import PaginatorConfigTypeDef


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

## DescribeEndpointsRequestTypeDef

```python
# DescribeEndpointsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DescribeEndpointsRequestTypeDef


def get_value() -> DescribeEndpointsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# DescribeEndpointsRequestTypeDef definition

class DescribeEndpointsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    Mode: NotRequired[DescribeEndpointsModeType],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: DescribeEndpointsModeType](./literals.md#describeendpointsmodetype) 
## EndpointTypeDef

```python
# EndpointTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import EndpointTypeDef


def get_value() -> EndpointTypeDef:
    return {
        "Url": ...,
    }


# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Url: NotRequired[str],
```

## DisassociateCertificateRequestTypeDef

```python
# DisassociateCertificateRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DisassociateCertificateRequestTypeDef


def get_value() -> DisassociateCertificateRequestTypeDef:
    return {
        "Arn": ...,
    }


# DisassociateCertificateRequestTypeDef definition

class DisassociateCertificateRequestTypeDef(TypedDict):
    Arn: str,
```

## DolbyVisionLevel6MetadataTypeDef

```python
# DolbyVisionLevel6MetadataTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DolbyVisionLevel6MetadataTypeDef


def get_value() -> DolbyVisionLevel6MetadataTypeDef:
    return {
        "MaxCll": ...,
    }


# DolbyVisionLevel6MetadataTypeDef definition

class DolbyVisionLevel6MetadataTypeDef(TypedDict):
    MaxCll: NotRequired[int],
    MaxFall: NotRequired[int],
```

## DvbNitSettingsTypeDef

```python
# DvbNitSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DvbNitSettingsTypeDef


def get_value() -> DvbNitSettingsTypeDef:
    return {
        "NetworkId": ...,
    }


# DvbNitSettingsTypeDef definition

class DvbNitSettingsTypeDef(TypedDict):
    NetworkId: NotRequired[int],
    NetworkName: NotRequired[str],
    NitInterval: NotRequired[int],
```

## DvbSdtSettingsTypeDef

```python
# DvbSdtSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DvbSdtSettingsTypeDef


def get_value() -> DvbSdtSettingsTypeDef:
    return {
        "OutputSdt": ...,
    }


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
# DvbTdtSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DvbTdtSettingsTypeDef


def get_value() -> DvbTdtSettingsTypeDef:
    return {
        "TdtInterval": ...,
    }


# DvbTdtSettingsTypeDef definition

class DvbTdtSettingsTypeDef(TypedDict):
    TdtInterval: NotRequired[int],
```

## DynamicAudioSelectorTypeDef

```python
# DynamicAudioSelectorTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DynamicAudioSelectorTypeDef


def get_value() -> DynamicAudioSelectorTypeDef:
    return {
        "AudioDurationCorrection": ...,
    }


# DynamicAudioSelectorTypeDef definition

class DynamicAudioSelectorTypeDef(TypedDict):
    AudioDurationCorrection: NotRequired[AudioDurationCorrectionType],  # (1)
    ExternalAudioFileInput: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    Offset: NotRequired[int],
    SelectorType: NotRequired[DynamicAudioSelectorTypeType],  # (3)
```

1. See [:material-code-brackets: AudioDurationCorrectionType](./literals.md#audiodurationcorrectiontype) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-brackets: DynamicAudioSelectorTypeType](./literals.md#dynamicaudioselectortypetype) 
## EncryptionContractConfigurationTypeDef

```python
# EncryptionContractConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import EncryptionContractConfigurationTypeDef


def get_value() -> EncryptionContractConfigurationTypeDef:
    return {
        "SpekeAudioPreset": ...,
    }


# EncryptionContractConfigurationTypeDef definition

class EncryptionContractConfigurationTypeDef(TypedDict):
    SpekeAudioPreset: NotRequired[PresetSpeke20AudioType],  # (1)
    SpekeVideoPreset: NotRequired[PresetSpeke20VideoType],  # (2)
```

1. See [:material-code-brackets: PresetSpeke20AudioType](./literals.md#presetspeke20audiotype) 
2. See [:material-code-brackets: PresetSpeke20VideoType](./literals.md#presetspeke20videotype) 
## EsamManifestConfirmConditionNotificationTypeDef

```python
# EsamManifestConfirmConditionNotificationTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import EsamManifestConfirmConditionNotificationTypeDef


def get_value() -> EsamManifestConfirmConditionNotificationTypeDef:
    return {
        "MccXml": ...,
    }


# EsamManifestConfirmConditionNotificationTypeDef definition

class EsamManifestConfirmConditionNotificationTypeDef(TypedDict):
    MccXml: NotRequired[str],
```

## EsamSignalProcessingNotificationTypeDef

```python
# EsamSignalProcessingNotificationTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import EsamSignalProcessingNotificationTypeDef


def get_value() -> EsamSignalProcessingNotificationTypeDef:
    return {
        "SccXml": ...,
    }


# EsamSignalProcessingNotificationTypeDef definition

class EsamSignalProcessingNotificationTypeDef(TypedDict):
    SccXml: NotRequired[str],
```

## ExtendedDataServicesTypeDef

```python
# ExtendedDataServicesTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ExtendedDataServicesTypeDef


def get_value() -> ExtendedDataServicesTypeDef:
    return {
        "CopyProtectionAction": ...,
    }


# ExtendedDataServicesTypeDef definition

class ExtendedDataServicesTypeDef(TypedDict):
    CopyProtectionAction: NotRequired[CopyProtectionActionType],  # (1)
    VchipAction: NotRequired[VchipActionType],  # (2)
```

1. See [:material-code-brackets: CopyProtectionActionType](./literals.md#copyprotectionactiontype) 
2. See [:material-code-brackets: VchipActionType](./literals.md#vchipactiontype) 
## FrameCaptureSettingsTypeDef

```python
# FrameCaptureSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import FrameCaptureSettingsTypeDef


def get_value() -> FrameCaptureSettingsTypeDef:
    return {
        "FramerateDenominator": ...,
    }


# FrameCaptureSettingsTypeDef definition

class FrameCaptureSettingsTypeDef(TypedDict):
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    MaxCaptures: NotRequired[int],
    Quality: NotRequired[int],
```

## GetJobRequestTypeDef

```python
# GetJobRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import GetJobRequestTypeDef


def get_value() -> GetJobRequestTypeDef:
    return {
        "Id": ...,
    }


# GetJobRequestTypeDef definition

class GetJobRequestTypeDef(TypedDict):
    Id: str,
```

## GetJobTemplateRequestTypeDef

```python
# GetJobTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import GetJobTemplateRequestTypeDef


def get_value() -> GetJobTemplateRequestTypeDef:
    return {
        "Name": ...,
    }


# GetJobTemplateRequestTypeDef definition

class GetJobTemplateRequestTypeDef(TypedDict):
    Name: str,
```

## PolicyTypeDef

```python
# PolicyTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import PolicyTypeDef


def get_value() -> PolicyTypeDef:
    return {
        "HttpInputs": ...,
    }


# PolicyTypeDef definition

class PolicyTypeDef(TypedDict):
    HttpInputs: NotRequired[InputPolicyType],  # (1)
    HttpsInputs: NotRequired[InputPolicyType],  # (1)
    S3Inputs: NotRequired[InputPolicyType],  # (1)
```

1. See [:material-code-brackets: InputPolicyType](./literals.md#inputpolicytype) 
2. See [:material-code-brackets: InputPolicyType](./literals.md#inputpolicytype) 
3. See [:material-code-brackets: InputPolicyType](./literals.md#inputpolicytype) 
## GetPresetRequestTypeDef

```python
# GetPresetRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import GetPresetRequestTypeDef


def get_value() -> GetPresetRequestTypeDef:
    return {
        "Name": ...,
    }


# GetPresetRequestTypeDef definition

class GetPresetRequestTypeDef(TypedDict):
    Name: str,
```

## GetQueueRequestTypeDef

```python
# GetQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import GetQueueRequestTypeDef


def get_value() -> GetQueueRequestTypeDef:
    return {
        "Name": ...,
    }


# GetQueueRequestTypeDef definition

class GetQueueRequestTypeDef(TypedDict):
    Name: str,
```

## GifSettingsTypeDef

```python
# GifSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import GifSettingsTypeDef


def get_value() -> GifSettingsTypeDef:
    return {
        "FramerateControl": ...,
    }


# GifSettingsTypeDef definition

class GifSettingsTypeDef(TypedDict):
    FramerateControl: NotRequired[GifFramerateControlType],  # (1)
    FramerateConversionAlgorithm: NotRequired[GifFramerateConversionAlgorithmType],  # (2)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
```

1. See [:material-code-brackets: GifFramerateControlType](./literals.md#gifframeratecontroltype) 
2. See [:material-code-brackets: GifFramerateConversionAlgorithmType](./literals.md#gifframerateconversionalgorithmtype) 
## H264QvbrSettingsTypeDef

```python
# H264QvbrSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import H264QvbrSettingsTypeDef


def get_value() -> H264QvbrSettingsTypeDef:
    return {
        "MaxAverageBitrate": ...,
    }


# H264QvbrSettingsTypeDef definition

class H264QvbrSettingsTypeDef(TypedDict):
    MaxAverageBitrate: NotRequired[int],
    QvbrQualityLevel: NotRequired[int],
    QvbrQualityLevelFineTune: NotRequired[float],
```

## H265QvbrSettingsTypeDef

```python
# H265QvbrSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import H265QvbrSettingsTypeDef


def get_value() -> H265QvbrSettingsTypeDef:
    return {
        "MaxAverageBitrate": ...,
    }


# H265QvbrSettingsTypeDef definition

class H265QvbrSettingsTypeDef(TypedDict):
    MaxAverageBitrate: NotRequired[int],
    QvbrQualityLevel: NotRequired[int],
    QvbrQualityLevelFineTune: NotRequired[float],
```

## Hdr10PlusTypeDef

```python
# Hdr10PlusTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Hdr10PlusTypeDef


def get_value() -> Hdr10PlusTypeDef:
    return {
        "MasteringMonitorNits": ...,
    }


# Hdr10PlusTypeDef definition

class Hdr10PlusTypeDef(TypedDict):
    MasteringMonitorNits: NotRequired[int],
    TargetMonitorNits: NotRequired[int],
```

## HlsAdditionalManifestOutputTypeDef

```python
# HlsAdditionalManifestOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import HlsAdditionalManifestOutputTypeDef


def get_value() -> HlsAdditionalManifestOutputTypeDef:
    return {
        "ManifestNameModifier": ...,
    }


# HlsAdditionalManifestOutputTypeDef definition

class HlsAdditionalManifestOutputTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[List[str]],
```

## HlsAdditionalManifestTypeDef

```python
# HlsAdditionalManifestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import HlsAdditionalManifestTypeDef


def get_value() -> HlsAdditionalManifestTypeDef:
    return {
        "ManifestNameModifier": ...,
    }


# HlsAdditionalManifestTypeDef definition

class HlsAdditionalManifestTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[Sequence[str]],
```

## HlsCaptionLanguageMappingTypeDef

```python
# HlsCaptionLanguageMappingTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import HlsCaptionLanguageMappingTypeDef


def get_value() -> HlsCaptionLanguageMappingTypeDef:
    return {
        "CaptionChannel": ...,
    }


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
# HlsImageBasedTrickPlaySettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import HlsImageBasedTrickPlaySettingsTypeDef


def get_value() -> HlsImageBasedTrickPlaySettingsTypeDef:
    return {
        "IntervalCadence": ...,
    }


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
# HlsSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import HlsSettingsTypeDef


def get_value() -> HlsSettingsTypeDef:
    return {
        "AudioGroupId": ...,
    }


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
# Id3InsertionTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Id3InsertionTypeDef


def get_value() -> Id3InsertionTypeDef:
    return {
        "Id3": ...,
    }


# Id3InsertionTypeDef definition

class Id3InsertionTypeDef(TypedDict):
    Id3: NotRequired[str],
    Timecode: NotRequired[str],
```

## InsertableImageTypeDef

```python
# InsertableImageTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import InsertableImageTypeDef


def get_value() -> InsertableImageTypeDef:
    return {
        "Duration": ...,
    }


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
# InputClippingTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import InputClippingTypeDef


def get_value() -> InputClippingTypeDef:
    return {
        "EndTimecode": ...,
    }


# InputClippingTypeDef definition

class InputClippingTypeDef(TypedDict):
    EndTimecode: NotRequired[str],
    StartTimecode: NotRequired[str],
```

## InputDecryptionSettingsTypeDef

```python
# InputDecryptionSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import InputDecryptionSettingsTypeDef


def get_value() -> InputDecryptionSettingsTypeDef:
    return {
        "DecryptionMode": ...,
    }


# InputDecryptionSettingsTypeDef definition

class InputDecryptionSettingsTypeDef(TypedDict):
    DecryptionMode: NotRequired[DecryptionModeType],  # (1)
    EncryptedDecryptionKey: NotRequired[str],
    InitializationVector: NotRequired[str],
    KmsKeyRegion: NotRequired[str],
```

1. See [:material-code-brackets: DecryptionModeType](./literals.md#decryptionmodetype) 
## InputVideoGeneratorTypeDef

```python
# InputVideoGeneratorTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import InputVideoGeneratorTypeDef


def get_value() -> InputVideoGeneratorTypeDef:
    return {
        "Channels": ...,
    }


# InputVideoGeneratorTypeDef definition

class InputVideoGeneratorTypeDef(TypedDict):
    Channels: NotRequired[int],
    Duration: NotRequired[int],
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    SampleRate: NotRequired[int],
```

## RectangleTypeDef

```python
# RectangleTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import RectangleTypeDef


def get_value() -> RectangleTypeDef:
    return {
        "Height": ...,
    }


# RectangleTypeDef definition

class RectangleTypeDef(TypedDict):
    Height: NotRequired[int],
    Width: NotRequired[int],
    X: NotRequired[int],
    Y: NotRequired[int],
```

## JobEngineVersionTypeDef

```python
# JobEngineVersionTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import JobEngineVersionTypeDef


def get_value() -> JobEngineVersionTypeDef:
    return {
        "ExpirationDate": ...,
    }


# JobEngineVersionTypeDef definition

class JobEngineVersionTypeDef(TypedDict):
    ExpirationDate: NotRequired[datetime],
    Version: NotRequired[str],
```

## JobMessagesTypeDef

```python
# JobMessagesTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import JobMessagesTypeDef


def get_value() -> JobMessagesTypeDef:
    return {
        "Info": ...,
    }


# JobMessagesTypeDef definition

class JobMessagesTypeDef(TypedDict):
    Info: NotRequired[List[str]],
    Warning: NotRequired[List[str]],
```

## KantarWatermarkSettingsTypeDef

```python
# KantarWatermarkSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import KantarWatermarkSettingsTypeDef


def get_value() -> KantarWatermarkSettingsTypeDef:
    return {
        "ChannelName": ...,
    }


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
# NielsenConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import NielsenConfigurationTypeDef


def get_value() -> NielsenConfigurationTypeDef:
    return {
        "BreakoutCode": ...,
    }


# NielsenConfigurationTypeDef definition

class NielsenConfigurationTypeDef(TypedDict):
    BreakoutCode: NotRequired[int],
    DistributorId: NotRequired[str],
```

## NielsenNonLinearWatermarkSettingsTypeDef

```python
# NielsenNonLinearWatermarkSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import NielsenNonLinearWatermarkSettingsTypeDef


def get_value() -> NielsenNonLinearWatermarkSettingsTypeDef:
    return {
        "ActiveWatermarkProcess": ...,
    }


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
# TimecodeConfigTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import TimecodeConfigTypeDef


def get_value() -> TimecodeConfigTypeDef:
    return {
        "Anchor": ...,
    }


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
# QueueTransitionTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import QueueTransitionTypeDef


def get_value() -> QueueTransitionTypeDef:
    return {
        "DestinationQueue": ...,
    }


# QueueTransitionTypeDef definition

class QueueTransitionTypeDef(TypedDict):
    DestinationQueue: NotRequired[str],
    SourceQueue: NotRequired[str],
    Timestamp: NotRequired[datetime],
```

## TimingTypeDef

```python
# TimingTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import TimingTypeDef


def get_value() -> TimingTypeDef:
    return {
        "FinishTime": ...,
    }


# TimingTypeDef definition

class TimingTypeDef(TypedDict):
    FinishTime: NotRequired[datetime],
    StartTime: NotRequired[datetime],
    SubmitTime: NotRequired[datetime],
```

## WarningGroupTypeDef

```python
# WarningGroupTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import WarningGroupTypeDef


def get_value() -> WarningGroupTypeDef:
    return {
        "Code": ...,
    }


# WarningGroupTypeDef definition

class WarningGroupTypeDef(TypedDict):
    Code: int,
    Count: int,
```

## ListJobTemplatesRequestTypeDef

```python
# ListJobTemplatesRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListJobTemplatesRequestTypeDef


def get_value() -> ListJobTemplatesRequestTypeDef:
    return {
        "Category": ...,
    }


# ListJobTemplatesRequestTypeDef definition

class ListJobTemplatesRequestTypeDef(TypedDict):
    Category: NotRequired[str],
    ListBy: NotRequired[JobTemplateListByType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Order: NotRequired[OrderType],  # (2)
```

1. See [:material-code-brackets: JobTemplateListByType](./literals.md#jobtemplatelistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## ListJobsRequestTypeDef

```python
# ListJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListJobsRequestTypeDef


def get_value() -> ListJobsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListJobsRequestTypeDef definition

class ListJobsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Order: NotRequired[OrderType],  # (1)
    Queue: NotRequired[str],
    Status: NotRequired[JobStatusType],  # (2)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## ListPresetsRequestTypeDef

```python
# ListPresetsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListPresetsRequestTypeDef


def get_value() -> ListPresetsRequestTypeDef:
    return {
        "Category": ...,
    }


# ListPresetsRequestTypeDef definition

class ListPresetsRequestTypeDef(TypedDict):
    Category: NotRequired[str],
    ListBy: NotRequired[PresetListByType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Order: NotRequired[OrderType],  # (2)
```

1. See [:material-code-brackets: PresetListByType](./literals.md#presetlistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## ListQueuesRequestTypeDef

```python
# ListQueuesRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListQueuesRequestTypeDef


def get_value() -> ListQueuesRequestTypeDef:
    return {
        "ListBy": ...,
    }


# ListQueuesRequestTypeDef definition

class ListQueuesRequestTypeDef(TypedDict):
    ListBy: NotRequired[QueueListByType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Order: NotRequired[OrderType],  # (2)
```

1. See [:material-code-brackets: QueueListByType](./literals.md#queuelistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "Arn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    Arn: str,
```

## ResourceTagsTypeDef

```python
# ResourceTagsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ResourceTagsTypeDef


def get_value() -> ResourceTagsTypeDef:
    return {
        "Arn": ...,
    }


# ResourceTagsTypeDef definition

class ResourceTagsTypeDef(TypedDict):
    Arn: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

## ListVersionsRequestTypeDef

```python
# ListVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListVersionsRequestTypeDef


def get_value() -> ListVersionsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListVersionsRequestTypeDef definition

class ListVersionsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## M2tsScte35EsamTypeDef

```python
# M2tsScte35EsamTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import M2tsScte35EsamTypeDef


def get_value() -> M2tsScte35EsamTypeDef:
    return {
        "Scte35EsamPid": ...,
    }


# M2tsScte35EsamTypeDef definition

class M2tsScte35EsamTypeDef(TypedDict):
    Scte35EsamPid: NotRequired[int],
```

## MotionImageInsertionFramerateTypeDef

```python
# MotionImageInsertionFramerateTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MotionImageInsertionFramerateTypeDef


def get_value() -> MotionImageInsertionFramerateTypeDef:
    return {
        "FramerateDenominator": ...,
    }


# MotionImageInsertionFramerateTypeDef definition

class MotionImageInsertionFramerateTypeDef(TypedDict):
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
```

## MotionImageInsertionOffsetTypeDef

```python
# MotionImageInsertionOffsetTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MotionImageInsertionOffsetTypeDef


def get_value() -> MotionImageInsertionOffsetTypeDef:
    return {
        "ImageX": ...,
    }


# MotionImageInsertionOffsetTypeDef definition

class MotionImageInsertionOffsetTypeDef(TypedDict):
    ImageX: NotRequired[int],
    ImageY: NotRequired[int],
```

## Mpeg2SettingsTypeDef

```python
# Mpeg2SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Mpeg2SettingsTypeDef


def get_value() -> Mpeg2SettingsTypeDef:
    return {
        "AdaptiveQuantization": ...,
    }


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
## MsSmoothAdditionalManifestOutputTypeDef

```python
# MsSmoothAdditionalManifestOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MsSmoothAdditionalManifestOutputTypeDef


def get_value() -> MsSmoothAdditionalManifestOutputTypeDef:
    return {
        "ManifestNameModifier": ...,
    }


# MsSmoothAdditionalManifestOutputTypeDef definition

class MsSmoothAdditionalManifestOutputTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[List[str]],
```

## MsSmoothAdditionalManifestTypeDef

```python
# MsSmoothAdditionalManifestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MsSmoothAdditionalManifestTypeDef


def get_value() -> MsSmoothAdditionalManifestTypeDef:
    return {
        "ManifestNameModifier": ...,
    }


# MsSmoothAdditionalManifestTypeDef definition

class MsSmoothAdditionalManifestTypeDef(TypedDict):
    ManifestNameModifier: NotRequired[str],
    SelectedOutputs: NotRequired[Sequence[str]],
```

## MxfXavcProfileSettingsTypeDef

```python
# MxfXavcProfileSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MxfXavcProfileSettingsTypeDef


def get_value() -> MxfXavcProfileSettingsTypeDef:
    return {
        "DurationMode": ...,
    }


# MxfXavcProfileSettingsTypeDef definition

class MxfXavcProfileSettingsTypeDef(TypedDict):
    DurationMode: NotRequired[MxfXavcDurationModeType],  # (1)
    MaxAncDataSize: NotRequired[int],
```

1. See [:material-code-brackets: MxfXavcDurationModeType](./literals.md#mxfxavcdurationmodetype) 
## NexGuardFileMarkerSettingsTypeDef

```python
# NexGuardFileMarkerSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import NexGuardFileMarkerSettingsTypeDef


def get_value() -> NexGuardFileMarkerSettingsTypeDef:
    return {
        "License": ...,
    }


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
# NoiseReducerFilterSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import NoiseReducerFilterSettingsTypeDef


def get_value() -> NoiseReducerFilterSettingsTypeDef:
    return {
        "Strength": ...,
    }


# NoiseReducerFilterSettingsTypeDef definition

class NoiseReducerFilterSettingsTypeDef(TypedDict):
    Strength: NotRequired[int],
```

## NoiseReducerSpatialFilterSettingsTypeDef

```python
# NoiseReducerSpatialFilterSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import NoiseReducerSpatialFilterSettingsTypeDef


def get_value() -> NoiseReducerSpatialFilterSettingsTypeDef:
    return {
        "PostFilterSharpenStrength": ...,
    }


# NoiseReducerSpatialFilterSettingsTypeDef definition

class NoiseReducerSpatialFilterSettingsTypeDef(TypedDict):
    PostFilterSharpenStrength: NotRequired[int],
    Speed: NotRequired[int],
    Strength: NotRequired[int],
```

## NoiseReducerTemporalFilterSettingsTypeDef

```python
# NoiseReducerTemporalFilterSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import NoiseReducerTemporalFilterSettingsTypeDef


def get_value() -> NoiseReducerTemporalFilterSettingsTypeDef:
    return {
        "AggressiveMode": ...,
    }


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
# VideoDetailTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoDetailTypeDef


def get_value() -> VideoDetailTypeDef:
    return {
        "HeightInPx": ...,
    }


# VideoDetailTypeDef definition

class VideoDetailTypeDef(TypedDict):
    HeightInPx: NotRequired[int],
    WidthInPx: NotRequired[int],
```

## ProresSettingsTypeDef

```python
# ProresSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ProresSettingsTypeDef


def get_value() -> ProresSettingsTypeDef:
    return {
        "ChromaSampling": ...,
    }


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
# ReservationPlanTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ReservationPlanTypeDef


def get_value() -> ReservationPlanTypeDef:
    return {
        "Commitment": ...,
    }


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
## ServiceOverrideTypeDef

```python
# ServiceOverrideTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ServiceOverrideTypeDef


def get_value() -> ServiceOverrideTypeDef:
    return {
        "Message": ...,
    }


# ServiceOverrideTypeDef definition

class ServiceOverrideTypeDef(TypedDict):
    Message: NotRequired[str],
    Name: NotRequired[str],
    OverrideValue: NotRequired[str],
    Value: NotRequired[str],
```

## S3DestinationAccessControlTypeDef

```python
# S3DestinationAccessControlTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import S3DestinationAccessControlTypeDef


def get_value() -> S3DestinationAccessControlTypeDef:
    return {
        "CannedAcl": ...,
    }


# S3DestinationAccessControlTypeDef definition

class S3DestinationAccessControlTypeDef(TypedDict):
    CannedAcl: NotRequired[S3ObjectCannedAclType],  # (1)
```

1. See [:material-code-brackets: S3ObjectCannedAclType](./literals.md#s3objectcannedacltype) 
## S3EncryptionSettingsTypeDef

```python
# S3EncryptionSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import S3EncryptionSettingsTypeDef


def get_value() -> S3EncryptionSettingsTypeDef:
    return {
        "EncryptionType": ...,
    }


# S3EncryptionSettingsTypeDef definition

class S3EncryptionSettingsTypeDef(TypedDict):
    EncryptionType: NotRequired[S3ServerSideEncryptionTypeType],  # (1)
    KmsEncryptionContext: NotRequired[str],
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: S3ServerSideEncryptionTypeType](./literals.md#s3serversideencryptiontypetype) 
## SearchJobsRequestTypeDef

```python
# SearchJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import SearchJobsRequestTypeDef


def get_value() -> SearchJobsRequestTypeDef:
    return {
        "InputFile": ...,
    }


# SearchJobsRequestTypeDef definition

class SearchJobsRequestTypeDef(TypedDict):
    InputFile: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Order: NotRequired[OrderType],  # (1)
    Queue: NotRequired[str],
    Status: NotRequired[JobStatusType],  # (2)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "Arn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    Arn: str,
    Tags: Mapping[str, str],
```

## TimecodeBurninTypeDef

```python
# TimecodeBurninTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import TimecodeBurninTypeDef


def get_value() -> TimecodeBurninTypeDef:
    return {
        "FontSize": ...,
    }


# TimecodeBurninTypeDef definition

class TimecodeBurninTypeDef(TypedDict):
    FontSize: NotRequired[int],
    Position: NotRequired[TimecodeBurninPositionType],  # (1)
    Prefix: NotRequired[str],
```

1. See [:material-code-brackets: TimecodeBurninPositionType](./literals.md#timecodeburninpositiontype) 
## UncompressedSettingsTypeDef

```python
# UncompressedSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import UncompressedSettingsTypeDef


def get_value() -> UncompressedSettingsTypeDef:
    return {
        "Fourcc": ...,
    }


# UncompressedSettingsTypeDef definition

class UncompressedSettingsTypeDef(TypedDict):
    Fourcc: NotRequired[UncompressedFourccType],  # (1)
    FramerateControl: NotRequired[UncompressedFramerateControlType],  # (2)
    FramerateConversionAlgorithm: NotRequired[UncompressedFramerateConversionAlgorithmType],  # (3)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    InterlaceMode: NotRequired[UncompressedInterlaceModeType],  # (4)
    ScanTypeConversionMode: NotRequired[UncompressedScanTypeConversionModeType],  # (5)
    SlowPal: NotRequired[UncompressedSlowPalType],  # (6)
    Telecine: NotRequired[UncompressedTelecineType],  # (7)
```

1. See [:material-code-brackets: UncompressedFourccType](./literals.md#uncompressedfourcctype) 
2. See [:material-code-brackets: UncompressedFramerateControlType](./literals.md#uncompressedframeratecontroltype) 
3. See [:material-code-brackets: UncompressedFramerateConversionAlgorithmType](./literals.md#uncompressedframerateconversionalgorithmtype) 
4. See [:material-code-brackets: UncompressedInterlaceModeType](./literals.md#uncompressedinterlacemodetype) 
5. See [:material-code-brackets: UncompressedScanTypeConversionModeType](./literals.md#uncompressedscantypeconversionmodetype) 
6. See [:material-code-brackets: UncompressedSlowPalType](./literals.md#uncompressedslowpaltype) 
7. See [:material-code-brackets: UncompressedTelecineType](./literals.md#uncompressedtelecinetype) 
## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "Arn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    Arn: str,
    TagKeys: NotRequired[Sequence[str]],
```

## Vc3SettingsTypeDef

```python
# Vc3SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Vc3SettingsTypeDef


def get_value() -> Vc3SettingsTypeDef:
    return {
        "FramerateControl": ...,
    }


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
# Vp8SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Vp8SettingsTypeDef


def get_value() -> Vp8SettingsTypeDef:
    return {
        "Bitrate": ...,
    }


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
# Vp9SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Vp9SettingsTypeDef


def get_value() -> Vp9SettingsTypeDef:
    return {
        "Bitrate": ...,
    }


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
## VideoOverlayInputClippingTypeDef

```python
# VideoOverlayInputClippingTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoOverlayInputClippingTypeDef


def get_value() -> VideoOverlayInputClippingTypeDef:
    return {
        "EndTimecode": ...,
    }


# VideoOverlayInputClippingTypeDef definition

class VideoOverlayInputClippingTypeDef(TypedDict):
    EndTimecode: NotRequired[str],
    StartTimecode: NotRequired[str],
```

## VideoOverlayPositionTypeDef

```python
# VideoOverlayPositionTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoOverlayPositionTypeDef


def get_value() -> VideoOverlayPositionTypeDef:
    return {
        "Height": ...,
    }


# VideoOverlayPositionTypeDef definition

class VideoOverlayPositionTypeDef(TypedDict):
    Height: NotRequired[int],
    Unit: NotRequired[VideoOverlayUnitType],  # (1)
    Width: NotRequired[int],
    XPosition: NotRequired[int],
    YPosition: NotRequired[int],
```

1. See [:material-code-brackets: VideoOverlayUnitType](./literals.md#videooverlayunittype) 
## Xavc4kIntraCbgProfileSettingsTypeDef

```python
# Xavc4kIntraCbgProfileSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Xavc4kIntraCbgProfileSettingsTypeDef


def get_value() -> Xavc4kIntraCbgProfileSettingsTypeDef:
    return {
        "XavcClass": ...,
    }


# Xavc4kIntraCbgProfileSettingsTypeDef definition

class Xavc4kIntraCbgProfileSettingsTypeDef(TypedDict):
    XavcClass: NotRequired[Xavc4kIntraCbgProfileClassType],  # (1)
```

1. See [:material-code-brackets: Xavc4kIntraCbgProfileClassType](./literals.md#xavc4kintracbgprofileclasstype) 
## Xavc4kIntraVbrProfileSettingsTypeDef

```python
# Xavc4kIntraVbrProfileSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Xavc4kIntraVbrProfileSettingsTypeDef


def get_value() -> Xavc4kIntraVbrProfileSettingsTypeDef:
    return {
        "XavcClass": ...,
    }


# Xavc4kIntraVbrProfileSettingsTypeDef definition

class Xavc4kIntraVbrProfileSettingsTypeDef(TypedDict):
    XavcClass: NotRequired[Xavc4kIntraVbrProfileClassType],  # (1)
```

1. See [:material-code-brackets: Xavc4kIntraVbrProfileClassType](./literals.md#xavc4kintravbrprofileclasstype) 
## Xavc4kProfileSettingsTypeDef

```python
# Xavc4kProfileSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Xavc4kProfileSettingsTypeDef


def get_value() -> Xavc4kProfileSettingsTypeDef:
    return {
        "BitrateClass": ...,
    }


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
# XavcHdIntraCbgProfileSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import XavcHdIntraCbgProfileSettingsTypeDef


def get_value() -> XavcHdIntraCbgProfileSettingsTypeDef:
    return {
        "XavcClass": ...,
    }


# XavcHdIntraCbgProfileSettingsTypeDef definition

class XavcHdIntraCbgProfileSettingsTypeDef(TypedDict):
    XavcClass: NotRequired[XavcHdIntraCbgProfileClassType],  # (1)
```

1. See [:material-code-brackets: XavcHdIntraCbgProfileClassType](./literals.md#xavchdintracbgprofileclasstype) 
## XavcHdProfileSettingsTypeDef

```python
# XavcHdProfileSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import XavcHdProfileSettingsTypeDef


def get_value() -> XavcHdProfileSettingsTypeDef:
    return {
        "BitrateClass": ...,
    }


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
# AudioCodecSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AudioCodecSettingsTypeDef


def get_value() -> AudioCodecSettingsTypeDef:
    return {
        "AacSettings": ...,
    }


# AudioCodecSettingsTypeDef definition

class AudioCodecSettingsTypeDef(TypedDict):
    AacSettings: NotRequired[AacSettingsTypeDef],  # (1)
    Ac3Settings: NotRequired[Ac3SettingsTypeDef],  # (2)
    AiffSettings: NotRequired[AiffSettingsTypeDef],  # (3)
    Codec: NotRequired[AudioCodecType],  # (4)
    Eac3AtmosSettings: NotRequired[Eac3AtmosSettingsTypeDef],  # (5)
    Eac3Settings: NotRequired[Eac3SettingsTypeDef],  # (6)
    FlacSettings: NotRequired[FlacSettingsTypeDef],  # (7)
    Mp2Settings: NotRequired[Mp2SettingsTypeDef],  # (8)
    Mp3Settings: NotRequired[Mp3SettingsTypeDef],  # (9)
    OpusSettings: NotRequired[OpusSettingsTypeDef],  # (10)
    VorbisSettings: NotRequired[VorbisSettingsTypeDef],  # (11)
    WavSettings: NotRequired[WavSettingsTypeDef],  # (12)
```

1. See [:material-code-braces: AacSettingsTypeDef](./type_defs.md#aacsettingstypedef) 
2. See [:material-code-braces: Ac3SettingsTypeDef](./type_defs.md#ac3settingstypedef) 
3. See [:material-code-braces: AiffSettingsTypeDef](./type_defs.md#aiffsettingstypedef) 
4. See [:material-code-brackets: AudioCodecType](./literals.md#audiocodectype) 
5. See [:material-code-braces: Eac3AtmosSettingsTypeDef](./type_defs.md#eac3atmossettingstypedef) 
6. See [:material-code-braces: Eac3SettingsTypeDef](./type_defs.md#eac3settingstypedef) 
7. See [:material-code-braces: FlacSettingsTypeDef](./type_defs.md#flacsettingstypedef) 
8. See [:material-code-braces: Mp2SettingsTypeDef](./type_defs.md#mp2settingstypedef) 
9. See [:material-code-braces: Mp3SettingsTypeDef](./type_defs.md#mp3settingstypedef) 
10. See [:material-code-braces: OpusSettingsTypeDef](./type_defs.md#opussettingstypedef) 
11. See [:material-code-braces: VorbisSettingsTypeDef](./type_defs.md#vorbissettingstypedef) 
12. See [:material-code-braces: WavSettingsTypeDef](./type_defs.md#wavsettingstypedef) 
## AutomatedAbrRuleOutputTypeDef

```python
# AutomatedAbrRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AutomatedAbrRuleOutputTypeDef


def get_value() -> AutomatedAbrRuleOutputTypeDef:
    return {
        "AllowedRenditions": ...,
    }


# AutomatedAbrRuleOutputTypeDef definition

class AutomatedAbrRuleOutputTypeDef(TypedDict):
    AllowedRenditions: NotRequired[List[AllowedRenditionSizeTypeDef]],  # (1)
    ForceIncludeRenditions: NotRequired[List[ForceIncludeRenditionSizeTypeDef]],  # (2)
    MinBottomRenditionSize: NotRequired[MinBottomRenditionSizeTypeDef],  # (3)
    MinTopRenditionSize: NotRequired[MinTopRenditionSizeTypeDef],  # (4)
    Type: NotRequired[RuleTypeType],  # (5)
```

1. See [:material-code-braces: AllowedRenditionSizeTypeDef](./type_defs.md#allowedrenditionsizetypedef) 
2. See [:material-code-braces: ForceIncludeRenditionSizeTypeDef](./type_defs.md#forceincluderenditionsizetypedef) 
3. See [:material-code-braces: MinBottomRenditionSizeTypeDef](./type_defs.md#minbottomrenditionsizetypedef) 
4. See [:material-code-braces: MinTopRenditionSizeTypeDef](./type_defs.md#mintoprenditionsizetypedef) 
5. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
## AutomatedAbrRuleTypeDef

```python
# AutomatedAbrRuleTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AutomatedAbrRuleTypeDef


def get_value() -> AutomatedAbrRuleTypeDef:
    return {
        "AllowedRenditions": ...,
    }


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
# Av1SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import Av1SettingsTypeDef


def get_value() -> Av1SettingsTypeDef:
    return {
        "AdaptiveQuantization": ...,
    }


# Av1SettingsTypeDef definition

class Av1SettingsTypeDef(TypedDict):
    AdaptiveQuantization: NotRequired[Av1AdaptiveQuantizationType],  # (1)
    BitDepth: NotRequired[Av1BitDepthType],  # (2)
    FilmGrainSynthesis: NotRequired[Av1FilmGrainSynthesisType],  # (3)
    FramerateControl: NotRequired[Av1FramerateControlType],  # (4)
    FramerateConversionAlgorithm: NotRequired[Av1FramerateConversionAlgorithmType],  # (5)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    GopSize: NotRequired[float],
    MaxBitrate: NotRequired[int],
    NumberBFramesBetweenReferenceFrames: NotRequired[int],
    QvbrSettings: NotRequired[Av1QvbrSettingsTypeDef],  # (6)
    RateControlMode: NotRequired[Av1RateControlModeType],  # (7)
    Slices: NotRequired[int],
    SpatialAdaptiveQuantization: NotRequired[Av1SpatialAdaptiveQuantizationType],  # (8)
```

1. See [:material-code-brackets: Av1AdaptiveQuantizationType](./literals.md#av1adaptivequantizationtype) 
2. See [:material-code-brackets: Av1BitDepthType](./literals.md#av1bitdepthtype) 
3. See [:material-code-brackets: Av1FilmGrainSynthesisType](./literals.md#av1filmgrainsynthesistype) 
4. See [:material-code-brackets: Av1FramerateControlType](./literals.md#av1frameratecontroltype) 
5. See [:material-code-brackets: Av1FramerateConversionAlgorithmType](./literals.md#av1framerateconversionalgorithmtype) 
6. See [:material-code-braces: Av1QvbrSettingsTypeDef](./type_defs.md#av1qvbrsettingstypedef) 
7. See [:material-code-brackets: Av1RateControlModeType](./literals.md#av1ratecontrolmodetype) 
8. See [:material-code-brackets: Av1SpatialAdaptiveQuantizationType](./literals.md#av1spatialadaptivequantizationtype) 
## AvcIntraSettingsTypeDef

```python
# AvcIntraSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AvcIntraSettingsTypeDef


def get_value() -> AvcIntraSettingsTypeDef:
    return {
        "AvcIntraClass": ...,
    }


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
## CaptionDestinationSettingsOutputTypeDef

```python
# CaptionDestinationSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CaptionDestinationSettingsOutputTypeDef


def get_value() -> CaptionDestinationSettingsOutputTypeDef:
    return {
        "BurninDestinationSettings": ...,
    }


# CaptionDestinationSettingsOutputTypeDef definition

class CaptionDestinationSettingsOutputTypeDef(TypedDict):
    BurninDestinationSettings: NotRequired[BurninDestinationSettingsTypeDef],  # (1)
    DestinationType: NotRequired[CaptionDestinationTypeType],  # (2)
    DvbSubDestinationSettings: NotRequired[DvbSubDestinationSettingsTypeDef],  # (3)
    EmbeddedDestinationSettings: NotRequired[EmbeddedDestinationSettingsTypeDef],  # (4)
    ImscDestinationSettings: NotRequired[ImscDestinationSettingsTypeDef],  # (5)
    SccDestinationSettings: NotRequired[SccDestinationSettingsTypeDef],  # (6)
    SrtDestinationSettings: NotRequired[SrtDestinationSettingsTypeDef],  # (7)
    TeletextDestinationSettings: NotRequired[TeletextDestinationSettingsOutputTypeDef],  # (8)
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
8. See [:material-code-braces: TeletextDestinationSettingsOutputTypeDef](./type_defs.md#teletextdestinationsettingsoutputtypedef) 
9. See [:material-code-braces: TtmlDestinationSettingsTypeDef](./type_defs.md#ttmldestinationsettingstypedef) 
10. See [:material-code-braces: WebvttDestinationSettingsTypeDef](./type_defs.md#webvttdestinationsettingstypedef) 
## CaptionDestinationSettingsTypeDef

```python
# CaptionDestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CaptionDestinationSettingsTypeDef


def get_value() -> CaptionDestinationSettingsTypeDef:
    return {
        "BurninDestinationSettings": ...,
    }


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
# FileSourceSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import FileSourceSettingsTypeDef


def get_value() -> FileSourceSettingsTypeDef:
    return {
        "ByteRateLimit": ...,
    }


# FileSourceSettingsTypeDef definition

class FileSourceSettingsTypeDef(TypedDict):
    ByteRateLimit: NotRequired[CaptionSourceByteRateLimitType],  # (1)
    Convert608To708: NotRequired[FileSourceConvert608To708Type],  # (2)
    ConvertPaintToPop: NotRequired[CaptionSourceConvertPaintOnToPopOnType],  # (3)
    Framerate: NotRequired[CaptionSourceFramerateTypeDef],  # (4)
    SourceFile: NotRequired[str],
    TimeDelta: NotRequired[int],
    TimeDeltaUnits: NotRequired[FileSourceTimeDeltaUnitsType],  # (5)
```

1. See [:material-code-brackets: CaptionSourceByteRateLimitType](./literals.md#captionsourcebyteratelimittype) 
2. See [:material-code-brackets: FileSourceConvert608To708Type](./literals.md#filesourceconvert608to708type) 
3. See [:material-code-brackets: CaptionSourceConvertPaintOnToPopOnType](./literals.md#captionsourceconvertpaintontopopontype) 
4. See [:material-code-braces: CaptionSourceFramerateTypeDef](./type_defs.md#captionsourceframeratetypedef) 
5. See [:material-code-brackets: FileSourceTimeDeltaUnitsType](./literals.md#filesourcetimedeltaunitstype) 
## ChannelMappingOutputTypeDef

```python
# ChannelMappingOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ChannelMappingOutputTypeDef


def get_value() -> ChannelMappingOutputTypeDef:
    return {
        "OutputChannels": ...,
    }


# ChannelMappingOutputTypeDef definition

class ChannelMappingOutputTypeDef(TypedDict):
    OutputChannels: NotRequired[List[OutputChannelMappingOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: OutputChannelMappingOutputTypeDef](./type_defs.md#outputchannelmappingoutputtypedef) 
## ChannelMappingTypeDef

```python
# ChannelMappingTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ChannelMappingTypeDef


def get_value() -> ChannelMappingTypeDef:
    return {
        "OutputChannels": ...,
    }


# ChannelMappingTypeDef definition

class ChannelMappingTypeDef(TypedDict):
    OutputChannels: NotRequired[Sequence[OutputChannelMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: OutputChannelMappingTypeDef](./type_defs.md#outputchannelmappingtypedef) 
## ColorCorrectorTypeDef

```python
# ColorCorrectorTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ColorCorrectorTypeDef


def get_value() -> ColorCorrectorTypeDef:
    return {
        "Brightness": ...,
    }


# ColorCorrectorTypeDef definition

class ColorCorrectorTypeDef(TypedDict):
    Brightness: NotRequired[int],
    ClipLimits: NotRequired[ClipLimitsTypeDef],  # (1)
    ColorSpaceConversion: NotRequired[ColorSpaceConversionType],  # (2)
    Contrast: NotRequired[int],
    Hdr10Metadata: NotRequired[Hdr10MetadataTypeDef],  # (3)
    HdrToSdrToneMapper: NotRequired[HDRToSDRToneMapperType],  # (4)
    Hue: NotRequired[int],
    MaxLuminance: NotRequired[int],
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
# VideoSelectorTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoSelectorTypeDef


def get_value() -> VideoSelectorTypeDef:
    return {
        "AlphaBehavior": ...,
    }


# VideoSelectorTypeDef definition

class VideoSelectorTypeDef(TypedDict):
    AlphaBehavior: NotRequired[AlphaBehaviorType],  # (1)
    ColorSpace: NotRequired[ColorSpaceType],  # (2)
    ColorSpaceUsage: NotRequired[ColorSpaceUsageType],  # (3)
    EmbeddedTimecodeOverride: NotRequired[EmbeddedTimecodeOverrideType],  # (4)
    Hdr10Metadata: NotRequired[Hdr10MetadataTypeDef],  # (5)
    MaxLuminance: NotRequired[int],
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
## CreateQueueRequestTypeDef

```python
# CreateQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CreateQueueRequestTypeDef


def get_value() -> CreateQueueRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateQueueRequestTypeDef definition

class CreateQueueRequestTypeDef(TypedDict):
    Name: str,
    ConcurrentJobs: NotRequired[int],
    Description: NotRequired[str],
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    ReservationPlanSettings: NotRequired[ReservationPlanSettingsTypeDef],  # (2)
    Status: NotRequired[QueueStatusType],  # (3)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: ReservationPlanSettingsTypeDef](./type_defs.md#reservationplansettingstypedef) 
3. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
## UpdateQueueRequestTypeDef

```python
# UpdateQueueRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import UpdateQueueRequestTypeDef


def get_value() -> UpdateQueueRequestTypeDef:
    return {
        "Name": ...,
    }


# UpdateQueueRequestTypeDef definition

class UpdateQueueRequestTypeDef(TypedDict):
    Name: str,
    ConcurrentJobs: NotRequired[int],
    Description: NotRequired[str],
    ReservationPlanSettings: NotRequired[ReservationPlanSettingsTypeDef],  # (1)
    Status: NotRequired[QueueStatusType],  # (2)
```

1. See [:material-code-braces: ReservationPlanSettingsTypeDef](./type_defs.md#reservationplansettingstypedef) 
2. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
## DescribeEndpointsRequestPaginateTypeDef

```python
# DescribeEndpointsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DescribeEndpointsRequestPaginateTypeDef


def get_value() -> DescribeEndpointsRequestPaginateTypeDef:
    return {
        "Mode": ...,
    }


# DescribeEndpointsRequestPaginateTypeDef definition

class DescribeEndpointsRequestPaginateTypeDef(TypedDict):
    Mode: NotRequired[DescribeEndpointsModeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DescribeEndpointsModeType](./literals.md#describeendpointsmodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobTemplatesRequestPaginateTypeDef

```python
# ListJobTemplatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListJobTemplatesRequestPaginateTypeDef


def get_value() -> ListJobTemplatesRequestPaginateTypeDef:
    return {
        "Category": ...,
    }


# ListJobTemplatesRequestPaginateTypeDef definition

class ListJobTemplatesRequestPaginateTypeDef(TypedDict):
    Category: NotRequired[str],
    ListBy: NotRequired[JobTemplateListByType],  # (1)
    Order: NotRequired[OrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: JobTemplateListByType](./literals.md#jobtemplatelistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestPaginateTypeDef

```python
# ListJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListJobsRequestPaginateTypeDef


def get_value() -> ListJobsRequestPaginateTypeDef:
    return {
        "Order": ...,
    }


# ListJobsRequestPaginateTypeDef definition

class ListJobsRequestPaginateTypeDef(TypedDict):
    Order: NotRequired[OrderType],  # (1)
    Queue: NotRequired[str],
    Status: NotRequired[JobStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPresetsRequestPaginateTypeDef

```python
# ListPresetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListPresetsRequestPaginateTypeDef


def get_value() -> ListPresetsRequestPaginateTypeDef:
    return {
        "Category": ...,
    }


# ListPresetsRequestPaginateTypeDef definition

class ListPresetsRequestPaginateTypeDef(TypedDict):
    Category: NotRequired[str],
    ListBy: NotRequired[PresetListByType],  # (1)
    Order: NotRequired[OrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PresetListByType](./literals.md#presetlistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueuesRequestPaginateTypeDef

```python
# ListQueuesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListQueuesRequestPaginateTypeDef


def get_value() -> ListQueuesRequestPaginateTypeDef:
    return {
        "ListBy": ...,
    }


# ListQueuesRequestPaginateTypeDef definition

class ListQueuesRequestPaginateTypeDef(TypedDict):
    ListBy: NotRequired[QueueListByType],  # (1)
    Order: NotRequired[OrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: QueueListByType](./literals.md#queuelistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVersionsRequestPaginateTypeDef

```python
# ListVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListVersionsRequestPaginateTypeDef


def get_value() -> ListVersionsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListVersionsRequestPaginateTypeDef definition

class ListVersionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchJobsRequestPaginateTypeDef

```python
# SearchJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import SearchJobsRequestPaginateTypeDef


def get_value() -> SearchJobsRequestPaginateTypeDef:
    return {
        "InputFile": ...,
    }


# SearchJobsRequestPaginateTypeDef definition

class SearchJobsRequestPaginateTypeDef(TypedDict):
    InputFile: NotRequired[str],
    Order: NotRequired[OrderType],  # (1)
    Queue: NotRequired[str],
    Status: NotRequired[JobStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEndpointsResponseTypeDef

```python
# DescribeEndpointsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DescribeEndpointsResponseTypeDef


def get_value() -> DescribeEndpointsResponseTypeDef:
    return {
        "Endpoints": ...,
    }


# DescribeEndpointsResponseTypeDef definition

class DescribeEndpointsResponseTypeDef(TypedDict):
    Endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DolbyVisionTypeDef

```python
# DolbyVisionTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DolbyVisionTypeDef


def get_value() -> DolbyVisionTypeDef:
    return {
        "L6Metadata": ...,
    }


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
## SpekeKeyProviderCmafOutputTypeDef

```python
# SpekeKeyProviderCmafOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import SpekeKeyProviderCmafOutputTypeDef


def get_value() -> SpekeKeyProviderCmafOutputTypeDef:
    return {
        "CertificateArn": ...,
    }


# SpekeKeyProviderCmafOutputTypeDef definition

class SpekeKeyProviderCmafOutputTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    DashSignaledSystemIds: NotRequired[List[str]],
    EncryptionContractConfiguration: NotRequired[EncryptionContractConfigurationTypeDef],  # (1)
    HlsSignaledSystemIds: NotRequired[List[str]],
    ResourceId: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-braces: EncryptionContractConfigurationTypeDef](./type_defs.md#encryptioncontractconfigurationtypedef) 
## SpekeKeyProviderCmafTypeDef

```python
# SpekeKeyProviderCmafTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import SpekeKeyProviderCmafTypeDef


def get_value() -> SpekeKeyProviderCmafTypeDef:
    return {
        "CertificateArn": ...,
    }


# SpekeKeyProviderCmafTypeDef definition

class SpekeKeyProviderCmafTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    DashSignaledSystemIds: NotRequired[Sequence[str]],
    EncryptionContractConfiguration: NotRequired[EncryptionContractConfigurationTypeDef],  # (1)
    HlsSignaledSystemIds: NotRequired[Sequence[str]],
    ResourceId: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-braces: EncryptionContractConfigurationTypeDef](./type_defs.md#encryptioncontractconfigurationtypedef) 
## SpekeKeyProviderOutputTypeDef

```python
# SpekeKeyProviderOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import SpekeKeyProviderOutputTypeDef


def get_value() -> SpekeKeyProviderOutputTypeDef:
    return {
        "CertificateArn": ...,
    }


# SpekeKeyProviderOutputTypeDef definition

class SpekeKeyProviderOutputTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    EncryptionContractConfiguration: NotRequired[EncryptionContractConfigurationTypeDef],  # (1)
    ResourceId: NotRequired[str],
    SystemIds: NotRequired[List[str]],
    Url: NotRequired[str],
```

1. See [:material-code-braces: EncryptionContractConfigurationTypeDef](./type_defs.md#encryptioncontractconfigurationtypedef) 
## SpekeKeyProviderTypeDef

```python
# SpekeKeyProviderTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import SpekeKeyProviderTypeDef


def get_value() -> SpekeKeyProviderTypeDef:
    return {
        "CertificateArn": ...,
    }


# SpekeKeyProviderTypeDef definition

class SpekeKeyProviderTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    EncryptionContractConfiguration: NotRequired[EncryptionContractConfigurationTypeDef],  # (1)
    ResourceId: NotRequired[str],
    SystemIds: NotRequired[Sequence[str]],
    Url: NotRequired[str],
```

1. See [:material-code-braces: EncryptionContractConfigurationTypeDef](./type_defs.md#encryptioncontractconfigurationtypedef) 
## EsamSettingsTypeDef

```python
# EsamSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import EsamSettingsTypeDef


def get_value() -> EsamSettingsTypeDef:
    return {
        "ManifestConfirmConditionNotification": ...,
    }


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
# GetPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import GetPolicyResponseTypeDef


def get_value() -> GetPolicyResponseTypeDef:
    return {
        "Policy": ...,
    }


# GetPolicyResponseTypeDef definition

class GetPolicyResponseTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutPolicyRequestTypeDef

```python
# PutPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import PutPolicyRequestTypeDef


def get_value() -> PutPolicyRequestTypeDef:
    return {
        "Policy": ...,
    }


# PutPolicyRequestTypeDef definition

class PutPolicyRequestTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
## PutPolicyResponseTypeDef

```python
# PutPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import PutPolicyResponseTypeDef


def get_value() -> PutPolicyResponseTypeDef:
    return {
        "Policy": ...,
    }


# PutPolicyResponseTypeDef definition

class PutPolicyResponseTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## H264SettingsTypeDef

```python
# H264SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import H264SettingsTypeDef


def get_value() -> H264SettingsTypeDef:
    return {
        "AdaptiveQuantization": ...,
    }


# H264SettingsTypeDef definition

class H264SettingsTypeDef(TypedDict):
    AdaptiveQuantization: NotRequired[H264AdaptiveQuantizationType],  # (1)
    BandwidthReductionFilter: NotRequired[BandwidthReductionFilterTypeDef],  # (2)
    Bitrate: NotRequired[int],
    CodecLevel: NotRequired[H264CodecLevelType],  # (3)
    CodecProfile: NotRequired[H264CodecProfileType],  # (4)
    DynamicSubGop: NotRequired[H264DynamicSubGopType],  # (5)
    EndOfStreamMarkers: NotRequired[H264EndOfStreamMarkersType],  # (6)
    EntropyEncoding: NotRequired[H264EntropyEncodingType],  # (7)
    FieldEncoding: NotRequired[H264FieldEncodingType],  # (8)
    FlickerAdaptiveQuantization: NotRequired[H264FlickerAdaptiveQuantizationType],  # (9)
    FramerateControl: NotRequired[H264FramerateControlType],  # (10)
    FramerateConversionAlgorithm: NotRequired[H264FramerateConversionAlgorithmType],  # (11)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    GopBReference: NotRequired[H264GopBReferenceType],  # (12)
    GopClosedCadence: NotRequired[int],
    GopSize: NotRequired[float],
    GopSizeUnits: NotRequired[H264GopSizeUnitsType],  # (13)
    HrdBufferFinalFillPercentage: NotRequired[int],
    HrdBufferInitialFillPercentage: NotRequired[int],
    HrdBufferSize: NotRequired[int],
    InterlaceMode: NotRequired[H264InterlaceModeType],  # (14)
    MaxBitrate: NotRequired[int],
    MinIInterval: NotRequired[int],
    NumberBFramesBetweenReferenceFrames: NotRequired[int],
    NumberReferenceFrames: NotRequired[int],
    ParControl: NotRequired[H264ParControlType],  # (15)
    ParDenominator: NotRequired[int],
    ParNumerator: NotRequired[int],
    QualityTuningLevel: NotRequired[H264QualityTuningLevelType],  # (16)
    QvbrSettings: NotRequired[H264QvbrSettingsTypeDef],  # (17)
    RateControlMode: NotRequired[H264RateControlModeType],  # (18)
    RepeatPps: NotRequired[H264RepeatPpsType],  # (19)
    SaliencyAwareEncoding: NotRequired[H264SaliencyAwareEncodingType],  # (20)
    ScanTypeConversionMode: NotRequired[H264ScanTypeConversionModeType],  # (21)
    SceneChangeDetect: NotRequired[H264SceneChangeDetectType],  # (22)
    Slices: NotRequired[int],
    SlowPal: NotRequired[H264SlowPalType],  # (23)
    Softness: NotRequired[int],
    SpatialAdaptiveQuantization: NotRequired[H264SpatialAdaptiveQuantizationType],  # (24)
    Syntax: NotRequired[H264SyntaxType],  # (25)
    Telecine: NotRequired[H264TelecineType],  # (26)
    TemporalAdaptiveQuantization: NotRequired[H264TemporalAdaptiveQuantizationType],  # (27)
    UnregisteredSeiTimecode: NotRequired[H264UnregisteredSeiTimecodeType],  # (28)
    WriteMp4PackagingType: NotRequired[H264WriteMp4PackagingTypeType],  # (29)
```

1. See [:material-code-brackets: H264AdaptiveQuantizationType](./literals.md#h264adaptivequantizationtype) 
2. See [:material-code-braces: BandwidthReductionFilterTypeDef](./type_defs.md#bandwidthreductionfiltertypedef) 
3. See [:material-code-brackets: H264CodecLevelType](./literals.md#h264codecleveltype) 
4. See [:material-code-brackets: H264CodecProfileType](./literals.md#h264codecprofiletype) 
5. See [:material-code-brackets: H264DynamicSubGopType](./literals.md#h264dynamicsubgoptype) 
6. See [:material-code-brackets: H264EndOfStreamMarkersType](./literals.md#h264endofstreammarkerstype) 
7. See [:material-code-brackets: H264EntropyEncodingType](./literals.md#h264entropyencodingtype) 
8. See [:material-code-brackets: H264FieldEncodingType](./literals.md#h264fieldencodingtype) 
9. See [:material-code-brackets: H264FlickerAdaptiveQuantizationType](./literals.md#h264flickeradaptivequantizationtype) 
10. See [:material-code-brackets: H264FramerateControlType](./literals.md#h264frameratecontroltype) 
11. See [:material-code-brackets: H264FramerateConversionAlgorithmType](./literals.md#h264framerateconversionalgorithmtype) 
12. See [:material-code-brackets: H264GopBReferenceType](./literals.md#h264gopbreferencetype) 
13. See [:material-code-brackets: H264GopSizeUnitsType](./literals.md#h264gopsizeunitstype) 
14. See [:material-code-brackets: H264InterlaceModeType](./literals.md#h264interlacemodetype) 
15. See [:material-code-brackets: H264ParControlType](./literals.md#h264parcontroltype) 
16. See [:material-code-brackets: H264QualityTuningLevelType](./literals.md#h264qualitytuningleveltype) 
17. See [:material-code-braces: H264QvbrSettingsTypeDef](./type_defs.md#h264qvbrsettingstypedef) 
18. See [:material-code-brackets: H264RateControlModeType](./literals.md#h264ratecontrolmodetype) 
19. See [:material-code-brackets: H264RepeatPpsType](./literals.md#h264repeatppstype) 
20. See [:material-code-brackets: H264SaliencyAwareEncodingType](./literals.md#h264saliencyawareencodingtype) 
21. See [:material-code-brackets: H264ScanTypeConversionModeType](./literals.md#h264scantypeconversionmodetype) 
22. See [:material-code-brackets: H264SceneChangeDetectType](./literals.md#h264scenechangedetecttype) 
23. See [:material-code-brackets: H264SlowPalType](./literals.md#h264slowpaltype) 
24. See [:material-code-brackets: H264SpatialAdaptiveQuantizationType](./literals.md#h264spatialadaptivequantizationtype) 
25. See [:material-code-brackets: H264SyntaxType](./literals.md#h264syntaxtype) 
26. See [:material-code-brackets: H264TelecineType](./literals.md#h264telecinetype) 
27. See [:material-code-brackets: H264TemporalAdaptiveQuantizationType](./literals.md#h264temporaladaptivequantizationtype) 
28. See [:material-code-brackets: H264UnregisteredSeiTimecodeType](./literals.md#h264unregisteredseitimecodetype) 
29. See [:material-code-brackets: H264WriteMp4PackagingTypeType](./literals.md#h264writemp4packagingtypetype) 
## H265SettingsTypeDef

```python
# H265SettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import H265SettingsTypeDef


def get_value() -> H265SettingsTypeDef:
    return {
        "AdaptiveQuantization": ...,
    }


# H265SettingsTypeDef definition

class H265SettingsTypeDef(TypedDict):
    AdaptiveQuantization: NotRequired[H265AdaptiveQuantizationType],  # (1)
    AlternateTransferFunctionSei: NotRequired[H265AlternateTransferFunctionSeiType],  # (2)
    BandwidthReductionFilter: NotRequired[BandwidthReductionFilterTypeDef],  # (3)
    Bitrate: NotRequired[int],
    CodecLevel: NotRequired[H265CodecLevelType],  # (4)
    CodecProfile: NotRequired[H265CodecProfileType],  # (5)
    Deblocking: NotRequired[H265DeblockingType],  # (6)
    DynamicSubGop: NotRequired[H265DynamicSubGopType],  # (7)
    EndOfStreamMarkers: NotRequired[H265EndOfStreamMarkersType],  # (8)
    FlickerAdaptiveQuantization: NotRequired[H265FlickerAdaptiveQuantizationType],  # (9)
    FramerateControl: NotRequired[H265FramerateControlType],  # (10)
    FramerateConversionAlgorithm: NotRequired[H265FramerateConversionAlgorithmType],  # (11)
    FramerateDenominator: NotRequired[int],
    FramerateNumerator: NotRequired[int],
    GopBReference: NotRequired[H265GopBReferenceType],  # (12)
    GopClosedCadence: NotRequired[int],
    GopSize: NotRequired[float],
    GopSizeUnits: NotRequired[H265GopSizeUnitsType],  # (13)
    HrdBufferFinalFillPercentage: NotRequired[int],
    HrdBufferInitialFillPercentage: NotRequired[int],
    HrdBufferSize: NotRequired[int],
    InterlaceMode: NotRequired[H265InterlaceModeType],  # (14)
    MaxBitrate: NotRequired[int],
    MinIInterval: NotRequired[int],
    NumberBFramesBetweenReferenceFrames: NotRequired[int],
    NumberReferenceFrames: NotRequired[int],
    ParControl: NotRequired[H265ParControlType],  # (15)
    ParDenominator: NotRequired[int],
    ParNumerator: NotRequired[int],
    QualityTuningLevel: NotRequired[H265QualityTuningLevelType],  # (16)
    QvbrSettings: NotRequired[H265QvbrSettingsTypeDef],  # (17)
    RateControlMode: NotRequired[H265RateControlModeType],  # (18)
    SampleAdaptiveOffsetFilterMode: NotRequired[H265SampleAdaptiveOffsetFilterModeType],  # (19)
    ScanTypeConversionMode: NotRequired[H265ScanTypeConversionModeType],  # (20)
    SceneChangeDetect: NotRequired[H265SceneChangeDetectType],  # (21)
    Slices: NotRequired[int],
    SlowPal: NotRequired[H265SlowPalType],  # (22)
    SpatialAdaptiveQuantization: NotRequired[H265SpatialAdaptiveQuantizationType],  # (23)
    Telecine: NotRequired[H265TelecineType],  # (24)
    TemporalAdaptiveQuantization: NotRequired[H265TemporalAdaptiveQuantizationType],  # (25)
    TemporalIds: NotRequired[H265TemporalIdsType],  # (26)
    Tiles: NotRequired[H265TilesType],  # (27)
    UnregisteredSeiTimecode: NotRequired[H265UnregisteredSeiTimecodeType],  # (28)
    WriteMp4PackagingType: NotRequired[H265WriteMp4PackagingTypeType],  # (29)
```

1. See [:material-code-brackets: H265AdaptiveQuantizationType](./literals.md#h265adaptivequantizationtype) 
2. See [:material-code-brackets: H265AlternateTransferFunctionSeiType](./literals.md#h265alternatetransferfunctionseitype) 
3. See [:material-code-braces: BandwidthReductionFilterTypeDef](./type_defs.md#bandwidthreductionfiltertypedef) 
4. See [:material-code-brackets: H265CodecLevelType](./literals.md#h265codecleveltype) 
5. See [:material-code-brackets: H265CodecProfileType](./literals.md#h265codecprofiletype) 
6. See [:material-code-brackets: H265DeblockingType](./literals.md#h265deblockingtype) 
7. See [:material-code-brackets: H265DynamicSubGopType](./literals.md#h265dynamicsubgoptype) 
8. See [:material-code-brackets: H265EndOfStreamMarkersType](./literals.md#h265endofstreammarkerstype) 
9. See [:material-code-brackets: H265FlickerAdaptiveQuantizationType](./literals.md#h265flickeradaptivequantizationtype) 
10. See [:material-code-brackets: H265FramerateControlType](./literals.md#h265frameratecontroltype) 
11. See [:material-code-brackets: H265FramerateConversionAlgorithmType](./literals.md#h265framerateconversionalgorithmtype) 
12. See [:material-code-brackets: H265GopBReferenceType](./literals.md#h265gopbreferencetype) 
13. See [:material-code-brackets: H265GopSizeUnitsType](./literals.md#h265gopsizeunitstype) 
14. See [:material-code-brackets: H265InterlaceModeType](./literals.md#h265interlacemodetype) 
15. See [:material-code-brackets: H265ParControlType](./literals.md#h265parcontroltype) 
16. See [:material-code-brackets: H265QualityTuningLevelType](./literals.md#h265qualitytuningleveltype) 
17. See [:material-code-braces: H265QvbrSettingsTypeDef](./type_defs.md#h265qvbrsettingstypedef) 
18. See [:material-code-brackets: H265RateControlModeType](./literals.md#h265ratecontrolmodetype) 
19. See [:material-code-brackets: H265SampleAdaptiveOffsetFilterModeType](./literals.md#h265sampleadaptiveoffsetfiltermodetype) 
20. See [:material-code-brackets: H265ScanTypeConversionModeType](./literals.md#h265scantypeconversionmodetype) 
21. See [:material-code-brackets: H265SceneChangeDetectType](./literals.md#h265scenechangedetecttype) 
22. See [:material-code-brackets: H265SlowPalType](./literals.md#h265slowpaltype) 
23. See [:material-code-brackets: H265SpatialAdaptiveQuantizationType](./literals.md#h265spatialadaptivequantizationtype) 
24. See [:material-code-brackets: H265TelecineType](./literals.md#h265telecinetype) 
25. See [:material-code-brackets: H265TemporalAdaptiveQuantizationType](./literals.md#h265temporaladaptivequantizationtype) 
26. See [:material-code-brackets: H265TemporalIdsType](./literals.md#h265temporalidstype) 
27. See [:material-code-brackets: H265TilesType](./literals.md#h265tilestype) 
28. See [:material-code-brackets: H265UnregisteredSeiTimecodeType](./literals.md#h265unregisteredseitimecodetype) 
29. See [:material-code-brackets: H265WriteMp4PackagingTypeType](./literals.md#h265writemp4packagingtypetype) 
## OutputSettingsTypeDef

```python
# OutputSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import OutputSettingsTypeDef


def get_value() -> OutputSettingsTypeDef:
    return {
        "HlsSettings": ...,
    }


# OutputSettingsTypeDef definition

class OutputSettingsTypeDef(TypedDict):
    HlsSettings: NotRequired[HlsSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: HlsSettingsTypeDef](./type_defs.md#hlssettingstypedef) 
## TimedMetadataInsertionOutputTypeDef

```python
# TimedMetadataInsertionOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import TimedMetadataInsertionOutputTypeDef


def get_value() -> TimedMetadataInsertionOutputTypeDef:
    return {
        "Id3Insertions": ...,
    }


# TimedMetadataInsertionOutputTypeDef definition

class TimedMetadataInsertionOutputTypeDef(TypedDict):
    Id3Insertions: NotRequired[List[Id3InsertionTypeDef]],  # (1)
```

1. See [:material-code-braces: Id3InsertionTypeDef](./type_defs.md#id3insertiontypedef) 
## TimedMetadataInsertionTypeDef

```python
# TimedMetadataInsertionTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import TimedMetadataInsertionTypeDef


def get_value() -> TimedMetadataInsertionTypeDef:
    return {
        "Id3Insertions": ...,
    }


# TimedMetadataInsertionTypeDef definition

class TimedMetadataInsertionTypeDef(TypedDict):
    Id3Insertions: NotRequired[Sequence[Id3InsertionTypeDef]],  # (1)
```

1. See [:material-code-braces: Id3InsertionTypeDef](./type_defs.md#id3insertiontypedef) 
## ImageInserterOutputTypeDef

```python
# ImageInserterOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ImageInserterOutputTypeDef


def get_value() -> ImageInserterOutputTypeDef:
    return {
        "InsertableImages": ...,
    }


# ImageInserterOutputTypeDef definition

class ImageInserterOutputTypeDef(TypedDict):
    InsertableImages: NotRequired[List[InsertableImageTypeDef]],  # (1)
    SdrReferenceWhiteLevel: NotRequired[int],
```

1. See [:material-code-braces: InsertableImageTypeDef](./type_defs.md#insertableimagetypedef) 
## ImageInserterTypeDef

```python
# ImageInserterTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ImageInserterTypeDef


def get_value() -> ImageInserterTypeDef:
    return {
        "InsertableImages": ...,
    }


# ImageInserterTypeDef definition

class ImageInserterTypeDef(TypedDict):
    InsertableImages: NotRequired[Sequence[InsertableImageTypeDef]],  # (1)
    SdrReferenceWhiteLevel: NotRequired[int],
```

1. See [:material-code-braces: InsertableImageTypeDef](./type_defs.md#insertableimagetypedef) 
## ListVersionsResponseTypeDef

```python
# ListVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListVersionsResponseTypeDef


def get_value() -> ListVersionsResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListVersionsResponseTypeDef definition

class ListVersionsResponseTypeDef(TypedDict):
    Versions: List[JobEngineVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JobEngineVersionTypeDef](./type_defs.md#jobengineversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "ResourceTags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    ResourceTags: ResourceTagsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagsTypeDef](./type_defs.md#resourcetagstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## M2tsSettingsOutputTypeDef

```python
# M2tsSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import M2tsSettingsOutputTypeDef


def get_value() -> M2tsSettingsOutputTypeDef:
    return {
        "AudioBufferModel": ...,
    }


# M2tsSettingsOutputTypeDef definition

class M2tsSettingsOutputTypeDef(TypedDict):
    AudioBufferModel: NotRequired[M2tsAudioBufferModelType],  # (1)
    AudioDuration: NotRequired[M2tsAudioDurationType],  # (2)
    AudioFramesPerPes: NotRequired[int],
    AudioPids: NotRequired[List[int]],
    Bitrate: NotRequired[int],
    BufferModel: NotRequired[M2tsBufferModelType],  # (3)
    DataPTSControl: NotRequired[M2tsDataPtsControlType],  # (4)
    DvbNitSettings: NotRequired[DvbNitSettingsTypeDef],  # (5)
    DvbSdtSettings: NotRequired[DvbSdtSettingsTypeDef],  # (6)
    DvbSubPids: NotRequired[List[int]],
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
    PreventBufferUnderflow: NotRequired[M2tsPreventBufferUnderflowType],  # (15)
    PrivateMetadataPid: NotRequired[int],
    ProgramNumber: NotRequired[int],
    PtsOffset: NotRequired[int],
    PtsOffsetMode: NotRequired[TsPtsOffsetType],  # (16)
    RateMode: NotRequired[M2tsRateModeType],  # (17)
    Scte35Esam: NotRequired[M2tsScte35EsamTypeDef],  # (18)
    Scte35Pid: NotRequired[int],
    Scte35Source: NotRequired[M2tsScte35SourceType],  # (19)
    SegmentationMarkers: NotRequired[M2tsSegmentationMarkersType],  # (20)
    SegmentationStyle: NotRequired[M2tsSegmentationStyleType],  # (21)
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
15. See [:material-code-brackets: M2tsPreventBufferUnderflowType](./literals.md#m2tspreventbufferunderflowtype) 
16. See [:material-code-brackets: TsPtsOffsetType](./literals.md#tsptsoffsettype) 
17. See [:material-code-brackets: M2tsRateModeType](./literals.md#m2tsratemodetype) 
18. See [:material-code-braces: M2tsScte35EsamTypeDef](./type_defs.md#m2tsscte35esamtypedef) 
19. See [:material-code-brackets: M2tsScte35SourceType](./literals.md#m2tsscte35sourcetype) 
20. See [:material-code-brackets: M2tsSegmentationMarkersType](./literals.md#m2tssegmentationmarkerstype) 
21. See [:material-code-brackets: M2tsSegmentationStyleType](./literals.md#m2tssegmentationstyletype) 
## M2tsSettingsTypeDef

```python
# M2tsSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import M2tsSettingsTypeDef


def get_value() -> M2tsSettingsTypeDef:
    return {
        "AudioBufferModel": ...,
    }


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
    PreventBufferUnderflow: NotRequired[M2tsPreventBufferUnderflowType],  # (15)
    PrivateMetadataPid: NotRequired[int],
    ProgramNumber: NotRequired[int],
    PtsOffset: NotRequired[int],
    PtsOffsetMode: NotRequired[TsPtsOffsetType],  # (16)
    RateMode: NotRequired[M2tsRateModeType],  # (17)
    Scte35Esam: NotRequired[M2tsScte35EsamTypeDef],  # (18)
    Scte35Pid: NotRequired[int],
    Scte35Source: NotRequired[M2tsScte35SourceType],  # (19)
    SegmentationMarkers: NotRequired[M2tsSegmentationMarkersType],  # (20)
    SegmentationStyle: NotRequired[M2tsSegmentationStyleType],  # (21)
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
15. See [:material-code-brackets: M2tsPreventBufferUnderflowType](./literals.md#m2tspreventbufferunderflowtype) 
16. See [:material-code-brackets: TsPtsOffsetType](./literals.md#tsptsoffsettype) 
17. See [:material-code-brackets: M2tsRateModeType](./literals.md#m2tsratemodetype) 
18. See [:material-code-braces: M2tsScte35EsamTypeDef](./type_defs.md#m2tsscte35esamtypedef) 
19. See [:material-code-brackets: M2tsScte35SourceType](./literals.md#m2tsscte35sourcetype) 
20. See [:material-code-brackets: M2tsSegmentationMarkersType](./literals.md#m2tssegmentationmarkerstype) 
21. See [:material-code-brackets: M2tsSegmentationStyleType](./literals.md#m2tssegmentationstyletype) 
## MotionImageInserterTypeDef

```python
# MotionImageInserterTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MotionImageInserterTypeDef


def get_value() -> MotionImageInserterTypeDef:
    return {
        "Framerate": ...,
    }


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
# MxfSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MxfSettingsTypeDef


def get_value() -> MxfSettingsTypeDef:
    return {
        "AfdSignaling": ...,
    }


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
# PartnerWatermarkingTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import PartnerWatermarkingTypeDef


def get_value() -> PartnerWatermarkingTypeDef:
    return {
        "NexguardFileMarkerSettings": ...,
    }


# PartnerWatermarkingTypeDef definition

class PartnerWatermarkingTypeDef(TypedDict):
    NexguardFileMarkerSettings: NotRequired[NexGuardFileMarkerSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: NexGuardFileMarkerSettingsTypeDef](./type_defs.md#nexguardfilemarkersettingstypedef) 
## NoiseReducerTypeDef

```python
# NoiseReducerTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import NoiseReducerTypeDef


def get_value() -> NoiseReducerTypeDef:
    return {
        "Filter": ...,
    }


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
# OutputDetailTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import OutputDetailTypeDef


def get_value() -> OutputDetailTypeDef:
    return {
        "DurationInMs": ...,
    }


# OutputDetailTypeDef definition

class OutputDetailTypeDef(TypedDict):
    DurationInMs: NotRequired[int],
    VideoDetails: NotRequired[VideoDetailTypeDef],  # (1)
```

1. See [:material-code-braces: VideoDetailTypeDef](./type_defs.md#videodetailtypedef) 
## QueueTypeDef

```python
# QueueTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import QueueTypeDef


def get_value() -> QueueTypeDef:
    return {
        "Arn": ...,
    }


# QueueTypeDef definition

class QueueTypeDef(TypedDict):
    Name: str,
    Arn: NotRequired[str],
    ConcurrentJobs: NotRequired[int],
    CreatedAt: NotRequired[datetime],
    Description: NotRequired[str],
    LastUpdated: NotRequired[datetime],
    PricingPlan: NotRequired[PricingPlanType],  # (1)
    ProgressingJobsCount: NotRequired[int],
    ReservationPlan: NotRequired[ReservationPlanTypeDef],  # (2)
    ServiceOverrides: NotRequired[List[ServiceOverrideTypeDef]],  # (3)
    Status: NotRequired[QueueStatusType],  # (4)
    SubmittedJobsCount: NotRequired[int],
    Type: NotRequired[TypeType],  # (5)
```

1. See [:material-code-brackets: PricingPlanType](./literals.md#pricingplantype) 
2. See [:material-code-braces: ReservationPlanTypeDef](./type_defs.md#reservationplantypedef) 
3. See [:material-code-braces: ServiceOverrideTypeDef](./type_defs.md#serviceoverridetypedef) 
4. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
5. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## S3DestinationSettingsTypeDef

```python
# S3DestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import S3DestinationSettingsTypeDef


def get_value() -> S3DestinationSettingsTypeDef:
    return {
        "AccessControl": ...,
    }


# S3DestinationSettingsTypeDef definition

class S3DestinationSettingsTypeDef(TypedDict):
    AccessControl: NotRequired[S3DestinationAccessControlTypeDef],  # (1)
    Encryption: NotRequired[S3EncryptionSettingsTypeDef],  # (2)
    StorageClass: NotRequired[S3StorageClassType],  # (3)
```

1. See [:material-code-braces: S3DestinationAccessControlTypeDef](./type_defs.md#s3destinationaccesscontroltypedef) 
2. See [:material-code-braces: S3EncryptionSettingsTypeDef](./type_defs.md#s3encryptionsettingstypedef) 
3. See [:material-code-brackets: S3StorageClassType](./literals.md#s3storageclasstype) 
## VideoOverlayInputOutputTypeDef

```python
# VideoOverlayInputOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoOverlayInputOutputTypeDef


def get_value() -> VideoOverlayInputOutputTypeDef:
    return {
        "FileInput": ...,
    }


# VideoOverlayInputOutputTypeDef definition

class VideoOverlayInputOutputTypeDef(TypedDict):
    FileInput: NotRequired[str],
    InputClippings: NotRequired[List[VideoOverlayInputClippingTypeDef]],  # (1)
    TimecodeSource: NotRequired[InputTimecodeSourceType],  # (2)
    TimecodeStart: NotRequired[str],
```

1. See [:material-code-braces: VideoOverlayInputClippingTypeDef](./type_defs.md#videooverlayinputclippingtypedef) 
2. See [:material-code-brackets: InputTimecodeSourceType](./literals.md#inputtimecodesourcetype) 
## VideoOverlayInputTypeDef

```python
# VideoOverlayInputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoOverlayInputTypeDef


def get_value() -> VideoOverlayInputTypeDef:
    return {
        "FileInput": ...,
    }


# VideoOverlayInputTypeDef definition

class VideoOverlayInputTypeDef(TypedDict):
    FileInput: NotRequired[str],
    InputClippings: NotRequired[Sequence[VideoOverlayInputClippingTypeDef]],  # (1)
    TimecodeSource: NotRequired[InputTimecodeSourceType],  # (2)
    TimecodeStart: NotRequired[str],
```

1. See [:material-code-braces: VideoOverlayInputClippingTypeDef](./type_defs.md#videooverlayinputclippingtypedef) 
2. See [:material-code-brackets: InputTimecodeSourceType](./literals.md#inputtimecodesourcetype) 
## VideoOverlayTransitionTypeDef

```python
# VideoOverlayTransitionTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoOverlayTransitionTypeDef


def get_value() -> VideoOverlayTransitionTypeDef:
    return {
        "EndPosition": ...,
    }


# VideoOverlayTransitionTypeDef definition

class VideoOverlayTransitionTypeDef(TypedDict):
    EndPosition: NotRequired[VideoOverlayPositionTypeDef],  # (1)
    EndTimecode: NotRequired[str],
    StartTimecode: NotRequired[str],
```

1. See [:material-code-braces: VideoOverlayPositionTypeDef](./type_defs.md#videooverlaypositiontypedef) 
## XavcSettingsTypeDef

```python
# XavcSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import XavcSettingsTypeDef


def get_value() -> XavcSettingsTypeDef:
    return {
        "AdaptiveQuantization": ...,
    }


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
## AutomatedAbrSettingsOutputTypeDef

```python
# AutomatedAbrSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AutomatedAbrSettingsOutputTypeDef


def get_value() -> AutomatedAbrSettingsOutputTypeDef:
    return {
        "MaxAbrBitrate": ...,
    }


# AutomatedAbrSettingsOutputTypeDef definition

class AutomatedAbrSettingsOutputTypeDef(TypedDict):
    MaxAbrBitrate: NotRequired[int],
    MaxRenditions: NotRequired[int],
    MinAbrBitrate: NotRequired[int],
    Rules: NotRequired[List[AutomatedAbrRuleOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: AutomatedAbrRuleOutputTypeDef](./type_defs.md#automatedabrruleoutputtypedef) 
## AutomatedAbrSettingsTypeDef

```python
# AutomatedAbrSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AutomatedAbrSettingsTypeDef


def get_value() -> AutomatedAbrSettingsTypeDef:
    return {
        "MaxAbrBitrate": ...,
    }


# AutomatedAbrSettingsTypeDef definition

class AutomatedAbrSettingsTypeDef(TypedDict):
    MaxAbrBitrate: NotRequired[int],
    MaxRenditions: NotRequired[int],
    MinAbrBitrate: NotRequired[int],
    Rules: NotRequired[Sequence[AutomatedAbrRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: AutomatedAbrRuleTypeDef](./type_defs.md#automatedabrruletypedef) 
## CaptionDescriptionOutputTypeDef

```python
# CaptionDescriptionOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CaptionDescriptionOutputTypeDef


def get_value() -> CaptionDescriptionOutputTypeDef:
    return {
        "CaptionSelectorName": ...,
    }


# CaptionDescriptionOutputTypeDef definition

class CaptionDescriptionOutputTypeDef(TypedDict):
    CaptionSelectorName: NotRequired[str],
    CustomLanguageCode: NotRequired[str],
    DestinationSettings: NotRequired[CaptionDestinationSettingsOutputTypeDef],  # (1)
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    LanguageDescription: NotRequired[str],
```

1. See [:material-code-braces: CaptionDestinationSettingsOutputTypeDef](./type_defs.md#captiondestinationsettingsoutputtypedef) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## CaptionDescriptionPresetOutputTypeDef

```python
# CaptionDescriptionPresetOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CaptionDescriptionPresetOutputTypeDef


def get_value() -> CaptionDescriptionPresetOutputTypeDef:
    return {
        "CustomLanguageCode": ...,
    }


# CaptionDescriptionPresetOutputTypeDef definition

class CaptionDescriptionPresetOutputTypeDef(TypedDict):
    CustomLanguageCode: NotRequired[str],
    DestinationSettings: NotRequired[CaptionDestinationSettingsOutputTypeDef],  # (1)
    LanguageCode: NotRequired[LanguageCodeType],  # (2)
    LanguageDescription: NotRequired[str],
```

1. See [:material-code-braces: CaptionDestinationSettingsOutputTypeDef](./type_defs.md#captiondestinationsettingsoutputtypedef) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
## CaptionDescriptionPresetTypeDef

```python
# CaptionDescriptionPresetTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CaptionDescriptionPresetTypeDef


def get_value() -> CaptionDescriptionPresetTypeDef:
    return {
        "CustomLanguageCode": ...,
    }


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
# CaptionDescriptionTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CaptionDescriptionTypeDef


def get_value() -> CaptionDescriptionTypeDef:
    return {
        "CaptionSelectorName": ...,
    }


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
# CaptionSourceSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CaptionSourceSettingsTypeDef


def get_value() -> CaptionSourceSettingsTypeDef:
    return {
        "AncillarySourceSettings": ...,
    }


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
## RemixSettingsOutputTypeDef

```python
# RemixSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import RemixSettingsOutputTypeDef


def get_value() -> RemixSettingsOutputTypeDef:
    return {
        "AudioDescriptionAudioChannel": ...,
    }


# RemixSettingsOutputTypeDef definition

class RemixSettingsOutputTypeDef(TypedDict):
    AudioDescriptionAudioChannel: NotRequired[int],
    AudioDescriptionDataChannel: NotRequired[int],
    ChannelMapping: NotRequired[ChannelMappingOutputTypeDef],  # (1)
    ChannelsIn: NotRequired[int],
    ChannelsOut: NotRequired[int],
```

1. See [:material-code-braces: ChannelMappingOutputTypeDef](./type_defs.md#channelmappingoutputtypedef) 
## RemixSettingsTypeDef

```python
# RemixSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import RemixSettingsTypeDef


def get_value() -> RemixSettingsTypeDef:
    return {
        "AudioDescriptionAudioChannel": ...,
    }


# RemixSettingsTypeDef definition

class RemixSettingsTypeDef(TypedDict):
    AudioDescriptionAudioChannel: NotRequired[int],
    AudioDescriptionDataChannel: NotRequired[int],
    ChannelMapping: NotRequired[ChannelMappingTypeDef],  # (1)
    ChannelsIn: NotRequired[int],
    ChannelsOut: NotRequired[int],
```

1. See [:material-code-braces: ChannelMappingTypeDef](./type_defs.md#channelmappingtypedef) 
## CmafEncryptionSettingsOutputTypeDef

```python
# CmafEncryptionSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CmafEncryptionSettingsOutputTypeDef


def get_value() -> CmafEncryptionSettingsOutputTypeDef:
    return {
        "ConstantInitializationVector": ...,
    }


# CmafEncryptionSettingsOutputTypeDef definition

class CmafEncryptionSettingsOutputTypeDef(TypedDict):
    ConstantInitializationVector: NotRequired[str],
    EncryptionMethod: NotRequired[CmafEncryptionTypeType],  # (1)
    InitializationVectorInManifest: NotRequired[CmafInitializationVectorInManifestType],  # (2)
    SpekeKeyProvider: NotRequired[SpekeKeyProviderCmafOutputTypeDef],  # (3)
    StaticKeyProvider: NotRequired[StaticKeyProviderTypeDef],  # (4)
    Type: NotRequired[CmafKeyProviderTypeType],  # (5)
```

1. See [:material-code-brackets: CmafEncryptionTypeType](./literals.md#cmafencryptiontypetype) 
2. See [:material-code-brackets: CmafInitializationVectorInManifestType](./literals.md#cmafinitializationvectorinmanifesttype) 
3. See [:material-code-braces: SpekeKeyProviderCmafOutputTypeDef](./type_defs.md#spekekeyprovidercmafoutputtypedef) 
4. See [:material-code-braces: StaticKeyProviderTypeDef](./type_defs.md#statickeyprovidertypedef) 
5. See [:material-code-brackets: CmafKeyProviderTypeType](./literals.md#cmafkeyprovidertypetype) 
## CmafEncryptionSettingsTypeDef

```python
# CmafEncryptionSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CmafEncryptionSettingsTypeDef


def get_value() -> CmafEncryptionSettingsTypeDef:
    return {
        "ConstantInitializationVector": ...,
    }


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
## DashIsoEncryptionSettingsOutputTypeDef

```python
# DashIsoEncryptionSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DashIsoEncryptionSettingsOutputTypeDef


def get_value() -> DashIsoEncryptionSettingsOutputTypeDef:
    return {
        "PlaybackDeviceCompatibility": ...,
    }


# DashIsoEncryptionSettingsOutputTypeDef definition

class DashIsoEncryptionSettingsOutputTypeDef(TypedDict):
    PlaybackDeviceCompatibility: NotRequired[DashIsoPlaybackDeviceCompatibilityType],  # (1)
    SpekeKeyProvider: NotRequired[SpekeKeyProviderOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: DashIsoPlaybackDeviceCompatibilityType](./literals.md#dashisoplaybackdevicecompatibilitytype) 
2. See [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 
## HlsEncryptionSettingsOutputTypeDef

```python
# HlsEncryptionSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import HlsEncryptionSettingsOutputTypeDef


def get_value() -> HlsEncryptionSettingsOutputTypeDef:
    return {
        "ConstantInitializationVector": ...,
    }


# HlsEncryptionSettingsOutputTypeDef definition

class HlsEncryptionSettingsOutputTypeDef(TypedDict):
    ConstantInitializationVector: NotRequired[str],
    EncryptionMethod: NotRequired[HlsEncryptionTypeType],  # (1)
    InitializationVectorInManifest: NotRequired[HlsInitializationVectorInManifestType],  # (2)
    OfflineEncrypted: NotRequired[HlsOfflineEncryptedType],  # (3)
    SpekeKeyProvider: NotRequired[SpekeKeyProviderOutputTypeDef],  # (4)
    StaticKeyProvider: NotRequired[StaticKeyProviderTypeDef],  # (5)
    Type: NotRequired[HlsKeyProviderTypeType],  # (6)
```

1. See [:material-code-brackets: HlsEncryptionTypeType](./literals.md#hlsencryptiontypetype) 
2. See [:material-code-brackets: HlsInitializationVectorInManifestType](./literals.md#hlsinitializationvectorinmanifesttype) 
3. See [:material-code-brackets: HlsOfflineEncryptedType](./literals.md#hlsofflineencryptedtype) 
4. See [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 
5. See [:material-code-braces: StaticKeyProviderTypeDef](./type_defs.md#statickeyprovidertypedef) 
6. See [:material-code-brackets: HlsKeyProviderTypeType](./literals.md#hlskeyprovidertypetype) 
## MsSmoothEncryptionSettingsOutputTypeDef

```python
# MsSmoothEncryptionSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MsSmoothEncryptionSettingsOutputTypeDef


def get_value() -> MsSmoothEncryptionSettingsOutputTypeDef:
    return {
        "SpekeKeyProvider": ...,
    }


# MsSmoothEncryptionSettingsOutputTypeDef definition

class MsSmoothEncryptionSettingsOutputTypeDef(TypedDict):
    SpekeKeyProvider: NotRequired[SpekeKeyProviderOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 
## DashIsoEncryptionSettingsTypeDef

```python
# DashIsoEncryptionSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DashIsoEncryptionSettingsTypeDef


def get_value() -> DashIsoEncryptionSettingsTypeDef:
    return {
        "PlaybackDeviceCompatibility": ...,
    }


# DashIsoEncryptionSettingsTypeDef definition

class DashIsoEncryptionSettingsTypeDef(TypedDict):
    PlaybackDeviceCompatibility: NotRequired[DashIsoPlaybackDeviceCompatibilityType],  # (1)
    SpekeKeyProvider: NotRequired[SpekeKeyProviderTypeDef],  # (2)
```

1. See [:material-code-brackets: DashIsoPlaybackDeviceCompatibilityType](./literals.md#dashisoplaybackdevicecompatibilitytype) 
2. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) 
## HlsEncryptionSettingsTypeDef

```python
# HlsEncryptionSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import HlsEncryptionSettingsTypeDef


def get_value() -> HlsEncryptionSettingsTypeDef:
    return {
        "ConstantInitializationVector": ...,
    }


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
# MsSmoothEncryptionSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MsSmoothEncryptionSettingsTypeDef


def get_value() -> MsSmoothEncryptionSettingsTypeDef:
    return {
        "SpekeKeyProvider": ...,
    }


# MsSmoothEncryptionSettingsTypeDef definition

class MsSmoothEncryptionSettingsTypeDef(TypedDict):
    SpekeKeyProvider: NotRequired[SpekeKeyProviderTypeDef],  # (1)
```

1. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) 
## ContainerSettingsOutputTypeDef

```python
# ContainerSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ContainerSettingsOutputTypeDef


def get_value() -> ContainerSettingsOutputTypeDef:
    return {
        "CmfcSettings": ...,
    }


# ContainerSettingsOutputTypeDef definition

class ContainerSettingsOutputTypeDef(TypedDict):
    CmfcSettings: NotRequired[CmfcSettingsTypeDef],  # (1)
    Container: NotRequired[ContainerTypeType],  # (2)
    F4vSettings: NotRequired[F4vSettingsTypeDef],  # (3)
    M2tsSettings: NotRequired[M2tsSettingsOutputTypeDef],  # (4)
    M3u8Settings: NotRequired[M3u8SettingsOutputTypeDef],  # (5)
    MovSettings: NotRequired[MovSettingsTypeDef],  # (6)
    Mp4Settings: NotRequired[Mp4SettingsTypeDef],  # (7)
    MpdSettings: NotRequired[MpdSettingsTypeDef],  # (8)
    MxfSettings: NotRequired[MxfSettingsTypeDef],  # (9)
```

1. See [:material-code-braces: CmfcSettingsTypeDef](./type_defs.md#cmfcsettingstypedef) 
2. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
3. See [:material-code-braces: F4vSettingsTypeDef](./type_defs.md#f4vsettingstypedef) 
4. See [:material-code-braces: M2tsSettingsOutputTypeDef](./type_defs.md#m2tssettingsoutputtypedef) 
5. See [:material-code-braces: M3u8SettingsOutputTypeDef](./type_defs.md#m3u8settingsoutputtypedef) 
6. See [:material-code-braces: MovSettingsTypeDef](./type_defs.md#movsettingstypedef) 
7. See [:material-code-braces: Mp4SettingsTypeDef](./type_defs.md#mp4settingstypedef) 
8. See [:material-code-braces: MpdSettingsTypeDef](./type_defs.md#mpdsettingstypedef) 
9. See [:material-code-braces: MxfSettingsTypeDef](./type_defs.md#mxfsettingstypedef) 
## ContainerSettingsTypeDef

```python
# ContainerSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ContainerSettingsTypeDef


def get_value() -> ContainerSettingsTypeDef:
    return {
        "CmfcSettings": ...,
    }


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
## VideoPreprocessorOutputTypeDef

```python
# VideoPreprocessorOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoPreprocessorOutputTypeDef


def get_value() -> VideoPreprocessorOutputTypeDef:
    return {
        "ColorCorrector": ...,
    }


# VideoPreprocessorOutputTypeDef definition

class VideoPreprocessorOutputTypeDef(TypedDict):
    ColorCorrector: NotRequired[ColorCorrectorTypeDef],  # (1)
    Deinterlacer: NotRequired[DeinterlacerTypeDef],  # (2)
    DolbyVision: NotRequired[DolbyVisionTypeDef],  # (3)
    Hdr10Plus: NotRequired[Hdr10PlusTypeDef],  # (4)
    ImageInserter: NotRequired[ImageInserterOutputTypeDef],  # (5)
    NoiseReducer: NotRequired[NoiseReducerTypeDef],  # (6)
    PartnerWatermarking: NotRequired[PartnerWatermarkingTypeDef],  # (7)
    TimecodeBurnin: NotRequired[TimecodeBurninTypeDef],  # (8)
```

1. See [:material-code-braces: ColorCorrectorTypeDef](./type_defs.md#colorcorrectortypedef) 
2. See [:material-code-braces: DeinterlacerTypeDef](./type_defs.md#deinterlacertypedef) 
3. See [:material-code-braces: DolbyVisionTypeDef](./type_defs.md#dolbyvisiontypedef) 
4. See [:material-code-braces: Hdr10PlusTypeDef](./type_defs.md#hdr10plustypedef) 
5. See [:material-code-braces: ImageInserterOutputTypeDef](./type_defs.md#imageinserteroutputtypedef) 
6. See [:material-code-braces: NoiseReducerTypeDef](./type_defs.md#noisereducertypedef) 
7. See [:material-code-braces: PartnerWatermarkingTypeDef](./type_defs.md#partnerwatermarkingtypedef) 
8. See [:material-code-braces: TimecodeBurninTypeDef](./type_defs.md#timecodeburnintypedef) 
## VideoPreprocessorTypeDef

```python
# VideoPreprocessorTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoPreprocessorTypeDef


def get_value() -> VideoPreprocessorTypeDef:
    return {
        "ColorCorrector": ...,
    }


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
# OutputGroupDetailTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import OutputGroupDetailTypeDef


def get_value() -> OutputGroupDetailTypeDef:
    return {
        "OutputDetails": ...,
    }


# OutputGroupDetailTypeDef definition

class OutputGroupDetailTypeDef(TypedDict):
    OutputDetails: NotRequired[List[OutputDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: OutputDetailTypeDef](./type_defs.md#outputdetailtypedef) 
## CreateQueueResponseTypeDef

```python
# CreateQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CreateQueueResponseTypeDef


def get_value() -> CreateQueueResponseTypeDef:
    return {
        "Queue": ...,
    }


# CreateQueueResponseTypeDef definition

class CreateQueueResponseTypeDef(TypedDict):
    Queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueueResponseTypeDef

```python
# GetQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import GetQueueResponseTypeDef


def get_value() -> GetQueueResponseTypeDef:
    return {
        "Queue": ...,
    }


# GetQueueResponseTypeDef definition

class GetQueueResponseTypeDef(TypedDict):
    Queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueuesResponseTypeDef

```python
# ListQueuesResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListQueuesResponseTypeDef


def get_value() -> ListQueuesResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListQueuesResponseTypeDef definition

class ListQueuesResponseTypeDef(TypedDict):
    Queues: List[QueueTypeDef],  # (1)
    TotalConcurrentJobs: int,
    UnallocatedConcurrentJobs: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQueueResponseTypeDef

```python
# UpdateQueueResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import UpdateQueueResponseTypeDef


def get_value() -> UpdateQueueResponseTypeDef:
    return {
        "Queue": ...,
    }


# UpdateQueueResponseTypeDef definition

class UpdateQueueResponseTypeDef(TypedDict):
    Queue: QueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationSettingsTypeDef

```python
# DestinationSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DestinationSettingsTypeDef


def get_value() -> DestinationSettingsTypeDef:
    return {
        "S3Settings": ...,
    }


# DestinationSettingsTypeDef definition

class DestinationSettingsTypeDef(TypedDict):
    S3Settings: NotRequired[S3DestinationSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: S3DestinationSettingsTypeDef](./type_defs.md#s3destinationsettingstypedef) 
## VideoOverlayOutputTypeDef

```python
# VideoOverlayOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoOverlayOutputTypeDef


def get_value() -> VideoOverlayOutputTypeDef:
    return {
        "EndTimecode": ...,
    }


# VideoOverlayOutputTypeDef definition

class VideoOverlayOutputTypeDef(TypedDict):
    EndTimecode: NotRequired[str],
    InitialPosition: NotRequired[VideoOverlayPositionTypeDef],  # (1)
    Input: NotRequired[VideoOverlayInputOutputTypeDef],  # (2)
    Playback: NotRequired[VideoOverlayPlayBackModeType],  # (3)
    StartTimecode: NotRequired[str],
    Transitions: NotRequired[List[VideoOverlayTransitionTypeDef]],  # (4)
```

1. See [:material-code-braces: VideoOverlayPositionTypeDef](./type_defs.md#videooverlaypositiontypedef) 
2. See [:material-code-braces: VideoOverlayInputOutputTypeDef](./type_defs.md#videooverlayinputoutputtypedef) 
3. See [:material-code-brackets: VideoOverlayPlayBackModeType](./literals.md#videooverlayplaybackmodetype) 
4. See [:material-code-braces: VideoOverlayTransitionTypeDef](./type_defs.md#videooverlaytransitiontypedef) 
## VideoOverlayTypeDef

```python
# VideoOverlayTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoOverlayTypeDef


def get_value() -> VideoOverlayTypeDef:
    return {
        "EndTimecode": ...,
    }


# VideoOverlayTypeDef definition

class VideoOverlayTypeDef(TypedDict):
    EndTimecode: NotRequired[str],
    InitialPosition: NotRequired[VideoOverlayPositionTypeDef],  # (1)
    Input: NotRequired[VideoOverlayInputTypeDef],  # (2)
    Playback: NotRequired[VideoOverlayPlayBackModeType],  # (3)
    StartTimecode: NotRequired[str],
    Transitions: NotRequired[Sequence[VideoOverlayTransitionTypeDef]],  # (4)
```

1. See [:material-code-braces: VideoOverlayPositionTypeDef](./type_defs.md#videooverlaypositiontypedef) 
2. See [:material-code-braces: VideoOverlayInputTypeDef](./type_defs.md#videooverlayinputtypedef) 
3. See [:material-code-brackets: VideoOverlayPlayBackModeType](./literals.md#videooverlayplaybackmodetype) 
4. See [:material-code-braces: VideoOverlayTransitionTypeDef](./type_defs.md#videooverlaytransitiontypedef) 
## VideoCodecSettingsTypeDef

```python
# VideoCodecSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoCodecSettingsTypeDef


def get_value() -> VideoCodecSettingsTypeDef:
    return {
        "Av1Settings": ...,
    }


# VideoCodecSettingsTypeDef definition

class VideoCodecSettingsTypeDef(TypedDict):
    Av1Settings: NotRequired[Av1SettingsTypeDef],  # (1)
    AvcIntraSettings: NotRequired[AvcIntraSettingsTypeDef],  # (2)
    Codec: NotRequired[VideoCodecType],  # (3)
    FrameCaptureSettings: NotRequired[FrameCaptureSettingsTypeDef],  # (4)
    GifSettings: NotRequired[GifSettingsTypeDef],  # (5)
    H264Settings: NotRequired[H264SettingsTypeDef],  # (6)
    H265Settings: NotRequired[H265SettingsTypeDef],  # (7)
    Mpeg2Settings: NotRequired[Mpeg2SettingsTypeDef],  # (8)
    ProresSettings: NotRequired[ProresSettingsTypeDef],  # (9)
    UncompressedSettings: NotRequired[UncompressedSettingsTypeDef],  # (10)
    Vc3Settings: NotRequired[Vc3SettingsTypeDef],  # (11)
    Vp8Settings: NotRequired[Vp8SettingsTypeDef],  # (12)
    Vp9Settings: NotRequired[Vp9SettingsTypeDef],  # (13)
    XavcSettings: NotRequired[XavcSettingsTypeDef],  # (14)
```

1. See [:material-code-braces: Av1SettingsTypeDef](./type_defs.md#av1settingstypedef) 
2. See [:material-code-braces: AvcIntraSettingsTypeDef](./type_defs.md#avcintrasettingstypedef) 
3. See [:material-code-brackets: VideoCodecType](./literals.md#videocodectype) 
4. See [:material-code-braces: FrameCaptureSettingsTypeDef](./type_defs.md#framecapturesettingstypedef) 
5. See [:material-code-braces: GifSettingsTypeDef](./type_defs.md#gifsettingstypedef) 
6. See [:material-code-braces: H264SettingsTypeDef](./type_defs.md#h264settingstypedef) 
7. See [:material-code-braces: H265SettingsTypeDef](./type_defs.md#h265settingstypedef) 
8. See [:material-code-braces: Mpeg2SettingsTypeDef](./type_defs.md#mpeg2settingstypedef) 
9. See [:material-code-braces: ProresSettingsTypeDef](./type_defs.md#proressettingstypedef) 
10. See [:material-code-braces: UncompressedSettingsTypeDef](./type_defs.md#uncompressedsettingstypedef) 
11. See [:material-code-braces: Vc3SettingsTypeDef](./type_defs.md#vc3settingstypedef) 
12. See [:material-code-braces: Vp8SettingsTypeDef](./type_defs.md#vp8settingstypedef) 
13. See [:material-code-braces: Vp9SettingsTypeDef](./type_defs.md#vp9settingstypedef) 
14. See [:material-code-braces: XavcSettingsTypeDef](./type_defs.md#xavcsettingstypedef) 
## AutomatedEncodingSettingsOutputTypeDef

```python
# AutomatedEncodingSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AutomatedEncodingSettingsOutputTypeDef


def get_value() -> AutomatedEncodingSettingsOutputTypeDef:
    return {
        "AbrSettings": ...,
    }


# AutomatedEncodingSettingsOutputTypeDef definition

class AutomatedEncodingSettingsOutputTypeDef(TypedDict):
    AbrSettings: NotRequired[AutomatedAbrSettingsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: AutomatedAbrSettingsOutputTypeDef](./type_defs.md#automatedabrsettingsoutputtypedef) 
## AutomatedEncodingSettingsTypeDef

```python
# AutomatedEncodingSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AutomatedEncodingSettingsTypeDef


def get_value() -> AutomatedEncodingSettingsTypeDef:
    return {
        "AbrSettings": ...,
    }


# AutomatedEncodingSettingsTypeDef definition

class AutomatedEncodingSettingsTypeDef(TypedDict):
    AbrSettings: NotRequired[AutomatedAbrSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: AutomatedAbrSettingsTypeDef](./type_defs.md#automatedabrsettingstypedef) 
## CaptionSelectorTypeDef

```python
# CaptionSelectorTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CaptionSelectorTypeDef


def get_value() -> CaptionSelectorTypeDef:
    return {
        "CustomLanguageCode": ...,
    }


# CaptionSelectorTypeDef definition

class CaptionSelectorTypeDef(TypedDict):
    CustomLanguageCode: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (1)
    SourceSettings: NotRequired[CaptionSourceSettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: CaptionSourceSettingsTypeDef](./type_defs.md#captionsourcesettingstypedef) 
## AudioDescriptionOutputTypeDef

```python
# AudioDescriptionOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AudioDescriptionOutputTypeDef


def get_value() -> AudioDescriptionOutputTypeDef:
    return {
        "AudioChannelTaggingSettings": ...,
    }


# AudioDescriptionOutputTypeDef definition

class AudioDescriptionOutputTypeDef(TypedDict):
    AudioChannelTaggingSettings: NotRequired[AudioChannelTaggingSettingsOutputTypeDef],  # (1)
    AudioNormalizationSettings: NotRequired[AudioNormalizationSettingsTypeDef],  # (2)
    AudioSourceName: NotRequired[str],
    AudioType: NotRequired[int],
    AudioTypeControl: NotRequired[AudioTypeControlType],  # (3)
    CodecSettings: NotRequired[AudioCodecSettingsTypeDef],  # (4)
    CustomLanguageCode: NotRequired[str],
    LanguageCode: NotRequired[LanguageCodeType],  # (5)
    LanguageCodeControl: NotRequired[AudioLanguageCodeControlType],  # (6)
    RemixSettings: NotRequired[RemixSettingsOutputTypeDef],  # (7)
    StreamName: NotRequired[str],
```

1. See [:material-code-braces: AudioChannelTaggingSettingsOutputTypeDef](./type_defs.md#audiochanneltaggingsettingsoutputtypedef) 
2. See [:material-code-braces: AudioNormalizationSettingsTypeDef](./type_defs.md#audionormalizationsettingstypedef) 
3. See [:material-code-brackets: AudioTypeControlType](./literals.md#audiotypecontroltype) 
4. See [:material-code-braces: AudioCodecSettingsTypeDef](./type_defs.md#audiocodecsettingstypedef) 
5. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
6. See [:material-code-brackets: AudioLanguageCodeControlType](./literals.md#audiolanguagecodecontroltype) 
7. See [:material-code-braces: RemixSettingsOutputTypeDef](./type_defs.md#remixsettingsoutputtypedef) 
## AudioSelectorOutputTypeDef

```python
# AudioSelectorOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AudioSelectorOutputTypeDef


def get_value() -> AudioSelectorOutputTypeDef:
    return {
        "AudioDurationCorrection": ...,
    }


# AudioSelectorOutputTypeDef definition

class AudioSelectorOutputTypeDef(TypedDict):
    AudioDurationCorrection: NotRequired[AudioDurationCorrectionType],  # (1)
    CustomLanguageCode: NotRequired[str],
    DefaultSelection: NotRequired[AudioDefaultSelectionType],  # (2)
    ExternalAudioFileInput: NotRequired[str],
    HlsRenditionGroupSettings: NotRequired[HlsRenditionGroupSettingsTypeDef],  # (3)
    LanguageCode: NotRequired[LanguageCodeType],  # (4)
    Offset: NotRequired[int],
    Pids: NotRequired[List[int]],
    ProgramSelection: NotRequired[int],
    RemixSettings: NotRequired[RemixSettingsOutputTypeDef],  # (5)
    SelectorType: NotRequired[AudioSelectorTypeType],  # (6)
    Tracks: NotRequired[List[int]],
```

1. See [:material-code-brackets: AudioDurationCorrectionType](./literals.md#audiodurationcorrectiontype) 
2. See [:material-code-brackets: AudioDefaultSelectionType](./literals.md#audiodefaultselectiontype) 
3. See [:material-code-braces: HlsRenditionGroupSettingsTypeDef](./type_defs.md#hlsrenditiongroupsettingstypedef) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-braces: RemixSettingsOutputTypeDef](./type_defs.md#remixsettingsoutputtypedef) 
6. See [:material-code-brackets: AudioSelectorTypeType](./literals.md#audioselectortypetype) 
## AudioDescriptionTypeDef

```python
# AudioDescriptionTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AudioDescriptionTypeDef


def get_value() -> AudioDescriptionTypeDef:
    return {
        "AudioChannelTaggingSettings": ...,
    }


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
# AudioSelectorTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import AudioSelectorTypeDef


def get_value() -> AudioSelectorTypeDef:
    return {
        "AudioDurationCorrection": ...,
    }


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
## CmafGroupSettingsOutputTypeDef

```python
# CmafGroupSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CmafGroupSettingsOutputTypeDef


def get_value() -> CmafGroupSettingsOutputTypeDef:
    return {
        "AdditionalManifests": ...,
    }


# CmafGroupSettingsOutputTypeDef definition

class CmafGroupSettingsOutputTypeDef(TypedDict):
    AdditionalManifests: NotRequired[List[CmafAdditionalManifestOutputTypeDef]],  # (1)
    BaseUrl: NotRequired[str],
    ClientCache: NotRequired[CmafClientCacheType],  # (2)
    CodecSpecification: NotRequired[CmafCodecSpecificationType],  # (3)
    DashIFrameTrickPlayNameModifier: NotRequired[str],
    DashManifestStyle: NotRequired[DashManifestStyleType],  # (4)
    Destination: NotRequired[str],
    DestinationSettings: NotRequired[DestinationSettingsTypeDef],  # (5)
    Encryption: NotRequired[CmafEncryptionSettingsOutputTypeDef],  # (6)
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

1. See [:material-code-braces: CmafAdditionalManifestOutputTypeDef](./type_defs.md#cmafadditionalmanifestoutputtypedef) 
2. See [:material-code-brackets: CmafClientCacheType](./literals.md#cmafclientcachetype) 
3. See [:material-code-brackets: CmafCodecSpecificationType](./literals.md#cmafcodecspecificationtype) 
4. See [:material-code-brackets: DashManifestStyleType](./literals.md#dashmanifeststyletype) 
5. See [:material-code-braces: DestinationSettingsTypeDef](./type_defs.md#destinationsettingstypedef) 
6. See [:material-code-braces: CmafEncryptionSettingsOutputTypeDef](./type_defs.md#cmafencryptionsettingsoutputtypedef) 
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
## CmafGroupSettingsTypeDef

```python
# CmafGroupSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CmafGroupSettingsTypeDef


def get_value() -> CmafGroupSettingsTypeDef:
    return {
        "AdditionalManifests": ...,
    }


# CmafGroupSettingsTypeDef definition

class CmafGroupSettingsTypeDef(TypedDict):
    AdditionalManifests: NotRequired[Sequence[CmafAdditionalManifestTypeDef]],  # (1)
    BaseUrl: NotRequired[str],
    ClientCache: NotRequired[CmafClientCacheType],  # (2)
    CodecSpecification: NotRequired[CmafCodecSpecificationType],  # (3)
    DashIFrameTrickPlayNameModifier: NotRequired[str],
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
## DashIsoGroupSettingsOutputTypeDef

```python
# DashIsoGroupSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DashIsoGroupSettingsOutputTypeDef


def get_value() -> DashIsoGroupSettingsOutputTypeDef:
    return {
        "AdditionalManifests": ...,
    }


# DashIsoGroupSettingsOutputTypeDef definition

class DashIsoGroupSettingsOutputTypeDef(TypedDict):
    AdditionalManifests: NotRequired[List[DashAdditionalManifestOutputTypeDef]],  # (1)
    AudioChannelConfigSchemeIdUri: NotRequired[DashIsoGroupAudioChannelConfigSchemeIdUriType],  # (2)
    BaseUrl: NotRequired[str],
    DashIFrameTrickPlayNameModifier: NotRequired[str],
    DashManifestStyle: NotRequired[DashManifestStyleType],  # (3)
    Destination: NotRequired[str],
    DestinationSettings: NotRequired[DestinationSettingsTypeDef],  # (4)
    Encryption: NotRequired[DashIsoEncryptionSettingsOutputTypeDef],  # (5)
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

1. See [:material-code-braces: DashAdditionalManifestOutputTypeDef](./type_defs.md#dashadditionalmanifestoutputtypedef) 
2. See [:material-code-brackets: DashIsoGroupAudioChannelConfigSchemeIdUriType](./literals.md#dashisogroupaudiochannelconfigschemeiduritype) 
3. See [:material-code-brackets: DashManifestStyleType](./literals.md#dashmanifeststyletype) 
4. See [:material-code-braces: DestinationSettingsTypeDef](./type_defs.md#destinationsettingstypedef) 
5. See [:material-code-braces: DashIsoEncryptionSettingsOutputTypeDef](./type_defs.md#dashisoencryptionsettingsoutputtypedef) 
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
## DashIsoGroupSettingsTypeDef

```python
# DashIsoGroupSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import DashIsoGroupSettingsTypeDef


def get_value() -> DashIsoGroupSettingsTypeDef:
    return {
        "AdditionalManifests": ...,
    }


# DashIsoGroupSettingsTypeDef definition

class DashIsoGroupSettingsTypeDef(TypedDict):
    AdditionalManifests: NotRequired[Sequence[DashAdditionalManifestTypeDef]],  # (1)
    AudioChannelConfigSchemeIdUri: NotRequired[DashIsoGroupAudioChannelConfigSchemeIdUriType],  # (2)
    BaseUrl: NotRequired[str],
    DashIFrameTrickPlayNameModifier: NotRequired[str],
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
# FileGroupSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import FileGroupSettingsTypeDef


def get_value() -> FileGroupSettingsTypeDef:
    return {
        "Destination": ...,
    }


# FileGroupSettingsTypeDef definition

class FileGroupSettingsTypeDef(TypedDict):
    Destination: NotRequired[str],
    DestinationSettings: NotRequired[DestinationSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: DestinationSettingsTypeDef](./type_defs.md#destinationsettingstypedef) 
## HlsGroupSettingsOutputTypeDef

```python
# HlsGroupSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import HlsGroupSettingsOutputTypeDef


def get_value() -> HlsGroupSettingsOutputTypeDef:
    return {
        "AdMarkers": ...,
    }


# HlsGroupSettingsOutputTypeDef definition

class HlsGroupSettingsOutputTypeDef(TypedDict):
    AdMarkers: NotRequired[List[HlsAdMarkersType]],  # (1)
    AdditionalManifests: NotRequired[List[HlsAdditionalManifestOutputTypeDef]],  # (2)
    AudioOnlyHeader: NotRequired[HlsAudioOnlyHeaderType],  # (3)
    BaseUrl: NotRequired[str],
    CaptionLanguageMappings: NotRequired[List[HlsCaptionLanguageMappingTypeDef]],  # (4)
    CaptionLanguageSetting: NotRequired[HlsCaptionLanguageSettingType],  # (5)
    CaptionSegmentLengthControl: NotRequired[HlsCaptionSegmentLengthControlType],  # (6)
    ClientCache: NotRequired[HlsClientCacheType],  # (7)
    CodecSpecification: NotRequired[HlsCodecSpecificationType],  # (8)
    Destination: NotRequired[str],
    DestinationSettings: NotRequired[DestinationSettingsTypeDef],  # (9)
    DirectoryStructure: NotRequired[HlsDirectoryStructureType],  # (10)
    Encryption: NotRequired[HlsEncryptionSettingsOutputTypeDef],  # (11)
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
2. See [:material-code-braces: HlsAdditionalManifestOutputTypeDef](./type_defs.md#hlsadditionalmanifestoutputtypedef) 
3. See [:material-code-brackets: HlsAudioOnlyHeaderType](./literals.md#hlsaudioonlyheadertype) 
4. See [:material-code-braces: HlsCaptionLanguageMappingTypeDef](./type_defs.md#hlscaptionlanguagemappingtypedef) 
5. See [:material-code-brackets: HlsCaptionLanguageSettingType](./literals.md#hlscaptionlanguagesettingtype) 
6. See [:material-code-brackets: HlsCaptionSegmentLengthControlType](./literals.md#hlscaptionsegmentlengthcontroltype) 
7. See [:material-code-brackets: HlsClientCacheType](./literals.md#hlsclientcachetype) 
8. See [:material-code-brackets: HlsCodecSpecificationType](./literals.md#hlscodecspecificationtype) 
9. See [:material-code-braces: DestinationSettingsTypeDef](./type_defs.md#destinationsettingstypedef) 
10. See [:material-code-brackets: HlsDirectoryStructureType](./literals.md#hlsdirectorystructuretype) 
11. See [:material-code-braces: HlsEncryptionSettingsOutputTypeDef](./type_defs.md#hlsencryptionsettingsoutputtypedef) 
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
## HlsGroupSettingsTypeDef

```python
# HlsGroupSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import HlsGroupSettingsTypeDef


def get_value() -> HlsGroupSettingsTypeDef:
    return {
        "AdMarkers": ...,
    }


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
## MsSmoothGroupSettingsOutputTypeDef

```python
# MsSmoothGroupSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MsSmoothGroupSettingsOutputTypeDef


def get_value() -> MsSmoothGroupSettingsOutputTypeDef:
    return {
        "AdditionalManifests": ...,
    }


# MsSmoothGroupSettingsOutputTypeDef definition

class MsSmoothGroupSettingsOutputTypeDef(TypedDict):
    AdditionalManifests: NotRequired[List[MsSmoothAdditionalManifestOutputTypeDef]],  # (1)
    AudioDeduplication: NotRequired[MsSmoothAudioDeduplicationType],  # (2)
    Destination: NotRequired[str],
    DestinationSettings: NotRequired[DestinationSettingsTypeDef],  # (3)
    Encryption: NotRequired[MsSmoothEncryptionSettingsOutputTypeDef],  # (4)
    FragmentLength: NotRequired[int],
    FragmentLengthControl: NotRequired[MsSmoothFragmentLengthControlType],  # (5)
    ManifestEncoding: NotRequired[MsSmoothManifestEncodingType],  # (6)
```

1. See [:material-code-braces: MsSmoothAdditionalManifestOutputTypeDef](./type_defs.md#mssmoothadditionalmanifestoutputtypedef) 
2. See [:material-code-brackets: MsSmoothAudioDeduplicationType](./literals.md#mssmoothaudiodeduplicationtype) 
3. See [:material-code-braces: DestinationSettingsTypeDef](./type_defs.md#destinationsettingstypedef) 
4. See [:material-code-braces: MsSmoothEncryptionSettingsOutputTypeDef](./type_defs.md#mssmoothencryptionsettingsoutputtypedef) 
5. See [:material-code-brackets: MsSmoothFragmentLengthControlType](./literals.md#mssmoothfragmentlengthcontroltype) 
6. See [:material-code-brackets: MsSmoothManifestEncodingType](./literals.md#mssmoothmanifestencodingtype) 
## MsSmoothGroupSettingsTypeDef

```python
# MsSmoothGroupSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import MsSmoothGroupSettingsTypeDef


def get_value() -> MsSmoothGroupSettingsTypeDef:
    return {
        "AdditionalManifests": ...,
    }


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
## VideoDescriptionOutputTypeDef

```python
# VideoDescriptionOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoDescriptionOutputTypeDef


def get_value() -> VideoDescriptionOutputTypeDef:
    return {
        "AfdSignaling": ...,
    }


# VideoDescriptionOutputTypeDef definition

class VideoDescriptionOutputTypeDef(TypedDict):
    AfdSignaling: NotRequired[AfdSignalingType],  # (1)
    AntiAlias: NotRequired[AntiAliasType],  # (2)
    ChromaPositionMode: NotRequired[ChromaPositionModeType],  # (3)
    CodecSettings: NotRequired[VideoCodecSettingsTypeDef],  # (4)
    ColorMetadata: NotRequired[ColorMetadataType],  # (5)
    Crop: NotRequired[RectangleTypeDef],  # (6)
    DropFrameTimecode: NotRequired[DropFrameTimecodeType],  # (7)
    FixedAfd: NotRequired[int],
    Height: NotRequired[int],
    Position: NotRequired[RectangleTypeDef],  # (6)
    RespondToAfd: NotRequired[RespondToAfdType],  # (9)
    ScalingBehavior: NotRequired[ScalingBehaviorType],  # (10)
    Sharpness: NotRequired[int],
    TimecodeInsertion: NotRequired[VideoTimecodeInsertionType],  # (11)
    TimecodeTrack: NotRequired[TimecodeTrackType],  # (12)
    VideoPreprocessors: NotRequired[VideoPreprocessorOutputTypeDef],  # (13)
    Width: NotRequired[int],
```

1. See [:material-code-brackets: AfdSignalingType](./literals.md#afdsignalingtype) 
2. See [:material-code-brackets: AntiAliasType](./literals.md#antialiastype) 
3. See [:material-code-brackets: ChromaPositionModeType](./literals.md#chromapositionmodetype) 
4. See [:material-code-braces: VideoCodecSettingsTypeDef](./type_defs.md#videocodecsettingstypedef) 
5. See [:material-code-brackets: ColorMetadataType](./literals.md#colormetadatatype) 
6. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
7. See [:material-code-brackets: DropFrameTimecodeType](./literals.md#dropframetimecodetype) 
8. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
9. See [:material-code-brackets: RespondToAfdType](./literals.md#respondtoafdtype) 
10. See [:material-code-brackets: ScalingBehaviorType](./literals.md#scalingbehaviortype) 
11. See [:material-code-brackets: VideoTimecodeInsertionType](./literals.md#videotimecodeinsertiontype) 
12. See [:material-code-brackets: TimecodeTrackType](./literals.md#timecodetracktype) 
13. See [:material-code-braces: VideoPreprocessorOutputTypeDef](./type_defs.md#videopreprocessoroutputtypedef) 
## VideoDescriptionTypeDef

```python
# VideoDescriptionTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import VideoDescriptionTypeDef


def get_value() -> VideoDescriptionTypeDef:
    return {
        "AfdSignaling": ...,
    }


# VideoDescriptionTypeDef definition

class VideoDescriptionTypeDef(TypedDict):
    AfdSignaling: NotRequired[AfdSignalingType],  # (1)
    AntiAlias: NotRequired[AntiAliasType],  # (2)
    ChromaPositionMode: NotRequired[ChromaPositionModeType],  # (3)
    CodecSettings: NotRequired[VideoCodecSettingsTypeDef],  # (4)
    ColorMetadata: NotRequired[ColorMetadataType],  # (5)
    Crop: NotRequired[RectangleTypeDef],  # (6)
    DropFrameTimecode: NotRequired[DropFrameTimecodeType],  # (7)
    FixedAfd: NotRequired[int],
    Height: NotRequired[int],
    Position: NotRequired[RectangleTypeDef],  # (6)
    RespondToAfd: NotRequired[RespondToAfdType],  # (9)
    ScalingBehavior: NotRequired[ScalingBehaviorType],  # (10)
    Sharpness: NotRequired[int],
    TimecodeInsertion: NotRequired[VideoTimecodeInsertionType],  # (11)
    TimecodeTrack: NotRequired[TimecodeTrackType],  # (12)
    VideoPreprocessors: NotRequired[VideoPreprocessorTypeDef],  # (13)
    Width: NotRequired[int],
```

1. See [:material-code-brackets: AfdSignalingType](./literals.md#afdsignalingtype) 
2. See [:material-code-brackets: AntiAliasType](./literals.md#antialiastype) 
3. See [:material-code-brackets: ChromaPositionModeType](./literals.md#chromapositionmodetype) 
4. See [:material-code-braces: VideoCodecSettingsTypeDef](./type_defs.md#videocodecsettingstypedef) 
5. See [:material-code-brackets: ColorMetadataType](./literals.md#colormetadatatype) 
6. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
7. See [:material-code-brackets: DropFrameTimecodeType](./literals.md#dropframetimecodetype) 
8. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
9. See [:material-code-brackets: RespondToAfdType](./literals.md#respondtoafdtype) 
10. See [:material-code-brackets: ScalingBehaviorType](./literals.md#scalingbehaviortype) 
11. See [:material-code-brackets: VideoTimecodeInsertionType](./literals.md#videotimecodeinsertiontype) 
12. See [:material-code-brackets: TimecodeTrackType](./literals.md#timecodetracktype) 
13. See [:material-code-braces: VideoPreprocessorTypeDef](./type_defs.md#videopreprocessortypedef) 
## InputOutputTypeDef

```python
# InputOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import InputOutputTypeDef


def get_value() -> InputOutputTypeDef:
    return {
        "AdvancedInputFilter": ...,
    }


# InputOutputTypeDef definition

class InputOutputTypeDef(TypedDict):
    AdvancedInputFilter: NotRequired[AdvancedInputFilterType],  # (1)
    AdvancedInputFilterSettings: NotRequired[AdvancedInputFilterSettingsTypeDef],  # (2)
    AudioSelectorGroups: NotRequired[Dict[str, AudioSelectorGroupOutputTypeDef]],  # (3)
    AudioSelectors: NotRequired[Dict[str, AudioSelectorOutputTypeDef]],  # (4)
    CaptionSelectors: NotRequired[Dict[str, CaptionSelectorTypeDef]],  # (5)
    Crop: NotRequired[RectangleTypeDef],  # (6)
    DeblockFilter: NotRequired[InputDeblockFilterType],  # (7)
    DecryptionSettings: NotRequired[InputDecryptionSettingsTypeDef],  # (8)
    DenoiseFilter: NotRequired[InputDenoiseFilterType],  # (9)
    DolbyVisionMetadataXml: NotRequired[str],
    DynamicAudioSelectors: NotRequired[Dict[str, DynamicAudioSelectorTypeDef]],  # (10)
    FileInput: NotRequired[str],
    FilterEnable: NotRequired[InputFilterEnableType],  # (11)
    FilterStrength: NotRequired[int],
    ImageInserter: NotRequired[ImageInserterOutputTypeDef],  # (12)
    InputClippings: NotRequired[List[InputClippingTypeDef]],  # (13)
    InputScanType: NotRequired[InputScanTypeType],  # (14)
    Position: NotRequired[RectangleTypeDef],  # (6)
    ProgramNumber: NotRequired[int],
    PsiControl: NotRequired[InputPsiControlType],  # (16)
    SupplementalImps: NotRequired[List[str]],
    TimecodeSource: NotRequired[InputTimecodeSourceType],  # (17)
    TimecodeStart: NotRequired[str],
    VideoGenerator: NotRequired[InputVideoGeneratorTypeDef],  # (18)
    VideoOverlays: NotRequired[List[VideoOverlayOutputTypeDef]],  # (19)
    VideoSelector: NotRequired[VideoSelectorTypeDef],  # (20)
```

1. See [:material-code-brackets: AdvancedInputFilterType](./literals.md#advancedinputfiltertype) 
2. See [:material-code-braces: AdvancedInputFilterSettingsTypeDef](./type_defs.md#advancedinputfiltersettingstypedef) 
3. See [:material-code-braces: AudioSelectorGroupOutputTypeDef](./type_defs.md#audioselectorgroupoutputtypedef) 
4. See [:material-code-braces: AudioSelectorOutputTypeDef](./type_defs.md#audioselectoroutputtypedef) 
5. See [:material-code-braces: CaptionSelectorTypeDef](./type_defs.md#captionselectortypedef) 
6. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
7. See [:material-code-brackets: InputDeblockFilterType](./literals.md#inputdeblockfiltertype) 
8. See [:material-code-braces: InputDecryptionSettingsTypeDef](./type_defs.md#inputdecryptionsettingstypedef) 
9. See [:material-code-brackets: InputDenoiseFilterType](./literals.md#inputdenoisefiltertype) 
10. See [:material-code-braces: DynamicAudioSelectorTypeDef](./type_defs.md#dynamicaudioselectortypedef) 
11. See [:material-code-brackets: InputFilterEnableType](./literals.md#inputfilterenabletype) 
12. See [:material-code-braces: ImageInserterOutputTypeDef](./type_defs.md#imageinserteroutputtypedef) 
13. See [:material-code-braces: InputClippingTypeDef](./type_defs.md#inputclippingtypedef) 
14. See [:material-code-brackets: InputScanTypeType](./literals.md#inputscantypetype) 
15. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
16. See [:material-code-brackets: InputPsiControlType](./literals.md#inputpsicontroltype) 
17. See [:material-code-brackets: InputTimecodeSourceType](./literals.md#inputtimecodesourcetype) 
18. See [:material-code-braces: InputVideoGeneratorTypeDef](./type_defs.md#inputvideogeneratortypedef) 
19. See [:material-code-braces: VideoOverlayOutputTypeDef](./type_defs.md#videooverlayoutputtypedef) 
20. See [:material-code-braces: VideoSelectorTypeDef](./type_defs.md#videoselectortypedef) 
## InputTemplateOutputTypeDef

```python
# InputTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import InputTemplateOutputTypeDef


def get_value() -> InputTemplateOutputTypeDef:
    return {
        "AdvancedInputFilter": ...,
    }


# InputTemplateOutputTypeDef definition

class InputTemplateOutputTypeDef(TypedDict):
    AdvancedInputFilter: NotRequired[AdvancedInputFilterType],  # (1)
    AdvancedInputFilterSettings: NotRequired[AdvancedInputFilterSettingsTypeDef],  # (2)
    AudioSelectorGroups: NotRequired[Dict[str, AudioSelectorGroupOutputTypeDef]],  # (3)
    AudioSelectors: NotRequired[Dict[str, AudioSelectorOutputTypeDef]],  # (4)
    CaptionSelectors: NotRequired[Dict[str, CaptionSelectorTypeDef]],  # (5)
    Crop: NotRequired[RectangleTypeDef],  # (6)
    DeblockFilter: NotRequired[InputDeblockFilterType],  # (7)
    DenoiseFilter: NotRequired[InputDenoiseFilterType],  # (8)
    DolbyVisionMetadataXml: NotRequired[str],
    DynamicAudioSelectors: NotRequired[Dict[str, DynamicAudioSelectorTypeDef]],  # (9)
    FilterEnable: NotRequired[InputFilterEnableType],  # (10)
    FilterStrength: NotRequired[int],
    ImageInserter: NotRequired[ImageInserterOutputTypeDef],  # (11)
    InputClippings: NotRequired[List[InputClippingTypeDef]],  # (12)
    InputScanType: NotRequired[InputScanTypeType],  # (13)
    Position: NotRequired[RectangleTypeDef],  # (6)
    ProgramNumber: NotRequired[int],
    PsiControl: NotRequired[InputPsiControlType],  # (15)
    TimecodeSource: NotRequired[InputTimecodeSourceType],  # (16)
    TimecodeStart: NotRequired[str],
    VideoOverlays: NotRequired[List[VideoOverlayOutputTypeDef]],  # (17)
    VideoSelector: NotRequired[VideoSelectorTypeDef],  # (18)
```

1. See [:material-code-brackets: AdvancedInputFilterType](./literals.md#advancedinputfiltertype) 
2. See [:material-code-braces: AdvancedInputFilterSettingsTypeDef](./type_defs.md#advancedinputfiltersettingstypedef) 
3. See [:material-code-braces: AudioSelectorGroupOutputTypeDef](./type_defs.md#audioselectorgroupoutputtypedef) 
4. See [:material-code-braces: AudioSelectorOutputTypeDef](./type_defs.md#audioselectoroutputtypedef) 
5. See [:material-code-braces: CaptionSelectorTypeDef](./type_defs.md#captionselectortypedef) 
6. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
7. See [:material-code-brackets: InputDeblockFilterType](./literals.md#inputdeblockfiltertype) 
8. See [:material-code-brackets: InputDenoiseFilterType](./literals.md#inputdenoisefiltertype) 
9. See [:material-code-braces: DynamicAudioSelectorTypeDef](./type_defs.md#dynamicaudioselectortypedef) 
10. See [:material-code-brackets: InputFilterEnableType](./literals.md#inputfilterenabletype) 
11. See [:material-code-braces: ImageInserterOutputTypeDef](./type_defs.md#imageinserteroutputtypedef) 
12. See [:material-code-braces: InputClippingTypeDef](./type_defs.md#inputclippingtypedef) 
13. See [:material-code-brackets: InputScanTypeType](./literals.md#inputscantypetype) 
14. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
15. See [:material-code-brackets: InputPsiControlType](./literals.md#inputpsicontroltype) 
16. See [:material-code-brackets: InputTimecodeSourceType](./literals.md#inputtimecodesourcetype) 
17. See [:material-code-braces: VideoOverlayOutputTypeDef](./type_defs.md#videooverlayoutputtypedef) 
18. See [:material-code-braces: VideoSelectorTypeDef](./type_defs.md#videoselectortypedef) 
## InputTemplateTypeDef

```python
# InputTemplateTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import InputTemplateTypeDef


def get_value() -> InputTemplateTypeDef:
    return {
        "AdvancedInputFilter": ...,
    }


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
    DynamicAudioSelectors: NotRequired[Mapping[str, DynamicAudioSelectorTypeDef]],  # (9)
    FilterEnable: NotRequired[InputFilterEnableType],  # (10)
    FilterStrength: NotRequired[int],
    ImageInserter: NotRequired[ImageInserterTypeDef],  # (11)
    InputClippings: NotRequired[Sequence[InputClippingTypeDef]],  # (12)
    InputScanType: NotRequired[InputScanTypeType],  # (13)
    Position: NotRequired[RectangleTypeDef],  # (6)
    ProgramNumber: NotRequired[int],
    PsiControl: NotRequired[InputPsiControlType],  # (15)
    TimecodeSource: NotRequired[InputTimecodeSourceType],  # (16)
    TimecodeStart: NotRequired[str],
    VideoOverlays: NotRequired[Sequence[VideoOverlayTypeDef]],  # (17)
    VideoSelector: NotRequired[VideoSelectorTypeDef],  # (18)
```

1. See [:material-code-brackets: AdvancedInputFilterType](./literals.md#advancedinputfiltertype) 
2. See [:material-code-braces: AdvancedInputFilterSettingsTypeDef](./type_defs.md#advancedinputfiltersettingstypedef) 
3. See [:material-code-braces: AudioSelectorGroupTypeDef](./type_defs.md#audioselectorgrouptypedef) 
4. See [:material-code-braces: AudioSelectorTypeDef](./type_defs.md#audioselectortypedef) 
5. See [:material-code-braces: CaptionSelectorTypeDef](./type_defs.md#captionselectortypedef) 
6. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
7. See [:material-code-brackets: InputDeblockFilterType](./literals.md#inputdeblockfiltertype) 
8. See [:material-code-brackets: InputDenoiseFilterType](./literals.md#inputdenoisefiltertype) 
9. See [:material-code-braces: DynamicAudioSelectorTypeDef](./type_defs.md#dynamicaudioselectortypedef) 
10. See [:material-code-brackets: InputFilterEnableType](./literals.md#inputfilterenabletype) 
11. See [:material-code-braces: ImageInserterTypeDef](./type_defs.md#imageinsertertypedef) 
12. See [:material-code-braces: InputClippingTypeDef](./type_defs.md#inputclippingtypedef) 
13. See [:material-code-brackets: InputScanTypeType](./literals.md#inputscantypetype) 
14. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
15. See [:material-code-brackets: InputPsiControlType](./literals.md#inputpsicontroltype) 
16. See [:material-code-brackets: InputTimecodeSourceType](./literals.md#inputtimecodesourcetype) 
17. See [:material-code-braces: VideoOverlayTypeDef](./type_defs.md#videooverlaytypedef) 
18. See [:material-code-braces: VideoSelectorTypeDef](./type_defs.md#videoselectortypedef) 
## InputTypeDef

```python
# InputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import InputTypeDef


def get_value() -> InputTypeDef:
    return {
        "AdvancedInputFilter": ...,
    }


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
    DynamicAudioSelectors: NotRequired[Mapping[str, DynamicAudioSelectorTypeDef]],  # (10)
    FileInput: NotRequired[str],
    FilterEnable: NotRequired[InputFilterEnableType],  # (11)
    FilterStrength: NotRequired[int],
    ImageInserter: NotRequired[ImageInserterTypeDef],  # (12)
    InputClippings: NotRequired[Sequence[InputClippingTypeDef]],  # (13)
    InputScanType: NotRequired[InputScanTypeType],  # (14)
    Position: NotRequired[RectangleTypeDef],  # (6)
    ProgramNumber: NotRequired[int],
    PsiControl: NotRequired[InputPsiControlType],  # (16)
    SupplementalImps: NotRequired[Sequence[str]],
    TimecodeSource: NotRequired[InputTimecodeSourceType],  # (17)
    TimecodeStart: NotRequired[str],
    VideoGenerator: NotRequired[InputVideoGeneratorTypeDef],  # (18)
    VideoOverlays: NotRequired[Sequence[VideoOverlayTypeDef]],  # (19)
    VideoSelector: NotRequired[VideoSelectorTypeDef],  # (20)
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
10. See [:material-code-braces: DynamicAudioSelectorTypeDef](./type_defs.md#dynamicaudioselectortypedef) 
11. See [:material-code-brackets: InputFilterEnableType](./literals.md#inputfilterenabletype) 
12. See [:material-code-braces: ImageInserterTypeDef](./type_defs.md#imageinsertertypedef) 
13. See [:material-code-braces: InputClippingTypeDef](./type_defs.md#inputclippingtypedef) 
14. See [:material-code-brackets: InputScanTypeType](./literals.md#inputscantypetype) 
15. See [:material-code-braces: RectangleTypeDef](./type_defs.md#rectangletypedef) 
16. See [:material-code-brackets: InputPsiControlType](./literals.md#inputpsicontroltype) 
17. See [:material-code-brackets: InputTimecodeSourceType](./literals.md#inputtimecodesourcetype) 
18. See [:material-code-braces: InputVideoGeneratorTypeDef](./type_defs.md#inputvideogeneratortypedef) 
19. See [:material-code-braces: VideoOverlayTypeDef](./type_defs.md#videooverlaytypedef) 
20. See [:material-code-braces: VideoSelectorTypeDef](./type_defs.md#videoselectortypedef) 
## OutputGroupSettingsOutputTypeDef

```python
# OutputGroupSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import OutputGroupSettingsOutputTypeDef


def get_value() -> OutputGroupSettingsOutputTypeDef:
    return {
        "CmafGroupSettings": ...,
    }


# OutputGroupSettingsOutputTypeDef definition

class OutputGroupSettingsOutputTypeDef(TypedDict):
    CmafGroupSettings: NotRequired[CmafGroupSettingsOutputTypeDef],  # (1)
    DashIsoGroupSettings: NotRequired[DashIsoGroupSettingsOutputTypeDef],  # (2)
    FileGroupSettings: NotRequired[FileGroupSettingsTypeDef],  # (3)
    HlsGroupSettings: NotRequired[HlsGroupSettingsOutputTypeDef],  # (4)
    MsSmoothGroupSettings: NotRequired[MsSmoothGroupSettingsOutputTypeDef],  # (5)
    Type: NotRequired[OutputGroupTypeType],  # (6)
```

1. See [:material-code-braces: CmafGroupSettingsOutputTypeDef](./type_defs.md#cmafgroupsettingsoutputtypedef) 
2. See [:material-code-braces: DashIsoGroupSettingsOutputTypeDef](./type_defs.md#dashisogroupsettingsoutputtypedef) 
3. See [:material-code-braces: FileGroupSettingsTypeDef](./type_defs.md#filegroupsettingstypedef) 
4. See [:material-code-braces: HlsGroupSettingsOutputTypeDef](./type_defs.md#hlsgroupsettingsoutputtypedef) 
5. See [:material-code-braces: MsSmoothGroupSettingsOutputTypeDef](./type_defs.md#mssmoothgroupsettingsoutputtypedef) 
6. See [:material-code-brackets: OutputGroupTypeType](./literals.md#outputgrouptypetype) 
## OutputGroupSettingsTypeDef

```python
# OutputGroupSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import OutputGroupSettingsTypeDef


def get_value() -> OutputGroupSettingsTypeDef:
    return {
        "CmafGroupSettings": ...,
    }


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
## ExtraTypeDef

```python
# ExtraTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ExtraTypeDef


def get_value() -> ExtraTypeDef:
    return {
        "AudioDescriptions": ...,
    }


# ExtraTypeDef definition

class ExtraTypeDef(TypedDict):
    AudioDescriptions: NotRequired[List[AudioDescriptionOutputTypeDef]],  # (1)
    CaptionDescriptions: NotRequired[List[CaptionDescriptionOutputTypeDef]],  # (2)
    ContainerSettings: NotRequired[ContainerSettingsOutputTypeDef],  # (3)
    Extension: NotRequired[str],
    NameModifier: NotRequired[str],
    OutputSettings: NotRequired[OutputSettingsTypeDef],  # (4)
    Preset: NotRequired[str],
    VideoDescription: NotRequired[VideoDescriptionOutputTypeDef],  # (5)
```

1. See [:material-code-braces: AudioDescriptionOutputTypeDef](./type_defs.md#audiodescriptionoutputtypedef) 
2. See [:material-code-braces: CaptionDescriptionOutputTypeDef](./type_defs.md#captiondescriptionoutputtypedef) 
3. See [:material-code-braces: ContainerSettingsOutputTypeDef](./type_defs.md#containersettingsoutputtypedef) 
4. See [:material-code-braces: OutputSettingsTypeDef](./type_defs.md#outputsettingstypedef) 
5. See [:material-code-braces: VideoDescriptionOutputTypeDef](./type_defs.md#videodescriptionoutputtypedef) 
## PresetSettingsOutputTypeDef

```python
# PresetSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import PresetSettingsOutputTypeDef


def get_value() -> PresetSettingsOutputTypeDef:
    return {
        "AudioDescriptions": ...,
    }


# PresetSettingsOutputTypeDef definition

class PresetSettingsOutputTypeDef(TypedDict):
    AudioDescriptions: NotRequired[List[AudioDescriptionOutputTypeDef]],  # (1)
    CaptionDescriptions: NotRequired[List[CaptionDescriptionPresetOutputTypeDef]],  # (2)
    ContainerSettings: NotRequired[ContainerSettingsOutputTypeDef],  # (3)
    VideoDescription: NotRequired[VideoDescriptionOutputTypeDef],  # (4)
```

1. See [:material-code-braces: AudioDescriptionOutputTypeDef](./type_defs.md#audiodescriptionoutputtypedef) 
2. See [:material-code-braces: CaptionDescriptionPresetOutputTypeDef](./type_defs.md#captiondescriptionpresetoutputtypedef) 
3. See [:material-code-braces: ContainerSettingsOutputTypeDef](./type_defs.md#containersettingsoutputtypedef) 
4. See [:material-code-braces: VideoDescriptionOutputTypeDef](./type_defs.md#videodescriptionoutputtypedef) 
## OutputTypeDef

```python
# OutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import OutputTypeDef


def get_value() -> OutputTypeDef:
    return {
        "AudioDescriptions": ...,
    }


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
# PresetSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import PresetSettingsTypeDef


def get_value() -> PresetSettingsTypeDef:
    return {
        "AudioDescriptions": ...,
    }


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
## OutputGroupOutputTypeDef

```python
# OutputGroupOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import OutputGroupOutputTypeDef


def get_value() -> OutputGroupOutputTypeDef:
    return {
        "AutomatedEncodingSettings": ...,
    }


# OutputGroupOutputTypeDef definition

class OutputGroupOutputTypeDef(TypedDict):
    AutomatedEncodingSettings: NotRequired[AutomatedEncodingSettingsOutputTypeDef],  # (1)
    CustomName: NotRequired[str],
    Name: NotRequired[str],
    OutputGroupSettings: NotRequired[OutputGroupSettingsOutputTypeDef],  # (2)
    Outputs: NotRequired[List[ExtraTypeDef]],  # (3)
```

1. See [:material-code-braces: AutomatedEncodingSettingsOutputTypeDef](./type_defs.md#automatedencodingsettingsoutputtypedef) 
2. See [:material-code-braces: OutputGroupSettingsOutputTypeDef](./type_defs.md#outputgroupsettingsoutputtypedef) 
3. See [:material-code-braces: ExtraTypeDef](./type_defs.md#extratypedef) 
## PresetTypeDef

```python
# PresetTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import PresetTypeDef


def get_value() -> PresetTypeDef:
    return {
        "Arn": ...,
    }


# PresetTypeDef definition

class PresetTypeDef(TypedDict):
    Name: str,
    Settings: PresetSettingsOutputTypeDef,  # (1)
    Arn: NotRequired[str],
    Category: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Description: NotRequired[str],
    LastUpdated: NotRequired[datetime],
    Type: NotRequired[TypeType],  # (2)
```

1. See [:material-code-braces: PresetSettingsOutputTypeDef](./type_defs.md#presetsettingsoutputtypedef) 
2. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## OutputGroupTypeDef

```python
# OutputGroupTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import OutputGroupTypeDef


def get_value() -> OutputGroupTypeDef:
    return {
        "AutomatedEncodingSettings": ...,
    }


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
## JobSettingsOutputTypeDef

```python
# JobSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import JobSettingsOutputTypeDef


def get_value() -> JobSettingsOutputTypeDef:
    return {
        "AdAvailOffset": ...,
    }


# JobSettingsOutputTypeDef definition

class JobSettingsOutputTypeDef(TypedDict):
    AdAvailOffset: NotRequired[int],
    AvailBlanking: NotRequired[AvailBlankingTypeDef],  # (1)
    ColorConversion3DLUTSettings: NotRequired[List[ColorConversion3DLUTSettingTypeDef]],  # (2)
    Esam: NotRequired[EsamSettingsTypeDef],  # (3)
    ExtendedDataServices: NotRequired[ExtendedDataServicesTypeDef],  # (4)
    FollowSource: NotRequired[int],
    Inputs: NotRequired[List[InputOutputTypeDef]],  # (5)
    KantarWatermark: NotRequired[KantarWatermarkSettingsTypeDef],  # (6)
    MotionImageInserter: NotRequired[MotionImageInserterTypeDef],  # (7)
    NielsenConfiguration: NotRequired[NielsenConfigurationTypeDef],  # (8)
    NielsenNonLinearWatermark: NotRequired[NielsenNonLinearWatermarkSettingsTypeDef],  # (9)
    OutputGroups: NotRequired[List[OutputGroupOutputTypeDef]],  # (10)
    TimecodeConfig: NotRequired[TimecodeConfigTypeDef],  # (11)
    TimedMetadataInsertion: NotRequired[TimedMetadataInsertionOutputTypeDef],  # (12)
```

1. See [:material-code-braces: AvailBlankingTypeDef](./type_defs.md#availblankingtypedef) 
2. See [:material-code-braces: ColorConversion3DLUTSettingTypeDef](./type_defs.md#colorconversion3dlutsettingtypedef) 
3. See [:material-code-braces: EsamSettingsTypeDef](./type_defs.md#esamsettingstypedef) 
4. See [:material-code-braces: ExtendedDataServicesTypeDef](./type_defs.md#extendeddataservicestypedef) 
5. See [:material-code-braces: InputOutputTypeDef](./type_defs.md#inputoutputtypedef) 
6. See [:material-code-braces: KantarWatermarkSettingsTypeDef](./type_defs.md#kantarwatermarksettingstypedef) 
7. See [:material-code-braces: MotionImageInserterTypeDef](./type_defs.md#motionimageinsertertypedef) 
8. See [:material-code-braces: NielsenConfigurationTypeDef](./type_defs.md#nielsenconfigurationtypedef) 
9. See [:material-code-braces: NielsenNonLinearWatermarkSettingsTypeDef](./type_defs.md#nielsennonlinearwatermarksettingstypedef) 
10. See [:material-code-braces: OutputGroupOutputTypeDef](./type_defs.md#outputgroupoutputtypedef) 
11. See [:material-code-braces: TimecodeConfigTypeDef](./type_defs.md#timecodeconfigtypedef) 
12. See [:material-code-braces: TimedMetadataInsertionOutputTypeDef](./type_defs.md#timedmetadatainsertionoutputtypedef) 
## JobTemplateSettingsOutputTypeDef

```python
# JobTemplateSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import JobTemplateSettingsOutputTypeDef


def get_value() -> JobTemplateSettingsOutputTypeDef:
    return {
        "AdAvailOffset": ...,
    }


# JobTemplateSettingsOutputTypeDef definition

class JobTemplateSettingsOutputTypeDef(TypedDict):
    AdAvailOffset: NotRequired[int],
    AvailBlanking: NotRequired[AvailBlankingTypeDef],  # (1)
    ColorConversion3DLUTSettings: NotRequired[List[ColorConversion3DLUTSettingTypeDef]],  # (2)
    Esam: NotRequired[EsamSettingsTypeDef],  # (3)
    ExtendedDataServices: NotRequired[ExtendedDataServicesTypeDef],  # (4)
    FollowSource: NotRequired[int],
    Inputs: NotRequired[List[InputTemplateOutputTypeDef]],  # (5)
    KantarWatermark: NotRequired[KantarWatermarkSettingsTypeDef],  # (6)
    MotionImageInserter: NotRequired[MotionImageInserterTypeDef],  # (7)
    NielsenConfiguration: NotRequired[NielsenConfigurationTypeDef],  # (8)
    NielsenNonLinearWatermark: NotRequired[NielsenNonLinearWatermarkSettingsTypeDef],  # (9)
    OutputGroups: NotRequired[List[OutputGroupOutputTypeDef]],  # (10)
    TimecodeConfig: NotRequired[TimecodeConfigTypeDef],  # (11)
    TimedMetadataInsertion: NotRequired[TimedMetadataInsertionOutputTypeDef],  # (12)
```

1. See [:material-code-braces: AvailBlankingTypeDef](./type_defs.md#availblankingtypedef) 
2. See [:material-code-braces: ColorConversion3DLUTSettingTypeDef](./type_defs.md#colorconversion3dlutsettingtypedef) 
3. See [:material-code-braces: EsamSettingsTypeDef](./type_defs.md#esamsettingstypedef) 
4. See [:material-code-braces: ExtendedDataServicesTypeDef](./type_defs.md#extendeddataservicestypedef) 
5. See [:material-code-braces: InputTemplateOutputTypeDef](./type_defs.md#inputtemplateoutputtypedef) 
6. See [:material-code-braces: KantarWatermarkSettingsTypeDef](./type_defs.md#kantarwatermarksettingstypedef) 
7. See [:material-code-braces: MotionImageInserterTypeDef](./type_defs.md#motionimageinsertertypedef) 
8. See [:material-code-braces: NielsenConfigurationTypeDef](./type_defs.md#nielsenconfigurationtypedef) 
9. See [:material-code-braces: NielsenNonLinearWatermarkSettingsTypeDef](./type_defs.md#nielsennonlinearwatermarksettingstypedef) 
10. See [:material-code-braces: OutputGroupOutputTypeDef](./type_defs.md#outputgroupoutputtypedef) 
11. See [:material-code-braces: TimecodeConfigTypeDef](./type_defs.md#timecodeconfigtypedef) 
12. See [:material-code-braces: TimedMetadataInsertionOutputTypeDef](./type_defs.md#timedmetadatainsertionoutputtypedef) 
## CreatePresetResponseTypeDef

```python
# CreatePresetResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CreatePresetResponseTypeDef


def get_value() -> CreatePresetResponseTypeDef:
    return {
        "Preset": ...,
    }


# CreatePresetResponseTypeDef definition

class CreatePresetResponseTypeDef(TypedDict):
    Preset: PresetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPresetResponseTypeDef

```python
# GetPresetResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import GetPresetResponseTypeDef


def get_value() -> GetPresetResponseTypeDef:
    return {
        "Preset": ...,
    }


# GetPresetResponseTypeDef definition

class GetPresetResponseTypeDef(TypedDict):
    Preset: PresetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPresetsResponseTypeDef

```python
# ListPresetsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListPresetsResponseTypeDef


def get_value() -> ListPresetsResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListPresetsResponseTypeDef definition

class ListPresetsResponseTypeDef(TypedDict):
    Presets: List[PresetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePresetResponseTypeDef

```python
# UpdatePresetResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import UpdatePresetResponseTypeDef


def get_value() -> UpdatePresetResponseTypeDef:
    return {
        "Preset": ...,
    }


# UpdatePresetResponseTypeDef definition

class UpdatePresetResponseTypeDef(TypedDict):
    Preset: PresetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PresetTypeDef](./type_defs.md#presettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobSettingsTypeDef

```python
# JobSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import JobSettingsTypeDef


def get_value() -> JobSettingsTypeDef:
    return {
        "AdAvailOffset": ...,
    }


# JobSettingsTypeDef definition

class JobSettingsTypeDef(TypedDict):
    AdAvailOffset: NotRequired[int],
    AvailBlanking: NotRequired[AvailBlankingTypeDef],  # (1)
    ColorConversion3DLUTSettings: NotRequired[Sequence[ColorConversion3DLUTSettingTypeDef]],  # (2)
    Esam: NotRequired[EsamSettingsTypeDef],  # (3)
    ExtendedDataServices: NotRequired[ExtendedDataServicesTypeDef],  # (4)
    FollowSource: NotRequired[int],
    Inputs: NotRequired[Sequence[InputTypeDef]],  # (5)
    KantarWatermark: NotRequired[KantarWatermarkSettingsTypeDef],  # (6)
    MotionImageInserter: NotRequired[MotionImageInserterTypeDef],  # (7)
    NielsenConfiguration: NotRequired[NielsenConfigurationTypeDef],  # (8)
    NielsenNonLinearWatermark: NotRequired[NielsenNonLinearWatermarkSettingsTypeDef],  # (9)
    OutputGroups: NotRequired[Sequence[OutputGroupTypeDef]],  # (10)
    TimecodeConfig: NotRequired[TimecodeConfigTypeDef],  # (11)
    TimedMetadataInsertion: NotRequired[TimedMetadataInsertionTypeDef],  # (12)
```

1. See [:material-code-braces: AvailBlankingTypeDef](./type_defs.md#availblankingtypedef) 
2. See [:material-code-braces: ColorConversion3DLUTSettingTypeDef](./type_defs.md#colorconversion3dlutsettingtypedef) 
3. See [:material-code-braces: EsamSettingsTypeDef](./type_defs.md#esamsettingstypedef) 
4. See [:material-code-braces: ExtendedDataServicesTypeDef](./type_defs.md#extendeddataservicestypedef) 
5. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
6. See [:material-code-braces: KantarWatermarkSettingsTypeDef](./type_defs.md#kantarwatermarksettingstypedef) 
7. See [:material-code-braces: MotionImageInserterTypeDef](./type_defs.md#motionimageinsertertypedef) 
8. See [:material-code-braces: NielsenConfigurationTypeDef](./type_defs.md#nielsenconfigurationtypedef) 
9. See [:material-code-braces: NielsenNonLinearWatermarkSettingsTypeDef](./type_defs.md#nielsennonlinearwatermarksettingstypedef) 
10. See [:material-code-braces: OutputGroupTypeDef](./type_defs.md#outputgrouptypedef) 
11. See [:material-code-braces: TimecodeConfigTypeDef](./type_defs.md#timecodeconfigtypedef) 
12. See [:material-code-braces: TimedMetadataInsertionTypeDef](./type_defs.md#timedmetadatainsertiontypedef) 
## JobTemplateSettingsTypeDef

```python
# JobTemplateSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import JobTemplateSettingsTypeDef


def get_value() -> JobTemplateSettingsTypeDef:
    return {
        "AdAvailOffset": ...,
    }


# JobTemplateSettingsTypeDef definition

class JobTemplateSettingsTypeDef(TypedDict):
    AdAvailOffset: NotRequired[int],
    AvailBlanking: NotRequired[AvailBlankingTypeDef],  # (1)
    ColorConversion3DLUTSettings: NotRequired[Sequence[ColorConversion3DLUTSettingTypeDef]],  # (2)
    Esam: NotRequired[EsamSettingsTypeDef],  # (3)
    ExtendedDataServices: NotRequired[ExtendedDataServicesTypeDef],  # (4)
    FollowSource: NotRequired[int],
    Inputs: NotRequired[Sequence[InputTemplateTypeDef]],  # (5)
    KantarWatermark: NotRequired[KantarWatermarkSettingsTypeDef],  # (6)
    MotionImageInserter: NotRequired[MotionImageInserterTypeDef],  # (7)
    NielsenConfiguration: NotRequired[NielsenConfigurationTypeDef],  # (8)
    NielsenNonLinearWatermark: NotRequired[NielsenNonLinearWatermarkSettingsTypeDef],  # (9)
    OutputGroups: NotRequired[Sequence[OutputGroupTypeDef]],  # (10)
    TimecodeConfig: NotRequired[TimecodeConfigTypeDef],  # (11)
    TimedMetadataInsertion: NotRequired[TimedMetadataInsertionTypeDef],  # (12)
```

1. See [:material-code-braces: AvailBlankingTypeDef](./type_defs.md#availblankingtypedef) 
2. See [:material-code-braces: ColorConversion3DLUTSettingTypeDef](./type_defs.md#colorconversion3dlutsettingtypedef) 
3. See [:material-code-braces: EsamSettingsTypeDef](./type_defs.md#esamsettingstypedef) 
4. See [:material-code-braces: ExtendedDataServicesTypeDef](./type_defs.md#extendeddataservicestypedef) 
5. See [:material-code-braces: InputTemplateTypeDef](./type_defs.md#inputtemplatetypedef) 
6. See [:material-code-braces: KantarWatermarkSettingsTypeDef](./type_defs.md#kantarwatermarksettingstypedef) 
7. See [:material-code-braces: MotionImageInserterTypeDef](./type_defs.md#motionimageinsertertypedef) 
8. See [:material-code-braces: NielsenConfigurationTypeDef](./type_defs.md#nielsenconfigurationtypedef) 
9. See [:material-code-braces: NielsenNonLinearWatermarkSettingsTypeDef](./type_defs.md#nielsennonlinearwatermarksettingstypedef) 
10. See [:material-code-braces: OutputGroupTypeDef](./type_defs.md#outputgrouptypedef) 
11. See [:material-code-braces: TimecodeConfigTypeDef](./type_defs.md#timecodeconfigtypedef) 
12. See [:material-code-braces: TimedMetadataInsertionTypeDef](./type_defs.md#timedmetadatainsertiontypedef) 
## CreatePresetRequestTypeDef

```python
# CreatePresetRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CreatePresetRequestTypeDef


def get_value() -> CreatePresetRequestTypeDef:
    return {
        "Name": ...,
    }


# CreatePresetRequestTypeDef definition

class CreatePresetRequestTypeDef(TypedDict):
    Name: str,
    Settings: PresetSettingsUnionTypeDef,  # (1)
    Category: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: PresetSettingsTypeDef](./type_defs.md#presetsettingstypedef) [:material-code-braces: PresetSettingsOutputTypeDef](./type_defs.md#presetsettingsoutputtypedef) 
## UpdatePresetRequestTypeDef

```python
# UpdatePresetRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import UpdatePresetRequestTypeDef


def get_value() -> UpdatePresetRequestTypeDef:
    return {
        "Name": ...,
    }


# UpdatePresetRequestTypeDef definition

class UpdatePresetRequestTypeDef(TypedDict):
    Name: str,
    Category: NotRequired[str],
    Description: NotRequired[str],
    Settings: NotRequired[PresetSettingsUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PresetSettingsTypeDef](./type_defs.md#presetsettingstypedef) [:material-code-braces: PresetSettingsOutputTypeDef](./type_defs.md#presetsettingsoutputtypedef) 
## JobTypeDef

```python
# JobTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import JobTypeDef


def get_value() -> JobTypeDef:
    return {
        "AccelerationSettings": ...,
    }


# JobTypeDef definition

class JobTypeDef(TypedDict):
    Role: str,
    Settings: JobSettingsOutputTypeDef,  # (9)
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
    JobEngineVersionRequested: NotRequired[str],
    JobEngineVersionUsed: NotRequired[str],
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
9. See [:material-code-braces: JobSettingsOutputTypeDef](./type_defs.md#jobsettingsoutputtypedef) 
10. See [:material-code-brackets: SimulateReservedQueueType](./literals.md#simulatereservedqueuetype) 
11. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
12. See [:material-code-brackets: StatusUpdateIntervalType](./literals.md#statusupdateintervaltype) 
13. See [:material-code-braces: TimingTypeDef](./type_defs.md#timingtypedef) 
14. See [:material-code-braces: WarningGroupTypeDef](./type_defs.md#warninggrouptypedef) 
## JobTemplateTypeDef

```python
# JobTemplateTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import JobTemplateTypeDef


def get_value() -> JobTemplateTypeDef:
    return {
        "AccelerationSettings": ...,
    }


# JobTemplateTypeDef definition

class JobTemplateTypeDef(TypedDict):
    Name: str,
    Settings: JobTemplateSettingsOutputTypeDef,  # (3)
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
3. See [:material-code-braces: JobTemplateSettingsOutputTypeDef](./type_defs.md#jobtemplatesettingsoutputtypedef) 
4. See [:material-code-brackets: StatusUpdateIntervalType](./literals.md#statusupdateintervaltype) 
5. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## CreateJobResponseTypeDef

```python
# CreateJobResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CreateJobResponseTypeDef


def get_value() -> CreateJobResponseTypeDef:
    return {
        "Job": ...,
    }


# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    Job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobResponseTypeDef

```python
# GetJobResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import GetJobResponseTypeDef


def get_value() -> GetJobResponseTypeDef:
    return {
        "Job": ...,
    }


# GetJobResponseTypeDef definition

class GetJobResponseTypeDef(TypedDict):
    Job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsResponseTypeDef

```python
# ListJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListJobsResponseTypeDef


def get_value() -> ListJobsResponseTypeDef:
    return {
        "Jobs": ...,
    }


# ListJobsResponseTypeDef definition

class ListJobsResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchJobsResponseTypeDef

```python
# SearchJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import SearchJobsResponseTypeDef


def get_value() -> SearchJobsResponseTypeDef:
    return {
        "Jobs": ...,
    }


# SearchJobsResponseTypeDef definition

class SearchJobsResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobTemplateResponseTypeDef

```python
# CreateJobTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CreateJobTemplateResponseTypeDef


def get_value() -> CreateJobTemplateResponseTypeDef:
    return {
        "JobTemplate": ...,
    }


# CreateJobTemplateResponseTypeDef definition

class CreateJobTemplateResponseTypeDef(TypedDict):
    JobTemplate: JobTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTemplateTypeDef](./type_defs.md#jobtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobTemplateResponseTypeDef

```python
# GetJobTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import GetJobTemplateResponseTypeDef


def get_value() -> GetJobTemplateResponseTypeDef:
    return {
        "JobTemplate": ...,
    }


# GetJobTemplateResponseTypeDef definition

class GetJobTemplateResponseTypeDef(TypedDict):
    JobTemplate: JobTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTemplateTypeDef](./type_defs.md#jobtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobTemplatesResponseTypeDef

```python
# ListJobTemplatesResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import ListJobTemplatesResponseTypeDef


def get_value() -> ListJobTemplatesResponseTypeDef:
    return {
        "JobTemplates": ...,
    }


# ListJobTemplatesResponseTypeDef definition

class ListJobTemplatesResponseTypeDef(TypedDict):
    JobTemplates: List[JobTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JobTemplateTypeDef](./type_defs.md#jobtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateJobTemplateResponseTypeDef

```python
# UpdateJobTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import UpdateJobTemplateResponseTypeDef


def get_value() -> UpdateJobTemplateResponseTypeDef:
    return {
        "JobTemplate": ...,
    }


# UpdateJobTemplateResponseTypeDef definition

class UpdateJobTemplateResponseTypeDef(TypedDict):
    JobTemplate: JobTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTemplateTypeDef](./type_defs.md#jobtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobRequestTypeDef

```python
# CreateJobRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CreateJobRequestTypeDef


def get_value() -> CreateJobRequestTypeDef:
    return {
        "Role": ...,
    }


# CreateJobRequestTypeDef definition

class CreateJobRequestTypeDef(TypedDict):
    Role: str,
    Settings: JobSettingsUnionTypeDef,  # (1)
    AccelerationSettings: NotRequired[AccelerationSettingsTypeDef],  # (2)
    BillingTagsSource: NotRequired[BillingTagsSourceType],  # (3)
    ClientRequestToken: NotRequired[str],
    HopDestinations: NotRequired[Sequence[HopDestinationTypeDef]],  # (4)
    JobEngineVersion: NotRequired[str],
    JobTemplate: NotRequired[str],
    Priority: NotRequired[int],
    Queue: NotRequired[str],
    SimulateReservedQueue: NotRequired[SimulateReservedQueueType],  # (5)
    StatusUpdateInterval: NotRequired[StatusUpdateIntervalType],  # (6)
    Tags: NotRequired[Mapping[str, str]],
    UserMetadata: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: JobSettingsTypeDef](./type_defs.md#jobsettingstypedef) [:material-code-braces: JobSettingsOutputTypeDef](./type_defs.md#jobsettingsoutputtypedef) 
2. See [:material-code-braces: AccelerationSettingsTypeDef](./type_defs.md#accelerationsettingstypedef) 
3. See [:material-code-brackets: BillingTagsSourceType](./literals.md#billingtagssourcetype) 
4. See [:material-code-braces: HopDestinationTypeDef](./type_defs.md#hopdestinationtypedef) 
5. See [:material-code-brackets: SimulateReservedQueueType](./literals.md#simulatereservedqueuetype) 
6. See [:material-code-brackets: StatusUpdateIntervalType](./literals.md#statusupdateintervaltype) 
## CreateJobTemplateRequestTypeDef

```python
# CreateJobTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import CreateJobTemplateRequestTypeDef


def get_value() -> CreateJobTemplateRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateJobTemplateRequestTypeDef definition

class CreateJobTemplateRequestTypeDef(TypedDict):
    Name: str,
    Settings: JobTemplateSettingsUnionTypeDef,  # (1)
    AccelerationSettings: NotRequired[AccelerationSettingsTypeDef],  # (2)
    Category: NotRequired[str],
    Description: NotRequired[str],
    HopDestinations: NotRequired[Sequence[HopDestinationTypeDef]],  # (3)
    Priority: NotRequired[int],
    Queue: NotRequired[str],
    StatusUpdateInterval: NotRequired[StatusUpdateIntervalType],  # (4)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: JobTemplateSettingsTypeDef](./type_defs.md#jobtemplatesettingstypedef) [:material-code-braces: JobTemplateSettingsOutputTypeDef](./type_defs.md#jobtemplatesettingsoutputtypedef) 
2. See [:material-code-braces: AccelerationSettingsTypeDef](./type_defs.md#accelerationsettingstypedef) 
3. See [:material-code-braces: HopDestinationTypeDef](./type_defs.md#hopdestinationtypedef) 
4. See [:material-code-brackets: StatusUpdateIntervalType](./literals.md#statusupdateintervaltype) 
## UpdateJobTemplateRequestTypeDef

```python
# UpdateJobTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_mediaconvert.type_defs import UpdateJobTemplateRequestTypeDef


def get_value() -> UpdateJobTemplateRequestTypeDef:
    return {
        "Name": ...,
    }


# UpdateJobTemplateRequestTypeDef definition

class UpdateJobTemplateRequestTypeDef(TypedDict):
    Name: str,
    AccelerationSettings: NotRequired[AccelerationSettingsTypeDef],  # (1)
    Category: NotRequired[str],
    Description: NotRequired[str],
    HopDestinations: NotRequired[Sequence[HopDestinationTypeDef]],  # (2)
    Priority: NotRequired[int],
    Queue: NotRequired[str],
    Settings: NotRequired[JobTemplateSettingsUnionTypeDef],  # (3)
    StatusUpdateInterval: NotRequired[StatusUpdateIntervalType],  # (4)
```

1. See [:material-code-braces: AccelerationSettingsTypeDef](./type_defs.md#accelerationsettingstypedef) 
2. See [:material-code-braces: HopDestinationTypeDef](./type_defs.md#hopdestinationtypedef) 
3. See [:material-code-braces: JobTemplateSettingsTypeDef](./type_defs.md#jobtemplatesettingstypedef) [:material-code-braces: JobTemplateSettingsOutputTypeDef](./type_defs.md#jobtemplatesettingsoutputtypedef) 
4. See [:material-code-brackets: StatusUpdateIntervalType](./literals.md#statusupdateintervaltype) 
