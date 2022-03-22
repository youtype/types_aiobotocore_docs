<a id="examples-for-aiobotocore-cloudcontrolapi-module"></a>

# Examples for aiobotocore CloudControlApi module

> [Index](../README.md) > [CloudControlApi](./README.md) > Examples

- [Examples for aiobotocore CloudControlApi module](#examples-for-aiobotocore-cloudcontrolapi-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cloudcontrol]` package installed.

Write your `CloudControlApi` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudControlApiClient
# and provides type checking and code completion
async with session.create_client("cloudcontrol") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
    # waiter has type ResourceRequestSuccessWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("resource_request_success")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cloudcontrol]` or a standalone
`types_aiobotocore_cloudcontrol` package, you have to explicitly specify
`client: CloudControlApiClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudcontrol.client import CloudControlApiClient
from types_aiobotocore_cloudcontrol.type_defs import bool

from types_aiobotocore_cloudcontrol.waiter import ResourceRequestSuccessWaiter

from types_aiobotocore_cloudcontrol.literals import WaiterName


session = get_session()

async with session.create_client("cloudcontrol") as client:
    client: CloudControlApiClient

    
    result: bool = client.can_paginate()
    

    

    
    waiter_name: WaiterName = "resource_request_success"
    waiter: ResourceRequestSuccessWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
