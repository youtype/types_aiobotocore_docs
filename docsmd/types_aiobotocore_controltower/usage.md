# Examples

> [Index](../README.md) > [ControlTower](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
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
    result = await client.disable_control()  # (2)
```

1. client: [ControlTowerClient](./client.md)
2. result: [:material-code-braces: DisableControlOutputTypeDef](./type_defs.md#disablecontroloutputtypedef) 



```python
# ListEnabledControlsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("controltower") as client:  # (1)
    paginator = client.get_paginator("list_enabled_controls")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ControlTowerClient](./client.md)
2. paginator: [ListEnabledControlsPaginator](./paginators.md#listenabledcontrolspaginator)
3. item: [:material-code-braces: ListEnabledControlsOutputTypeDef](./type_defs.md#listenabledcontrolsoutputtypedef) 




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
from types_aiobotocore_controltower.type_defs import DisableControlOutputTypeDef
from types_aiobotocore_controltower.type_defs import DisableControlInputRequestTypeDef


session = get_session()

async with session.create_client("controltower") as client:
    client: ControlTowerClient
    kwargs: DisableControlInputRequestTypeDef = {...}
    result: DisableControlOutputTypeDef = await client.disable_control(**kwargs)
```



```python
# ListEnabledControlsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_controltower.client import ControlTowerClient
from types_aiobotocore_controltower.paginator import ListEnabledControlsPaginator
from types_aiobotocore_controltower.type_defs import ListEnabledControlsOutputTypeDef


session = get_session()

async with session.create_client("controltower") as client:
    client: ControlTowerClient
    paginator: ListEnabledControlsPaginator = client.get_paginator("list_enabled_controls")
    async for item in paginator.paginate(...):
        item: ListEnabledControlsOutputTypeDef
        print(item)
```


