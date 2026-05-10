# Examples

> [Index](../README.md) > [ManagedintegrationsforIoTDeviceManagement](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ManagedintegrationsforIoTDeviceManagement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations.html#managedintegrationsforiotdevicemanagement)
    type annotations stubs module [types-aiobotocore-iot-managed-integrations](https://pypi.org/project/types-aiobotocore-iot-managed-integrations/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iot-managed-integrations]` package installed.

Write your `ManagedintegrationsforIoTDeviceManagement` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# ManagedintegrationsforIoTDeviceManagementClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iot-managed-integrations") as client:  # (1)
    result = await client.create_account_association()  # (2)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. result: [:material-code-braces: CreateAccountAssociationResponseTypeDef](./type_defs.md#createaccountassociationresponsetypedef)



#### Paginator usage example

```python
# ListAccountAssociationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator = client.get_paginator("list_account_associations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListAccountAssociationsPaginator](./paginators.md#listaccountassociationspaginator)
3. item: [:material-code-braces: ListAccountAssociationsResponseTypeDef](./type_defs.md#listaccountassociationsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[iot-managed-integrations]`
or a standalone `types_aiobotocore_iot_managed_integrations` package, you have to explicitly specify
`client: ManagedintegrationsforIoTDeviceManagementClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# ManagedintegrationsforIoTDeviceManagementClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.client import ManagedintegrationsforIoTDeviceManagementClient
from types_aiobotocore_iot_managed_integrations.type_defs import CreateAccountAssociationResponseTypeDef
from types_aiobotocore_iot_managed_integrations.type_defs import CreateAccountAssociationRequestTypeDef


session = get_session()

async with session.create_client("iot-managed-integrations") as client:
    client: ManagedintegrationsforIoTDeviceManagementClient
    kwargs: CreateAccountAssociationRequestTypeDef = {...}
    result: CreateAccountAssociationResponseTypeDef = await client.create_account_association(**kwargs)
```



#### Paginator usage example

```python
# ListAccountAssociationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.client import ManagedintegrationsforIoTDeviceManagementClient
from types_aiobotocore_iot_managed_integrations.paginator import ListAccountAssociationsPaginator
from types_aiobotocore_iot_managed_integrations.type_defs import ListAccountAssociationsResponseTypeDef


session = get_session()

async with session.create_client("iot-managed-integrations") as client:
    client: ManagedintegrationsforIoTDeviceManagementClient
    paginator: ListAccountAssociationsPaginator = client.get_paginator("list_account_associations")
    async for item in paginator.paginate(...):
        item: ListAccountAssociationsResponseTypeDef
        print(item)
```


