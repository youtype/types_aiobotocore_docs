# Paginators

> [Index](../README.md) > [RoboMaker](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RoboMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#robomaker)
    type annotations stubs module [types-aiobotocore-robomaker](https://pypi.org/project/types-aiobotocore-robomaker/).

## ListDeploymentJobsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_deployment_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/paginator/ListDeploymentJobs.html#RoboMaker.Paginator.ListDeploymentJobs)

```python
# ListDeploymentJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListDeploymentJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:  # (1)
    paginator: ListDeploymentJobsPaginator = client.get_paginator("list_deployment_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListDeploymentJobsPaginator](./paginators.md#listdeploymentjobspaginator)
3. item: [:material-code-braces: ListDeploymentJobsResponseTypeDef](./type_defs.md#listdeploymentjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDeploymentJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDeploymentJobsResponseTypeDef](./type_defs.md#listdeploymentjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeploymentJobsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentJobsRequestPaginateTypeDef](./type_defs.md#listdeploymentjobsrequestpaginatetypedef) 
## ListFleetsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/paginator/ListFleets.html#RoboMaker.Paginator.ListFleets)

```python
# ListFleetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListFleetsPaginator

session = get_session()
async with session.create_client("robomaker") as client:  # (1)
    paginator: ListFleetsPaginator = client.get_paginator("list_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: ListFleetsResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListFleetsPaginator](./paginators.md#listfleetspaginator)
3. item: [:material-code-braces: ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListFleetsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFleetsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFleetsRequestPaginateTypeDef](./type_defs.md#listfleetsrequestpaginatetypedef) 
## ListRobotApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_robot_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/paginator/ListRobotApplications.html#RoboMaker.Paginator.ListRobotApplications)

```python
# ListRobotApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListRobotApplicationsPaginator

session = get_session()
async with session.create_client("robomaker") as client:  # (1)
    paginator: ListRobotApplicationsPaginator = client.get_paginator("list_robot_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListRobotApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListRobotApplicationsPaginator](./paginators.md#listrobotapplicationspaginator)
3. item: [:material-code-braces: ListRobotApplicationsResponseTypeDef](./type_defs.md#listrobotapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRobotApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    versionQualifier: str = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListRobotApplicationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListRobotApplicationsResponseTypeDef](./type_defs.md#listrobotapplicationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRobotApplicationsRequestPaginateTypeDef = {  # (1)
    "versionQualifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRobotApplicationsRequestPaginateTypeDef](./type_defs.md#listrobotapplicationsrequestpaginatetypedef) 
## ListRobotsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_robots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/paginator/ListRobots.html#RoboMaker.Paginator.ListRobots)

```python
# ListRobotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListRobotsPaginator

session = get_session()
async with session.create_client("robomaker") as client:  # (1)
    paginator: ListRobotsPaginator = client.get_paginator("list_robots")  # (2)
    async for item in paginator.paginate(...):
        item: ListRobotsResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListRobotsPaginator](./paginators.md#listrobotspaginator)
3. item: [:material-code-braces: ListRobotsResponseTypeDef](./type_defs.md#listrobotsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRobotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListRobotsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListRobotsResponseTypeDef](./type_defs.md#listrobotsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRobotsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRobotsRequestPaginateTypeDef](./type_defs.md#listrobotsrequestpaginatetypedef) 
## ListSimulationApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_simulation_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/paginator/ListSimulationApplications.html#RoboMaker.Paginator.ListSimulationApplications)

```python
# ListSimulationApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListSimulationApplicationsPaginator

session = get_session()
async with session.create_client("robomaker") as client:  # (1)
    paginator: ListSimulationApplicationsPaginator = client.get_paginator("list_simulation_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListSimulationApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListSimulationApplicationsPaginator](./paginators.md#listsimulationapplicationspaginator)
3. item: [:material-code-braces: ListSimulationApplicationsResponseTypeDef](./type_defs.md#listsimulationapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSimulationApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    versionQualifier: str = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSimulationApplicationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSimulationApplicationsResponseTypeDef](./type_defs.md#listsimulationapplicationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSimulationApplicationsRequestPaginateTypeDef = {  # (1)
    "versionQualifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSimulationApplicationsRequestPaginateTypeDef](./type_defs.md#listsimulationapplicationsrequestpaginatetypedef) 
## ListSimulationJobBatchesPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_simulation_job_batches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/paginator/ListSimulationJobBatches.html#RoboMaker.Paginator.ListSimulationJobBatches)

```python
# ListSimulationJobBatchesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListSimulationJobBatchesPaginator

session = get_session()
async with session.create_client("robomaker") as client:  # (1)
    paginator: ListSimulationJobBatchesPaginator = client.get_paginator("list_simulation_job_batches")  # (2)
    async for item in paginator.paginate(...):
        item: ListSimulationJobBatchesResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListSimulationJobBatchesPaginator](./paginators.md#listsimulationjobbatchespaginator)
3. item: [:material-code-braces: ListSimulationJobBatchesResponseTypeDef](./type_defs.md#listsimulationjobbatchesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSimulationJobBatchesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSimulationJobBatchesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSimulationJobBatchesResponseTypeDef](./type_defs.md#listsimulationjobbatchesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSimulationJobBatchesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSimulationJobBatchesRequestPaginateTypeDef](./type_defs.md#listsimulationjobbatchesrequestpaginatetypedef) 
## ListSimulationJobsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_simulation_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/paginator/ListSimulationJobs.html#RoboMaker.Paginator.ListSimulationJobs)

```python
# ListSimulationJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListSimulationJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:  # (1)
    paginator: ListSimulationJobsPaginator = client.get_paginator("list_simulation_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListSimulationJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListSimulationJobsPaginator](./paginators.md#listsimulationjobspaginator)
3. item: [:material-code-braces: ListSimulationJobsResponseTypeDef](./type_defs.md#listsimulationjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSimulationJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSimulationJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSimulationJobsResponseTypeDef](./type_defs.md#listsimulationjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSimulationJobsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSimulationJobsRequestPaginateTypeDef](./type_defs.md#listsimulationjobsrequestpaginatetypedef) 
## ListWorldExportJobsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_world_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/paginator/ListWorldExportJobs.html#RoboMaker.Paginator.ListWorldExportJobs)

```python
# ListWorldExportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldExportJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:  # (1)
    paginator: ListWorldExportJobsPaginator = client.get_paginator("list_world_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorldExportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListWorldExportJobsPaginator](./paginators.md#listworldexportjobspaginator)
3. item: [:material-code-braces: ListWorldExportJobsResponseTypeDef](./type_defs.md#listworldexportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorldExportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListWorldExportJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWorldExportJobsResponseTypeDef](./type_defs.md#listworldexportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorldExportJobsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorldExportJobsRequestPaginateTypeDef](./type_defs.md#listworldexportjobsrequestpaginatetypedef) 
## ListWorldGenerationJobsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_world_generation_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/paginator/ListWorldGenerationJobs.html#RoboMaker.Paginator.ListWorldGenerationJobs)

```python
# ListWorldGenerationJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldGenerationJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:  # (1)
    paginator: ListWorldGenerationJobsPaginator = client.get_paginator("list_world_generation_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorldGenerationJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListWorldGenerationJobsPaginator](./paginators.md#listworldgenerationjobspaginator)
3. item: [:material-code-braces: ListWorldGenerationJobsResponseTypeDef](./type_defs.md#listworldgenerationjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorldGenerationJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListWorldGenerationJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWorldGenerationJobsResponseTypeDef](./type_defs.md#listworldgenerationjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorldGenerationJobsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorldGenerationJobsRequestPaginateTypeDef](./type_defs.md#listworldgenerationjobsrequestpaginatetypedef) 
## ListWorldTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_world_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/paginator/ListWorldTemplates.html#RoboMaker.Paginator.ListWorldTemplates)

```python
# ListWorldTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldTemplatesPaginator

session = get_session()
async with session.create_client("robomaker") as client:  # (1)
    paginator: ListWorldTemplatesPaginator = client.get_paginator("list_world_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorldTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListWorldTemplatesPaginator](./paginators.md#listworldtemplatespaginator)
3. item: [:material-code-braces: ListWorldTemplatesResponseTypeDef](./type_defs.md#listworldtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorldTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorldTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorldTemplatesResponseTypeDef](./type_defs.md#listworldtemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorldTemplatesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorldTemplatesRequestPaginateTypeDef](./type_defs.md#listworldtemplatesrequestpaginatetypedef) 
## ListWorldsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_worlds")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker/paginator/ListWorlds.html#RoboMaker.Paginator.ListWorlds)

```python
# ListWorldsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldsPaginator

session = get_session()
async with session.create_client("robomaker") as client:  # (1)
    paginator: ListWorldsPaginator = client.get_paginator("list_worlds")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorldsResponseTypeDef
        print(item)  # (3)
```

1. client: [RoboMakerClient](./client.md)
2. paginator: [ListWorldsPaginator](./paginators.md#listworldspaginator)
3. item: [:material-code-braces: ListWorldsResponseTypeDef](./type_defs.md#listworldsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorldsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListWorldsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWorldsResponseTypeDef](./type_defs.md#listworldsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorldsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorldsRequestPaginateTypeDef](./type_defs.md#listworldsrequestpaginatetypedef) 
