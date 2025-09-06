# Paginators

> [Index](../README.md) > [SystemsManagerQuickSetup](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SystemsManagerQuickSetup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#systemsmanagerquicksetup)
    type annotations stubs module [types-aiobotocore-ssm-quicksetup](https://pypi.org/project/types-aiobotocore-ssm-quicksetup/).

## ListConfigurationManagersPaginator

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").get_paginator("list_configuration_managers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup/paginator/ListConfigurationManagers.html#SystemsManagerQuickSetup.Paginator.ListConfigurationManagers)

```python
# ListConfigurationManagersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_quicksetup.paginator import ListConfigurationManagersPaginator

session = get_session()
async with session.create_client("ssm-quicksetup") as client:  # (1)
    paginator: ListConfigurationManagersPaginator = client.get_paginator("list_configuration_managers")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationManagersOutputTypeDef
        print(item)  # (3)
```

1. client: [SystemsManagerQuickSetupClient](./client.md)
2. paginator: [ListConfigurationManagersPaginator](./paginators.md#listconfigurationmanagerspaginator)
3. item: `AioPageIterator[ListConfigurationManagersOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConfigurationManagersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListConfigurationManagersOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListConfigurationManagersOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConfigurationManagersInputPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationManagersInputPaginateTypeDef](./type_defs.md#listconfigurationmanagersinputpaginatetypedef)
## ListConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("ssm-quicksetup").get_paginator("list_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup/paginator/ListConfigurations.html#SystemsManagerQuickSetup.Paginator.ListConfigurations)

```python
# ListConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_quicksetup.paginator import ListConfigurationsPaginator

session = get_session()
async with session.create_client("ssm-quicksetup") as client:  # (1)
    paginator: ListConfigurationsPaginator = client.get_paginator("list_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationsOutputTypeDef
        print(item)  # (3)
```

1. client: [SystemsManagerQuickSetupClient](./client.md)
2. paginator: [ListConfigurationsPaginator](./paginators.md#listconfigurationspaginator)
3. item: `AioPageIterator[ListConfigurationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigurationDefinitionId: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ManagerArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListConfigurationsOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListConfigurationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConfigurationsInputPaginateTypeDef = {  # (1)
    "ConfigurationDefinitionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationsInputPaginateTypeDef](./type_defs.md#listconfigurationsinputpaginatetypedef)
