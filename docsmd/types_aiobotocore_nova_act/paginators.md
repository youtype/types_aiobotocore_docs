# Paginators

> [Index](../README.md) > [NovaActService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [NovaActService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nova-act.html#novaactservice)
    type annotations stubs module [types-aiobotocore-nova-act](https://pypi.org/project/types-aiobotocore-nova-act/).

## ListActsPaginator

Type annotations and code completion for `#!python session.create_client("nova-act").get_paginator("list_acts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nova-act/paginator/ListActs.html#NovaActService.Paginator.ListActs)

```python
# ListActsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_nova_act.paginator import ListActsPaginator

session = get_session()
async with session.create_client("nova-act") as client:  # (1)
    paginator: ListActsPaginator = client.get_paginator("list_acts")  # (2)
    async for item in paginator.paginate(...):
        item: ListActsResponseTypeDef
        print(item)  # (3)
```

1. client: [NovaActServiceClient](./client.md)
2. paginator: [ListActsPaginator](./paginators.md#listactspaginator)
3. item: `AioPageIterator[ListActsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListActsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workflowDefinitionName: str,
    workflowRunId: str = ...,
    sessionId: str = ...,
    sortOrder: SortOrderType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListActsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListActsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListActsRequestPaginateTypeDef = {  # (1)
    "workflowDefinitionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActsRequestPaginateTypeDef](./type_defs.md#listactsrequestpaginatetypedef)
## ListSessionsPaginator

Type annotations and code completion for `#!python session.create_client("nova-act").get_paginator("list_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nova-act/paginator/ListSessions.html#NovaActService.Paginator.ListSessions)

```python
# ListSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_nova_act.paginator import ListSessionsPaginator

session = get_session()
async with session.create_client("nova-act") as client:  # (1)
    paginator: ListSessionsPaginator = client.get_paginator("list_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSessionsResponseTypeDef
        print(item)  # (3)
```

1. client: [NovaActServiceClient](./client.md)
2. paginator: [ListSessionsPaginator](./paginators.md#listsessionspaginator)
3. item: `AioPageIterator[ListSessionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workflowDefinitionName: str,
    workflowRunId: str,
    sortOrder: SortOrderType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListSessionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListSessionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSessionsRequestPaginateTypeDef = {  # (1)
    "workflowDefinitionName": ...,
    "workflowRunId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSessionsRequestPaginateTypeDef](./type_defs.md#listsessionsrequestpaginatetypedef)
## ListWorkflowDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("nova-act").get_paginator("list_workflow_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nova-act/paginator/ListWorkflowDefinitions.html#NovaActService.Paginator.ListWorkflowDefinitions)

```python
# ListWorkflowDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_nova_act.paginator import ListWorkflowDefinitionsPaginator

session = get_session()
async with session.create_client("nova-act") as client:  # (1)
    paginator: ListWorkflowDefinitionsPaginator = client.get_paginator("list_workflow_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [NovaActServiceClient](./client.md)
2. paginator: [ListWorkflowDefinitionsPaginator](./paginators.md#listworkflowdefinitionspaginator)
3. item: `AioPageIterator[ListWorkflowDefinitionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkflowDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sortOrder: SortOrderType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListWorkflowDefinitionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListWorkflowDefinitionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowDefinitionsRequestPaginateTypeDef = {  # (1)
    "sortOrder": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowDefinitionsRequestPaginateTypeDef](./type_defs.md#listworkflowdefinitionsrequestpaginatetypedef)
## ListWorkflowRunsPaginator

Type annotations and code completion for `#!python session.create_client("nova-act").get_paginator("list_workflow_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nova-act/paginator/ListWorkflowRuns.html#NovaActService.Paginator.ListWorkflowRuns)

```python
# ListWorkflowRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_nova_act.paginator import ListWorkflowRunsPaginator

session = get_session()
async with session.create_client("nova-act") as client:  # (1)
    paginator: ListWorkflowRunsPaginator = client.get_paginator("list_workflow_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [NovaActServiceClient](./client.md)
2. paginator: [ListWorkflowRunsPaginator](./paginators.md#listworkflowrunspaginator)
3. item: `AioPageIterator[ListWorkflowRunsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkflowRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workflowDefinitionName: str,
    sortOrder: SortOrderType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListWorkflowRunsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListWorkflowRunsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowRunsRequestPaginateTypeDef = {  # (1)
    "workflowDefinitionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowRunsRequestPaginateTypeDef](./type_defs.md#listworkflowrunsrequestpaginatetypedef)
