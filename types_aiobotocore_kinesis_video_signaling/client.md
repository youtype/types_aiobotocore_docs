<a id="kinesisvideosignalingchannelsclient-for-aiobotocore-kinesisvideosignalingchannels-module"></a>

# KinesisVideoSignalingChannelsClient for aiobotocore KinesisVideoSignalingChannels module

> [Index](..) > [KinesisVideoSignalingChannels](.) >
> KinesisVideoSignalingChannelsClient

Auto-generated documentation for
[KinesisVideoSignalingChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
type annotations stubs module
[types-aiobotocore-kinesis-video-signaling](https://pypi.org/project/types-aiobotocore-kinesis-video-signaling/).

- [KinesisVideoSignalingChannelsClient for aiobotocore KinesisVideoSignalingChannels module](#kinesisvideosignalingchannelsclient-for-aiobotocore-kinesisvideosignalingchannels-module)
  - [KinesisVideoSignalingChannelsClient](#kinesisvideosignalingchannelsclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_ice_server_config](#get_ice_server_config)
    - [send_alexa_offer_to_master](#send_alexa_offer_to_master)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="kinesisvideosignalingchannelsclient"></a>

## KinesisVideoSignalingChannelsClient

Type annotations for `session.create_client("kinesis-video-signaling")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_kinesis_video_signaling.client import KinesisVideoSignalingChannelsClient

session = get_session()
async with session.create_client("kinesis-video-signaling") as client:
    client: KinesisVideoSignalingChannelsClient
```

Boto3 documentation:
[KinesisVideoSignalingChannels.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_kinesis_video_signaling.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ClientLimitExceededException`
- `Exceptions.InvalidArgumentException`
- `Exceptions.InvalidClientException`
- `Exceptions.NotAuthorizedException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.SessionExpiredException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

KinesisVideoSignalingChannelsClient exceptions.

Type annotations for
`session.create_client("kinesis-video-signaling").exceptions` method.

Boto3 documentation:
[KinesisVideoSignalingChannels.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("kinesis-video-signaling").can_paginate` method.

Boto3 documentation:
[KinesisVideoSignalingChannels.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("kinesis-video-signaling").generate_presigned_url`
method.

Boto3 documentation:
[KinesisVideoSignalingChannels.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_ice_server_config"></a>

### get_ice_server_config

Gets the Interactive Connectivity Establishment (ICE) server configuration
information, including URIs, username, and password which can be used to
configure the WebRTC connection.

Type annotations for
`session.create_client("kinesis-video-signaling").get_ice_server_config`
method.

Boto3 documentation:
[KinesisVideoSignalingChannels.Client.get_ice_server_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels.Client.get_ice_server_config)

Asynchronous method. Use `await get_ice_server_config(...)` for a synchronous
call.

Arguments mapping described in
[GetIceServerConfigRequestRequestTypeDef](./type_defs.md#geticeserverconfigrequestrequesttypedef).

Keyword-only arguments:

- `ChannelARN`: `str` *(required)*
- `ClientId`: `str`
- `Service`: `Literal['TURN']` (see [ServiceType](./literals.md#servicetype))
- `Username`: `str`

Returns a `Coroutine` for
[GetIceServerConfigResponseTypeDef](./type_defs.md#geticeserverconfigresponsetypedef).

<a id="send_alexa_offer_to_master"></a>

### send_alexa_offer_to_master

This API allows you to connect WebRTC-enabled devices with Alexa display
devices.

Type annotations for
`session.create_client("kinesis-video-signaling").send_alexa_offer_to_master`
method.

Boto3 documentation:
[KinesisVideoSignalingChannels.Client.send_alexa_offer_to_master](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels.Client.send_alexa_offer_to_master)

Asynchronous method. Use `await send_alexa_offer_to_master(...)` for a
synchronous call.

Arguments mapping described in
[SendAlexaOfferToMasterRequestRequestTypeDef](./type_defs.md#sendalexaoffertomasterrequestrequesttypedef).

Keyword-only arguments:

- `ChannelARN`: `str` *(required)*
- `SenderClientId`: `str` *(required)*
- `MessagePayload`: `str` *(required)*

Returns a `Coroutine` for
[SendAlexaOfferToMasterResponseTypeDef](./type_defs.md#sendalexaoffertomasterresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for
`session.create_client("kinesis-video-signaling").__aenter__` method.

Boto3 documentation:
[KinesisVideoSignalingChannels.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[KinesisVideoSignalingChannelsClient](#kinesisvideosignalingchannelsclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for
`session.create_client("kinesis-video-signaling").__aexit__` method.

Boto3 documentation:
[KinesisVideoSignalingChannels.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
