<a id="paginators-for-aiobotocore-personalize-module"></a>

# Paginators for aiobotocore Personalize module

> [Index](../README.md) > [Personalize](./README.md) > Paginators

Auto-generated documentation for
[Personalize](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
type annotations stubs module
[types-aiobotocore-personalize](https://pypi.org/project/types-aiobotocore-personalize/).

- [Paginators for aiobotocore Personalize module](#paginators-for-aiobotocore-personalize-module)
  - [ListBatchInferenceJobsPaginator](#listbatchinferencejobspaginator)
  - [ListBatchSegmentJobsPaginator](#listbatchsegmentjobspaginator)
  - [ListCampaignsPaginator](#listcampaignspaginator)
  - [ListDatasetExportJobsPaginator](#listdatasetexportjobspaginator)
  - [ListDatasetGroupsPaginator](#listdatasetgroupspaginator)
  - [ListDatasetImportJobsPaginator](#listdatasetimportjobspaginator)
  - [ListDatasetsPaginator](#listdatasetspaginator)
  - [ListEventTrackersPaginator](#listeventtrackerspaginator)
  - [ListFiltersPaginator](#listfilterspaginator)
  - [ListRecipesPaginator](#listrecipespaginator)
  - [ListRecommendersPaginator](#listrecommenderspaginator)
  - [ListSchemasPaginator](#listschemaspaginator)
  - [ListSolutionVersionsPaginator](#listsolutionversionspaginator)
  - [ListSolutionsPaginator](#listsolutionspaginator)

<a id="listbatchinferencejobspaginator"></a>

## ListBatchInferenceJobsPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_batch_inference_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListBatchInferenceJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListBatchInferenceJobsPaginator = client.get_paginator("list_batch_inference_jobs")
```

Boto3 documentation:
[Personalize.Paginator.ListBatchInferenceJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchInferenceJobs)

Arguments for `ListBatchInferenceJobsPaginator.paginate` method:

- `solutionVersionArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBatchInferenceJobsPaginator.paginate` returns
`AsyncIterator`\[[ListBatchInferenceJobsResponseTypeDef](./type_defs.md#listbatchinferencejobsresponsetypedef)\].

<a id="listbatchsegmentjobspaginator"></a>

## ListBatchSegmentJobsPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_batch_segment_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListBatchSegmentJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListBatchSegmentJobsPaginator = client.get_paginator("list_batch_segment_jobs")
```

Boto3 documentation:
[Personalize.Paginator.ListBatchSegmentJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListBatchSegmentJobs)

Arguments for `ListBatchSegmentJobsPaginator.paginate` method:

- `solutionVersionArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBatchSegmentJobsPaginator.paginate` returns
`AsyncIterator`\[[ListBatchSegmentJobsResponseTypeDef](./type_defs.md#listbatchsegmentjobsresponsetypedef)\].

<a id="listcampaignspaginator"></a>

## ListCampaignsPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_campaigns")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListCampaignsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListCampaignsPaginator = client.get_paginator("list_campaigns")
```

Boto3 documentation:
[Personalize.Paginator.ListCampaigns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListCampaigns)

Arguments for `ListCampaignsPaginator.paginate` method:

- `solutionArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCampaignsPaginator.paginate` returns
`AsyncIterator`\[[ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef)\].

<a id="listdatasetexportjobspaginator"></a>

## ListDatasetExportJobsPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_dataset_export_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetExportJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListDatasetExportJobsPaginator = client.get_paginator("list_dataset_export_jobs")
```

Boto3 documentation:
[Personalize.Paginator.ListDatasetExportJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetExportJobs)

Arguments for `ListDatasetExportJobsPaginator.paginate` method:

- `datasetArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatasetExportJobsPaginator.paginate` returns
`AsyncIterator`\[[ListDatasetExportJobsResponseTypeDef](./type_defs.md#listdatasetexportjobsresponsetypedef)\].

<a id="listdatasetgroupspaginator"></a>

## ListDatasetGroupsPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_dataset_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetGroupsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListDatasetGroupsPaginator = client.get_paginator("list_dataset_groups")
```

Boto3 documentation:
[Personalize.Paginator.ListDatasetGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetGroups)

Arguments for `ListDatasetGroupsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatasetGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef)\].

<a id="listdatasetimportjobspaginator"></a>

## ListDatasetImportJobsPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_dataset_import_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetImportJobsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListDatasetImportJobsPaginator = client.get_paginator("list_dataset_import_jobs")
```

Boto3 documentation:
[Personalize.Paginator.ListDatasetImportJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasetImportJobs)

Arguments for `ListDatasetImportJobsPaginator.paginate` method:

- `datasetArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatasetImportJobsPaginator.paginate` returns
`AsyncIterator`\[[ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef)\].

<a id="listdatasetspaginator"></a>

## ListDatasetsPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_datasets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
```

Boto3 documentation:
[Personalize.Paginator.ListDatasets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListDatasets)

Arguments for `ListDatasetsPaginator.paginate` method:

- `datasetGroupArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatasetsPaginator.paginate` returns
`AsyncIterator`\[[ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)\].

<a id="listeventtrackerspaginator"></a>

## ListEventTrackersPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_event_trackers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListEventTrackersPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListEventTrackersPaginator = client.get_paginator("list_event_trackers")
```

Boto3 documentation:
[Personalize.Paginator.ListEventTrackers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListEventTrackers)

Arguments for `ListEventTrackersPaginator.paginate` method:

- `datasetGroupArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEventTrackersPaginator.paginate` returns
`AsyncIterator`\[[ListEventTrackersResponseTypeDef](./type_defs.md#listeventtrackersresponsetypedef)\].

<a id="listfilterspaginator"></a>

## ListFiltersPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_filters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListFiltersPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListFiltersPaginator = client.get_paginator("list_filters")
```

Boto3 documentation:
[Personalize.Paginator.ListFilters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListFilters)

Arguments for `ListFiltersPaginator.paginate` method:

- `datasetGroupArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFiltersPaginator.paginate` returns
`AsyncIterator`\[[ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef)\].

<a id="listrecipespaginator"></a>

## ListRecipesPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_recipes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListRecipesPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListRecipesPaginator = client.get_paginator("list_recipes")
```

Boto3 documentation:
[Personalize.Paginator.ListRecipes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecipes)

Arguments for `ListRecipesPaginator.paginate` method:

- `recipeProvider`: `Literal['SERVICE']` (see
  [RecipeProviderType](./literals.md#recipeprovidertype))
- `domain`: [DomainType](./literals.md#domaintype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRecipesPaginator.paginate` returns
`AsyncIterator`\[[ListRecipesResponseTypeDef](./type_defs.md#listrecipesresponsetypedef)\].

<a id="listrecommenderspaginator"></a>

## ListRecommendersPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_recommenders")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListRecommendersPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListRecommendersPaginator = client.get_paginator("list_recommenders")
```

Boto3 documentation:
[Personalize.Paginator.ListRecommenders](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecommenders)

Arguments for `ListRecommendersPaginator.paginate` method:

- `datasetGroupArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRecommendersPaginator.paginate` returns
`AsyncIterator`\[[ListRecommendersResponseTypeDef](./type_defs.md#listrecommendersresponsetypedef)\].

<a id="listschemaspaginator"></a>

## ListSchemasPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_schemas")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListSchemasPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListSchemasPaginator = client.get_paginator("list_schemas")
```

Boto3 documentation:
[Personalize.Paginator.ListSchemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSchemas)

Arguments for `ListSchemasPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSchemasPaginator.paginate` returns
`AsyncIterator`\[[ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef)\].

<a id="listsolutionversionspaginator"></a>

## ListSolutionVersionsPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_solution_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListSolutionVersionsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListSolutionVersionsPaginator = client.get_paginator("list_solution_versions")
```

Boto3 documentation:
[Personalize.Paginator.ListSolutionVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutionVersions)

Arguments for `ListSolutionVersionsPaginator.paginate` method:

- `solutionArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSolutionVersionsPaginator.paginate` returns
`AsyncIterator`\[[ListSolutionVersionsResponseTypeDef](./type_defs.md#listsolutionversionsresponsetypedef)\].

<a id="listsolutionspaginator"></a>

## ListSolutionsPaginator

Type annotations for
`session.create_client("personalize").get_paginator("list_solutions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize.paginator import ListSolutionsPaginator

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
    paginator: ListSolutionsPaginator = client.get_paginator("list_solutions")
```

Boto3 documentation:
[Personalize.Paginator.ListSolutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListSolutions)

Arguments for `ListSolutionsPaginator.paginate` method:

- `datasetGroupArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSolutionsPaginator.paginate` returns
`AsyncIterator`\[[ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef)\].
