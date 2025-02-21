# Examples

> [Index](../README.md) > [LicenseManagerUserSubscriptions](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LicenseManagerUserSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#licensemanagerusersubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-user-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[license-manager-user-subscriptions]` package installed.

Write your `LicenseManagerUserSubscriptions` code as usual,
type checking and code completion should work out of the box.



```python
# LicenseManagerUserSubscriptionsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("license-manager-user-subscriptions") as client:  # (1)
    result = await client.associate_user()  # (2)
```

1. client: [LicenseManagerUserSubscriptionsClient](./client.md)
2. result: [:material-code-braces: AssociateUserResponseTypeDef](./type_defs.md#associateuserresponsetypedef) 



```python
# ListIdentityProvidersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("license-manager-user-subscriptions") as client:  # (1)
    paginator = client.get_paginator("list_identity_providers")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [LicenseManagerUserSubscriptionsClient](./client.md)
2. paginator: [ListIdentityProvidersPaginator](./paginators.md#listidentityproviderspaginator)
3. item: [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[license-manager-user-subscriptions]`
or a standalone `types_aiobotocore_license_manager_user_subscriptions` package, you have to explicitly specify
`client: LicenseManagerUserSubscriptionsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LicenseManagerUserSubscriptionsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_user_subscriptions.client import LicenseManagerUserSubscriptionsClient
from types_aiobotocore_license_manager_user_subscriptions.type_defs import AssociateUserResponseTypeDef
from types_aiobotocore_license_manager_user_subscriptions.type_defs import AssociateUserRequestTypeDef


session = get_session()

async with session.create_client("license-manager-user-subscriptions") as client:
    client: LicenseManagerUserSubscriptionsClient
    kwargs: AssociateUserRequestTypeDef = {...}
    result: AssociateUserResponseTypeDef = await client.associate_user(**kwargs)
```



```python
# ListIdentityProvidersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_license_manager_user_subscriptions.client import LicenseManagerUserSubscriptionsClient
from types_aiobotocore_license_manager_user_subscriptions.paginator import ListIdentityProvidersPaginator
from types_aiobotocore_license_manager_user_subscriptions.type_defs import ListIdentityProvidersResponseTypeDef


session = get_session()

async with session.create_client("license-manager-user-subscriptions") as client:
    client: LicenseManagerUserSubscriptionsClient
    paginator: ListIdentityProvidersPaginator = client.get_paginator("list_identity_providers")
    async for item in paginator.paginate(...):
        item: ListIdentityProvidersResponseTypeDef
        print(item)
```


