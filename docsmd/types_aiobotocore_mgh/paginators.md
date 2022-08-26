# Paginators

> [Index](../README.md) > [MigrationHub](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MigrationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
    type annotations stubs module [types-aiobotocore-mgh](https://pypi.org/project/types-aiobotocore-mgh/).

## ListApplicationStatesPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_application_states")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListApplicationStates)

```python title="Usage example"
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
3. item: [:material-code-braces: ListApplicationStatesResultTypeDef](./type_defs.md#listapplicationstatesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListApplicationStatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ApplicationIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApplicationStatesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApplicationStatesResultTypeDef](./type_defs.md#listapplicationstatesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListApplicationStatesRequestListApplicationStatesPaginateTypeDef = {  # (1)
    "ApplicationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationStatesRequestListApplicationStatesPaginateTypeDef](./type_defs.md#listapplicationstatesrequestlistapplicationstatespaginatetypedef) 
## ListCreatedArtifactsPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_created_artifacts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListCreatedArtifacts)

```python title="Usage example"
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
3. item: [:material-code-braces: ListCreatedArtifactsResultTypeDef](./type_defs.md#listcreatedartifactsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListCreatedArtifactsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCreatedArtifactsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCreatedArtifactsResultTypeDef](./type_defs.md#listcreatedartifactsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef](./type_defs.md#listcreatedartifactsrequestlistcreatedartifactspaginatetypedef) 
## ListDiscoveredResourcesPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_discovered_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListDiscoveredResources)

```python title="Usage example"
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
3. item: [:material-code-braces: ListDiscoveredResourcesResultTypeDef](./type_defs.md#listdiscoveredresourcesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListDiscoveredResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDiscoveredResourcesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDiscoveredResourcesResultTypeDef](./type_defs.md#listdiscoveredresourcesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = {  # (1)
    "ProgressUpdateStream": ...,
    "MigrationTaskName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef](./type_defs.md#listdiscoveredresourcesrequestlistdiscoveredresourcespaginatetypedef) 
## ListMigrationTasksPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_migration_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListMigrationTasks)

```python title="Usage example"
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
3. item: [:material-code-braces: ListMigrationTasksResultTypeDef](./type_defs.md#listmigrationtasksresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListMigrationTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMigrationTasksResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMigrationTasksResultTypeDef](./type_defs.md#listmigrationtasksresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListMigrationTasksRequestListMigrationTasksPaginateTypeDef = {  # (1)
    "ResourceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMigrationTasksRequestListMigrationTasksPaginateTypeDef](./type_defs.md#listmigrationtasksrequestlistmigrationtaskspaginatetypedef) 
## ListProgressUpdateStreamsPaginator

Type annotations and code completion for `#!python session.create_client("mgh").get_paginator("list_progress_update_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListProgressUpdateStreams)

```python title="Usage example"
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
3. item: [:material-code-braces: ListProgressUpdateStreamsResultTypeDef](./type_defs.md#listprogressupdatestreamsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListProgressUpdateStreamsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProgressUpdateStreamsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProgressUpdateStreamsResultTypeDef](./type_defs.md#listprogressupdatestreamsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef](./type_defs.md#listprogressupdatestreamsrequestlistprogressupdatestreamspaginatetypedef) 
