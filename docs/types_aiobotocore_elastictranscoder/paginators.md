<a id="paginators-for-aiobotocore-elastictranscoder-module"></a>

# Paginators for aiobotocore ElasticTranscoder module

> [Index](../README.md) > [ElasticTranscoder](./README.md) > Paginators

Auto-generated documentation for
[ElasticTranscoder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
type annotations stubs module
[types-aiobotocore-elastictranscoder](https://pypi.org/project/types-aiobotocore-elastictranscoder/).

- [Paginators for aiobotocore ElasticTranscoder module](#paginators-for-aiobotocore-elastictranscoder-module)
  - [ListJobsByPipelinePaginator](#listjobsbypipelinepaginator)
  - [ListJobsByStatusPaginator](#listjobsbystatuspaginator)
  - [ListPipelinesPaginator](#listpipelinespaginator)
  - [ListPresetsPaginator](#listpresetspaginator)

<a id="listjobsbypipelinepaginator"></a>

## ListJobsByPipelinePaginator

Type annotations for
`session.create_client("elastictranscoder").get_paginator("list_jobs_by_pipeline")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListJobsByPipelinePaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:
    client: ElasticTranscoderClient
    paginator: ListJobsByPipelinePaginator = client.get_paginator("list_jobs_by_pipeline")
```

Boto3 documentation:
[ElasticTranscoder.Paginator.ListJobsByPipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline)

Arguments for `ListJobsByPipelinePaginator.paginate` method:

- `PipelineId`: `str` *(required)*
- `Ascending`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsByPipelinePaginator.paginate` returns
`AsyncIterator`\[[ListJobsByPipelineResponseTypeDef](./type_defs.md#listjobsbypipelineresponsetypedef)\].

<a id="listjobsbystatuspaginator"></a>

## ListJobsByStatusPaginator

Type annotations for
`session.create_client("elastictranscoder").get_paginator("list_jobs_by_status")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListJobsByStatusPaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:
    client: ElasticTranscoderClient
    paginator: ListJobsByStatusPaginator = client.get_paginator("list_jobs_by_status")
```

Boto3 documentation:
[ElasticTranscoder.Paginator.ListJobsByStatus](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus)

Arguments for `ListJobsByStatusPaginator.paginate` method:

- `Status`: `str` *(required)*
- `Ascending`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsByStatusPaginator.paginate` returns
`AsyncIterator`\[[ListJobsByStatusResponseTypeDef](./type_defs.md#listjobsbystatusresponsetypedef)\].

<a id="listpipelinespaginator"></a>

## ListPipelinesPaginator

Type annotations for
`session.create_client("elastictranscoder").get_paginator("list_pipelines")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListPipelinesPaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:
    client: ElasticTranscoderClient
    paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
```

Boto3 documentation:
[ElasticTranscoder.Paginator.ListPipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines)

Arguments for `ListPipelinesPaginator.paginate` method:

- `Ascending`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPipelinesPaginator.paginate` returns
`AsyncIterator`\[[ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef)\].

<a id="listpresetspaginator"></a>

## ListPresetsPaginator

Type annotations for
`session.create_client("elastictranscoder").get_paginator("list_presets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListPresetsPaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:
    client: ElasticTranscoderClient
    paginator: ListPresetsPaginator = client.get_paginator("list_presets")
```

Boto3 documentation:
[ElasticTranscoder.Paginator.ListPresets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets)

Arguments for `ListPresetsPaginator.paginate` method:

- `Ascending`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPresetsPaginator.paginate` returns
`AsyncIterator`\[[ListPresetsResponseTypeDef](./type_defs.md#listpresetsresponsetypedef)\].
