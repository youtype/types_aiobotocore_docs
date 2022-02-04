<a id="type-annotations-for-aiobotocore-kinesisvideomedia-module"></a>

# Type annotations for aiobotocore KinesisVideoMedia module

> [Index](..) > KinesisVideoMedia

Auto-generated documentation for
[KinesisVideoMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
type annotations stubs module
[types-aiobotocore-kinesis-video-media](https://pypi.org/project/types-aiobotocore-kinesis-video-media/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[kinesis-video-media]'

# install as a standalone
pip install types-aiobotocore-kinesis-video-media
```

- [Type annotations for aiobotocore KinesisVideoMedia module](#type-annotations-for-aiobotocore-kinesisvideomedia-module)
  - [KinesisVideoMediaClient](#kinesisvideomediaclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="kinesisvideomediaclient"></a>

## KinesisVideoMediaClient

Type annotations for `aiobotocore.create_client("kinesis-video-media")` as
[KinesisVideoMediaClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_kinesis_video_media.client import KinesisVideoMediaClient
```

<a id="methods"></a>

### Methods

- [can_paginate](./client.md#can_paginate)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_media](./client.md#get_media)

<a id="exceptions"></a>

### Exceptions

KinesisVideoMediaClient [exceptions](./client.md#exceptions)

- ClientError
- ClientLimitExceededException
- ConnectionLimitExceededException
- InvalidArgumentException
- InvalidEndpointException
- NotAuthorizedException
- ResourceNotFoundException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_kinesis_video_media.literals import StartSelectorTypeType, ...
```

- [StartSelectorTypeType](./literals.md#startselectortypetype)
- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_kinesis_video_media.type_defs import GetMediaInputRequestTypeDef, ...
```

- [GetMediaInputRequestTypeDef](./type_defs.md#getmediainputrequesttypedef)
- [GetMediaOutputTypeDef](./type_defs.md#getmediaoutputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [StartSelectorTypeDef](./type_defs.md#startselectortypedef)
