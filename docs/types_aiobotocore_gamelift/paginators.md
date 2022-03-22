<a id="paginators-for-aiobotocore-gamelift-module"></a>

# Paginators for aiobotocore GameLift module

> [Index](../README.md) > [GameLift](./README.md) > Paginators

Auto-generated documentation for
[GameLift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
type annotations stubs module
[types-aiobotocore-gamelift](https://pypi.org/project/types-aiobotocore-gamelift/).

- [Paginators for aiobotocore GameLift module](#paginators-for-aiobotocore-gamelift-module)
  - [DescribeFleetAttributesPaginator](#describefleetattributespaginator)
  - [DescribeFleetCapacityPaginator](#describefleetcapacitypaginator)
  - [DescribeFleetEventsPaginator](#describefleeteventspaginator)
  - [DescribeFleetUtilizationPaginator](#describefleetutilizationpaginator)
  - [DescribeGameServerInstancesPaginator](#describegameserverinstancespaginator)
  - [DescribeGameSessionDetailsPaginator](#describegamesessiondetailspaginator)
  - [DescribeGameSessionQueuesPaginator](#describegamesessionqueuespaginator)
  - [DescribeGameSessionsPaginator](#describegamesessionspaginator)
  - [DescribeInstancesPaginator](#describeinstancespaginator)
  - [DescribeMatchmakingConfigurationsPaginator](#describematchmakingconfigurationspaginator)
  - [DescribeMatchmakingRuleSetsPaginator](#describematchmakingrulesetspaginator)
  - [DescribePlayerSessionsPaginator](#describeplayersessionspaginator)
  - [DescribeScalingPoliciesPaginator](#describescalingpoliciespaginator)
  - [ListAliasesPaginator](#listaliasespaginator)
  - [ListBuildsPaginator](#listbuildspaginator)
  - [ListFleetsPaginator](#listfleetspaginator)
  - [ListGameServerGroupsPaginator](#listgameservergroupspaginator)
  - [ListGameServersPaginator](#listgameserverspaginator)
  - [ListScriptsPaginator](#listscriptspaginator)
  - [SearchGameSessionsPaginator](#searchgamesessionspaginator)

<a id="describefleetattributespaginator"></a>

## DescribeFleetAttributesPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_fleet_attributes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeFleetAttributesPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeFleetAttributesPaginator = client.get_paginator("describe_fleet_attributes")
```

Boto3 documentation:
[GameLift.Paginator.DescribeFleetAttributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetAttributes)

Arguments for `DescribeFleetAttributesPaginator.paginate` method:

- `FleetIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeFleetAttributesPaginator.paginate` returns
`AsyncIterator`\[[DescribeFleetAttributesOutputTypeDef](./type_defs.md#describefleetattributesoutputtypedef)\].

<a id="describefleetcapacitypaginator"></a>

## DescribeFleetCapacityPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_fleet_capacity")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeFleetCapacityPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeFleetCapacityPaginator = client.get_paginator("describe_fleet_capacity")
```

Boto3 documentation:
[GameLift.Paginator.DescribeFleetCapacity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetCapacity)

Arguments for `DescribeFleetCapacityPaginator.paginate` method:

- `FleetIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeFleetCapacityPaginator.paginate` returns
`AsyncIterator`\[[DescribeFleetCapacityOutputTypeDef](./type_defs.md#describefleetcapacityoutputtypedef)\].

<a id="describefleeteventspaginator"></a>

## DescribeFleetEventsPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_fleet_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeFleetEventsPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeFleetEventsPaginator = client.get_paginator("describe_fleet_events")
```

Boto3 documentation:
[GameLift.Paginator.DescribeFleetEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetEvents)

Arguments for `DescribeFleetEventsPaginator.paginate` method:

- `FleetId`: `str` *(required)*
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeFleetEventsPaginator.paginate` returns
`AsyncIterator`\[[DescribeFleetEventsOutputTypeDef](./type_defs.md#describefleeteventsoutputtypedef)\].

<a id="describefleetutilizationpaginator"></a>

## DescribeFleetUtilizationPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_fleet_utilization")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeFleetUtilizationPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeFleetUtilizationPaginator = client.get_paginator("describe_fleet_utilization")
```

Boto3 documentation:
[GameLift.Paginator.DescribeFleetUtilization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetUtilization)

Arguments for `DescribeFleetUtilizationPaginator.paginate` method:

- `FleetIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeFleetUtilizationPaginator.paginate` returns
`AsyncIterator`\[[DescribeFleetUtilizationOutputTypeDef](./type_defs.md#describefleetutilizationoutputtypedef)\].

<a id="describegameserverinstancespaginator"></a>

## DescribeGameServerInstancesPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_game_server_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeGameServerInstancesPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeGameServerInstancesPaginator = client.get_paginator("describe_game_server_instances")
```

Boto3 documentation:
[GameLift.Paginator.DescribeGameServerInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameServerInstances)

Arguments for `DescribeGameServerInstancesPaginator.paginate` method:

- `GameServerGroupName`: `str` *(required)*
- `InstanceIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeGameServerInstancesPaginator.paginate` returns
`AsyncIterator`\[[DescribeGameServerInstancesOutputTypeDef](./type_defs.md#describegameserverinstancesoutputtypedef)\].

<a id="describegamesessiondetailspaginator"></a>

## DescribeGameSessionDetailsPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_game_session_details")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeGameSessionDetailsPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeGameSessionDetailsPaginator = client.get_paginator("describe_game_session_details")
```

Boto3 documentation:
[GameLift.Paginator.DescribeGameSessionDetails](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessionDetails)

Arguments for `DescribeGameSessionDetailsPaginator.paginate` method:

- `FleetId`: `str`
- `GameSessionId`: `str`
- `AliasId`: `str`
- `Location`: `str`
- `StatusFilter`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeGameSessionDetailsPaginator.paginate` returns
`AsyncIterator`\[[DescribeGameSessionDetailsOutputTypeDef](./type_defs.md#describegamesessiondetailsoutputtypedef)\].

<a id="describegamesessionqueuespaginator"></a>

## DescribeGameSessionQueuesPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_game_session_queues")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeGameSessionQueuesPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeGameSessionQueuesPaginator = client.get_paginator("describe_game_session_queues")
```

Boto3 documentation:
[GameLift.Paginator.DescribeGameSessionQueues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessionQueues)

Arguments for `DescribeGameSessionQueuesPaginator.paginate` method:

- `Names`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeGameSessionQueuesPaginator.paginate` returns
`AsyncIterator`\[[DescribeGameSessionQueuesOutputTypeDef](./type_defs.md#describegamesessionqueuesoutputtypedef)\].

<a id="describegamesessionspaginator"></a>

## DescribeGameSessionsPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_game_sessions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeGameSessionsPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeGameSessionsPaginator = client.get_paginator("describe_game_sessions")
```

Boto3 documentation:
[GameLift.Paginator.DescribeGameSessions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessions)

Arguments for `DescribeGameSessionsPaginator.paginate` method:

- `FleetId`: `str`
- `GameSessionId`: `str`
- `AliasId`: `str`
- `Location`: `str`
- `StatusFilter`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeGameSessionsPaginator.paginate` returns
`AsyncIterator`\[[DescribeGameSessionsOutputTypeDef](./type_defs.md#describegamesessionsoutputtypedef)\].

<a id="describeinstancespaginator"></a>

## DescribeInstancesPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeInstancesPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeInstancesPaginator = client.get_paginator("describe_instances")
```

Boto3 documentation:
[GameLift.Paginator.DescribeInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeInstances)

Arguments for `DescribeInstancesPaginator.paginate` method:

- `FleetId`: `str` *(required)*
- `InstanceId`: `str`
- `Location`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeInstancesPaginator.paginate` returns
`AsyncIterator`\[[DescribeInstancesOutputTypeDef](./type_defs.md#describeinstancesoutputtypedef)\].

<a id="describematchmakingconfigurationspaginator"></a>

## DescribeMatchmakingConfigurationsPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_matchmaking_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeMatchmakingConfigurationsPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeMatchmakingConfigurationsPaginator = client.get_paginator("describe_matchmaking_configurations")
```

Boto3 documentation:
[GameLift.Paginator.DescribeMatchmakingConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeMatchmakingConfigurations)

Arguments for `DescribeMatchmakingConfigurationsPaginator.paginate` method:

- `Names`: `Sequence`\[`str`\]
- `RuleSetName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeMatchmakingConfigurationsPaginator.paginate` returns
`AsyncIterator`\[[DescribeMatchmakingConfigurationsOutputTypeDef](./type_defs.md#describematchmakingconfigurationsoutputtypedef)\].

<a id="describematchmakingrulesetspaginator"></a>

## DescribeMatchmakingRuleSetsPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_matchmaking_rule_sets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeMatchmakingRuleSetsPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeMatchmakingRuleSetsPaginator = client.get_paginator("describe_matchmaking_rule_sets")
```

Boto3 documentation:
[GameLift.Paginator.DescribeMatchmakingRuleSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeMatchmakingRuleSets)

Arguments for `DescribeMatchmakingRuleSetsPaginator.paginate` method:

- `Names`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeMatchmakingRuleSetsPaginator.paginate` returns
`AsyncIterator`\[[DescribeMatchmakingRuleSetsOutputTypeDef](./type_defs.md#describematchmakingrulesetsoutputtypedef)\].

<a id="describeplayersessionspaginator"></a>

## DescribePlayerSessionsPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_player_sessions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribePlayerSessionsPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribePlayerSessionsPaginator = client.get_paginator("describe_player_sessions")
```

Boto3 documentation:
[GameLift.Paginator.DescribePlayerSessions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribePlayerSessions)

Arguments for `DescribePlayerSessionsPaginator.paginate` method:

- `GameSessionId`: `str`
- `PlayerId`: `str`
- `PlayerSessionId`: `str`
- `PlayerSessionStatusFilter`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribePlayerSessionsPaginator.paginate` returns
`AsyncIterator`\[[DescribePlayerSessionsOutputTypeDef](./type_defs.md#describeplayersessionsoutputtypedef)\].

<a id="describescalingpoliciespaginator"></a>

## DescribeScalingPoliciesPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("describe_scaling_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import DescribeScalingPoliciesPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: DescribeScalingPoliciesPaginator = client.get_paginator("describe_scaling_policies")
```

Boto3 documentation:
[GameLift.Paginator.DescribeScalingPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeScalingPolicies)

Arguments for `DescribeScalingPoliciesPaginator.paginate` method:

- `FleetId`: `str` *(required)*
- `StatusFilter`: [ScalingStatusTypeType](./literals.md#scalingstatustypetype)
- `Location`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeScalingPoliciesPaginator.paginate` returns
`AsyncIterator`\[[DescribeScalingPoliciesOutputTypeDef](./type_defs.md#describescalingpoliciesoutputtypedef)\].

<a id="listaliasespaginator"></a>

## ListAliasesPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("list_aliases")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListAliasesPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
```

Boto3 documentation:
[GameLift.Paginator.ListAliases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListAliases)

Arguments for `ListAliasesPaginator.paginate` method:

- `RoutingStrategyType`:
  [RoutingStrategyTypeType](./literals.md#routingstrategytypetype)
- `Name`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAliasesPaginator.paginate` returns
`AsyncIterator`\[[ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef)\].

<a id="listbuildspaginator"></a>

## ListBuildsPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("list_builds")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListBuildsPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListBuildsPaginator = client.get_paginator("list_builds")
```

Boto3 documentation:
[GameLift.Paginator.ListBuilds](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListBuilds)

Arguments for `ListBuildsPaginator.paginate` method:

- `Status`: [BuildStatusType](./literals.md#buildstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBuildsPaginator.paginate` returns
`AsyncIterator`\[[ListBuildsOutputTypeDef](./type_defs.md#listbuildsoutputtypedef)\].

<a id="listfleetspaginator"></a>

## ListFleetsPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("list_fleets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListFleetsPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListFleetsPaginator = client.get_paginator("list_fleets")
```

Boto3 documentation:
[GameLift.Paginator.ListFleets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListFleets)

Arguments for `ListFleetsPaginator.paginate` method:

- `BuildId`: `str`
- `ScriptId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFleetsPaginator.paginate` returns
`AsyncIterator`\[[ListFleetsOutputTypeDef](./type_defs.md#listfleetsoutputtypedef)\].

<a id="listgameservergroupspaginator"></a>

## ListGameServerGroupsPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("list_game_server_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListGameServerGroupsPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListGameServerGroupsPaginator = client.get_paginator("list_game_server_groups")
```

Boto3 documentation:
[GameLift.Paginator.ListGameServerGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListGameServerGroups)

Arguments for `ListGameServerGroupsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGameServerGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListGameServerGroupsOutputTypeDef](./type_defs.md#listgameservergroupsoutputtypedef)\].

<a id="listgameserverspaginator"></a>

## ListGameServersPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("list_game_servers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListGameServersPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")
```

Boto3 documentation:
[GameLift.Paginator.ListGameServers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListGameServers)

Arguments for `ListGameServersPaginator.paginate` method:

- `GameServerGroupName`: `str` *(required)*
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGameServersPaginator.paginate` returns
`AsyncIterator`\[[ListGameServersOutputTypeDef](./type_defs.md#listgameserversoutputtypedef)\].

<a id="listscriptspaginator"></a>

## ListScriptsPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("list_scripts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import ListScriptsPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: ListScriptsPaginator = client.get_paginator("list_scripts")
```

Boto3 documentation:
[GameLift.Paginator.ListScripts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListScripts)

Arguments for `ListScriptsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListScriptsPaginator.paginate` returns
`AsyncIterator`\[[ListScriptsOutputTypeDef](./type_defs.md#listscriptsoutputtypedef)\].

<a id="searchgamesessionspaginator"></a>

## SearchGameSessionsPaginator

Type annotations for
`session.create_client("gamelift").get_paginator("search_game_sessions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_gamelift.paginator import SearchGameSessionsPaginator

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
    paginator: SearchGameSessionsPaginator = client.get_paginator("search_game_sessions")
```

Boto3 documentation:
[GameLift.Paginator.SearchGameSessions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.SearchGameSessions)

Arguments for `SearchGameSessionsPaginator.paginate` method:

- `FleetId`: `str`
- `AliasId`: `str`
- `Location`: `str`
- `FilterExpression`: `str`
- `SortExpression`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchGameSessionsPaginator.paginate` returns
`AsyncIterator`\[[SearchGameSessionsOutputTypeDef](./type_defs.md#searchgamesessionsoutputtypedef)\].
