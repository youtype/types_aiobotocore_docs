# Paginators

> [Index](../README.md) > [EntityResolution](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## ListMatchingJobsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_matching_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListMatchingJobs)

```python
# ListMatchingJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.paginator import ListMatchingJobsPaginator

session = get_session()
async with session.create_client("entityresolution") as client:  # (1)
    paginator: ListMatchingJobsPaginator = client.get_paginator("list_matching_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListMatchingJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListMatchingJobsPaginator](./paginators.md#listmatchingjobspaginator)
3. item: [:material-code-braces: ListMatchingJobsOutputTypeDef](./type_defs.md#listmatchingjobsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListMatchingJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workflowName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMatchingJobsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMatchingJobsOutputTypeDef](./type_defs.md#listmatchingjobsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMatchingJobsInputListMatchingJobsPaginateTypeDef = {  # (1)
    "workflowName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMatchingJobsInputListMatchingJobsPaginateTypeDef](./type_defs.md#listmatchingjobsinputlistmatchingjobspaginatetypedef) 
## ListMatchingWorkflowsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_matching_workflows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListMatchingWorkflows)

```python
# ListMatchingWorkflowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.paginator import ListMatchingWorkflowsPaginator

session = get_session()
async with session.create_client("entityresolution") as client:  # (1)
    paginator: ListMatchingWorkflowsPaginator = client.get_paginator("list_matching_workflows")  # (2)
    async for item in paginator.paginate(...):
        item: ListMatchingWorkflowsOutputTypeDef
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListMatchingWorkflowsPaginator](./paginators.md#listmatchingworkflowspaginator)
3. item: [:material-code-braces: ListMatchingWorkflowsOutputTypeDef](./type_defs.md#listmatchingworkflowsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListMatchingWorkflowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMatchingWorkflowsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMatchingWorkflowsOutputTypeDef](./type_defs.md#listmatchingworkflowsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef](./type_defs.md#listmatchingworkflowsinputlistmatchingworkflowspaginatetypedef) 
## ListSchemaMappingsPaginator

Type annotations and code completion for `#!python session.create_client("entityresolution").get_paginator("list_schema_mappings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Paginator.ListSchemaMappings)

```python
# ListSchemaMappingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.paginator import ListSchemaMappingsPaginator

session = get_session()
async with session.create_client("entityresolution") as client:  # (1)
    paginator: ListSchemaMappingsPaginator = client.get_paginator("list_schema_mappings")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemaMappingsOutputTypeDef
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListSchemaMappingsPaginator](./paginators.md#listschemamappingspaginator)
3. item: [:material-code-braces: ListSchemaMappingsOutputTypeDef](./type_defs.md#listschemamappingsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemaMappingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSchemaMappingsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemaMappingsOutputTypeDef](./type_defs.md#listschemamappingsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef](./type_defs.md#listschemamappingsinputlistschemamappingspaginatetypedef) 
