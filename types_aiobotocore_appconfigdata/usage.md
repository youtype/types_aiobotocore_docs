<a id="examples-for-aiobotocore-appconfigdata-module"></a>

# Examples for aiobotocore AppConfigData module

> [Index](../README.md) > [AppConfigData](./README.md) > Examples

- [Examples for aiobotocore AppConfigData module](#examples-for-aiobotocore-appconfigdata-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[appconfigdata]` package installed.

Write your `AppConfigData` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AppConfigDataClient
# and provides type checking and code completion
async with session.create_client("appconfigdata") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[appconfigdata]` or a standalone
`types_aiobotocore_appconfigdata` package, you have to explicitly specify
`client: AppConfigDataClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_appconfigdata.client import AppConfigDataClient
from types_aiobotocore_appconfigdata.type_defs import bool






session = get_session()

async with session.create_client("appconfigdata") as client:
    client: AppConfigDataClient

    
    result: bool = client.can_paginate()
    

    

    
```
