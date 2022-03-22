<a id="examples-for-aiobotocore-personalizeevents-module"></a>

# Examples for aiobotocore PersonalizeEvents module

> [Index](../README.md) > [PersonalizeEvents](./README.md) > Examples

- [Examples for aiobotocore PersonalizeEvents module](#examples-for-aiobotocore-personalizeevents-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[personalize-events]` package installed.

Write your `PersonalizeEvents` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type PersonalizeEventsClient
# and provides type checking and code completion
async with session.create_client("personalize-events") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[personalize-events]` or a standalone
`types_aiobotocore_personalize_events` package, you have to explicitly specify
`client: PersonalizeEventsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_personalize_events.client import PersonalizeEventsClient
from types_aiobotocore_personalize_events.type_defs import bool






session = get_session()

async with session.create_client("personalize-events") as client:
    client: PersonalizeEventsClient

    
    result: bool = client.can_paginate()
    

    

    
```
