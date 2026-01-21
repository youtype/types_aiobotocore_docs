# Paginators

> [Index](../README.md) > [GameLift](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GameLift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#gamelift)
    type annotations stubs module [types-aiobotocore-gamelift](https://pypi.org/project/types-aiobotocore-gamelift/).

## DescribeFleetAttributesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_fleet_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeFleetAttributes.html#GameLift.Paginator.DescribeFleetAttributes)

```python
# DescribeFleetAttributesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeFleetAttributesPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeFleetAttributesPaginator = client.get_paginator("describe_fleet_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFleetAttributesOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeFleetAttributesPaginator](./paginators.md#describefleetattributespaginator)
3. item: `AioPageIterator[DescribeFleetAttributesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFleetAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeFleetAttributesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeFleetAttributesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFleetAttributesInputPaginateTypeDef = {  # (1)
    "FleetIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetAttributesInputPaginateTypeDef](./type_defs.md#describefleetattributesinputpaginatetypedef)
## DescribeFleetCapacityPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_fleet_capacity")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeFleetCapacity.html#GameLift.Paginator.DescribeFleetCapacity)

```python
# DescribeFleetCapacityPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeFleetCapacityPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeFleetCapacityPaginator = client.get_paginator("describe_fleet_capacity")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFleetCapacityOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeFleetCapacityPaginator](./paginators.md#describefleetcapacitypaginator)
3. item: `AioPageIterator[DescribeFleetCapacityOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFleetCapacityPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeFleetCapacityOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeFleetCapacityOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFleetCapacityInputPaginateTypeDef = {  # (1)
    "FleetIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetCapacityInputPaginateTypeDef](./type_defs.md#describefleetcapacityinputpaginatetypedef)
## DescribeFleetEventsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_fleet_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeFleetEvents.html#GameLift.Paginator.DescribeFleetEvents)

```python
# DescribeFleetEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeFleetEventsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeFleetEventsPaginator = client.get_paginator("describe_fleet_events")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFleetEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeFleetEventsPaginator](./paginators.md#describefleeteventspaginator)
3. item: `AioPageIterator[DescribeFleetEventsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFleetEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetId: str,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeFleetEventsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeFleetEventsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFleetEventsInputPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetEventsInputPaginateTypeDef](./type_defs.md#describefleeteventsinputpaginatetypedef)
## DescribeFleetUtilizationPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_fleet_utilization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeFleetUtilization.html#GameLift.Paginator.DescribeFleetUtilization)

```python
# DescribeFleetUtilizationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeFleetUtilizationPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeFleetUtilizationPaginator = client.get_paginator("describe_fleet_utilization")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFleetUtilizationOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeFleetUtilizationPaginator](./paginators.md#describefleetutilizationpaginator)
3. item: `AioPageIterator[DescribeFleetUtilizationOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFleetUtilizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeFleetUtilizationOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeFleetUtilizationOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFleetUtilizationInputPaginateTypeDef = {  # (1)
    "FleetIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetUtilizationInputPaginateTypeDef](./type_defs.md#describefleetutilizationinputpaginatetypedef)
## DescribeGameServerInstancesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_game_server_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeGameServerInstances.html#GameLift.Paginator.DescribeGameServerInstances)

```python
# DescribeGameServerInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeGameServerInstancesPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeGameServerInstancesPaginator = client.get_paginator("describe_game_server_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeGameServerInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeGameServerInstancesPaginator](./paginators.md#describegameserverinstancespaginator)
3. item: `AioPageIterator[DescribeGameServerInstancesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeGameServerInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GameServerGroupName: str,
    InstanceIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeGameServerInstancesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeGameServerInstancesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeGameServerInstancesInputPaginateTypeDef = {  # (1)
    "GameServerGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGameServerInstancesInputPaginateTypeDef](./type_defs.md#describegameserverinstancesinputpaginatetypedef)
## DescribeGameSessionDetailsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_game_session_details")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeGameSessionDetails.html#GameLift.Paginator.DescribeGameSessionDetails)

```python
# DescribeGameSessionDetailsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeGameSessionDetailsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeGameSessionDetailsPaginator = client.get_paginator("describe_game_session_details")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeGameSessionDetailsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeGameSessionDetailsPaginator](./paginators.md#describegamesessiondetailspaginator)
3. item: `AioPageIterator[DescribeGameSessionDetailsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeGameSessionDetailsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetId: str = ...,
    GameSessionId: str = ...,
    AliasId: str = ...,
    Location: str = ...,
    StatusFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeGameSessionDetailsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeGameSessionDetailsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeGameSessionDetailsInputPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGameSessionDetailsInputPaginateTypeDef](./type_defs.md#describegamesessiondetailsinputpaginatetypedef)
## DescribeGameSessionQueuesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_game_session_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeGameSessionQueues.html#GameLift.Paginator.DescribeGameSessionQueues)

```python
# DescribeGameSessionQueuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeGameSessionQueuesPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeGameSessionQueuesPaginator = client.get_paginator("describe_game_session_queues")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeGameSessionQueuesOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeGameSessionQueuesPaginator](./paginators.md#describegamesessionqueuespaginator)
3. item: `AioPageIterator[DescribeGameSessionQueuesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeGameSessionQueuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeGameSessionQueuesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeGameSessionQueuesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeGameSessionQueuesInputPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGameSessionQueuesInputPaginateTypeDef](./type_defs.md#describegamesessionqueuesinputpaginatetypedef)
## DescribeGameSessionsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_game_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeGameSessions.html#GameLift.Paginator.DescribeGameSessions)

```python
# DescribeGameSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeGameSessionsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeGameSessionsPaginator = client.get_paginator("describe_game_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeGameSessionsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeGameSessionsPaginator](./paginators.md#describegamesessionspaginator)
3. item: `AioPageIterator[DescribeGameSessionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeGameSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetId: str = ...,
    GameSessionId: str = ...,
    AliasId: str = ...,
    Location: str = ...,
    StatusFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeGameSessionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeGameSessionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeGameSessionsInputPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGameSessionsInputPaginateTypeDef](./type_defs.md#describegamesessionsinputpaginatetypedef)
## DescribeInstancesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeInstances.html#GameLift.Paginator.DescribeInstances)

```python
# DescribeInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeInstancesPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeInstancesPaginator = client.get_paginator("describe_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeInstancesPaginator](./paginators.md#describeinstancespaginator)
3. item: `AioPageIterator[DescribeInstancesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetId: str,
    InstanceId: str = ...,
    Location: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeInstancesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeInstancesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInstancesInputPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstancesInputPaginateTypeDef](./type_defs.md#describeinstancesinputpaginatetypedef)
## DescribeMatchmakingConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_matchmaking_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeMatchmakingConfigurations.html#GameLift.Paginator.DescribeMatchmakingConfigurations)

```python
# DescribeMatchmakingConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeMatchmakingConfigurationsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeMatchmakingConfigurationsPaginator = client.get_paginator("describe_matchmaking_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeMatchmakingConfigurationsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeMatchmakingConfigurationsPaginator](./paginators.md#describematchmakingconfigurationspaginator)
3. item: `AioPageIterator[DescribeMatchmakingConfigurationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeMatchmakingConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    RuleSetName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeMatchmakingConfigurationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeMatchmakingConfigurationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeMatchmakingConfigurationsInputPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMatchmakingConfigurationsInputPaginateTypeDef](./type_defs.md#describematchmakingconfigurationsinputpaginatetypedef)
## DescribeMatchmakingRuleSetsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_matchmaking_rule_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeMatchmakingRuleSets.html#GameLift.Paginator.DescribeMatchmakingRuleSets)

```python
# DescribeMatchmakingRuleSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeMatchmakingRuleSetsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeMatchmakingRuleSetsPaginator = client.get_paginator("describe_matchmaking_rule_sets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeMatchmakingRuleSetsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeMatchmakingRuleSetsPaginator](./paginators.md#describematchmakingrulesetspaginator)
3. item: `AioPageIterator[DescribeMatchmakingRuleSetsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeMatchmakingRuleSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeMatchmakingRuleSetsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeMatchmakingRuleSetsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeMatchmakingRuleSetsInputPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMatchmakingRuleSetsInputPaginateTypeDef](./type_defs.md#describematchmakingrulesetsinputpaginatetypedef)
## DescribePlayerSessionsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_player_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribePlayerSessions.html#GameLift.Paginator.DescribePlayerSessions)

```python
# DescribePlayerSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribePlayerSessionsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribePlayerSessionsPaginator = client.get_paginator("describe_player_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribePlayerSessionsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribePlayerSessionsPaginator](./paginators.md#describeplayersessionspaginator)
3. item: `AioPageIterator[DescribePlayerSessionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribePlayerSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GameSessionId: str = ...,
    PlayerId: str = ...,
    PlayerSessionId: str = ...,
    PlayerSessionStatusFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribePlayerSessionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribePlayerSessionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribePlayerSessionsInputPaginateTypeDef = {  # (1)
    "GameSessionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePlayerSessionsInputPaginateTypeDef](./type_defs.md#describeplayersessionsinputpaginatetypedef)
## DescribeScalingPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_scaling_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/DescribeScalingPolicies.html#GameLift.Paginator.DescribeScalingPolicies)

```python
# DescribeScalingPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeScalingPoliciesPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: DescribeScalingPoliciesPaginator = client.get_paginator("describe_scaling_policies")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeScalingPoliciesOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [DescribeScalingPoliciesPaginator](./paginators.md#describescalingpoliciespaginator)
3. item: `AioPageIterator[DescribeScalingPoliciesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeScalingPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetId: str,
    StatusFilter: ScalingStatusTypeType = ...,  # (1)
    Location: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeScalingPoliciesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ScalingStatusTypeType](./literals.md#scalingstatustypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeScalingPoliciesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeScalingPoliciesInputPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScalingPoliciesInputPaginateTypeDef](./type_defs.md#describescalingpoliciesinputpaginatetypedef)
## ListAliasesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListAliases.html#GameLift.Paginator.ListAliases)

```python
# ListAliasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListAliasesPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListAliasesOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
3. item: `AioPageIterator[ListAliasesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAliasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RoutingStrategyType: RoutingStrategyTypeType = ...,  # (1)
    Name: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAliasesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RoutingStrategyTypeType](./literals.md#routingstrategytypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAliasesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAliasesInputPaginateTypeDef = {  # (1)
    "RoutingStrategyType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAliasesInputPaginateTypeDef](./type_defs.md#listaliasesinputpaginatetypedef)
## ListBuildsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_builds")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListBuilds.html#GameLift.Paginator.ListBuilds)

```python
# ListBuildsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListBuildsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListBuildsPaginator = client.get_paginator("list_builds")  # (2)
    async for item in paginator.paginate(...):
        item: ListBuildsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListBuildsPaginator](./paginators.md#listbuildspaginator)
3. item: `AioPageIterator[ListBuildsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBuildsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Status: BuildStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListBuildsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: BuildStatusType](./literals.md#buildstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBuildsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBuildsInputPaginateTypeDef = {  # (1)
    "Status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBuildsInputPaginateTypeDef](./type_defs.md#listbuildsinputpaginatetypedef)
## ListComputePaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_compute")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListCompute.html#GameLift.Paginator.ListCompute)

```python
# ListComputePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListComputePaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListComputePaginator = client.get_paginator("list_compute")  # (2)
    async for item in paginator.paginate(...):
        item: ListComputeOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListComputePaginator](./paginators.md#listcomputepaginator)
3. item: `AioPageIterator[ListComputeOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListComputePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetId: str,
    Location: str = ...,
    ContainerGroupDefinitionName: str = ...,
    ComputeStatus: ListComputeInputStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListComputeOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListComputeInputStatusType](./literals.md#listcomputeinputstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListComputeOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListComputeInputPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListComputeInputPaginateTypeDef](./type_defs.md#listcomputeinputpaginatetypedef)
## ListContainerFleetsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_container_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListContainerFleets.html#GameLift.Paginator.ListContainerFleets)

```python
# ListContainerFleetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListContainerFleetsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListContainerFleetsPaginator = client.get_paginator("list_container_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: ListContainerFleetsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListContainerFleetsPaginator](./paginators.md#listcontainerfleetspaginator)
3. item: `AioPageIterator[ListContainerFleetsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContainerFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ContainerGroupDefinitionName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListContainerFleetsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListContainerFleetsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContainerFleetsInputPaginateTypeDef = {  # (1)
    "ContainerGroupDefinitionName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContainerFleetsInputPaginateTypeDef](./type_defs.md#listcontainerfleetsinputpaginatetypedef)
## ListContainerGroupDefinitionVersionsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_container_group_definition_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListContainerGroupDefinitionVersions.html#GameLift.Paginator.ListContainerGroupDefinitionVersions)

```python
# ListContainerGroupDefinitionVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListContainerGroupDefinitionVersionsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListContainerGroupDefinitionVersionsPaginator = client.get_paginator("list_container_group_definition_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListContainerGroupDefinitionVersionsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListContainerGroupDefinitionVersionsPaginator](./paginators.md#listcontainergroupdefinitionversionspaginator)
3. item: `AioPageIterator[ListContainerGroupDefinitionVersionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContainerGroupDefinitionVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListContainerGroupDefinitionVersionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListContainerGroupDefinitionVersionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContainerGroupDefinitionVersionsInputPaginateTypeDef = {  # (1)
    "Name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContainerGroupDefinitionVersionsInputPaginateTypeDef](./type_defs.md#listcontainergroupdefinitionversionsinputpaginatetypedef)
## ListContainerGroupDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_container_group_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListContainerGroupDefinitions.html#GameLift.Paginator.ListContainerGroupDefinitions)

```python
# ListContainerGroupDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListContainerGroupDefinitionsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListContainerGroupDefinitionsPaginator = client.get_paginator("list_container_group_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListContainerGroupDefinitionsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListContainerGroupDefinitionsPaginator](./paginators.md#listcontainergroupdefinitionspaginator)
3. item: `AioPageIterator[ListContainerGroupDefinitionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContainerGroupDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ContainerGroupType: ContainerGroupTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListContainerGroupDefinitionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ContainerGroupTypeType](./literals.md#containergrouptypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListContainerGroupDefinitionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContainerGroupDefinitionsInputPaginateTypeDef = {  # (1)
    "ContainerGroupType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContainerGroupDefinitionsInputPaginateTypeDef](./type_defs.md#listcontainergroupdefinitionsinputpaginatetypedef)
## ListFleetDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_fleet_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListFleetDeployments.html#GameLift.Paginator.ListFleetDeployments)

```python
# ListFleetDeploymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListFleetDeploymentsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListFleetDeploymentsPaginator = client.get_paginator("list_fleet_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListFleetDeploymentsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListFleetDeploymentsPaginator](./paginators.md#listfleetdeploymentspaginator)
3. item: `AioPageIterator[ListFleetDeploymentsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFleetDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFleetDeploymentsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFleetDeploymentsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFleetDeploymentsInputPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFleetDeploymentsInputPaginateTypeDef](./type_defs.md#listfleetdeploymentsinputpaginatetypedef)
## ListFleetsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListFleets.html#GameLift.Paginator.ListFleets)

```python
# ListFleetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListFleetsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListFleetsPaginator = client.get_paginator("list_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: ListFleetsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListFleetsPaginator](./paginators.md#listfleetspaginator)
3. item: `AioPageIterator[ListFleetsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BuildId: str = ...,
    ScriptId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFleetsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFleetsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFleetsInputPaginateTypeDef = {  # (1)
    "BuildId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFleetsInputPaginateTypeDef](./type_defs.md#listfleetsinputpaginatetypedef)
## ListGameServerGroupsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_game_server_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListGameServerGroups.html#GameLift.Paginator.ListGameServerGroups)

```python
# ListGameServerGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListGameServerGroupsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListGameServerGroupsPaginator = client.get_paginator("list_game_server_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGameServerGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListGameServerGroupsPaginator](./paginators.md#listgameservergroupspaginator)
3. item: `AioPageIterator[ListGameServerGroupsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGameServerGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListGameServerGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListGameServerGroupsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGameServerGroupsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGameServerGroupsInputPaginateTypeDef](./type_defs.md#listgameservergroupsinputpaginatetypedef)
## ListGameServersPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_game_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListGameServers.html#GameLift.Paginator.ListGameServers)

```python
# ListGameServersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListGameServersPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")  # (2)
    async for item in paginator.paginate(...):
        item: ListGameServersOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListGameServersPaginator](./paginators.md#listgameserverspaginator)
3. item: `AioPageIterator[ListGameServersOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGameServersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GameServerGroupName: str,
    SortOrder: SortOrderType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListGameServersOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListGameServersOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGameServersInputPaginateTypeDef = {  # (1)
    "GameServerGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGameServersInputPaginateTypeDef](./type_defs.md#listgameserversinputpaginatetypedef)
## ListLocationsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_locations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListLocations.html#GameLift.Paginator.ListLocations)

```python
# ListLocationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListLocationsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListLocationsPaginator = client.get_paginator("list_locations")  # (2)
    async for item in paginator.paginate(...):
        item: ListLocationsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListLocationsPaginator](./paginators.md#listlocationspaginator)
3. item: `AioPageIterator[ListLocationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLocationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[LocationFilterType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListLocationsOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[LocationFilterType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListLocationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLocationsInputPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLocationsInputPaginateTypeDef](./type_defs.md#listlocationsinputpaginatetypedef)
## ListScriptsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_scripts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/ListScripts.html#GameLift.Paginator.ListScripts)

```python
# ListScriptsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListScriptsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: ListScriptsPaginator = client.get_paginator("list_scripts")  # (2)
    async for item in paginator.paginate(...):
        item: ListScriptsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [ListScriptsPaginator](./paginators.md#listscriptspaginator)
3. item: `AioPageIterator[ListScriptsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListScriptsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListScriptsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListScriptsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListScriptsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScriptsInputPaginateTypeDef](./type_defs.md#listscriptsinputpaginatetypedef)
## SearchGameSessionsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("search_game_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/paginator/SearchGameSessions.html#GameLift.Paginator.SearchGameSessions)

```python
# SearchGameSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import SearchGameSessionsPaginator

session = get_session()
async with session.create_client("gamelift") as client:  # (1)
    paginator: SearchGameSessionsPaginator = client.get_paginator("search_game_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: SearchGameSessionsOutputTypeDef
        print(item)  # (3)
```

1. client: [GameLiftClient](./client.md)
2. paginator: [SearchGameSessionsPaginator](./paginators.md#searchgamesessionspaginator)
3. item: `AioPageIterator[SearchGameSessionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchGameSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetId: str = ...,
    AliasId: str = ...,
    Location: str = ...,
    FilterExpression: str = ...,
    SortExpression: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[SearchGameSessionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[SearchGameSessionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchGameSessionsInputPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchGameSessionsInputPaginateTypeDef](./type_defs.md#searchgamesessionsinputpaginatetypedef)
