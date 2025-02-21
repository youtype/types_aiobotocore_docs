# Examples

> [Index](../README.md) > [MarketplaceMetering](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceMetering](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#marketplacemetering)
    type annotations stubs module [types-aiobotocore-meteringmarketplace](https://pypi.org/project/types-aiobotocore-meteringmarketplace/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[meteringmarketplace]` package installed.

Write your `MarketplaceMetering` code as usual,
type checking and code completion should work out of the box.



```python
# MarketplaceMeteringClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("meteringmarketplace") as client:  # (1)
    result = await client.batch_meter_usage()  # (2)
```

1. client: [MarketplaceMeteringClient](./client.md)
2. result: [:material-code-braces: BatchMeterUsageResultTypeDef](./type_defs.md#batchmeterusageresulttypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[meteringmarketplace]`
or a standalone `types_aiobotocore_meteringmarketplace` package, you have to explicitly specify
`client: MarketplaceMeteringClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MarketplaceMeteringClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_meteringmarketplace.client import MarketplaceMeteringClient
from types_aiobotocore_meteringmarketplace.type_defs import BatchMeterUsageResultTypeDef
from types_aiobotocore_meteringmarketplace.type_defs import BatchMeterUsageRequestTypeDef


session = get_session()

async with session.create_client("meteringmarketplace") as client:
    client: MarketplaceMeteringClient
    kwargs: BatchMeterUsageRequestTypeDef = {...}
    result: BatchMeterUsageResultTypeDef = await client.batch_meter_usage(**kwargs)
```




