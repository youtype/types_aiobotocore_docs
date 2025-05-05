# Paginators

> [Index](../README.md) > [GlueDataBrew](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GlueDataBrew](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#gluedatabrew)
    type annotations stubs module [types-aiobotocore-databrew](https://pypi.org/project/types-aiobotocore-databrew/).

## ListDatasetsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew/paginator/ListDatasets.html#GlueDataBrew.Paginator.ListDatasets)

```python
# ListDatasetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("databrew") as client:  # (1)
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
3. item: `AioPageIterator[ListDatasetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDatasetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestPaginateTypeDef](./type_defs.md#listdatasetsrequestpaginatetypedef)
## ListJobRunsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_job_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew/paginator/ListJobRuns.html#GlueDataBrew.Paginator.ListJobRuns)

```python
# ListJobRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListJobRunsPaginator

session = get_session()
async with session.create_client("databrew") as client:  # (1)
    paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)
3. item: `AioPageIterator[ListJobRunsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListJobRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListJobRunsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListJobRunsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListJobRunsRequestPaginateTypeDef = {  # (1)
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobRunsRequestPaginateTypeDef](./type_defs.md#listjobrunsrequestpaginatetypedef)
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew/paginator/ListJobs.html#GlueDataBrew.Paginator.ListJobs)

```python
# ListJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("databrew") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: `AioPageIterator[ListJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DatasetName: str = ...,
    ProjectName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsRequestPaginateTypeDef = {  # (1)
    "DatasetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestPaginateTypeDef](./type_defs.md#listjobsrequestpaginatetypedef)
## ListProjectsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew/paginator/ListProjects.html#GlueDataBrew.Paginator.ListProjects)

```python
# ListProjectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("databrew") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: `AioPageIterator[ListProjectsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProjectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProjectsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestPaginateTypeDef](./type_defs.md#listprojectsrequestpaginatetypedef)
## ListRecipeVersionsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_recipe_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew/paginator/ListRecipeVersions.html#GlueDataBrew.Paginator.ListRecipeVersions)

```python
# ListRecipeVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListRecipeVersionsPaginator

session = get_session()
async with session.create_client("databrew") as client:  # (1)
    paginator: ListRecipeVersionsPaginator = client.get_paginator("list_recipe_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecipeVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListRecipeVersionsPaginator](./paginators.md#listrecipeversionspaginator)
3. item: `AioPageIterator[ListRecipeVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRecipeVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRecipeVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRecipeVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecipeVersionsRequestPaginateTypeDef = {  # (1)
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecipeVersionsRequestPaginateTypeDef](./type_defs.md#listrecipeversionsrequestpaginatetypedef)
## ListRecipesPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_recipes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew/paginator/ListRecipes.html#GlueDataBrew.Paginator.ListRecipes)

```python
# ListRecipesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListRecipesPaginator

session = get_session()
async with session.create_client("databrew") as client:  # (1)
    paginator: ListRecipesPaginator = client.get_paginator("list_recipes")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecipesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListRecipesPaginator](./paginators.md#listrecipespaginator)
3. item: `AioPageIterator[ListRecipesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRecipesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RecipeVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRecipesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRecipesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecipesRequestPaginateTypeDef = {  # (1)
    "RecipeVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecipesRequestPaginateTypeDef](./type_defs.md#listrecipesrequestpaginatetypedef)
## ListRulesetsPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_rulesets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew/paginator/ListRulesets.html#GlueDataBrew.Paginator.ListRulesets)

```python
# ListRulesetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListRulesetsPaginator

session = get_session()
async with session.create_client("databrew") as client:  # (1)
    paginator: ListRulesetsPaginator = client.get_paginator("list_rulesets")  # (2)
    async for item in paginator.paginate(...):
        item: ListRulesetsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListRulesetsPaginator](./paginators.md#listrulesetspaginator)
3. item: `AioPageIterator[ListRulesetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRulesetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TargetArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRulesetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRulesetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRulesetsRequestPaginateTypeDef = {  # (1)
    "TargetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRulesetsRequestPaginateTypeDef](./type_defs.md#listrulesetsrequestpaginatetypedef)
## ListSchedulesPaginator

Type annotations and code completion for `#!python session.create_client("databrew").get_paginator("list_schedules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew/paginator/ListSchedules.html#GlueDataBrew.Paginator.ListSchedules)

```python
# ListSchedulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_databrew.paginator import ListSchedulesPaginator

session = get_session()
async with session.create_client("databrew") as client:  # (1)
    paginator: ListSchedulesPaginator = client.get_paginator("list_schedules")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchedulesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlueDataBrewClient](./client.md)
2. paginator: [ListSchedulesPaginator](./paginators.md#listschedulespaginator)
3. item: `AioPageIterator[ListSchedulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSchedulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    JobName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSchedulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSchedulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSchedulesRequestPaginateTypeDef = {  # (1)
    "JobName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchedulesRequestPaginateTypeDef](./type_defs.md#listschedulesrequestpaginatetypedef)
