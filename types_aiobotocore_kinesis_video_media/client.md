<a id="kinesisvideomediaclient-for-aiobotocore-kinesisvideomedia-module"></a>

# KinesisVideoMediaClient for aiobotocore KinesisVideoMedia module

> [Index](..) > [KinesisVideoMedia](.) > KinesisVideoMediaClient

Auto-generated documentation for
[KinesisVideoMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
type annotations stubs module
[types-aiobotocore-kinesis-video-media](https://pypi.org/project/types-aiobotocore-kinesis-video-media/).

- [KinesisVideoMediaClient for aiobotocore KinesisVideoMedia module](#kinesisvideomediaclient-for-aiobotocore-kinesisvideomedia-module)
  - [KinesisVideoMediaClient](#kinesisvideomediaclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_media](#get_media)

<a id="kinesisvideomediaclient"></a>

## KinesisVideoMediaClient

Type annotations for `aiobotocore.create_client("kinesis-video-media")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_kinesis_video_media.client import KinesisVideoMediaClient

def get_kinesis-video-media_client() -> KinesisVideoMediaClient:
    return Session().client("kinesis-video-media")
```

Boto3 documentation:
[KinesisVideoMedia.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_kinesis_video_media.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ClientLimitExceededException`
- `Exceptions.ConnectionLimitExceededException`
- `Exceptions.InvalidArgumentException`
- `Exceptions.InvalidEndpointException`
- `Exceptions.NotAuthorizedException`
- `Exceptions.ResourceNotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

KinesisVideoMediaClient exceptions.

Type annotations for
`aiobotocore.create_client("kinesis-video-media").exceptions` method.

Boto3 documentation:
[KinesisVideoMedia.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`aiobotocore.create_client("kinesis-video-media").can_paginate` method.

Boto3 documentation:
[KinesisVideoMedia.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("kinesis-video-media").generate_presigned_url`
method.

Boto3 documentation:
[KinesisVideoMedia.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_media"></a>

### get_media

Use this API to retrieve media content from a Kinesis video stream.

Type annotations for
`aiobotocore.create_client("kinesis-video-media").get_media` method.

Boto3 documentation:
[KinesisVideoMedia.Client.get_media](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client.get_media)

Asynchronous method. Use `await get_media(...)` for a synchronous call.

Arguments mapping described in
[GetMediaInputRequestTypeDef](./type_defs.md#getmediainputrequesttypedef).

Keyword-only arguments:

- `StartSelector`: [StartSelectorTypeDef](./type_defs.md#startselectortypedef)
  *(required)*
- `StreamName`: `str`
- `StreamARN`: `str`

Returns a `Coroutine` for
[GetMediaOutputTypeDef](./type_defs.md#getmediaoutputtypedef).
