# Examples

> [Index](../README.md) > [SystemsManagerQuickSetup](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SystemsManagerQuickSetup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#systemsmanagerquicksetup)
    type annotations stubs module [types-aiobotocore-ssm-quicksetup](https://pypi.org/project/types-aiobotocore-ssm-quicksetup/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ssm-quicksetup]` package installed.

Write your `SystemsManagerQuickSetup` code as usual,
type checking and code completion should work out of the box.



```python
# SystemsManagerQuickSetupClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm-quicksetup") as client:  # (1)
    result = await client.create_configuration_manager()  # (2)
```

1. client: [SystemsManagerQuickSetupClient](./client.md)
2. result: [:material-code-braces: CreateConfigurationManagerOutputTypeDef](./type_defs.md#createconfigurationmanageroutputtypedef) 



```python
# ListConfigurationManagersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm-quicksetup") as client:  # (1)
    paginator = client.get_paginator("list_configuration_managers")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SystemsManagerQuickSetupClient](./client.md)
2. paginator: [ListConfigurationManagersPaginator](./paginators.md#listconfigurationmanagerspaginator)
3. item: [:material-code-braces: ListConfigurationManagersOutputTypeDef](./type_defs.md#listconfigurationmanagersoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[ssm-quicksetup]`
or a standalone `types_aiobotocore_ssm_quicksetup` package, you have to explicitly specify
`client: SystemsManagerQuickSetupClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SystemsManagerQuickSetupClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm_quicksetup.client import SystemsManagerQuickSetupClient
from types_aiobotocore_ssm_quicksetup.type_defs import CreateConfigurationManagerOutputTypeDef
from types_aiobotocore_ssm_quicksetup.type_defs import CreateConfigurationManagerInputTypeDef


session = get_session()

async with session.create_client("ssm-quicksetup") as client:
    client: SystemsManagerQuickSetupClient
    kwargs: CreateConfigurationManagerInputTypeDef = {...}
    result: CreateConfigurationManagerOutputTypeDef = await client.create_configuration_manager(**kwargs)
```



```python
# ListConfigurationManagersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm_quicksetup.client import SystemsManagerQuickSetupClient
from types_aiobotocore_ssm_quicksetup.paginator import ListConfigurationManagersPaginator
from types_aiobotocore_ssm_quicksetup.type_defs import ListConfigurationManagersOutputTypeDef


session = get_session()

async with session.create_client("ssm-quicksetup") as client:
    client: SystemsManagerQuickSetupClient
    paginator: ListConfigurationManagersPaginator = client.get_paginator("list_configuration_managers")
    async for item in paginator.paginate(...):
        item: ListConfigurationManagersOutputTypeDef
        print(item)
```


