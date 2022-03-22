<a id="examples-for-aiobotocore-marketplacecatalog-module"></a>

# Examples for aiobotocore MarketplaceCatalog module

> [Index](../README.md) > [MarketplaceCatalog](./README.md) > Examples

- [Examples for aiobotocore MarketplaceCatalog module](#examples-for-aiobotocore-marketplacecatalog-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[marketplace-catalog]` package installed.

Write your `MarketplaceCatalog` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MarketplaceCatalogClient
# and provides type checking and code completion
async with session.create_client("marketplace-catalog") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[marketplace-catalog]` or a standalone
`types_aiobotocore_marketplace_catalog` package, you have to explicitly specify
`client: MarketplaceCatalogClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_marketplace_catalog.client import MarketplaceCatalogClient
from types_aiobotocore_marketplace_catalog.type_defs import bool






session = get_session()

async with session.create_client("marketplace-catalog") as client:
    client: MarketplaceCatalogClient

    
    result: bool = client.can_paginate()
    

    

    
```
