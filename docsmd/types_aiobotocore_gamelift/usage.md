# Examples

> [Index](../README.md) > [GameLift](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [GameLift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#gamelift)
    type annotations stubs module [types-aiobotocore-gamelift](https://pypi.org/project/types-aiobotocore-gamelift/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[gamelift]` package installed.

Write your `GameLift` code as usual,
type checking and code completion should work out of the box.



```python
# GameLiftClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("gamelift") as client:  # (1)
    result = await client.claim_game_server()  # (2)
```

1. client: [GameLiftClient](./client.md)
2. result: [:material-code-braces: ClaimGameServerOutputTypeDef](./type_defs.md#claimgameserveroutputtypedef) 



```python
# DescribeFleetAttributesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("gamelift") as client:  # (1)
    paginator = client.get_paginator("describe_fleet_attributes")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeFleetAttributesPaginator](./paginators.md#describefleetattributespaginator)
3. item: [:material-code-braces: DescribeFleetAttributesOutputTypeDef](./type_defs.md#describefleetattributesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[gamelift]`
or a standalone `types_aiobotocore_gamelift` package, you have to explicitly specify
`client: GameLiftClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# GameLiftClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.client import GameLiftClient
from types_aiobotocore_gamelift.type_defs import ClaimGameServerOutputTypeDef
from types_aiobotocore_gamelift.type_defs import ClaimGameServerInputTypeDef


session = get_session()

async with session.create_client("gamelift") as client:
    client: GameLiftClient
    kwargs: ClaimGameServerInputTypeDef = {...}
    result: ClaimGameServerOutputTypeDef = await client.claim_game_server(**kwargs)
```



```python
# DescribeFleetAttributesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.client import GameLiftClient
from types_aiobotocore_gamelift.paginator import DescribeFleetAttributesPaginator
from types_aiobotocore_gamelift.type_defs import DescribeFleetAttributesOutputTypeDef


session = get_session()

async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeFleetAttributesPaginator = client.get_paginator("describe_fleet_attributes")
    async for item in paginator.paginate(...):
        item: DescribeFleetAttributesOutputTypeDef
        print(item)
```


