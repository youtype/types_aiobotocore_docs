# Paginators

> [Index](../README.md) > [GameLift](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GameLift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
    type annotations stubs module [types-aiobotocore-gamelift](https://pypi.org/project/types-aiobotocore-gamelift/).

## DescribeFleetAttributesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_fleet_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetAttributes)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeFleetAttributesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFleetAttributesOutputTypeDef](./type_defs.md#describefleetattributesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFleetAttributesInputDescribeFleetAttributesPaginateTypeDef = {  # (1)
    "FleetIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetAttributesInputDescribeFleetAttributesPaginateTypeDef](./type_defs.md#describefleetattributesinputdescribefleetattributespaginatetypedef) 
## DescribeFleetCapacityPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_fleet_capacity")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetCapacity)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeFleetCapacityOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFleetCapacityOutputTypeDef](./type_defs.md#describefleetcapacityoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFleetCapacityInputDescribeFleetCapacityPaginateTypeDef = {  # (1)
    "FleetIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetCapacityInputDescribeFleetCapacityPaginateTypeDef](./type_defs.md#describefleetcapacityinputdescribefleetcapacitypaginatetypedef) 
## DescribeFleetEventsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_fleet_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetEvents)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    FleetId: str,
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeFleetEventsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFleetEventsOutputTypeDef](./type_defs.md#describefleeteventsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef](./type_defs.md#describefleeteventsinputdescribefleeteventspaginatetypedef) 
## DescribeFleetUtilizationPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_fleet_utilization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetUtilization)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeFleetUtilizationOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFleetUtilizationOutputTypeDef](./type_defs.md#describefleetutilizationoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef = {  # (1)
    "FleetIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef](./type_defs.md#describefleetutilizationinputdescribefleetutilizationpaginatetypedef) 
## DescribeGameServerInstancesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_game_server_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameServerInstances)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    GameServerGroupName: str,
    InstanceIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeGameServerInstancesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeGameServerInstancesOutputTypeDef](./type_defs.md#describegameserverinstancesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef = {  # (1)
    "GameServerGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef](./type_defs.md#describegameserverinstancesinputdescribegameserverinstancespaginatetypedef) 
## DescribeGameSessionDetailsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_game_session_details")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessionDetails)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    FleetId: str = ...,
    GameSessionId: str = ...,
    AliasId: str = ...,
    Location: str = ...,
    StatusFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeGameSessionDetailsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeGameSessionDetailsOutputTypeDef](./type_defs.md#describegamesessiondetailsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeGameSessionDetailsInputDescribeGameSessionDetailsPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGameSessionDetailsInputDescribeGameSessionDetailsPaginateTypeDef](./type_defs.md#describegamesessiondetailsinputdescribegamesessiondetailspaginatetypedef) 
## DescribeGameSessionQueuesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_game_session_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessionQueues)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeGameSessionQueuesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeGameSessionQueuesOutputTypeDef](./type_defs.md#describegamesessionqueuesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeGameSessionQueuesInputDescribeGameSessionQueuesPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGameSessionQueuesInputDescribeGameSessionQueuesPaginateTypeDef](./type_defs.md#describegamesessionqueuesinputdescribegamesessionqueuespaginatetypedef) 
## DescribeGameSessionsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_game_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessions)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    FleetId: str = ...,
    GameSessionId: str = ...,
    AliasId: str = ...,
    Location: str = ...,
    StatusFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeGameSessionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeGameSessionsOutputTypeDef](./type_defs.md#describegamesessionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeGameSessionsInputDescribeGameSessionsPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGameSessionsInputDescribeGameSessionsPaginateTypeDef](./type_defs.md#describegamesessionsinputdescribegamesessionspaginatetypedef) 
## DescribeInstancesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeInstances)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    FleetId: str,
    InstanceId: str = ...,
    Location: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeInstancesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeInstancesOutputTypeDef](./type_defs.md#describeinstancesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeInstancesInputDescribeInstancesPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstancesInputDescribeInstancesPaginateTypeDef](./type_defs.md#describeinstancesinputdescribeinstancespaginatetypedef) 
## DescribeMatchmakingConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_matchmaking_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeMatchmakingConfigurations)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    RuleSetName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeMatchmakingConfigurationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeMatchmakingConfigurationsOutputTypeDef](./type_defs.md#describematchmakingconfigurationsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef](./type_defs.md#describematchmakingconfigurationsinputdescribematchmakingconfigurationspaginatetypedef) 
## DescribeMatchmakingRuleSetsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_matchmaking_rule_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeMatchmakingRuleSets)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeMatchmakingRuleSetsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeMatchmakingRuleSetsOutputTypeDef](./type_defs.md#describematchmakingrulesetsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeMatchmakingRuleSetsInputDescribeMatchmakingRuleSetsPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMatchmakingRuleSetsInputDescribeMatchmakingRuleSetsPaginateTypeDef](./type_defs.md#describematchmakingrulesetsinputdescribematchmakingrulesetspaginatetypedef) 
## DescribePlayerSessionsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_player_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribePlayerSessions)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    GameSessionId: str = ...,
    PlayerId: str = ...,
    PlayerSessionId: str = ...,
    PlayerSessionStatusFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribePlayerSessionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribePlayerSessionsOutputTypeDef](./type_defs.md#describeplayersessionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribePlayerSessionsInputDescribePlayerSessionsPaginateTypeDef = {  # (1)
    "GameSessionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePlayerSessionsInputDescribePlayerSessionsPaginateTypeDef](./type_defs.md#describeplayersessionsinputdescribeplayersessionspaginatetypedef) 
## DescribeScalingPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("describe_scaling_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeScalingPolicies)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    FleetId: str,
    StatusFilter: ScalingStatusTypeType = ...,  # (1)
    Location: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeScalingPoliciesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ScalingStatusTypeType](./literals.md#scalingstatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeScalingPoliciesOutputTypeDef](./type_defs.md#describescalingpoliciesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef](./type_defs.md#describescalingpoliciesinputdescribescalingpoliciespaginatetypedef) 
## ListAliasesPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListAliases)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    RoutingStrategyType: RoutingStrategyTypeType = ...,  # (1)
    Name: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAliasesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RoutingStrategyTypeType](./literals.md#routingstrategytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListAliasesInputListAliasesPaginateTypeDef = {  # (1)
    "RoutingStrategyType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAliasesInputListAliasesPaginateTypeDef](./type_defs.md#listaliasesinputlistaliasespaginatetypedef) 
## ListBuildsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_builds")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListBuilds)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    Status: BuildStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListBuildsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: BuildStatusType](./literals.md#buildstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBuildsOutputTypeDef](./type_defs.md#listbuildsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBuildsInputListBuildsPaginateTypeDef = {  # (1)
    "Status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBuildsInputListBuildsPaginateTypeDef](./type_defs.md#listbuildsinputlistbuildspaginatetypedef) 
## ListFleetsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListFleets)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    BuildId: str = ...,
    ScriptId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFleetsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFleetsOutputTypeDef](./type_defs.md#listfleetsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListFleetsInputListFleetsPaginateTypeDef = {  # (1)
    "BuildId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFleetsInputListFleetsPaginateTypeDef](./type_defs.md#listfleetsinputlistfleetspaginatetypedef) 
## ListGameServerGroupsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_game_server_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListGameServerGroups)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGameServerGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGameServerGroupsOutputTypeDef](./type_defs.md#listgameservergroupsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef](./type_defs.md#listgameservergroupsinputlistgameservergroupspaginatetypedef) 
## ListGameServersPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_game_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListGameServers)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    GameServerGroupName: str,
    SortOrder: SortOrderType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListGameServersOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListGameServersOutputTypeDef](./type_defs.md#listgameserversoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListGameServersInputListGameServersPaginateTypeDef = {  # (1)
    "GameServerGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGameServersInputListGameServersPaginateTypeDef](./type_defs.md#listgameserversinputlistgameserverspaginatetypedef) 
## ListScriptsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("list_scripts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListScripts)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListScriptsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListScriptsOutputTypeDef](./type_defs.md#listscriptsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListScriptsInputListScriptsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScriptsInputListScriptsPaginateTypeDef](./type_defs.md#listscriptsinputlistscriptspaginatetypedef) 
## SearchGameSessionsPaginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator("search_game_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.SearchGameSessions)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    FleetId: str = ...,
    AliasId: str = ...,
    Location: str = ...,
    FilterExpression: str = ...,
    SortExpression: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[SearchGameSessionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SearchGameSessionsOutputTypeDef](./type_defs.md#searchgamesessionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: SearchGameSessionsInputSearchGameSessionsPaginateTypeDef = {  # (1)
    "FleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchGameSessionsInputSearchGameSessionsPaginateTypeDef](./type_defs.md#searchgamesessionsinputsearchgamesessionspaginatetypedef) 
