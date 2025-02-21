# Type definitions

> [Index](../README.md) > [MediaTailor](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MediaTailor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#mediatailor)
    type annotations stubs module [types-aiobotocore-mediatailor](https://pypi.org/project/types-aiobotocore-mediatailor/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_mediatailor.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## HlsPlaylistSettingsUnionTypeDef

```python
# HlsPlaylistSettingsUnionTypeDef Union usage example

from types_aiobotocore_mediatailor.type_defs import HlsPlaylistSettingsUnionTypeDef


def get_value() -> HlsPlaylistSettingsUnionTypeDef:
    return ...


# HlsPlaylistSettingsUnionTypeDef definition

HlsPlaylistSettingsUnionTypeDef = Union[
    HlsPlaylistSettingsTypeDef,  # (1)
    HlsPlaylistSettingsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HlsPlaylistSettingsTypeDef](./type_defs.md#hlsplaylistsettingstypedef) 
2. See [:material-code-braces: HlsPlaylistSettingsOutputTypeDef](./type_defs.md#hlsplaylistsettingsoutputtypedef) 

## PrefetchConsumptionUnionTypeDef

```python
# PrefetchConsumptionUnionTypeDef Union usage example

from types_aiobotocore_mediatailor.type_defs import PrefetchConsumptionUnionTypeDef


def get_value() -> PrefetchConsumptionUnionTypeDef:
    return ...


# PrefetchConsumptionUnionTypeDef definition

PrefetchConsumptionUnionTypeDef = Union[
    PrefetchConsumptionTypeDef,  # (1)
    PrefetchConsumptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PrefetchConsumptionTypeDef](./type_defs.md#prefetchconsumptiontypedef) 
2. See [:material-code-braces: PrefetchConsumptionOutputTypeDef](./type_defs.md#prefetchconsumptionoutputtypedef) 

## PrefetchRetrievalUnionTypeDef

```python
# PrefetchRetrievalUnionTypeDef Union usage example

from types_aiobotocore_mediatailor.type_defs import PrefetchRetrievalUnionTypeDef


def get_value() -> PrefetchRetrievalUnionTypeDef:
    return ...


# PrefetchRetrievalUnionTypeDef definition

PrefetchRetrievalUnionTypeDef = Union[
    PrefetchRetrievalTypeDef,  # (1)
    PrefetchRetrievalOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PrefetchRetrievalTypeDef](./type_defs.md#prefetchretrievaltypedef) 
2. See [:material-code-braces: PrefetchRetrievalOutputTypeDef](./type_defs.md#prefetchretrievaloutputtypedef) 

## TimeSignalMessageUnionTypeDef

```python
# TimeSignalMessageUnionTypeDef Union usage example

from types_aiobotocore_mediatailor.type_defs import TimeSignalMessageUnionTypeDef


def get_value() -> TimeSignalMessageUnionTypeDef:
    return ...


# TimeSignalMessageUnionTypeDef definition

TimeSignalMessageUnionTypeDef = Union[
    TimeSignalMessageTypeDef,  # (1)
    TimeSignalMessageOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TimeSignalMessageTypeDef](./type_defs.md#timesignalmessagetypedef) 
2. See [:material-code-braces: TimeSignalMessageOutputTypeDef](./type_defs.md#timesignalmessageoutputtypedef) 

## AdBreakUnionTypeDef

```python
# AdBreakUnionTypeDef Union usage example

from types_aiobotocore_mediatailor.type_defs import AdBreakUnionTypeDef


def get_value() -> AdBreakUnionTypeDef:
    return ...


# AdBreakUnionTypeDef definition

AdBreakUnionTypeDef = Union[
    AdBreakTypeDef,  # (1)
    AdBreakOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AdBreakTypeDef](./type_defs.md#adbreaktypedef) 
2. See [:material-code-braces: AdBreakOutputTypeDef](./type_defs.md#adbreakoutputtypedef) 

## AlternateMediaUnionTypeDef

```python
# AlternateMediaUnionTypeDef Union usage example

from types_aiobotocore_mediatailor.type_defs import AlternateMediaUnionTypeDef


def get_value() -> AlternateMediaUnionTypeDef:
    return ...


# AlternateMediaUnionTypeDef definition

AlternateMediaUnionTypeDef = Union[
    AlternateMediaTypeDef,  # (1)
    AlternateMediaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AlternateMediaTypeDef](./type_defs.md#alternatemediatypedef) 
2. See [:material-code-braces: AlternateMediaOutputTypeDef](./type_defs.md#alternatemediaoutputtypedef) 

## AudienceMediaUnionTypeDef

```python
# AudienceMediaUnionTypeDef Union usage example

from types_aiobotocore_mediatailor.type_defs import AudienceMediaUnionTypeDef


def get_value() -> AudienceMediaUnionTypeDef:
    return ...


# AudienceMediaUnionTypeDef definition

AudienceMediaUnionTypeDef = Union[
    AudienceMediaTypeDef,  # (1)
    AudienceMediaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AudienceMediaTypeDef](./type_defs.md#audiencemediatypedef) 
2. See [:material-code-braces: AudienceMediaOutputTypeDef](./type_defs.md#audiencemediaoutputtypedef) 



## SecretsManagerAccessTokenConfigurationTypeDef

```python
# SecretsManagerAccessTokenConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import SecretsManagerAccessTokenConfigurationTypeDef


def get_value() -> SecretsManagerAccessTokenConfigurationTypeDef:
    return {
        "HeaderName": ...,
    }


# SecretsManagerAccessTokenConfigurationTypeDef definition

class SecretsManagerAccessTokenConfigurationTypeDef(TypedDict):
    HeaderName: NotRequired[str],
    SecretArn: NotRequired[str],
    SecretStringKey: NotRequired[str],
```

## AdBreakOpportunityTypeDef

```python
# AdBreakOpportunityTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AdBreakOpportunityTypeDef


def get_value() -> AdBreakOpportunityTypeDef:
    return {
        "OffsetMillis": ...,
    }


# AdBreakOpportunityTypeDef definition

class AdBreakOpportunityTypeDef(TypedDict):
    OffsetMillis: int,
```

## KeyValuePairTypeDef

```python
# KeyValuePairTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import KeyValuePairTypeDef


def get_value() -> KeyValuePairTypeDef:
    return {
        "Key": ...,
    }


# KeyValuePairTypeDef definition

class KeyValuePairTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## SlateSourceTypeDef

```python
# SlateSourceTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import SlateSourceTypeDef


def get_value() -> SlateSourceTypeDef:
    return {
        "SourceLocationName": ...,
    }


# SlateSourceTypeDef definition

class SlateSourceTypeDef(TypedDict):
    SourceLocationName: NotRequired[str],
    VodSourceName: NotRequired[str],
```

## SpliceInsertMessageTypeDef

```python
# SpliceInsertMessageTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import SpliceInsertMessageTypeDef


def get_value() -> SpliceInsertMessageTypeDef:
    return {
        "AvailNum": ...,
    }


# SpliceInsertMessageTypeDef definition

class SpliceInsertMessageTypeDef(TypedDict):
    AvailNum: NotRequired[int],
    AvailsExpected: NotRequired[int],
    SpliceEventId: NotRequired[int],
    UniqueProgramId: NotRequired[int],
```

## AdConditioningConfigurationTypeDef

```python
# AdConditioningConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AdConditioningConfigurationTypeDef


def get_value() -> AdConditioningConfigurationTypeDef:
    return {
        "StreamingMediaFileConditioning": ...,
    }


# AdConditioningConfigurationTypeDef definition

class AdConditioningConfigurationTypeDef(TypedDict):
    StreamingMediaFileConditioning: StreamingMediaFileConditioningType,  # (1)
```

1. See [:material-code-brackets: StreamingMediaFileConditioningType](./literals.md#streamingmediafileconditioningtype) 
## AdMarkerPassthroughTypeDef

```python
# AdMarkerPassthroughTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AdMarkerPassthroughTypeDef


def get_value() -> AdMarkerPassthroughTypeDef:
    return {
        "Enabled": ...,
    }


# AdMarkerPassthroughTypeDef definition

class AdMarkerPassthroughTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## AlertTypeDef

```python
# AlertTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AlertTypeDef


def get_value() -> AlertTypeDef:
    return {
        "AlertCode": ...,
    }


# AlertTypeDef definition

class AlertTypeDef(TypedDict):
    AlertCode: str,
    AlertMessage: str,
    LastModifiedTime: datetime,
    RelatedResourceArns: List[str],
    ResourceArn: str,
    Category: NotRequired[AlertCategoryType],  # (1)
```

1. See [:material-code-brackets: AlertCategoryType](./literals.md#alertcategorytype) 
## ClipRangeTypeDef

```python
# ClipRangeTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ClipRangeTypeDef


def get_value() -> ClipRangeTypeDef:
    return {
        "EndOffsetMillis": ...,
    }


# ClipRangeTypeDef definition

class ClipRangeTypeDef(TypedDict):
    EndOffsetMillis: NotRequired[int],
    StartOffsetMillis: NotRequired[int],
```

## AvailMatchingCriteriaTypeDef

```python
# AvailMatchingCriteriaTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AvailMatchingCriteriaTypeDef


def get_value() -> AvailMatchingCriteriaTypeDef:
    return {
        "DynamicVariable": ...,
    }


# AvailMatchingCriteriaTypeDef definition

class AvailMatchingCriteriaTypeDef(TypedDict):
    DynamicVariable: str,
    Operator: OperatorType,  # (1)
```

1. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## AvailSuppressionTypeDef

```python
# AvailSuppressionTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AvailSuppressionTypeDef


def get_value() -> AvailSuppressionTypeDef:
    return {
        "Mode": ...,
    }


# AvailSuppressionTypeDef definition

class AvailSuppressionTypeDef(TypedDict):
    Mode: NotRequired[ModeType],  # (1)
    Value: NotRequired[str],
    FillPolicy: NotRequired[FillPolicyType],  # (2)
```

1. See [:material-code-brackets: ModeType](./literals.md#modetype) 
2. See [:material-code-brackets: FillPolicyType](./literals.md#fillpolicytype) 
## BumperTypeDef

```python
# BumperTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import BumperTypeDef


def get_value() -> BumperTypeDef:
    return {
        "EndUrl": ...,
    }


# BumperTypeDef definition

class BumperTypeDef(TypedDict):
    EndUrl: NotRequired[str],
    StartUrl: NotRequired[str],
```

## CdnConfigurationTypeDef

```python
# CdnConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CdnConfigurationTypeDef


def get_value() -> CdnConfigurationTypeDef:
    return {
        "AdSegmentUrlPrefix": ...,
    }


# CdnConfigurationTypeDef definition

class CdnConfigurationTypeDef(TypedDict):
    AdSegmentUrlPrefix: NotRequired[str],
    ContentSegmentUrlPrefix: NotRequired[str],
```

## LogConfigurationForChannelTypeDef

```python
# LogConfigurationForChannelTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import LogConfigurationForChannelTypeDef


def get_value() -> LogConfigurationForChannelTypeDef:
    return {
        "LogTypes": ...,
    }


# LogConfigurationForChannelTypeDef definition

class LogConfigurationForChannelTypeDef(TypedDict):
    LogTypes: NotRequired[List[LogTypeType]],  # (1)
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
## ConfigureLogsForChannelRequestTypeDef

```python
# ConfigureLogsForChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ConfigureLogsForChannelRequestTypeDef


def get_value() -> ConfigureLogsForChannelRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# ConfigureLogsForChannelRequestTypeDef definition

class ConfigureLogsForChannelRequestTypeDef(TypedDict):
    ChannelName: str,
    LogTypes: Sequence[LogTypeType],  # (1)
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ResponseMetadataTypeDef


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

## ConfigureLogsForPlaybackConfigurationRequestTypeDef

```python
# ConfigureLogsForPlaybackConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ConfigureLogsForPlaybackConfigurationRequestTypeDef


def get_value() -> ConfigureLogsForPlaybackConfigurationRequestTypeDef:
    return {
        "PercentEnabled": ...,
    }


# ConfigureLogsForPlaybackConfigurationRequestTypeDef definition

class ConfigureLogsForPlaybackConfigurationRequestTypeDef(TypedDict):
    PercentEnabled: int,
    PlaybackConfigurationName: str,
    EnabledLoggingStrategies: NotRequired[Sequence[LoggingStrategyType]],  # (1)
```

1. See [:material-code-brackets: LoggingStrategyType](./literals.md#loggingstrategytype) 
## TimeShiftConfigurationTypeDef

```python
# TimeShiftConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import TimeShiftConfigurationTypeDef


def get_value() -> TimeShiftConfigurationTypeDef:
    return {
        "MaxTimeDelaySeconds": ...,
    }


# TimeShiftConfigurationTypeDef definition

class TimeShiftConfigurationTypeDef(TypedDict):
    MaxTimeDelaySeconds: int,
```

## HttpPackageConfigurationTypeDef

```python
# HttpPackageConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import HttpPackageConfigurationTypeDef


def get_value() -> HttpPackageConfigurationTypeDef:
    return {
        "Path": ...,
    }


# HttpPackageConfigurationTypeDef definition

class HttpPackageConfigurationTypeDef(TypedDict):
    Path: str,
    SourceGroup: str,
    Type: TypeType,  # (1)
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## PrefetchRetrievalOutputTypeDef

```python
# PrefetchRetrievalOutputTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import PrefetchRetrievalOutputTypeDef


def get_value() -> PrefetchRetrievalOutputTypeDef:
    return {
        "DynamicVariables": ...,
    }


# PrefetchRetrievalOutputTypeDef definition

class PrefetchRetrievalOutputTypeDef(TypedDict):
    EndTime: datetime,
    DynamicVariables: NotRequired[Dict[str, str]],
    StartTime: NotRequired[datetime],
```

## DefaultSegmentDeliveryConfigurationTypeDef

```python
# DefaultSegmentDeliveryConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DefaultSegmentDeliveryConfigurationTypeDef


def get_value() -> DefaultSegmentDeliveryConfigurationTypeDef:
    return {
        "BaseUrl": ...,
    }


# DefaultSegmentDeliveryConfigurationTypeDef definition

class DefaultSegmentDeliveryConfigurationTypeDef(TypedDict):
    BaseUrl: NotRequired[str],
```

## HttpConfigurationTypeDef

```python
# HttpConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import HttpConfigurationTypeDef


def get_value() -> HttpConfigurationTypeDef:
    return {
        "BaseUrl": ...,
    }


# HttpConfigurationTypeDef definition

class HttpConfigurationTypeDef(TypedDict):
    BaseUrl: str,
```

## SegmentDeliveryConfigurationTypeDef

```python
# SegmentDeliveryConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import SegmentDeliveryConfigurationTypeDef


def get_value() -> SegmentDeliveryConfigurationTypeDef:
    return {
        "BaseUrl": ...,
    }


# SegmentDeliveryConfigurationTypeDef definition

class SegmentDeliveryConfigurationTypeDef(TypedDict):
    BaseUrl: NotRequired[str],
    Name: NotRequired[str],
```

## DashConfigurationForPutTypeDef

```python
# DashConfigurationForPutTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DashConfigurationForPutTypeDef


def get_value() -> DashConfigurationForPutTypeDef:
    return {
        "MpdLocation": ...,
    }


# DashConfigurationForPutTypeDef definition

class DashConfigurationForPutTypeDef(TypedDict):
    MpdLocation: NotRequired[str],
    OriginManifestType: NotRequired[OriginManifestTypeType],  # (1)
```

1. See [:material-code-brackets: OriginManifestTypeType](./literals.md#originmanifesttypetype) 
## DashConfigurationTypeDef

```python
# DashConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DashConfigurationTypeDef


def get_value() -> DashConfigurationTypeDef:
    return {
        "ManifestEndpointPrefix": ...,
    }


# DashConfigurationTypeDef definition

class DashConfigurationTypeDef(TypedDict):
    ManifestEndpointPrefix: NotRequired[str],
    MpdLocation: NotRequired[str],
    OriginManifestType: NotRequired[OriginManifestTypeType],  # (1)
```

1. See [:material-code-brackets: OriginManifestTypeType](./literals.md#originmanifesttypetype) 
## DashPlaylistSettingsTypeDef

```python
# DashPlaylistSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DashPlaylistSettingsTypeDef


def get_value() -> DashPlaylistSettingsTypeDef:
    return {
        "ManifestWindowSeconds": ...,
    }


# DashPlaylistSettingsTypeDef definition

class DashPlaylistSettingsTypeDef(TypedDict):
    ManifestWindowSeconds: NotRequired[int],
    MinBufferTimeSeconds: NotRequired[int],
    MinUpdatePeriodSeconds: NotRequired[int],
    SuggestedPresentationDelaySeconds: NotRequired[int],
```

## DeleteChannelPolicyRequestTypeDef

```python
# DeleteChannelPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DeleteChannelPolicyRequestTypeDef


def get_value() -> DeleteChannelPolicyRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# DeleteChannelPolicyRequestTypeDef definition

class DeleteChannelPolicyRequestTypeDef(TypedDict):
    ChannelName: str,
```

## DeleteChannelRequestTypeDef

```python
# DeleteChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DeleteChannelRequestTypeDef


def get_value() -> DeleteChannelRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# DeleteChannelRequestTypeDef definition

class DeleteChannelRequestTypeDef(TypedDict):
    ChannelName: str,
```

## DeleteLiveSourceRequestTypeDef

```python
# DeleteLiveSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DeleteLiveSourceRequestTypeDef


def get_value() -> DeleteLiveSourceRequestTypeDef:
    return {
        "LiveSourceName": ...,
    }


# DeleteLiveSourceRequestTypeDef definition

class DeleteLiveSourceRequestTypeDef(TypedDict):
    LiveSourceName: str,
    SourceLocationName: str,
```

## DeletePlaybackConfigurationRequestTypeDef

```python
# DeletePlaybackConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DeletePlaybackConfigurationRequestTypeDef


def get_value() -> DeletePlaybackConfigurationRequestTypeDef:
    return {
        "Name": ...,
    }


# DeletePlaybackConfigurationRequestTypeDef definition

class DeletePlaybackConfigurationRequestTypeDef(TypedDict):
    Name: str,
```

## DeletePrefetchScheduleRequestTypeDef

```python
# DeletePrefetchScheduleRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DeletePrefetchScheduleRequestTypeDef


def get_value() -> DeletePrefetchScheduleRequestTypeDef:
    return {
        "Name": ...,
    }


# DeletePrefetchScheduleRequestTypeDef definition

class DeletePrefetchScheduleRequestTypeDef(TypedDict):
    Name: str,
    PlaybackConfigurationName: str,
```

## DeleteProgramRequestTypeDef

```python
# DeleteProgramRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DeleteProgramRequestTypeDef


def get_value() -> DeleteProgramRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# DeleteProgramRequestTypeDef definition

class DeleteProgramRequestTypeDef(TypedDict):
    ChannelName: str,
    ProgramName: str,
```

## DeleteSourceLocationRequestTypeDef

```python
# DeleteSourceLocationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DeleteSourceLocationRequestTypeDef


def get_value() -> DeleteSourceLocationRequestTypeDef:
    return {
        "SourceLocationName": ...,
    }


# DeleteSourceLocationRequestTypeDef definition

class DeleteSourceLocationRequestTypeDef(TypedDict):
    SourceLocationName: str,
```

## DeleteVodSourceRequestTypeDef

```python
# DeleteVodSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DeleteVodSourceRequestTypeDef


def get_value() -> DeleteVodSourceRequestTypeDef:
    return {
        "SourceLocationName": ...,
    }


# DeleteVodSourceRequestTypeDef definition

class DeleteVodSourceRequestTypeDef(TypedDict):
    SourceLocationName: str,
    VodSourceName: str,
```

## DescribeChannelRequestTypeDef

```python
# DescribeChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DescribeChannelRequestTypeDef


def get_value() -> DescribeChannelRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# DescribeChannelRequestTypeDef definition

class DescribeChannelRequestTypeDef(TypedDict):
    ChannelName: str,
```

## DescribeLiveSourceRequestTypeDef

```python
# DescribeLiveSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DescribeLiveSourceRequestTypeDef


def get_value() -> DescribeLiveSourceRequestTypeDef:
    return {
        "LiveSourceName": ...,
    }


# DescribeLiveSourceRequestTypeDef definition

class DescribeLiveSourceRequestTypeDef(TypedDict):
    LiveSourceName: str,
    SourceLocationName: str,
```

## DescribeProgramRequestTypeDef

```python
# DescribeProgramRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DescribeProgramRequestTypeDef


def get_value() -> DescribeProgramRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# DescribeProgramRequestTypeDef definition

class DescribeProgramRequestTypeDef(TypedDict):
    ChannelName: str,
    ProgramName: str,
```

## DescribeSourceLocationRequestTypeDef

```python
# DescribeSourceLocationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DescribeSourceLocationRequestTypeDef


def get_value() -> DescribeSourceLocationRequestTypeDef:
    return {
        "SourceLocationName": ...,
    }


# DescribeSourceLocationRequestTypeDef definition

class DescribeSourceLocationRequestTypeDef(TypedDict):
    SourceLocationName: str,
```

## DescribeVodSourceRequestTypeDef

```python
# DescribeVodSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DescribeVodSourceRequestTypeDef


def get_value() -> DescribeVodSourceRequestTypeDef:
    return {
        "SourceLocationName": ...,
    }


# DescribeVodSourceRequestTypeDef definition

class DescribeVodSourceRequestTypeDef(TypedDict):
    SourceLocationName: str,
    VodSourceName: str,
```

## GetChannelPolicyRequestTypeDef

```python
# GetChannelPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import GetChannelPolicyRequestTypeDef


def get_value() -> GetChannelPolicyRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# GetChannelPolicyRequestTypeDef definition

class GetChannelPolicyRequestTypeDef(TypedDict):
    ChannelName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import PaginatorConfigTypeDef


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

## GetChannelScheduleRequestTypeDef

```python
# GetChannelScheduleRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import GetChannelScheduleRequestTypeDef


def get_value() -> GetChannelScheduleRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# GetChannelScheduleRequestTypeDef definition

class GetChannelScheduleRequestTypeDef(TypedDict):
    ChannelName: str,
    DurationMinutes: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Audience: NotRequired[str],
```

## GetPlaybackConfigurationRequestTypeDef

```python
# GetPlaybackConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import GetPlaybackConfigurationRequestTypeDef


def get_value() -> GetPlaybackConfigurationRequestTypeDef:
    return {
        "Name": ...,
    }


# GetPlaybackConfigurationRequestTypeDef definition

class GetPlaybackConfigurationRequestTypeDef(TypedDict):
    Name: str,
```

## HlsConfigurationTypeDef

```python
# HlsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import HlsConfigurationTypeDef


def get_value() -> HlsConfigurationTypeDef:
    return {
        "ManifestEndpointPrefix": ...,
    }


# HlsConfigurationTypeDef definition

class HlsConfigurationTypeDef(TypedDict):
    ManifestEndpointPrefix: NotRequired[str],
```

## LivePreRollConfigurationTypeDef

```python
# LivePreRollConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import LivePreRollConfigurationTypeDef


def get_value() -> LivePreRollConfigurationTypeDef:
    return {
        "AdDecisionServerUrl": ...,
    }


# LivePreRollConfigurationTypeDef definition

class LivePreRollConfigurationTypeDef(TypedDict):
    AdDecisionServerUrl: NotRequired[str],
    MaxDurationSeconds: NotRequired[int],
```

## LogConfigurationTypeDef

```python
# LogConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import LogConfigurationTypeDef


def get_value() -> LogConfigurationTypeDef:
    return {
        "PercentEnabled": ...,
    }


# LogConfigurationTypeDef definition

class LogConfigurationTypeDef(TypedDict):
    PercentEnabled: int,
    EnabledLoggingStrategies: NotRequired[List[LoggingStrategyType]],  # (1)
```

1. See [:material-code-brackets: LoggingStrategyType](./literals.md#loggingstrategytype) 
## GetPrefetchScheduleRequestTypeDef

```python
# GetPrefetchScheduleRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import GetPrefetchScheduleRequestTypeDef


def get_value() -> GetPrefetchScheduleRequestTypeDef:
    return {
        "Name": ...,
    }


# GetPrefetchScheduleRequestTypeDef definition

class GetPrefetchScheduleRequestTypeDef(TypedDict):
    Name: str,
    PlaybackConfigurationName: str,
```

## HlsPlaylistSettingsOutputTypeDef

```python
# HlsPlaylistSettingsOutputTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import HlsPlaylistSettingsOutputTypeDef


def get_value() -> HlsPlaylistSettingsOutputTypeDef:
    return {
        "ManifestWindowSeconds": ...,
    }


# HlsPlaylistSettingsOutputTypeDef definition

class HlsPlaylistSettingsOutputTypeDef(TypedDict):
    ManifestWindowSeconds: NotRequired[int],
    AdMarkupType: NotRequired[List[AdMarkupTypeType]],  # (1)
```

1. See [:material-code-brackets: AdMarkupTypeType](./literals.md#admarkuptypetype) 
## HlsPlaylistSettingsTypeDef

```python
# HlsPlaylistSettingsTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import HlsPlaylistSettingsTypeDef


def get_value() -> HlsPlaylistSettingsTypeDef:
    return {
        "ManifestWindowSeconds": ...,
    }


# HlsPlaylistSettingsTypeDef definition

class HlsPlaylistSettingsTypeDef(TypedDict):
    ManifestWindowSeconds: NotRequired[int],
    AdMarkupType: NotRequired[Sequence[AdMarkupTypeType]],  # (1)
```

1. See [:material-code-brackets: AdMarkupTypeType](./literals.md#admarkuptypetype) 
## ListAlertsRequestTypeDef

```python
# ListAlertsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListAlertsRequestTypeDef


def get_value() -> ListAlertsRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListAlertsRequestTypeDef definition

class ListAlertsRequestTypeDef(TypedDict):
    ResourceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListChannelsRequestTypeDef

```python
# ListChannelsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListChannelsRequestTypeDef


def get_value() -> ListChannelsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListChannelsRequestTypeDef definition

class ListChannelsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListLiveSourcesRequestTypeDef

```python
# ListLiveSourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListLiveSourcesRequestTypeDef


def get_value() -> ListLiveSourcesRequestTypeDef:
    return {
        "SourceLocationName": ...,
    }


# ListLiveSourcesRequestTypeDef definition

class ListLiveSourcesRequestTypeDef(TypedDict):
    SourceLocationName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListPlaybackConfigurationsRequestTypeDef

```python
# ListPlaybackConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListPlaybackConfigurationsRequestTypeDef


def get_value() -> ListPlaybackConfigurationsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListPlaybackConfigurationsRequestTypeDef definition

class ListPlaybackConfigurationsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListPrefetchSchedulesRequestTypeDef

```python
# ListPrefetchSchedulesRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListPrefetchSchedulesRequestTypeDef


def get_value() -> ListPrefetchSchedulesRequestTypeDef:
    return {
        "PlaybackConfigurationName": ...,
    }


# ListPrefetchSchedulesRequestTypeDef definition

class ListPrefetchSchedulesRequestTypeDef(TypedDict):
    PlaybackConfigurationName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    StreamId: NotRequired[str],
```

## ListSourceLocationsRequestTypeDef

```python
# ListSourceLocationsRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListSourceLocationsRequestTypeDef


def get_value() -> ListSourceLocationsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListSourceLocationsRequestTypeDef definition

class ListSourceLocationsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListVodSourcesRequestTypeDef

```python
# ListVodSourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListVodSourcesRequestTypeDef


def get_value() -> ListVodSourcesRequestTypeDef:
    return {
        "SourceLocationName": ...,
    }


# ListVodSourcesRequestTypeDef definition

class ListVodSourcesRequestTypeDef(TypedDict):
    SourceLocationName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PutChannelPolicyRequestTypeDef

```python
# PutChannelPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import PutChannelPolicyRequestTypeDef


def get_value() -> PutChannelPolicyRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# PutChannelPolicyRequestTypeDef definition

class PutChannelPolicyRequestTypeDef(TypedDict):
    ChannelName: str,
    Policy: str,
```

## ScheduleAdBreakTypeDef

```python
# ScheduleAdBreakTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ScheduleAdBreakTypeDef


def get_value() -> ScheduleAdBreakTypeDef:
    return {
        "ApproximateDurationSeconds": ...,
    }


# ScheduleAdBreakTypeDef definition

class ScheduleAdBreakTypeDef(TypedDict):
    ApproximateDurationSeconds: NotRequired[int],
    ApproximateStartTime: NotRequired[datetime],
    SourceLocationName: NotRequired[str],
    VodSourceName: NotRequired[str],
```

## TransitionTypeDef

```python
# TransitionTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import TransitionTypeDef


def get_value() -> TransitionTypeDef:
    return {
        "DurationMillis": ...,
    }


# TransitionTypeDef definition

class TransitionTypeDef(TypedDict):
    RelativePosition: RelativePositionType,  # (1)
    Type: str,
    DurationMillis: NotRequired[int],
    RelativeProgram: NotRequired[str],
    ScheduledStartTimeMillis: NotRequired[int],
```

1. See [:material-code-brackets: RelativePositionType](./literals.md#relativepositiontype) 
## SegmentationDescriptorTypeDef

```python
# SegmentationDescriptorTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import SegmentationDescriptorTypeDef


def get_value() -> SegmentationDescriptorTypeDef:
    return {
        "SegmentationEventId": ...,
    }


# SegmentationDescriptorTypeDef definition

class SegmentationDescriptorTypeDef(TypedDict):
    SegmentationEventId: NotRequired[int],
    SegmentationUpidType: NotRequired[int],
    SegmentationUpid: NotRequired[str],
    SegmentationTypeId: NotRequired[int],
    SegmentNum: NotRequired[int],
    SegmentsExpected: NotRequired[int],
    SubSegmentNum: NotRequired[int],
    SubSegmentsExpected: NotRequired[int],
```

## StartChannelRequestTypeDef

```python
# StartChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import StartChannelRequestTypeDef


def get_value() -> StartChannelRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# StartChannelRequestTypeDef definition

class StartChannelRequestTypeDef(TypedDict):
    ChannelName: str,
```

## StopChannelRequestTypeDef

```python
# StopChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import StopChannelRequestTypeDef


def get_value() -> StopChannelRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# StopChannelRequestTypeDef definition

class StopChannelRequestTypeDef(TypedDict):
    ChannelName: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateProgramTransitionTypeDef

```python
# UpdateProgramTransitionTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateProgramTransitionTypeDef


def get_value() -> UpdateProgramTransitionTypeDef:
    return {
        "ScheduledStartTimeMillis": ...,
    }


# UpdateProgramTransitionTypeDef definition

class UpdateProgramTransitionTypeDef(TypedDict):
    ScheduledStartTimeMillis: NotRequired[int],
    DurationMillis: NotRequired[int],
```

## AccessConfigurationTypeDef

```python
# AccessConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AccessConfigurationTypeDef


def get_value() -> AccessConfigurationTypeDef:
    return {
        "AccessType": ...,
    }


# AccessConfigurationTypeDef definition

class AccessConfigurationTypeDef(TypedDict):
    AccessType: NotRequired[AccessTypeType],  # (1)
    SecretsManagerAccessTokenConfiguration: NotRequired[SecretsManagerAccessTokenConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: AccessTypeType](./literals.md#accesstypetype) 
2. See [:material-code-braces: SecretsManagerAccessTokenConfigurationTypeDef](./type_defs.md#secretsmanageraccesstokenconfigurationtypedef) 
## ManifestProcessingRulesTypeDef

```python
# ManifestProcessingRulesTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ManifestProcessingRulesTypeDef


def get_value() -> ManifestProcessingRulesTypeDef:
    return {
        "AdMarkerPassthrough": ...,
    }


# ManifestProcessingRulesTypeDef definition

class ManifestProcessingRulesTypeDef(TypedDict):
    AdMarkerPassthrough: NotRequired[AdMarkerPassthroughTypeDef],  # (1)
```

1. See [:material-code-braces: AdMarkerPassthroughTypeDef](./type_defs.md#admarkerpassthroughtypedef) 
## PrefetchConsumptionOutputTypeDef

```python
# PrefetchConsumptionOutputTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import PrefetchConsumptionOutputTypeDef


def get_value() -> PrefetchConsumptionOutputTypeDef:
    return {
        "AvailMatchingCriteria": ...,
    }


# PrefetchConsumptionOutputTypeDef definition

class PrefetchConsumptionOutputTypeDef(TypedDict):
    EndTime: datetime,
    AvailMatchingCriteria: NotRequired[List[AvailMatchingCriteriaTypeDef]],  # (1)
    StartTime: NotRequired[datetime],
```

1. See [:material-code-braces: AvailMatchingCriteriaTypeDef](./type_defs.md#availmatchingcriteriatypedef) 
## ConfigureLogsForChannelResponseTypeDef

```python
# ConfigureLogsForChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ConfigureLogsForChannelResponseTypeDef


def get_value() -> ConfigureLogsForChannelResponseTypeDef:
    return {
        "ChannelName": ...,
    }


# ConfigureLogsForChannelResponseTypeDef definition

class ConfigureLogsForChannelResponseTypeDef(TypedDict):
    ChannelName: str,
    LogTypes: List[LogTypeType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigureLogsForPlaybackConfigurationResponseTypeDef

```python
# ConfigureLogsForPlaybackConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ConfigureLogsForPlaybackConfigurationResponseTypeDef


def get_value() -> ConfigureLogsForPlaybackConfigurationResponseTypeDef:
    return {
        "PercentEnabled": ...,
    }


# ConfigureLogsForPlaybackConfigurationResponseTypeDef definition

class ConfigureLogsForPlaybackConfigurationResponseTypeDef(TypedDict):
    PercentEnabled: int,
    PlaybackConfigurationName: str,
    EnabledLoggingStrategies: List[LoggingStrategyType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LoggingStrategyType](./literals.md#loggingstrategytype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChannelPolicyResponseTypeDef

```python
# GetChannelPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import GetChannelPolicyResponseTypeDef


def get_value() -> GetChannelPolicyResponseTypeDef:
    return {
        "Policy": ...,
    }


# GetChannelPolicyResponseTypeDef definition

class GetChannelPolicyResponseTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAlertsResponseTypeDef

```python
# ListAlertsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListAlertsResponseTypeDef


def get_value() -> ListAlertsResponseTypeDef:
    return {
        "Items": ...,
    }


# ListAlertsResponseTypeDef definition

class ListAlertsResponseTypeDef(TypedDict):
    Items: List[AlertTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AlertTypeDef](./type_defs.md#alerttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLiveSourceRequestTypeDef

```python
# CreateLiveSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreateLiveSourceRequestTypeDef


def get_value() -> CreateLiveSourceRequestTypeDef:
    return {
        "HttpPackageConfigurations": ...,
    }


# CreateLiveSourceRequestTypeDef definition

class CreateLiveSourceRequestTypeDef(TypedDict):
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    LiveSourceName: str,
    SourceLocationName: str,
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
## CreateLiveSourceResponseTypeDef

```python
# CreateLiveSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreateLiveSourceResponseTypeDef


def get_value() -> CreateLiveSourceResponseTypeDef:
    return {
        "Arn": ...,
    }


# CreateLiveSourceResponseTypeDef definition

class CreateLiveSourceResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    HttpPackageConfigurations: List[HttpPackageConfigurationTypeDef],  # (1)
    LastModifiedTime: datetime,
    LiveSourceName: str,
    SourceLocationName: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVodSourceRequestTypeDef

```python
# CreateVodSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreateVodSourceRequestTypeDef


def get_value() -> CreateVodSourceRequestTypeDef:
    return {
        "HttpPackageConfigurations": ...,
    }


# CreateVodSourceRequestTypeDef definition

class CreateVodSourceRequestTypeDef(TypedDict):
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    SourceLocationName: str,
    VodSourceName: str,
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
## CreateVodSourceResponseTypeDef

```python
# CreateVodSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreateVodSourceResponseTypeDef


def get_value() -> CreateVodSourceResponseTypeDef:
    return {
        "Arn": ...,
    }


# CreateVodSourceResponseTypeDef definition

class CreateVodSourceResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    HttpPackageConfigurations: List[HttpPackageConfigurationTypeDef],  # (1)
    LastModifiedTime: datetime,
    SourceLocationName: str,
    Tags: Dict[str, str],
    VodSourceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLiveSourceResponseTypeDef

```python
# DescribeLiveSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DescribeLiveSourceResponseTypeDef


def get_value() -> DescribeLiveSourceResponseTypeDef:
    return {
        "Arn": ...,
    }


# DescribeLiveSourceResponseTypeDef definition

class DescribeLiveSourceResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    HttpPackageConfigurations: List[HttpPackageConfigurationTypeDef],  # (1)
    LastModifiedTime: datetime,
    LiveSourceName: str,
    SourceLocationName: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVodSourceResponseTypeDef

```python
# DescribeVodSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DescribeVodSourceResponseTypeDef


def get_value() -> DescribeVodSourceResponseTypeDef:
    return {
        "AdBreakOpportunities": ...,
    }


# DescribeVodSourceResponseTypeDef definition

class DescribeVodSourceResponseTypeDef(TypedDict):
    AdBreakOpportunities: List[AdBreakOpportunityTypeDef],  # (1)
    Arn: str,
    CreationTime: datetime,
    HttpPackageConfigurations: List[HttpPackageConfigurationTypeDef],  # (2)
    LastModifiedTime: datetime,
    SourceLocationName: str,
    Tags: Dict[str, str],
    VodSourceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AdBreakOpportunityTypeDef](./type_defs.md#adbreakopportunitytypedef) 
2. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LiveSourceTypeDef

```python
# LiveSourceTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import LiveSourceTypeDef


def get_value() -> LiveSourceTypeDef:
    return {
        "Arn": ...,
    }


# LiveSourceTypeDef definition

class LiveSourceTypeDef(TypedDict):
    Arn: str,
    HttpPackageConfigurations: List[HttpPackageConfigurationTypeDef],  # (1)
    LiveSourceName: str,
    SourceLocationName: str,
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
## UpdateLiveSourceRequestTypeDef

```python
# UpdateLiveSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateLiveSourceRequestTypeDef


def get_value() -> UpdateLiveSourceRequestTypeDef:
    return {
        "HttpPackageConfigurations": ...,
    }


# UpdateLiveSourceRequestTypeDef definition

class UpdateLiveSourceRequestTypeDef(TypedDict):
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    LiveSourceName: str,
    SourceLocationName: str,
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
## UpdateLiveSourceResponseTypeDef

```python
# UpdateLiveSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateLiveSourceResponseTypeDef


def get_value() -> UpdateLiveSourceResponseTypeDef:
    return {
        "Arn": ...,
    }


# UpdateLiveSourceResponseTypeDef definition

class UpdateLiveSourceResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    HttpPackageConfigurations: List[HttpPackageConfigurationTypeDef],  # (1)
    LastModifiedTime: datetime,
    LiveSourceName: str,
    SourceLocationName: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVodSourceRequestTypeDef

```python
# UpdateVodSourceRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateVodSourceRequestTypeDef


def get_value() -> UpdateVodSourceRequestTypeDef:
    return {
        "HttpPackageConfigurations": ...,
    }


# UpdateVodSourceRequestTypeDef definition

class UpdateVodSourceRequestTypeDef(TypedDict):
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    SourceLocationName: str,
    VodSourceName: str,
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
## UpdateVodSourceResponseTypeDef

```python
# UpdateVodSourceResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateVodSourceResponseTypeDef


def get_value() -> UpdateVodSourceResponseTypeDef:
    return {
        "Arn": ...,
    }


# UpdateVodSourceResponseTypeDef definition

class UpdateVodSourceResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    HttpPackageConfigurations: List[HttpPackageConfigurationTypeDef],  # (1)
    LastModifiedTime: datetime,
    SourceLocationName: str,
    Tags: Dict[str, str],
    VodSourceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VodSourceTypeDef

```python
# VodSourceTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import VodSourceTypeDef


def get_value() -> VodSourceTypeDef:
    return {
        "Arn": ...,
    }


# VodSourceTypeDef definition

class VodSourceTypeDef(TypedDict):
    Arn: str,
    HttpPackageConfigurations: List[HttpPackageConfigurationTypeDef],  # (1)
    SourceLocationName: str,
    VodSourceName: str,
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
## GetChannelScheduleRequestPaginateTypeDef

```python
# GetChannelScheduleRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import GetChannelScheduleRequestPaginateTypeDef


def get_value() -> GetChannelScheduleRequestPaginateTypeDef:
    return {
        "ChannelName": ...,
    }


# GetChannelScheduleRequestPaginateTypeDef definition

class GetChannelScheduleRequestPaginateTypeDef(TypedDict):
    ChannelName: str,
    DurationMinutes: NotRequired[str],
    Audience: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAlertsRequestPaginateTypeDef

```python
# ListAlertsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListAlertsRequestPaginateTypeDef


def get_value() -> ListAlertsRequestPaginateTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListAlertsRequestPaginateTypeDef definition

class ListAlertsRequestPaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListChannelsRequestPaginateTypeDef

```python
# ListChannelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListChannelsRequestPaginateTypeDef


def get_value() -> ListChannelsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListChannelsRequestPaginateTypeDef definition

class ListChannelsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLiveSourcesRequestPaginateTypeDef

```python
# ListLiveSourcesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListLiveSourcesRequestPaginateTypeDef


def get_value() -> ListLiveSourcesRequestPaginateTypeDef:
    return {
        "SourceLocationName": ...,
    }


# ListLiveSourcesRequestPaginateTypeDef definition

class ListLiveSourcesRequestPaginateTypeDef(TypedDict):
    SourceLocationName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPlaybackConfigurationsRequestPaginateTypeDef

```python
# ListPlaybackConfigurationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListPlaybackConfigurationsRequestPaginateTypeDef


def get_value() -> ListPlaybackConfigurationsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListPlaybackConfigurationsRequestPaginateTypeDef definition

class ListPlaybackConfigurationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrefetchSchedulesRequestPaginateTypeDef

```python
# ListPrefetchSchedulesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListPrefetchSchedulesRequestPaginateTypeDef


def get_value() -> ListPrefetchSchedulesRequestPaginateTypeDef:
    return {
        "PlaybackConfigurationName": ...,
    }


# ListPrefetchSchedulesRequestPaginateTypeDef definition

class ListPrefetchSchedulesRequestPaginateTypeDef(TypedDict):
    PlaybackConfigurationName: str,
    StreamId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSourceLocationsRequestPaginateTypeDef

```python
# ListSourceLocationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListSourceLocationsRequestPaginateTypeDef


def get_value() -> ListSourceLocationsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListSourceLocationsRequestPaginateTypeDef definition

class ListSourceLocationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVodSourcesRequestPaginateTypeDef

```python
# ListVodSourcesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListVodSourcesRequestPaginateTypeDef


def get_value() -> ListVodSourcesRequestPaginateTypeDef:
    return {
        "SourceLocationName": ...,
    }


# ListVodSourcesRequestPaginateTypeDef definition

class ListVodSourcesRequestPaginateTypeDef(TypedDict):
    SourceLocationName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ResponseOutputItemTypeDef

```python
# ResponseOutputItemTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ResponseOutputItemTypeDef


def get_value() -> ResponseOutputItemTypeDef:
    return {
        "DashPlaylistSettings": ...,
    }


# ResponseOutputItemTypeDef definition

class ResponseOutputItemTypeDef(TypedDict):
    ManifestName: str,
    PlaybackUrl: str,
    SourceGroup: str,
    DashPlaylistSettings: NotRequired[DashPlaylistSettingsTypeDef],  # (1)
    HlsPlaylistSettings: NotRequired[HlsPlaylistSettingsOutputTypeDef],  # (2)
```

1. See [:material-code-braces: DashPlaylistSettingsTypeDef](./type_defs.md#dashplaylistsettingstypedef) 
2. See [:material-code-braces: HlsPlaylistSettingsOutputTypeDef](./type_defs.md#hlsplaylistsettingsoutputtypedef) 
## PrefetchConsumptionTypeDef

```python
# PrefetchConsumptionTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import PrefetchConsumptionTypeDef


def get_value() -> PrefetchConsumptionTypeDef:
    return {
        "AvailMatchingCriteria": ...,
    }


# PrefetchConsumptionTypeDef definition

class PrefetchConsumptionTypeDef(TypedDict):
    EndTime: TimestampTypeDef,
    AvailMatchingCriteria: NotRequired[Sequence[AvailMatchingCriteriaTypeDef]],  # (1)
    StartTime: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: AvailMatchingCriteriaTypeDef](./type_defs.md#availmatchingcriteriatypedef) 
## PrefetchRetrievalTypeDef

```python
# PrefetchRetrievalTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import PrefetchRetrievalTypeDef


def get_value() -> PrefetchRetrievalTypeDef:
    return {
        "DynamicVariables": ...,
    }


# PrefetchRetrievalTypeDef definition

class PrefetchRetrievalTypeDef(TypedDict):
    EndTime: TimestampTypeDef,
    DynamicVariables: NotRequired[Mapping[str, str]],
    StartTime: NotRequired[TimestampTypeDef],
```

## ScheduleEntryTypeDef

```python
# ScheduleEntryTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ScheduleEntryTypeDef


def get_value() -> ScheduleEntryTypeDef:
    return {
        "ApproximateDurationSeconds": ...,
    }


# ScheduleEntryTypeDef definition

class ScheduleEntryTypeDef(TypedDict):
    Arn: str,
    ChannelName: str,
    ProgramName: str,
    SourceLocationName: str,
    ApproximateDurationSeconds: NotRequired[int],
    ApproximateStartTime: NotRequired[datetime],
    LiveSourceName: NotRequired[str],
    ScheduleAdBreaks: NotRequired[List[ScheduleAdBreakTypeDef]],  # (1)
    ScheduleEntryType: NotRequired[ScheduleEntryTypeType],  # (2)
    VodSourceName: NotRequired[str],
    Audiences: NotRequired[List[str]],
```

1. See [:material-code-braces: ScheduleAdBreakTypeDef](./type_defs.md#scheduleadbreaktypedef) 
2. See [:material-code-brackets: ScheduleEntryTypeType](./literals.md#scheduleentrytypetype) 
## ScheduleConfigurationTypeDef

```python
# ScheduleConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ScheduleConfigurationTypeDef


def get_value() -> ScheduleConfigurationTypeDef:
    return {
        "Transition": ...,
    }


# ScheduleConfigurationTypeDef definition

class ScheduleConfigurationTypeDef(TypedDict):
    Transition: TransitionTypeDef,  # (1)
    ClipRange: NotRequired[ClipRangeTypeDef],  # (2)
```

1. See [:material-code-braces: TransitionTypeDef](./type_defs.md#transitiontypedef) 
2. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
## TimeSignalMessageOutputTypeDef

```python
# TimeSignalMessageOutputTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import TimeSignalMessageOutputTypeDef


def get_value() -> TimeSignalMessageOutputTypeDef:
    return {
        "SegmentationDescriptors": ...,
    }


# TimeSignalMessageOutputTypeDef definition

class TimeSignalMessageOutputTypeDef(TypedDict):
    SegmentationDescriptors: NotRequired[List[SegmentationDescriptorTypeDef]],  # (1)
```

1. See [:material-code-braces: SegmentationDescriptorTypeDef](./type_defs.md#segmentationdescriptortypedef) 
## TimeSignalMessageTypeDef

```python
# TimeSignalMessageTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import TimeSignalMessageTypeDef


def get_value() -> TimeSignalMessageTypeDef:
    return {
        "SegmentationDescriptors": ...,
    }


# TimeSignalMessageTypeDef definition

class TimeSignalMessageTypeDef(TypedDict):
    SegmentationDescriptors: NotRequired[Sequence[SegmentationDescriptorTypeDef]],  # (1)
```

1. See [:material-code-braces: SegmentationDescriptorTypeDef](./type_defs.md#segmentationdescriptortypedef) 
## UpdateProgramScheduleConfigurationTypeDef

```python
# UpdateProgramScheduleConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateProgramScheduleConfigurationTypeDef


def get_value() -> UpdateProgramScheduleConfigurationTypeDef:
    return {
        "Transition": ...,
    }


# UpdateProgramScheduleConfigurationTypeDef definition

class UpdateProgramScheduleConfigurationTypeDef(TypedDict):
    Transition: NotRequired[UpdateProgramTransitionTypeDef],  # (1)
    ClipRange: NotRequired[ClipRangeTypeDef],  # (2)
```

1. See [:material-code-braces: UpdateProgramTransitionTypeDef](./type_defs.md#updateprogramtransitiontypedef) 
2. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
## CreateSourceLocationRequestTypeDef

```python
# CreateSourceLocationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreateSourceLocationRequestTypeDef


def get_value() -> CreateSourceLocationRequestTypeDef:
    return {
        "HttpConfiguration": ...,
    }


# CreateSourceLocationRequestTypeDef definition

class CreateSourceLocationRequestTypeDef(TypedDict):
    HttpConfiguration: HttpConfigurationTypeDef,  # (1)
    SourceLocationName: str,
    AccessConfiguration: NotRequired[AccessConfigurationTypeDef],  # (2)
    DefaultSegmentDeliveryConfiguration: NotRequired[DefaultSegmentDeliveryConfigurationTypeDef],  # (3)
    SegmentDeliveryConfigurations: NotRequired[Sequence[SegmentDeliveryConfigurationTypeDef]],  # (4)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: HttpConfigurationTypeDef](./type_defs.md#httpconfigurationtypedef) 
2. See [:material-code-braces: AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef) 
3. See [:material-code-braces: DefaultSegmentDeliveryConfigurationTypeDef](./type_defs.md#defaultsegmentdeliveryconfigurationtypedef) 
4. See [:material-code-braces: SegmentDeliveryConfigurationTypeDef](./type_defs.md#segmentdeliveryconfigurationtypedef) 
## CreateSourceLocationResponseTypeDef

```python
# CreateSourceLocationResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreateSourceLocationResponseTypeDef


def get_value() -> CreateSourceLocationResponseTypeDef:
    return {
        "AccessConfiguration": ...,
    }


# CreateSourceLocationResponseTypeDef definition

class CreateSourceLocationResponseTypeDef(TypedDict):
    AccessConfiguration: AccessConfigurationTypeDef,  # (1)
    Arn: str,
    CreationTime: datetime,
    DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef,  # (2)
    HttpConfiguration: HttpConfigurationTypeDef,  # (3)
    LastModifiedTime: datetime,
    SegmentDeliveryConfigurations: List[SegmentDeliveryConfigurationTypeDef],  # (4)
    SourceLocationName: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef) 
2. See [:material-code-braces: DefaultSegmentDeliveryConfigurationTypeDef](./type_defs.md#defaultsegmentdeliveryconfigurationtypedef) 
3. See [:material-code-braces: HttpConfigurationTypeDef](./type_defs.md#httpconfigurationtypedef) 
4. See [:material-code-braces: SegmentDeliveryConfigurationTypeDef](./type_defs.md#segmentdeliveryconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSourceLocationResponseTypeDef

```python
# DescribeSourceLocationResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DescribeSourceLocationResponseTypeDef


def get_value() -> DescribeSourceLocationResponseTypeDef:
    return {
        "AccessConfiguration": ...,
    }


# DescribeSourceLocationResponseTypeDef definition

class DescribeSourceLocationResponseTypeDef(TypedDict):
    AccessConfiguration: AccessConfigurationTypeDef,  # (1)
    Arn: str,
    CreationTime: datetime,
    DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef,  # (2)
    HttpConfiguration: HttpConfigurationTypeDef,  # (3)
    LastModifiedTime: datetime,
    SegmentDeliveryConfigurations: List[SegmentDeliveryConfigurationTypeDef],  # (4)
    SourceLocationName: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef) 
2. See [:material-code-braces: DefaultSegmentDeliveryConfigurationTypeDef](./type_defs.md#defaultsegmentdeliveryconfigurationtypedef) 
3. See [:material-code-braces: HttpConfigurationTypeDef](./type_defs.md#httpconfigurationtypedef) 
4. See [:material-code-braces: SegmentDeliveryConfigurationTypeDef](./type_defs.md#segmentdeliveryconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceLocationTypeDef

```python
# SourceLocationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import SourceLocationTypeDef


def get_value() -> SourceLocationTypeDef:
    return {
        "AccessConfiguration": ...,
    }


# SourceLocationTypeDef definition

class SourceLocationTypeDef(TypedDict):
    Arn: str,
    HttpConfiguration: HttpConfigurationTypeDef,  # (3)
    SourceLocationName: str,
    AccessConfiguration: NotRequired[AccessConfigurationTypeDef],  # (1)
    CreationTime: NotRequired[datetime],
    DefaultSegmentDeliveryConfiguration: NotRequired[DefaultSegmentDeliveryConfigurationTypeDef],  # (2)
    LastModifiedTime: NotRequired[datetime],
    SegmentDeliveryConfigurations: NotRequired[List[SegmentDeliveryConfigurationTypeDef]],  # (4)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef) 
2. See [:material-code-braces: DefaultSegmentDeliveryConfigurationTypeDef](./type_defs.md#defaultsegmentdeliveryconfigurationtypedef) 
3. See [:material-code-braces: HttpConfigurationTypeDef](./type_defs.md#httpconfigurationtypedef) 
4. See [:material-code-braces: SegmentDeliveryConfigurationTypeDef](./type_defs.md#segmentdeliveryconfigurationtypedef) 
## UpdateSourceLocationRequestTypeDef

```python
# UpdateSourceLocationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateSourceLocationRequestTypeDef


def get_value() -> UpdateSourceLocationRequestTypeDef:
    return {
        "HttpConfiguration": ...,
    }


# UpdateSourceLocationRequestTypeDef definition

class UpdateSourceLocationRequestTypeDef(TypedDict):
    HttpConfiguration: HttpConfigurationTypeDef,  # (1)
    SourceLocationName: str,
    AccessConfiguration: NotRequired[AccessConfigurationTypeDef],  # (2)
    DefaultSegmentDeliveryConfiguration: NotRequired[DefaultSegmentDeliveryConfigurationTypeDef],  # (3)
    SegmentDeliveryConfigurations: NotRequired[Sequence[SegmentDeliveryConfigurationTypeDef]],  # (4)
```

1. See [:material-code-braces: HttpConfigurationTypeDef](./type_defs.md#httpconfigurationtypedef) 
2. See [:material-code-braces: AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef) 
3. See [:material-code-braces: DefaultSegmentDeliveryConfigurationTypeDef](./type_defs.md#defaultsegmentdeliveryconfigurationtypedef) 
4. See [:material-code-braces: SegmentDeliveryConfigurationTypeDef](./type_defs.md#segmentdeliveryconfigurationtypedef) 
## UpdateSourceLocationResponseTypeDef

```python
# UpdateSourceLocationResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateSourceLocationResponseTypeDef


def get_value() -> UpdateSourceLocationResponseTypeDef:
    return {
        "AccessConfiguration": ...,
    }


# UpdateSourceLocationResponseTypeDef definition

class UpdateSourceLocationResponseTypeDef(TypedDict):
    AccessConfiguration: AccessConfigurationTypeDef,  # (1)
    Arn: str,
    CreationTime: datetime,
    DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef,  # (2)
    HttpConfiguration: HttpConfigurationTypeDef,  # (3)
    LastModifiedTime: datetime,
    SegmentDeliveryConfigurations: List[SegmentDeliveryConfigurationTypeDef],  # (4)
    SourceLocationName: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef) 
2. See [:material-code-braces: DefaultSegmentDeliveryConfigurationTypeDef](./type_defs.md#defaultsegmentdeliveryconfigurationtypedef) 
3. See [:material-code-braces: HttpConfigurationTypeDef](./type_defs.md#httpconfigurationtypedef) 
4. See [:material-code-braces: SegmentDeliveryConfigurationTypeDef](./type_defs.md#segmentdeliveryconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPlaybackConfigurationResponseTypeDef

```python
# GetPlaybackConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import GetPlaybackConfigurationResponseTypeDef


def get_value() -> GetPlaybackConfigurationResponseTypeDef:
    return {
        "AdDecisionServerUrl": ...,
    }


# GetPlaybackConfigurationResponseTypeDef definition

class GetPlaybackConfigurationResponseTypeDef(TypedDict):
    AdDecisionServerUrl: str,
    AvailSuppression: AvailSuppressionTypeDef,  # (1)
    Bumper: BumperTypeDef,  # (2)
    CdnConfiguration: CdnConfigurationTypeDef,  # (3)
    ConfigurationAliases: Dict[str, Dict[str, str]],
    DashConfiguration: DashConfigurationTypeDef,  # (4)
    HlsConfiguration: HlsConfigurationTypeDef,  # (5)
    InsertionMode: InsertionModeType,  # (6)
    LivePreRollConfiguration: LivePreRollConfigurationTypeDef,  # (7)
    LogConfiguration: LogConfigurationTypeDef,  # (8)
    ManifestProcessingRules: ManifestProcessingRulesTypeDef,  # (9)
    Name: str,
    PersonalizationThresholdSeconds: int,
    PlaybackConfigurationArn: str,
    PlaybackEndpointPrefix: str,
    SessionInitializationEndpointPrefix: str,
    SlateAdUrl: str,
    Tags: Dict[str, str],
    TranscodeProfileName: str,
    VideoContentSourceUrl: str,
    AdConditioningConfiguration: AdConditioningConfigurationTypeDef,  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: AvailSuppressionTypeDef](./type_defs.md#availsuppressiontypedef) 
2. See [:material-code-braces: BumperTypeDef](./type_defs.md#bumpertypedef) 
3. See [:material-code-braces: CdnConfigurationTypeDef](./type_defs.md#cdnconfigurationtypedef) 
4. See [:material-code-braces: DashConfigurationTypeDef](./type_defs.md#dashconfigurationtypedef) 
5. See [:material-code-braces: HlsConfigurationTypeDef](./type_defs.md#hlsconfigurationtypedef) 
6. See [:material-code-brackets: InsertionModeType](./literals.md#insertionmodetype) 
7. See [:material-code-braces: LivePreRollConfigurationTypeDef](./type_defs.md#liveprerollconfigurationtypedef) 
8. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
9. See [:material-code-braces: ManifestProcessingRulesTypeDef](./type_defs.md#manifestprocessingrulestypedef) 
10. See [:material-code-braces: AdConditioningConfigurationTypeDef](./type_defs.md#adconditioningconfigurationtypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PlaybackConfigurationTypeDef

```python
# PlaybackConfigurationTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import PlaybackConfigurationTypeDef


def get_value() -> PlaybackConfigurationTypeDef:
    return {
        "AdDecisionServerUrl": ...,
    }


# PlaybackConfigurationTypeDef definition

class PlaybackConfigurationTypeDef(TypedDict):
    AdDecisionServerUrl: NotRequired[str],
    AvailSuppression: NotRequired[AvailSuppressionTypeDef],  # (1)
    Bumper: NotRequired[BumperTypeDef],  # (2)
    CdnConfiguration: NotRequired[CdnConfigurationTypeDef],  # (3)
    ConfigurationAliases: NotRequired[Dict[str, Dict[str, str]]],
    DashConfiguration: NotRequired[DashConfigurationTypeDef],  # (4)
    HlsConfiguration: NotRequired[HlsConfigurationTypeDef],  # (5)
    InsertionMode: NotRequired[InsertionModeType],  # (6)
    LivePreRollConfiguration: NotRequired[LivePreRollConfigurationTypeDef],  # (7)
    LogConfiguration: NotRequired[LogConfigurationTypeDef],  # (8)
    ManifestProcessingRules: NotRequired[ManifestProcessingRulesTypeDef],  # (9)
    Name: NotRequired[str],
    PersonalizationThresholdSeconds: NotRequired[int],
    PlaybackConfigurationArn: NotRequired[str],
    PlaybackEndpointPrefix: NotRequired[str],
    SessionInitializationEndpointPrefix: NotRequired[str],
    SlateAdUrl: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    TranscodeProfileName: NotRequired[str],
    VideoContentSourceUrl: NotRequired[str],
    AdConditioningConfiguration: NotRequired[AdConditioningConfigurationTypeDef],  # (10)
```

1. See [:material-code-braces: AvailSuppressionTypeDef](./type_defs.md#availsuppressiontypedef) 
2. See [:material-code-braces: BumperTypeDef](./type_defs.md#bumpertypedef) 
3. See [:material-code-braces: CdnConfigurationTypeDef](./type_defs.md#cdnconfigurationtypedef) 
4. See [:material-code-braces: DashConfigurationTypeDef](./type_defs.md#dashconfigurationtypedef) 
5. See [:material-code-braces: HlsConfigurationTypeDef](./type_defs.md#hlsconfigurationtypedef) 
6. See [:material-code-brackets: InsertionModeType](./literals.md#insertionmodetype) 
7. See [:material-code-braces: LivePreRollConfigurationTypeDef](./type_defs.md#liveprerollconfigurationtypedef) 
8. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
9. See [:material-code-braces: ManifestProcessingRulesTypeDef](./type_defs.md#manifestprocessingrulestypedef) 
10. See [:material-code-braces: AdConditioningConfigurationTypeDef](./type_defs.md#adconditioningconfigurationtypedef) 
## PutPlaybackConfigurationRequestTypeDef

```python
# PutPlaybackConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import PutPlaybackConfigurationRequestTypeDef


def get_value() -> PutPlaybackConfigurationRequestTypeDef:
    return {
        "Name": ...,
    }


# PutPlaybackConfigurationRequestTypeDef definition

class PutPlaybackConfigurationRequestTypeDef(TypedDict):
    Name: str,
    AdDecisionServerUrl: NotRequired[str],
    AvailSuppression: NotRequired[AvailSuppressionTypeDef],  # (1)
    Bumper: NotRequired[BumperTypeDef],  # (2)
    CdnConfiguration: NotRequired[CdnConfigurationTypeDef],  # (3)
    ConfigurationAliases: NotRequired[Mapping[str, Mapping[str, str]]],
    DashConfiguration: NotRequired[DashConfigurationForPutTypeDef],  # (4)
    InsertionMode: NotRequired[InsertionModeType],  # (5)
    LivePreRollConfiguration: NotRequired[LivePreRollConfigurationTypeDef],  # (6)
    ManifestProcessingRules: NotRequired[ManifestProcessingRulesTypeDef],  # (7)
    PersonalizationThresholdSeconds: NotRequired[int],
    SlateAdUrl: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    TranscodeProfileName: NotRequired[str],
    VideoContentSourceUrl: NotRequired[str],
    AdConditioningConfiguration: NotRequired[AdConditioningConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: AvailSuppressionTypeDef](./type_defs.md#availsuppressiontypedef) 
2. See [:material-code-braces: BumperTypeDef](./type_defs.md#bumpertypedef) 
3. See [:material-code-braces: CdnConfigurationTypeDef](./type_defs.md#cdnconfigurationtypedef) 
4. See [:material-code-braces: DashConfigurationForPutTypeDef](./type_defs.md#dashconfigurationforputtypedef) 
5. See [:material-code-brackets: InsertionModeType](./literals.md#insertionmodetype) 
6. See [:material-code-braces: LivePreRollConfigurationTypeDef](./type_defs.md#liveprerollconfigurationtypedef) 
7. See [:material-code-braces: ManifestProcessingRulesTypeDef](./type_defs.md#manifestprocessingrulestypedef) 
8. See [:material-code-braces: AdConditioningConfigurationTypeDef](./type_defs.md#adconditioningconfigurationtypedef) 
## PutPlaybackConfigurationResponseTypeDef

```python
# PutPlaybackConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import PutPlaybackConfigurationResponseTypeDef


def get_value() -> PutPlaybackConfigurationResponseTypeDef:
    return {
        "AdDecisionServerUrl": ...,
    }


# PutPlaybackConfigurationResponseTypeDef definition

class PutPlaybackConfigurationResponseTypeDef(TypedDict):
    AdDecisionServerUrl: str,
    AvailSuppression: AvailSuppressionTypeDef,  # (1)
    Bumper: BumperTypeDef,  # (2)
    CdnConfiguration: CdnConfigurationTypeDef,  # (3)
    ConfigurationAliases: Dict[str, Dict[str, str]],
    DashConfiguration: DashConfigurationTypeDef,  # (4)
    HlsConfiguration: HlsConfigurationTypeDef,  # (5)
    InsertionMode: InsertionModeType,  # (6)
    LivePreRollConfiguration: LivePreRollConfigurationTypeDef,  # (7)
    LogConfiguration: LogConfigurationTypeDef,  # (8)
    ManifestProcessingRules: ManifestProcessingRulesTypeDef,  # (9)
    Name: str,
    PersonalizationThresholdSeconds: int,
    PlaybackConfigurationArn: str,
    PlaybackEndpointPrefix: str,
    SessionInitializationEndpointPrefix: str,
    SlateAdUrl: str,
    Tags: Dict[str, str],
    TranscodeProfileName: str,
    VideoContentSourceUrl: str,
    AdConditioningConfiguration: AdConditioningConfigurationTypeDef,  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: AvailSuppressionTypeDef](./type_defs.md#availsuppressiontypedef) 
2. See [:material-code-braces: BumperTypeDef](./type_defs.md#bumpertypedef) 
3. See [:material-code-braces: CdnConfigurationTypeDef](./type_defs.md#cdnconfigurationtypedef) 
4. See [:material-code-braces: DashConfigurationTypeDef](./type_defs.md#dashconfigurationtypedef) 
5. See [:material-code-braces: HlsConfigurationTypeDef](./type_defs.md#hlsconfigurationtypedef) 
6. See [:material-code-brackets: InsertionModeType](./literals.md#insertionmodetype) 
7. See [:material-code-braces: LivePreRollConfigurationTypeDef](./type_defs.md#liveprerollconfigurationtypedef) 
8. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
9. See [:material-code-braces: ManifestProcessingRulesTypeDef](./type_defs.md#manifestprocessingrulestypedef) 
10. See [:material-code-braces: AdConditioningConfigurationTypeDef](./type_defs.md#adconditioningconfigurationtypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePrefetchScheduleResponseTypeDef

```python
# CreatePrefetchScheduleResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreatePrefetchScheduleResponseTypeDef


def get_value() -> CreatePrefetchScheduleResponseTypeDef:
    return {
        "Arn": ...,
    }


# CreatePrefetchScheduleResponseTypeDef definition

class CreatePrefetchScheduleResponseTypeDef(TypedDict):
    Arn: str,
    Consumption: PrefetchConsumptionOutputTypeDef,  # (1)
    Name: str,
    PlaybackConfigurationName: str,
    Retrieval: PrefetchRetrievalOutputTypeDef,  # (2)
    StreamId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PrefetchConsumptionOutputTypeDef](./type_defs.md#prefetchconsumptionoutputtypedef) 
2. See [:material-code-braces: PrefetchRetrievalOutputTypeDef](./type_defs.md#prefetchretrievaloutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPrefetchScheduleResponseTypeDef

```python
# GetPrefetchScheduleResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import GetPrefetchScheduleResponseTypeDef


def get_value() -> GetPrefetchScheduleResponseTypeDef:
    return {
        "Arn": ...,
    }


# GetPrefetchScheduleResponseTypeDef definition

class GetPrefetchScheduleResponseTypeDef(TypedDict):
    Arn: str,
    Consumption: PrefetchConsumptionOutputTypeDef,  # (1)
    Name: str,
    PlaybackConfigurationName: str,
    Retrieval: PrefetchRetrievalOutputTypeDef,  # (2)
    StreamId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PrefetchConsumptionOutputTypeDef](./type_defs.md#prefetchconsumptionoutputtypedef) 
2. See [:material-code-braces: PrefetchRetrievalOutputTypeDef](./type_defs.md#prefetchretrievaloutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PrefetchScheduleTypeDef

```python
# PrefetchScheduleTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import PrefetchScheduleTypeDef


def get_value() -> PrefetchScheduleTypeDef:
    return {
        "Arn": ...,
    }


# PrefetchScheduleTypeDef definition

class PrefetchScheduleTypeDef(TypedDict):
    Arn: str,
    Consumption: PrefetchConsumptionOutputTypeDef,  # (1)
    Name: str,
    PlaybackConfigurationName: str,
    Retrieval: PrefetchRetrievalOutputTypeDef,  # (2)
    StreamId: NotRequired[str],
```

1. See [:material-code-braces: PrefetchConsumptionOutputTypeDef](./type_defs.md#prefetchconsumptionoutputtypedef) 
2. See [:material-code-braces: PrefetchRetrievalOutputTypeDef](./type_defs.md#prefetchretrievaloutputtypedef) 
## ListLiveSourcesResponseTypeDef

```python
# ListLiveSourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListLiveSourcesResponseTypeDef


def get_value() -> ListLiveSourcesResponseTypeDef:
    return {
        "Items": ...,
    }


# ListLiveSourcesResponseTypeDef definition

class ListLiveSourcesResponseTypeDef(TypedDict):
    Items: List[LiveSourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LiveSourceTypeDef](./type_defs.md#livesourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVodSourcesResponseTypeDef

```python
# ListVodSourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListVodSourcesResponseTypeDef


def get_value() -> ListVodSourcesResponseTypeDef:
    return {
        "Items": ...,
    }


# ListVodSourcesResponseTypeDef definition

class ListVodSourcesResponseTypeDef(TypedDict):
    Items: List[VodSourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VodSourceTypeDef](./type_defs.md#vodsourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChannelTypeDef

```python
# ChannelTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ChannelTypeDef


def get_value() -> ChannelTypeDef:
    return {
        "Arn": ...,
    }


# ChannelTypeDef definition

class ChannelTypeDef(TypedDict):
    Arn: str,
    ChannelName: str,
    ChannelState: str,
    Outputs: List[ResponseOutputItemTypeDef],  # (2)
    PlaybackMode: str,
    Tier: str,
    LogConfiguration: LogConfigurationForChannelTypeDef,  # (3)
    CreationTime: NotRequired[datetime],
    FillerSlate: NotRequired[SlateSourceTypeDef],  # (1)
    LastModifiedTime: NotRequired[datetime],
    Tags: NotRequired[Dict[str, str]],
    Audiences: NotRequired[List[str]],
```

1. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
2. See [:material-code-braces: ResponseOutputItemTypeDef](./type_defs.md#responseoutputitemtypedef) 
3. See [:material-code-braces: LogConfigurationForChannelTypeDef](./type_defs.md#logconfigurationforchanneltypedef) 
## CreateChannelResponseTypeDef

```python
# CreateChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreateChannelResponseTypeDef


def get_value() -> CreateChannelResponseTypeDef:
    return {
        "Arn": ...,
    }


# CreateChannelResponseTypeDef definition

class CreateChannelResponseTypeDef(TypedDict):
    Arn: str,
    ChannelName: str,
    ChannelState: ChannelStateType,  # (1)
    CreationTime: datetime,
    FillerSlate: SlateSourceTypeDef,  # (2)
    LastModifiedTime: datetime,
    Outputs: List[ResponseOutputItemTypeDef],  # (3)
    PlaybackMode: str,
    Tags: Dict[str, str],
    Tier: str,
    TimeShiftConfiguration: TimeShiftConfigurationTypeDef,  # (4)
    Audiences: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
2. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
3. See [:material-code-braces: ResponseOutputItemTypeDef](./type_defs.md#responseoutputitemtypedef) 
4. See [:material-code-braces: TimeShiftConfigurationTypeDef](./type_defs.md#timeshiftconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelResponseTypeDef

```python
# DescribeChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DescribeChannelResponseTypeDef


def get_value() -> DescribeChannelResponseTypeDef:
    return {
        "Arn": ...,
    }


# DescribeChannelResponseTypeDef definition

class DescribeChannelResponseTypeDef(TypedDict):
    Arn: str,
    ChannelName: str,
    ChannelState: ChannelStateType,  # (1)
    CreationTime: datetime,
    FillerSlate: SlateSourceTypeDef,  # (2)
    LastModifiedTime: datetime,
    Outputs: List[ResponseOutputItemTypeDef],  # (3)
    PlaybackMode: str,
    Tags: Dict[str, str],
    Tier: str,
    LogConfiguration: LogConfigurationForChannelTypeDef,  # (4)
    TimeShiftConfiguration: TimeShiftConfigurationTypeDef,  # (5)
    Audiences: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
2. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
3. See [:material-code-braces: ResponseOutputItemTypeDef](./type_defs.md#responseoutputitemtypedef) 
4. See [:material-code-braces: LogConfigurationForChannelTypeDef](./type_defs.md#logconfigurationforchanneltypedef) 
5. See [:material-code-braces: TimeShiftConfigurationTypeDef](./type_defs.md#timeshiftconfigurationtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelResponseTypeDef

```python
# UpdateChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateChannelResponseTypeDef


def get_value() -> UpdateChannelResponseTypeDef:
    return {
        "Arn": ...,
    }


# UpdateChannelResponseTypeDef definition

class UpdateChannelResponseTypeDef(TypedDict):
    Arn: str,
    ChannelName: str,
    ChannelState: ChannelStateType,  # (1)
    CreationTime: datetime,
    FillerSlate: SlateSourceTypeDef,  # (2)
    LastModifiedTime: datetime,
    Outputs: List[ResponseOutputItemTypeDef],  # (3)
    PlaybackMode: str,
    Tags: Dict[str, str],
    Tier: str,
    TimeShiftConfiguration: TimeShiftConfigurationTypeDef,  # (4)
    Audiences: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
2. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
3. See [:material-code-braces: ResponseOutputItemTypeDef](./type_defs.md#responseoutputitemtypedef) 
4. See [:material-code-braces: TimeShiftConfigurationTypeDef](./type_defs.md#timeshiftconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RequestOutputItemTypeDef

```python
# RequestOutputItemTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import RequestOutputItemTypeDef


def get_value() -> RequestOutputItemTypeDef:
    return {
        "DashPlaylistSettings": ...,
    }


# RequestOutputItemTypeDef definition

class RequestOutputItemTypeDef(TypedDict):
    ManifestName: str,
    SourceGroup: str,
    DashPlaylistSettings: NotRequired[DashPlaylistSettingsTypeDef],  # (1)
    HlsPlaylistSettings: NotRequired[HlsPlaylistSettingsUnionTypeDef],  # (2)
```

1. See [:material-code-braces: DashPlaylistSettingsTypeDef](./type_defs.md#dashplaylistsettingstypedef) 
2. See [:material-code-braces: HlsPlaylistSettingsTypeDef](./type_defs.md#hlsplaylistsettingstypedef) [:material-code-braces: HlsPlaylistSettingsOutputTypeDef](./type_defs.md#hlsplaylistsettingsoutputtypedef) 
## GetChannelScheduleResponseTypeDef

```python
# GetChannelScheduleResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import GetChannelScheduleResponseTypeDef


def get_value() -> GetChannelScheduleResponseTypeDef:
    return {
        "Items": ...,
    }


# GetChannelScheduleResponseTypeDef definition

class GetChannelScheduleResponseTypeDef(TypedDict):
    Items: List[ScheduleEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScheduleEntryTypeDef](./type_defs.md#scheduleentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdBreakOutputTypeDef

```python
# AdBreakOutputTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AdBreakOutputTypeDef


def get_value() -> AdBreakOutputTypeDef:
    return {
        "MessageType": ...,
    }


# AdBreakOutputTypeDef definition

class AdBreakOutputTypeDef(TypedDict):
    OffsetMillis: int,
    MessageType: NotRequired[MessageTypeType],  # (1)
    Slate: NotRequired[SlateSourceTypeDef],  # (2)
    SpliceInsertMessage: NotRequired[SpliceInsertMessageTypeDef],  # (3)
    TimeSignalMessage: NotRequired[TimeSignalMessageOutputTypeDef],  # (4)
    AdBreakMetadata: NotRequired[List[KeyValuePairTypeDef]],  # (5)
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
3. See [:material-code-braces: SpliceInsertMessageTypeDef](./type_defs.md#spliceinsertmessagetypedef) 
4. See [:material-code-braces: TimeSignalMessageOutputTypeDef](./type_defs.md#timesignalmessageoutputtypedef) 
5. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
## ListSourceLocationsResponseTypeDef

```python
# ListSourceLocationsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListSourceLocationsResponseTypeDef


def get_value() -> ListSourceLocationsResponseTypeDef:
    return {
        "Items": ...,
    }


# ListSourceLocationsResponseTypeDef definition

class ListSourceLocationsResponseTypeDef(TypedDict):
    Items: List[SourceLocationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SourceLocationTypeDef](./type_defs.md#sourcelocationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPlaybackConfigurationsResponseTypeDef

```python
# ListPlaybackConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListPlaybackConfigurationsResponseTypeDef


def get_value() -> ListPlaybackConfigurationsResponseTypeDef:
    return {
        "Items": ...,
    }


# ListPlaybackConfigurationsResponseTypeDef definition

class ListPlaybackConfigurationsResponseTypeDef(TypedDict):
    Items: List[PlaybackConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PlaybackConfigurationTypeDef](./type_defs.md#playbackconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPrefetchSchedulesResponseTypeDef

```python
# ListPrefetchSchedulesResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListPrefetchSchedulesResponseTypeDef


def get_value() -> ListPrefetchSchedulesResponseTypeDef:
    return {
        "Items": ...,
    }


# ListPrefetchSchedulesResponseTypeDef definition

class ListPrefetchSchedulesResponseTypeDef(TypedDict):
    Items: List[PrefetchScheduleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PrefetchScheduleTypeDef](./type_defs.md#prefetchscheduletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import ListChannelsResponseTypeDef


def get_value() -> ListChannelsResponseTypeDef:
    return {
        "Items": ...,
    }


# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    Items: List[ChannelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelRequestTypeDef

```python
# CreateChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreateChannelRequestTypeDef


def get_value() -> CreateChannelRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# CreateChannelRequestTypeDef definition

class CreateChannelRequestTypeDef(TypedDict):
    ChannelName: str,
    Outputs: Sequence[RequestOutputItemTypeDef],  # (1)
    PlaybackMode: PlaybackModeType,  # (2)
    FillerSlate: NotRequired[SlateSourceTypeDef],  # (3)
    Tags: NotRequired[Mapping[str, str]],
    Tier: NotRequired[TierType],  # (4)
    TimeShiftConfiguration: NotRequired[TimeShiftConfigurationTypeDef],  # (5)
    Audiences: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: RequestOutputItemTypeDef](./type_defs.md#requestoutputitemtypedef) 
2. See [:material-code-brackets: PlaybackModeType](./literals.md#playbackmodetype) 
3. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
4. See [:material-code-brackets: TierType](./literals.md#tiertype) 
5. See [:material-code-braces: TimeShiftConfigurationTypeDef](./type_defs.md#timeshiftconfigurationtypedef) 
## UpdateChannelRequestTypeDef

```python
# UpdateChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateChannelRequestTypeDef


def get_value() -> UpdateChannelRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# UpdateChannelRequestTypeDef definition

class UpdateChannelRequestTypeDef(TypedDict):
    ChannelName: str,
    Outputs: Sequence[RequestOutputItemTypeDef],  # (1)
    FillerSlate: NotRequired[SlateSourceTypeDef],  # (2)
    TimeShiftConfiguration: NotRequired[TimeShiftConfigurationTypeDef],  # (3)
    Audiences: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: RequestOutputItemTypeDef](./type_defs.md#requestoutputitemtypedef) 
2. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
3. See [:material-code-braces: TimeShiftConfigurationTypeDef](./type_defs.md#timeshiftconfigurationtypedef) 
## CreatePrefetchScheduleRequestTypeDef

```python
# CreatePrefetchScheduleRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreatePrefetchScheduleRequestTypeDef


def get_value() -> CreatePrefetchScheduleRequestTypeDef:
    return {
        "Consumption": ...,
    }


# CreatePrefetchScheduleRequestTypeDef definition

class CreatePrefetchScheduleRequestTypeDef(TypedDict):
    Consumption: PrefetchConsumptionUnionTypeDef,  # (1)
    Name: str,
    PlaybackConfigurationName: str,
    Retrieval: PrefetchRetrievalUnionTypeDef,  # (2)
    StreamId: NotRequired[str],
```

1. See [:material-code-braces: PrefetchConsumptionTypeDef](./type_defs.md#prefetchconsumptiontypedef) [:material-code-braces: PrefetchConsumptionOutputTypeDef](./type_defs.md#prefetchconsumptionoutputtypedef) 
2. See [:material-code-braces: PrefetchRetrievalTypeDef](./type_defs.md#prefetchretrievaltypedef) [:material-code-braces: PrefetchRetrievalOutputTypeDef](./type_defs.md#prefetchretrievaloutputtypedef) 
## AlternateMediaOutputTypeDef

```python
# AlternateMediaOutputTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AlternateMediaOutputTypeDef


def get_value() -> AlternateMediaOutputTypeDef:
    return {
        "SourceLocationName": ...,
    }


# AlternateMediaOutputTypeDef definition

class AlternateMediaOutputTypeDef(TypedDict):
    SourceLocationName: NotRequired[str],
    LiveSourceName: NotRequired[str],
    VodSourceName: NotRequired[str],
    ClipRange: NotRequired[ClipRangeTypeDef],  # (1)
    ScheduledStartTimeMillis: NotRequired[int],
    AdBreaks: NotRequired[List[AdBreakOutputTypeDef]],  # (2)
    DurationMillis: NotRequired[int],
```

1. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
2. See [:material-code-braces: AdBreakOutputTypeDef](./type_defs.md#adbreakoutputtypedef) 
## AdBreakTypeDef

```python
# AdBreakTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AdBreakTypeDef


def get_value() -> AdBreakTypeDef:
    return {
        "MessageType": ...,
    }


# AdBreakTypeDef definition

class AdBreakTypeDef(TypedDict):
    OffsetMillis: int,
    MessageType: NotRequired[MessageTypeType],  # (1)
    Slate: NotRequired[SlateSourceTypeDef],  # (2)
    SpliceInsertMessage: NotRequired[SpliceInsertMessageTypeDef],  # (3)
    TimeSignalMessage: NotRequired[TimeSignalMessageUnionTypeDef],  # (4)
    AdBreakMetadata: NotRequired[Sequence[KeyValuePairTypeDef]],  # (5)
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
2. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
3. See [:material-code-braces: SpliceInsertMessageTypeDef](./type_defs.md#spliceinsertmessagetypedef) 
4. See [:material-code-braces: TimeSignalMessageTypeDef](./type_defs.md#timesignalmessagetypedef) [:material-code-braces: TimeSignalMessageOutputTypeDef](./type_defs.md#timesignalmessageoutputtypedef) 
5. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
## AudienceMediaOutputTypeDef

```python
# AudienceMediaOutputTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AudienceMediaOutputTypeDef


def get_value() -> AudienceMediaOutputTypeDef:
    return {
        "Audience": ...,
    }


# AudienceMediaOutputTypeDef definition

class AudienceMediaOutputTypeDef(TypedDict):
    Audience: NotRequired[str],
    AlternateMedia: NotRequired[List[AlternateMediaOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: AlternateMediaOutputTypeDef](./type_defs.md#alternatemediaoutputtypedef) 
## CreateProgramResponseTypeDef

```python
# CreateProgramResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreateProgramResponseTypeDef


def get_value() -> CreateProgramResponseTypeDef:
    return {
        "AdBreaks": ...,
    }


# CreateProgramResponseTypeDef definition

class CreateProgramResponseTypeDef(TypedDict):
    AdBreaks: List[AdBreakOutputTypeDef],  # (1)
    Arn: str,
    ChannelName: str,
    CreationTime: datetime,
    LiveSourceName: str,
    ProgramName: str,
    ScheduledStartTime: datetime,
    SourceLocationName: str,
    VodSourceName: str,
    ClipRange: ClipRangeTypeDef,  # (2)
    DurationMillis: int,
    AudienceMedia: List[AudienceMediaOutputTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AdBreakOutputTypeDef](./type_defs.md#adbreakoutputtypedef) 
2. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
3. See [:material-code-braces: AudienceMediaOutputTypeDef](./type_defs.md#audiencemediaoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProgramResponseTypeDef

```python
# DescribeProgramResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import DescribeProgramResponseTypeDef


def get_value() -> DescribeProgramResponseTypeDef:
    return {
        "AdBreaks": ...,
    }


# DescribeProgramResponseTypeDef definition

class DescribeProgramResponseTypeDef(TypedDict):
    AdBreaks: List[AdBreakOutputTypeDef],  # (1)
    Arn: str,
    ChannelName: str,
    CreationTime: datetime,
    LiveSourceName: str,
    ProgramName: str,
    ScheduledStartTime: datetime,
    SourceLocationName: str,
    VodSourceName: str,
    ClipRange: ClipRangeTypeDef,  # (2)
    DurationMillis: int,
    AudienceMedia: List[AudienceMediaOutputTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AdBreakOutputTypeDef](./type_defs.md#adbreakoutputtypedef) 
2. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
3. See [:material-code-braces: AudienceMediaOutputTypeDef](./type_defs.md#audiencemediaoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProgramResponseTypeDef

```python
# UpdateProgramResponseTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateProgramResponseTypeDef


def get_value() -> UpdateProgramResponseTypeDef:
    return {
        "AdBreaks": ...,
    }


# UpdateProgramResponseTypeDef definition

class UpdateProgramResponseTypeDef(TypedDict):
    AdBreaks: List[AdBreakOutputTypeDef],  # (1)
    Arn: str,
    ChannelName: str,
    CreationTime: datetime,
    ProgramName: str,
    SourceLocationName: str,
    VodSourceName: str,
    LiveSourceName: str,
    ClipRange: ClipRangeTypeDef,  # (2)
    DurationMillis: int,
    ScheduledStartTime: datetime,
    AudienceMedia: List[AudienceMediaOutputTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AdBreakOutputTypeDef](./type_defs.md#adbreakoutputtypedef) 
2. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
3. See [:material-code-braces: AudienceMediaOutputTypeDef](./type_defs.md#audiencemediaoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AlternateMediaTypeDef

```python
# AlternateMediaTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AlternateMediaTypeDef


def get_value() -> AlternateMediaTypeDef:
    return {
        "SourceLocationName": ...,
    }


# AlternateMediaTypeDef definition

class AlternateMediaTypeDef(TypedDict):
    SourceLocationName: NotRequired[str],
    LiveSourceName: NotRequired[str],
    VodSourceName: NotRequired[str],
    ClipRange: NotRequired[ClipRangeTypeDef],  # (1)
    ScheduledStartTimeMillis: NotRequired[int],
    AdBreaks: NotRequired[Sequence[AdBreakUnionTypeDef]],  # (2)
    DurationMillis: NotRequired[int],
```

1. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
2. See [:material-code-braces: AdBreakTypeDef](./type_defs.md#adbreaktypedef) [:material-code-braces: AdBreakOutputTypeDef](./type_defs.md#adbreakoutputtypedef) 
## AudienceMediaTypeDef

```python
# AudienceMediaTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import AudienceMediaTypeDef


def get_value() -> AudienceMediaTypeDef:
    return {
        "Audience": ...,
    }


# AudienceMediaTypeDef definition

class AudienceMediaTypeDef(TypedDict):
    Audience: NotRequired[str],
    AlternateMedia: NotRequired[Sequence[AlternateMediaUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: AlternateMediaTypeDef](./type_defs.md#alternatemediatypedef) [:material-code-braces: AlternateMediaOutputTypeDef](./type_defs.md#alternatemediaoutputtypedef) 
## CreateProgramRequestTypeDef

```python
# CreateProgramRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import CreateProgramRequestTypeDef


def get_value() -> CreateProgramRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# CreateProgramRequestTypeDef definition

class CreateProgramRequestTypeDef(TypedDict):
    ChannelName: str,
    ProgramName: str,
    ScheduleConfiguration: ScheduleConfigurationTypeDef,  # (1)
    SourceLocationName: str,
    AdBreaks: NotRequired[Sequence[AdBreakUnionTypeDef]],  # (2)
    LiveSourceName: NotRequired[str],
    VodSourceName: NotRequired[str],
    AudienceMedia: NotRequired[Sequence[AudienceMediaUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
2. See [:material-code-braces: AdBreakTypeDef](./type_defs.md#adbreaktypedef) [:material-code-braces: AdBreakOutputTypeDef](./type_defs.md#adbreakoutputtypedef) 
3. See [:material-code-braces: AudienceMediaTypeDef](./type_defs.md#audiencemediatypedef) [:material-code-braces: AudienceMediaOutputTypeDef](./type_defs.md#audiencemediaoutputtypedef) 
## UpdateProgramRequestTypeDef

```python
# UpdateProgramRequestTypeDef TypedDict usage example

from types_aiobotocore_mediatailor.type_defs import UpdateProgramRequestTypeDef


def get_value() -> UpdateProgramRequestTypeDef:
    return {
        "ChannelName": ...,
    }


# UpdateProgramRequestTypeDef definition

class UpdateProgramRequestTypeDef(TypedDict):
    ChannelName: str,
    ProgramName: str,
    ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,  # (1)
    AdBreaks: NotRequired[Sequence[AdBreakUnionTypeDef]],  # (2)
    AudienceMedia: NotRequired[Sequence[AudienceMediaUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: UpdateProgramScheduleConfigurationTypeDef](./type_defs.md#updateprogramscheduleconfigurationtypedef) 
2. See [:material-code-braces: AdBreakTypeDef](./type_defs.md#adbreaktypedef) [:material-code-braces: AdBreakOutputTypeDef](./type_defs.md#adbreakoutputtypedef) 
3. See [:material-code-braces: AudienceMediaTypeDef](./type_defs.md#audiencemediatypedef) [:material-code-braces: AudienceMediaOutputTypeDef](./type_defs.md#audiencemediaoutputtypedef) 
