<a id="examples-for-aiobotocore-migrationhubstrategyrecommendations-module"></a>

# Examples for aiobotocore MigrationHubStrategyRecommendations module

> [Index](../README.md) > [MigrationHubStrategyRecommendations](./README.md) >
> Examples

- [Examples for aiobotocore MigrationHubStrategyRecommendations module](#examples-for-aiobotocore-migrationhubstrategyrecommendations-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[migrationhubstrategy]` package installed.

Write your `MigrationHubStrategyRecommendations` code as usual, type checking
and code completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MigrationHubStrategyRecommendationsClient
# and provides type checking and code completion
async with session.create_client("migrationhubstrategy") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetServerDetailsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_server_details")
    async for item in paginator.paginate(...):
        # item has type GetServerDetailsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[migrationhubstrategy]` or a standalone
`types_aiobotocore_migrationhubstrategy` package, you have to explicitly
specify `client: MigrationHubStrategyRecommendationsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient
from types_aiobotocore_migrationhubstrategy.type_defs import bool
from types_aiobotocore_migrationhubstrategy.paginator import GetServerDetailsPaginator

from types_aiobotocore_migrationhubstrategy.literals import PaginatorName



session = get_session()

async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_server_details"
    paginator: GetServerDetailsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetServerDetailsResponseTypeDef
        print(item)
    

    
```