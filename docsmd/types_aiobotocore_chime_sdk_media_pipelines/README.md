# ChimeSDKMediaPipelines module

> [Index](../README.md) > ChimeSDKMediaPipelines


!!! note ""

    Auto-generated documentation for [ChimeSDKMediaPipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
    type annotations stubs module [types-aiobotocore-chime-sdk-media-pipelines](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `ChimeSDKMediaPipelines`.

### From PyPI with pip

Install `types-aiobotocore` for `ChimeSDKMediaPipelines` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[chime-sdk-media-pipelines]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[chime-sdk-media-pipelines]'


# standalone installation
python -m pip install types-aiobotocore-chime-sdk-media-pipelines
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-chime-sdk-media-pipelines
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ChimeSDKMediaPipelinesClient

Type annotations and code completion for  `#!python session.create_client("chime-sdk-media-pipelines")` as [ChimeSDKMediaPipelinesClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_media_pipelines.client import ChimeSDKMediaPipelinesClient


session = get_session()
async with session.create_client("chime-sdk-media-pipelines") as client:
    client: ChimeSDKMediaPipelinesClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_chime_sdk_media_pipelines.literals import ArtifactsStateType

def get_value() -> ArtifactsStateType:
    return "Disabled"
```

- [ArtifactsStateType](./literals.md#artifactsstatetype)
- [AudioMuxTypeType](./literals.md#audiomuxtypetype)
- [ContentMuxTypeType](./literals.md#contentmuxtypetype)
- [MediaPipelineSinkTypeType](./literals.md#mediapipelinesinktypetype)
- [MediaPipelineSourceTypeType](./literals.md#mediapipelinesourcetypetype)
- [MediaPipelineStatusType](./literals.md#mediapipelinestatustype)
- [VideoMuxTypeType](./literals.md#videomuxtypetype)
- [ChimeSDKMediaPipelinesServiceName](./literals.md#chimesdkmediapipelinesservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_chime_sdk_media_pipelines.type_defs import ArtifactsConfigurationTypeDef

def get_value() -> ArtifactsConfigurationTypeDef:
    return {
        "Audio": ...,
        "Video": ...,
        "Content": ...,
    }
```

- [ArtifactsConfigurationTypeDef](./type_defs.md#artifactsconfigurationtypedef)
- [AudioArtifactsConfigurationTypeDef](./type_defs.md#audioartifactsconfigurationtypedef)
- [ChimeSdkMeetingConfigurationTypeDef](./type_defs.md#chimesdkmeetingconfigurationtypedef)
- [ContentArtifactsConfigurationTypeDef](./type_defs.md#contentartifactsconfigurationtypedef)
- [CreateMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#createmediacapturepipelinerequestrequesttypedef)
- [CreateMediaCapturePipelineResponseTypeDef](./type_defs.md#createmediacapturepipelineresponsetypedef)
- [DeleteMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#deletemediacapturepipelinerequestrequesttypedef)
- [GetMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#getmediacapturepipelinerequestrequesttypedef)
- [GetMediaCapturePipelineResponseTypeDef](./type_defs.md#getmediacapturepipelineresponsetypedef)
- [ListMediaCapturePipelinesRequestRequestTypeDef](./type_defs.md#listmediacapturepipelinesrequestrequesttypedef)
- [ListMediaCapturePipelinesResponseTypeDef](./type_defs.md#listmediacapturepipelinesresponsetypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [MediaCapturePipelineSummaryTypeDef](./type_defs.md#mediacapturepipelinesummarytypedef)
- [MediaCapturePipelineTypeDef](./type_defs.md#mediacapturepipelinetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SelectedVideoStreamsTypeDef](./type_defs.md#selectedvideostreamstypedef)
- [SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [VideoArtifactsConfigurationTypeDef](./type_defs.md#videoartifactsconfigurationtypedef)

