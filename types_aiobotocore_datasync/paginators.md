<a id="paginators-for-aiobotocore-datasync-module"></a>

# Paginators for aiobotocore DataSync module

> [Index](..) > [DataSync](.) > Paginators

Auto-generated documentation for
[DataSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
type annotations stubs module
[types-aiobotocore-datasync](https://pypi.org/project/types-aiobotocore-datasync/).

- [Paginators for aiobotocore DataSync module](#paginators-for-aiobotocore-datasync-module)
  - [ListAgentsPaginator](#listagentspaginator)
  - [ListLocationsPaginator](#listlocationspaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)
  - [ListTaskExecutionsPaginator](#listtaskexecutionspaginator)
  - [ListTasksPaginator](#listtaskspaginator)

<a id="listagentspaginator"></a>

## ListAgentsPaginator

Type annotations for
`session.create_client("datasync").get_paginator("list_agents")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_datasync.paginator import ListAgentsPaginator

session = get_session()
async with session.create_client("datasync") as client:
    client: DataSyncClient
    paginator: ListAgentsPaginator = client.get_paginator("list_agents")
```

Boto3 documentation:
[DataSync.Paginator.ListAgents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListAgents)

Arguments for `ListAgentsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAgentsPaginator.paginate` returns
`AsyncIterable`\[[ListAgentsResponseTypeDef](./type_defs.md#listagentsresponsetypedef)\].

<a id="listlocationspaginator"></a>

## ListLocationsPaginator

Type annotations for
`session.create_client("datasync").get_paginator("list_locations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_datasync.paginator import ListLocationsPaginator

session = get_session()
async with session.create_client("datasync") as client:
    client: DataSyncClient
    paginator: ListLocationsPaginator = client.get_paginator("list_locations")
```

Boto3 documentation:
[DataSync.Paginator.ListLocations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListLocations)

Arguments for `ListLocationsPaginator.paginate` method:

- `Filters`:
  `Sequence`\[[LocationFilterTypeDef](./type_defs.md#locationfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListLocationsPaginator.paginate` returns
`AsyncIterable`\[[ListLocationsResponseTypeDef](./type_defs.md#listlocationsresponsetypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("datasync").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_datasync.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("datasync") as client:
    client: DataSyncClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[DataSync.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `ResourceArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterable`\[[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)\].

<a id="listtaskexecutionspaginator"></a>

## ListTaskExecutionsPaginator

Type annotations for
`session.create_client("datasync").get_paginator("list_task_executions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_datasync.paginator import ListTaskExecutionsPaginator

session = get_session()
async with session.create_client("datasync") as client:
    client: DataSyncClient
    paginator: ListTaskExecutionsPaginator = client.get_paginator("list_task_executions")
```

Boto3 documentation:
[DataSync.Paginator.ListTaskExecutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTaskExecutions)

Arguments for `ListTaskExecutionsPaginator.paginate` method:

- `TaskArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTaskExecutionsPaginator.paginate` returns
`AsyncIterable`\[[ListTaskExecutionsResponseTypeDef](./type_defs.md#listtaskexecutionsresponsetypedef)\].

<a id="listtaskspaginator"></a>

## ListTasksPaginator

Type annotations for
`session.create_client("datasync").get_paginator("list_tasks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_datasync.paginator import ListTasksPaginator

session = get_session()
async with session.create_client("datasync") as client:
    client: DataSyncClient
    paginator: ListTasksPaginator = client.get_paginator("list_tasks")
```

Boto3 documentation:
[DataSync.Paginator.ListTasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTasks)

Arguments for `ListTasksPaginator.paginate` method:

- `Filters`:
  `Sequence`\[[TaskFilterTypeDef](./type_defs.md#taskfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTasksPaginator.paginate` returns
`AsyncIterable`\[[ListTasksResponseTypeDef](./type_defs.md#listtasksresponsetypedef)\].
