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
3. item: [:material-code-braces: DescribeFleetAttributesOutputTypeDef](./type_defs.md#describefleetattributesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFleetAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeFleetAttributesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFleetAttributesOutputTypeDef](./type_defs.md#describefleetattributesoutputtypedef) 


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
3. item: [:material-code-braces: DescribeFleetCapacityOutputTypeDef](./type_defs.md#describefleetcapacityoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFleetCapacityPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeFleetCapacityOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFleetCapacityOutputTypeDef](./type_defs.md#describefleetcapacityoutputtypedef) 


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
3. item: [:material-code-braces: DescribeFleetEventsOutputTypeDef](./type_defs.md#describefleeteventsoutputtypedef) 


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
) -> AioPageIterator[DescribeFleetEventsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFleetEventsOutputTypeDef](./type_defs.md#describefleeteventsoutputtypedef) 


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
3. item: [:material-code-braces: DescribeFleetUtilizationOutputTypeDef](./type_defs.md#describefleetutilizationoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFleetUtilizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeFleetUtilizationOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFleetUtilizationOutputTypeDef](./type_defs.md#describefleetutilizationoutputtypedef) 


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
3. item: [:material-code-braces: DescribeGameServerInstancesOutputTypeDef](./type_defs.md#describegameserverinstancesoutputtypedef) 


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
) -> AioPageIterator[DescribeGameServerInstancesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeGameServerInstancesOutputTypeDef](./type_defs.md#describegameserverinstancesoutputtypedef) 


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
3. item: [:material-code-braces: DescribeGameSessionDetailsOutputTypeDef](./type_defs.md#describegamesessiondetailsoutputtypedef) 


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
) -> AioPageIterator[DescribeGameSessionDetailsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeGameSessionDetailsOutputTypeDef](./type_defs.md#describegamesessiondetailsoutputtypedef) 


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
3. item: [:material-code-braces: DescribeGameSessionQueuesOutputTypeDef](./type_defs.md#describegamesessionqueuesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeGameSessionQueuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeGameSessionQueuesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeGameSessionQueuesOutputTypeDef](./type_defs.md#describegamesessionqueuesoutputtypedef) 


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
3. item: [:material-code-braces: DescribeGameSessionsOutputTypeDef](./type_defs.md#describegamesessionsoutputtypedef) 


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
) -> AioPageIterator[DescribeGameSessionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeGameSessionsOutputTypeDef](./type_defs.md#describegamesessionsoutputtypedef) 


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
3. item: [:material-code-braces: DescribeInstancesOutputTypeDef](./type_defs.md#describeinstancesoutputtypedef) 


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
) -> AioPageIterator[DescribeInstancesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeInstancesOutputTypeDef](./type_defs.md#describeinstancesoutputtypedef) 


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
3. item: [:material-code-braces: DescribeMatchmakingConfigurationsOutputTypeDef](./type_defs.md#describematchmakingconfigurationsoutputtypedef) 


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
) -> AioPageIterator[DescribeMatchmakingConfigurationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeMatchmakingConfigurationsOutputTypeDef](./type_defs.md#describematchmakingconfigurationsoutputtypedef) 


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
3. item: [:material-code-braces: DescribeMatchmakingRuleSetsOutputTypeDef](./type_defs.md#describematchmakingrulesetsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeMatchmakingRuleSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeMatchmakingRuleSetsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeMatchmakingRuleSetsOutputTypeDef](./type_defs.md#describematchmakingrulesetsoutputtypedef) 


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
3. item: [:material-code-braces: DescribePlayerSessionsOutputTypeDef](./type_defs.md#describeplayersessionsoutputtypedef) 


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
) -> AioPageIterator[DescribePlayerSessionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribePlayerSessionsOutputTypeDef](./type_defs.md#describeplayersessionsoutputtypedef) 


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
3. item: [:material-code-braces: DescribeScalingPoliciesOutputTypeDef](./type_defs.md#describescalingpoliciesoutputtypedef) 


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
) -> AioPageIterator[DescribeScalingPoliciesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ScalingStatusTypeType](./literals.md#scalingstatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeScalingPoliciesOutputTypeDef](./type_defs.md#describescalingpoliciesoutputtypedef) 


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
3. item: [:material-code-braces: ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef) 


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
) -> AioPageIterator[ListAliasesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RoutingStrategyTypeType](./literals.md#routingstrategytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef) 


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
3. item: [:material-code-braces: ListBuildsOutputTypeDef](./type_defs.md#listbuildsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBuildsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Status: BuildStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListBuildsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: BuildStatusType](./literals.md#buildstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBuildsOutputTypeDef](./type_defs.md#listbuildsoutputtypedef) 


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
3. item: [:material-code-braces: ListComputeOutputTypeDef](./type_defs.md#listcomputeoutputtypedef) 


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
) -> AioPageIterator[ListComputeOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListComputeInputStatusType](./literals.md#listcomputeinputstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListComputeOutputTypeDef](./type_defs.md#listcomputeoutputtypedef) 


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
3. item: [:material-code-braces: ListContainerFleetsOutputTypeDef](./type_defs.md#listcontainerfleetsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListContainerFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ContainerGroupDefinitionName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListContainerFleetsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListContainerFleetsOutputTypeDef](./type_defs.md#listcontainerfleetsoutputtypedef) 


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
3. item: [:material-code-braces: ListContainerGroupDefinitionVersionsOutputTypeDef](./type_defs.md#listcontainergroupdefinitionversionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListContainerGroupDefinitionVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListContainerGroupDefinitionVersionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListContainerGroupDefinitionVersionsOutputTypeDef](./type_defs.md#listcontainergroupdefinitionversionsoutputtypedef) 


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
3. item: [:material-code-braces: ListContainerGroupDefinitionsOutputTypeDef](./type_defs.md#listcontainergroupdefinitionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListContainerGroupDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ContainerGroupType: ContainerGroupTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListContainerGroupDefinitionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ContainerGroupTypeType](./literals.md#containergrouptypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListContainerGroupDefinitionsOutputTypeDef](./type_defs.md#listcontainergroupdefinitionsoutputtypedef) 


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
3. item: [:material-code-braces: ListFleetDeploymentsOutputTypeDef](./type_defs.md#listfleetdeploymentsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListFleetDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFleetDeploymentsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFleetDeploymentsOutputTypeDef](./type_defs.md#listfleetdeploymentsoutputtypedef) 


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
3. item: [:material-code-braces: ListFleetsOutputTypeDef](./type_defs.md#listfleetsoutputtypedef) 


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
) -> AioPageIterator[ListFleetsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFleetsOutputTypeDef](./type_defs.md#listfleetsoutputtypedef) 


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
3. item: [:material-code-braces: ListGameServerGroupsOutputTypeDef](./type_defs.md#listgameservergroupsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGameServerGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGameServerGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGameServerGroupsOutputTypeDef](./type_defs.md#listgameservergroupsoutputtypedef) 


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
3. item: [:material-code-braces: ListGameServersOutputTypeDef](./type_defs.md#listgameserversoutputtypedef) 


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
) -> AioPageIterator[ListGameServersOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListGameServersOutputTypeDef](./type_defs.md#listgameserversoutputtypedef) 


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
3. item: [:material-code-braces: ListLocationsOutputTypeDef](./type_defs.md#listlocationsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListLocationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[LocationFilterType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListLocationsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LocationFilterType](./literals.md#locationfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListLocationsOutputTypeDef](./type_defs.md#listlocationsoutputtypedef) 


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
3. item: [:material-code-braces: ListScriptsOutputTypeDef](./type_defs.md#listscriptsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListScriptsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListScriptsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListScriptsOutputTypeDef](./type_defs.md#listscriptsoutputtypedef) 


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
3. item: [:material-code-braces: SearchGameSessionsOutputTypeDef](./type_defs.md#searchgamesessionsoutputtypedef) 


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
) -> AioPageIterator[SearchGameSessionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SearchGameSessionsOutputTypeDef](./type_defs.md#searchgamesessionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchGameSessionsInputPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchGameSessionsInputPaginateTypeDef](./type_defs.md#searchgamesessionsinputpaginatetypedef) 
