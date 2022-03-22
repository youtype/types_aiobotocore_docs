<a id="examples-for-aiobotocore-snowdevicemanagement-module"></a>

# Examples for aiobotocore SnowDeviceManagement module

> [Index](../README.md) > [SnowDeviceManagement](./README.md) > Examples

- [Examples for aiobotocore SnowDeviceManagement module](#examples-for-aiobotocore-snowdevicemanagement-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[snow-device-management]` package installed.

Write your `SnowDeviceManagement` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SnowDeviceManagementClient
# and provides type checking and code completion
async with session.create_client("snow-device-management") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListDeviceResourcesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_device_resources")
    async for item in paginator.paginate(...):
        # item has type ListDeviceResourcesOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[snow-device-management]` or a standalone
`types_aiobotocore_snow_device_management` package, you have to explicitly
specify `client: SnowDeviceManagementClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_snow_device_management.client import SnowDeviceManagementClient
from types_aiobotocore_snow_device_management.type_defs import bool
from types_aiobotocore_snow_device_management.paginator import ListDeviceResourcesPaginator

from types_aiobotocore_snow_device_management.literals import PaginatorName



session = get_session()

async with session.create_client("snow-device-management") as client:
    client: SnowDeviceManagementClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_device_resources"
    paginator: ListDeviceResourcesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDeviceResourcesOutputTypeDef
        print(item)
    

    
```
