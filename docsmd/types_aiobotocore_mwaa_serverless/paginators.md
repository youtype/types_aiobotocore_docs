# Paginators

> [Index](../README.md) > [MWAAServerless](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MWAAServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa-serverless.html#mwaaserverless)
    type annotations stubs module [types-aiobotocore-mwaa-serverless](https://pypi.org/project/types-aiobotocore-mwaa-serverless/).

## ListTaskInstancesPaginator

Type annotations and code completion for `#!python session.create_client("mwaa-serverless").get_paginator("list_task_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa-serverless/paginator/ListTaskInstances.html#MWAAServerless.Paginator.ListTaskInstances)

```python
# ListTaskInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mwaa_serverless.paginator import ListTaskInstancesPaginator

session = get_session()
async with session.create_client("mwaa-serverless") as client:  # (1)
    paginator: ListTaskInstancesPaginator = client.get_paginator("list_task_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListTaskInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [MWAAServerlessClient](./client.md)
2. paginator: [ListTaskInstancesPaginator](./paginators.md#listtaskinstancespaginator)
3. item: `AioPageIterator[ListTaskInstancesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTaskInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    WorkflowArn: str,
    RunId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTaskInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTaskInstancesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTaskInstancesRequestPaginateTypeDef = {  # (1)
    "WorkflowArn": ...,
    "RunId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTaskInstancesRequestPaginateTypeDef](./type_defs.md#listtaskinstancesrequestpaginatetypedef)
## ListWorkflowRunsPaginator

Type annotations and code completion for `#!python session.create_client("mwaa-serverless").get_paginator("list_workflow_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa-serverless/paginator/ListWorkflowRuns.html#MWAAServerless.Paginator.ListWorkflowRuns)

```python
# ListWorkflowRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mwaa_serverless.paginator import ListWorkflowRunsPaginator

session = get_session()
async with session.create_client("mwaa-serverless") as client:  # (1)
    paginator: ListWorkflowRunsPaginator = client.get_paginator("list_workflow_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [MWAAServerlessClient](./client.md)
2. paginator: [ListWorkflowRunsPaginator](./paginators.md#listworkflowrunspaginator)
3. item: `AioPageIterator[ListWorkflowRunsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkflowRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    WorkflowArn: str,
    WorkflowVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWorkflowRunsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWorkflowRunsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowRunsRequestPaginateTypeDef = {  # (1)
    "WorkflowArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowRunsRequestPaginateTypeDef](./type_defs.md#listworkflowrunsrequestpaginatetypedef)
## ListWorkflowVersionsPaginator

Type annotations and code completion for `#!python session.create_client("mwaa-serverless").get_paginator("list_workflow_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa-serverless/paginator/ListWorkflowVersions.html#MWAAServerless.Paginator.ListWorkflowVersions)

```python
# ListWorkflowVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mwaa_serverless.paginator import ListWorkflowVersionsPaginator

session = get_session()
async with session.create_client("mwaa-serverless") as client:  # (1)
    paginator: ListWorkflowVersionsPaginator = client.get_paginator("list_workflow_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MWAAServerlessClient](./client.md)
2. paginator: [ListWorkflowVersionsPaginator](./paginators.md#listworkflowversionspaginator)
3. item: `AioPageIterator[ListWorkflowVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkflowVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    WorkflowArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWorkflowVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWorkflowVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowVersionsRequestPaginateTypeDef = {  # (1)
    "WorkflowArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowVersionsRequestPaginateTypeDef](./type_defs.md#listworkflowversionsrequestpaginatetypedef)
## ListWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("mwaa-serverless").get_paginator("list_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa-serverless/paginator/ListWorkflows.html#MWAAServerless.Paginator.ListWorkflows)

```python
# ListWorkflowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mwaa_serverless.paginator import ListWorkflowsPaginator

session = get_session()
async with session.create_client("mwaa-serverless") as client:  # (1)
    paginator: ListWorkflowsPaginator = client.get_paginator("list_workflows")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowsResponseTypeDef
        print(item)  # (3)
```

1. client: [MWAAServerlessClient](./client.md)
2. paginator: [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)
3. item: `AioPageIterator[ListWorkflowsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkflowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWorkflowsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWorkflowsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowsRequestPaginateTypeDef](./type_defs.md#listworkflowsrequestpaginatetypedef)
