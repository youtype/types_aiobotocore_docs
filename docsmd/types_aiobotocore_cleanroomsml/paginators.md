# Paginators

> [Index](../README.md) > [CleanRoomsML](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CleanRoomsML](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
    type annotations stubs module [types-aiobotocore-cleanroomsml](https://pypi.org/project/types-aiobotocore-cleanroomsml/).

## ListAudienceExportJobsPaginator

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_paginator("list_audience_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Paginator.ListAudienceExportJobs)

```python
# ListAudienceExportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanroomsml.paginator import ListAudienceExportJobsPaginator

session = get_session()
async with session.create_client("cleanroomsml") as client:  # (1)
    paginator: ListAudienceExportJobsPaginator = client.get_paginator("list_audience_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListAudienceExportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsMLClient](./client.md)
2. paginator: [ListAudienceExportJobsPaginator](./paginators.md#listaudienceexportjobspaginator)
3. item: [:material-code-braces: ListAudienceExportJobsResponseTypeDef](./type_defs.md#listaudienceexportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAudienceExportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    audienceGenerationJobArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAudienceExportJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAudienceExportJobsResponseTypeDef](./type_defs.md#listaudienceexportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAudienceExportJobsRequestListAudienceExportJobsPaginateTypeDef = {  # (1)
    "audienceGenerationJobArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAudienceExportJobsRequestListAudienceExportJobsPaginateTypeDef](./type_defs.md#listaudienceexportjobsrequestlistaudienceexportjobspaginatetypedef) 
## ListAudienceGenerationJobsPaginator

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_paginator("list_audience_generation_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Paginator.ListAudienceGenerationJobs)

```python
# ListAudienceGenerationJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanroomsml.paginator import ListAudienceGenerationJobsPaginator

session = get_session()
async with session.create_client("cleanroomsml") as client:  # (1)
    paginator: ListAudienceGenerationJobsPaginator = client.get_paginator("list_audience_generation_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListAudienceGenerationJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsMLClient](./client.md)
2. paginator: [ListAudienceGenerationJobsPaginator](./paginators.md#listaudiencegenerationjobspaginator)
3. item: [:material-code-braces: ListAudienceGenerationJobsResponseTypeDef](./type_defs.md#listaudiencegenerationjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAudienceGenerationJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    configuredAudienceModelArn: str = ...,
    collaborationId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAudienceGenerationJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAudienceGenerationJobsResponseTypeDef](./type_defs.md#listaudiencegenerationjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAudienceGenerationJobsRequestListAudienceGenerationJobsPaginateTypeDef = {  # (1)
    "configuredAudienceModelArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAudienceGenerationJobsRequestListAudienceGenerationJobsPaginateTypeDef](./type_defs.md#listaudiencegenerationjobsrequestlistaudiencegenerationjobspaginatetypedef) 
## ListAudienceModelsPaginator

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_paginator("list_audience_models")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Paginator.ListAudienceModels)

```python
# ListAudienceModelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanroomsml.paginator import ListAudienceModelsPaginator

session = get_session()
async with session.create_client("cleanroomsml") as client:  # (1)
    paginator: ListAudienceModelsPaginator = client.get_paginator("list_audience_models")  # (2)
    async for item in paginator.paginate(...):
        item: ListAudienceModelsResponseTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsMLClient](./client.md)
2. paginator: [ListAudienceModelsPaginator](./paginators.md#listaudiencemodelspaginator)
3. item: [:material-code-braces: ListAudienceModelsResponseTypeDef](./type_defs.md#listaudiencemodelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAudienceModelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAudienceModelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAudienceModelsResponseTypeDef](./type_defs.md#listaudiencemodelsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAudienceModelsRequestListAudienceModelsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAudienceModelsRequestListAudienceModelsPaginateTypeDef](./type_defs.md#listaudiencemodelsrequestlistaudiencemodelspaginatetypedef) 
## ListConfiguredAudienceModelsPaginator

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_paginator("list_configured_audience_models")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Paginator.ListConfiguredAudienceModels)

```python
# ListConfiguredAudienceModelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanroomsml.paginator import ListConfiguredAudienceModelsPaginator

session = get_session()
async with session.create_client("cleanroomsml") as client:  # (1)
    paginator: ListConfiguredAudienceModelsPaginator = client.get_paginator("list_configured_audience_models")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfiguredAudienceModelsResponseTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsMLClient](./client.md)
2. paginator: [ListConfiguredAudienceModelsPaginator](./paginators.md#listconfiguredaudiencemodelspaginator)
3. item: [:material-code-braces: ListConfiguredAudienceModelsResponseTypeDef](./type_defs.md#listconfiguredaudiencemodelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConfiguredAudienceModelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListConfiguredAudienceModelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConfiguredAudienceModelsResponseTypeDef](./type_defs.md#listconfiguredaudiencemodelsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConfiguredAudienceModelsRequestListConfiguredAudienceModelsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfiguredAudienceModelsRequestListConfiguredAudienceModelsPaginateTypeDef](./type_defs.md#listconfiguredaudiencemodelsrequestlistconfiguredaudiencemodelspaginatetypedef) 
## ListTrainingDatasetsPaginator

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_paginator("list_training_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Paginator.ListTrainingDatasets)

```python
# ListTrainingDatasetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanroomsml.paginator import ListTrainingDatasetsPaginator

session = get_session()
async with session.create_client("cleanroomsml") as client:  # (1)
    paginator: ListTrainingDatasetsPaginator = client.get_paginator("list_training_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrainingDatasetsResponseTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsMLClient](./client.md)
2. paginator: [ListTrainingDatasetsPaginator](./paginators.md#listtrainingdatasetspaginator)
3. item: [:material-code-braces: ListTrainingDatasetsResponseTypeDef](./type_defs.md#listtrainingdatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTrainingDatasetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTrainingDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrainingDatasetsResponseTypeDef](./type_defs.md#listtrainingdatasetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTrainingDatasetsRequestListTrainingDatasetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrainingDatasetsRequestListTrainingDatasetsPaginateTypeDef](./type_defs.md#listtrainingdatasetsrequestlisttrainingdatasetspaginatetypedef) 
