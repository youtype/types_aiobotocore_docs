# Examples

> [Index](../README.md) > [GreengrassV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [GreengrassV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#greengrassv2)
    type annotations stubs module [types-aiobotocore-greengrassv2](https://pypi.org/project/types-aiobotocore-greengrassv2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[greengrassv2]` package installed.

Write your `GreengrassV2` code as usual,
type checking and code completion should work out of the box.



```python
# GreengrassV2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("greengrassv2") as client:  # (1)
    result = await client.associate_service_role_to_account()  # (2)
```

1. client: [GreengrassV2Client](./client.md)
2. result: [:material-code-braces: AssociateServiceRoleToAccountResponseTypeDef](./type_defs.md#associateserviceroletoaccountresponsetypedef) 



```python
# ListClientDevicesAssociatedWithCoreDevicePaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("greengrassv2") as client:  # (1)
    paginator = client.get_paginator("list_client_devices_associated_with_core_device")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListClientDevicesAssociatedWithCoreDevicePaginator](./paginators.md#listclientdevicesassociatedwithcoredevicepaginator)
3. item: [:material-code-braces: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredeviceresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[greengrassv2]`
or a standalone `types_aiobotocore_greengrassv2` package, you have to explicitly specify
`client: GreengrassV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# GreengrassV2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_greengrassv2.client import GreengrassV2Client
from types_aiobotocore_greengrassv2.type_defs import AssociateServiceRoleToAccountResponseTypeDef
from types_aiobotocore_greengrassv2.type_defs import AssociateServiceRoleToAccountRequestTypeDef


session = get_session()

async with session.create_client("greengrassv2") as client:
    client: GreengrassV2Client
    kwargs: AssociateServiceRoleToAccountRequestTypeDef = {...}
    result: AssociateServiceRoleToAccountResponseTypeDef = await client.associate_service_role_to_account(**kwargs)
```



```python
# ListClientDevicesAssociatedWithCoreDevicePaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_greengrassv2.client import GreengrassV2Client
from types_aiobotocore_greengrassv2.paginator import ListClientDevicesAssociatedWithCoreDevicePaginator
from types_aiobotocore_greengrassv2.type_defs import ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef


session = get_session()

async with session.create_client("greengrassv2") as client:
    client: GreengrassV2Client
    paginator: ListClientDevicesAssociatedWithCoreDevicePaginator = client.get_paginator("list_client_devices_associated_with_core_device")
    async for item in paginator.paginate(...):
        item: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef
        print(item)
```


