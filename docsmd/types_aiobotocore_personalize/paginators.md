# Paginators

> [Index](../README.md) > [Personalize](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Personalize](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#personalize)
    type annotations stubs module [types-aiobotocore-personalize](https://pypi.org/project/types-aiobotocore-personalize/).

## ListBatchInferenceJobsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_batch_inference_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListBatchInferenceJobs.html#Personalize.Paginator.ListBatchInferenceJobs)

```python
# ListBatchInferenceJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListBatchInferenceJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListBatchInferenceJobsPaginator = client.get_paginator("list_batch_inference_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListBatchInferenceJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListBatchInferenceJobsPaginator](./paginators.md#listbatchinferencejobspaginator)
3. item: [:material-code-braces: ListBatchInferenceJobsResponseTypeDef](./type_defs.md#listbatchinferencejobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBatchInferenceJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    solutionVersionArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBatchInferenceJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBatchInferenceJobsResponseTypeDef](./type_defs.md#listbatchinferencejobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBatchInferenceJobsRequestPaginateTypeDef = {  # (1)
    "solutionVersionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBatchInferenceJobsRequestPaginateTypeDef](./type_defs.md#listbatchinferencejobsrequestpaginatetypedef) 
## ListBatchSegmentJobsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_batch_segment_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListBatchSegmentJobs.html#Personalize.Paginator.ListBatchSegmentJobs)

```python
# ListBatchSegmentJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListBatchSegmentJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListBatchSegmentJobsPaginator = client.get_paginator("list_batch_segment_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListBatchSegmentJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListBatchSegmentJobsPaginator](./paginators.md#listbatchsegmentjobspaginator)
3. item: [:material-code-braces: ListBatchSegmentJobsResponseTypeDef](./type_defs.md#listbatchsegmentjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBatchSegmentJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    solutionVersionArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBatchSegmentJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBatchSegmentJobsResponseTypeDef](./type_defs.md#listbatchsegmentjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBatchSegmentJobsRequestPaginateTypeDef = {  # (1)
    "solutionVersionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBatchSegmentJobsRequestPaginateTypeDef](./type_defs.md#listbatchsegmentjobsrequestpaginatetypedef) 
## ListCampaignsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_campaigns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListCampaigns.html#Personalize.Paginator.ListCampaigns)

```python
# ListCampaignsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListCampaignsPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListCampaignsPaginator = client.get_paginator("list_campaigns")  # (2)
    async for item in paginator.paginate(...):
        item: ListCampaignsResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)
3. item: [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCampaignsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    solutionArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCampaignsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCampaignsRequestPaginateTypeDef = {  # (1)
    "solutionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCampaignsRequestPaginateTypeDef](./type_defs.md#listcampaignsrequestpaginatetypedef) 
## ListDatasetExportJobsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_dataset_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListDatasetExportJobs.html#Personalize.Paginator.ListDatasetExportJobs)

```python
# ListDatasetExportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetExportJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListDatasetExportJobsPaginator = client.get_paginator("list_dataset_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetExportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListDatasetExportJobsPaginator](./paginators.md#listdatasetexportjobspaginator)
3. item: [:material-code-braces: ListDatasetExportJobsResponseTypeDef](./type_defs.md#listdatasetexportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetExportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datasetArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDatasetExportJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetExportJobsResponseTypeDef](./type_defs.md#listdatasetexportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetExportJobsRequestPaginateTypeDef = {  # (1)
    "datasetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetExportJobsRequestPaginateTypeDef](./type_defs.md#listdatasetexportjobsrequestpaginatetypedef) 
## ListDatasetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_dataset_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListDatasetGroups.html#Personalize.Paginator.ListDatasetGroups)

```python
# ListDatasetGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetGroupsPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListDatasetGroupsPaginator = client.get_paginator("list_dataset_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListDatasetGroupsPaginator](./paginators.md#listdatasetgroupspaginator)
3. item: [:material-code-braces: ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDatasetGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetGroupsRequestPaginateTypeDef](./type_defs.md#listdatasetgroupsrequestpaginatetypedef) 
## ListDatasetImportJobsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_dataset_import_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListDatasetImportJobs.html#Personalize.Paginator.ListDatasetImportJobs)

```python
# ListDatasetImportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetImportJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListDatasetImportJobsPaginator = client.get_paginator("list_dataset_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetImportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListDatasetImportJobsPaginator](./paginators.md#listdatasetimportjobspaginator)
3. item: [:material-code-braces: ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetImportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datasetArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDatasetImportJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetImportJobsRequestPaginateTypeDef = {  # (1)
    "datasetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetImportJobsRequestPaginateTypeDef](./type_defs.md#listdatasetimportjobsrequestpaginatetypedef) 
## ListDatasetsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListDatasets.html#Personalize.Paginator.ListDatasets)

```python
# ListDatasetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetsResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
3. item: [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datasetGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetsRequestPaginateTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestPaginateTypeDef](./type_defs.md#listdatasetsrequestpaginatetypedef) 
## ListEventTrackersPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_event_trackers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListEventTrackers.html#Personalize.Paginator.ListEventTrackers)

```python
# ListEventTrackersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListEventTrackersPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListEventTrackersPaginator = client.get_paginator("list_event_trackers")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventTrackersResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListEventTrackersPaginator](./paginators.md#listeventtrackerspaginator)
3. item: [:material-code-braces: ListEventTrackersResponseTypeDef](./type_defs.md#listeventtrackersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventTrackersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datasetGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEventTrackersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventTrackersResponseTypeDef](./type_defs.md#listeventtrackersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventTrackersRequestPaginateTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventTrackersRequestPaginateTypeDef](./type_defs.md#listeventtrackersrequestpaginatetypedef) 
## ListFiltersPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListFilters.html#Personalize.Paginator.ListFilters)

```python
# ListFiltersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListFiltersPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListFiltersPaginator = client.get_paginator("list_filters")  # (2)
    async for item in paginator.paginate(...):
        item: ListFiltersResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListFiltersPaginator](./paginators.md#listfilterspaginator)
3. item: [:material-code-braces: ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFiltersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datasetGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFiltersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFiltersRequestPaginateTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFiltersRequestPaginateTypeDef](./type_defs.md#listfiltersrequestpaginatetypedef) 
## ListMetricAttributionMetricsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_metric_attribution_metrics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListMetricAttributionMetrics.html#Personalize.Paginator.ListMetricAttributionMetrics)

```python
# ListMetricAttributionMetricsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListMetricAttributionMetricsPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListMetricAttributionMetricsPaginator = client.get_paginator("list_metric_attribution_metrics")  # (2)
    async for item in paginator.paginate(...):
        item: ListMetricAttributionMetricsResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListMetricAttributionMetricsPaginator](./paginators.md#listmetricattributionmetricspaginator)
3. item: [:material-code-braces: ListMetricAttributionMetricsResponseTypeDef](./type_defs.md#listmetricattributionmetricsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMetricAttributionMetricsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    metricAttributionArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMetricAttributionMetricsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMetricAttributionMetricsResponseTypeDef](./type_defs.md#listmetricattributionmetricsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMetricAttributionMetricsRequestPaginateTypeDef = {  # (1)
    "metricAttributionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMetricAttributionMetricsRequestPaginateTypeDef](./type_defs.md#listmetricattributionmetricsrequestpaginatetypedef) 
## ListMetricAttributionsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_metric_attributions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListMetricAttributions.html#Personalize.Paginator.ListMetricAttributions)

```python
# ListMetricAttributionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListMetricAttributionsPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListMetricAttributionsPaginator = client.get_paginator("list_metric_attributions")  # (2)
    async for item in paginator.paginate(...):
        item: ListMetricAttributionsResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListMetricAttributionsPaginator](./paginators.md#listmetricattributionspaginator)
3. item: [:material-code-braces: ListMetricAttributionsResponseTypeDef](./type_defs.md#listmetricattributionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMetricAttributionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datasetGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMetricAttributionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMetricAttributionsResponseTypeDef](./type_defs.md#listmetricattributionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMetricAttributionsRequestPaginateTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMetricAttributionsRequestPaginateTypeDef](./type_defs.md#listmetricattributionsrequestpaginatetypedef) 
## ListRecipesPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_recipes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListRecipes.html#Personalize.Paginator.ListRecipes)

```python
# ListRecipesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListRecipesPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListRecipesPaginator = client.get_paginator("list_recipes")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecipesResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListRecipesPaginator](./paginators.md#listrecipespaginator)
3. item: [:material-code-braces: ListRecipesResponseTypeDef](./type_defs.md#listrecipesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRecipesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    recipeProvider: RecipeProviderType = ...,  # (1)
    domain: DomainType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListRecipesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: RecipeProviderType](./literals.md#recipeprovidertype) 
2. See [:material-code-brackets: DomainType](./literals.md#domaintype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListRecipesResponseTypeDef](./type_defs.md#listrecipesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecipesRequestPaginateTypeDef = {  # (1)
    "recipeProvider": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecipesRequestPaginateTypeDef](./type_defs.md#listrecipesrequestpaginatetypedef) 
## ListRecommendersPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_recommenders")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListRecommenders.html#Personalize.Paginator.ListRecommenders)

```python
# ListRecommendersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListRecommendersPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListRecommendersPaginator = client.get_paginator("list_recommenders")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendersResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListRecommendersPaginator](./paginators.md#listrecommenderspaginator)
3. item: [:material-code-braces: ListRecommendersResponseTypeDef](./type_defs.md#listrecommendersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRecommendersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datasetGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRecommendersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecommendersResponseTypeDef](./type_defs.md#listrecommendersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendersRequestPaginateTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendersRequestPaginateTypeDef](./type_defs.md#listrecommendersrequestpaginatetypedef) 
## ListSchemasPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListSchemas.html#Personalize.Paginator.ListSchemas)

```python
# ListSchemasPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListSchemasPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListSchemasPaginator = client.get_paginator("list_schemas")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemasResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListSchemasPaginator](./paginators.md#listschemaspaginator)
3. item: [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemasPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSchemasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemasRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemasRequestPaginateTypeDef](./type_defs.md#listschemasrequestpaginatetypedef) 
## ListSolutionVersionsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_solution_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListSolutionVersions.html#Personalize.Paginator.ListSolutionVersions)

```python
# ListSolutionVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListSolutionVersionsPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListSolutionVersionsPaginator = client.get_paginator("list_solution_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSolutionVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListSolutionVersionsPaginator](./paginators.md#listsolutionversionspaginator)
3. item: [:material-code-braces: ListSolutionVersionsResponseTypeDef](./type_defs.md#listsolutionversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSolutionVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    solutionArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSolutionVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSolutionVersionsResponseTypeDef](./type_defs.md#listsolutionversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSolutionVersionsRequestPaginateTypeDef = {  # (1)
    "solutionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSolutionVersionsRequestPaginateTypeDef](./type_defs.md#listsolutionversionsrequestpaginatetypedef) 
## ListSolutionsPaginator

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator("list_solutions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize/paginator/ListSolutions.html#Personalize.Paginator.ListSolutions)

```python
# ListSolutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListSolutionsPaginator

session = get_session()
async with session.create_client("personalize") as client:  # (1)
    paginator: ListSolutionsPaginator = client.get_paginator("list_solutions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSolutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [PersonalizeClient](./client.md)
2. paginator: [ListSolutionsPaginator](./paginators.md#listsolutionspaginator)
3. item: [:material-code-braces: ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSolutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datasetGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSolutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSolutionsRequestPaginateTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSolutionsRequestPaginateTypeDef](./type_defs.md#listsolutionsrequestpaginatetypedef) 
