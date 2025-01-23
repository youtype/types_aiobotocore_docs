# Paginators

> [Index](../README.md) > [BedrockRuntime](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#bedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-runtime](https://pypi.org/project/types-aiobotocore-bedrock-runtime/).

## ListAsyncInvokesPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-runtime").get_paginator("list_async_invokes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime/paginator/ListAsyncInvokes.html#BedrockRuntime.Paginator.ListAsyncInvokes)

```python
# ListAsyncInvokesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_runtime.paginator import ListAsyncInvokesPaginator

session = get_session()
async with session.create_client("bedrock-runtime") as client:  # (1)
    paginator: ListAsyncInvokesPaginator = client.get_paginator("list_async_invokes")  # (2)
    async for item in paginator.paginate(...):
        item: ListAsyncInvokesResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockRuntimeClient](./client.md)
2. paginator: [ListAsyncInvokesPaginator](./paginators.md#listasyncinvokespaginator)
3. item: [:material-code-braces: ListAsyncInvokesResponseTypeDef](./type_defs.md#listasyncinvokesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAsyncInvokesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    submitTimeAfter: TimestampTypeDef = ...,
    submitTimeBefore: TimestampTypeDef = ...,
    statusEquals: AsyncInvokeStatusType = ...,  # (1)
    sortBy: SortAsyncInvocationByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListAsyncInvokesResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: AsyncInvokeStatusType](./literals.md#asyncinvokestatustype) 
2. See [:material-code-brackets: SortAsyncInvocationByType](./literals.md#sortasyncinvocationbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListAsyncInvokesResponseTypeDef](./type_defs.md#listasyncinvokesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAsyncInvokesRequestPaginateTypeDef = {  # (1)
    "submitTimeAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAsyncInvokesRequestPaginateTypeDef](./type_defs.md#listasyncinvokesrequestpaginatetypedef) 
