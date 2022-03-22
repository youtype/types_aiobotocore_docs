<a id="examples-for-aiobotocore-emrcontainers-module"></a>

# Examples for aiobotocore EMRContainers module

> [Index](../README.md) > [EMRContainers](./README.md) > Examples

- [Examples for aiobotocore EMRContainers module](#examples-for-aiobotocore-emrcontainers-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[emr-containers]` package installed.

Write your `EMRContainers` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type EMRContainersClient
# and provides type checking and code completion
async with session.create_client("emr-containers") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListJobRunsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_job_runs")
    async for item in paginator.paginate(...):
        # item has type ListJobRunsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[emr-containers]` or a standalone
`types_aiobotocore_emr_containers` package, you have to explicitly specify
`client: EMRContainersClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.client import EMRContainersClient
from types_aiobotocore_emr_containers.type_defs import bool
from types_aiobotocore_emr_containers.paginator import ListJobRunsPaginator

from types_aiobotocore_emr_containers.literals import PaginatorName



session = get_session()

async with session.create_client("emr-containers") as client:
    client: EMRContainersClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_job_runs"
    paginator: ListJobRunsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListJobRunsResponseTypeDef
        print(item)
    

    
```
