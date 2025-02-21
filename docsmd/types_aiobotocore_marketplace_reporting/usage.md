# Examples

> [Index](../README.md) > [MarketplaceReportingService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceReportingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting.html#marketplacereportingservice)
    type annotations stubs module [types-aiobotocore-marketplace-reporting](https://pypi.org/project/types-aiobotocore-marketplace-reporting/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[marketplace-reporting]` package installed.

Write your `MarketplaceReportingService` code as usual,
type checking and code completion should work out of the box.



```python
# MarketplaceReportingServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("marketplace-reporting") as client:  # (1)
    result = await client.get_buyer_dashboard()  # (2)
```

1. client: [MarketplaceReportingServiceClient](./client.md)
2. result: [:material-code-braces: GetBuyerDashboardOutputTypeDef](./type_defs.md#getbuyerdashboardoutputtypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[marketplace-reporting]`
or a standalone `types_aiobotocore_marketplace_reporting` package, you have to explicitly specify
`client: MarketplaceReportingServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MarketplaceReportingServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_reporting.client import MarketplaceReportingServiceClient
from types_aiobotocore_marketplace_reporting.type_defs import GetBuyerDashboardOutputTypeDef
from types_aiobotocore_marketplace_reporting.type_defs import GetBuyerDashboardInputTypeDef


session = get_session()

async with session.create_client("marketplace-reporting") as client:
    client: MarketplaceReportingServiceClient
    kwargs: GetBuyerDashboardInputTypeDef = {...}
    result: GetBuyerDashboardOutputTypeDef = await client.get_buyer_dashboard(**kwargs)
```




