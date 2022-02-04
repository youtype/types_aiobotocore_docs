<a id="typed-dictionaries-for-aiobotocore-kinesisvideomedia-module"></a>

# Typed dictionaries for aiobotocore KinesisVideoMedia module

> [Index](..) > [KinesisVideoMedia](.) > Typed dictionaries

Auto-generated documentation for
[KinesisVideoMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
type annotations stubs module
[types-aiobotocore-kinesis-video-media](https://pypi.org/project/types-aiobotocore-kinesis-video-media/).

- [Typed dictionaries for aiobotocore KinesisVideoMedia module](#typed-dictionaries-for-aiobotocore-kinesisvideomedia-module)
  - [GetMediaInputRequestTypeDef](#getmediainputrequesttypedef)
  - [GetMediaOutputTypeDef](#getmediaoutputtypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [StartSelectorTypeDef](#startselectortypedef)

<a id="getmediainputrequesttypedef"></a>

## GetMediaInputRequestTypeDef

```python
from types_aiobotocore_kinesis_video_media.type_defs import GetMediaInputRequestTypeDef
```

Required fields:

- `StartSelector`: [StartSelectorTypeDef](./type_defs.md#startselectortypedef)

Optional fields:

- `StreamName`: `str`
- `StreamARN`: `str`

<a id="getmediaoutputtypedef"></a>

## GetMediaOutputTypeDef

```python
from types_aiobotocore_kinesis_video_media.type_defs import GetMediaOutputTypeDef
```

Required fields:

- `ContentType`: `str`
- `Payload`: `StreamingBody`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_kinesis_video_media.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="startselectortypedef"></a>

## StartSelectorTypeDef

```python
from types_aiobotocore_kinesis_video_media.type_defs import StartSelectorTypeDef
```

Required fields:

- `StartSelectorType`:
  [StartSelectorTypeType](./literals.md#startselectortypetype)

Optional fields:

- `AfterFragmentNumber`: `str`
- `StartTimestamp`: `Union`\[`datetime`, `str`\]
- `ContinuationToken`: `str`
