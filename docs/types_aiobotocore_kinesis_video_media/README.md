<a id="type-annotations-for-aiobotocore-kinesisvideomedia-module"></a>

# Type annotations for aiobotocore KinesisVideoMedia module

> [Index](../README.md) > KinesisVideoMedia

Auto-generated documentation for
[KinesisVideoMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
type annotations stubs module
[types-aiobotocore-kinesis-video-media](https://pypi.org/project/types-aiobotocore-kinesis-video-media/).

- [Type annotations for aiobotocore KinesisVideoMedia module](#type-annotations-for-aiobotocore-kinesisvideomedia-module)
  - [How to install](#how-to-install)
    - [VSCode extension](#vscode-extension)
    - [From PyPI with pip](#from-pypi-with-pip)
  - [How to uninstall](#how-to-uninstall)
  - [Usage](#usage)
  - [KinesisVideoMediaClient](#kinesisvideomediaclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="how-to-install"></a>

## How to install

<a id="vscode-extension"></a>

### VSCode extension

Add
[AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `KinesisVideoMedia`.

<a id="from-pypi-with-pip"></a>

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

<a id="how-to-uninstall"></a>

## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-kinesis-video-media
```

<a id="usage"></a>

## Usage

Code samples can be found [here](./usage.md).

<a id="kinesisvideomediaclient"></a>

## KinesisVideoMediaClient

Type annotations for `session.create_client("kinesis-video-media")` as
[KinesisVideoMediaClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_kinesis_video_media.client import KinesisVideoMediaClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
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
- [KinesisVideoMediaServiceName](./literals.md#kinesisvideomediaservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from types_aiobotocore_kinesis_video_media.type_defs import GetMediaInputRequestTypeDef, ...
```

- [GetMediaInputRequestTypeDef](./type_defs.md#getmediainputrequesttypedef)
- [GetMediaOutputTypeDef](./type_defs.md#getmediaoutputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [StartSelectorTypeDef](./type_defs.md#startselectortypedef)
