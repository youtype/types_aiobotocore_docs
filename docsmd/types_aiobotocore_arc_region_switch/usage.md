# Examples

> [Index](../README.md) > [ARCRegionswitch](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ARCRegionswitch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-region-switch.html#arcregionswitch)
    type annotations stubs module [types-aiobotocore-arc-region-switch](https://pypi.org/project/types-aiobotocore-arc-region-switch/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[arc-region-switch]` package installed.

Write your `ARCRegionswitch` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ARCRegionswitchClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("arc-region-switch") as client:  # (1)
    result = await client.create_plan()  # (2)
```

1. client: [ARCRegionswitchClient](./client.md)
2. result: [:material-code-braces: CreatePlanResponseTypeDef](./type_defs.md#createplanresponsetypedef)



#### Paginator usage example

```python
# GetPlanEvaluationStatusPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("arc-region-switch") as client:  # (1)
    paginator = client.get_paginator("get_plan_evaluation_status")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ARCRegionswitchClient](./client.md)
2. paginator: [GetPlanEvaluationStatusPaginator](./paginators.md#getplanevaluationstatuspaginator)
3. item: [:material-code-braces: GetPlanEvaluationStatusResponseTypeDef](./type_defs.md#getplanevaluationstatusresponsetypedef)



#### Waiter usage example

```python
# PlanEvaluationStatusPassedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("arc-region-switch") as client:  # (1)
    waiter = client.get_waiter("plan_evaluation_status_passed")  # (2)
    await waiter.wait(...)
```

1. client: [ARCRegionswitchClient](./client.md)
2. waiter: [PlanEvaluationStatusPassedWaiter](./waiters.md#planevaluationstatuspassedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[arc-region-switch]`
or a standalone `types_aiobotocore_arc_region_switch` package, you have to explicitly specify
`client: ARCRegionswitchClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ARCRegionswitchClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_arc_region_switch.client import ARCRegionswitchClient
from types_aiobotocore_arc_region_switch.type_defs import CreatePlanResponseTypeDef
from types_aiobotocore_arc_region_switch.type_defs import CreatePlanRequestTypeDef


session = get_session()

async with session.create_client("arc-region-switch") as client:
    client: ARCRegionswitchClient
    kwargs: CreatePlanRequestTypeDef = {...}
    result: CreatePlanResponseTypeDef = await client.create_plan(**kwargs)
```



#### Paginator usage example

```python
# GetPlanEvaluationStatusPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_arc_region_switch.client import ARCRegionswitchClient
from types_aiobotocore_arc_region_switch.paginator import GetPlanEvaluationStatusPaginator
from types_aiobotocore_arc_region_switch.type_defs import GetPlanEvaluationStatusResponseTypeDef


session = get_session()

async with session.create_client("arc-region-switch") as client:
    client: ARCRegionswitchClient
    paginator: GetPlanEvaluationStatusPaginator = client.get_paginator("get_plan_evaluation_status")
    async for item in paginator.paginate(...):
        item: GetPlanEvaluationStatusResponseTypeDef
        print(item)
```



#### Waiter usage example

```python
# PlanEvaluationStatusPassedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_arc_region_switch.client import ARCRegionswitchClient
from types_aiobotocore_arc_region_switch.waiter import PlanEvaluationStatusPassedWaiter


session = get_session()

async with session.create_client("arc-region-switch") as client:
    client: ARCRegionswitchClient
    waiter: PlanEvaluationStatusPassedWaiter = client.get_waiter("plan_evaluation_status_passed")
    await waiter.wait(...)
```
