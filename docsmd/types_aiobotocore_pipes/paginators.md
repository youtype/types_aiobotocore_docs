# Paginators

> [Index](../README.md) > [EventBridgePipes](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EventBridgePipes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
    type annotations stubs module [types-aiobotocore-pipes](https://pypi.org/project/types-aiobotocore-pipes/).

## ListPipesPaginator

Type annotations and code completion for `#!python session.create_client("pipes").get_paginator("list_pipes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Paginator.ListPipes)

```python
# ListPipesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pipes.paginator import ListPipesPaginator

session = get_session()
async with session.create_client("pipes") as client:  # (1)
    paginator: ListPipesPaginator = client.get_paginator("list_pipes")  # (2)
    async for item in paginator.paginate(...):
        item: ListPipesResponseTypeDef
        print(item)  # (3)
```

1. client: [EventBridgePipesClient](./client.md)
2. paginator: [ListPipesPaginator](./paginators.md#listpipespaginator)
3. item: [:material-code-braces: ListPipesResponseTypeDef](./type_defs.md#listpipesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPipesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CurrentState: PipeStateType = ...,  # (1)
    DesiredState: RequestedPipeStateType = ...,  # (2)
    NamePrefix: str = ...,
    SourcePrefix: str = ...,
    TargetPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListPipesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: PipeStateType](./literals.md#pipestatetype) 
2. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListPipesResponseTypeDef](./type_defs.md#listpipesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPipesRequestListPipesPaginateTypeDef = {  # (1)
    "CurrentState": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipesRequestListPipesPaginateTypeDef](./type_defs.md#listpipesrequestlistpipespaginatetypedef) 
