# Examples

> [Index](../README.md) > [MigrationHubStrategyRecommendations](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MigrationHubStrategyRecommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#migrationhubstrategyrecommendations)
    type annotations stubs module [types-aiobotocore-migrationhubstrategy](https://pypi.org/project/types-aiobotocore-migrationhubstrategy/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[migrationhubstrategy]` package installed.

Write your `MigrationHubStrategyRecommendations` code as usual,
type checking and code completion should work out of the box.



```python
# MigrationHubStrategyRecommendationsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("migrationhubstrategy") as client:  # (1)
    result = await client.get_application_component_details()  # (2)
```

1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
2. result: [:material-code-braces: GetApplicationComponentDetailsResponseTypeDef](./type_defs.md#getapplicationcomponentdetailsresponsetypedef) 



```python
# GetServerDetailsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("migrationhubstrategy") as client:  # (1)
    paginator = client.get_paginator("get_server_details")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
2. paginator: [GetServerDetailsPaginator](./paginators.md#getserverdetailspaginator)
3. item: [:material-code-braces: GetServerDetailsResponseTypeDef](./type_defs.md#getserverdetailsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[migrationhubstrategy]`
or a standalone `types_aiobotocore_migrationhubstrategy` package, you have to explicitly specify
`client: MigrationHubStrategyRecommendationsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MigrationHubStrategyRecommendationsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient
from types_aiobotocore_migrationhubstrategy.type_defs import GetApplicationComponentDetailsResponseTypeDef
from types_aiobotocore_migrationhubstrategy.type_defs import GetApplicationComponentDetailsRequestTypeDef


session = get_session()

async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    kwargs: GetApplicationComponentDetailsRequestTypeDef = {...}
    result: GetApplicationComponentDetailsResponseTypeDef = await client.get_application_component_details(**kwargs)
```



```python
# GetServerDetailsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient
from types_aiobotocore_migrationhubstrategy.paginator import GetServerDetailsPaginator
from types_aiobotocore_migrationhubstrategy.type_defs import GetServerDetailsResponseTypeDef


session = get_session()

async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    paginator: GetServerDetailsPaginator = client.get_paginator("get_server_details")
    async for item in paginator.paginate(...):
        item: GetServerDetailsResponseTypeDef
        print(item)
```


