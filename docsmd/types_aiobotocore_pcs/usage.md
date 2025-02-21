# Examples

> [Index](../README.md) > [ParallelComputingService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ParallelComputingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#parallelcomputingservice)
    type annotations stubs module [types-aiobotocore-pcs](https://pypi.org/project/types-aiobotocore-pcs/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[pcs]` package installed.

Write your `ParallelComputingService` code as usual,
type checking and code completion should work out of the box.



```python
# ParallelComputingServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pcs") as client:  # (1)
    result = await client.create_cluster()  # (2)
```

1. client: [ParallelComputingServiceClient](./client.md)
2. result: [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef) 



```python
# ListClustersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pcs") as client:  # (1)
    paginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ParallelComputingServiceClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[pcs]`
or a standalone `types_aiobotocore_pcs` package, you have to explicitly specify
`client: ParallelComputingServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ParallelComputingServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pcs.client import ParallelComputingServiceClient
from types_aiobotocore_pcs.type_defs import CreateClusterResponseTypeDef
from types_aiobotocore_pcs.type_defs import CreateClusterRequestTypeDef


session = get_session()

async with session.create_client("pcs") as client:
    client: ParallelComputingServiceClient
    kwargs: CreateClusterRequestTypeDef = {...}
    result: CreateClusterResponseTypeDef = await client.create_cluster(**kwargs)
```



```python
# ListClustersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pcs.client import ParallelComputingServiceClient
from types_aiobotocore_pcs.paginator import ListClustersPaginator
from types_aiobotocore_pcs.type_defs import ListClustersResponseTypeDef


session = get_session()

async with session.create_client("pcs") as client:
    client: ParallelComputingServiceClient
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")
    async for item in paginator.paginate(...):
        item: ListClustersResponseTypeDef
        print(item)
```


