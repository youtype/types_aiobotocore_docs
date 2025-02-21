# Paginators

> [Index](../README.md) > [CodeCatalyst](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeCatalyst](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#codecatalyst)
    type annotations stubs module [types-aiobotocore-codecatalyst](https://pypi.org/project/types-aiobotocore-codecatalyst/).

## ListAccessTokensPaginator

Type annotations and code completion for `#!python session.create_client("codecatalyst").get_paginator("list_access_tokens")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst/paginator/ListAccessTokens.html#CodeCatalyst.Paginator.ListAccessTokens)

```python
# ListAccessTokensPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.paginator import ListAccessTokensPaginator

session = get_session()
async with session.create_client("codecatalyst") as client:  # (1)
    paginator: ListAccessTokensPaginator = client.get_paginator("list_access_tokens")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessTokensResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListAccessTokensPaginator](./paginators.md#listaccesstokenspaginator)
3. item: [:material-code-braces: ListAccessTokensResponseTypeDef](./type_defs.md#listaccesstokensresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccessTokensPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAccessTokensResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccessTokensResponseTypeDef](./type_defs.md#listaccesstokensresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessTokensRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessTokensRequestPaginateTypeDef](./type_defs.md#listaccesstokensrequestpaginatetypedef) 
## ListDevEnvironmentSessionsPaginator

Type annotations and code completion for `#!python session.create_client("codecatalyst").get_paginator("list_dev_environment_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst/paginator/ListDevEnvironmentSessions.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions)

```python
# ListDevEnvironmentSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.paginator import ListDevEnvironmentSessionsPaginator

session = get_session()
async with session.create_client("codecatalyst") as client:  # (1)
    paginator: ListDevEnvironmentSessionsPaginator = client.get_paginator("list_dev_environment_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevEnvironmentSessionsResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListDevEnvironmentSessionsPaginator](./paginators.md#listdevenvironmentsessionspaginator)
3. item: [:material-code-braces: ListDevEnvironmentSessionsResponseTypeDef](./type_defs.md#listdevenvironmentsessionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDevEnvironmentSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    spaceName: str,
    projectName: str,
    devEnvironmentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDevEnvironmentSessionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDevEnvironmentSessionsResponseTypeDef](./type_defs.md#listdevenvironmentsessionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDevEnvironmentSessionsRequestPaginateTypeDef = {  # (1)
    "spaceName": ...,
    "projectName": ...,
    "devEnvironmentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevEnvironmentSessionsRequestPaginateTypeDef](./type_defs.md#listdevenvironmentsessionsrequestpaginatetypedef) 
## ListDevEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("codecatalyst").get_paginator("list_dev_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst/paginator/ListDevEnvironments.html#CodeCatalyst.Paginator.ListDevEnvironments)

```python
# ListDevEnvironmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.paginator import ListDevEnvironmentsPaginator

session = get_session()
async with session.create_client("codecatalyst") as client:  # (1)
    paginator: ListDevEnvironmentsPaginator = client.get_paginator("list_dev_environments")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListDevEnvironmentsPaginator](./paginators.md#listdevenvironmentspaginator)
3. item: [:material-code-braces: ListDevEnvironmentsResponseTypeDef](./type_defs.md#listdevenvironmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDevEnvironmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    spaceName: str,
    projectName: str = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDevEnvironmentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDevEnvironmentsResponseTypeDef](./type_defs.md#listdevenvironmentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDevEnvironmentsRequestPaginateTypeDef = {  # (1)
    "spaceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevEnvironmentsRequestPaginateTypeDef](./type_defs.md#listdevenvironmentsrequestpaginatetypedef) 
## ListEventLogsPaginator

Type annotations and code completion for `#!python session.create_client("codecatalyst").get_paginator("list_event_logs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst/paginator/ListEventLogs.html#CodeCatalyst.Paginator.ListEventLogs)

```python
# ListEventLogsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.paginator import ListEventLogsPaginator

session = get_session()
async with session.create_client("codecatalyst") as client:  # (1)
    paginator: ListEventLogsPaginator = client.get_paginator("list_event_logs")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventLogsResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListEventLogsPaginator](./paginators.md#listeventlogspaginator)
3. item: [:material-code-braces: ListEventLogsResponseTypeDef](./type_defs.md#listeventlogsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventLogsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    spaceName: str,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    eventName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEventLogsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventLogsResponseTypeDef](./type_defs.md#listeventlogsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventLogsRequestPaginateTypeDef = {  # (1)
    "spaceName": ...,
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventLogsRequestPaginateTypeDef](./type_defs.md#listeventlogsrequestpaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.create_client("codecatalyst").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst/paginator/ListProjects.html#CodeCatalyst.Paginator.ListProjects)

```python
# ListProjectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("codecatalyst") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    spaceName: str,
    filters: Sequence[ProjectListFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListProjectsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ProjectListFilterTypeDef](./type_defs.md#projectlistfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectsRequestPaginateTypeDef = {  # (1)
    "spaceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestPaginateTypeDef](./type_defs.md#listprojectsrequestpaginatetypedef) 
## ListSourceRepositoriesPaginator

Type annotations and code completion for `#!python session.create_client("codecatalyst").get_paginator("list_source_repositories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst/paginator/ListSourceRepositories.html#CodeCatalyst.Paginator.ListSourceRepositories)

```python
# ListSourceRepositoriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.paginator import ListSourceRepositoriesPaginator

session = get_session()
async with session.create_client("codecatalyst") as client:  # (1)
    paginator: ListSourceRepositoriesPaginator = client.get_paginator("list_source_repositories")  # (2)
    async for item in paginator.paginate(...):
        item: ListSourceRepositoriesResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListSourceRepositoriesPaginator](./paginators.md#listsourcerepositoriespaginator)
3. item: [:material-code-braces: ListSourceRepositoriesResponseTypeDef](./type_defs.md#listsourcerepositoriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSourceRepositoriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    spaceName: str,
    projectName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSourceRepositoriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSourceRepositoriesResponseTypeDef](./type_defs.md#listsourcerepositoriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSourceRepositoriesRequestPaginateTypeDef = {  # (1)
    "spaceName": ...,
    "projectName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSourceRepositoriesRequestPaginateTypeDef](./type_defs.md#listsourcerepositoriesrequestpaginatetypedef) 
## ListSourceRepositoryBranchesPaginator

Type annotations and code completion for `#!python session.create_client("codecatalyst").get_paginator("list_source_repository_branches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst/paginator/ListSourceRepositoryBranches.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches)

```python
# ListSourceRepositoryBranchesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.paginator import ListSourceRepositoryBranchesPaginator

session = get_session()
async with session.create_client("codecatalyst") as client:  # (1)
    paginator: ListSourceRepositoryBranchesPaginator = client.get_paginator("list_source_repository_branches")  # (2)
    async for item in paginator.paginate(...):
        item: ListSourceRepositoryBranchesResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListSourceRepositoryBranchesPaginator](./paginators.md#listsourcerepositorybranchespaginator)
3. item: [:material-code-braces: ListSourceRepositoryBranchesResponseTypeDef](./type_defs.md#listsourcerepositorybranchesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSourceRepositoryBranchesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    spaceName: str,
    projectName: str,
    sourceRepositoryName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSourceRepositoryBranchesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSourceRepositoryBranchesResponseTypeDef](./type_defs.md#listsourcerepositorybranchesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSourceRepositoryBranchesRequestPaginateTypeDef = {  # (1)
    "spaceName": ...,
    "projectName": ...,
    "sourceRepositoryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSourceRepositoryBranchesRequestPaginateTypeDef](./type_defs.md#listsourcerepositorybranchesrequestpaginatetypedef) 
## ListSpacesPaginator

Type annotations and code completion for `#!python session.create_client("codecatalyst").get_paginator("list_spaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst/paginator/ListSpaces.html#CodeCatalyst.Paginator.ListSpaces)

```python
# ListSpacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.paginator import ListSpacesPaginator

session = get_session()
async with session.create_client("codecatalyst") as client:  # (1)
    paginator: ListSpacesPaginator = client.get_paginator("list_spaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListSpacesResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListSpacesPaginator](./paginators.md#listspacespaginator)
3. item: [:material-code-braces: ListSpacesResponseTypeDef](./type_defs.md#listspacesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSpacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSpacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSpacesResponseTypeDef](./type_defs.md#listspacesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSpacesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSpacesRequestPaginateTypeDef](./type_defs.md#listspacesrequestpaginatetypedef) 
## ListWorkflowRunsPaginator

Type annotations and code completion for `#!python session.create_client("codecatalyst").get_paginator("list_workflow_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst/paginator/ListWorkflowRuns.html#CodeCatalyst.Paginator.ListWorkflowRuns)

```python
# ListWorkflowRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.paginator import ListWorkflowRunsPaginator

session = get_session()
async with session.create_client("codecatalyst") as client:  # (1)
    paginator: ListWorkflowRunsPaginator = client.get_paginator("list_workflow_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListWorkflowRunsPaginator](./paginators.md#listworkflowrunspaginator)
3. item: [:material-code-braces: ListWorkflowRunsResponseTypeDef](./type_defs.md#listworkflowrunsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkflowRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    spaceName: str,
    projectName: str,
    workflowId: str = ...,
    sortBy: Sequence[Mapping[str, Any]] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkflowRunsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkflowRunsResponseTypeDef](./type_defs.md#listworkflowrunsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowRunsRequestPaginateTypeDef = {  # (1)
    "spaceName": ...,
    "projectName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowRunsRequestPaginateTypeDef](./type_defs.md#listworkflowrunsrequestpaginatetypedef) 
## ListWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("codecatalyst").get_paginator("list_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst/paginator/ListWorkflows.html#CodeCatalyst.Paginator.ListWorkflows)

```python
# ListWorkflowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.paginator import ListWorkflowsPaginator

session = get_session()
async with session.create_client("codecatalyst") as client:  # (1)
    paginator: ListWorkflowsPaginator = client.get_paginator("list_workflows")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowsResponseTypeDef
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)
3. item: [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkflowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    spaceName: str,
    projectName: str,
    sortBy: Sequence[Mapping[str, Any]] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkflowsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowsRequestPaginateTypeDef = {  # (1)
    "spaceName": ...,
    "projectName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowsRequestPaginateTypeDef](./type_defs.md#listworkflowsrequestpaginatetypedef) 
