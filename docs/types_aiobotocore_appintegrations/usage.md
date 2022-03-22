<a id="examples-for-aiobotocore-appintegrationsservice-module"></a>

# Examples for aiobotocore AppIntegrationsService module

> [Index](../README.md) > [AppIntegrationsService](./README.md) > Examples

- [Examples for aiobotocore AppIntegrationsService module](#examples-for-aiobotocore-appintegrationsservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[appintegrations]` package installed.

Write your `AppIntegrationsService` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AppIntegrationsServiceClient
# and provides type checking and code completion
async with session.create_client("appintegrations") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[appintegrations]` or a standalone
`types_aiobotocore_appintegrations` package, you have to explicitly specify
`client: AppIntegrationsServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_appintegrations.client import AppIntegrationsServiceClient
from types_aiobotocore_appintegrations.type_defs import bool






session = get_session()

async with session.create_client("appintegrations") as client:
    client: AppIntegrationsServiceClient

    
    result: bool = client.can_paginate()
    

    

    
```
