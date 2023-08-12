# Type definitions

> [Index](../README.md) > [MediaTailor](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MediaTailor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
    type annotations stubs module [types-aiobotocore-mediatailor](https://pypi.org/project/types-aiobotocore-mediatailor/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## SecretsManagerAccessTokenConfigurationTypeDef

```python
# SecretsManagerAccessTokenConfigurationTypeDef definition

class SecretsManagerAccessTokenConfigurationTypeDef(TypedDict):
    HeaderName: NotRequired[str],
    SecretArn: NotRequired[str],
    SecretStringKey: NotRequired[str],
```

## KeyValuePairTypeDef

```python
# KeyValuePairTypeDef definition

class KeyValuePairTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## SlateSourceTypeDef

```python
# SlateSourceTypeDef definition

class SlateSourceTypeDef(TypedDict):
    SourceLocationName: NotRequired[str],
    VodSourceName: NotRequired[str],
```

## SpliceInsertMessageTypeDef

```python
# SpliceInsertMessageTypeDef definition

class SpliceInsertMessageTypeDef(TypedDict):
    AvailNum: NotRequired[int],
    AvailsExpected: NotRequired[int],
    SpliceEventId: NotRequired[int],
    UniqueProgramId: NotRequired[int],
```

## AdMarkerPassthroughTypeDef

```python
# AdMarkerPassthroughTypeDef definition

class AdMarkerPassthroughTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## AlertTypeDef

```python
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
## AvailMatchingCriteriaTypeDef

```python
# AvailMatchingCriteriaTypeDef definition

class AvailMatchingCriteriaTypeDef(TypedDict):
    DynamicVariable: str,
    Operator: OperatorType,  # (1)
```

1. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## AvailSuppressionTypeDef

```python
# AvailSuppressionTypeDef definition

class AvailSuppressionTypeDef(TypedDict):
    FillPolicy: NotRequired[FillPolicyType],  # (1)
    Mode: NotRequired[ModeType],  # (2)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: FillPolicyType](./literals.md#fillpolicytype) 
2. See [:material-code-brackets: ModeType](./literals.md#modetype) 
## BumperTypeDef

```python
# BumperTypeDef definition

class BumperTypeDef(TypedDict):
    EndUrl: NotRequired[str],
    StartUrl: NotRequired[str],
```

## CdnConfigurationTypeDef

```python
# CdnConfigurationTypeDef definition

class CdnConfigurationTypeDef(TypedDict):
    AdSegmentUrlPrefix: NotRequired[str],
    ContentSegmentUrlPrefix: NotRequired[str],
```

## LogConfigurationForChannelTypeDef

```python
# LogConfigurationForChannelTypeDef definition

class LogConfigurationForChannelTypeDef(TypedDict):
    LogTypes: NotRequired[List[LogTypeType]],  # (1)
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
## ClipRangeTypeDef

```python
# ClipRangeTypeDef definition

class ClipRangeTypeDef(TypedDict):
    EndOffsetMillis: int,
```

## ConfigureLogsForChannelRequestRequestTypeDef

```python
# ConfigureLogsForChannelRequestRequestTypeDef definition

class ConfigureLogsForChannelRequestRequestTypeDef(TypedDict):
    ChannelName: str,
    LogTypes: Sequence[LogTypeType],  # (1)
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
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

## ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef

```python
# ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef definition

class ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef(TypedDict):
    PercentEnabled: int,
    PlaybackConfigurationName: str,
```

## HttpPackageConfigurationTypeDef

```python
# HttpPackageConfigurationTypeDef definition

class HttpPackageConfigurationTypeDef(TypedDict):
    Path: str,
    SourceGroup: str,
    Type: TypeType,  # (1)
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## DefaultSegmentDeliveryConfigurationTypeDef

```python
# DefaultSegmentDeliveryConfigurationTypeDef definition

class DefaultSegmentDeliveryConfigurationTypeDef(TypedDict):
    BaseUrl: NotRequired[str],
```

## HttpConfigurationTypeDef

```python
# HttpConfigurationTypeDef definition

class HttpConfigurationTypeDef(TypedDict):
    BaseUrl: str,
```

## SegmentDeliveryConfigurationTypeDef

```python
# SegmentDeliveryConfigurationTypeDef definition

class SegmentDeliveryConfigurationTypeDef(TypedDict):
    BaseUrl: NotRequired[str],
    Name: NotRequired[str],
```

## DashConfigurationForPutTypeDef

```python
# DashConfigurationForPutTypeDef definition

class DashConfigurationForPutTypeDef(TypedDict):
    MpdLocation: NotRequired[str],
    OriginManifestType: NotRequired[OriginManifestTypeType],  # (1)
```

1. See [:material-code-brackets: OriginManifestTypeType](./literals.md#originmanifesttypetype) 
## DashConfigurationTypeDef

```python
# DashConfigurationTypeDef definition

class DashConfigurationTypeDef(TypedDict):
    ManifestEndpointPrefix: NotRequired[str],
    MpdLocation: NotRequired[str],
    OriginManifestType: NotRequired[OriginManifestTypeType],  # (1)
```

1. See [:material-code-brackets: OriginManifestTypeType](./literals.md#originmanifesttypetype) 
## DashPlaylistSettingsTypeDef

```python
# DashPlaylistSettingsTypeDef definition

class DashPlaylistSettingsTypeDef(TypedDict):
    ManifestWindowSeconds: NotRequired[int],
    MinBufferTimeSeconds: NotRequired[int],
    MinUpdatePeriodSeconds: NotRequired[int],
    SuggestedPresentationDelaySeconds: NotRequired[int],
```

## DeleteChannelPolicyRequestRequestTypeDef

```python
# DeleteChannelPolicyRequestRequestTypeDef definition

class DeleteChannelPolicyRequestRequestTypeDef(TypedDict):
    ChannelName: str,
```

## DeleteChannelRequestRequestTypeDef

```python
# DeleteChannelRequestRequestTypeDef definition

class DeleteChannelRequestRequestTypeDef(TypedDict):
    ChannelName: str,
```

## DeleteLiveSourceRequestRequestTypeDef

```python
# DeleteLiveSourceRequestRequestTypeDef definition

class DeleteLiveSourceRequestRequestTypeDef(TypedDict):
    LiveSourceName: str,
    SourceLocationName: str,
```

## DeletePlaybackConfigurationRequestRequestTypeDef

```python
# DeletePlaybackConfigurationRequestRequestTypeDef definition

class DeletePlaybackConfigurationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeletePrefetchScheduleRequestRequestTypeDef

```python
# DeletePrefetchScheduleRequestRequestTypeDef definition

class DeletePrefetchScheduleRequestRequestTypeDef(TypedDict):
    Name: str,
    PlaybackConfigurationName: str,
```

## DeleteProgramRequestRequestTypeDef

```python
# DeleteProgramRequestRequestTypeDef definition

class DeleteProgramRequestRequestTypeDef(TypedDict):
    ChannelName: str,
    ProgramName: str,
```

## DeleteSourceLocationRequestRequestTypeDef

```python
# DeleteSourceLocationRequestRequestTypeDef definition

class DeleteSourceLocationRequestRequestTypeDef(TypedDict):
    SourceLocationName: str,
```

## DeleteVodSourceRequestRequestTypeDef

```python
# DeleteVodSourceRequestRequestTypeDef definition

class DeleteVodSourceRequestRequestTypeDef(TypedDict):
    SourceLocationName: str,
    VodSourceName: str,
```

## DescribeChannelRequestRequestTypeDef

```python
# DescribeChannelRequestRequestTypeDef definition

class DescribeChannelRequestRequestTypeDef(TypedDict):
    ChannelName: str,
```

## DescribeLiveSourceRequestRequestTypeDef

```python
# DescribeLiveSourceRequestRequestTypeDef definition

class DescribeLiveSourceRequestRequestTypeDef(TypedDict):
    LiveSourceName: str,
    SourceLocationName: str,
```

## DescribeProgramRequestRequestTypeDef

```python
# DescribeProgramRequestRequestTypeDef definition

class DescribeProgramRequestRequestTypeDef(TypedDict):
    ChannelName: str,
    ProgramName: str,
```

## DescribeSourceLocationRequestRequestTypeDef

```python
# DescribeSourceLocationRequestRequestTypeDef definition

class DescribeSourceLocationRequestRequestTypeDef(TypedDict):
    SourceLocationName: str,
```

## DescribeVodSourceRequestRequestTypeDef

```python
# DescribeVodSourceRequestRequestTypeDef definition

class DescribeVodSourceRequestRequestTypeDef(TypedDict):
    SourceLocationName: str,
    VodSourceName: str,
```

## GetChannelPolicyRequestRequestTypeDef

```python
# GetChannelPolicyRequestRequestTypeDef definition

class GetChannelPolicyRequestRequestTypeDef(TypedDict):
    ChannelName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetChannelScheduleRequestRequestTypeDef

```python
# GetChannelScheduleRequestRequestTypeDef definition

class GetChannelScheduleRequestRequestTypeDef(TypedDict):
    ChannelName: str,
    DurationMinutes: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetPlaybackConfigurationRequestRequestTypeDef

```python
# GetPlaybackConfigurationRequestRequestTypeDef definition

class GetPlaybackConfigurationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## HlsConfigurationTypeDef

```python
# HlsConfigurationTypeDef definition

class HlsConfigurationTypeDef(TypedDict):
    ManifestEndpointPrefix: NotRequired[str],
```

## LivePreRollConfigurationTypeDef

```python
# LivePreRollConfigurationTypeDef definition

class LivePreRollConfigurationTypeDef(TypedDict):
    AdDecisionServerUrl: NotRequired[str],
    MaxDurationSeconds: NotRequired[int],
```

## LogConfigurationTypeDef

```python
# LogConfigurationTypeDef definition

class LogConfigurationTypeDef(TypedDict):
    PercentEnabled: int,
```

## GetPrefetchScheduleRequestRequestTypeDef

```python
# GetPrefetchScheduleRequestRequestTypeDef definition

class GetPrefetchScheduleRequestRequestTypeDef(TypedDict):
    Name: str,
    PlaybackConfigurationName: str,
```

## HlsPlaylistSettingsTypeDef

```python
# HlsPlaylistSettingsTypeDef definition

class HlsPlaylistSettingsTypeDef(TypedDict):
    AdMarkupType: NotRequired[Sequence[AdMarkupTypeType]],  # (1)
    ManifestWindowSeconds: NotRequired[int],
```

1. See [:material-code-brackets: AdMarkupTypeType](./literals.md#admarkuptypetype) 
## ListAlertsRequestRequestTypeDef

```python
# ListAlertsRequestRequestTypeDef definition

class ListAlertsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListChannelsRequestRequestTypeDef

```python
# ListChannelsRequestRequestTypeDef definition

class ListChannelsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListLiveSourcesRequestRequestTypeDef

```python
# ListLiveSourcesRequestRequestTypeDef definition

class ListLiveSourcesRequestRequestTypeDef(TypedDict):
    SourceLocationName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListPlaybackConfigurationsRequestRequestTypeDef

```python
# ListPlaybackConfigurationsRequestRequestTypeDef definition

class ListPlaybackConfigurationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListPrefetchSchedulesRequestRequestTypeDef

```python
# ListPrefetchSchedulesRequestRequestTypeDef definition

class ListPrefetchSchedulesRequestRequestTypeDef(TypedDict):
    PlaybackConfigurationName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    StreamId: NotRequired[str],
```

## ListSourceLocationsRequestRequestTypeDef

```python
# ListSourceLocationsRequestRequestTypeDef definition

class ListSourceLocationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListVodSourcesRequestRequestTypeDef

```python
# ListVodSourcesRequestRequestTypeDef definition

class ListVodSourcesRequestRequestTypeDef(TypedDict):
    SourceLocationName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PutChannelPolicyRequestRequestTypeDef

```python
# PutChannelPolicyRequestRequestTypeDef definition

class PutChannelPolicyRequestRequestTypeDef(TypedDict):
    ChannelName: str,
    Policy: str,
```

## ScheduleAdBreakTypeDef

```python
# ScheduleAdBreakTypeDef definition

class ScheduleAdBreakTypeDef(TypedDict):
    ApproximateDurationSeconds: NotRequired[int],
    ApproximateStartTime: NotRequired[datetime],
    SourceLocationName: NotRequired[str],
    VodSourceName: NotRequired[str],
```

## TransitionTypeDef

```python
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
# SegmentationDescriptorTypeDef definition

class SegmentationDescriptorTypeDef(TypedDict):
    SegmentNum: NotRequired[int],
    SegmentationEventId: NotRequired[int],
    SegmentationTypeId: NotRequired[int],
    SegmentationUpid: NotRequired[str],
    SegmentationUpidType: NotRequired[int],
    SegmentsExpected: NotRequired[int],
    SubSegmentNum: NotRequired[int],
    SubSegmentsExpected: NotRequired[int],
```

## StartChannelRequestRequestTypeDef

```python
# StartChannelRequestRequestTypeDef definition

class StartChannelRequestRequestTypeDef(TypedDict):
    ChannelName: str,
```

## StopChannelRequestRequestTypeDef

```python
# StopChannelRequestRequestTypeDef definition

class StopChannelRequestRequestTypeDef(TypedDict):
    ChannelName: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateProgramTransitionTypeDef

```python
# UpdateProgramTransitionTypeDef definition

class UpdateProgramTransitionTypeDef(TypedDict):
    DurationMillis: NotRequired[int],
    ScheduledStartTimeMillis: NotRequired[int],
```

## AccessConfigurationTypeDef

```python
# AccessConfigurationTypeDef definition

class AccessConfigurationTypeDef(TypedDict):
    AccessType: NotRequired[AccessTypeType],  # (1)
    SecretsManagerAccessTokenConfiguration: NotRequired[SecretsManagerAccessTokenConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: AccessTypeType](./literals.md#accesstypetype) 
2. See [:material-code-braces: SecretsManagerAccessTokenConfigurationTypeDef](./type_defs.md#secretsmanageraccesstokenconfigurationtypedef) 
## ManifestProcessingRulesTypeDef

```python
# ManifestProcessingRulesTypeDef definition

class ManifestProcessingRulesTypeDef(TypedDict):
    AdMarkerPassthrough: NotRequired[AdMarkerPassthroughTypeDef],  # (1)
```

1. See [:material-code-braces: AdMarkerPassthroughTypeDef](./type_defs.md#admarkerpassthroughtypedef) 
## ConfigureLogsForChannelResponseTypeDef

```python
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
# ConfigureLogsForPlaybackConfigurationResponseTypeDef definition

class ConfigureLogsForPlaybackConfigurationResponseTypeDef(TypedDict):
    PercentEnabled: int,
    PlaybackConfigurationName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChannelPolicyResponseTypeDef

```python
# GetChannelPolicyResponseTypeDef definition

class GetChannelPolicyResponseTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAlertsResponseTypeDef

```python
# ListAlertsResponseTypeDef definition

class ListAlertsResponseTypeDef(TypedDict):
    Items: List[AlertTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlertTypeDef](./type_defs.md#alerttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLiveSourceRequestRequestTypeDef

```python
# CreateLiveSourceRequestRequestTypeDef definition

class CreateLiveSourceRequestRequestTypeDef(TypedDict):
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    LiveSourceName: str,
    SourceLocationName: str,
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
## CreateLiveSourceResponseTypeDef

```python
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
## CreateVodSourceRequestRequestTypeDef

```python
# CreateVodSourceRequestRequestTypeDef definition

class CreateVodSourceRequestRequestTypeDef(TypedDict):
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    SourceLocationName: str,
    VodSourceName: str,
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
## CreateVodSourceResponseTypeDef

```python
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
# DescribeVodSourceResponseTypeDef definition

class DescribeVodSourceResponseTypeDef(TypedDict):
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
## LiveSourceTypeDef

```python
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
## UpdateLiveSourceRequestRequestTypeDef

```python
# UpdateLiveSourceRequestRequestTypeDef definition

class UpdateLiveSourceRequestRequestTypeDef(TypedDict):
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    LiveSourceName: str,
    SourceLocationName: str,
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
## UpdateLiveSourceResponseTypeDef

```python
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
## UpdateVodSourceRequestRequestTypeDef

```python
# UpdateVodSourceRequestRequestTypeDef definition

class UpdateVodSourceRequestRequestTypeDef(TypedDict):
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    SourceLocationName: str,
    VodSourceName: str,
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
## UpdateVodSourceResponseTypeDef

```python
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
## GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef

```python
# GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef definition

class GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef(TypedDict):
    ChannelName: str,
    DurationMinutes: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAlertsRequestListAlertsPaginateTypeDef

```python
# ListAlertsRequestListAlertsPaginateTypeDef definition

class ListAlertsRequestListAlertsPaginateTypeDef(TypedDict):
    ResourceArn: str,
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
## ListLiveSourcesRequestListLiveSourcesPaginateTypeDef

```python
# ListLiveSourcesRequestListLiveSourcesPaginateTypeDef definition

class ListLiveSourcesRequestListLiveSourcesPaginateTypeDef(TypedDict):
    SourceLocationName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef

```python
# ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef definition

class ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef

```python
# ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef definition

class ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef(TypedDict):
    PlaybackConfigurationName: str,
    StreamId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSourceLocationsRequestListSourceLocationsPaginateTypeDef

```python
# ListSourceLocationsRequestListSourceLocationsPaginateTypeDef definition

class ListSourceLocationsRequestListSourceLocationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVodSourcesRequestListVodSourcesPaginateTypeDef

```python
# ListVodSourcesRequestListVodSourcesPaginateTypeDef definition

class ListVodSourcesRequestListVodSourcesPaginateTypeDef(TypedDict):
    SourceLocationName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## RequestOutputItemTypeDef

```python
# RequestOutputItemTypeDef definition

class RequestOutputItemTypeDef(TypedDict):
    ManifestName: str,
    SourceGroup: str,
    DashPlaylistSettings: NotRequired[DashPlaylistSettingsTypeDef],  # (1)
    HlsPlaylistSettings: NotRequired[HlsPlaylistSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: DashPlaylistSettingsTypeDef](./type_defs.md#dashplaylistsettingstypedef) 
2. See [:material-code-braces: HlsPlaylistSettingsTypeDef](./type_defs.md#hlsplaylistsettingstypedef) 
## ResponseOutputItemTypeDef

```python
# ResponseOutputItemTypeDef definition

class ResponseOutputItemTypeDef(TypedDict):
    ManifestName: str,
    PlaybackUrl: str,
    SourceGroup: str,
    DashPlaylistSettings: NotRequired[DashPlaylistSettingsTypeDef],  # (1)
    HlsPlaylistSettings: NotRequired[HlsPlaylistSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: DashPlaylistSettingsTypeDef](./type_defs.md#dashplaylistsettingstypedef) 
2. See [:material-code-braces: HlsPlaylistSettingsTypeDef](./type_defs.md#hlsplaylistsettingstypedef) 
## PrefetchConsumptionTypeDef

```python
# PrefetchConsumptionTypeDef definition

class PrefetchConsumptionTypeDef(TypedDict):
    EndTime: Union[datetime, str],
    AvailMatchingCriteria: NotRequired[Sequence[AvailMatchingCriteriaTypeDef]],  # (1)
    StartTime: NotRequired[Union[datetime, str]],
```

1. See [:material-code-braces: AvailMatchingCriteriaTypeDef](./type_defs.md#availmatchingcriteriatypedef) 
## PrefetchRetrievalTypeDef

```python
# PrefetchRetrievalTypeDef definition

class PrefetchRetrievalTypeDef(TypedDict):
    EndTime: Union[datetime, str],
    DynamicVariables: NotRequired[Mapping[str, str]],
    StartTime: NotRequired[Union[datetime, str]],
```

## ScheduleEntryTypeDef

```python
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
```

1. See [:material-code-braces: ScheduleAdBreakTypeDef](./type_defs.md#scheduleadbreaktypedef) 
2. See [:material-code-brackets: ScheduleEntryTypeType](./literals.md#scheduleentrytypetype) 
## ScheduleConfigurationTypeDef

```python
# ScheduleConfigurationTypeDef definition

class ScheduleConfigurationTypeDef(TypedDict):
    Transition: TransitionTypeDef,  # (2)
    ClipRange: NotRequired[ClipRangeTypeDef],  # (1)
```

1. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
2. See [:material-code-braces: TransitionTypeDef](./type_defs.md#transitiontypedef) 
## TimeSignalMessageTypeDef

```python
# TimeSignalMessageTypeDef definition

class TimeSignalMessageTypeDef(TypedDict):
    SegmentationDescriptors: NotRequired[Sequence[SegmentationDescriptorTypeDef]],  # (1)
```

1. See [:material-code-braces: SegmentationDescriptorTypeDef](./type_defs.md#segmentationdescriptortypedef) 
## UpdateProgramScheduleConfigurationTypeDef

```python
# UpdateProgramScheduleConfigurationTypeDef definition

class UpdateProgramScheduleConfigurationTypeDef(TypedDict):
    ClipRange: NotRequired[ClipRangeTypeDef],  # (1)
    Transition: NotRequired[UpdateProgramTransitionTypeDef],  # (2)
```

1. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
2. See [:material-code-braces: UpdateProgramTransitionTypeDef](./type_defs.md#updateprogramtransitiontypedef) 
## CreateSourceLocationRequestRequestTypeDef

```python
# CreateSourceLocationRequestRequestTypeDef definition

class CreateSourceLocationRequestRequestTypeDef(TypedDict):
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
## UpdateSourceLocationRequestRequestTypeDef

```python
# UpdateSourceLocationRequestRequestTypeDef definition

class UpdateSourceLocationRequestRequestTypeDef(TypedDict):
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
# GetPlaybackConfigurationResponseTypeDef definition

class GetPlaybackConfigurationResponseTypeDef(TypedDict):
    AdDecisionServerUrl: str,
    AvailSuppression: AvailSuppressionTypeDef,  # (1)
    Bumper: BumperTypeDef,  # (2)
    CdnConfiguration: CdnConfigurationTypeDef,  # (3)
    ConfigurationAliases: Dict[str, Dict[str, str]],
    DashConfiguration: DashConfigurationTypeDef,  # (4)
    HlsConfiguration: HlsConfigurationTypeDef,  # (5)
    LivePreRollConfiguration: LivePreRollConfigurationTypeDef,  # (6)
    LogConfiguration: LogConfigurationTypeDef,  # (7)
    ManifestProcessingRules: ManifestProcessingRulesTypeDef,  # (8)
    Name: str,
    PersonalizationThresholdSeconds: int,
    PlaybackConfigurationArn: str,
    PlaybackEndpointPrefix: str,
    SessionInitializationEndpointPrefix: str,
    SlateAdUrl: str,
    Tags: Dict[str, str],
    TranscodeProfileName: str,
    VideoContentSourceUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-braces: AvailSuppressionTypeDef](./type_defs.md#availsuppressiontypedef) 
2. See [:material-code-braces: BumperTypeDef](./type_defs.md#bumpertypedef) 
3. See [:material-code-braces: CdnConfigurationTypeDef](./type_defs.md#cdnconfigurationtypedef) 
4. See [:material-code-braces: DashConfigurationTypeDef](./type_defs.md#dashconfigurationtypedef) 
5. See [:material-code-braces: HlsConfigurationTypeDef](./type_defs.md#hlsconfigurationtypedef) 
6. See [:material-code-braces: LivePreRollConfigurationTypeDef](./type_defs.md#liveprerollconfigurationtypedef) 
7. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
8. See [:material-code-braces: ManifestProcessingRulesTypeDef](./type_defs.md#manifestprocessingrulestypedef) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PlaybackConfigurationTypeDef

```python
# PlaybackConfigurationTypeDef definition

class PlaybackConfigurationTypeDef(TypedDict):
    AdDecisionServerUrl: NotRequired[str],
    AvailSuppression: NotRequired[AvailSuppressionTypeDef],  # (1)
    Bumper: NotRequired[BumperTypeDef],  # (2)
    CdnConfiguration: NotRequired[CdnConfigurationTypeDef],  # (3)
    ConfigurationAliases: NotRequired[Dict[str, Dict[str, str]]],
    DashConfiguration: NotRequired[DashConfigurationTypeDef],  # (4)
    HlsConfiguration: NotRequired[HlsConfigurationTypeDef],  # (5)
    LivePreRollConfiguration: NotRequired[LivePreRollConfigurationTypeDef],  # (6)
    LogConfiguration: NotRequired[LogConfigurationTypeDef],  # (7)
    ManifestProcessingRules: NotRequired[ManifestProcessingRulesTypeDef],  # (8)
    Name: NotRequired[str],
    PersonalizationThresholdSeconds: NotRequired[int],
    PlaybackConfigurationArn: NotRequired[str],
    PlaybackEndpointPrefix: NotRequired[str],
    SessionInitializationEndpointPrefix: NotRequired[str],
    SlateAdUrl: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    TranscodeProfileName: NotRequired[str],
    VideoContentSourceUrl: NotRequired[str],
```

1. See [:material-code-braces: AvailSuppressionTypeDef](./type_defs.md#availsuppressiontypedef) 
2. See [:material-code-braces: BumperTypeDef](./type_defs.md#bumpertypedef) 
3. See [:material-code-braces: CdnConfigurationTypeDef](./type_defs.md#cdnconfigurationtypedef) 
4. See [:material-code-braces: DashConfigurationTypeDef](./type_defs.md#dashconfigurationtypedef) 
5. See [:material-code-braces: HlsConfigurationTypeDef](./type_defs.md#hlsconfigurationtypedef) 
6. See [:material-code-braces: LivePreRollConfigurationTypeDef](./type_defs.md#liveprerollconfigurationtypedef) 
7. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
8. See [:material-code-braces: ManifestProcessingRulesTypeDef](./type_defs.md#manifestprocessingrulestypedef) 
## PutPlaybackConfigurationRequestRequestTypeDef

```python
# PutPlaybackConfigurationRequestRequestTypeDef definition

class PutPlaybackConfigurationRequestRequestTypeDef(TypedDict):
    Name: str,
    AdDecisionServerUrl: NotRequired[str],
    AvailSuppression: NotRequired[AvailSuppressionTypeDef],  # (1)
    Bumper: NotRequired[BumperTypeDef],  # (2)
    CdnConfiguration: NotRequired[CdnConfigurationTypeDef],  # (3)
    ConfigurationAliases: NotRequired[Mapping[str, Mapping[str, str]]],
    DashConfiguration: NotRequired[DashConfigurationForPutTypeDef],  # (4)
    LivePreRollConfiguration: NotRequired[LivePreRollConfigurationTypeDef],  # (5)
    ManifestProcessingRules: NotRequired[ManifestProcessingRulesTypeDef],  # (6)
    PersonalizationThresholdSeconds: NotRequired[int],
    SlateAdUrl: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    TranscodeProfileName: NotRequired[str],
    VideoContentSourceUrl: NotRequired[str],
```

1. See [:material-code-braces: AvailSuppressionTypeDef](./type_defs.md#availsuppressiontypedef) 
2. See [:material-code-braces: BumperTypeDef](./type_defs.md#bumpertypedef) 
3. See [:material-code-braces: CdnConfigurationTypeDef](./type_defs.md#cdnconfigurationtypedef) 
4. See [:material-code-braces: DashConfigurationForPutTypeDef](./type_defs.md#dashconfigurationforputtypedef) 
5. See [:material-code-braces: LivePreRollConfigurationTypeDef](./type_defs.md#liveprerollconfigurationtypedef) 
6. See [:material-code-braces: ManifestProcessingRulesTypeDef](./type_defs.md#manifestprocessingrulestypedef) 
## PutPlaybackConfigurationResponseTypeDef

```python
# PutPlaybackConfigurationResponseTypeDef definition

class PutPlaybackConfigurationResponseTypeDef(TypedDict):
    AdDecisionServerUrl: str,
    AvailSuppression: AvailSuppressionTypeDef,  # (1)
    Bumper: BumperTypeDef,  # (2)
    CdnConfiguration: CdnConfigurationTypeDef,  # (3)
    ConfigurationAliases: Dict[str, Dict[str, str]],
    DashConfiguration: DashConfigurationTypeDef,  # (4)
    HlsConfiguration: HlsConfigurationTypeDef,  # (5)
    LivePreRollConfiguration: LivePreRollConfigurationTypeDef,  # (6)
    LogConfiguration: LogConfigurationTypeDef,  # (7)
    ManifestProcessingRules: ManifestProcessingRulesTypeDef,  # (8)
    Name: str,
    PersonalizationThresholdSeconds: int,
    PlaybackConfigurationArn: str,
    PlaybackEndpointPrefix: str,
    SessionInitializationEndpointPrefix: str,
    SlateAdUrl: str,
    Tags: Dict[str, str],
    TranscodeProfileName: str,
    VideoContentSourceUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-braces: AvailSuppressionTypeDef](./type_defs.md#availsuppressiontypedef) 
2. See [:material-code-braces: BumperTypeDef](./type_defs.md#bumpertypedef) 
3. See [:material-code-braces: CdnConfigurationTypeDef](./type_defs.md#cdnconfigurationtypedef) 
4. See [:material-code-braces: DashConfigurationTypeDef](./type_defs.md#dashconfigurationtypedef) 
5. See [:material-code-braces: HlsConfigurationTypeDef](./type_defs.md#hlsconfigurationtypedef) 
6. See [:material-code-braces: LivePreRollConfigurationTypeDef](./type_defs.md#liveprerollconfigurationtypedef) 
7. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
8. See [:material-code-braces: ManifestProcessingRulesTypeDef](./type_defs.md#manifestprocessingrulestypedef) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLiveSourcesResponseTypeDef

```python
# ListLiveSourcesResponseTypeDef definition

class ListLiveSourcesResponseTypeDef(TypedDict):
    Items: List[LiveSourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LiveSourceTypeDef](./type_defs.md#livesourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVodSourcesResponseTypeDef

```python
# ListVodSourcesResponseTypeDef definition

class ListVodSourcesResponseTypeDef(TypedDict):
    Items: List[VodSourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VodSourceTypeDef](./type_defs.md#vodsourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelRequestRequestTypeDef

```python
# CreateChannelRequestRequestTypeDef definition

class CreateChannelRequestRequestTypeDef(TypedDict):
    ChannelName: str,
    Outputs: Sequence[RequestOutputItemTypeDef],  # (1)
    PlaybackMode: PlaybackModeType,  # (2)
    FillerSlate: NotRequired[SlateSourceTypeDef],  # (3)
    Tags: NotRequired[Mapping[str, str]],
    Tier: NotRequired[TierType],  # (4)
```

1. See [:material-code-braces: RequestOutputItemTypeDef](./type_defs.md#requestoutputitemtypedef) 
2. See [:material-code-brackets: PlaybackModeType](./literals.md#playbackmodetype) 
3. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
4. See [:material-code-brackets: TierType](./literals.md#tiertype) 
## UpdateChannelRequestRequestTypeDef

```python
# UpdateChannelRequestRequestTypeDef definition

class UpdateChannelRequestRequestTypeDef(TypedDict):
    ChannelName: str,
    Outputs: Sequence[RequestOutputItemTypeDef],  # (1)
    FillerSlate: NotRequired[SlateSourceTypeDef],  # (2)
```

1. See [:material-code-braces: RequestOutputItemTypeDef](./type_defs.md#requestoutputitemtypedef) 
2. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
## ChannelTypeDef

```python
# ChannelTypeDef definition

class ChannelTypeDef(TypedDict):
    Arn: str,
    ChannelName: str,
    ChannelState: str,
    LogConfiguration: LogConfigurationForChannelTypeDef,  # (2)
    Outputs: List[ResponseOutputItemTypeDef],  # (3)
    PlaybackMode: str,
    Tier: str,
    CreationTime: NotRequired[datetime],
    FillerSlate: NotRequired[SlateSourceTypeDef],  # (1)
    LastModifiedTime: NotRequired[datetime],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
2. See [:material-code-braces: LogConfigurationForChannelTypeDef](./type_defs.md#logconfigurationforchanneltypedef) 
3. See [:material-code-braces: ResponseOutputItemTypeDef](./type_defs.md#responseoutputitemtypedef) 
## CreateChannelResponseTypeDef

```python
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
2. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
3. See [:material-code-braces: ResponseOutputItemTypeDef](./type_defs.md#responseoutputitemtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelResponseTypeDef

```python
# DescribeChannelResponseTypeDef definition

class DescribeChannelResponseTypeDef(TypedDict):
    Arn: str,
    ChannelName: str,
    ChannelState: ChannelStateType,  # (1)
    CreationTime: datetime,
    FillerSlate: SlateSourceTypeDef,  # (2)
    LastModifiedTime: datetime,
    LogConfiguration: LogConfigurationForChannelTypeDef,  # (3)
    Outputs: List[ResponseOutputItemTypeDef],  # (4)
    PlaybackMode: str,
    Tags: Dict[str, str],
    Tier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
2. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
3. See [:material-code-braces: LogConfigurationForChannelTypeDef](./type_defs.md#logconfigurationforchanneltypedef) 
4. See [:material-code-braces: ResponseOutputItemTypeDef](./type_defs.md#responseoutputitemtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelResponseTypeDef

```python
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ChannelStateType](./literals.md#channelstatetype) 
2. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
3. See [:material-code-braces: ResponseOutputItemTypeDef](./type_defs.md#responseoutputitemtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePrefetchScheduleRequestRequestTypeDef

```python
# CreatePrefetchScheduleRequestRequestTypeDef definition

class CreatePrefetchScheduleRequestRequestTypeDef(TypedDict):
    Consumption: PrefetchConsumptionTypeDef,  # (1)
    Name: str,
    PlaybackConfigurationName: str,
    Retrieval: PrefetchRetrievalTypeDef,  # (2)
    StreamId: NotRequired[str],
```

1. See [:material-code-braces: PrefetchConsumptionTypeDef](./type_defs.md#prefetchconsumptiontypedef) 
2. See [:material-code-braces: PrefetchRetrievalTypeDef](./type_defs.md#prefetchretrievaltypedef) 
## CreatePrefetchScheduleResponseTypeDef

```python
# CreatePrefetchScheduleResponseTypeDef definition

class CreatePrefetchScheduleResponseTypeDef(TypedDict):
    Arn: str,
    Consumption: PrefetchConsumptionTypeDef,  # (1)
    Name: str,
    PlaybackConfigurationName: str,
    Retrieval: PrefetchRetrievalTypeDef,  # (2)
    StreamId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PrefetchConsumptionTypeDef](./type_defs.md#prefetchconsumptiontypedef) 
2. See [:material-code-braces: PrefetchRetrievalTypeDef](./type_defs.md#prefetchretrievaltypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPrefetchScheduleResponseTypeDef

```python
# GetPrefetchScheduleResponseTypeDef definition

class GetPrefetchScheduleResponseTypeDef(TypedDict):
    Arn: str,
    Consumption: PrefetchConsumptionTypeDef,  # (1)
    Name: str,
    PlaybackConfigurationName: str,
    Retrieval: PrefetchRetrievalTypeDef,  # (2)
    StreamId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PrefetchConsumptionTypeDef](./type_defs.md#prefetchconsumptiontypedef) 
2. See [:material-code-braces: PrefetchRetrievalTypeDef](./type_defs.md#prefetchretrievaltypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PrefetchScheduleTypeDef

```python
# PrefetchScheduleTypeDef definition

class PrefetchScheduleTypeDef(TypedDict):
    Arn: str,
    Consumption: PrefetchConsumptionTypeDef,  # (1)
    Name: str,
    PlaybackConfigurationName: str,
    Retrieval: PrefetchRetrievalTypeDef,  # (2)
    StreamId: NotRequired[str],
```

1. See [:material-code-braces: PrefetchConsumptionTypeDef](./type_defs.md#prefetchconsumptiontypedef) 
2. See [:material-code-braces: PrefetchRetrievalTypeDef](./type_defs.md#prefetchretrievaltypedef) 
## GetChannelScheduleResponseTypeDef

```python
# GetChannelScheduleResponseTypeDef definition

class GetChannelScheduleResponseTypeDef(TypedDict):
    Items: List[ScheduleEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduleEntryTypeDef](./type_defs.md#scheduleentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdBreakTypeDef

```python
# AdBreakTypeDef definition

class AdBreakTypeDef(TypedDict):
    AdBreakMetadata: NotRequired[Sequence[KeyValuePairTypeDef]],  # (1)
    MessageType: NotRequired[MessageTypeType],  # (2)
    OffsetMillis: NotRequired[int],
    Slate: NotRequired[SlateSourceTypeDef],  # (3)
    SpliceInsertMessage: NotRequired[SpliceInsertMessageTypeDef],  # (4)
    TimeSignalMessage: NotRequired[TimeSignalMessageTypeDef],  # (5)
```

1. See [:material-code-braces: KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
4. See [:material-code-braces: SpliceInsertMessageTypeDef](./type_defs.md#spliceinsertmessagetypedef) 
5. See [:material-code-braces: TimeSignalMessageTypeDef](./type_defs.md#timesignalmessagetypedef) 
## ListSourceLocationsResponseTypeDef

```python
# ListSourceLocationsResponseTypeDef definition

class ListSourceLocationsResponseTypeDef(TypedDict):
    Items: List[SourceLocationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceLocationTypeDef](./type_defs.md#sourcelocationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPlaybackConfigurationsResponseTypeDef

```python
# ListPlaybackConfigurationsResponseTypeDef definition

class ListPlaybackConfigurationsResponseTypeDef(TypedDict):
    Items: List[PlaybackConfigurationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlaybackConfigurationTypeDef](./type_defs.md#playbackconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    Items: List[ChannelTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPrefetchSchedulesResponseTypeDef

```python
# ListPrefetchSchedulesResponseTypeDef definition

class ListPrefetchSchedulesResponseTypeDef(TypedDict):
    Items: List[PrefetchScheduleTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrefetchScheduleTypeDef](./type_defs.md#prefetchscheduletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProgramRequestRequestTypeDef

```python
# CreateProgramRequestRequestTypeDef definition

class CreateProgramRequestRequestTypeDef(TypedDict):
    ChannelName: str,
    ProgramName: str,
    ScheduleConfiguration: ScheduleConfigurationTypeDef,  # (1)
    SourceLocationName: str,
    AdBreaks: NotRequired[Sequence[AdBreakTypeDef]],  # (2)
    LiveSourceName: NotRequired[str],
    VodSourceName: NotRequired[str],
```

1. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
2. See [:material-code-braces: AdBreakTypeDef](./type_defs.md#adbreaktypedef) 
## CreateProgramResponseTypeDef

```python
# CreateProgramResponseTypeDef definition

class CreateProgramResponseTypeDef(TypedDict):
    AdBreaks: List[AdBreakTypeDef],  # (1)
    Arn: str,
    ChannelName: str,
    ClipRange: ClipRangeTypeDef,  # (2)
    CreationTime: datetime,
    DurationMillis: int,
    LiveSourceName: str,
    ProgramName: str,
    ScheduledStartTime: datetime,
    SourceLocationName: str,
    VodSourceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AdBreakTypeDef](./type_defs.md#adbreaktypedef) 
2. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProgramResponseTypeDef

```python
# DescribeProgramResponseTypeDef definition

class DescribeProgramResponseTypeDef(TypedDict):
    AdBreaks: List[AdBreakTypeDef],  # (1)
    Arn: str,
    ChannelName: str,
    ClipRange: ClipRangeTypeDef,  # (2)
    CreationTime: datetime,
    DurationMillis: int,
    LiveSourceName: str,
    ProgramName: str,
    ScheduledStartTime: datetime,
    SourceLocationName: str,
    VodSourceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AdBreakTypeDef](./type_defs.md#adbreaktypedef) 
2. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProgramRequestRequestTypeDef

```python
# UpdateProgramRequestRequestTypeDef definition

class UpdateProgramRequestRequestTypeDef(TypedDict):
    ChannelName: str,
    ProgramName: str,
    ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,  # (1)
    AdBreaks: NotRequired[Sequence[AdBreakTypeDef]],  # (2)
```

1. See [:material-code-braces: UpdateProgramScheduleConfigurationTypeDef](./type_defs.md#updateprogramscheduleconfigurationtypedef) 
2. See [:material-code-braces: AdBreakTypeDef](./type_defs.md#adbreaktypedef) 
## UpdateProgramResponseTypeDef

```python
# UpdateProgramResponseTypeDef definition

class UpdateProgramResponseTypeDef(TypedDict):
    AdBreaks: List[AdBreakTypeDef],  # (1)
    Arn: str,
    ChannelName: str,
    ClipRange: ClipRangeTypeDef,  # (2)
    CreationTime: datetime,
    DurationMillis: int,
    LiveSourceName: str,
    ProgramName: str,
    ScheduledStartTime: datetime,
    SourceLocationName: str,
    VodSourceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AdBreakTypeDef](./type_defs.md#adbreaktypedef) 
2. See [:material-code-braces: ClipRangeTypeDef](./type_defs.md#cliprangetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
