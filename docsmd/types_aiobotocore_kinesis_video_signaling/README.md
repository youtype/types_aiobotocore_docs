# KinesisVideoSignalingChannels module

> [Index](../README.md) > KinesisVideoSignalingChannels


!!! note ""

    Auto-generated documentation for [KinesisVideoSignalingChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#kinesisvideosignalingchannels)
    type annotations stubs module [types-aiobotocore-kinesis-video-signaling](https://pypi.org/project/types-aiobotocore-kinesis-video-signaling/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `KinesisVideoSignalingChannels` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `KinesisVideoSignalingChannels` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[kinesis-video-signaling]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[kinesis-video-signaling]'

# standalone installation
python -m pip install types-aiobotocore-kinesis-video-signaling
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-kinesis-video-signaling
```

## Usage

Code samples can be found in [Examples](./usage.md).

## KinesisVideoSignalingChannelsClient

Type annotations and code completion for  `#!python session.create_client("kinesis-video-signaling")` as [KinesisVideoSignalingChannelsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels.Client)

```python
# KinesisVideoSignalingChannelsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_signaling.client import KinesisVideoSignalingChannelsClient


session = get_session()
async with session.create_client("kinesis-video-signaling") as client:
    client: KinesisVideoSignalingChannelsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ServiceType usage example

from types_aiobotocore_kinesis_video_signaling.literals import ServiceType

def get_value() -> ServiceType:
    return "TURN"
```

- [ServiceType](./literals.md#servicetype)
- [KinesisVideoSignalingChannelsServiceName](./literals.md#kinesisvideosignalingchannelsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [GetIceServerConfigRequestTypeDef](./type_defs.md#geticeserverconfigrequesttypedef)
- [IceServerTypeDef](./type_defs.md#iceservertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SendAlexaOfferToMasterRequestTypeDef](./type_defs.md#sendalexaoffertomasterrequesttypedef)
- [GetIceServerConfigResponseTypeDef](./type_defs.md#geticeserverconfigresponsetypedef)
- [SendAlexaOfferToMasterResponseTypeDef](./type_defs.md#sendalexaoffertomasterresponsetypedef)

