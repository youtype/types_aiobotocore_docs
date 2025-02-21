# Examples

> [Index](../README.md) > [EventBridgePipes](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EventBridgePipes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#eventbridgepipes)
    type annotations stubs module [types-aiobotocore-pipes](https://pypi.org/project/types-aiobotocore-pipes/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[pipes]` package installed.

Write your `EventBridgePipes` code as usual,
type checking and code completion should work out of the box.



```python
# EventBridgePipesClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pipes") as client:  # (1)
    result = await client.create_pipe()  # (2)
```

1. client: [EventBridgePipesClient](./client.md)
2. result: [:material-code-braces: CreatePipeResponseTypeDef](./type_defs.md#createpiperesponsetypedef) 



```python
# ListPipesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pipes") as client:  # (1)
    paginator = client.get_paginator("list_pipes")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EventBridgePipesClient](./client.md)
2. paginator: [ListPipesPaginator](./paginators.md#listpipespaginator)
3. item: [:material-code-braces: ListPipesResponseTypeDef](./type_defs.md#listpipesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[pipes]`
or a standalone `types_aiobotocore_pipes` package, you have to explicitly specify
`client: EventBridgePipesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EventBridgePipesClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pipes.client import EventBridgePipesClient
from types_aiobotocore_pipes.type_defs import CreatePipeResponseTypeDef
from types_aiobotocore_pipes.type_defs import CreatePipeRequestTypeDef


session = get_session()

async with session.create_client("pipes") as client:
    client: EventBridgePipesClient
    kwargs: CreatePipeRequestTypeDef = {...}
    result: CreatePipeResponseTypeDef = await client.create_pipe(**kwargs)
```



```python
# ListPipesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pipes.client import EventBridgePipesClient
from types_aiobotocore_pipes.paginator import ListPipesPaginator
from types_aiobotocore_pipes.type_defs import ListPipesResponseTypeDef


session = get_session()

async with session.create_client("pipes") as client:
    client: EventBridgePipesClient
    paginator: ListPipesPaginator = client.get_paginator("list_pipes")
    async for item in paginator.paginate(...):
        item: ListPipesResponseTypeDef
        print(item)
```


