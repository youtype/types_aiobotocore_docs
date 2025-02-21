# Examples

> [Index](../README.md) > [EMR](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EMR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#emr)
    type annotations stubs module [types-aiobotocore-emr](https://pypi.org/project/types-aiobotocore-emr/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[emr]` package installed.

Write your `EMR` code as usual,
type checking and code completion should work out of the box.



```python
# EMRClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("emr") as client:  # (1)
    result = await client.add_instance_fleet()  # (2)
```

1. client: [EMRClient](./client.md)
2. result: [:material-code-braces: AddInstanceFleetOutputTypeDef](./type_defs.md#addinstancefleetoutputtypedef) 



```python
# ListBootstrapActionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("emr") as client:  # (1)
    paginator = client.get_paginator("list_bootstrap_actions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EMRClient](./client.md)
2. paginator: [ListBootstrapActionsPaginator](./paginators.md#listbootstrapactionspaginator)
3. item: [:material-code-braces: ListBootstrapActionsOutputTypeDef](./type_defs.md#listbootstrapactionsoutputtypedef) 



```python
# ClusterRunningWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("emr") as client:  # (1)
    waiter = client.get_waiter("cluster_running")  # (2)
    await waiter.wait()
```

1. client: [EMRClient](./client.md)
2. waiter: [ClusterRunningWaiter](./waiters.md#clusterrunningwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[emr]`
or a standalone `types_aiobotocore_emr` package, you have to explicitly specify
`client: EMRClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EMRClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_emr.client import EMRClient
from types_aiobotocore_emr.type_defs import AddInstanceFleetOutputTypeDef
from types_aiobotocore_emr.type_defs import AddInstanceFleetInputTypeDef


session = get_session()

async with session.create_client("emr") as client:
    client: EMRClient
    kwargs: AddInstanceFleetInputTypeDef = {...}
    result: AddInstanceFleetOutputTypeDef = await client.add_instance_fleet(**kwargs)
```



```python
# ListBootstrapActionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_emr.client import EMRClient
from types_aiobotocore_emr.paginator import ListBootstrapActionsPaginator
from types_aiobotocore_emr.type_defs import ListBootstrapActionsOutputTypeDef


session = get_session()

async with session.create_client("emr") as client:
    client: EMRClient
    paginator: ListBootstrapActionsPaginator = client.get_paginator("list_bootstrap_actions")
    async for item in paginator.paginate(...):
        item: ListBootstrapActionsOutputTypeDef
        print(item)
```



```python
# ClusterRunningWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_emr.client import EMRClient
from types_aiobotocore_emr.waiter import ClusterRunningWaiter


session = get_session()

async with session.create_client("emr") as client:
    client: EMRClient
    waiter: ClusterRunningWaiter = client.get_waiter("cluster_running")
    await waiter.wait()
```
