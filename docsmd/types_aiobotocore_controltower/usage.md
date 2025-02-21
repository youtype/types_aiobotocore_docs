# Examples

> [Index](../README.md) > [ControlTower](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#controltower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[controltower]` package installed.

Write your `ControlTower` code as usual,
type checking and code completion should work out of the box.



```python
# ControlTowerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("controltower") as client:  # (1)
    result = await client.create_landing_zone()  # (2)
```

1. client: [ControlTowerClient](./client.md)
2. result: [:material-code-braces: CreateLandingZoneOutputTypeDef](./type_defs.md#createlandingzoneoutputtypedef) 



```python
# ListBaselinesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("controltower") as client:  # (1)
    paginator = client.get_paginator("list_baselines")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListBaselinesPaginator](./paginators.md#listbaselinespaginator)
3. item: [:material-code-braces: ListBaselinesOutputTypeDef](./type_defs.md#listbaselinesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[controltower]`
or a standalone `types_aiobotocore_controltower` package, you have to explicitly specify
`client: ControlTowerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ControlTowerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_controltower.client import ControlTowerClient
from types_aiobotocore_controltower.type_defs import CreateLandingZoneOutputTypeDef
from types_aiobotocore_controltower.type_defs import CreateLandingZoneInputTypeDef


session = get_session()

async with session.create_client("controltower") as client:
    client: ControlTowerClient
    kwargs: CreateLandingZoneInputTypeDef = {...}
    result: CreateLandingZoneOutputTypeDef = await client.create_landing_zone(**kwargs)
```



```python
# ListBaselinesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_controltower.client import ControlTowerClient
from types_aiobotocore_controltower.paginator import ListBaselinesPaginator
from types_aiobotocore_controltower.type_defs import ListBaselinesOutputTypeDef


session = get_session()

async with session.create_client("controltower") as client:
    client: ControlTowerClient
    paginator: ListBaselinesPaginator = client.get_paginator("list_baselines")
    async for item in paginator.paginate(...):
        item: ListBaselinesOutputTypeDef
        print(item)
```


