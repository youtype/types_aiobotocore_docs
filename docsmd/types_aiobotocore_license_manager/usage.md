# Examples

> [Index](../README.md) > [LicenseManager](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LicenseManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#licensemanager)
    type annotations stubs module [types-aiobotocore-license-manager](https://pypi.org/project/types-aiobotocore-license-manager/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[license-manager]` package installed.

Write your `LicenseManager` code as usual,
type checking and code completion should work out of the box.



```python
# LicenseManagerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("license-manager") as client:  # (1)
    result = await client.accept_grant()  # (2)
```

1. client: [LicenseManagerClient](./client.md)
2. result: [:material-code-braces: AcceptGrantResponseTypeDef](./type_defs.md#acceptgrantresponsetypedef) 



```python
# ListAssociationsForLicenseConfigurationPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("license-manager") as client:  # (1)
    paginator = client.get_paginator("list_associations_for_license_configuration")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [LicenseManagerClient](./client.md)
2. paginator: [ListAssociationsForLicenseConfigurationPaginator](./paginators.md#listassociationsforlicenseconfigurationpaginator)
3. item: [:material-code-braces: ListAssociationsForLicenseConfigurationResponseTypeDef](./type_defs.md#listassociationsforlicenseconfigurationresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[license-manager]`
or a standalone `types_aiobotocore_license_manager` package, you have to explicitly specify
`client: LicenseManagerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LicenseManagerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_license_manager.client import LicenseManagerClient
from types_aiobotocore_license_manager.type_defs import AcceptGrantResponseTypeDef
from types_aiobotocore_license_manager.type_defs import AcceptGrantRequestTypeDef


session = get_session()

async with session.create_client("license-manager") as client:
    client: LicenseManagerClient
    kwargs: AcceptGrantRequestTypeDef = {...}
    result: AcceptGrantResponseTypeDef = await client.accept_grant(**kwargs)
```



```python
# ListAssociationsForLicenseConfigurationPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_license_manager.client import LicenseManagerClient
from types_aiobotocore_license_manager.paginator import ListAssociationsForLicenseConfigurationPaginator
from types_aiobotocore_license_manager.type_defs import ListAssociationsForLicenseConfigurationResponseTypeDef


session = get_session()

async with session.create_client("license-manager") as client:
    client: LicenseManagerClient
    paginator: ListAssociationsForLicenseConfigurationPaginator = client.get_paginator("list_associations_for_license_configuration")
    async for item in paginator.paginate(...):
        item: ListAssociationsForLicenseConfigurationResponseTypeDef
        print(item)
```


