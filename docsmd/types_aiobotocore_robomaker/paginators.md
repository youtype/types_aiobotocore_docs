# Paginators

> [Index](../README.md) > [RoboMaker](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RoboMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
    type annotations stubs module [types-aiobotocore-robomaker](https://pypi.org/project/types-aiobotocore-robomaker/).

## ListDeploymentJobsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_deployment_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListDeploymentJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListDeploymentJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListDeploymentJobsPaginator = client.get_paginator("list_deployment_jobs")
```


### paginate

Type annotations and code completion for `#!python ListDeploymentJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDeploymentJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDeploymentJobsResponseTypeDef](./type_defs.md#listdeploymentjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef](./type_defs.md#listdeploymentjobsrequestlistdeploymentjobspaginatetypedef) 
## ListFleetsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListFleets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListFleetsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListFleetsPaginator = client.get_paginator("list_fleets")
```


### paginate

Type annotations and code completion for `#!python ListFleetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListFleetsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFleetsRequestListFleetsPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFleetsRequestListFleetsPaginateTypeDef](./type_defs.md#listfleetsrequestlistfleetspaginatetypedef) 
## ListRobotApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_robot_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobotApplications)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListRobotApplicationsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListRobotApplicationsPaginator = client.get_paginator("list_robot_applications")
```


### paginate

Type annotations and code completion for `#!python ListRobotApplicationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    versionQualifier: str = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListRobotApplicationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListRobotApplicationsResponseTypeDef](./type_defs.md#listrobotapplicationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = {  # (1)
    "versionQualifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef](./type_defs.md#listrobotapplicationsrequestlistrobotapplicationspaginatetypedef) 
## ListRobotsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_robots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobots)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListRobotsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListRobotsPaginator = client.get_paginator("list_robots")
```


### paginate

Type annotations and code completion for `#!python ListRobotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListRobotsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListRobotsResponseTypeDef](./type_defs.md#listrobotsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRobotsRequestListRobotsPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRobotsRequestListRobotsPaginateTypeDef](./type_defs.md#listrobotsrequestlistrobotspaginatetypedef) 
## ListSimulationApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_simulation_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationApplications)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListSimulationApplicationsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListSimulationApplicationsPaginator = client.get_paginator("list_simulation_applications")
```


### paginate

Type annotations and code completion for `#!python ListSimulationApplicationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    versionQualifier: str = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListSimulationApplicationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSimulationApplicationsResponseTypeDef](./type_defs.md#listsimulationapplicationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = {  # (1)
    "versionQualifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef](./type_defs.md#listsimulationapplicationsrequestlistsimulationapplicationspaginatetypedef) 
## ListSimulationJobBatchesPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_simulation_job_batches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobBatches)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListSimulationJobBatchesPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListSimulationJobBatchesPaginator = client.get_paginator("list_simulation_job_batches")
```


### paginate

Type annotations and code completion for `#!python ListSimulationJobBatchesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListSimulationJobBatchesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSimulationJobBatchesResponseTypeDef](./type_defs.md#listsimulationjobbatchesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef](./type_defs.md#listsimulationjobbatchesrequestlistsimulationjobbatchespaginatetypedef) 
## ListSimulationJobsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_simulation_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListSimulationJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListSimulationJobsPaginator = client.get_paginator("list_simulation_jobs")
```


### paginate

Type annotations and code completion for `#!python ListSimulationJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListSimulationJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSimulationJobsResponseTypeDef](./type_defs.md#listsimulationjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSimulationJobsRequestListSimulationJobsPaginateTypeDef](./type_defs.md#listsimulationjobsrequestlistsimulationjobspaginatetypedef) 
## ListWorldExportJobsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_world_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldExportJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldExportJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListWorldExportJobsPaginator = client.get_paginator("list_world_export_jobs")
```


### paginate

Type annotations and code completion for `#!python ListWorldExportJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListWorldExportJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWorldExportJobsResponseTypeDef](./type_defs.md#listworldexportjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef](./type_defs.md#listworldexportjobsrequestlistworldexportjobspaginatetypedef) 
## ListWorldGenerationJobsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_world_generation_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldGenerationJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldGenerationJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListWorldGenerationJobsPaginator = client.get_paginator("list_world_generation_jobs")
```


### paginate

Type annotations and code completion for `#!python ListWorldGenerationJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListWorldGenerationJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWorldGenerationJobsResponseTypeDef](./type_defs.md#listworldgenerationjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef](./type_defs.md#listworldgenerationjobsrequestlistworldgenerationjobspaginatetypedef) 
## ListWorldTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_world_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldTemplatesPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListWorldTemplatesPaginator = client.get_paginator("list_world_templates")
```


### paginate

Type annotations and code completion for `#!python ListWorldTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListWorldTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorldTemplatesResponseTypeDef](./type_defs.md#listworldtemplatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef](./type_defs.md#listworldtemplatesrequestlistworldtemplatespaginatetypedef) 
## ListWorldsPaginator

Type annotations and code completion for `#!python session.create_client("robomaker").get_paginator("list_worlds")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorlds)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListWorldsPaginator = client.get_paginator("list_worlds")
```


### paginate

Type annotations and code completion for `#!python ListWorldsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListWorldsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWorldsResponseTypeDef](./type_defs.md#listworldsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListWorldsRequestListWorldsPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorldsRequestListWorldsPaginateTypeDef](./type_defs.md#listworldsrequestlistworldspaginatetypedef) 
