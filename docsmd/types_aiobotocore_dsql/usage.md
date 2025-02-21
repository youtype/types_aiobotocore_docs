# Examples

> [Index](../README.md) > [AuroraDSQL](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AuroraDSQL](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#auroradsql)
    type annotations stubs module [types-aiobotocore-dsql](https://pypi.org/project/types-aiobotocore-dsql/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[dsql]` package installed.

Write your `AuroraDSQL` code as usual,
type checking and code completion should work out of the box.



```python
# AuroraDSQLClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dsql") as client:  # (1)
    result = await client.create_cluster()  # (2)
```

1. client: [AuroraDSQLClient](./client.md)
2. result: [:material-code-braces: CreateClusterOutputTypeDef](./type_defs.md#createclusteroutputtypedef) 



```python
# ListClustersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dsql") as client:  # (1)
    paginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AuroraDSQLClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef) 



```python
# ClusterActiveWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dsql") as client:  # (1)
    waiter = client.get_waiter("cluster_active")  # (2)
    await waiter.wait()
```

1. client: [AuroraDSQLClient](./client.md)
2. waiter: [ClusterActiveWaiter](./waiters.md#clusteractivewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[dsql]`
or a standalone `types_aiobotocore_dsql` package, you have to explicitly specify
`client: AuroraDSQLClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AuroraDSQLClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dsql.client import AuroraDSQLClient
from types_aiobotocore_dsql.type_defs import CreateClusterOutputTypeDef
from types_aiobotocore_dsql.type_defs import CreateClusterInputTypeDef


session = get_session()

async with session.create_client("dsql") as client:
    client: AuroraDSQLClient
    kwargs: CreateClusterInputTypeDef = {...}
    result: CreateClusterOutputTypeDef = await client.create_cluster(**kwargs)
```



```python
# ListClustersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dsql.client import AuroraDSQLClient
from types_aiobotocore_dsql.paginator import ListClustersPaginator
from types_aiobotocore_dsql.type_defs import ListClustersOutputTypeDef


session = get_session()

async with session.create_client("dsql") as client:
    client: AuroraDSQLClient
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")
    async for item in paginator.paginate(...):
        item: ListClustersOutputTypeDef
        print(item)
```



```python
# ClusterActiveWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dsql.client import AuroraDSQLClient
from types_aiobotocore_dsql.waiter import ClusterActiveWaiter


session = get_session()

async with session.create_client("dsql") as client:
    client: AuroraDSQLClient
    waiter: ClusterActiveWaiter = client.get_waiter("cluster_active")
    await waiter.wait()
```
