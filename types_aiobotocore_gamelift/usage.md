<a id="examples-for-aiobotocore-gamelift-module"></a>

# Examples for aiobotocore GameLift module

> [Index](../README.md) > [GameLift](./README.md) > Examples

- [Examples for aiobotocore GameLift module](#examples-for-aiobotocore-gamelift-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[gamelift]` package installed.

Write your `GameLift` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type GameLiftClient
# and provides type checking and code completion
async with session.create_client("gamelift") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_match()
    

    
    # paginator has type DescribeFleetAttributesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_fleet_attributes")
    async for item in paginator.paginate(...):
        # item has type DescribeFleetAttributesOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[gamelift]` or a standalone
`types_aiobotocore_gamelift` package, you have to explicitly specify
`client: GameLiftClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.client import GameLiftClient
from types_aiobotocore_gamelift.type_defs import Dict[str, Any]
from types_aiobotocore_gamelift.paginator import DescribeFleetAttributesPaginator

from types_aiobotocore_gamelift.literals import PaginatorName



session = get_session()

async with session.create_client("gamelift") as client:
    client: GameLiftClient

    
    result: Dict[str, Any] = client.accept_match()
    

    
    paginator_name: PaginatorName = "describe_fleet_attributes"
    paginator: DescribeFleetAttributesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeFleetAttributesOutputTypeDef
        print(item)
    

    
```
