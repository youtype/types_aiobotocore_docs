# ElasticTranscoder module

> [Index](../README.md) > ElasticTranscoder


!!! note ""

    Auto-generated documentation for [ElasticTranscoder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#elastictranscoder)
    type annotations stubs module [types-aiobotocore-elastictranscoder](https://pypi.org/project/types-aiobotocore-elastictranscoder/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ElasticTranscoder` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ElasticTranscoder` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[elastictranscoder]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[elastictranscoder]'

# standalone installation
python -m pip install types-aiobotocore-elastictranscoder
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-elastictranscoder
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ElasticTranscoderClient

Type annotations and code completion for  `#!python session.create_client("elastictranscoder")` as [ElasticTranscoderClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client)

```python
# ElasticTranscoderClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.client import ElasticTranscoderClient


session = get_session()
async with session.create_client("elastictranscoder") as client:
    client: ElasticTranscoderClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("elastictranscoder").get_paginator("...")`.

```python
# ListJobsByPipelinePaginator usage example

from types_aiobotocore_elastictranscoder.paginator import ListJobsByPipelinePaginator

def get_list_jobs_by_pipeline_paginator() -> ListJobsByPipelinePaginator:
    return client.get_paginator("list_jobs_by_pipeline"))
```

- [ListJobsByPipelinePaginator](./paginators.md#listjobsbypipelinepaginator)
- [ListJobsByStatusPaginator](./paginators.md#listjobsbystatuspaginator)
- [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
- [ListPresetsPaginator](./paginators.md#listpresetspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("elastictranscoder").get_waiter("...")`.

```python
# JobCompleteWaiter usage example

from types_aiobotocore_elastictranscoder.waiter import JobCompleteWaiter

def get_job_complete_waiter() -> JobCompleteWaiter:
    return Session().client("elastictranscoder").get_waiter("job_complete")
```

- [JobCompleteWaiter](./waiters.md#jobcompletewaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# JobCompleteWaiterName usage example

from types_aiobotocore_elastictranscoder.literals import JobCompleteWaiterName

def get_value() -> JobCompleteWaiterName:
    return "job_complete"
```

- [JobCompleteWaiterName](./literals.md#jobcompletewaitername)
- [ListJobsByPipelinePaginatorName](./literals.md#listjobsbypipelinepaginatorname)
- [ListJobsByStatusPaginatorName](./literals.md#listjobsbystatuspaginatorname)
- [ListPipelinesPaginatorName](./literals.md#listpipelinespaginatorname)
- [ListPresetsPaginatorName](./literals.md#listpresetspaginatorname)
- [ElasticTranscoderServiceName](./literals.md#elastictranscoderservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [EncryptionTypeDef](./type_defs.md#encryptiontypedef)
- [AudioCodecOptionsTypeDef](./type_defs.md#audiocodecoptionstypedef)
- [CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef)
- [TimeSpanTypeDef](./type_defs.md#timespantypedef)
- [HlsContentProtectionTypeDef](./type_defs.md#hlscontentprotectiontypedef)
- [PlayReadyDrmTypeDef](./type_defs.md#playreadydrmtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [NotificationsTypeDef](./type_defs.md#notificationstypedef)
- [WarningTypeDef](./type_defs.md#warningtypedef)
- [ThumbnailsTypeDef](./type_defs.md#thumbnailstypedef)
- [DeletePipelineRequestRequestTypeDef](./type_defs.md#deletepipelinerequestrequesttypedef)
- [DeletePresetRequestRequestTypeDef](./type_defs.md#deletepresetrequestrequesttypedef)
- [DetectedPropertiesTypeDef](./type_defs.md#detectedpropertiestypedef)
- [TimingTypeDef](./type_defs.md#timingtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListJobsByPipelineRequestRequestTypeDef](./type_defs.md#listjobsbypipelinerequestrequesttypedef)
- [ListJobsByStatusRequestRequestTypeDef](./type_defs.md#listjobsbystatusrequestrequesttypedef)
- [ListPipelinesRequestRequestTypeDef](./type_defs.md#listpipelinesrequestrequesttypedef)
- [ListPresetsRequestRequestTypeDef](./type_defs.md#listpresetsrequestrequesttypedef)
- [PermissionOutputTypeDef](./type_defs.md#permissionoutputtypedef)
- [PermissionTypeDef](./type_defs.md#permissiontypedef)
- [PresetWatermarkTypeDef](./type_defs.md#presetwatermarktypedef)
- [ReadJobRequestRequestTypeDef](./type_defs.md#readjobrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [ReadPipelineRequestRequestTypeDef](./type_defs.md#readpipelinerequestrequesttypedef)
- [ReadPresetRequestRequestTypeDef](./type_defs.md#readpresetrequestrequesttypedef)
- [TestRoleRequestRequestTypeDef](./type_defs.md#testrolerequestrequesttypedef)
- [UpdatePipelineStatusRequestRequestTypeDef](./type_defs.md#updatepipelinestatusrequestrequesttypedef)
- [ArtworkTypeDef](./type_defs.md#artworktypedef)
- [CaptionFormatTypeDef](./type_defs.md#captionformattypedef)
- [CaptionSourceTypeDef](./type_defs.md#captionsourcetypedef)
- [JobWatermarkTypeDef](./type_defs.md#jobwatermarktypedef)
- [AudioParametersTypeDef](./type_defs.md#audioparameterstypedef)
- [ClipTypeDef](./type_defs.md#cliptypedef)
- [CreateJobPlaylistTypeDef](./type_defs.md#createjobplaylisttypedef)
- [PlaylistTypeDef](./type_defs.md#playlisttypedef)
- [TestRoleResponseTypeDef](./type_defs.md#testroleresponsetypedef)
- [UpdatePipelineNotificationsRequestRequestTypeDef](./type_defs.md#updatepipelinenotificationsrequestrequesttypedef)
- [ListJobsByPipelineRequestPaginateTypeDef](./type_defs.md#listjobsbypipelinerequestpaginatetypedef)
- [ListJobsByStatusRequestPaginateTypeDef](./type_defs.md#listjobsbystatusrequestpaginatetypedef)
- [ListPipelinesRequestPaginateTypeDef](./type_defs.md#listpipelinesrequestpaginatetypedef)
- [ListPresetsRequestPaginateTypeDef](./type_defs.md#listpresetsrequestpaginatetypedef)
- [PipelineOutputConfigOutputTypeDef](./type_defs.md#pipelineoutputconfigoutputtypedef)
- [PermissionUnionTypeDef](./type_defs.md#permissionuniontypedef)
- [VideoParametersOutputTypeDef](./type_defs.md#videoparametersoutputtypedef)
- [VideoParametersTypeDef](./type_defs.md#videoparameterstypedef)
- [ReadJobRequestWaitTypeDef](./type_defs.md#readjobrequestwaittypedef)
- [JobAlbumArtOutputTypeDef](./type_defs.md#jobalbumartoutputtypedef)
- [JobAlbumArtTypeDef](./type_defs.md#jobalbumarttypedef)
- [CaptionsOutputTypeDef](./type_defs.md#captionsoutputtypedef)
- [CaptionsTypeDef](./type_defs.md#captionstypedef)
- [InputCaptionsOutputTypeDef](./type_defs.md#inputcaptionsoutputtypedef)
- [InputCaptionsTypeDef](./type_defs.md#inputcaptionstypedef)
- [PipelineTypeDef](./type_defs.md#pipelinetypedef)
- [PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef)
- [PresetTypeDef](./type_defs.md#presettypedef)
- [CreatePresetRequestRequestTypeDef](./type_defs.md#createpresetrequestrequesttypedef)
- [JobAlbumArtUnionTypeDef](./type_defs.md#jobalbumartuniontypedef)
- [JobOutputTypeDef](./type_defs.md#joboutputtypedef)
- [CaptionsUnionTypeDef](./type_defs.md#captionsuniontypedef)
- [JobInputOutputTypeDef](./type_defs.md#jobinputoutputtypedef)
- [InputCaptionsUnionTypeDef](./type_defs.md#inputcaptionsuniontypedef)
- [CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef)
- [ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef)
- [ReadPipelineResponseTypeDef](./type_defs.md#readpipelineresponsetypedef)
- [UpdatePipelineNotificationsResponseTypeDef](./type_defs.md#updatepipelinenotificationsresponsetypedef)
- [UpdatePipelineResponseTypeDef](./type_defs.md#updatepipelineresponsetypedef)
- [UpdatePipelineStatusResponseTypeDef](./type_defs.md#updatepipelinestatusresponsetypedef)
- [CreatePipelineRequestRequestTypeDef](./type_defs.md#createpipelinerequestrequesttypedef)
- [UpdatePipelineRequestRequestTypeDef](./type_defs.md#updatepipelinerequestrequesttypedef)
- [CreatePresetResponseTypeDef](./type_defs.md#createpresetresponsetypedef)
- [ListPresetsResponseTypeDef](./type_defs.md#listpresetsresponsetypedef)
- [ReadPresetResponseTypeDef](./type_defs.md#readpresetresponsetypedef)
- [CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef)
- [JobTypeDef](./type_defs.md#jobtypedef)
- [JobInputTypeDef](./type_defs.md#jobinputtypedef)
- [CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef)
- [ListJobsByPipelineResponseTypeDef](./type_defs.md#listjobsbypipelineresponsetypedef)
- [ListJobsByStatusResponseTypeDef](./type_defs.md#listjobsbystatusresponsetypedef)
- [ReadJobResponseTypeDef](./type_defs.md#readjobresponsetypedef)
- [JobInputUnionTypeDef](./type_defs.md#jobinputuniontypedef)
- [CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef)

