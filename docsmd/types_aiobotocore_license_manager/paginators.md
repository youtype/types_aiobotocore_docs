# Paginators

> [Index](../README.md) > [LicenseManager](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [LicenseManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#licensemanager)
    type annotations stubs module [types-aiobotocore-license-manager](https://pypi.org/project/types-aiobotocore-license-manager/).

## ListAssociationsForLicenseConfigurationPaginator

Type annotations and code completion for `#!python session.create_client("license-manager").get_paginator("list_associations_for_license_configuration")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/paginator/ListAssociationsForLicenseConfiguration.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration)

```python
# ListAssociationsForLicenseConfigurationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager.paginator import ListAssociationsForLicenseConfigurationPaginator

session = get_session()
async with session.create_client("license-manager") as client:  # (1)
    paginator: ListAssociationsForLicenseConfigurationPaginator = client.get_paginator("list_associations_for_license_configuration")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociationsForLicenseConfigurationResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerClient](./client.md)
2. paginator: [ListAssociationsForLicenseConfigurationPaginator](./paginators.md#listassociationsforlicenseconfigurationpaginator)
3. item: [:material-code-braces: ListAssociationsForLicenseConfigurationResponseTypeDef](./type_defs.md#listassociationsforlicenseconfigurationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociationsForLicenseConfigurationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LicenseConfigurationArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAssociationsForLicenseConfigurationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociationsForLicenseConfigurationResponseTypeDef](./type_defs.md#listassociationsforlicenseconfigurationresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssociationsForLicenseConfigurationRequestPaginateTypeDef = {  # (1)
    "LicenseConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociationsForLicenseConfigurationRequestPaginateTypeDef](./type_defs.md#listassociationsforlicenseconfigurationrequestpaginatetypedef) 
## ListLicenseConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("license-manager").get_paginator("list_license_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/paginator/ListLicenseConfigurations.html#LicenseManager.Paginator.ListLicenseConfigurations)

```python
# ListLicenseConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager.paginator import ListLicenseConfigurationsPaginator

session = get_session()
async with session.create_client("license-manager") as client:  # (1)
    paginator: ListLicenseConfigurationsPaginator = client.get_paginator("list_license_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListLicenseConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerClient](./client.md)
2. paginator: [ListLicenseConfigurationsPaginator](./paginators.md#listlicenseconfigurationspaginator)
3. item: [:material-code-braces: ListLicenseConfigurationsResponseTypeDef](./type_defs.md#listlicenseconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLicenseConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LicenseConfigurationArns: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListLicenseConfigurationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListLicenseConfigurationsResponseTypeDef](./type_defs.md#listlicenseconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLicenseConfigurationsRequestPaginateTypeDef = {  # (1)
    "LicenseConfigurationArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLicenseConfigurationsRequestPaginateTypeDef](./type_defs.md#listlicenseconfigurationsrequestpaginatetypedef) 
## ListLicenseSpecificationsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("license-manager").get_paginator("list_license_specifications_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/paginator/ListLicenseSpecificationsForResource.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource)

```python
# ListLicenseSpecificationsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager.paginator import ListLicenseSpecificationsForResourcePaginator

session = get_session()
async with session.create_client("license-manager") as client:  # (1)
    paginator: ListLicenseSpecificationsForResourcePaginator = client.get_paginator("list_license_specifications_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListLicenseSpecificationsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerClient](./client.md)
2. paginator: [ListLicenseSpecificationsForResourcePaginator](./paginators.md#listlicensespecificationsforresourcepaginator)
3. item: [:material-code-braces: ListLicenseSpecificationsForResourceResponseTypeDef](./type_defs.md#listlicensespecificationsforresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLicenseSpecificationsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListLicenseSpecificationsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLicenseSpecificationsForResourceResponseTypeDef](./type_defs.md#listlicensespecificationsforresourceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLicenseSpecificationsForResourceRequestPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLicenseSpecificationsForResourceRequestPaginateTypeDef](./type_defs.md#listlicensespecificationsforresourcerequestpaginatetypedef) 
## ListResourceInventoryPaginator

Type annotations and code completion for `#!python session.create_client("license-manager").get_paginator("list_resource_inventory")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/paginator/ListResourceInventory.html#LicenseManager.Paginator.ListResourceInventory)

```python
# ListResourceInventoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager.paginator import ListResourceInventoryPaginator

session = get_session()
async with session.create_client("license-manager") as client:  # (1)
    paginator: ListResourceInventoryPaginator = client.get_paginator("list_resource_inventory")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceInventoryResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerClient](./client.md)
2. paginator: [ListResourceInventoryPaginator](./paginators.md#listresourceinventorypaginator)
3. item: [:material-code-braces: ListResourceInventoryResponseTypeDef](./type_defs.md#listresourceinventoryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceInventoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[InventoryFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListResourceInventoryResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListResourceInventoryResponseTypeDef](./type_defs.md#listresourceinventoryresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceInventoryRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceInventoryRequestPaginateTypeDef](./type_defs.md#listresourceinventoryrequestpaginatetypedef) 
## ListUsageForLicenseConfigurationPaginator

Type annotations and code completion for `#!python session.create_client("license-manager").get_paginator("list_usage_for_license_configuration")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager/paginator/ListUsageForLicenseConfiguration.html#LicenseManager.Paginator.ListUsageForLicenseConfiguration)

```python
# ListUsageForLicenseConfigurationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_license_manager.paginator import ListUsageForLicenseConfigurationPaginator

session = get_session()
async with session.create_client("license-manager") as client:  # (1)
    paginator: ListUsageForLicenseConfigurationPaginator = client.get_paginator("list_usage_for_license_configuration")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsageForLicenseConfigurationResponseTypeDef
        print(item)  # (3)
```

1. client: [LicenseManagerClient](./client.md)
2. paginator: [ListUsageForLicenseConfigurationPaginator](./paginators.md#listusageforlicenseconfigurationpaginator)
3. item: [:material-code-braces: ListUsageForLicenseConfigurationResponseTypeDef](./type_defs.md#listusageforlicenseconfigurationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsageForLicenseConfigurationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LicenseConfigurationArn: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListUsageForLicenseConfigurationResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListUsageForLicenseConfigurationResponseTypeDef](./type_defs.md#listusageforlicenseconfigurationresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsageForLicenseConfigurationRequestPaginateTypeDef = {  # (1)
    "LicenseConfigurationArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsageForLicenseConfigurationRequestPaginateTypeDef](./type_defs.md#listusageforlicenseconfigurationrequestpaginatetypedef) 
