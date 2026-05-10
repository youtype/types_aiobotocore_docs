# Examples

> [Index](../README.md) > [MarketplaceDiscovery](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceDiscovery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-discovery.html#marketplacediscovery)
    type annotations stubs module [types-aiobotocore-marketplace-discovery](https://pypi.org/project/types-aiobotocore-marketplace-discovery/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[marketplace-discovery]` package installed.

Write your `MarketplaceDiscovery` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MarketplaceDiscoveryClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("marketplace-discovery") as client:  # (1)
    result = await client.get_listing()  # (2)
```

1. client: [MarketplaceDiscoveryClient](./client.md)
2. result: [:material-code-braces: GetListingOutputTypeDef](./type_defs.md#getlistingoutputtypedef)



#### Paginator usage example

```python
# GetOfferTermsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("marketplace-discovery") as client:  # (1)
    paginator = client.get_paginator("get_offer_terms")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MarketplaceDiscoveryClient](./client.md)
2. paginator: [GetOfferTermsPaginator](./paginators.md#getoffertermspaginator)
3. item: [:material-code-braces: GetOfferTermsOutputTypeDef](./type_defs.md#getoffertermsoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[marketplace-discovery]`
or a standalone `types_aiobotocore_marketplace_discovery` package, you have to explicitly specify
`client: MarketplaceDiscoveryClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MarketplaceDiscoveryClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_discovery.client import MarketplaceDiscoveryClient
from types_aiobotocore_marketplace_discovery.type_defs import GetListingOutputTypeDef
from types_aiobotocore_marketplace_discovery.type_defs import GetListingInputTypeDef


session = get_session()

async with session.create_client("marketplace-discovery") as client:
    client: MarketplaceDiscoveryClient
    kwargs: GetListingInputTypeDef = {...}
    result: GetListingOutputTypeDef = await client.get_listing(**kwargs)
```



#### Paginator usage example

```python
# GetOfferTermsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_discovery.client import MarketplaceDiscoveryClient
from types_aiobotocore_marketplace_discovery.paginator import GetOfferTermsPaginator
from types_aiobotocore_marketplace_discovery.type_defs import GetOfferTermsOutputTypeDef


session = get_session()

async with session.create_client("marketplace-discovery") as client:
    client: MarketplaceDiscoveryClient
    paginator: GetOfferTermsPaginator = client.get_paginator("get_offer_terms")
    async for item in paginator.paginate(...):
        item: GetOfferTermsOutputTypeDef
        print(item)
```


