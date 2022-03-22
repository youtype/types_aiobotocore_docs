<a id="examples-for-aiobotocore-redshift-module"></a>

# Examples for aiobotocore Redshift module

> [Index](../README.md) > [Redshift](./README.md) > Examples

- [Examples for aiobotocore Redshift module](#examples-for-aiobotocore-redshift-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[redshift]` package installed.

Write your `Redshift` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type RedshiftClient
# and provides type checking and code completion
async with session.create_client("redshift") as client:
    
    # result has type AcceptReservedNodeExchangeOutputMessageTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_reserved_node_exchange()
    

    
    # paginator has type DescribeClusterDbRevisionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_cluster_db_revisions")
    async for item in paginator.paginate(...):
        # item has type ClusterDbRevisionsMessageTypeDef
        print(item)
    

    
    # waiter has type ClusterAvailableWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("cluster_available")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[redshift]` or a standalone
`types_aiobotocore_redshift` package, you have to explicitly specify
`client: RedshiftClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_redshift.client import RedshiftClient
from types_aiobotocore_redshift.type_defs import AcceptReservedNodeExchangeOutputMessageTypeDef
from types_aiobotocore_redshift.paginator import DescribeClusterDbRevisionsPaginator
from types_aiobotocore_redshift.waiter import ClusterAvailableWaiter
from types_aiobotocore_redshift.literals import PaginatorName
from types_aiobotocore_redshift.literals import WaiterName


session = get_session()

async with session.create_client("redshift") as client:
    client: RedshiftClient

    
    result: AcceptReservedNodeExchangeOutputMessageTypeDef = client.accept_reserved_node_exchange()
    

    
    paginator_name: PaginatorName = "describe_cluster_db_revisions"
    paginator: DescribeClusterDbRevisionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ClusterDbRevisionsMessageTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "cluster_available"
    waiter: ClusterAvailableWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
