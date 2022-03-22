<a id="examples-for-aiobotocore-iotevents-module"></a>

# Examples for aiobotocore IoTEvents module

> [Index](../README.md) > [IoTEvents](./README.md) > Examples

- [Examples for aiobotocore IoTEvents module](#examples-for-aiobotocore-iotevents-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iotevents]` package installed.

Write your `IoTEvents` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTEventsClient
# and provides type checking and code completion
async with session.create_client("iotevents") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iotevents]` or a standalone
`types_aiobotocore_iotevents` package, you have to explicitly specify
`client: IoTEventsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotevents.client import IoTEventsClient
from types_aiobotocore_iotevents.type_defs import bool






session = get_session()

async with session.create_client("iotevents") as client:
    client: IoTEventsClient

    
    result: bool = client.can_paginate()
    

    

    
```
