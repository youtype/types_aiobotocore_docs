<a id="paginators-for-aiobotocore-robomaker-module"></a>

# Paginators for aiobotocore RoboMaker module

> [Index](../README.md) > [RoboMaker](./README.md) > Paginators

Auto-generated documentation for
[RoboMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
type annotations stubs module
[types-aiobotocore-robomaker](https://pypi.org/project/types-aiobotocore-robomaker/).

- [Paginators for aiobotocore RoboMaker module](#paginators-for-aiobotocore-robomaker-module)
  - [ListDeploymentJobsPaginator](#listdeploymentjobspaginator)
  - [ListFleetsPaginator](#listfleetspaginator)
  - [ListRobotApplicationsPaginator](#listrobotapplicationspaginator)
  - [ListRobotsPaginator](#listrobotspaginator)
  - [ListSimulationApplicationsPaginator](#listsimulationapplicationspaginator)
  - [ListSimulationJobBatchesPaginator](#listsimulationjobbatchespaginator)
  - [ListSimulationJobsPaginator](#listsimulationjobspaginator)
  - [ListWorldExportJobsPaginator](#listworldexportjobspaginator)
  - [ListWorldGenerationJobsPaginator](#listworldgenerationjobspaginator)
  - [ListWorldTemplatesPaginator](#listworldtemplatespaginator)
  - [ListWorldsPaginator](#listworldspaginator)

<a id="listdeploymentjobspaginator"></a>

## ListDeploymentJobsPaginator

Type annotations for
`session.create_client("robomaker").get_paginator("list_deployment_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListDeploymentJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListDeploymentJobsPaginator = client.get_paginator("list_deployment_jobs")
```

Boto3 documentation:
[RoboMaker.Paginator.ListDeploymentJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListDeploymentJobs)

Arguments for `ListDeploymentJobsPaginator.paginate` method:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeploymentJobsPaginator.paginate` returns
`AsyncIterator`\[[ListDeploymentJobsResponseTypeDef](./type_defs.md#listdeploymentjobsresponsetypedef)\].

<a id="listfleetspaginator"></a>

## ListFleetsPaginator

Type annotations for
`session.create_client("robomaker").get_paginator("list_fleets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListFleetsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListFleetsPaginator = client.get_paginator("list_fleets")
```

Boto3 documentation:
[RoboMaker.Paginator.ListFleets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListFleets)

Arguments for `ListFleetsPaginator.paginate` method:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFleetsPaginator.paginate` returns
`AsyncIterator`\[[ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef)\].

<a id="listrobotapplicationspaginator"></a>

## ListRobotApplicationsPaginator

Type annotations for
`session.create_client("robomaker").get_paginator("list_robot_applications")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListRobotApplicationsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListRobotApplicationsPaginator = client.get_paginator("list_robot_applications")
```

Boto3 documentation:
[RoboMaker.Paginator.ListRobotApplications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobotApplications)

Arguments for `ListRobotApplicationsPaginator.paginate` method:

- `versionQualifier`: `str`
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRobotApplicationsPaginator.paginate` returns
`AsyncIterator`\[[ListRobotApplicationsResponseTypeDef](./type_defs.md#listrobotapplicationsresponsetypedef)\].

<a id="listrobotspaginator"></a>

## ListRobotsPaginator

Type annotations for
`session.create_client("robomaker").get_paginator("list_robots")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListRobotsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListRobotsPaginator = client.get_paginator("list_robots")
```

Boto3 documentation:
[RoboMaker.Paginator.ListRobots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobots)

Arguments for `ListRobotsPaginator.paginate` method:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRobotsPaginator.paginate` returns
`AsyncIterator`\[[ListRobotsResponseTypeDef](./type_defs.md#listrobotsresponsetypedef)\].

<a id="listsimulationapplicationspaginator"></a>

## ListSimulationApplicationsPaginator

Type annotations for
`session.create_client("robomaker").get_paginator("list_simulation_applications")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListSimulationApplicationsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListSimulationApplicationsPaginator = client.get_paginator("list_simulation_applications")
```

Boto3 documentation:
[RoboMaker.Paginator.ListSimulationApplications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationApplications)

Arguments for `ListSimulationApplicationsPaginator.paginate` method:

- `versionQualifier`: `str`
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSimulationApplicationsPaginator.paginate` returns
`AsyncIterator`\[[ListSimulationApplicationsResponseTypeDef](./type_defs.md#listsimulationapplicationsresponsetypedef)\].

<a id="listsimulationjobbatchespaginator"></a>

## ListSimulationJobBatchesPaginator

Type annotations for
`session.create_client("robomaker").get_paginator("list_simulation_job_batches")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListSimulationJobBatchesPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListSimulationJobBatchesPaginator = client.get_paginator("list_simulation_job_batches")
```

Boto3 documentation:
[RoboMaker.Paginator.ListSimulationJobBatches](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobBatches)

Arguments for `ListSimulationJobBatchesPaginator.paginate` method:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSimulationJobBatchesPaginator.paginate` returns
`AsyncIterator`\[[ListSimulationJobBatchesResponseTypeDef](./type_defs.md#listsimulationjobbatchesresponsetypedef)\].

<a id="listsimulationjobspaginator"></a>

## ListSimulationJobsPaginator

Type annotations for
`session.create_client("robomaker").get_paginator("list_simulation_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListSimulationJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListSimulationJobsPaginator = client.get_paginator("list_simulation_jobs")
```

Boto3 documentation:
[RoboMaker.Paginator.ListSimulationJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobs)

Arguments for `ListSimulationJobsPaginator.paginate` method:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSimulationJobsPaginator.paginate` returns
`AsyncIterator`\[[ListSimulationJobsResponseTypeDef](./type_defs.md#listsimulationjobsresponsetypedef)\].

<a id="listworldexportjobspaginator"></a>

## ListWorldExportJobsPaginator

Type annotations for
`session.create_client("robomaker").get_paginator("list_world_export_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldExportJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListWorldExportJobsPaginator = client.get_paginator("list_world_export_jobs")
```

Boto3 documentation:
[RoboMaker.Paginator.ListWorldExportJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldExportJobs)

Arguments for `ListWorldExportJobsPaginator.paginate` method:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWorldExportJobsPaginator.paginate` returns
`AsyncIterator`\[[ListWorldExportJobsResponseTypeDef](./type_defs.md#listworldexportjobsresponsetypedef)\].

<a id="listworldgenerationjobspaginator"></a>

## ListWorldGenerationJobsPaginator

Type annotations for
`session.create_client("robomaker").get_paginator("list_world_generation_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldGenerationJobsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListWorldGenerationJobsPaginator = client.get_paginator("list_world_generation_jobs")
```

Boto3 documentation:
[RoboMaker.Paginator.ListWorldGenerationJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldGenerationJobs)

Arguments for `ListWorldGenerationJobsPaginator.paginate` method:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWorldGenerationJobsPaginator.paginate` returns
`AsyncIterator`\[[ListWorldGenerationJobsResponseTypeDef](./type_defs.md#listworldgenerationjobsresponsetypedef)\].

<a id="listworldtemplatespaginator"></a>

## ListWorldTemplatesPaginator

Type annotations for
`session.create_client("robomaker").get_paginator("list_world_templates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldTemplatesPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListWorldTemplatesPaginator = client.get_paginator("list_world_templates")
```

Boto3 documentation:
[RoboMaker.Paginator.ListWorldTemplates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates)

Arguments for `ListWorldTemplatesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWorldTemplatesPaginator.paginate` returns
`AsyncIterator`\[[ListWorldTemplatesResponseTypeDef](./type_defs.md#listworldtemplatesresponsetypedef)\].

<a id="listworldspaginator"></a>

## ListWorldsPaginator

Type annotations for
`session.create_client("robomaker").get_paginator("list_worlds")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.paginator import ListWorldsPaginator

session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
    paginator: ListWorldsPaginator = client.get_paginator("list_worlds")
```

Boto3 documentation:
[RoboMaker.Paginator.ListWorlds](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorlds)

Arguments for `ListWorldsPaginator.paginate` method:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWorldsPaginator.paginate` returns
`AsyncIterator`\[[ListWorldsResponseTypeDef](./type_defs.md#listworldsresponsetypedef)\].
