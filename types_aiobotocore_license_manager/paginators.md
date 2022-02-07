<a id="paginators-for-aiobotocore-licensemanager-module"></a>

# Paginators for aiobotocore LicenseManager module

> [Index](..) > [LicenseManager](.) > Paginators

Auto-generated documentation for
[LicenseManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
type annotations stubs module
[types-aiobotocore-license-manager](https://pypi.org/project/types-aiobotocore-license-manager/).

- [Paginators for aiobotocore LicenseManager module](#paginators-for-aiobotocore-licensemanager-module)
  - [ListAssociationsForLicenseConfigurationPaginator](#listassociationsforlicenseconfigurationpaginator)
  - [ListLicenseConfigurationsPaginator](#listlicenseconfigurationspaginator)
  - [ListLicenseSpecificationsForResourcePaginator](#listlicensespecificationsforresourcepaginator)
  - [ListResourceInventoryPaginator](#listresourceinventorypaginator)
  - [ListUsageForLicenseConfigurationPaginator](#listusageforlicenseconfigurationpaginator)

<a id="listassociationsforlicenseconfigurationpaginator"></a>

## ListAssociationsForLicenseConfigurationPaginator

Type annotations for
`session.create_client("license-manager").get_paginator("list_associations_for_license_configuration")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_license_manager.paginator import ListAssociationsForLicenseConfigurationPaginator

session = get_session()
async with session.create_client("license-manager") as client:
    client: LicenseManagerClient
    paginator: ListAssociationsForLicenseConfigurationPaginator = client.get_paginator("list_associations_for_license_configuration")
```

Boto3 documentation:
[LicenseManager.Paginator.ListAssociationsForLicenseConfiguration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration)

Arguments for `ListAssociationsForLicenseConfigurationPaginator.paginate`
method:

- `LicenseConfigurationArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssociationsForLicenseConfigurationPaginator.paginate` returns
`_PageIterator`\[[ListAssociationsForLicenseConfigurationResponseTypeDef](./type_defs.md#listassociationsforlicenseconfigurationresponsetypedef)\].

<a id="listlicenseconfigurationspaginator"></a>

## ListLicenseConfigurationsPaginator

Type annotations for
`session.create_client("license-manager").get_paginator("list_license_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_license_manager.paginator import ListLicenseConfigurationsPaginator

session = get_session()
async with session.create_client("license-manager") as client:
    client: LicenseManagerClient
    paginator: ListLicenseConfigurationsPaginator = client.get_paginator("list_license_configurations")
```

Boto3 documentation:
[LicenseManager.Paginator.ListLicenseConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseConfigurations)

Arguments for `ListLicenseConfigurationsPaginator.paginate` method:

- `LicenseConfigurationArns`: `Sequence`\[`str`\]
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListLicenseConfigurationsPaginator.paginate` returns
`_PageIterator`\[[ListLicenseConfigurationsResponseTypeDef](./type_defs.md#listlicenseconfigurationsresponsetypedef)\].

<a id="listlicensespecificationsforresourcepaginator"></a>

## ListLicenseSpecificationsForResourcePaginator

Type annotations for
`session.create_client("license-manager").get_paginator("list_license_specifications_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_license_manager.paginator import ListLicenseSpecificationsForResourcePaginator

session = get_session()
async with session.create_client("license-manager") as client:
    client: LicenseManagerClient
    paginator: ListLicenseSpecificationsForResourcePaginator = client.get_paginator("list_license_specifications_for_resource")
```

Boto3 documentation:
[LicenseManager.Paginator.ListLicenseSpecificationsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource)

Arguments for `ListLicenseSpecificationsForResourcePaginator.paginate` method:

- `ResourceArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListLicenseSpecificationsForResourcePaginator.paginate` returns
`_PageIterator`\[[ListLicenseSpecificationsForResourceResponseTypeDef](./type_defs.md#listlicensespecificationsforresourceresponsetypedef)\].

<a id="listresourceinventorypaginator"></a>

## ListResourceInventoryPaginator

Type annotations for
`session.create_client("license-manager").get_paginator("list_resource_inventory")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_license_manager.paginator import ListResourceInventoryPaginator

session = get_session()
async with session.create_client("license-manager") as client:
    client: LicenseManagerClient
    paginator: ListResourceInventoryPaginator = client.get_paginator("list_resource_inventory")
```

Boto3 documentation:
[LicenseManager.Paginator.ListResourceInventory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListResourceInventory)

Arguments for `ListResourceInventoryPaginator.paginate` method:

- `Filters`:
  `Sequence`\[[InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResourceInventoryPaginator.paginate` returns
`_PageIterator`\[[ListResourceInventoryResponseTypeDef](./type_defs.md#listresourceinventoryresponsetypedef)\].

<a id="listusageforlicenseconfigurationpaginator"></a>

## ListUsageForLicenseConfigurationPaginator

Type annotations for
`session.create_client("license-manager").get_paginator("list_usage_for_license_configuration")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_license_manager.paginator import ListUsageForLicenseConfigurationPaginator

session = get_session()
async with session.create_client("license-manager") as client:
    client: LicenseManagerClient
    paginator: ListUsageForLicenseConfigurationPaginator = client.get_paginator("list_usage_for_license_configuration")
```

Boto3 documentation:
[LicenseManager.Paginator.ListUsageForLicenseConfiguration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListUsageForLicenseConfiguration)

Arguments for `ListUsageForLicenseConfigurationPaginator.paginate` method:

- `LicenseConfigurationArn`: `str` *(required)*
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUsageForLicenseConfigurationPaginator.paginate` returns
`_PageIterator`\[[ListUsageForLicenseConfigurationResponseTypeDef](./type_defs.md#listusageforlicenseconfigurationresponsetypedef)\].
