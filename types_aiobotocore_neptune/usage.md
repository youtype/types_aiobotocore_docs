<a id="examples-for-aiobotocore-neptune-module"></a>

# Examples for aiobotocore Neptune module

> [Index](../README.md) > [Neptune](./README.md) > Examples

- [Examples for aiobotocore Neptune module](#examples-for-aiobotocore-neptune-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[neptune]` package installed.

Write your `Neptune` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type NeptuneClient
# and provides type checking and code completion
async with session.create_client("neptune") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_role_to_db_cluster()
    

    
    # paginator has type DescribeDBClusterEndpointsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_db_cluster_endpoints")
    async for item in paginator.paginate(...):
        # item has type DBClusterEndpointMessageTypeDef
        print(item)
    

    
    # waiter has type DBInstanceAvailableWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("db_instance_available")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[neptune]` or a standalone
`types_aiobotocore_neptune` package, you have to explicitly specify
`client: NeptuneClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_neptune.client import NeptuneClient
from types_aiobotocore_neptune.type_defs import None
from types_aiobotocore_neptune.paginator import DescribeDBClusterEndpointsPaginator
from types_aiobotocore_neptune.waiter import DBInstanceAvailableWaiter
from types_aiobotocore_neptune.literals import PaginatorName
from types_aiobotocore_neptune.literals import WaiterName


session = get_session()

async with session.create_client("neptune") as client:
    client: NeptuneClient

    
    result: None = client.add_role_to_db_cluster()
    

    
    paginator_name: PaginatorName = "describe_db_cluster_endpoints"
    paginator: DescribeDBClusterEndpointsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DBClusterEndpointMessageTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "db_instance_available"
    waiter: DBInstanceAvailableWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
