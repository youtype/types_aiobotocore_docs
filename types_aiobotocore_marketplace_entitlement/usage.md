<a id="examples-for-aiobotocore-marketplaceentitlementservice-module"></a>

# Examples for aiobotocore MarketplaceEntitlementService module

> [Index](../README.md) > [MarketplaceEntitlementService](./README.md) >
> Examples

- [Examples for aiobotocore MarketplaceEntitlementService module](#examples-for-aiobotocore-marketplaceentitlementservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[marketplace-entitlement]` package
installed.

Write your `MarketplaceEntitlementService` code as usual, type checking and
code completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MarketplaceEntitlementServiceClient
# and provides type checking and code completion
async with session.create_client("marketplace-entitlement") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetEntitlementsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_entitlements")
    async for item in paginator.paginate(...):
        # item has type GetEntitlementsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[marketplace-entitlement]` or a standalone
`types_aiobotocore_marketplace_entitlement` package, you have to explicitly
specify `client: MarketplaceEntitlementServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_marketplace_entitlement.client import MarketplaceEntitlementServiceClient
from types_aiobotocore_marketplace_entitlement.type_defs import bool
from types_aiobotocore_marketplace_entitlement.paginator import GetEntitlementsPaginator

from types_aiobotocore_marketplace_entitlement.literals import PaginatorName



session = get_session()

async with session.create_client("marketplace-entitlement") as client:
    client: MarketplaceEntitlementServiceClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_entitlements"
    paginator: GetEntitlementsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetEntitlementsResultTypeDef
        print(item)
    

    
```
