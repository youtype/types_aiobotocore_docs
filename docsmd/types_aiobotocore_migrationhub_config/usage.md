# Examples

> [Index](../README.md) > [MigrationHubConfig](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MigrationHubConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#migrationhubconfig)
    type annotations stubs module [types-aiobotocore-migrationhub-config](https://pypi.org/project/types-aiobotocore-migrationhub-config/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[migrationhub-config]` package installed.

Write your `MigrationHubConfig` code as usual,
type checking and code completion should work out of the box.



```python
# MigrationHubConfigClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("migrationhub-config") as client:  # (1)
    result = await client.create_home_region_control()  # (2)
```

1. client: [MigrationHubConfigClient](./client.md)
2. result: [:material-code-braces: CreateHomeRegionControlResultTypeDef](./type_defs.md#createhomeregioncontrolresulttypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[migrationhub-config]`
or a standalone `types_aiobotocore_migrationhub_config` package, you have to explicitly specify
`client: MigrationHubConfigClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MigrationHubConfigClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_migrationhub_config.client import MigrationHubConfigClient
from types_aiobotocore_migrationhub_config.type_defs import CreateHomeRegionControlResultTypeDef
from types_aiobotocore_migrationhub_config.type_defs import CreateHomeRegionControlRequestTypeDef


session = get_session()

async with session.create_client("migrationhub-config") as client:
    client: MigrationHubConfigClient
    kwargs: CreateHomeRegionControlRequestTypeDef = {...}
    result: CreateHomeRegionControlResultTypeDef = await client.create_home_region_control(**kwargs)
```




