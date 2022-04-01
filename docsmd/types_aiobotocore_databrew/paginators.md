# Paginators

> [Index](../README.md) > [GlueDataBrew](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GlueDataBrew](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
    type annotations stubs module [types-aiobotocore-databrew](https://pypi.org/project/types-aiobotocore-databrew/).

## ListDatasetsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
```


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetsRequestListDatasetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef) 
## ListJobRunsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_job_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListJobRunsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
```


### paginate

Type annotations and code completion for `#!python ListJobRunsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobRunsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobRunsRequestListJobRunsPaginateTypeDef = {  # (1)
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobRunsRequestListJobRunsPaginateTypeDef](./type_defs.md#listjobrunsrequestlistjobrunspaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
```


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DatasetName: str = ...,
    ProjectName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsRequestListJobsPaginateTypeDef = {  # (1)
    "DatasetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestListJobsPaginateTypeDef](./type_defs.md#listjobsrequestlistjobspaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")
```


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProjectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListProjectsRequestListProjectsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestListProjectsPaginateTypeDef](./type_defs.md#listprojectsrequestlistprojectspaginatetypedef) 
## ListRecipeVersionsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_recipe_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListRecipeVersionsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListRecipeVersionsPaginator = client.get_paginator("list_recipe_versions")
```


### paginate

Type annotations and code completion for `#!python ListRecipeVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecipeVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecipeVersionsResponseTypeDef](./type_defs.md#listrecipeversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = {  # (1)
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef](./type_defs.md#listrecipeversionsrequestlistrecipeversionspaginatetypedef) 
## ListRecipesPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_recipes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListRecipesPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListRecipesPaginator = client.get_paginator("list_recipes")
```


### paginate

Type annotations and code completion for `#!python ListRecipesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RecipeVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecipesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecipesResponseTypeDef](./type_defs.md#listrecipesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRecipesRequestListRecipesPaginateTypeDef = {  # (1)
    "RecipeVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecipesRequestListRecipesPaginateTypeDef](./type_defs.md#listrecipesrequestlistrecipespaginatetypedef) 
## ListRulesetsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_rulesets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListRulesetsPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListRulesetsPaginator = client.get_paginator("list_rulesets")
```


### paginate

Type annotations and code completion for `#!python ListRulesetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TargetArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRulesetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRulesetsResponseTypeDef](./type_defs.md#listrulesetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRulesetsRequestListRulesetsPaginateTypeDef = {  # (1)
    "TargetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRulesetsRequestListRulesetsPaginateTypeDef](./type_defs.md#listrulesetsrequestlistrulesetspaginatetypedef) 
## ListSchedulesPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_schedules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListSchedulesPaginator

session = get_session()
async with session.create_client("databrew") as client:
    client: GlueDataBrewClient
    paginator: ListSchedulesPaginator = client.get_paginator("list_schedules")
```


### paginate

Type annotations and code completion for `#!python ListSchedulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    JobName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSchedulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchedulesResponseTypeDef](./type_defs.md#listschedulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSchedulesRequestListSchedulesPaginateTypeDef = {  # (1)
    "JobName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchedulesRequestListSchedulesPaginateTypeDef](./type_defs.md#listschedulesrequestlistschedulespaginatetypedef) 
