# Examples

> [Index](../README.md) > [MarketplaceEntitlementService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#marketplaceentitlementservice)
    type annotations stubs module [types-aiobotocore-marketplace-entitlement](https://pypi.org/project/types-aiobotocore-marketplace-entitlement/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[marketplace-entitlement]` package installed.

Write your `MarketplaceEntitlementService` code as usual,
type checking and code completion should work out of the box.



```python
# MarketplaceEntitlementServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("marketplace-entitlement") as client:  # (1)
    result = await client.get_entitlements()  # (2)
```

1. client: [MarketplaceEntitlementServiceClient](./client.md)
2. result: [:material-code-braces: GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef) 



```python
# GetEntitlementsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("marketplace-entitlement") as client:  # (1)
    paginator = client.get_paginator("get_entitlements")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MarketplaceEntitlementServiceClient](./client.md)
2. paginator: [GetEntitlementsPaginator](./paginators.md#getentitlementspaginator)
3. item: [:material-code-braces: GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[marketplace-entitlement]`
or a standalone `types_aiobotocore_marketplace_entitlement` package, you have to explicitly specify
`client: MarketplaceEntitlementServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MarketplaceEntitlementServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_entitlement.client import MarketplaceEntitlementServiceClient
from types_aiobotocore_marketplace_entitlement.type_defs import GetEntitlementsResultTypeDef
from types_aiobotocore_marketplace_entitlement.type_defs import GetEntitlementsRequestTypeDef


session = get_session()

async with session.create_client("marketplace-entitlement") as client:
    client: MarketplaceEntitlementServiceClient
    kwargs: GetEntitlementsRequestTypeDef = {...}
    result: GetEntitlementsResultTypeDef = await client.get_entitlements(**kwargs)
```



```python
# GetEntitlementsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_entitlement.client import MarketplaceEntitlementServiceClient
from types_aiobotocore_marketplace_entitlement.paginator import GetEntitlementsPaginator
from types_aiobotocore_marketplace_entitlement.type_defs import GetEntitlementsResultTypeDef


session = get_session()

async with session.create_client("marketplace-entitlement") as client:
    client: MarketplaceEntitlementServiceClient
    paginator: GetEntitlementsPaginator = client.get_paginator("get_entitlements")
    async for item in paginator.paginate(...):
        item: GetEntitlementsResultTypeDef
        print(item)
```


