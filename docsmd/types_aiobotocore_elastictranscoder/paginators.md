# Paginators

> [Index](../README.md) > [ElasticTranscoder](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticTranscoder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
    type annotations stubs module [types-aiobotocore-elastictranscoder](https://pypi.org/project/types-aiobotocore-elastictranscoder/).

## ListJobsByPipelinePaginator

Type annotations and code completion for `#!python session.create_client("elastictranscoder").get_paginator("list_jobs_by_pipeline")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListJobsByPipelinePaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:
    client: ElasticTranscoderClient
    paginator: ListJobsByPipelinePaginator = client.get_paginator("list_jobs_by_pipeline")
```


### paginate

Type annotations and code completion for `#!python ListJobsByPipelinePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PipelineId: str,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsByPipelineResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsByPipelineResponseTypeDef](./type_defs.md#listjobsbypipelineresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = {  # (1)
    "PipelineId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef](./type_defs.md#listjobsbypipelinerequestlistjobsbypipelinepaginatetypedef) 
## ListJobsByStatusPaginator

Type annotations and code completion for `#!python session.create_client("elastictranscoder").get_paginator("list_jobs_by_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListJobsByStatusPaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:
    client: ElasticTranscoderClient
    paginator: ListJobsByStatusPaginator = client.get_paginator("list_jobs_by_status")
```


### paginate

Type annotations and code completion for `#!python ListJobsByStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Status: str,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsByStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsByStatusResponseTypeDef](./type_defs.md#listjobsbystatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsByStatusRequestListJobsByStatusPaginateTypeDef = {  # (1)
    "Status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsByStatusRequestListJobsByStatusPaginateTypeDef](./type_defs.md#listjobsbystatusrequestlistjobsbystatuspaginatetypedef) 
## ListPipelinesPaginator

Type annotations and code completion for `#!python session.create_client("elastictranscoder").get_paginator("list_pipelines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListPipelinesPaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:
    client: ElasticTranscoderClient
    paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
```


### paginate

Type annotations and code completion for `#!python ListPipelinesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPipelinesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPipelinesRequestListPipelinesPaginateTypeDef = {  # (1)
    "Ascending": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipelinesRequestListPipelinesPaginateTypeDef](./type_defs.md#listpipelinesrequestlistpipelinespaginatetypedef) 
## ListPresetsPaginator

Type annotations and code completion for `#!python session.create_client("elastictranscoder").get_paginator("list_presets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListPresetsPaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:
    client: ElasticTranscoderClient
    paginator: ListPresetsPaginator = client.get_paginator("list_presets")
```


### paginate

Type annotations and code completion for `#!python ListPresetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPresetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPresetsResponseTypeDef](./type_defs.md#listpresetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPresetsRequestListPresetsPaginateTypeDef = {  # (1)
    "Ascending": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPresetsRequestListPresetsPaginateTypeDef](./type_defs.md#listpresetsrequestlistpresetspaginatetypedef) 
