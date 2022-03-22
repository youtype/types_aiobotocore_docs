<a id="examples-for-aiobotocore-pinpointemail-module"></a>

# Examples for aiobotocore PinpointEmail module

> [Index](../README.md) > [PinpointEmail](./README.md) > Examples

- [Examples for aiobotocore PinpointEmail module](#examples-for-aiobotocore-pinpointemail-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[pinpoint-email]` package installed.

Write your `PinpointEmail` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type PinpointEmailClient
# and provides type checking and code completion
async with session.create_client("pinpoint-email") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetDedicatedIpsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_dedicated_ips")
    async for item in paginator.paginate(...):
        # item has type GetDedicatedIpsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[pinpoint-email]` or a standalone
`types_aiobotocore_pinpoint_email` package, you have to explicitly specify
`client: PinpointEmailClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.client import PinpointEmailClient
from types_aiobotocore_pinpoint_email.type_defs import bool
from types_aiobotocore_pinpoint_email.paginator import GetDedicatedIpsPaginator

from types_aiobotocore_pinpoint_email.literals import PaginatorName



session = get_session()

async with session.create_client("pinpoint-email") as client:
    client: PinpointEmailClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_dedicated_ips"
    paginator: GetDedicatedIpsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetDedicatedIpsResponseTypeDef
        print(item)
    

    
```
