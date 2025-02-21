# Examples

> [Index](../README.md) > [MarketplaceCommerceAnalytics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceCommerceAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#marketplacecommerceanalytics)
    type annotations stubs module [types-aiobotocore-marketplacecommerceanalytics](https://pypi.org/project/types-aiobotocore-marketplacecommerceanalytics/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[marketplacecommerceanalytics]` package installed.

Write your `MarketplaceCommerceAnalytics` code as usual,
type checking and code completion should work out of the box.



```python
# MarketplaceCommerceAnalyticsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("marketplacecommerceanalytics") as client:  # (1)
    result = await client.generate_data_set()  # (2)
```

1. client: [MarketplaceCommerceAnalyticsClient](./client.md)
2. result: [:material-code-braces: GenerateDataSetResultTypeDef](./type_defs.md#generatedatasetresulttypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[marketplacecommerceanalytics]`
or a standalone `types_aiobotocore_marketplacecommerceanalytics` package, you have to explicitly specify
`client: MarketplaceCommerceAnalyticsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MarketplaceCommerceAnalyticsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_marketplacecommerceanalytics.client import MarketplaceCommerceAnalyticsClient
from types_aiobotocore_marketplacecommerceanalytics.type_defs import GenerateDataSetResultTypeDef
from types_aiobotocore_marketplacecommerceanalytics.type_defs import GenerateDataSetRequestTypeDef


session = get_session()

async with session.create_client("marketplacecommerceanalytics") as client:
    client: MarketplaceCommerceAnalyticsClient
    kwargs: GenerateDataSetRequestTypeDef = {...}
    result: GenerateDataSetResultTypeDef = await client.generate_data_set(**kwargs)
```




