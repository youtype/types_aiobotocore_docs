# Paginators

> [Index](../README.md) > [Personalize](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Personalize](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
    type annotations stubs module [types-aiobotocore-personalize](https://pypi.org/project/types-aiobotocore-personalize/).

## ListBatchInferenceJobsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_batch_inference_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListBatchInferenceJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListBatchInferenceJobsPaginator = client.get_paginator("list_batch_inference_jobs")
```


### paginate

Type annotations and code completion for `#!python ListBatchInferenceJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    solutionVersionArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBatchInferenceJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBatchInferenceJobsResponseTypeDef](./type_defs.md#listbatchinferencejobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef = {  # (1)
    "solutionVersionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBatchInferenceJobsRequestListBatchInferenceJobsPaginateTypeDef](./type_defs.md#listbatchinferencejobsrequestlistbatchinferencejobspaginatetypedef) 
## ListBatchSegmentJobsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_batch_segment_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListBatchSegmentJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListBatchSegmentJobsPaginator = client.get_paginator("list_batch_segment_jobs")
```


### paginate

Type annotations and code completion for `#!python ListBatchSegmentJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    solutionVersionArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBatchSegmentJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBatchSegmentJobsResponseTypeDef](./type_defs.md#listbatchsegmentjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef = {  # (1)
    "solutionVersionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBatchSegmentJobsRequestListBatchSegmentJobsPaginateTypeDef](./type_defs.md#listbatchsegmentjobsrequestlistbatchsegmentjobspaginatetypedef) 
## ListCampaignsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_campaigns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListCampaignsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListCampaignsPaginator = client.get_paginator("list_campaigns")
```


### paginate

Type annotations and code completion for `#!python ListCampaignsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    solutionArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCampaignsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCampaignsRequestListCampaignsPaginateTypeDef = {  # (1)
    "solutionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCampaignsRequestListCampaignsPaginateTypeDef](./type_defs.md#listcampaignsrequestlistcampaignspaginatetypedef) 
## ListDatasetExportJobsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_dataset_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetExportJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListDatasetExportJobsPaginator = client.get_paginator("list_dataset_export_jobs")
```


### paginate

Type annotations and code completion for `#!python ListDatasetExportJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    datasetArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetExportJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetExportJobsResponseTypeDef](./type_defs.md#listdatasetexportjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef = {  # (1)
    "datasetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetExportJobsRequestListDatasetExportJobsPaginateTypeDef](./type_defs.md#listdatasetexportjobsrequestlistdatasetexportjobspaginatetypedef) 
## ListDatasetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_dataset_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetGroupsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListDatasetGroupsPaginator = client.get_paginator("list_dataset_groups")
```


### paginate

Type annotations and code completion for `#!python ListDatasetGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef](./type_defs.md#listdatasetgroupsrequestlistdatasetgroupspaginatetypedef) 
## ListDatasetImportJobsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_dataset_import_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetImportJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListDatasetImportJobsPaginator = client.get_paginator("list_dataset_import_jobs")
```


### paginate

Type annotations and code completion for `#!python ListDatasetImportJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    datasetArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetImportJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = {  # (1)
    "datasetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef](./type_defs.md#listdatasetimportjobsrequestlistdatasetimportjobspaginatetypedef) 
## ListDatasetsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
```


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    datasetGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetsRequestListDatasetsPaginateTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef) 
## ListEventTrackersPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_event_trackers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListEventTrackersPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListEventTrackersPaginator = client.get_paginator("list_event_trackers")
```


### paginate

Type annotations and code completion for `#!python ListEventTrackersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    datasetGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEventTrackersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventTrackersResponseTypeDef](./type_defs.md#listeventtrackersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEventTrackersRequestListEventTrackersPaginateTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventTrackersRequestListEventTrackersPaginateTypeDef](./type_defs.md#listeventtrackersrequestlisteventtrackerspaginatetypedef) 
## ListFiltersPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListFiltersPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListFiltersPaginator = client.get_paginator("list_filters")
```


### paginate

Type annotations and code completion for `#!python ListFiltersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    datasetGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFiltersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFiltersRequestListFiltersPaginateTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFiltersRequestListFiltersPaginateTypeDef](./type_defs.md#listfiltersrequestlistfilterspaginatetypedef) 
## ListRecipesPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_recipes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecipes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListRecipesPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListRecipesPaginator = client.get_paginator("list_recipes")
```


### paginate

Type annotations and code completion for `#!python ListRecipesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    recipeProvider: RecipeProviderType = ...,  # (1)
    domain: DomainType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListRecipesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: RecipeProviderType](./literals.md#recipeprovidertype) 
2. See [:material-code-brackets: DomainType](./literals.md#domaintype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListRecipesResponseTypeDef](./type_defs.md#listrecipesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRecipesRequestListRecipesPaginateTypeDef = {  # (1)
    "recipeProvider": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecipesRequestListRecipesPaginateTypeDef](./type_defs.md#listrecipesrequestlistrecipespaginatetypedef) 
## ListRecommendersPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_recommenders")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListRecommendersPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListRecommendersPaginator = client.get_paginator("list_recommenders")
```


### paginate

Type annotations and code completion for `#!python ListRecommendersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    datasetGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecommendersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecommendersResponseTypeDef](./type_defs.md#listrecommendersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRecommendersRequestListRecommendersPaginateTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendersRequestListRecommendersPaginateTypeDef](./type_defs.md#listrecommendersrequestlistrecommenderspaginatetypedef) 
## ListSchemasPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListSchemasPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListSchemasPaginator = client.get_paginator("list_schemas")
```


### paginate

Type annotations and code completion for `#!python ListSchemasPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSchemasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSchemasRequestListSchemasPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemasRequestListSchemasPaginateTypeDef](./type_defs.md#listschemasrequestlistschemaspaginatetypedef) 
## ListSolutionVersionsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_solution_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListSolutionVersionsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListSolutionVersionsPaginator = client.get_paginator("list_solution_versions")
```


### paginate

Type annotations and code completion for `#!python ListSolutionVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    solutionArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSolutionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSolutionVersionsResponseTypeDef](./type_defs.md#listsolutionversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef = {  # (1)
    "solutionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSolutionVersionsRequestListSolutionVersionsPaginateTypeDef](./type_defs.md#listsolutionversionsrequestlistsolutionversionspaginatetypedef) 
## ListSolutionsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_solutions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListSolutionsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListSolutionsPaginator = client.get_paginator("list_solutions")
```


### paginate

Type annotations and code completion for `#!python ListSolutionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    datasetGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSolutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSolutionsRequestListSolutionsPaginateTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSolutionsRequestListSolutionsPaginateTypeDef](./type_defs.md#listsolutionsrequestlistsolutionspaginatetypedef) 
