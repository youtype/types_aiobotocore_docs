# Paginators

> [Index](../README.md) > [DevOpsAgentService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DevOpsAgentService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent.html#devopsagentservice)
    type annotations stubs module [types-aiobotocore-devops-agent](https://pypi.org/project/types-aiobotocore-devops-agent/).

## ListAgentSpacesPaginator

Type annotations and code completion for `#!python session.create_client("devops-agent").get_paginator("list_agent_spaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/paginator/ListAgentSpaces.html#DevOpsAgentService.Paginator.ListAgentSpaces)

```python
# ListAgentSpacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devops_agent.paginator import ListAgentSpacesPaginator

session = get_session()
async with session.create_client("devops-agent") as client:  # (1)
    paginator: ListAgentSpacesPaginator = client.get_paginator("list_agent_spaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgentSpacesOutputTypeDef
        print(item)  # (3)
```

1. client: [DevOpsAgentServiceClient](./client.md)
2. paginator: [ListAgentSpacesPaginator](./paginators.md#listagentspacespaginator)
3. item: `AioPageIterator[ListAgentSpacesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAgentSpacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAgentSpacesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAgentSpacesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAgentSpacesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgentSpacesInputPaginateTypeDef](./type_defs.md#listagentspacesinputpaginatetypedef)
## ListAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("devops-agent").get_paginator("list_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/paginator/ListAssociations.html#DevOpsAgentService.Paginator.ListAssociations)

```python
# ListAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devops_agent.paginator import ListAssociationsPaginator

session = get_session()
async with session.create_client("devops-agent") as client:  # (1)
    paginator: ListAssociationsPaginator = client.get_paginator("list_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociationsOutputTypeDef
        print(item)  # (3)
```

1. client: [DevOpsAgentServiceClient](./client.md)
2. paginator: [ListAssociationsPaginator](./paginators.md#listassociationspaginator)
3. item: `AioPageIterator[ListAssociationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentSpaceId: str,
    filterServiceTypes: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAssociationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAssociationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAssociationsInputPaginateTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociationsInputPaginateTypeDef](./type_defs.md#listassociationsinputpaginatetypedef)
## ListBacklogTasksPaginator

Type annotations and code completion for `#!python session.create_client("devops-agent").get_paginator("list_backlog_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/paginator/ListBacklogTasks.html#DevOpsAgentService.Paginator.ListBacklogTasks)

```python
# ListBacklogTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devops_agent.paginator import ListBacklogTasksPaginator

session = get_session()
async with session.create_client("devops-agent") as client:  # (1)
    paginator: ListBacklogTasksPaginator = client.get_paginator("list_backlog_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListBacklogTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsAgentServiceClient](./client.md)
2. paginator: [ListBacklogTasksPaginator](./paginators.md#listbacklogtaskspaginator)
3. item: `AioPageIterator[ListBacklogTasksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBacklogTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentSpaceId: str,
    filter: TaskFilterTypeDef = ...,  # (1)
    sortField: TaskSortFieldType = ...,  # (2)
    order: TaskSortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListBacklogTasksResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: TaskFilterTypeDef](./type_defs.md#taskfiltertypedef)
2. See [:material-code-brackets: TaskSortFieldType](./literals.md#tasksortfieldtype)
3. See [:material-code-brackets: TaskSortOrderType](./literals.md#tasksortordertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListBacklogTasksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBacklogTasksRequestPaginateTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBacklogTasksRequestPaginateTypeDef](./type_defs.md#listbacklogtasksrequestpaginatetypedef)
## ListExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("devops-agent").get_paginator("list_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/paginator/ListExecutions.html#DevOpsAgentService.Paginator.ListExecutions)

```python
# ListExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devops_agent.paginator import ListExecutionsPaginator

session = get_session()
async with session.create_client("devops-agent") as client:  # (1)
    paginator: ListExecutionsPaginator = client.get_paginator("list_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsAgentServiceClient](./client.md)
2. paginator: [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
3. item: `AioPageIterator[ListExecutionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentSpaceId: str,
    taskId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListExecutionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListExecutionsRequestPaginateTypeDef = {  # (1)
    "agentSpaceId": ...,
    "taskId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExecutionsRequestPaginateTypeDef](./type_defs.md#listexecutionsrequestpaginatetypedef)
## ListGoalsPaginator

Type annotations and code completion for `#!python session.create_client("devops-agent").get_paginator("list_goals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/paginator/ListGoals.html#DevOpsAgentService.Paginator.ListGoals)

```python
# ListGoalsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devops_agent.paginator import ListGoalsPaginator

session = get_session()
async with session.create_client("devops-agent") as client:  # (1)
    paginator: ListGoalsPaginator = client.get_paginator("list_goals")  # (2)
    async for item in paginator.paginate(...):
        item: ListGoalsResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsAgentServiceClient](./client.md)
2. paginator: [ListGoalsPaginator](./paginators.md#listgoalspaginator)
3. item: `AioPageIterator[ListGoalsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGoalsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentSpaceId: str,
    status: GoalStatusType = ...,  # (1)
    goalType: GoalTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListGoalsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: GoalStatusType](./literals.md#goalstatustype)
2. See [:material-code-brackets: GoalTypeType](./literals.md#goaltypetype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListGoalsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGoalsRequestPaginateTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGoalsRequestPaginateTypeDef](./type_defs.md#listgoalsrequestpaginatetypedef)
## ListJournalRecordsPaginator

Type annotations and code completion for `#!python session.create_client("devops-agent").get_paginator("list_journal_records")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/paginator/ListJournalRecords.html#DevOpsAgentService.Paginator.ListJournalRecords)

```python
# ListJournalRecordsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devops_agent.paginator import ListJournalRecordsPaginator

session = get_session()
async with session.create_client("devops-agent") as client:  # (1)
    paginator: ListJournalRecordsPaginator = client.get_paginator("list_journal_records")  # (2)
    async for item in paginator.paginate(...):
        item: ListJournalRecordsResponseTypeDef
        print(item)  # (3)
```

1. client: [DevOpsAgentServiceClient](./client.md)
2. paginator: [ListJournalRecordsPaginator](./paginators.md#listjournalrecordspaginator)
3. item: `AioPageIterator[ListJournalRecordsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListJournalRecordsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentSpaceId: str,
    executionId: str,
    recordType: str = ...,
    order: OrderTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListJournalRecordsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OrderTypeType](./literals.md#ordertypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListJournalRecordsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListJournalRecordsRequestPaginateTypeDef = {  # (1)
    "agentSpaceId": ...,
    "executionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJournalRecordsRequestPaginateTypeDef](./type_defs.md#listjournalrecordsrequestpaginatetypedef)
## ListServicesPaginator

Type annotations and code completion for `#!python session.create_client("devops-agent").get_paginator("list_services")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/paginator/ListServices.html#DevOpsAgentService.Paginator.ListServices)

```python
# ListServicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_devops_agent.paginator import ListServicesPaginator

session = get_session()
async with session.create_client("devops-agent") as client:  # (1)
    paginator: ListServicesPaginator = client.get_paginator("list_services")  # (2)
    async for item in paginator.paginate(...):
        item: ListServicesOutputTypeDef
        print(item)  # (3)
```

1. client: [DevOpsAgentServiceClient](./client.md)
2. paginator: [ListServicesPaginator](./paginators.md#listservicespaginator)
3. item: `AioPageIterator[ListServicesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListServicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filterServiceType: ServiceType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListServicesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceType](./literals.md#servicetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListServicesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListServicesInputPaginateTypeDef = {  # (1)
    "filterServiceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServicesInputPaginateTypeDef](./type_defs.md#listservicesinputpaginatetypedef)
