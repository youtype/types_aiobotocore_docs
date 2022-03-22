<a id="examples-for-aiobotocore-robomaker-module"></a>

# Examples for aiobotocore RoboMaker module

> [Index](../README.md) > [RoboMaker](./README.md) > Examples

- [Examples for aiobotocore RoboMaker module](#examples-for-aiobotocore-robomaker-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[robomaker]` package installed.

Write your `RoboMaker` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type RoboMakerClient
# and provides type checking and code completion
async with session.create_client("robomaker") as client:
    
    # result has type BatchDeleteWorldsResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_delete_worlds()
    

    
    # paginator has type ListDeploymentJobsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_deployment_jobs")
    async for item in paginator.paginate(...):
        # item has type ListDeploymentJobsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[robomaker]` or a standalone
`types_aiobotocore_robomaker` package, you have to explicitly specify
`client: RoboMakerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_robomaker.client import RoboMakerClient
from types_aiobotocore_robomaker.type_defs import BatchDeleteWorldsResponseTypeDef
from types_aiobotocore_robomaker.paginator import ListDeploymentJobsPaginator

from types_aiobotocore_robomaker.literals import PaginatorName



session = get_session()

async with session.create_client("robomaker") as client:
    client: RoboMakerClient

    
    result: BatchDeleteWorldsResponseTypeDef = client.batch_delete_worlds()
    

    
    paginator_name: PaginatorName = "list_deployment_jobs"
    paginator: ListDeploymentJobsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDeploymentJobsResponseTypeDef
        print(item)
    

    
```
