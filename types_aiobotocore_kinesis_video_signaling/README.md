<a id="type-annotations-for-aiobotocore-kinesisvideosignalingchannels-module"></a>

# Type annotations for aiobotocore KinesisVideoSignalingChannels module

> [Index](..) > KinesisVideoSignalingChannels

Auto-generated documentation for
[KinesisVideoSignalingChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
type annotations stubs module
[types-aiobotocore-kinesis-video-signaling](https://pypi.org/project/types-aiobotocore-kinesis-video-signaling/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[kinesis-video-signaling]'

# Lite version does not provide session.create_client overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[kinesis-video-signaling]'

# standalone installation
pip install types-aiobotocore-kinesis-video-signaling
```

- [Type annotations for aiobotocore KinesisVideoSignalingChannels module](#type-annotations-for-aiobotocore-kinesisvideosignalingchannels-module)
  - [KinesisVideoSignalingChannelsClient](#kinesisvideosignalingchannelsclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="kinesisvideosignalingchannelsclient"></a>

## KinesisVideoSignalingChannelsClient

Type annotations for `session.create_client("kinesis-video-signaling")` as
[KinesisVideoSignalingChannelsClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_kinesis_video_signaling.client import KinesisVideoSignalingChannelsClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_ice_server_config](./client.md#get_ice_server_config)
- [send_alexa_offer_to_master](./client.md#send_alexa_offer_to_master)

<a id="exceptions"></a>

### Exceptions

KinesisVideoSignalingChannelsClient [exceptions](./client.md#exceptions)

- ClientError
- ClientLimitExceededException
- InvalidArgumentException
- InvalidClientException
- NotAuthorizedException
- ResourceNotFoundException
- SessionExpiredException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_kinesis_video_signaling.literals import ServiceType, ...
```

- [ServiceType](./literals.md#servicetype)
- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_kinesis_video_signaling.type_defs import GetIceServerConfigRequestRequestTypeDef, ...
```

- [GetIceServerConfigRequestRequestTypeDef](./type_defs.md#geticeserverconfigrequestrequesttypedef)
- [GetIceServerConfigResponseTypeDef](./type_defs.md#geticeserverconfigresponsetypedef)
- [IceServerTypeDef](./type_defs.md#iceservertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SendAlexaOfferToMasterRequestRequestTypeDef](./type_defs.md#sendalexaoffertomasterrequestrequesttypedef)
- [SendAlexaOfferToMasterResponseTypeDef](./type_defs.md#sendalexaoffertomasterresponsetypedef)
