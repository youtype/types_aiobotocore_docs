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
    result = await client.create_credential_locker()  # (2)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. result: [:material-code-braces: CreateCredentialLockerResponseTypeDef](./type_defs.md#createcredentiallockerresponsetypedef)



#### Paginator usage example

```python
# ListCredentialLockersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator = client.get_paginator("list_credential_lockers")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListCredentialLockersPaginator](./paginators.md#listcredentiallockerspaginator)
3. item: [:material-code-braces: ListCredentialLockersResponseTypeDef](./type_defs.md#listcredentiallockersresponsetypedef)




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
from types_aiobotocore_iot_managed_integrations.type_defs import CreateCredentialLockerResponseTypeDef
from types_aiobotocore_iot_managed_integrations.type_defs import CreateCredentialLockerRequestTypeDef


session = get_session()

async with session.create_client("iot-managed-integrations") as client:
    client: ManagedintegrationsforIoTDeviceManagementClient
    kwargs: CreateCredentialLockerRequestTypeDef = {...}
    result: CreateCredentialLockerResponseTypeDef = await client.create_credential_locker(**kwargs)
```



#### Paginator usage example

```python
# ListCredentialLockersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.client import ManagedintegrationsforIoTDeviceManagementClient
from types_aiobotocore_iot_managed_integrations.paginator import ListCredentialLockersPaginator
from types_aiobotocore_iot_managed_integrations.type_defs import ListCredentialLockersResponseTypeDef


session = get_session()

async with session.create_client("iot-managed-integrations") as client:
    client: ManagedintegrationsforIoTDeviceManagementClient
    paginator: ListCredentialLockersPaginator = client.get_paginator("list_credential_lockers")
    async for item in paginator.paginate(...):
        item: ListCredentialLockersResponseTypeDef
        print(item)
```


