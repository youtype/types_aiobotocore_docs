<a id="examples-for-aiobotocore-servicecatalog-module"></a>

# Examples for aiobotocore ServiceCatalog module

> [Index](../README.md) > [ServiceCatalog](./README.md) > Examples

- [Examples for aiobotocore ServiceCatalog module](#examples-for-aiobotocore-servicecatalog-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[servicecatalog]` package installed.

Write your `ServiceCatalog` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ServiceCatalogClient
# and provides type checking and code completion
async with session.create_client("servicecatalog") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_portfolio_share()
    

    
    # paginator has type ListAcceptedPortfolioSharesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_accepted_portfolio_shares")
    async for item in paginator.paginate(...):
        # item has type ListAcceptedPortfolioSharesOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[servicecatalog]` or a standalone
`types_aiobotocore_servicecatalog` package, you have to explicitly specify
`client: ServiceCatalogClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog.client import ServiceCatalogClient
from types_aiobotocore_servicecatalog.type_defs import Dict[str, Any]
from types_aiobotocore_servicecatalog.paginator import ListAcceptedPortfolioSharesPaginator

from types_aiobotocore_servicecatalog.literals import PaginatorName



session = get_session()

async with session.create_client("servicecatalog") as client:
    client: ServiceCatalogClient

    
    result: Dict[str, Any] = client.accept_portfolio_share()
    

    
    paginator_name: PaginatorName = "list_accepted_portfolio_shares"
    paginator: ListAcceptedPortfolioSharesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAcceptedPortfolioSharesOutputTypeDef
        print(item)
    

    
```
