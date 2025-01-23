# Paginators

> [Index](../README.md) > [ElasticTranscoder](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticTranscoder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#elastictranscoder)
    type annotations stubs module [types-aiobotocore-elastictranscoder](https://pypi.org/project/types-aiobotocore-elastictranscoder/).

## ListJobsByPipelinePaginator

Type annotations and code completion for `#!python session.create_client("elastictranscoder").get_paginator("list_jobs_by_pipeline")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder/paginator/ListJobsByPipeline.html#ElasticTranscoder.Paginator.ListJobsByPipeline)

```python
# ListJobsByPipelinePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListJobsByPipelinePaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:  # (1)
    paginator: ListJobsByPipelinePaginator = client.get_paginator("list_jobs_by_pipeline")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsByPipelineResponseTypeDef
        print(item)  # (3)
```

1. client: [ElasticTranscoderClient](./client.md)
2. paginator: [ListJobsByPipelinePaginator](./paginators.md#listjobsbypipelinepaginator)
3. item: [:material-code-braces: ListJobsByPipelineResponseTypeDef](./type_defs.md#listjobsbypipelineresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsByPipelinePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PipelineId: str,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListJobsByPipelineResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsByPipelineResponseTypeDef](./type_defs.md#listjobsbypipelineresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsByPipelineRequestPaginateTypeDef = {  # (1)
    "PipelineId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsByPipelineRequestPaginateTypeDef](./type_defs.md#listjobsbypipelinerequestpaginatetypedef) 
## ListJobsByStatusPaginator

Type annotations and code completion for `#!python session.create_client("elastictranscoder").get_paginator("list_jobs_by_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder/paginator/ListJobsByStatus.html#ElasticTranscoder.Paginator.ListJobsByStatus)

```python
# ListJobsByStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListJobsByStatusPaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:  # (1)
    paginator: ListJobsByStatusPaginator = client.get_paginator("list_jobs_by_status")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsByStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ElasticTranscoderClient](./client.md)
2. paginator: [ListJobsByStatusPaginator](./paginators.md#listjobsbystatuspaginator)
3. item: [:material-code-braces: ListJobsByStatusResponseTypeDef](./type_defs.md#listjobsbystatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsByStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Status: str,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListJobsByStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsByStatusResponseTypeDef](./type_defs.md#listjobsbystatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsByStatusRequestPaginateTypeDef = {  # (1)
    "Status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsByStatusRequestPaginateTypeDef](./type_defs.md#listjobsbystatusrequestpaginatetypedef) 
## ListPipelinesPaginator

Type annotations and code completion for `#!python session.create_client("elastictranscoder").get_paginator("list_pipelines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder/paginator/ListPipelines.html#ElasticTranscoder.Paginator.ListPipelines)

```python
# ListPipelinesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListPipelinesPaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:  # (1)
    paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")  # (2)
    async for item in paginator.paginate(...):
        item: ListPipelinesResponseTypeDef
        print(item)  # (3)
```

1. client: [ElasticTranscoderClient](./client.md)
2. paginator: [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
3. item: [:material-code-braces: ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPipelinesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPipelinesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPipelinesRequestPaginateTypeDef = {  # (1)
    "Ascending": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipelinesRequestPaginateTypeDef](./type_defs.md#listpipelinesrequestpaginatetypedef) 
## ListPresetsPaginator

Type annotations and code completion for `#!python session.create_client("elastictranscoder").get_paginator("list_presets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder/paginator/ListPresets.html#ElasticTranscoder.Paginator.ListPresets)

```python
# ListPresetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elastictranscoder.paginator import ListPresetsPaginator

session = get_session()
async with session.create_client("elastictranscoder") as client:  # (1)
    paginator: ListPresetsPaginator = client.get_paginator("list_presets")  # (2)
    async for item in paginator.paginate(...):
        item: ListPresetsResponseTypeDef
        print(item)  # (3)
```

1. client: [ElasticTranscoderClient](./client.md)
2. paginator: [ListPresetsPaginator](./paginators.md#listpresetspaginator)
3. item: [:material-code-braces: ListPresetsResponseTypeDef](./type_defs.md#listpresetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPresetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Ascending: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPresetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPresetsResponseTypeDef](./type_defs.md#listpresetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPresetsRequestPaginateTypeDef = {  # (1)
    "Ascending": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPresetsRequestPaginateTypeDef](./type_defs.md#listpresetsrequestpaginatetypedef) 
