<a id="examples-for-aiobotocore-licensemanager-module"></a>

# Examples for aiobotocore LicenseManager module

> [Index](../README.md) > [LicenseManager](./README.md) > Examples

- [Examples for aiobotocore LicenseManager module](#examples-for-aiobotocore-licensemanager-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[license-manager]` package installed.

Write your `LicenseManager` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type LicenseManagerClient
# and provides type checking and code completion
async with session.create_client("license-manager") as client:
    
    # result has type AcceptGrantResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_grant()
    

    
    # paginator has type ListAssociationsForLicenseConfigurationPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_associations_for_license_configuration")
    async for item in paginator.paginate(...):
        # item has type ListAssociationsForLicenseConfigurationResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[license-manager]` or a standalone
`types_aiobotocore_license_manager` package, you have to explicitly specify
`client: LicenseManagerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_license_manager.client import LicenseManagerClient
from types_aiobotocore_license_manager.type_defs import AcceptGrantResponseTypeDef
from types_aiobotocore_license_manager.paginator import ListAssociationsForLicenseConfigurationPaginator

from types_aiobotocore_license_manager.literals import PaginatorName



session = get_session()

async with session.create_client("license-manager") as client:
    client: LicenseManagerClient

    
    result: AcceptGrantResponseTypeDef = client.accept_grant()
    

    
    paginator_name: PaginatorName = "list_associations_for_license_configuration"
    paginator: ListAssociationsForLicenseConfigurationPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAssociationsForLicenseConfigurationResponseTypeDef
        print(item)
    

    
```
