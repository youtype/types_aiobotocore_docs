# Examples

> [Index](../README.md) > [LicenseManagerLinuxSubscriptions](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LicenseManagerLinuxSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#licensemanagerlinuxsubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-linux-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-linux-subscriptions/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[license-manager-linux-subscriptions]` package installed.

Write your `LicenseManagerLinuxSubscriptions` code as usual,
type checking and code completion should work out of the box.



```python
# LicenseManagerLinuxSubscriptionsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("license-manager-linux-subscriptions") as client:  # (1)
    result = await client.get_registered_subscription_provider()  # (2)
```

1. client: [LicenseManagerLinuxSubscriptionsClient](./client.md)
2. result: [:material-code-braces: GetRegisteredSubscriptionProviderResponseTypeDef](./type_defs.md#getregisteredsubscriptionproviderresponsetypedef) 



```python
# ListLinuxSubscriptionInstancesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("license-manager-linux-subscriptions") as client:  # (1)
    paginator = client.get_paginator("list_linux_subscription_instances")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [LicenseManagerLinuxSubscriptionsClient](./client.md)
2. paginator: [ListLinuxSubscriptionInstancesPaginator](./paginators.md#listlinuxsubscriptioninstancespaginator)
3. item: [:material-code-braces: ListLinuxSubscriptionInstancesResponseTypeDef](./type_defs.md#listlinuxsubscriptioninstancesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[license-manager-linux-subscriptions]`
or a standalone `types_aiobotocore_license_manager_linux_subscriptions` package, you have to explicitly specify
`client: LicenseManagerLinuxSubscriptionsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LicenseManagerLinuxSubscriptionsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_linux_subscriptions.client import LicenseManagerLinuxSubscriptionsClient
from types_aiobotocore_license_manager_linux_subscriptions.type_defs import GetRegisteredSubscriptionProviderResponseTypeDef
from types_aiobotocore_license_manager_linux_subscriptions.type_defs import GetRegisteredSubscriptionProviderRequestTypeDef


session = get_session()

async with session.create_client("license-manager-linux-subscriptions") as client:
    client: LicenseManagerLinuxSubscriptionsClient
    kwargs: GetRegisteredSubscriptionProviderRequestTypeDef = {...}
    result: GetRegisteredSubscriptionProviderResponseTypeDef = await client.get_registered_subscription_provider(**kwargs)
```



```python
# ListLinuxSubscriptionInstancesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_linux_subscriptions.client import LicenseManagerLinuxSubscriptionsClient
from types_aiobotocore_license_manager_linux_subscriptions.paginator import ListLinuxSubscriptionInstancesPaginator
from types_aiobotocore_license_manager_linux_subscriptions.type_defs import ListLinuxSubscriptionInstancesResponseTypeDef


session = get_session()

async with session.create_client("license-manager-linux-subscriptions") as client:
    client: LicenseManagerLinuxSubscriptionsClient
    paginator: ListLinuxSubscriptionInstancesPaginator = client.get_paginator("list_linux_subscription_instances")
    async for item in paginator.paginate(...):
        item: ListLinuxSubscriptionInstancesResponseTypeDef
        print(item)
```


