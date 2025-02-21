# Examples

> [Index](../README.md) > [DeviceFarm](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DeviceFarm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#devicefarm)
    type annotations stubs module [types-aiobotocore-devicefarm](https://pypi.org/project/types-aiobotocore-devicefarm/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[devicefarm]` package installed.

Write your `DeviceFarm` code as usual,
type checking and code completion should work out of the box.



```python
# DeviceFarmClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("devicefarm") as client:  # (1)
    result = await client.create_device_pool()  # (2)
```

1. client: [DeviceFarmClient](./client.md)
2. result: [:material-code-braces: CreateDevicePoolResultTypeDef](./type_defs.md#createdevicepoolresulttypedef) 



```python
# GetOfferingStatusPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("devicefarm") as client:  # (1)
    paginator = client.get_paginator("get_offering_status")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DeviceFarmClient](./client.md)
2. paginator: [GetOfferingStatusPaginator](./paginators.md#getofferingstatuspaginator)
3. item: [:material-code-braces: GetOfferingStatusResultTypeDef](./type_defs.md#getofferingstatusresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[devicefarm]`
or a standalone `types_aiobotocore_devicefarm` package, you have to explicitly specify
`client: DeviceFarmClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DeviceFarmClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.client import DeviceFarmClient
from types_aiobotocore_devicefarm.type_defs import CreateDevicePoolResultTypeDef
from types_aiobotocore_devicefarm.type_defs import CreateDevicePoolRequestTypeDef


session = get_session()

async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    kwargs: CreateDevicePoolRequestTypeDef = {...}
    result: CreateDevicePoolResultTypeDef = await client.create_device_pool(**kwargs)
```



```python
# GetOfferingStatusPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.client import DeviceFarmClient
from types_aiobotocore_devicefarm.paginator import GetOfferingStatusPaginator
from types_aiobotocore_devicefarm.type_defs import GetOfferingStatusResultTypeDef


session = get_session()

async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient
    paginator: GetOfferingStatusPaginator = client.get_paginator("get_offering_status")
    async for item in paginator.paginate(...):
        item: GetOfferingStatusResultTypeDef
        print(item)
```


