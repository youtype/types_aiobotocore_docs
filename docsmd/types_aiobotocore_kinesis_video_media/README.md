# KinesisVideoMedia module

> [Index](../README.md) > KinesisVideoMedia


!!! note ""

    Auto-generated documentation for [KinesisVideoMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#kinesisvideomedia)
    type annotations stubs module [types-aiobotocore-kinesis-video-media](https://pypi.org/project/types-aiobotocore-kinesis-video-media/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `KinesisVideoMedia` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `KinesisVideoMedia` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[kinesis-video-media]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[kinesis-video-media]'

# standalone installation
python -m pip install types-aiobotocore-kinesis-video-media
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-kinesis-video-media
```

## Usage

Code samples can be found in [Examples](./usage.md).

## KinesisVideoMediaClient

Type annotations and code completion for  `#!python session.create_client("kinesis-video-media")` as [KinesisVideoMediaClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client)

```python
# KinesisVideoMediaClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_media.client import KinesisVideoMediaClient


session = get_session()
async with session.create_client("kinesis-video-media") as client:
    client: KinesisVideoMediaClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# StartSelectorTypeType usage example

from types_aiobotocore_kinesis_video_media.literals import StartSelectorTypeType

def get_value() -> StartSelectorTypeType:
    return "CONTINUATION_TOKEN"
```

- [StartSelectorTypeType](./literals.md#startselectortypetype)
- [KinesisVideoMediaServiceName](./literals.md#kinesisvideomediaservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetMediaOutputTypeDef](./type_defs.md#getmediaoutputtypedef)
- [StartSelectorTypeDef](./type_defs.md#startselectortypedef)
- [GetMediaInputTypeDef](./type_defs.md#getmediainputtypedef)

