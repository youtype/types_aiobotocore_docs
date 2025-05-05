# Paginators

> [Index](../README.md) > [Imagebuilder](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Imagebuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
    type annotations stubs module [types-aiobotocore-imagebuilder](https://pypi.org/project/types-aiobotocore-imagebuilder/).

## ListLifecycleExecutionResourcesPaginator

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_paginator("list_lifecycle_execution_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/paginator/ListLifecycleExecutionResources.html#Imagebuilder.Paginator.ListLifecycleExecutionResources)

```python
# ListLifecycleExecutionResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_imagebuilder.paginator import ListLifecycleExecutionResourcesPaginator

session = get_session()
async with session.create_client("imagebuilder") as client:  # (1)
    paginator: ListLifecycleExecutionResourcesPaginator = client.get_paginator("list_lifecycle_execution_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListLifecycleExecutionResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [ImagebuilderClient](./client.md)
2. paginator: [ListLifecycleExecutionResourcesPaginator](./paginators.md#listlifecycleexecutionresourcespaginator)
3. item: `AioPageIterator[ListLifecycleExecutionResourcesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLifecycleExecutionResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    lifecycleExecutionId: str,
    parentResourceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListLifecycleExecutionResourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListLifecycleExecutionResourcesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLifecycleExecutionResourcesRequestPaginateTypeDef = {  # (1)
    "lifecycleExecutionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLifecycleExecutionResourcesRequestPaginateTypeDef](./type_defs.md#listlifecycleexecutionresourcesrequestpaginatetypedef)
## ListLifecycleExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_paginator("list_lifecycle_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/paginator/ListLifecycleExecutions.html#Imagebuilder.Paginator.ListLifecycleExecutions)

```python
# ListLifecycleExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_imagebuilder.paginator import ListLifecycleExecutionsPaginator

session = get_session()
async with session.create_client("imagebuilder") as client:  # (1)
    paginator: ListLifecycleExecutionsPaginator = client.get_paginator("list_lifecycle_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLifecycleExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ImagebuilderClient](./client.md)
2. paginator: [ListLifecycleExecutionsPaginator](./paginators.md#listlifecycleexecutionspaginator)
3. item: `AioPageIterator[ListLifecycleExecutionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLifecycleExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListLifecycleExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListLifecycleExecutionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLifecycleExecutionsRequestPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLifecycleExecutionsRequestPaginateTypeDef](./type_defs.md#listlifecycleexecutionsrequestpaginatetypedef)
## ListLifecyclePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_paginator("list_lifecycle_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/paginator/ListLifecyclePolicies.html#Imagebuilder.Paginator.ListLifecyclePolicies)

```python
# ListLifecyclePoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_imagebuilder.paginator import ListLifecyclePoliciesPaginator

session = get_session()
async with session.create_client("imagebuilder") as client:  # (1)
    paginator: ListLifecyclePoliciesPaginator = client.get_paginator("list_lifecycle_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListLifecyclePoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [ImagebuilderClient](./client.md)
2. paginator: [ListLifecyclePoliciesPaginator](./paginators.md#listlifecyclepoliciespaginator)
3. item: `AioPageIterator[ListLifecyclePoliciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLifecyclePoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListLifecyclePoliciesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListLifecyclePoliciesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLifecyclePoliciesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLifecyclePoliciesRequestPaginateTypeDef](./type_defs.md#listlifecyclepoliciesrequestpaginatetypedef)
## ListWaitingWorkflowStepsPaginator

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_paginator("list_waiting_workflow_steps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/paginator/ListWaitingWorkflowSteps.html#Imagebuilder.Paginator.ListWaitingWorkflowSteps)

```python
# ListWaitingWorkflowStepsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_imagebuilder.paginator import ListWaitingWorkflowStepsPaginator

session = get_session()
async with session.create_client("imagebuilder") as client:  # (1)
    paginator: ListWaitingWorkflowStepsPaginator = client.get_paginator("list_waiting_workflow_steps")  # (2)
    async for item in paginator.paginate(...):
        item: ListWaitingWorkflowStepsResponseTypeDef
        print(item)  # (3)
```

1. client: [ImagebuilderClient](./client.md)
2. paginator: [ListWaitingWorkflowStepsPaginator](./paginators.md#listwaitingworkflowstepspaginator)
3. item: `AioPageIterator[ListWaitingWorkflowStepsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWaitingWorkflowStepsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWaitingWorkflowStepsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWaitingWorkflowStepsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWaitingWorkflowStepsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWaitingWorkflowStepsRequestPaginateTypeDef](./type_defs.md#listwaitingworkflowstepsrequestpaginatetypedef)
## ListWorkflowBuildVersionsPaginator

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_paginator("list_workflow_build_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/paginator/ListWorkflowBuildVersions.html#Imagebuilder.Paginator.ListWorkflowBuildVersions)

```python
# ListWorkflowBuildVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_imagebuilder.paginator import ListWorkflowBuildVersionsPaginator

session = get_session()
async with session.create_client("imagebuilder") as client:  # (1)
    paginator: ListWorkflowBuildVersionsPaginator = client.get_paginator("list_workflow_build_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowBuildVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ImagebuilderClient](./client.md)
2. paginator: [ListWorkflowBuildVersionsPaginator](./paginators.md#listworkflowbuildversionspaginator)
3. item: `AioPageIterator[ListWorkflowBuildVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkflowBuildVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workflowVersionArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListWorkflowBuildVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListWorkflowBuildVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowBuildVersionsRequestPaginateTypeDef = {  # (1)
    "workflowVersionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowBuildVersionsRequestPaginateTypeDef](./type_defs.md#listworkflowbuildversionsrequestpaginatetypedef)
## ListWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_paginator("list_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/paginator/ListWorkflows.html#Imagebuilder.Paginator.ListWorkflows)

```python
# ListWorkflowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_imagebuilder.paginator import ListWorkflowsPaginator

session = get_session()
async with session.create_client("imagebuilder") as client:  # (1)
    paginator: ListWorkflowsPaginator = client.get_paginator("list_workflows")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkflowsResponseTypeDef
        print(item)  # (3)
```

1. client: [ImagebuilderClient](./client.md)
2. paginator: [ListWorkflowsPaginator](./paginators.md#listworkflowspaginator)
3. item: `AioPageIterator[ListWorkflowsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkflowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    owner: OwnershipType = ...,  # (1)
    filters: Sequence[FilterTypeDef] = ...,  # (2)
    byName: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListWorkflowsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype)
2. See `Sequence[FilterTypeDef]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListWorkflowsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowsRequestPaginateTypeDef = {  # (1)
    "owner": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowsRequestPaginateTypeDef](./type_defs.md#listworkflowsrequestpaginatetypedef)
