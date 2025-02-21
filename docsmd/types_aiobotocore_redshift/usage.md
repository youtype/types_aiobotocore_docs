# Examples

> [Index](../README.md) > [Redshift](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Redshift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#redshift)
    type annotations stubs module [types-aiobotocore-redshift](https://pypi.org/project/types-aiobotocore-redshift/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[redshift]` package installed.

Write your `Redshift` code as usual,
type checking and code completion should work out of the box.



```python
# RedshiftClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("redshift") as client:  # (1)
    result = await client.accept_reserved_node_exchange()  # (2)
```

1. client: [RedshiftClient](./client.md)
2. result: [:material-code-braces: AcceptReservedNodeExchangeOutputMessageTypeDef](./type_defs.md#acceptreservednodeexchangeoutputmessagetypedef) 



```python
# DescribeClusterDbRevisionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("redshift") as client:  # (1)
    paginator = client.get_paginator("describe_cluster_db_revisions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [RedshiftClient](./client.md)
2. paginator: [DescribeClusterDbRevisionsPaginator](./paginators.md#describeclusterdbrevisionspaginator)
3. item: [:material-code-braces: ClusterDbRevisionsMessageTypeDef](./type_defs.md#clusterdbrevisionsmessagetypedef) 



```python
# ClusterAvailableWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("redshift") as client:  # (1)
    waiter = client.get_waiter("cluster_available")  # (2)
    await waiter.wait()
```

1. client: [RedshiftClient](./client.md)
2. waiter: [ClusterAvailableWaiter](./waiters.md#clusteravailablewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[redshift]`
or a standalone `types_aiobotocore_redshift` package, you have to explicitly specify
`client: RedshiftClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# RedshiftClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_redshift.client import RedshiftClient
from types_aiobotocore_redshift.type_defs import AcceptReservedNodeExchangeOutputMessageTypeDef
from types_aiobotocore_redshift.type_defs import AcceptReservedNodeExchangeInputMessageTypeDef


session = get_session()

async with session.create_client("redshift") as client:
    client: RedshiftClient
    kwargs: AcceptReservedNodeExchangeInputMessageTypeDef = {...}
    result: AcceptReservedNodeExchangeOutputMessageTypeDef = await client.accept_reserved_node_exchange(**kwargs)
```



```python
# DescribeClusterDbRevisionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_redshift.client import RedshiftClient
from types_aiobotocore_redshift.paginator import DescribeClusterDbRevisionsPaginator
from types_aiobotocore_redshift.type_defs import ClusterDbRevisionsMessageTypeDef


session = get_session()

async with session.create_client("redshift") as client:
    client: RedshiftClient
    paginator: DescribeClusterDbRevisionsPaginator = client.get_paginator("describe_cluster_db_revisions")
    async for item in paginator.paginate(...):
        item: ClusterDbRevisionsMessageTypeDef
        print(item)
```



```python
# ClusterAvailableWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_redshift.client import RedshiftClient
from types_aiobotocore_redshift.waiter import ClusterAvailableWaiter


session = get_session()

async with session.create_client("redshift") as client:
    client: RedshiftClient
    waiter: ClusterAvailableWaiter = client.get_waiter("cluster_available")
    await waiter.wait()
```
