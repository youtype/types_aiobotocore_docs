<a id="examples-for-aiobotocore-forecastservice-module"></a>

# Examples for aiobotocore ForecastService module

> [Index](../README.md) > [ForecastService](./README.md) > Examples

- [Examples for aiobotocore ForecastService module](#examples-for-aiobotocore-forecastservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[forecast]` package installed.

Write your `ForecastService` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ForecastServiceClient
# and provides type checking and code completion
async with session.create_client("forecast") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListDatasetGroupsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_dataset_groups")
    async for item in paginator.paginate(...):
        # item has type ListDatasetGroupsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[forecast]` or a standalone
`types_aiobotocore_forecast` package, you have to explicitly specify
`client: ForecastServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_forecast.client import ForecastServiceClient
from types_aiobotocore_forecast.type_defs import bool
from types_aiobotocore_forecast.paginator import ListDatasetGroupsPaginator

from types_aiobotocore_forecast.literals import PaginatorName



session = get_session()

async with session.create_client("forecast") as client:
    client: ForecastServiceClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_dataset_groups"
    paginator: ListDatasetGroupsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDatasetGroupsResponseTypeDef
        print(item)
    

    
```
