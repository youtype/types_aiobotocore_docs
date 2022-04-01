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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeFleetAttributesPaginator = client.get_paginator("describe_fleet_attributes")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeFleetCapacityPaginator = client.get_paginator("describe_fleet_capacity")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeFleetEventsPaginator = client.get_paginator("describe_fleet_events")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeFleetUtilizationPaginator = client.get_paginator("describe_fleet_utilization")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeGameServerInstancesPaginator = client.get_paginator("describe_game_server_instances")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeGameSessionDetailsPaginator = client.get_paginator("describe_game_session_details")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeGameSessionQueuesPaginator = client.get_paginator("describe_game_session_queues")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeGameSessionsPaginator = client.get_paginator("describe_game_sessions")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeInstancesPaginator = client.get_paginator("describe_instances")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeMatchmakingConfigurationsPaginator = client.get_paginator("describe_matchmaking_configurations")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeMatchmakingRuleSetsPaginator = client.get_paginator("describe_matchmaking_rule_sets")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribePlayerSessionsPaginator = client.get_paginator("describe_player_sessions")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeScalingPoliciesPaginator = client.get_paginator("describe_scaling_policies")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListBuildsPaginator = client.get_paginator("list_builds")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListFleetsPaginator = client.get_paginator("list_fleets")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListGameServerGroupsPaginator = client.get_paginator("list_game_server_groups")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListScriptsPaginator = client.get_paginator("list_scripts")
```


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
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: SearchGameSessionsPaginator = client.get_paginator("search_game_sessions")
```


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
