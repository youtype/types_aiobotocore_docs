<a id="examples-for-aiobotocore-marketplacemetering-module"></a>

# Examples for aiobotocore MarketplaceMetering module

> [Index](../README.md) > [MarketplaceMetering](./README.md) > Examples

- [Examples for aiobotocore MarketplaceMetering module](#examples-for-aiobotocore-marketplacemetering-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[meteringmarketplace]` package installed.

Write your `MarketplaceMetering` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MarketplaceMeteringClient
# and provides type checking and code completion
async with session.create_client("meteringmarketplace") as client:
    
    # result has type BatchMeterUsageResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_meter_usage()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[meteringmarketplace]` or a standalone
`types_aiobotocore_meteringmarketplace` package, you have to explicitly specify
`client: MarketplaceMeteringClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_meteringmarketplace.client import MarketplaceMeteringClient
from types_aiobotocore_meteringmarketplace.type_defs import BatchMeterUsageResultTypeDef






session = get_session()

async with session.create_client("meteringmarketplace") as client:
    client: MarketplaceMeteringClient

    
    result: BatchMeterUsageResultTypeDef = client.batch_meter_usage()
    

    

    
```
