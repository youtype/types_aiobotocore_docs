# Paginators

> [Index](../README.md) > [AugmentedAIRuntime](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AugmentedAIRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#augmentedairuntime)
    type annotations stubs module [types-aiobotocore-sagemaker-a2i-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime/).

## ListHumanLoopsPaginator

Type annotations and code completion for `#!python session.create_client("sagemaker-a2i-runtime").get_paginator("list_human_loops")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime/paginator/ListHumanLoops.html#AugmentedAIRuntime.Paginator.ListHumanLoops)

```python
# ListHumanLoopsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_a2i_runtime.paginator import ListHumanLoopsPaginator

session = get_session()
async with session.create_client("sagemaker-a2i-runtime") as client:  # (1)
    paginator: ListHumanLoopsPaginator = client.get_paginator("list_human_loops")  # (2)
    async for item in paginator.paginate(...):
        item: ListHumanLoopsResponseTypeDef
        print(item)  # (3)
```

1. client: [AugmentedAIRuntimeClient](./client.md)
2. paginator: [ListHumanLoopsPaginator](./paginators.md#listhumanloopspaginator)
3. item: [:material-code-braces: ListHumanLoopsResponseTypeDef](./type_defs.md#listhumanloopsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHumanLoopsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FlowDefinitionArn: str,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    SortOrder: SortOrderType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListHumanLoopsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListHumanLoopsResponseTypeDef](./type_defs.md#listhumanloopsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHumanLoopsRequestPaginateTypeDef = {  # (1)
    "FlowDefinitionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHumanLoopsRequestPaginateTypeDef](./type_defs.md#listhumanloopsrequestpaginatetypedef) 
