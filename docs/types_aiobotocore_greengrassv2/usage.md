<a id="examples-for-aiobotocore-greengrassv2-module"></a>

# Examples for aiobotocore GreengrassV2 module

> [Index](../README.md) > [GreengrassV2](./README.md) > Examples

- [Examples for aiobotocore GreengrassV2 module](#examples-for-aiobotocore-greengrassv2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[greengrassv2]` package installed.

Write your `GreengrassV2` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type GreengrassV2Client
# and provides type checking and code completion
async with session.create_client("greengrassv2") as client:
    
    # result has type AssociateServiceRoleToAccountResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_service_role_to_account()
    

    
    # paginator has type ListClientDevicesAssociatedWithCoreDevicePaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_client_devices_associated_with_core_device")
    async for item in paginator.paginate(...):
        # item has type ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[greengrassv2]` or a standalone
`types_aiobotocore_greengrassv2` package, you have to explicitly specify
`client: GreengrassV2Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_greengrassv2.client import GreengrassV2Client
from types_aiobotocore_greengrassv2.type_defs import AssociateServiceRoleToAccountResponseTypeDef
from types_aiobotocore_greengrassv2.paginator import ListClientDevicesAssociatedWithCoreDevicePaginator

from types_aiobotocore_greengrassv2.literals import PaginatorName



session = get_session()

async with session.create_client("greengrassv2") as client:
    client: GreengrassV2Client

    
    result: AssociateServiceRoleToAccountResponseTypeDef = client.associate_service_role_to_account()
    

    
    paginator_name: PaginatorName = "list_client_devices_associated_with_core_device"
    paginator: ListClientDevicesAssociatedWithCoreDevicePaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef
        print(item)
    

    
```
