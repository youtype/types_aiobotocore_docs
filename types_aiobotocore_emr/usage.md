<a id="examples-for-aiobotocore-emr-module"></a>

# Examples for aiobotocore EMR module

> [Index](../README.md) > [EMR](./README.md) > Examples

- [Examples for aiobotocore EMR module](#examples-for-aiobotocore-emr-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[emr]` package installed.

Write your `EMR` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type EMRClient
# and provides type checking and code completion
async with session.create_client("emr") as client:
    
    # result has type AddInstanceFleetOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_instance_fleet()
    

    
    # paginator has type ListBootstrapActionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_bootstrap_actions")
    async for item in paginator.paginate(...):
        # item has type ListBootstrapActionsOutputTypeDef
        print(item)
    

    
    # waiter has type ClusterRunningWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("cluster_running")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[emr]` or a standalone `types_aiobotocore_emr`
package, you have to explicitly specify `client: EMRClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_emr.client import EMRClient
from types_aiobotocore_emr.type_defs import AddInstanceFleetOutputTypeDef
from types_aiobotocore_emr.paginator import ListBootstrapActionsPaginator
from types_aiobotocore_emr.waiter import ClusterRunningWaiter
from types_aiobotocore_emr.literals import PaginatorName
from types_aiobotocore_emr.literals import WaiterName


session = get_session()

async with session.create_client("emr") as client:
    client: EMRClient

    
    result: AddInstanceFleetOutputTypeDef = client.add_instance_fleet()
    

    
    paginator_name: PaginatorName = "list_bootstrap_actions"
    paginator: ListBootstrapActionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListBootstrapActionsOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "cluster_running"
    waiter: ClusterRunningWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
