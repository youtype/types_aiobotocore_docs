# Examples

> [Index](../README.md) > [MarketplaceCatalog](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MarketplaceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#marketplacecatalog)
    type annotations stubs module [types-aiobotocore-marketplace-catalog](https://pypi.org/project/types-aiobotocore-marketplace-catalog/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[marketplace-catalog]` package installed.

Write your `MarketplaceCatalog` code as usual,
type checking and code completion should work out of the box.



```python
# MarketplaceCatalogClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("marketplace-catalog") as client:  # (1)
    result = await client.batch_describe_entities()  # (2)
```

1. client: [MarketplaceCatalogClient](./client.md)
2. result: [:material-code-braces: BatchDescribeEntitiesResponseTypeDef](./type_defs.md#batchdescribeentitiesresponsetypedef) 



```python
# ListChangeSetsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("marketplace-catalog") as client:  # (1)
    paginator = client.get_paginator("list_change_sets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MarketplaceCatalogClient](./client.md)
2. paginator: [ListChangeSetsPaginator](./paginators.md#listchangesetspaginator)
3. item: [:material-code-braces: ListChangeSetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[marketplace-catalog]`
or a standalone `types_aiobotocore_marketplace_catalog` package, you have to explicitly specify
`client: MarketplaceCatalogClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MarketplaceCatalogClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_catalog.client import MarketplaceCatalogClient
from types_aiobotocore_marketplace_catalog.type_defs import BatchDescribeEntitiesResponseTypeDef
from types_aiobotocore_marketplace_catalog.type_defs import BatchDescribeEntitiesRequestTypeDef


session = get_session()

async with session.create_client("marketplace-catalog") as client:
    client: MarketplaceCatalogClient
    kwargs: BatchDescribeEntitiesRequestTypeDef = {...}
    result: BatchDescribeEntitiesResponseTypeDef = await client.batch_describe_entities(**kwargs)
```



```python
# ListChangeSetsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_catalog.client import MarketplaceCatalogClient
from types_aiobotocore_marketplace_catalog.paginator import ListChangeSetsPaginator
from types_aiobotocore_marketplace_catalog.type_defs import ListChangeSetsResponseTypeDef


session = get_session()

async with session.create_client("marketplace-catalog") as client:
    client: MarketplaceCatalogClient
    paginator: ListChangeSetsPaginator = client.get_paginator("list_change_sets")
    async for item in paginator.paginate(...):
        item: ListChangeSetsResponseTypeDef
        print(item)
```


