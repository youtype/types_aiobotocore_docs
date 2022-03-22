<a id="examples-for-aiobotocore-forecastqueryservice-module"></a>

# Examples for aiobotocore ForecastQueryService module

> [Index](../README.md) > [ForecastQueryService](./README.md) > Examples

- [Examples for aiobotocore ForecastQueryService module](#examples-for-aiobotocore-forecastqueryservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[forecastquery]` package installed.

Write your `ForecastQueryService` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ForecastQueryServiceClient
# and provides type checking and code completion
async with session.create_client("forecastquery") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[forecastquery]` or a standalone
`types_aiobotocore_forecastquery` package, you have to explicitly specify
`client: ForecastQueryServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_forecastquery.client import ForecastQueryServiceClient
from types_aiobotocore_forecastquery.type_defs import bool






session = get_session()

async with session.create_client("forecastquery") as client:
    client: ForecastQueryServiceClient

    
    result: bool = client.can_paginate()
    

    

    
```
