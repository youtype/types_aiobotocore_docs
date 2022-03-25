<a id="examples-for-aiobotocore-applicationinsights-module"></a>

# Examples for aiobotocore ApplicationInsights module

> [Index](../README.md) > [ApplicationInsights](./README.md) > Examples

- [Examples for aiobotocore ApplicationInsights module](#examples-for-aiobotocore-applicationinsights-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[application-insights]` package installed.

Write your `ApplicationInsights` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ApplicationInsightsClient
# and provides type checking and code completion
async with session.create_client("application-insights") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[application-insights]` or a standalone
`types_aiobotocore_application_insights` package, you have to explicitly
specify `client: ApplicationInsightsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_application_insights.client import ApplicationInsightsClient
from types_aiobotocore_application_insights.type_defs import bool






session = get_session()

async with session.create_client("application-insights") as client:
    client: ApplicationInsightsClient

    
    result: bool = client.can_paginate()
    

    

    
```