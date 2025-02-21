# Examples

> [Index](../README.md) > [DeadlineCloud](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DeadlineCloud](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline.html#deadlinecloud)
    type annotations stubs module [types-aiobotocore-deadline](https://pypi.org/project/types-aiobotocore-deadline/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[deadline]` package installed.

Write your `DeadlineCloud` code as usual,
type checking and code completion should work out of the box.



```python
# DeadlineCloudClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("deadline") as client:  # (1)
    result = await client.assume_fleet_role_for_read()  # (2)
```

1. client: [DeadlineCloudClient](./client.md)
2. result: [:material-code-braces: AssumeFleetRoleForReadResponseTypeDef](./type_defs.md#assumefleetroleforreadresponsetypedef) 



```python
# GetSessionsStatisticsAggregationPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("deadline") as client:  # (1)
    paginator = client.get_paginator("get_sessions_statistics_aggregation")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DeadlineCloudClient](./client.md)
2. paginator: [GetSessionsStatisticsAggregationPaginator](./paginators.md#getsessionsstatisticsaggregationpaginator)
3. item: [:material-code-braces: GetSessionsStatisticsAggregationResponseTypeDef](./type_defs.md#getsessionsstatisticsaggregationresponsetypedef) 



```python
# FleetActiveWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("deadline") as client:  # (1)
    waiter = client.get_waiter("fleet_active")  # (2)
    await waiter.wait()
```

1. client: [DeadlineCloudClient](./client.md)
2. waiter: [FleetActiveWaiter](./waiters.md#fleetactivewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[deadline]`
or a standalone `types_aiobotocore_deadline` package, you have to explicitly specify
`client: DeadlineCloudClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DeadlineCloudClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_deadline.client import DeadlineCloudClient
from types_aiobotocore_deadline.type_defs import AssumeFleetRoleForReadResponseTypeDef
from types_aiobotocore_deadline.type_defs import AssumeFleetRoleForReadRequestTypeDef


session = get_session()

async with session.create_client("deadline") as client:
    client: DeadlineCloudClient
    kwargs: AssumeFleetRoleForReadRequestTypeDef = {...}
    result: AssumeFleetRoleForReadResponseTypeDef = await client.assume_fleet_role_for_read(**kwargs)
```



```python
# GetSessionsStatisticsAggregationPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_deadline.client import DeadlineCloudClient
from types_aiobotocore_deadline.paginator import GetSessionsStatisticsAggregationPaginator
from types_aiobotocore_deadline.type_defs import GetSessionsStatisticsAggregationResponseTypeDef


session = get_session()

async with session.create_client("deadline") as client:
    client: DeadlineCloudClient
    paginator: GetSessionsStatisticsAggregationPaginator = client.get_paginator("get_sessions_statistics_aggregation")
    async for item in paginator.paginate(...):
        item: GetSessionsStatisticsAggregationResponseTypeDef
        print(item)
```



```python
# FleetActiveWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_deadline.client import DeadlineCloudClient
from types_aiobotocore_deadline.waiter import FleetActiveWaiter


session = get_session()

async with session.create_client("deadline") as client:
    client: DeadlineCloudClient
    waiter: FleetActiveWaiter = client.get_waiter("fleet_active")
    await waiter.wait()
```
