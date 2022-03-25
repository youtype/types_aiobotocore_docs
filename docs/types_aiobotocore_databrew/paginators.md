<a id="paginators-for-aiobotocore-gluedatabrew-module"></a>

# Paginators for aiobotocore GlueDataBrew module

> [Index](../README.md) > [GlueDataBrew](./README.md) > Paginators

Auto-generated documentation for
[GlueDataBrew](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
type annotations stubs module
[types-aiobotocore-databrew](https://pypi.org/project/types-aiobotocore-databrew/).

- [Paginators for aiobotocore GlueDataBrew module](#paginators-for-aiobotocore-gluedatabrew-module)
  - [ListDatasetsPaginator](#listdatasetspaginator)
  - [ListJobRunsPaginator](#listjobrunspaginator)
  - [ListJobsPaginator](#listjobspaginator)
  - [ListProjectsPaginator](#listprojectspaginator)
  - [ListRecipeVersionsPaginator](#listrecipeversionspaginator)
  - [ListRecipesPaginator](#listrecipespaginator)
  - [ListRulesetsPaginator](#listrulesetspaginator)
  - [ListSchedulesPaginator](#listschedulespaginator)

<a id="listdatasetspaginator"></a>

## ListDatasetsPaginator

Type annotations for
`session.create_client("databrew").get_paginator("list_datasets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
```

Boto3 documentation:
[GlueDataBrew.Paginator.ListDatasets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets)

Arguments for `ListDatasetsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatasetsPaginator.paginate` returns
`AsyncIterator`\[[ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)\].

<a id="listjobrunspaginator"></a>

## ListJobRunsPaginator

Type annotations for
`session.create_client("databrew").get_paginator("list_job_runs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListJobRunsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
```

Boto3 documentation:
[GlueDataBrew.Paginator.ListJobRuns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns)

Arguments for `ListJobRunsPaginator.paginate` method:

- `Name`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobRunsPaginator.paginate` returns
`AsyncIterator`\[[ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef)\].

<a id="listjobspaginator"></a>

## ListJobsPaginator

Type annotations for
`session.create_client("databrew").get_paginator("list_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
```

Boto3 documentation:
[GlueDataBrew.Paginator.ListJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobs)

Arguments for `ListJobsPaginator.paginate` method:

- `DatasetName`: `str`
- `ProjectName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsPaginator.paginate` returns
`AsyncIterator`\[[ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef)\].

<a id="listprojectspaginator"></a>

## ListProjectsPaginator

Type annotations for
`session.create_client("databrew").get_paginator("list_projects")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")
```

Boto3 documentation:
[GlueDataBrew.Paginator.ListProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects)

Arguments for `ListProjectsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProjectsPaginator.paginate` returns
`AsyncIterator`\[[ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef)\].

<a id="listrecipeversionspaginator"></a>

## ListRecipeVersionsPaginator

Type annotations for
`session.create_client("databrew").get_paginator("list_recipe_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListRecipeVersionsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListRecipeVersionsPaginator = client.get_paginator("list_recipe_versions")
```

Boto3 documentation:
[GlueDataBrew.Paginator.ListRecipeVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions)

Arguments for `ListRecipeVersionsPaginator.paginate` method:

- `Name`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRecipeVersionsPaginator.paginate` returns
`AsyncIterator`\[[ListRecipeVersionsResponseTypeDef](./type_defs.md#listrecipeversionsresponsetypedef)\].

<a id="listrecipespaginator"></a>

## ListRecipesPaginator

Type annotations for
`session.create_client("databrew").get_paginator("list_recipes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListRecipesPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListRecipesPaginator = client.get_paginator("list_recipes")
```

Boto3 documentation:
[GlueDataBrew.Paginator.ListRecipes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes)

Arguments for `ListRecipesPaginator.paginate` method:

- `RecipeVersion`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRecipesPaginator.paginate` returns
`AsyncIterator`\[[ListRecipesResponseTypeDef](./type_defs.md#listrecipesresponsetypedef)\].

<a id="listrulesetspaginator"></a>

## ListRulesetsPaginator

Type annotations for
`session.create_client("databrew").get_paginator("list_rulesets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListRulesetsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListRulesetsPaginator = client.get_paginator("list_rulesets")
```

Boto3 documentation:
[GlueDataBrew.Paginator.ListRulesets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets)

Arguments for `ListRulesetsPaginator.paginate` method:

- `TargetArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRulesetsPaginator.paginate` returns
`AsyncIterator`\[[ListRulesetsResponseTypeDef](./type_defs.md#listrulesetsresponsetypedef)\].

<a id="listschedulespaginator"></a>

## ListSchedulesPaginator

Type annotations for
`session.create_client("databrew").get_paginator("list_schedules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListSchedulesPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListSchedulesPaginator = client.get_paginator("list_schedules")
```

Boto3 documentation:
[GlueDataBrew.Paginator.ListSchedules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules)

Arguments for `ListSchedulesPaginator.paginate` method:

- `JobName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSchedulesPaginator.paginate` returns
`AsyncIterator`\[[ListSchedulesResponseTypeDef](./type_defs.md#listschedulesresponsetypedef)\].