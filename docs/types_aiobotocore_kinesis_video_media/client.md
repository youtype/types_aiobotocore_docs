<a id="kinesisvideomediaclient-for-aiobotocore-kinesisvideomedia-module"></a>

# KinesisVideoMediaClient for aiobotocore KinesisVideoMedia module

> [Index](../README.md) > [KinesisVideoMedia](./README.md) >
> KinesisVideoMediaClient

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
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="kinesisvideomediaclient"></a>

## KinesisVideoMediaClient

Type annotations for `session.create_client("kinesis-video-media")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_kinesis_video_media.client import KinesisVideoMediaClient

session = get_session()
async with session.create_client("kinesis-video-media") as client:
    client: KinesisVideoMediaClient
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

Type annotations for `session.create_client("kinesis-video-media").exceptions`
method.

Boto3 documentation:
[KinesisVideoMedia.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("kinesis-video-media").can_paginate` method.

Boto3 documentation:
[KinesisVideoMedia.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("kinesis-video-media").generate_presigned_url` method.

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

<a id="get\_media"></a>

### get_media

Use this API to retrieve media content from a Kinesis video stream.

Type annotations for `session.create_client("kinesis-video-media").get_media`
method.

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

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("kinesis-video-media").__aenter__`
method.

Boto3 documentation:
[KinesisVideoMedia.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [KinesisVideoMediaClient](#kinesisvideomediaclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("kinesis-video-media").__aexit__`
method.

Boto3 documentation:
[KinesisVideoMedia.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.