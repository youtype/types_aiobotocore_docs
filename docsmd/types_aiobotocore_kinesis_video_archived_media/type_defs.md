# Type definitions

> [Index](../README.md) > [KinesisVideoArchivedMedia](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [KinesisVideoArchivedMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#kinesisvideoarchivedmedia)
    type annotations stubs module [types-aiobotocore-kinesis-video-archived-media](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## FragmentTypeDef

```python
# FragmentTypeDef definition

class FragmentTypeDef(TypedDict):
    FragmentNumber: NotRequired[str],
    FragmentSizeInBytes: NotRequired[int],
    ProducerTimestamp: NotRequired[datetime],
    ServerTimestamp: NotRequired[datetime],
    FragmentLengthInMilliseconds: NotRequired[int],
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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ImageTypeDef

```python
# ImageTypeDef definition

class ImageTypeDef(TypedDict):
    TimeStamp: NotRequired[datetime],
    Error: NotRequired[ImageErrorType],  # (1)
    ImageContent: NotRequired[str],
```

1. See [:material-code-brackets: ImageErrorType](./literals.md#imageerrortype) 
## GetMediaForFragmentListInputRequestTypeDef

```python
# GetMediaForFragmentListInputRequestTypeDef definition

class GetMediaForFragmentListInputRequestTypeDef(TypedDict):
    Fragments: Sequence[str],
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

## ClipTimestampRangeTypeDef

```python
# ClipTimestampRangeTypeDef definition

class ClipTimestampRangeTypeDef(TypedDict):
    StartTimestamp: TimestampTypeDef,
    EndTimestamp: TimestampTypeDef,
```

## DASHTimestampRangeTypeDef

```python
# DASHTimestampRangeTypeDef definition

class DASHTimestampRangeTypeDef(TypedDict):
    StartTimestamp: NotRequired[TimestampTypeDef],
    EndTimestamp: NotRequired[TimestampTypeDef],
```

## GetImagesInputRequestTypeDef

```python
# GetImagesInputRequestTypeDef definition

class GetImagesInputRequestTypeDef(TypedDict):
    ImageSelectorType: ImageSelectorTypeType,  # (1)
    StartTimestamp: TimestampTypeDef,
    EndTimestamp: TimestampTypeDef,
    Format: FormatType,  # (2)
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
    SamplingInterval: NotRequired[int],
    FormatConfig: NotRequired[Mapping[FormatConfigKeyType, str]],  # (3)
    WidthPixels: NotRequired[int],
    HeightPixels: NotRequired[int],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ImageSelectorTypeType](./literals.md#imageselectortypetype) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
3. See [:material-code-brackets: FormatConfigKeyType](./literals.md#formatconfigkeytype) 
## HLSTimestampRangeTypeDef

```python
# HLSTimestampRangeTypeDef definition

class HLSTimestampRangeTypeDef(TypedDict):
    StartTimestamp: NotRequired[TimestampTypeDef],
    EndTimestamp: NotRequired[TimestampTypeDef],
```

## TimestampRangeTypeDef

```python
# TimestampRangeTypeDef definition

class TimestampRangeTypeDef(TypedDict):
    StartTimestamp: TimestampTypeDef,
    EndTimestamp: TimestampTypeDef,
```

## GetClipOutputTypeDef

```python
# GetClipOutputTypeDef definition

class GetClipOutputTypeDef(TypedDict):
    ContentType: str,
    Payload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDASHStreamingSessionURLOutputTypeDef

```python
# GetDASHStreamingSessionURLOutputTypeDef definition

class GetDASHStreamingSessionURLOutputTypeDef(TypedDict):
    DASHStreamingSessionURL: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetHLSStreamingSessionURLOutputTypeDef

```python
# GetHLSStreamingSessionURLOutputTypeDef definition

class GetHLSStreamingSessionURLOutputTypeDef(TypedDict):
    HLSStreamingSessionURL: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMediaForFragmentListOutputTypeDef

```python
# GetMediaForFragmentListOutputTypeDef definition

class GetMediaForFragmentListOutputTypeDef(TypedDict):
    ContentType: str,
    Payload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFragmentsOutputTypeDef

```python
# ListFragmentsOutputTypeDef definition

class ListFragmentsOutputTypeDef(TypedDict):
    Fragments: List[FragmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FragmentTypeDef](./type_defs.md#fragmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetImagesInputPaginateTypeDef

```python
# GetImagesInputPaginateTypeDef definition

class GetImagesInputPaginateTypeDef(TypedDict):
    ImageSelectorType: ImageSelectorTypeType,  # (1)
    StartTimestamp: TimestampTypeDef,
    EndTimestamp: TimestampTypeDef,
    Format: FormatType,  # (2)
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
    SamplingInterval: NotRequired[int],
    FormatConfig: NotRequired[Mapping[FormatConfigKeyType, str]],  # (3)
    WidthPixels: NotRequired[int],
    HeightPixels: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ImageSelectorTypeType](./literals.md#imageselectortypetype) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
3. See [:material-code-brackets: FormatConfigKeyType](./literals.md#formatconfigkeytype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetImagesOutputTypeDef

```python
# GetImagesOutputTypeDef definition

class GetImagesOutputTypeDef(TypedDict):
    Images: List[ImageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClipFragmentSelectorTypeDef

```python
# ClipFragmentSelectorTypeDef definition

class ClipFragmentSelectorTypeDef(TypedDict):
    FragmentSelectorType: ClipFragmentSelectorTypeType,  # (1)
    TimestampRange: ClipTimestampRangeTypeDef,  # (2)
```

1. See [:material-code-brackets: ClipFragmentSelectorTypeType](./literals.md#clipfragmentselectortypetype) 
2. See [:material-code-braces: ClipTimestampRangeTypeDef](./type_defs.md#cliptimestamprangetypedef) 
## DASHFragmentSelectorTypeDef

```python
# DASHFragmentSelectorTypeDef definition

class DASHFragmentSelectorTypeDef(TypedDict):
    FragmentSelectorType: NotRequired[DASHFragmentSelectorTypeType],  # (1)
    TimestampRange: NotRequired[DASHTimestampRangeTypeDef],  # (2)
```

1. See [:material-code-brackets: DASHFragmentSelectorTypeType](./literals.md#dashfragmentselectortypetype) 
2. See [:material-code-braces: DASHTimestampRangeTypeDef](./type_defs.md#dashtimestamprangetypedef) 
## HLSFragmentSelectorTypeDef

```python
# HLSFragmentSelectorTypeDef definition

class HLSFragmentSelectorTypeDef(TypedDict):
    FragmentSelectorType: NotRequired[HLSFragmentSelectorTypeType],  # (1)
    TimestampRange: NotRequired[HLSTimestampRangeTypeDef],  # (2)
```

1. See [:material-code-brackets: HLSFragmentSelectorTypeType](./literals.md#hlsfragmentselectortypetype) 
2. See [:material-code-braces: HLSTimestampRangeTypeDef](./type_defs.md#hlstimestamprangetypedef) 
## FragmentSelectorTypeDef

```python
# FragmentSelectorTypeDef definition

class FragmentSelectorTypeDef(TypedDict):
    FragmentSelectorType: FragmentSelectorTypeType,  # (1)
    TimestampRange: TimestampRangeTypeDef,  # (2)
```

1. See [:material-code-brackets: FragmentSelectorTypeType](./literals.md#fragmentselectortypetype) 
2. See [:material-code-braces: TimestampRangeTypeDef](./type_defs.md#timestamprangetypedef) 
## GetClipInputRequestTypeDef

```python
# GetClipInputRequestTypeDef definition

class GetClipInputRequestTypeDef(TypedDict):
    ClipFragmentSelector: ClipFragmentSelectorTypeDef,  # (1)
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
```

1. See [:material-code-braces: ClipFragmentSelectorTypeDef](./type_defs.md#clipfragmentselectortypedef) 
## GetDASHStreamingSessionURLInputRequestTypeDef

```python
# GetDASHStreamingSessionURLInputRequestTypeDef definition

class GetDASHStreamingSessionURLInputRequestTypeDef(TypedDict):
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
    PlaybackMode: NotRequired[DASHPlaybackModeType],  # (1)
    DisplayFragmentTimestamp: NotRequired[DASHDisplayFragmentTimestampType],  # (2)
    DisplayFragmentNumber: NotRequired[DASHDisplayFragmentNumberType],  # (3)
    DASHFragmentSelector: NotRequired[DASHFragmentSelectorTypeDef],  # (4)
    Expires: NotRequired[int],
    MaxManifestFragmentResults: NotRequired[int],
```

1. See [:material-code-brackets: DASHPlaybackModeType](./literals.md#dashplaybackmodetype) 
2. See [:material-code-brackets: DASHDisplayFragmentTimestampType](./literals.md#dashdisplayfragmenttimestamptype) 
3. See [:material-code-brackets: DASHDisplayFragmentNumberType](./literals.md#dashdisplayfragmentnumbertype) 
4. See [:material-code-braces: DASHFragmentSelectorTypeDef](./type_defs.md#dashfragmentselectortypedef) 
## GetHLSStreamingSessionURLInputRequestTypeDef

```python
# GetHLSStreamingSessionURLInputRequestTypeDef definition

class GetHLSStreamingSessionURLInputRequestTypeDef(TypedDict):
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
    PlaybackMode: NotRequired[HLSPlaybackModeType],  # (1)
    HLSFragmentSelector: NotRequired[HLSFragmentSelectorTypeDef],  # (2)
    ContainerFormat: NotRequired[ContainerFormatType],  # (3)
    DiscontinuityMode: NotRequired[HLSDiscontinuityModeType],  # (4)
    DisplayFragmentTimestamp: NotRequired[HLSDisplayFragmentTimestampType],  # (5)
    Expires: NotRequired[int],
    MaxMediaPlaylistFragmentResults: NotRequired[int],
```

1. See [:material-code-brackets: HLSPlaybackModeType](./literals.md#hlsplaybackmodetype) 
2. See [:material-code-braces: HLSFragmentSelectorTypeDef](./type_defs.md#hlsfragmentselectortypedef) 
3. See [:material-code-brackets: ContainerFormatType](./literals.md#containerformattype) 
4. See [:material-code-brackets: HLSDiscontinuityModeType](./literals.md#hlsdiscontinuitymodetype) 
5. See [:material-code-brackets: HLSDisplayFragmentTimestampType](./literals.md#hlsdisplayfragmenttimestamptype) 
## ListFragmentsInputPaginateTypeDef

```python
# ListFragmentsInputPaginateTypeDef definition

class ListFragmentsInputPaginateTypeDef(TypedDict):
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
    FragmentSelector: NotRequired[FragmentSelectorTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FragmentSelectorTypeDef](./type_defs.md#fragmentselectortypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFragmentsInputRequestTypeDef

```python
# ListFragmentsInputRequestTypeDef definition

class ListFragmentsInputRequestTypeDef(TypedDict):
    StreamName: NotRequired[str],
    StreamARN: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    FragmentSelector: NotRequired[FragmentSelectorTypeDef],  # (1)
```

1. See [:material-code-braces: FragmentSelectorTypeDef](./type_defs.md#fragmentselectortypedef) 
