<a id="examples-for-aiobotocore-migrationhubconfig-module"></a>

# Examples for aiobotocore MigrationHubConfig module

> [Index](../README.md) > [MigrationHubConfig](./README.md) > Examples

- [Examples for aiobotocore MigrationHubConfig module](#examples-for-aiobotocore-migrationhubconfig-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[migrationhub-config]` package installed.

Write your `MigrationHubConfig` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MigrationHubConfigClient
# and provides type checking and code completion
async with session.create_client("migrationhub-config") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[migrationhub-config]` or a standalone
`types_aiobotocore_migrationhub_config` package, you have to explicitly specify
`client: MigrationHubConfigClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_migrationhub_config.client import MigrationHubConfigClient
from types_aiobotocore_migrationhub_config.type_defs import bool






session = get_session()

async with session.create_client("migrationhub-config") as client:
    client: MigrationHubConfigClient

    
    result: bool = client.can_paginate()
    

    

    
```
