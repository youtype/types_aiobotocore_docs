<a id="examples-for-aiobotocore-route53-module"></a>

# Examples for aiobotocore Route53 module

> [Index](../README.md) > [Route53](./README.md) > Examples

- [Examples for aiobotocore Route53 module](#examples-for-aiobotocore-route53-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[route53]` package installed.

Write your `Route53` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type Route53Client
# and provides type checking and code completion
async with session.create_client("route53") as client:
    
    # result has type ActivateKeySigningKeyResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.activate_key_signing_key()
    

    
    # paginator has type ListHealthChecksPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_health_checks")
    async for item in paginator.paginate(...):
        # item has type ListHealthChecksResponseTypeDef
        print(item)
    

    
    # waiter has type ResourceRecordSetsChangedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("resource_record_sets_changed")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[route53]` or a standalone
`types_aiobotocore_route53` package, you have to explicitly specify
`client: Route53Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53.client import Route53Client
from types_aiobotocore_route53.type_defs import ActivateKeySigningKeyResponseTypeDef
from types_aiobotocore_route53.paginator import ListHealthChecksPaginator
from types_aiobotocore_route53.waiter import ResourceRecordSetsChangedWaiter
from types_aiobotocore_route53.literals import PaginatorName
from types_aiobotocore_route53.literals import WaiterName


session = get_session()

async with session.create_client("route53") as client:
    client: Route53Client

    
    result: ActivateKeySigningKeyResponseTypeDef = client.activate_key_signing_key()
    

    
    paginator_name: PaginatorName = "list_health_checks"
    paginator: ListHealthChecksPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListHealthChecksResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "resource_record_sets_changed"
    waiter: ResourceRecordSetsChangedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
