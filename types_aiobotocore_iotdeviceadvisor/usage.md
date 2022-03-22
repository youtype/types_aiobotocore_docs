<a id="examples-for-aiobotocore-iotdeviceadvisor-module"></a>

# Examples for aiobotocore IoTDeviceAdvisor module

> [Index](../README.md) > [IoTDeviceAdvisor](./README.md) > Examples

- [Examples for aiobotocore IoTDeviceAdvisor module](#examples-for-aiobotocore-iotdeviceadvisor-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iotdeviceadvisor]` package installed.

Write your `IoTDeviceAdvisor` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTDeviceAdvisorClient
# and provides type checking and code completion
async with session.create_client("iotdeviceadvisor") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iotdeviceadvisor]` or a standalone
`types_aiobotocore_iotdeviceadvisor` package, you have to explicitly specify
`client: IoTDeviceAdvisorClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotdeviceadvisor.client import IoTDeviceAdvisorClient
from types_aiobotocore_iotdeviceadvisor.type_defs import bool






session = get_session()

async with session.create_client("iotdeviceadvisor") as client:
    client: IoTDeviceAdvisorClient

    
    result: bool = client.can_paginate()
    

    

    
```
