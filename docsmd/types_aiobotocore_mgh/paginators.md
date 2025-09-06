# Paginators

> [Index](../README.md) > [MigrationHub](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MigrationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#migrationhub)
    type annotations stubs module [types-aiobotocore-mgh](https://pypi.org/project/types-aiobotocore-mgh/).

## ListApplicationStatesPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_application_states")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/paginator/ListApplicationStates.html#MigrationHub.Paginator.ListApplicationStates)

```python
# ListApplicationStatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgh.paginator import ListApplicationStatesPaginator

session = get_session()
async with session.create_client("mgh") as client:  # (1)
    paginator: ListApplicationStatesPaginator = client.get_paginator("list_application_states")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationStatesResultTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubClient](./client.md)
2. paginator: [ListApplicationStatesPaginator](./paginators.md#listapplicationstatespaginator)
3. item: `AioPageIterator[ListApplicationStatesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListApplicationStatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApplicationIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListApplicationStatesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListApplicationStatesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationStatesRequestPaginateTypeDef = {  # (1)
    "ApplicationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationStatesRequestPaginateTypeDef](./type_defs.md#listapplicationstatesrequestpaginatetypedef)
## ListCreatedArtifactsPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_created_artifacts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/paginator/ListCreatedArtifacts.html#MigrationHub.Paginator.ListCreatedArtifacts)

```python
# ListCreatedArtifactsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgh.paginator import ListCreatedArtifactsPaginator

session = get_session()
async with session.create_client("mgh") as client:  # (1)
    paginator: ListCreatedArtifactsPaginator = client.get_paginator("list_created_artifacts")  # (2)
    async for item in paginator.paginate(...):
        item: ListCreatedArtifactsResultTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubClient](./client.md)
2. paginator: [ListCreatedArtifactsPaginator](./paginators.md#listcreatedartifactspaginator)
3. item: `AioPageIterator[ListCreatedArtifactsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCreatedArtifactsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCreatedArtifactsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCreatedArtifactsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCreatedArtifactsRequestPaginateTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCreatedArtifactsRequestPaginateTypeDef](./type_defs.md#listcreatedartifactsrequestpaginatetypedef)
## ListDiscoveredResourcesPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_discovered_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/paginator/ListDiscoveredResources.html#MigrationHub.Paginator.ListDiscoveredResources)

```python
# ListDiscoveredResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgh.paginator import ListDiscoveredResourcesPaginator

session = get_session()
async with session.create_client("mgh") as client:  # (1)
    paginator: ListDiscoveredResourcesPaginator = client.get_paginator("list_discovered_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListDiscoveredResourcesResultTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubClient](./client.md)
2. paginator: [ListDiscoveredResourcesPaginator](./paginators.md#listdiscoveredresourcespaginator)
3. item: `AioPageIterator[ListDiscoveredResourcesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDiscoveredResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDiscoveredResourcesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDiscoveredResourcesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDiscoveredResourcesRequestPaginateTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDiscoveredResourcesRequestPaginateTypeDef](./type_defs.md#listdiscoveredresourcesrequestpaginatetypedef)
## ListMigrationTaskUpdatesPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_migration_task_updates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/paginator/ListMigrationTaskUpdates.html#MigrationHub.Paginator.ListMigrationTaskUpdates)

```python
# ListMigrationTaskUpdatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgh.paginator import ListMigrationTaskUpdatesPaginator

session = get_session()
async with session.create_client("mgh") as client:  # (1)
    paginator: ListMigrationTaskUpdatesPaginator = client.get_paginator("list_migration_task_updates")  # (2)
    async for item in paginator.paginate(...):
        item: ListMigrationTaskUpdatesResultTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubClient](./client.md)
2. paginator: [ListMigrationTaskUpdatesPaginator](./paginators.md#listmigrationtaskupdatespaginator)
3. item: `AioPageIterator[ListMigrationTaskUpdatesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMigrationTaskUpdatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListMigrationTaskUpdatesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListMigrationTaskUpdatesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMigrationTaskUpdatesRequestPaginateTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMigrationTaskUpdatesRequestPaginateTypeDef](./type_defs.md#listmigrationtaskupdatesrequestpaginatetypedef)
## ListMigrationTasksPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_migration_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/paginator/ListMigrationTasks.html#MigrationHub.Paginator.ListMigrationTasks)

```python
# ListMigrationTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgh.paginator import ListMigrationTasksPaginator

session = get_session()
async with session.create_client("mgh") as client:  # (1)
    paginator: ListMigrationTasksPaginator = client.get_paginator("list_migration_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListMigrationTasksResultTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubClient](./client.md)
2. paginator: [ListMigrationTasksPaginator](./paginators.md#listmigrationtaskspaginator)
3. item: `AioPageIterator[ListMigrationTasksResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMigrationTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListMigrationTasksResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListMigrationTasksResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMigrationTasksRequestPaginateTypeDef = {  # (1)
    "ResourceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMigrationTasksRequestPaginateTypeDef](./type_defs.md#listmigrationtasksrequestpaginatetypedef)
## ListProgressUpdateStreamsPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_progress_update_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/paginator/ListProgressUpdateStreams.html#MigrationHub.Paginator.ListProgressUpdateStreams)

```python
# ListProgressUpdateStreamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgh.paginator import ListProgressUpdateStreamsPaginator

session = get_session()
async with session.create_client("mgh") as client:  # (1)
    paginator: ListProgressUpdateStreamsPaginator = client.get_paginator("list_progress_update_streams")  # (2)
    async for item in paginator.paginate(...):
        item: ListProgressUpdateStreamsResultTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubClient](./client.md)
2. paginator: [ListProgressUpdateStreamsPaginator](./paginators.md#listprogressupdatestreamspaginator)
3. item: `AioPageIterator[ListProgressUpdateStreamsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProgressUpdateStreamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProgressUpdateStreamsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProgressUpdateStreamsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProgressUpdateStreamsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProgressUpdateStreamsRequestPaginateTypeDef](./type_defs.md#listprogressupdatestreamsrequestpaginatetypedef)
## ListSourceResourcesPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_source_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh/paginator/ListSourceResources.html#MigrationHub.Paginator.ListSourceResources)

```python
# ListSourceResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mgh.paginator import ListSourceResourcesPaginator

session = get_session()
async with session.create_client("mgh") as client:  # (1)
    paginator: ListSourceResourcesPaginator = client.get_paginator("list_source_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListSourceResourcesResultTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubClient](./client.md)
2. paginator: [ListSourceResourcesPaginator](./paginators.md#listsourceresourcespaginator)
3. item: `AioPageIterator[ListSourceResourcesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSourceResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSourceResourcesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSourceResourcesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSourceResourcesRequestPaginateTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSourceResourcesRequestPaginateTypeDef](./type_defs.md#listsourceresourcesrequestpaginatetypedef)
