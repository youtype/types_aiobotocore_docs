<a id="examples-for-aiobotocore-iot1clickdevicesservice-module"></a>

# Examples for aiobotocore IoT1ClickDevicesService module

> [Index](../README.md) > [IoT1ClickDevicesService](./README.md) > Examples

- [Examples for aiobotocore IoT1ClickDevicesService module](#examples-for-aiobotocore-iot1clickdevicesservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iot1click-devices]` package installed.

Write your `IoT1ClickDevicesService` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoT1ClickDevicesServiceClient
# and provides type checking and code completion
async with session.create_client("iot1click-devices") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListDeviceEventsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_device_events")
    async for item in paginator.paginate(...):
        # item has type ListDeviceEventsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iot1click-devices]` or a standalone
`types_aiobotocore_iot1click_devices` package, you have to explicitly specify
`client: IoT1ClickDevicesServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot1click_devices.client import IoT1ClickDevicesServiceClient
from types_aiobotocore_iot1click_devices.type_defs import bool
from types_aiobotocore_iot1click_devices.paginator import ListDeviceEventsPaginator

from types_aiobotocore_iot1click_devices.literals import PaginatorName



session = get_session()

async with session.create_client("iot1click-devices") as client:
    client: IoT1ClickDevicesServiceClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_device_events"
    paginator: ListDeviceEventsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDeviceEventsResponseTypeDef
        print(item)
    

    
```
