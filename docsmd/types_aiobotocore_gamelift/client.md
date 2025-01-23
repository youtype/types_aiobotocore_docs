# GameLiftClient

> [Index](../README.md) > [GameLift](./README.md) > GameLiftClient

!!! note ""

    Auto-generated documentation for [GameLift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#gamelift)
    type annotations stubs module [types-aiobotocore-gamelift](https://pypi.org/project/types-aiobotocore-gamelift/).

## GameLiftClient

Type annotations and code completion for `#!python session.create_client("gamelift")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client)

```python
# GameLiftClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_gamelift.client import GameLiftClient

session = get_session()
async with session.create_client("gamelift") as client:
    client: GameLiftClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("gamelift").exceptions` structure.

```python
# GameLiftClient.exceptions usage example

async with session.create_client("gamelift") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConflictException,
        client.FleetCapacityExceededException,
        client.GameSessionFullException,
        client.IdempotentParameterMismatchException,
        client.InternalServiceException,
        client.InvalidFleetStatusException,
        client.InvalidGameSessionStatusException,
        client.InvalidRequestException,
        client.LimitExceededException,
        client.NotFoundException,
        client.NotReadyException,
        client.OutOfCapacityException,
        client.TaggingFailedException,
        client.TerminalRoutingStrategyException,
        client.UnauthorizedException,
        client.UnsupportedRegionException,
    ) as e:
        print(e)
```

```python
# GameLiftClient usage type checking example

from types_aiobotocore_gamelift.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("gamelift").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("gamelift").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### accept\_match

Registers a player's acceptance or rejection of a proposed FlexMatch match.

Type annotations and code completion for `#!python session.create_client("gamelift").accept_match` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/accept_match.html)

```python
# accept_match method definition

await def accept_match(
    self,
    *,
    TicketId: str,
    PlayerIds: Sequence[str],
    AcceptanceType: AcceptanceTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: AcceptanceTypeType](./literals.md#acceptancetypetype) 


```python
# accept_match method usage example with argument unpacking

kwargs: AcceptMatchInputRequestTypeDef = {  # (1)
    "TicketId": ...,
    "PlayerIds": ...,
    "AcceptanceType": ...,
}

parent.accept_match(**kwargs)
```

1. See [:material-code-braces: AcceptMatchInputRequestTypeDef](./type_defs.md#acceptmatchinputrequesttypedef) 

### claim\_game\_server

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").claim_game_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/claim_game_server.html)

```python
# claim_game_server method definition

await def claim_game_server(
    self,
    *,
    GameServerGroupName: str,
    GameServerId: str = ...,
    GameServerData: str = ...,
    FilterOption: ClaimFilterOptionTypeDef = ...,  # (1)
) -> ClaimGameServerOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ClaimFilterOptionTypeDef](./type_defs.md#claimfilteroptiontypedef) 
2. See [:material-code-braces: ClaimGameServerOutputTypeDef](./type_defs.md#claimgameserveroutputtypedef) 


```python
# claim_game_server method usage example with argument unpacking

kwargs: ClaimGameServerInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
}

parent.claim_game_server(**kwargs)
```

1. See [:material-code-braces: ClaimGameServerInputRequestTypeDef](./type_defs.md#claimgameserverinputrequesttypedef) 

### create\_alias

Creates an alias for a fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").create_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_alias.html)

```python
# create_alias method definition

await def create_alias(
    self,
    *,
    Name: str,
    RoutingStrategy: RoutingStrategyTypeDef,  # (1)
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateAliasOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RoutingStrategyTypeDef](./type_defs.md#routingstrategytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateAliasOutputTypeDef](./type_defs.md#createaliasoutputtypedef) 


```python
# create_alias method usage example with argument unpacking

kwargs: CreateAliasInputRequestTypeDef = {  # (1)
    "Name": ...,
    "RoutingStrategy": ...,
}

parent.create_alias(**kwargs)
```

1. See [:material-code-braces: CreateAliasInputRequestTypeDef](./type_defs.md#createaliasinputrequesttypedef) 

### create\_build

Creates a new Amazon GameLift build resource for your game server binary files.

Type annotations and code completion for `#!python session.create_client("gamelift").create_build` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_build.html)

```python
# create_build method definition

await def create_build(
    self,
    *,
    Name: str = ...,
    Version: str = ...,
    StorageLocation: S3LocationTypeDef = ...,  # (1)
    OperatingSystem: OperatingSystemType = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    ServerSdkVersion: str = ...,
) -> CreateBuildOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateBuildOutputTypeDef](./type_defs.md#createbuildoutputtypedef) 


```python
# create_build method usage example with argument unpacking

kwargs: CreateBuildInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_build(**kwargs)
```

1. See [:material-code-braces: CreateBuildInputRequestTypeDef](./type_defs.md#createbuildinputrequesttypedef) 

### create\_container\_fleet

Creates a managed fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances
to host your containerized game servers.

Type annotations and code completion for `#!python session.create_client("gamelift").create_container_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_container_fleet.html)

```python
# create_container_fleet method definition

await def create_container_fleet(
    self,
    *,
    FleetRoleArn: str,
    Description: str = ...,
    GameServerContainerGroupDefinitionName: str = ...,
    PerInstanceContainerGroupDefinitionName: str = ...,
    InstanceConnectionPortRange: ConnectionPortRangeTypeDef = ...,  # (1)
    InstanceInboundPermissions: Sequence[IpPermissionTypeDef] = ...,  # (2)
    GameServerContainerGroupsPerInstance: int = ...,
    InstanceType: str = ...,
    BillingType: ContainerFleetBillingTypeType = ...,  # (3)
    Locations: Sequence[LocationConfigurationTypeDef] = ...,  # (4)
    MetricGroups: Sequence[str] = ...,
    NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,  # (5)
    GameSessionCreationLimitPolicy: GameSessionCreationLimitPolicyTypeDef = ...,  # (6)
    LogConfiguration: LogConfigurationTypeDef = ...,  # (7)
    Tags: Sequence[TagTypeDef] = ...,  # (8)
) -> CreateContainerFleetOutputTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: ConnectionPortRangeTypeDef](./type_defs.md#connectionportrangetypedef) 
2. See [:material-code-braces: IpPermissionTypeDef](./type_defs.md#ippermissiontypedef) 
3. See [:material-code-brackets: ContainerFleetBillingTypeType](./literals.md#containerfleetbillingtypetype) 
4. See [:material-code-braces: LocationConfigurationTypeDef](./type_defs.md#locationconfigurationtypedef) 
5. See [:material-code-brackets: ProtectionPolicyType](./literals.md#protectionpolicytype) 
6. See [:material-code-braces: GameSessionCreationLimitPolicyTypeDef](./type_defs.md#gamesessioncreationlimitpolicytypedef) 
7. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: CreateContainerFleetOutputTypeDef](./type_defs.md#createcontainerfleetoutputtypedef) 


```python
# create_container_fleet method usage example with argument unpacking

kwargs: CreateContainerFleetInputRequestTypeDef = {  # (1)
    "FleetRoleArn": ...,
}

parent.create_container_fleet(**kwargs)
```

1. See [:material-code-braces: CreateContainerFleetInputRequestTypeDef](./type_defs.md#createcontainerfleetinputrequesttypedef) 

### create\_container\_group\_definition

Creates a <code>ContainerGroupDefinition</code> that describes a set of
containers for hosting your game server with Amazon GameLift managed containers
hosting.

Type annotations and code completion for `#!python session.create_client("gamelift").create_container_group_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_container_group_definition.html)

```python
# create_container_group_definition method definition

await def create_container_group_definition(
    self,
    *,
    Name: str,
    TotalMemoryLimitMebibytes: int,
    TotalVcpuLimit: float,
    OperatingSystem: ContainerOperatingSystemType,  # (1)
    ContainerGroupType: ContainerGroupTypeType = ...,  # (2)
    GameServerContainerDefinition: GameServerContainerDefinitionInputTypeDef = ...,  # (3)
    SupportContainerDefinitions: Sequence[SupportContainerDefinitionInputTypeDef] = ...,  # (4)
    VersionDescription: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreateContainerGroupDefinitionOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ContainerOperatingSystemType](./literals.md#containeroperatingsystemtype) 
2. See [:material-code-brackets: ContainerGroupTypeType](./literals.md#containergrouptypetype) 
3. See [:material-code-braces: GameServerContainerDefinitionInputTypeDef](./type_defs.md#gameservercontainerdefinitioninputtypedef) 
4. See [:material-code-braces: SupportContainerDefinitionInputTypeDef](./type_defs.md#supportcontainerdefinitioninputtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateContainerGroupDefinitionOutputTypeDef](./type_defs.md#createcontainergroupdefinitionoutputtypedef) 


```python
# create_container_group_definition method usage example with argument unpacking

kwargs: CreateContainerGroupDefinitionInputRequestTypeDef = {  # (1)
    "Name": ...,
    "TotalMemoryLimitMebibytes": ...,
    "TotalVcpuLimit": ...,
    "OperatingSystem": ...,
}

parent.create_container_group_definition(**kwargs)
```

1. See [:material-code-braces: CreateContainerGroupDefinitionInputRequestTypeDef](./type_defs.md#createcontainergroupdefinitioninputrequesttypedef) 

### create\_fleet

Creates a fleet of compute resources to host your game servers.

Type annotations and code completion for `#!python session.create_client("gamelift").create_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_fleet.html)

```python
# create_fleet method definition

await def create_fleet(
    self,
    *,
    Name: str,
    Description: str = ...,
    BuildId: str = ...,
    ScriptId: str = ...,
    ServerLaunchPath: str = ...,
    ServerLaunchParameters: str = ...,
    LogPaths: Sequence[str] = ...,
    EC2InstanceType: EC2InstanceTypeType = ...,  # (1)
    EC2InboundPermissions: Sequence[IpPermissionTypeDef] = ...,  # (2)
    NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,  # (3)
    RuntimeConfiguration: RuntimeConfigurationTypeDef = ...,  # (4)
    ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,  # (5)
    MetricGroups: Sequence[str] = ...,
    PeerVpcAwsAccountId: str = ...,
    PeerVpcId: str = ...,
    FleetType: FleetTypeType = ...,  # (6)
    InstanceRoleArn: str = ...,
    CertificateConfiguration: CertificateConfigurationTypeDef = ...,  # (7)
    Locations: Sequence[LocationConfigurationTypeDef] = ...,  # (8)
    Tags: Sequence[TagTypeDef] = ...,  # (9)
    ComputeType: ComputeTypeType = ...,  # (10)
    AnywhereConfiguration: AnywhereConfigurationTypeDef = ...,  # (11)
    InstanceRoleCredentialsProvider: InstanceRoleCredentialsProviderType = ...,  # (12)
) -> CreateFleetOutputTypeDef:  # (13)
    ...
```

1. See [:material-code-brackets: EC2InstanceTypeType](./literals.md#ec2instancetypetype) 
2. See [:material-code-braces: IpPermissionTypeDef](./type_defs.md#ippermissiontypedef) 
3. See [:material-code-brackets: ProtectionPolicyType](./literals.md#protectionpolicytype) 
4. See [:material-code-braces: RuntimeConfigurationTypeDef](./type_defs.md#runtimeconfigurationtypedef) 
5. See [:material-code-braces: ResourceCreationLimitPolicyTypeDef](./type_defs.md#resourcecreationlimitpolicytypedef) 
6. See [:material-code-brackets: FleetTypeType](./literals.md#fleettypetype) 
7. See [:material-code-braces: CertificateConfigurationTypeDef](./type_defs.md#certificateconfigurationtypedef) 
8. See [:material-code-braces: LocationConfigurationTypeDef](./type_defs.md#locationconfigurationtypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
10. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
11. See [:material-code-braces: AnywhereConfigurationTypeDef](./type_defs.md#anywhereconfigurationtypedef) 
12. See [:material-code-brackets: InstanceRoleCredentialsProviderType](./literals.md#instancerolecredentialsprovidertype) 
13. See [:material-code-braces: CreateFleetOutputTypeDef](./type_defs.md#createfleetoutputtypedef) 


```python
# create_fleet method usage example with argument unpacking

kwargs: CreateFleetInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_fleet(**kwargs)
```

1. See [:material-code-braces: CreateFleetInputRequestTypeDef](./type_defs.md#createfleetinputrequesttypedef) 

### create\_fleet\_locations

Adds remote locations to an EC2 and begins populating the new locations with
instances.

Type annotations and code completion for `#!python session.create_client("gamelift").create_fleet_locations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_fleet_locations.html)

```python
# create_fleet_locations method definition

await def create_fleet_locations(
    self,
    *,
    FleetId: str,
    Locations: Sequence[LocationConfigurationTypeDef],  # (1)
) -> CreateFleetLocationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LocationConfigurationTypeDef](./type_defs.md#locationconfigurationtypedef) 
2. See [:material-code-braces: CreateFleetLocationsOutputTypeDef](./type_defs.md#createfleetlocationsoutputtypedef) 


```python
# create_fleet_locations method usage example with argument unpacking

kwargs: CreateFleetLocationsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "Locations": ...,
}

parent.create_fleet_locations(**kwargs)
```

1. See [:material-code-braces: CreateFleetLocationsInputRequestTypeDef](./type_defs.md#createfleetlocationsinputrequesttypedef) 

### create\_game\_server\_group

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").create_game_server_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_game_server_group.html)

```python
# create_game_server_group method definition

await def create_game_server_group(
    self,
    *,
    GameServerGroupName: str,
    RoleArn: str,
    MinSize: int,
    MaxSize: int,
    LaunchTemplate: LaunchTemplateSpecificationTypeDef,  # (1)
    InstanceDefinitions: Sequence[InstanceDefinitionTypeDef],  # (2)
    AutoScalingPolicy: GameServerGroupAutoScalingPolicyTypeDef = ...,  # (3)
    BalancingStrategy: BalancingStrategyType = ...,  # (4)
    GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,  # (5)
    VpcSubnets: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (6)
) -> CreateGameServerGroupOutputTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
2. See [:material-code-braces: InstanceDefinitionTypeDef](./type_defs.md#instancedefinitiontypedef) 
3. See [:material-code-braces: GameServerGroupAutoScalingPolicyTypeDef](./type_defs.md#gameservergroupautoscalingpolicytypedef) 
4. See [:material-code-brackets: BalancingStrategyType](./literals.md#balancingstrategytype) 
5. See [:material-code-brackets: GameServerProtectionPolicyType](./literals.md#gameserverprotectionpolicytype) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: CreateGameServerGroupOutputTypeDef](./type_defs.md#creategameservergroupoutputtypedef) 


```python
# create_game_server_group method usage example with argument unpacking

kwargs: CreateGameServerGroupInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
    "RoleArn": ...,
    "MinSize": ...,
    "MaxSize": ...,
    "LaunchTemplate": ...,
    "InstanceDefinitions": ...,
}

parent.create_game_server_group(**kwargs)
```

1. See [:material-code-braces: CreateGameServerGroupInputRequestTypeDef](./type_defs.md#creategameservergroupinputrequesttypedef) 

### create\_game\_session

Creates a multiplayer game session for players in a specific fleet location.

Type annotations and code completion for `#!python session.create_client("gamelift").create_game_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_game_session.html)

```python
# create_game_session method definition

await def create_game_session(
    self,
    *,
    MaximumPlayerSessionCount: int,
    FleetId: str = ...,
    AliasId: str = ...,
    Name: str = ...,
    GameProperties: Sequence[GamePropertyTypeDef] = ...,  # (1)
    CreatorId: str = ...,
    GameSessionId: str = ...,
    IdempotencyToken: str = ...,
    GameSessionData: str = ...,
    Location: str = ...,
) -> CreateGameSessionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
2. See [:material-code-braces: CreateGameSessionOutputTypeDef](./type_defs.md#creategamesessionoutputtypedef) 


```python
# create_game_session method usage example with argument unpacking

kwargs: CreateGameSessionInputRequestTypeDef = {  # (1)
    "MaximumPlayerSessionCount": ...,
}

parent.create_game_session(**kwargs)
```

1. See [:material-code-braces: CreateGameSessionInputRequestTypeDef](./type_defs.md#creategamesessioninputrequesttypedef) 

### create\_game\_session\_queue

Creates a placement queue that processes requests for new game sessions.

Type annotations and code completion for `#!python session.create_client("gamelift").create_game_session_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_game_session_queue.html)

```python
# create_game_session_queue method definition

await def create_game_session_queue(
    self,
    *,
    Name: str,
    TimeoutInSeconds: int = ...,
    PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,  # (1)
    Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,  # (2)
    FilterConfiguration: FilterConfigurationTypeDef = ...,  # (3)
    PriorityConfiguration: PriorityConfigurationTypeDef = ...,  # (4)
    CustomEventData: str = ...,
    NotificationTarget: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreateGameSessionQueueOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: PlayerLatencyPolicyTypeDef](./type_defs.md#playerlatencypolicytypedef) 
2. See [:material-code-braces: GameSessionQueueDestinationTypeDef](./type_defs.md#gamesessionqueuedestinationtypedef) 
3. See [:material-code-braces: FilterConfigurationTypeDef](./type_defs.md#filterconfigurationtypedef) 
4. See [:material-code-braces: PriorityConfigurationTypeDef](./type_defs.md#priorityconfigurationtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateGameSessionQueueOutputTypeDef](./type_defs.md#creategamesessionqueueoutputtypedef) 


```python
# create_game_session_queue method usage example with argument unpacking

kwargs: CreateGameSessionQueueInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_game_session_queue(**kwargs)
```

1. See [:material-code-braces: CreateGameSessionQueueInputRequestTypeDef](./type_defs.md#creategamesessionqueueinputrequesttypedef) 

### create\_location

Creates a custom location for use in an Anywhere fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").create_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_location.html)

```python
# create_location method definition

await def create_location(
    self,
    *,
    LocationName: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateLocationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateLocationOutputTypeDef](./type_defs.md#createlocationoutputtypedef) 


```python
# create_location method usage example with argument unpacking

kwargs: CreateLocationInputRequestTypeDef = {  # (1)
    "LocationName": ...,
}

parent.create_location(**kwargs)
```

1. See [:material-code-braces: CreateLocationInputRequestTypeDef](./type_defs.md#createlocationinputrequesttypedef) 

### create\_matchmaking\_configuration

Defines a new matchmaking configuration for use with FlexMatch.

Type annotations and code completion for `#!python session.create_client("gamelift").create_matchmaking_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_matchmaking_configuration.html)

```python
# create_matchmaking_configuration method definition

await def create_matchmaking_configuration(
    self,
    *,
    Name: str,
    RequestTimeoutSeconds: int,
    AcceptanceRequired: bool,
    RuleSetName: str,
    Description: str = ...,
    GameSessionQueueArns: Sequence[str] = ...,
    AcceptanceTimeoutSeconds: int = ...,
    NotificationTarget: str = ...,
    AdditionalPlayerCount: int = ...,
    CustomEventData: str = ...,
    GameProperties: Sequence[GamePropertyTypeDef] = ...,  # (1)
    GameSessionData: str = ...,
    BackfillMode: BackfillModeType = ...,  # (2)
    FlexMatchMode: FlexMatchModeType = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateMatchmakingConfigurationOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
2. See [:material-code-brackets: BackfillModeType](./literals.md#backfillmodetype) 
3. See [:material-code-brackets: FlexMatchModeType](./literals.md#flexmatchmodetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateMatchmakingConfigurationOutputTypeDef](./type_defs.md#creatematchmakingconfigurationoutputtypedef) 


```python
# create_matchmaking_configuration method usage example with argument unpacking

kwargs: CreateMatchmakingConfigurationInputRequestTypeDef = {  # (1)
    "Name": ...,
    "RequestTimeoutSeconds": ...,
    "AcceptanceRequired": ...,
    "RuleSetName": ...,
}

parent.create_matchmaking_configuration(**kwargs)
```

1. See [:material-code-braces: CreateMatchmakingConfigurationInputRequestTypeDef](./type_defs.md#creatematchmakingconfigurationinputrequesttypedef) 

### create\_matchmaking\_rule\_set

Creates a new rule set for FlexMatch matchmaking.

Type annotations and code completion for `#!python session.create_client("gamelift").create_matchmaking_rule_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_matchmaking_rule_set.html)

```python
# create_matchmaking_rule_set method definition

await def create_matchmaking_rule_set(
    self,
    *,
    Name: str,
    RuleSetBody: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateMatchmakingRuleSetOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateMatchmakingRuleSetOutputTypeDef](./type_defs.md#creatematchmakingrulesetoutputtypedef) 


```python
# create_matchmaking_rule_set method usage example with argument unpacking

kwargs: CreateMatchmakingRuleSetInputRequestTypeDef = {  # (1)
    "Name": ...,
    "RuleSetBody": ...,
}

parent.create_matchmaking_rule_set(**kwargs)
```

1. See [:material-code-braces: CreateMatchmakingRuleSetInputRequestTypeDef](./type_defs.md#creatematchmakingrulesetinputrequesttypedef) 

### create\_player\_session

Reserves an open player slot in a game session for a player.

Type annotations and code completion for `#!python session.create_client("gamelift").create_player_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_player_session.html)

```python
# create_player_session method definition

await def create_player_session(
    self,
    *,
    GameSessionId: str,
    PlayerId: str,
    PlayerData: str = ...,
) -> CreatePlayerSessionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePlayerSessionOutputTypeDef](./type_defs.md#createplayersessionoutputtypedef) 


```python
# create_player_session method usage example with argument unpacking

kwargs: CreatePlayerSessionInputRequestTypeDef = {  # (1)
    "GameSessionId": ...,
    "PlayerId": ...,
}

parent.create_player_session(**kwargs)
```

1. See [:material-code-braces: CreatePlayerSessionInputRequestTypeDef](./type_defs.md#createplayersessioninputrequesttypedef) 

### create\_player\_sessions

Reserves open slots in a game session for a group of players.

Type annotations and code completion for `#!python session.create_client("gamelift").create_player_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_player_sessions.html)

```python
# create_player_sessions method definition

await def create_player_sessions(
    self,
    *,
    GameSessionId: str,
    PlayerIds: Sequence[str],
    PlayerDataMap: Mapping[str, str] = ...,
) -> CreatePlayerSessionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePlayerSessionsOutputTypeDef](./type_defs.md#createplayersessionsoutputtypedef) 


```python
# create_player_sessions method usage example with argument unpacking

kwargs: CreatePlayerSessionsInputRequestTypeDef = {  # (1)
    "GameSessionId": ...,
    "PlayerIds": ...,
}

parent.create_player_sessions(**kwargs)
```

1. See [:material-code-braces: CreatePlayerSessionsInputRequestTypeDef](./type_defs.md#createplayersessionsinputrequesttypedef) 

### create\_script

Creates a new script record for your Realtime Servers script.

Type annotations and code completion for `#!python session.create_client("gamelift").create_script` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_script.html)

```python
# create_script method definition

await def create_script(
    self,
    *,
    Name: str = ...,
    Version: str = ...,
    StorageLocation: S3LocationTypeDef = ...,  # (1)
    ZipFile: BlobTypeDef = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateScriptOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateScriptOutputTypeDef](./type_defs.md#createscriptoutputtypedef) 


```python
# create_script method usage example with argument unpacking

kwargs: CreateScriptInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_script(**kwargs)
```

1. See [:material-code-braces: CreateScriptInputRequestTypeDef](./type_defs.md#createscriptinputrequesttypedef) 

### create\_vpc\_peering\_authorization

Requests authorization to create or delete a peer connection between the VPC
for your Amazon GameLift fleet and a virtual private cloud (VPC) in your Amazon
Web Services account.

Type annotations and code completion for `#!python session.create_client("gamelift").create_vpc_peering_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_vpc_peering_authorization.html)

```python
# create_vpc_peering_authorization method definition

await def create_vpc_peering_authorization(
    self,
    *,
    GameLiftAwsAccountId: str,
    PeerVpcId: str,
) -> CreateVpcPeeringAuthorizationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateVpcPeeringAuthorizationOutputTypeDef](./type_defs.md#createvpcpeeringauthorizationoutputtypedef) 


```python
# create_vpc_peering_authorization method usage example with argument unpacking

kwargs: CreateVpcPeeringAuthorizationInputRequestTypeDef = {  # (1)
    "GameLiftAwsAccountId": ...,
    "PeerVpcId": ...,
}

parent.create_vpc_peering_authorization(**kwargs)
```

1. See [:material-code-braces: CreateVpcPeeringAuthorizationInputRequestTypeDef](./type_defs.md#createvpcpeeringauthorizationinputrequesttypedef) 

### create\_vpc\_peering\_connection

Establishes a VPC peering connection between a virtual private cloud (VPC) in
an Amazon Web Services account with the VPC for your Amazon GameLift fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").create_vpc_peering_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/create_vpc_peering_connection.html)

```python
# create_vpc_peering_connection method definition

await def create_vpc_peering_connection(
    self,
    *,
    FleetId: str,
    PeerVpcAwsAccountId: str,
    PeerVpcId: str,
) -> Dict[str, Any]:
    ...
```



```python
# create_vpc_peering_connection method usage example with argument unpacking

kwargs: CreateVpcPeeringConnectionInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "PeerVpcAwsAccountId": ...,
    "PeerVpcId": ...,
}

parent.create_vpc_peering_connection(**kwargs)
```

1. See [:material-code-braces: CreateVpcPeeringConnectionInputRequestTypeDef](./type_defs.md#createvpcpeeringconnectioninputrequesttypedef) 

### delete\_alias

Deletes an alias.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_alias.html)

```python
# delete_alias method definition

await def delete_alias(
    self,
    *,
    AliasId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_alias method usage example with argument unpacking

kwargs: DeleteAliasInputRequestTypeDef = {  # (1)
    "AliasId": ...,
}

parent.delete_alias(**kwargs)
```

1. See [:material-code-braces: DeleteAliasInputRequestTypeDef](./type_defs.md#deletealiasinputrequesttypedef) 

### delete\_build

Deletes a build.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_build` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_build.html)

```python
# delete_build method definition

await def delete_build(
    self,
    *,
    BuildId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_build method usage example with argument unpacking

kwargs: DeleteBuildInputRequestTypeDef = {  # (1)
    "BuildId": ...,
}

parent.delete_build(**kwargs)
```

1. See [:material-code-braces: DeleteBuildInputRequestTypeDef](./type_defs.md#deletebuildinputrequesttypedef) 

### delete\_container\_fleet

Deletes all resources and information related to a container fleet and shuts
down currently running fleet instances, including those in remote locations.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_container_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_container_fleet.html)

```python
# delete_container_fleet method definition

await def delete_container_fleet(
    self,
    *,
    FleetId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_container_fleet method usage example with argument unpacking

kwargs: DeleteContainerFleetInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.delete_container_fleet(**kwargs)
```

1. See [:material-code-braces: DeleteContainerFleetInputRequestTypeDef](./type_defs.md#deletecontainerfleetinputrequesttypedef) 

### delete\_container\_group\_definition

Deletes a container group definition.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_container_group_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_container_group_definition.html)

```python
# delete_container_group_definition method definition

await def delete_container_group_definition(
    self,
    *,
    Name: str,
    VersionNumber: int = ...,
    VersionCountToRetain: int = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_container_group_definition method usage example with argument unpacking

kwargs: DeleteContainerGroupDefinitionInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_container_group_definition(**kwargs)
```

1. See [:material-code-braces: DeleteContainerGroupDefinitionInputRequestTypeDef](./type_defs.md#deletecontainergroupdefinitioninputrequesttypedef) 

### delete\_fleet

Deletes all resources and information related to a fleet and shuts down any
currently running fleet instances, including those in remote locations.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_fleet.html)

```python
# delete_fleet method definition

await def delete_fleet(
    self,
    *,
    FleetId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_fleet method usage example with argument unpacking

kwargs: DeleteFleetInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.delete_fleet(**kwargs)
```

1. See [:material-code-braces: DeleteFleetInputRequestTypeDef](./type_defs.md#deletefleetinputrequesttypedef) 

### delete\_fleet\_locations

Removes locations from a multi-location fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_fleet_locations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_fleet_locations.html)

```python
# delete_fleet_locations method definition

await def delete_fleet_locations(
    self,
    *,
    FleetId: str,
    Locations: Sequence[str],
) -> DeleteFleetLocationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFleetLocationsOutputTypeDef](./type_defs.md#deletefleetlocationsoutputtypedef) 


```python
# delete_fleet_locations method usage example with argument unpacking

kwargs: DeleteFleetLocationsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "Locations": ...,
}

parent.delete_fleet_locations(**kwargs)
```

1. See [:material-code-braces: DeleteFleetLocationsInputRequestTypeDef](./type_defs.md#deletefleetlocationsinputrequesttypedef) 

### delete\_game\_server\_group

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_game_server_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_game_server_group.html)

```python
# delete_game_server_group method definition

await def delete_game_server_group(
    self,
    *,
    GameServerGroupName: str,
    DeleteOption: GameServerGroupDeleteOptionType = ...,  # (1)
) -> DeleteGameServerGroupOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GameServerGroupDeleteOptionType](./literals.md#gameservergroupdeleteoptiontype) 
2. See [:material-code-braces: DeleteGameServerGroupOutputTypeDef](./type_defs.md#deletegameservergroupoutputtypedef) 


```python
# delete_game_server_group method usage example with argument unpacking

kwargs: DeleteGameServerGroupInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
}

parent.delete_game_server_group(**kwargs)
```

1. See [:material-code-braces: DeleteGameServerGroupInputRequestTypeDef](./type_defs.md#deletegameservergroupinputrequesttypedef) 

### delete\_game\_session\_queue

Deletes a game session queue.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_game_session_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_game_session_queue.html)

```python
# delete_game_session_queue method definition

await def delete_game_session_queue(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_game_session_queue method usage example with argument unpacking

kwargs: DeleteGameSessionQueueInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_game_session_queue(**kwargs)
```

1. See [:material-code-braces: DeleteGameSessionQueueInputRequestTypeDef](./type_defs.md#deletegamesessionqueueinputrequesttypedef) 

### delete\_location

Deletes a custom location.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_location.html)

```python
# delete_location method definition

await def delete_location(
    self,
    *,
    LocationName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_location method usage example with argument unpacking

kwargs: DeleteLocationInputRequestTypeDef = {  # (1)
    "LocationName": ...,
}

parent.delete_location(**kwargs)
```

1. See [:material-code-braces: DeleteLocationInputRequestTypeDef](./type_defs.md#deletelocationinputrequesttypedef) 

### delete\_matchmaking\_configuration

Permanently removes a FlexMatch matchmaking configuration.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_matchmaking_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_matchmaking_configuration.html)

```python
# delete_matchmaking_configuration method definition

await def delete_matchmaking_configuration(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_matchmaking_configuration method usage example with argument unpacking

kwargs: DeleteMatchmakingConfigurationInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_matchmaking_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteMatchmakingConfigurationInputRequestTypeDef](./type_defs.md#deletematchmakingconfigurationinputrequesttypedef) 

### delete\_matchmaking\_rule\_set

Deletes an existing matchmaking rule set.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_matchmaking_rule_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_matchmaking_rule_set.html)

```python
# delete_matchmaking_rule_set method definition

await def delete_matchmaking_rule_set(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_matchmaking_rule_set method usage example with argument unpacking

kwargs: DeleteMatchmakingRuleSetInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_matchmaking_rule_set(**kwargs)
```

1. See [:material-code-braces: DeleteMatchmakingRuleSetInputRequestTypeDef](./type_defs.md#deletematchmakingrulesetinputrequesttypedef) 

### delete\_scaling\_policy

Deletes a fleet scaling policy.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_scaling_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_scaling_policy.html)

```python
# delete_scaling_policy method definition

await def delete_scaling_policy(
    self,
    *,
    Name: str,
    FleetId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_scaling_policy method usage example with argument unpacking

kwargs: DeleteScalingPolicyInputRequestTypeDef = {  # (1)
    "Name": ...,
    "FleetId": ...,
}

parent.delete_scaling_policy(**kwargs)
```

1. See [:material-code-braces: DeleteScalingPolicyInputRequestTypeDef](./type_defs.md#deletescalingpolicyinputrequesttypedef) 

### delete\_script

Deletes a Realtime script.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_script` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_script.html)

```python
# delete_script method definition

await def delete_script(
    self,
    *,
    ScriptId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_script method usage example with argument unpacking

kwargs: DeleteScriptInputRequestTypeDef = {  # (1)
    "ScriptId": ...,
}

parent.delete_script(**kwargs)
```

1. See [:material-code-braces: DeleteScriptInputRequestTypeDef](./type_defs.md#deletescriptinputrequesttypedef) 

### delete\_vpc\_peering\_authorization

Cancels a pending VPC peering authorization for the specified VPC.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_vpc_peering_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_vpc_peering_authorization.html)

```python
# delete_vpc_peering_authorization method definition

await def delete_vpc_peering_authorization(
    self,
    *,
    GameLiftAwsAccountId: str,
    PeerVpcId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_vpc_peering_authorization method usage example with argument unpacking

kwargs: DeleteVpcPeeringAuthorizationInputRequestTypeDef = {  # (1)
    "GameLiftAwsAccountId": ...,
    "PeerVpcId": ...,
}

parent.delete_vpc_peering_authorization(**kwargs)
```

1. See [:material-code-braces: DeleteVpcPeeringAuthorizationInputRequestTypeDef](./type_defs.md#deletevpcpeeringauthorizationinputrequesttypedef) 

### delete\_vpc\_peering\_connection

Removes a VPC peering connection.

Type annotations and code completion for `#!python session.create_client("gamelift").delete_vpc_peering_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/delete_vpc_peering_connection.html)

```python
# delete_vpc_peering_connection method definition

await def delete_vpc_peering_connection(
    self,
    *,
    FleetId: str,
    VpcPeeringConnectionId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_vpc_peering_connection method usage example with argument unpacking

kwargs: DeleteVpcPeeringConnectionInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "VpcPeeringConnectionId": ...,
}

parent.delete_vpc_peering_connection(**kwargs)
```

1. See [:material-code-braces: DeleteVpcPeeringConnectionInputRequestTypeDef](./type_defs.md#deletevpcpeeringconnectioninputrequesttypedef) 

### deregister\_compute

Removes a compute resource from an Amazon GameLift Anywhere fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").deregister_compute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/deregister_compute.html)

```python
# deregister_compute method definition

await def deregister_compute(
    self,
    *,
    FleetId: str,
    ComputeName: str,
) -> Dict[str, Any]:
    ...
```



```python
# deregister_compute method usage example with argument unpacking

kwargs: DeregisterComputeInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "ComputeName": ...,
}

parent.deregister_compute(**kwargs)
```

1. See [:material-code-braces: DeregisterComputeInputRequestTypeDef](./type_defs.md#deregistercomputeinputrequesttypedef) 

### deregister\_game\_server

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").deregister_game_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/deregister_game_server.html)

```python
# deregister_game_server method definition

await def deregister_game_server(
    self,
    *,
    GameServerGroupName: str,
    GameServerId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# deregister_game_server method usage example with argument unpacking

kwargs: DeregisterGameServerInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
    "GameServerId": ...,
}

parent.deregister_game_server(**kwargs)
```

1. See [:material-code-braces: DeregisterGameServerInputRequestTypeDef](./type_defs.md#deregistergameserverinputrequesttypedef) 

### describe\_alias

Retrieves properties for an alias.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_alias.html)

```python
# describe_alias method definition

await def describe_alias(
    self,
    *,
    AliasId: str,
) -> DescribeAliasOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAliasOutputTypeDef](./type_defs.md#describealiasoutputtypedef) 


```python
# describe_alias method usage example with argument unpacking

kwargs: DescribeAliasInputRequestTypeDef = {  # (1)
    "AliasId": ...,
}

parent.describe_alias(**kwargs)
```

1. See [:material-code-braces: DescribeAliasInputRequestTypeDef](./type_defs.md#describealiasinputrequesttypedef) 

### describe\_build

Retrieves properties for a custom game build.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_build` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_build.html)

```python
# describe_build method definition

await def describe_build(
    self,
    *,
    BuildId: str,
) -> DescribeBuildOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBuildOutputTypeDef](./type_defs.md#describebuildoutputtypedef) 


```python
# describe_build method usage example with argument unpacking

kwargs: DescribeBuildInputRequestTypeDef = {  # (1)
    "BuildId": ...,
}

parent.describe_build(**kwargs)
```

1. See [:material-code-braces: DescribeBuildInputRequestTypeDef](./type_defs.md#describebuildinputrequesttypedef) 

### describe\_compute

Retrieves properties for a compute resource in an Amazon GameLift fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_compute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_compute.html)

```python
# describe_compute method definition

await def describe_compute(
    self,
    *,
    FleetId: str,
    ComputeName: str,
) -> DescribeComputeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeComputeOutputTypeDef](./type_defs.md#describecomputeoutputtypedef) 


```python
# describe_compute method usage example with argument unpacking

kwargs: DescribeComputeInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "ComputeName": ...,
}

parent.describe_compute(**kwargs)
```

1. See [:material-code-braces: DescribeComputeInputRequestTypeDef](./type_defs.md#describecomputeinputrequesttypedef) 

### describe\_container\_fleet

Retrieves the properties for a container fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_container_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_container_fleet.html)

```python
# describe_container_fleet method definition

await def describe_container_fleet(
    self,
    *,
    FleetId: str,
) -> DescribeContainerFleetOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeContainerFleetOutputTypeDef](./type_defs.md#describecontainerfleetoutputtypedef) 


```python
# describe_container_fleet method usage example with argument unpacking

kwargs: DescribeContainerFleetInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.describe_container_fleet(**kwargs)
```

1. See [:material-code-braces: DescribeContainerFleetInputRequestTypeDef](./type_defs.md#describecontainerfleetinputrequesttypedef) 

### describe\_container\_group\_definition

Retrieves the properties of a container group definition, including all
container definitions in the group.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_container_group_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_container_group_definition.html)

```python
# describe_container_group_definition method definition

await def describe_container_group_definition(
    self,
    *,
    Name: str,
    VersionNumber: int = ...,
) -> DescribeContainerGroupDefinitionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeContainerGroupDefinitionOutputTypeDef](./type_defs.md#describecontainergroupdefinitionoutputtypedef) 


```python
# describe_container_group_definition method usage example with argument unpacking

kwargs: DescribeContainerGroupDefinitionInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_container_group_definition(**kwargs)
```

1. See [:material-code-braces: DescribeContainerGroupDefinitionInputRequestTypeDef](./type_defs.md#describecontainergroupdefinitioninputrequesttypedef) 

### describe\_ec2\_instance\_limits

Retrieves the instance limits and current utilization for an Amazon Web
Services Region or location.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_ec2_instance_limits` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_ec2_instance_limits.html)

```python
# describe_ec2_instance_limits method definition

await def describe_ec2_instance_limits(
    self,
    *,
    EC2InstanceType: EC2InstanceTypeType = ...,  # (1)
    Location: str = ...,
) -> DescribeEC2InstanceLimitsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EC2InstanceTypeType](./literals.md#ec2instancetypetype) 
2. See [:material-code-braces: DescribeEC2InstanceLimitsOutputTypeDef](./type_defs.md#describeec2instancelimitsoutputtypedef) 


```python
# describe_ec2_instance_limits method usage example with argument unpacking

kwargs: DescribeEC2InstanceLimitsInputRequestTypeDef = {  # (1)
    "EC2InstanceType": ...,
}

parent.describe_ec2_instance_limits(**kwargs)
```

1. See [:material-code-braces: DescribeEC2InstanceLimitsInputRequestTypeDef](./type_defs.md#describeec2instancelimitsinputrequesttypedef) 

### describe\_fleet\_attributes

Retrieves core fleet-wide properties for fleets in an Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_fleet_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_fleet_attributes.html)

```python
# describe_fleet_attributes method definition

await def describe_fleet_attributes(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeFleetAttributesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetAttributesOutputTypeDef](./type_defs.md#describefleetattributesoutputtypedef) 


```python
# describe_fleet_attributes method usage example with argument unpacking

kwargs: DescribeFleetAttributesInputRequestTypeDef = {  # (1)
    "FleetIds": ...,
}

parent.describe_fleet_attributes(**kwargs)
```

1. See [:material-code-braces: DescribeFleetAttributesInputRequestTypeDef](./type_defs.md#describefleetattributesinputrequesttypedef) 

### describe\_fleet\_capacity

Retrieves the resource capacity settings for one or more fleets.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_fleet_capacity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_fleet_capacity.html)

```python
# describe_fleet_capacity method definition

await def describe_fleet_capacity(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeFleetCapacityOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetCapacityOutputTypeDef](./type_defs.md#describefleetcapacityoutputtypedef) 


```python
# describe_fleet_capacity method usage example with argument unpacking

kwargs: DescribeFleetCapacityInputRequestTypeDef = {  # (1)
    "FleetIds": ...,
}

parent.describe_fleet_capacity(**kwargs)
```

1. See [:material-code-braces: DescribeFleetCapacityInputRequestTypeDef](./type_defs.md#describefleetcapacityinputrequesttypedef) 

### describe\_fleet\_deployment

Retrieves information about a managed container fleet deployment.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_fleet_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_fleet_deployment.html)

```python
# describe_fleet_deployment method definition

await def describe_fleet_deployment(
    self,
    *,
    FleetId: str,
    DeploymentId: str = ...,
) -> DescribeFleetDeploymentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetDeploymentOutputTypeDef](./type_defs.md#describefleetdeploymentoutputtypedef) 


```python
# describe_fleet_deployment method usage example with argument unpacking

kwargs: DescribeFleetDeploymentInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.describe_fleet_deployment(**kwargs)
```

1. See [:material-code-braces: DescribeFleetDeploymentInputRequestTypeDef](./type_defs.md#describefleetdeploymentinputrequesttypedef) 

### describe\_fleet\_events

Retrieves entries from a fleet's event log.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_fleet_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_fleet_events.html)

```python
# describe_fleet_events method definition

await def describe_fleet_events(
    self,
    *,
    FleetId: str,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeFleetEventsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetEventsOutputTypeDef](./type_defs.md#describefleeteventsoutputtypedef) 


```python
# describe_fleet_events method usage example with argument unpacking

kwargs: DescribeFleetEventsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.describe_fleet_events(**kwargs)
```

1. See [:material-code-braces: DescribeFleetEventsInputRequestTypeDef](./type_defs.md#describefleeteventsinputrequesttypedef) 

### describe\_fleet\_location\_attributes

Retrieves information on a fleet's remote locations, including life-cycle
status and any suspended fleet activity.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_fleet_location_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_fleet_location_attributes.html)

```python
# describe_fleet_location_attributes method definition

await def describe_fleet_location_attributes(
    self,
    *,
    FleetId: str,
    Locations: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeFleetLocationAttributesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetLocationAttributesOutputTypeDef](./type_defs.md#describefleetlocationattributesoutputtypedef) 


```python
# describe_fleet_location_attributes method usage example with argument unpacking

kwargs: DescribeFleetLocationAttributesInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.describe_fleet_location_attributes(**kwargs)
```

1. See [:material-code-braces: DescribeFleetLocationAttributesInputRequestTypeDef](./type_defs.md#describefleetlocationattributesinputrequesttypedef) 

### describe\_fleet\_location\_capacity

Retrieves the resource capacity settings for a fleet location.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_fleet_location_capacity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_fleet_location_capacity.html)

```python
# describe_fleet_location_capacity method definition

await def describe_fleet_location_capacity(
    self,
    *,
    FleetId: str,
    Location: str,
) -> DescribeFleetLocationCapacityOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetLocationCapacityOutputTypeDef](./type_defs.md#describefleetlocationcapacityoutputtypedef) 


```python
# describe_fleet_location_capacity method usage example with argument unpacking

kwargs: DescribeFleetLocationCapacityInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "Location": ...,
}

parent.describe_fleet_location_capacity(**kwargs)
```

1. See [:material-code-braces: DescribeFleetLocationCapacityInputRequestTypeDef](./type_defs.md#describefleetlocationcapacityinputrequesttypedef) 

### describe\_fleet\_location\_utilization

Retrieves current usage data for a fleet location.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_fleet_location_utilization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_fleet_location_utilization.html)

```python
# describe_fleet_location_utilization method definition

await def describe_fleet_location_utilization(
    self,
    *,
    FleetId: str,
    Location: str,
) -> DescribeFleetLocationUtilizationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetLocationUtilizationOutputTypeDef](./type_defs.md#describefleetlocationutilizationoutputtypedef) 


```python
# describe_fleet_location_utilization method usage example with argument unpacking

kwargs: DescribeFleetLocationUtilizationInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "Location": ...,
}

parent.describe_fleet_location_utilization(**kwargs)
```

1. See [:material-code-braces: DescribeFleetLocationUtilizationInputRequestTypeDef](./type_defs.md#describefleetlocationutilizationinputrequesttypedef) 

### describe\_fleet\_port\_settings

Retrieves a fleet's inbound connection permissions.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_fleet_port_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_fleet_port_settings.html)

```python
# describe_fleet_port_settings method definition

await def describe_fleet_port_settings(
    self,
    *,
    FleetId: str,
    Location: str = ...,
) -> DescribeFleetPortSettingsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetPortSettingsOutputTypeDef](./type_defs.md#describefleetportsettingsoutputtypedef) 


```python
# describe_fleet_port_settings method usage example with argument unpacking

kwargs: DescribeFleetPortSettingsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.describe_fleet_port_settings(**kwargs)
```

1. See [:material-code-braces: DescribeFleetPortSettingsInputRequestTypeDef](./type_defs.md#describefleetportsettingsinputrequesttypedef) 

### describe\_fleet\_utilization

Retrieves utilization statistics for one or more fleets.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_fleet_utilization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_fleet_utilization.html)

```python
# describe_fleet_utilization method definition

await def describe_fleet_utilization(
    self,
    *,
    FleetIds: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeFleetUtilizationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFleetUtilizationOutputTypeDef](./type_defs.md#describefleetutilizationoutputtypedef) 


```python
# describe_fleet_utilization method usage example with argument unpacking

kwargs: DescribeFleetUtilizationInputRequestTypeDef = {  # (1)
    "FleetIds": ...,
}

parent.describe_fleet_utilization(**kwargs)
```

1. See [:material-code-braces: DescribeFleetUtilizationInputRequestTypeDef](./type_defs.md#describefleetutilizationinputrequesttypedef) 

### describe\_game\_server

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_game_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_game_server.html)

```python
# describe_game_server method definition

await def describe_game_server(
    self,
    *,
    GameServerGroupName: str,
    GameServerId: str,
) -> DescribeGameServerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGameServerOutputTypeDef](./type_defs.md#describegameserveroutputtypedef) 


```python
# describe_game_server method usage example with argument unpacking

kwargs: DescribeGameServerInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
    "GameServerId": ...,
}

parent.describe_game_server(**kwargs)
```

1. See [:material-code-braces: DescribeGameServerInputRequestTypeDef](./type_defs.md#describegameserverinputrequesttypedef) 

### describe\_game\_server\_group

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_game_server_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_game_server_group.html)

```python
# describe_game_server_group method definition

await def describe_game_server_group(
    self,
    *,
    GameServerGroupName: str,
) -> DescribeGameServerGroupOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGameServerGroupOutputTypeDef](./type_defs.md#describegameservergroupoutputtypedef) 


```python
# describe_game_server_group method usage example with argument unpacking

kwargs: DescribeGameServerGroupInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
}

parent.describe_game_server_group(**kwargs)
```

1. See [:material-code-braces: DescribeGameServerGroupInputRequestTypeDef](./type_defs.md#describegameservergroupinputrequesttypedef) 

### describe\_game\_server\_instances

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_game_server_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_game_server_instances.html)

```python
# describe_game_server_instances method definition

await def describe_game_server_instances(
    self,
    *,
    GameServerGroupName: str,
    InstanceIds: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeGameServerInstancesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGameServerInstancesOutputTypeDef](./type_defs.md#describegameserverinstancesoutputtypedef) 


```python
# describe_game_server_instances method usage example with argument unpacking

kwargs: DescribeGameServerInstancesInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
}

parent.describe_game_server_instances(**kwargs)
```

1. See [:material-code-braces: DescribeGameServerInstancesInputRequestTypeDef](./type_defs.md#describegameserverinstancesinputrequesttypedef) 

### describe\_game\_session\_details

Retrieves additional game session properties, including the game session
protection policy in force, a set of one or more game sessions in a specific
fleet location.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_game_session_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_game_session_details.html)

```python
# describe_game_session_details method definition

await def describe_game_session_details(
    self,
    *,
    FleetId: str = ...,
    GameSessionId: str = ...,
    AliasId: str = ...,
    Location: str = ...,
    StatusFilter: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeGameSessionDetailsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGameSessionDetailsOutputTypeDef](./type_defs.md#describegamesessiondetailsoutputtypedef) 


```python
# describe_game_session_details method usage example with argument unpacking

kwargs: DescribeGameSessionDetailsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.describe_game_session_details(**kwargs)
```

1. See [:material-code-braces: DescribeGameSessionDetailsInputRequestTypeDef](./type_defs.md#describegamesessiondetailsinputrequesttypedef) 

### describe\_game\_session\_placement

Retrieves information, including current status, about a game session placement
request.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_game_session_placement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_game_session_placement.html)

```python
# describe_game_session_placement method definition

await def describe_game_session_placement(
    self,
    *,
    PlacementId: str,
) -> DescribeGameSessionPlacementOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGameSessionPlacementOutputTypeDef](./type_defs.md#describegamesessionplacementoutputtypedef) 


```python
# describe_game_session_placement method usage example with argument unpacking

kwargs: DescribeGameSessionPlacementInputRequestTypeDef = {  # (1)
    "PlacementId": ...,
}

parent.describe_game_session_placement(**kwargs)
```

1. See [:material-code-braces: DescribeGameSessionPlacementInputRequestTypeDef](./type_defs.md#describegamesessionplacementinputrequesttypedef) 

### describe\_game\_session\_queues

Retrieves the properties for one or more game session queues.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_game_session_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_game_session_queues.html)

```python
# describe_game_session_queues method definition

await def describe_game_session_queues(
    self,
    *,
    Names: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeGameSessionQueuesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGameSessionQueuesOutputTypeDef](./type_defs.md#describegamesessionqueuesoutputtypedef) 


```python
# describe_game_session_queues method usage example with argument unpacking

kwargs: DescribeGameSessionQueuesInputRequestTypeDef = {  # (1)
    "Names": ...,
}

parent.describe_game_session_queues(**kwargs)
```

1. See [:material-code-braces: DescribeGameSessionQueuesInputRequestTypeDef](./type_defs.md#describegamesessionqueuesinputrequesttypedef) 

### describe\_game\_sessions

Retrieves a set of one or more game sessions in a specific fleet location.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_game_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_game_sessions.html)

```python
# describe_game_sessions method definition

await def describe_game_sessions(
    self,
    *,
    FleetId: str = ...,
    GameSessionId: str = ...,
    AliasId: str = ...,
    Location: str = ...,
    StatusFilter: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeGameSessionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGameSessionsOutputTypeDef](./type_defs.md#describegamesessionsoutputtypedef) 


```python
# describe_game_sessions method usage example with argument unpacking

kwargs: DescribeGameSessionsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.describe_game_sessions(**kwargs)
```

1. See [:material-code-braces: DescribeGameSessionsInputRequestTypeDef](./type_defs.md#describegamesessionsinputrequesttypedef) 

### describe\_instances

Retrieves information about the EC2 instances in an Amazon GameLift managed
fleet, including instance ID, connection data, and status.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_instances.html)

```python
# describe_instances method definition

await def describe_instances(
    self,
    *,
    FleetId: str,
    InstanceId: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
    Location: str = ...,
) -> DescribeInstancesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInstancesOutputTypeDef](./type_defs.md#describeinstancesoutputtypedef) 


```python
# describe_instances method usage example with argument unpacking

kwargs: DescribeInstancesInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.describe_instances(**kwargs)
```

1. See [:material-code-braces: DescribeInstancesInputRequestTypeDef](./type_defs.md#describeinstancesinputrequesttypedef) 

### describe\_matchmaking

Retrieves one or more matchmaking tickets.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_matchmaking` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_matchmaking.html)

```python
# describe_matchmaking method definition

await def describe_matchmaking(
    self,
    *,
    TicketIds: Sequence[str],
) -> DescribeMatchmakingOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMatchmakingOutputTypeDef](./type_defs.md#describematchmakingoutputtypedef) 


```python
# describe_matchmaking method usage example with argument unpacking

kwargs: DescribeMatchmakingInputRequestTypeDef = {  # (1)
    "TicketIds": ...,
}

parent.describe_matchmaking(**kwargs)
```

1. See [:material-code-braces: DescribeMatchmakingInputRequestTypeDef](./type_defs.md#describematchmakinginputrequesttypedef) 

### describe\_matchmaking\_configurations

Retrieves the details of FlexMatch matchmaking configurations.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_matchmaking_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_matchmaking_configurations.html)

```python
# describe_matchmaking_configurations method definition

await def describe_matchmaking_configurations(
    self,
    *,
    Names: Sequence[str] = ...,
    RuleSetName: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeMatchmakingConfigurationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMatchmakingConfigurationsOutputTypeDef](./type_defs.md#describematchmakingconfigurationsoutputtypedef) 


```python
# describe_matchmaking_configurations method usage example with argument unpacking

kwargs: DescribeMatchmakingConfigurationsInputRequestTypeDef = {  # (1)
    "Names": ...,
}

parent.describe_matchmaking_configurations(**kwargs)
```

1. See [:material-code-braces: DescribeMatchmakingConfigurationsInputRequestTypeDef](./type_defs.md#describematchmakingconfigurationsinputrequesttypedef) 

### describe\_matchmaking\_rule\_sets

Retrieves the details for FlexMatch matchmaking rule sets.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_matchmaking_rule_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_matchmaking_rule_sets.html)

```python
# describe_matchmaking_rule_sets method definition

await def describe_matchmaking_rule_sets(
    self,
    *,
    Names: Sequence[str] = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribeMatchmakingRuleSetsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMatchmakingRuleSetsOutputTypeDef](./type_defs.md#describematchmakingrulesetsoutputtypedef) 


```python
# describe_matchmaking_rule_sets method usage example with argument unpacking

kwargs: DescribeMatchmakingRuleSetsInputRequestTypeDef = {  # (1)
    "Names": ...,
}

parent.describe_matchmaking_rule_sets(**kwargs)
```

1. See [:material-code-braces: DescribeMatchmakingRuleSetsInputRequestTypeDef](./type_defs.md#describematchmakingrulesetsinputrequesttypedef) 

### describe\_player\_sessions

Retrieves properties for one or more player sessions.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_player_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_player_sessions.html)

```python
# describe_player_sessions method definition

await def describe_player_sessions(
    self,
    *,
    GameSessionId: str = ...,
    PlayerId: str = ...,
    PlayerSessionId: str = ...,
    PlayerSessionStatusFilter: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> DescribePlayerSessionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePlayerSessionsOutputTypeDef](./type_defs.md#describeplayersessionsoutputtypedef) 


```python
# describe_player_sessions method usage example with argument unpacking

kwargs: DescribePlayerSessionsInputRequestTypeDef = {  # (1)
    "GameSessionId": ...,
}

parent.describe_player_sessions(**kwargs)
```

1. See [:material-code-braces: DescribePlayerSessionsInputRequestTypeDef](./type_defs.md#describeplayersessionsinputrequesttypedef) 

### describe\_runtime\_configuration

Retrieves a fleet's runtime configuration settings.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_runtime_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_runtime_configuration.html)

```python
# describe_runtime_configuration method definition

await def describe_runtime_configuration(
    self,
    *,
    FleetId: str,
) -> DescribeRuntimeConfigurationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRuntimeConfigurationOutputTypeDef](./type_defs.md#describeruntimeconfigurationoutputtypedef) 


```python
# describe_runtime_configuration method usage example with argument unpacking

kwargs: DescribeRuntimeConfigurationInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.describe_runtime_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeRuntimeConfigurationInputRequestTypeDef](./type_defs.md#describeruntimeconfigurationinputrequesttypedef) 

### describe\_scaling\_policies

Retrieves all scaling policies applied to a fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_scaling_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_scaling_policies.html)

```python
# describe_scaling_policies method definition

await def describe_scaling_policies(
    self,
    *,
    FleetId: str,
    StatusFilter: ScalingStatusTypeType = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
    Location: str = ...,
) -> DescribeScalingPoliciesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScalingStatusTypeType](./literals.md#scalingstatustypetype) 
2. See [:material-code-braces: DescribeScalingPoliciesOutputTypeDef](./type_defs.md#describescalingpoliciesoutputtypedef) 


```python
# describe_scaling_policies method usage example with argument unpacking

kwargs: DescribeScalingPoliciesInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.describe_scaling_policies(**kwargs)
```

1. See [:material-code-braces: DescribeScalingPoliciesInputRequestTypeDef](./type_defs.md#describescalingpoliciesinputrequesttypedef) 

### describe\_script

Retrieves properties for a Realtime script.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_script` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_script.html)

```python
# describe_script method definition

await def describe_script(
    self,
    *,
    ScriptId: str,
) -> DescribeScriptOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeScriptOutputTypeDef](./type_defs.md#describescriptoutputtypedef) 


```python
# describe_script method usage example with argument unpacking

kwargs: DescribeScriptInputRequestTypeDef = {  # (1)
    "ScriptId": ...,
}

parent.describe_script(**kwargs)
```

1. See [:material-code-braces: DescribeScriptInputRequestTypeDef](./type_defs.md#describescriptinputrequesttypedef) 

### describe\_vpc\_peering\_authorizations

Retrieves valid VPC peering authorizations that are pending for the Amazon Web
Services account.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_vpc_peering_authorizations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_vpc_peering_authorizations.html)

```python
# describe_vpc_peering_authorizations method definition

await def describe_vpc_peering_authorizations(
    self,
) -> DescribeVpcPeeringAuthorizationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVpcPeeringAuthorizationsOutputTypeDef](./type_defs.md#describevpcpeeringauthorizationsoutputtypedef) 

### describe\_vpc\_peering\_connections

Retrieves information on VPC peering connections.

Type annotations and code completion for `#!python session.create_client("gamelift").describe_vpc_peering_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/describe_vpc_peering_connections.html)

```python
# describe_vpc_peering_connections method definition

await def describe_vpc_peering_connections(
    self,
    *,
    FleetId: str = ...,
) -> DescribeVpcPeeringConnectionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVpcPeeringConnectionsOutputTypeDef](./type_defs.md#describevpcpeeringconnectionsoutputtypedef) 


```python
# describe_vpc_peering_connections method usage example with argument unpacking

kwargs: DescribeVpcPeeringConnectionsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.describe_vpc_peering_connections(**kwargs)
```

1. See [:material-code-braces: DescribeVpcPeeringConnectionsInputRequestTypeDef](./type_defs.md#describevpcpeeringconnectionsinputrequesttypedef) 

### get\_compute\_access

Requests authorization to remotely connect to a hosting resource in a Amazon
GameLift managed fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").get_compute_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/get_compute_access.html)

```python
# get_compute_access method definition

await def get_compute_access(
    self,
    *,
    FleetId: str,
    ComputeName: str,
) -> GetComputeAccessOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComputeAccessOutputTypeDef](./type_defs.md#getcomputeaccessoutputtypedef) 


```python
# get_compute_access method usage example with argument unpacking

kwargs: GetComputeAccessInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "ComputeName": ...,
}

parent.get_compute_access(**kwargs)
```

1. See [:material-code-braces: GetComputeAccessInputRequestTypeDef](./type_defs.md#getcomputeaccessinputrequesttypedef) 

### get\_compute\_auth\_token

Requests an authentication token from Amazon GameLift for a compute resource in
an Amazon GameLift fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").get_compute_auth_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/get_compute_auth_token.html)

```python
# get_compute_auth_token method definition

await def get_compute_auth_token(
    self,
    *,
    FleetId: str,
    ComputeName: str,
) -> GetComputeAuthTokenOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComputeAuthTokenOutputTypeDef](./type_defs.md#getcomputeauthtokenoutputtypedef) 


```python
# get_compute_auth_token method usage example with argument unpacking

kwargs: GetComputeAuthTokenInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "ComputeName": ...,
}

parent.get_compute_auth_token(**kwargs)
```

1. See [:material-code-braces: GetComputeAuthTokenInputRequestTypeDef](./type_defs.md#getcomputeauthtokeninputrequesttypedef) 

### get\_game\_session\_log\_url

Retrieves the location of stored game session logs for a specified game session
on Amazon GameLift managed fleets.

Type annotations and code completion for `#!python session.create_client("gamelift").get_game_session_log_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/get_game_session_log_url.html)

```python
# get_game_session_log_url method definition

await def get_game_session_log_url(
    self,
    *,
    GameSessionId: str,
) -> GetGameSessionLogUrlOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGameSessionLogUrlOutputTypeDef](./type_defs.md#getgamesessionlogurloutputtypedef) 


```python
# get_game_session_log_url method usage example with argument unpacking

kwargs: GetGameSessionLogUrlInputRequestTypeDef = {  # (1)
    "GameSessionId": ...,
}

parent.get_game_session_log_url(**kwargs)
```

1. See [:material-code-braces: GetGameSessionLogUrlInputRequestTypeDef](./type_defs.md#getgamesessionlogurlinputrequesttypedef) 

### get\_instance\_access

Requests authorization to remotely connect to an instance in an Amazon GameLift
managed fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").get_instance_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/get_instance_access.html)

```python
# get_instance_access method definition

await def get_instance_access(
    self,
    *,
    FleetId: str,
    InstanceId: str,
) -> GetInstanceAccessOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInstanceAccessOutputTypeDef](./type_defs.md#getinstanceaccessoutputtypedef) 


```python
# get_instance_access method usage example with argument unpacking

kwargs: GetInstanceAccessInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "InstanceId": ...,
}

parent.get_instance_access(**kwargs)
```

1. See [:material-code-braces: GetInstanceAccessInputRequestTypeDef](./type_defs.md#getinstanceaccessinputrequesttypedef) 

### list\_aliases

Retrieves all aliases for this Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("gamelift").list_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_aliases.html)

```python
# list_aliases method definition

await def list_aliases(
    self,
    *,
    RoutingStrategyType: RoutingStrategyTypeType = ...,  # (1)
    Name: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> ListAliasesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoutingStrategyTypeType](./literals.md#routingstrategytypetype) 
2. See [:material-code-braces: ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef) 


```python
# list_aliases method usage example with argument unpacking

kwargs: ListAliasesInputRequestTypeDef = {  # (1)
    "RoutingStrategyType": ...,
}

parent.list_aliases(**kwargs)
```

1. See [:material-code-braces: ListAliasesInputRequestTypeDef](./type_defs.md#listaliasesinputrequesttypedef) 

### list\_builds

Retrieves build resources for all builds associated with the Amazon Web
Services account in use.

Type annotations and code completion for `#!python session.create_client("gamelift").list_builds` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_builds.html)

```python
# list_builds method definition

await def list_builds(
    self,
    *,
    Status: BuildStatusType = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> ListBuildsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: BuildStatusType](./literals.md#buildstatustype) 
2. See [:material-code-braces: ListBuildsOutputTypeDef](./type_defs.md#listbuildsoutputtypedef) 


```python
# list_builds method usage example with argument unpacking

kwargs: ListBuildsInputRequestTypeDef = {  # (1)
    "Status": ...,
}

parent.list_builds(**kwargs)
```

1. See [:material-code-braces: ListBuildsInputRequestTypeDef](./type_defs.md#listbuildsinputrequesttypedef) 

### list\_compute

Retrieves information on the compute resources in an Amazon GameLift fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").list_compute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_compute.html)

```python
# list_compute method definition

await def list_compute(
    self,
    *,
    FleetId: str,
    Location: str = ...,
    ContainerGroupDefinitionName: str = ...,
    ComputeStatus: ListComputeInputStatusType = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> ListComputeOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ListComputeInputStatusType](./literals.md#listcomputeinputstatustype) 
2. See [:material-code-braces: ListComputeOutputTypeDef](./type_defs.md#listcomputeoutputtypedef) 


```python
# list_compute method usage example with argument unpacking

kwargs: ListComputeInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.list_compute(**kwargs)
```

1. See [:material-code-braces: ListComputeInputRequestTypeDef](./type_defs.md#listcomputeinputrequesttypedef) 

### list\_container\_fleets

Retrieves a collection of container fleet resources in an Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("gamelift").list_container_fleets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_container_fleets.html)

```python
# list_container_fleets method definition

await def list_container_fleets(
    self,
    *,
    ContainerGroupDefinitionName: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> ListContainerFleetsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListContainerFleetsOutputTypeDef](./type_defs.md#listcontainerfleetsoutputtypedef) 


```python
# list_container_fleets method usage example with argument unpacking

kwargs: ListContainerFleetsInputRequestTypeDef = {  # (1)
    "ContainerGroupDefinitionName": ...,
}

parent.list_container_fleets(**kwargs)
```

1. See [:material-code-braces: ListContainerFleetsInputRequestTypeDef](./type_defs.md#listcontainerfleetsinputrequesttypedef) 

### list\_container\_group\_definition\_versions

Retrieves all versions of a container group definition.

Type annotations and code completion for `#!python session.create_client("gamelift").list_container_group_definition_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_container_group_definition_versions.html)

```python
# list_container_group_definition_versions method definition

await def list_container_group_definition_versions(
    self,
    *,
    Name: str,
    Limit: int = ...,
    NextToken: str = ...,
) -> ListContainerGroupDefinitionVersionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListContainerGroupDefinitionVersionsOutputTypeDef](./type_defs.md#listcontainergroupdefinitionversionsoutputtypedef) 


```python
# list_container_group_definition_versions method usage example with argument unpacking

kwargs: ListContainerGroupDefinitionVersionsInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.list_container_group_definition_versions(**kwargs)
```

1. See [:material-code-braces: ListContainerGroupDefinitionVersionsInputRequestTypeDef](./type_defs.md#listcontainergroupdefinitionversionsinputrequesttypedef) 

### list\_container\_group\_definitions

Retrieves container group definitions for the Amazon Web Services account and
Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("gamelift").list_container_group_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_container_group_definitions.html)

```python
# list_container_group_definitions method definition

await def list_container_group_definitions(
    self,
    *,
    ContainerGroupType: ContainerGroupTypeType = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> ListContainerGroupDefinitionsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContainerGroupTypeType](./literals.md#containergrouptypetype) 
2. See [:material-code-braces: ListContainerGroupDefinitionsOutputTypeDef](./type_defs.md#listcontainergroupdefinitionsoutputtypedef) 


```python
# list_container_group_definitions method usage example with argument unpacking

kwargs: ListContainerGroupDefinitionsInputRequestTypeDef = {  # (1)
    "ContainerGroupType": ...,
}

parent.list_container_group_definitions(**kwargs)
```

1. See [:material-code-braces: ListContainerGroupDefinitionsInputRequestTypeDef](./type_defs.md#listcontainergroupdefinitionsinputrequesttypedef) 

### list\_fleet\_deployments

Retrieves a collection of container fleet deployments in an Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("gamelift").list_fleet_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_fleet_deployments.html)

```python
# list_fleet_deployments method definition

await def list_fleet_deployments(
    self,
    *,
    FleetId: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> ListFleetDeploymentsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFleetDeploymentsOutputTypeDef](./type_defs.md#listfleetdeploymentsoutputtypedef) 


```python
# list_fleet_deployments method usage example with argument unpacking

kwargs: ListFleetDeploymentsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.list_fleet_deployments(**kwargs)
```

1. See [:material-code-braces: ListFleetDeploymentsInputRequestTypeDef](./type_defs.md#listfleetdeploymentsinputrequesttypedef) 

### list\_fleets

Retrieves a collection of fleet resources in an Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("gamelift").list_fleets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_fleets.html)

```python
# list_fleets method definition

await def list_fleets(
    self,
    *,
    BuildId: str = ...,
    ScriptId: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> ListFleetsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFleetsOutputTypeDef](./type_defs.md#listfleetsoutputtypedef) 


```python
# list_fleets method usage example with argument unpacking

kwargs: ListFleetsInputRequestTypeDef = {  # (1)
    "BuildId": ...,
}

parent.list_fleets(**kwargs)
```

1. See [:material-code-braces: ListFleetsInputRequestTypeDef](./type_defs.md#listfleetsinputrequesttypedef) 

### list\_game\_server\_groups

Lists a game server groups.

Type annotations and code completion for `#!python session.create_client("gamelift").list_game_server_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_game_server_groups.html)

```python
# list_game_server_groups method definition

await def list_game_server_groups(
    self,
    *,
    Limit: int = ...,
    NextToken: str = ...,
) -> ListGameServerGroupsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGameServerGroupsOutputTypeDef](./type_defs.md#listgameservergroupsoutputtypedef) 


```python
# list_game_server_groups method usage example with argument unpacking

kwargs: ListGameServerGroupsInputRequestTypeDef = {  # (1)
    "Limit": ...,
}

parent.list_game_server_groups(**kwargs)
```

1. See [:material-code-braces: ListGameServerGroupsInputRequestTypeDef](./type_defs.md#listgameservergroupsinputrequesttypedef) 

### list\_game\_servers

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").list_game_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_game_servers.html)

```python
# list_game_servers method definition

await def list_game_servers(
    self,
    *,
    GameServerGroupName: str,
    SortOrder: SortOrderType = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> ListGameServersOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: ListGameServersOutputTypeDef](./type_defs.md#listgameserversoutputtypedef) 


```python
# list_game_servers method usage example with argument unpacking

kwargs: ListGameServersInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
}

parent.list_game_servers(**kwargs)
```

1. See [:material-code-braces: ListGameServersInputRequestTypeDef](./type_defs.md#listgameserversinputrequesttypedef) 

### list\_locations

Lists all custom and Amazon Web Services locations.

Type annotations and code completion for `#!python session.create_client("gamelift").list_locations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_locations.html)

```python
# list_locations method definition

await def list_locations(
    self,
    *,
    Filters: Sequence[LocationFilterType] = ...,  # (1)
    Limit: int = ...,
    NextToken: str = ...,
) -> ListLocationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LocationFilterType](./literals.md#locationfiltertype) 
2. See [:material-code-braces: ListLocationsOutputTypeDef](./type_defs.md#listlocationsoutputtypedef) 


```python
# list_locations method usage example with argument unpacking

kwargs: ListLocationsInputRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_locations(**kwargs)
```

1. See [:material-code-braces: ListLocationsInputRequestTypeDef](./type_defs.md#listlocationsinputrequesttypedef) 

### list\_scripts

Retrieves script records for all Realtime scripts that are associated with the
Amazon Web Services account in use.

Type annotations and code completion for `#!python session.create_client("gamelift").list_scripts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_scripts.html)

```python
# list_scripts method definition

await def list_scripts(
    self,
    *,
    Limit: int = ...,
    NextToken: str = ...,
) -> ListScriptsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListScriptsOutputTypeDef](./type_defs.md#listscriptsoutputtypedef) 


```python
# list_scripts method usage example with argument unpacking

kwargs: ListScriptsInputRequestTypeDef = {  # (1)
    "Limit": ...,
}

parent.list_scripts(**kwargs)
```

1. See [:material-code-braces: ListScriptsInputRequestTypeDef](./type_defs.md#listscriptsinputrequesttypedef) 

### list\_tags\_for\_resource

Retrieves all tags assigned to a Amazon GameLift resource.

Type annotations and code completion for `#!python session.create_client("gamelift").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_scaling\_policy

Creates or updates a scaling policy for a fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").put_scaling_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/put_scaling_policy.html)

```python
# put_scaling_policy method definition

await def put_scaling_policy(
    self,
    *,
    Name: str,
    FleetId: str,
    MetricName: MetricNameType,  # (1)
    ScalingAdjustment: int = ...,
    ScalingAdjustmentType: ScalingAdjustmentTypeType = ...,  # (2)
    Threshold: float = ...,
    ComparisonOperator: ComparisonOperatorTypeType = ...,  # (3)
    EvaluationPeriods: int = ...,
    PolicyType: PolicyTypeType = ...,  # (4)
    TargetConfiguration: TargetConfigurationTypeDef = ...,  # (5)
) -> PutScalingPolicyOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: MetricNameType](./literals.md#metricnametype) 
2. See [:material-code-brackets: ScalingAdjustmentTypeType](./literals.md#scalingadjustmenttypetype) 
3. See [:material-code-brackets: ComparisonOperatorTypeType](./literals.md#comparisonoperatortypetype) 
4. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
5. See [:material-code-braces: TargetConfigurationTypeDef](./type_defs.md#targetconfigurationtypedef) 
6. See [:material-code-braces: PutScalingPolicyOutputTypeDef](./type_defs.md#putscalingpolicyoutputtypedef) 


```python
# put_scaling_policy method usage example with argument unpacking

kwargs: PutScalingPolicyInputRequestTypeDef = {  # (1)
    "Name": ...,
    "FleetId": ...,
    "MetricName": ...,
}

parent.put_scaling_policy(**kwargs)
```

1. See [:material-code-braces: PutScalingPolicyInputRequestTypeDef](./type_defs.md#putscalingpolicyinputrequesttypedef) 

### register\_compute

Registers a compute resource in an Amazon GameLift Anywhere fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").register_compute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/register_compute.html)

```python
# register_compute method definition

await def register_compute(
    self,
    *,
    FleetId: str,
    ComputeName: str,
    CertificatePath: str = ...,
    DnsName: str = ...,
    IpAddress: str = ...,
    Location: str = ...,
) -> RegisterComputeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterComputeOutputTypeDef](./type_defs.md#registercomputeoutputtypedef) 


```python
# register_compute method usage example with argument unpacking

kwargs: RegisterComputeInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "ComputeName": ...,
}

parent.register_compute(**kwargs)
```

1. See [:material-code-braces: RegisterComputeInputRequestTypeDef](./type_defs.md#registercomputeinputrequesttypedef) 

### register\_game\_server

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").register_game_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/register_game_server.html)

```python
# register_game_server method definition

await def register_game_server(
    self,
    *,
    GameServerGroupName: str,
    GameServerId: str,
    InstanceId: str,
    ConnectionInfo: str = ...,
    GameServerData: str = ...,
) -> RegisterGameServerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterGameServerOutputTypeDef](./type_defs.md#registergameserveroutputtypedef) 


```python
# register_game_server method usage example with argument unpacking

kwargs: RegisterGameServerInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
    "GameServerId": ...,
    "InstanceId": ...,
}

parent.register_game_server(**kwargs)
```

1. See [:material-code-braces: RegisterGameServerInputRequestTypeDef](./type_defs.md#registergameserverinputrequesttypedef) 

### request\_upload\_credentials

Retrieves a fresh set of credentials for use when uploading a new set of game
build files to Amazon GameLift's Amazon S3.

Type annotations and code completion for `#!python session.create_client("gamelift").request_upload_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/request_upload_credentials.html)

```python
# request_upload_credentials method definition

await def request_upload_credentials(
    self,
    *,
    BuildId: str,
) -> RequestUploadCredentialsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RequestUploadCredentialsOutputTypeDef](./type_defs.md#requestuploadcredentialsoutputtypedef) 


```python
# request_upload_credentials method usage example with argument unpacking

kwargs: RequestUploadCredentialsInputRequestTypeDef = {  # (1)
    "BuildId": ...,
}

parent.request_upload_credentials(**kwargs)
```

1. See [:material-code-braces: RequestUploadCredentialsInputRequestTypeDef](./type_defs.md#requestuploadcredentialsinputrequesttypedef) 

### resolve\_alias

Attempts to retrieve a fleet ID that is associated with an alias.

Type annotations and code completion for `#!python session.create_client("gamelift").resolve_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/resolve_alias.html)

```python
# resolve_alias method definition

await def resolve_alias(
    self,
    *,
    AliasId: str,
) -> ResolveAliasOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResolveAliasOutputTypeDef](./type_defs.md#resolvealiasoutputtypedef) 


```python
# resolve_alias method usage example with argument unpacking

kwargs: ResolveAliasInputRequestTypeDef = {  # (1)
    "AliasId": ...,
}

parent.resolve_alias(**kwargs)
```

1. See [:material-code-braces: ResolveAliasInputRequestTypeDef](./type_defs.md#resolvealiasinputrequesttypedef) 

### resume\_game\_server\_group

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").resume_game_server_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/resume_game_server_group.html)

```python
# resume_game_server_group method definition

await def resume_game_server_group(
    self,
    *,
    GameServerGroupName: str,
    ResumeActions: Sequence[GameServerGroupActionType],  # (1)
) -> ResumeGameServerGroupOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GameServerGroupActionType](./literals.md#gameservergroupactiontype) 
2. See [:material-code-braces: ResumeGameServerGroupOutputTypeDef](./type_defs.md#resumegameservergroupoutputtypedef) 


```python
# resume_game_server_group method usage example with argument unpacking

kwargs: ResumeGameServerGroupInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
    "ResumeActions": ...,
}

parent.resume_game_server_group(**kwargs)
```

1. See [:material-code-braces: ResumeGameServerGroupInputRequestTypeDef](./type_defs.md#resumegameservergroupinputrequesttypedef) 

### search\_game\_sessions

Retrieves all active game sessions that match a set of search criteria and
sorts them into a specified order.

Type annotations and code completion for `#!python session.create_client("gamelift").search_game_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/search_game_sessions.html)

```python
# search_game_sessions method definition

await def search_game_sessions(
    self,
    *,
    FleetId: str = ...,
    AliasId: str = ...,
    Location: str = ...,
    FilterExpression: str = ...,
    SortExpression: str = ...,
    Limit: int = ...,
    NextToken: str = ...,
) -> SearchGameSessionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SearchGameSessionsOutputTypeDef](./type_defs.md#searchgamesessionsoutputtypedef) 


```python
# search_game_sessions method usage example with argument unpacking

kwargs: SearchGameSessionsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.search_game_sessions(**kwargs)
```

1. See [:material-code-braces: SearchGameSessionsInputRequestTypeDef](./type_defs.md#searchgamesessionsinputrequesttypedef) 

### start\_fleet\_actions

Resumes certain types of activity on fleet instances that were suspended with
<a
href="https://docs.aws.amazon.com/gamelift/latest/apireference/API_StopFleetActions.html">StopFleetActions</a>.

Type annotations and code completion for `#!python session.create_client("gamelift").start_fleet_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/start_fleet_actions.html)

```python
# start_fleet_actions method definition

await def start_fleet_actions(
    self,
    *,
    FleetId: str,
    Actions: Sequence[FleetActionType],  # (1)
    Location: str = ...,
) -> StartFleetActionsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FleetActionType](./literals.md#fleetactiontype) 
2. See [:material-code-braces: StartFleetActionsOutputTypeDef](./type_defs.md#startfleetactionsoutputtypedef) 


```python
# start_fleet_actions method usage example with argument unpacking

kwargs: StartFleetActionsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "Actions": ...,
}

parent.start_fleet_actions(**kwargs)
```

1. See [:material-code-braces: StartFleetActionsInputRequestTypeDef](./type_defs.md#startfleetactionsinputrequesttypedef) 

### start\_game\_session\_placement

Makes a request to start a new game session using a game session queue.

Type annotations and code completion for `#!python session.create_client("gamelift").start_game_session_placement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/start_game_session_placement.html)

```python
# start_game_session_placement method definition

await def start_game_session_placement(
    self,
    *,
    PlacementId: str,
    GameSessionQueueName: str,
    MaximumPlayerSessionCount: int,
    GameProperties: Sequence[GamePropertyTypeDef] = ...,  # (1)
    GameSessionName: str = ...,
    PlayerLatencies: Sequence[PlayerLatencyTypeDef] = ...,  # (2)
    DesiredPlayerSessions: Sequence[DesiredPlayerSessionTypeDef] = ...,  # (3)
    GameSessionData: str = ...,
    PriorityConfigurationOverride: PriorityConfigurationOverrideTypeDef = ...,  # (4)
) -> StartGameSessionPlacementOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
2. See [:material-code-braces: PlayerLatencyTypeDef](./type_defs.md#playerlatencytypedef) 
3. See [:material-code-braces: DesiredPlayerSessionTypeDef](./type_defs.md#desiredplayersessiontypedef) 
4. See [:material-code-braces: PriorityConfigurationOverrideTypeDef](./type_defs.md#priorityconfigurationoverridetypedef) 
5. See [:material-code-braces: StartGameSessionPlacementOutputTypeDef](./type_defs.md#startgamesessionplacementoutputtypedef) 


```python
# start_game_session_placement method usage example with argument unpacking

kwargs: StartGameSessionPlacementInputRequestTypeDef = {  # (1)
    "PlacementId": ...,
    "GameSessionQueueName": ...,
    "MaximumPlayerSessionCount": ...,
}

parent.start_game_session_placement(**kwargs)
```

1. See [:material-code-braces: StartGameSessionPlacementInputRequestTypeDef](./type_defs.md#startgamesessionplacementinputrequesttypedef) 

### start\_match\_backfill

Finds new players to fill open slots in currently running game sessions.

Type annotations and code completion for `#!python session.create_client("gamelift").start_match_backfill` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/start_match_backfill.html)

```python
# start_match_backfill method definition

await def start_match_backfill(
    self,
    *,
    ConfigurationName: str,
    Players: Sequence[PlayerUnionTypeDef],  # (1)
    TicketId: str = ...,
    GameSessionArn: str = ...,
) -> StartMatchBackfillOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PlayerTypeDef](./type_defs.md#playertypedef) [:material-code-braces: PlayerOutputTypeDef](./type_defs.md#playeroutputtypedef) 
2. See [:material-code-braces: StartMatchBackfillOutputTypeDef](./type_defs.md#startmatchbackfilloutputtypedef) 


```python
# start_match_backfill method usage example with argument unpacking

kwargs: StartMatchBackfillInputRequestTypeDef = {  # (1)
    "ConfigurationName": ...,
    "Players": ...,
}

parent.start_match_backfill(**kwargs)
```

1. See [:material-code-braces: StartMatchBackfillInputRequestTypeDef](./type_defs.md#startmatchbackfillinputrequesttypedef) 

### start\_matchmaking

Uses FlexMatch to create a game match for a group of players based on custom
matchmaking rules.

Type annotations and code completion for `#!python session.create_client("gamelift").start_matchmaking` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/start_matchmaking.html)

```python
# start_matchmaking method definition

await def start_matchmaking(
    self,
    *,
    ConfigurationName: str,
    Players: Sequence[PlayerTypeDef],  # (1)
    TicketId: str = ...,
) -> StartMatchmakingOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PlayerTypeDef](./type_defs.md#playertypedef) 
2. See [:material-code-braces: StartMatchmakingOutputTypeDef](./type_defs.md#startmatchmakingoutputtypedef) 


```python
# start_matchmaking method usage example with argument unpacking

kwargs: StartMatchmakingInputRequestTypeDef = {  # (1)
    "ConfigurationName": ...,
    "Players": ...,
}

parent.start_matchmaking(**kwargs)
```

1. See [:material-code-braces: StartMatchmakingInputRequestTypeDef](./type_defs.md#startmatchmakinginputrequesttypedef) 

### stop\_fleet\_actions

Suspends certain types of activity in a fleet location.

Type annotations and code completion for `#!python session.create_client("gamelift").stop_fleet_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/stop_fleet_actions.html)

```python
# stop_fleet_actions method definition

await def stop_fleet_actions(
    self,
    *,
    FleetId: str,
    Actions: Sequence[FleetActionType],  # (1)
    Location: str = ...,
) -> StopFleetActionsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FleetActionType](./literals.md#fleetactiontype) 
2. See [:material-code-braces: StopFleetActionsOutputTypeDef](./type_defs.md#stopfleetactionsoutputtypedef) 


```python
# stop_fleet_actions method usage example with argument unpacking

kwargs: StopFleetActionsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "Actions": ...,
}

parent.stop_fleet_actions(**kwargs)
```

1. See [:material-code-braces: StopFleetActionsInputRequestTypeDef](./type_defs.md#stopfleetactionsinputrequesttypedef) 

### stop\_game\_session\_placement

Cancels a game session placement that is in <code>PENDING</code> status.

Type annotations and code completion for `#!python session.create_client("gamelift").stop_game_session_placement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/stop_game_session_placement.html)

```python
# stop_game_session_placement method definition

await def stop_game_session_placement(
    self,
    *,
    PlacementId: str,
) -> StopGameSessionPlacementOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopGameSessionPlacementOutputTypeDef](./type_defs.md#stopgamesessionplacementoutputtypedef) 


```python
# stop_game_session_placement method usage example with argument unpacking

kwargs: StopGameSessionPlacementInputRequestTypeDef = {  # (1)
    "PlacementId": ...,
}

parent.stop_game_session_placement(**kwargs)
```

1. See [:material-code-braces: StopGameSessionPlacementInputRequestTypeDef](./type_defs.md#stopgamesessionplacementinputrequesttypedef) 

### stop\_matchmaking

Cancels a matchmaking ticket or match backfill ticket that is currently being
processed.

Type annotations and code completion for `#!python session.create_client("gamelift").stop_matchmaking` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/stop_matchmaking.html)

```python
# stop_matchmaking method definition

await def stop_matchmaking(
    self,
    *,
    TicketId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_matchmaking method usage example with argument unpacking

kwargs: StopMatchmakingInputRequestTypeDef = {  # (1)
    "TicketId": ...,
}

parent.stop_matchmaking(**kwargs)
```

1. See [:material-code-braces: StopMatchmakingInputRequestTypeDef](./type_defs.md#stopmatchmakinginputrequesttypedef) 

### suspend\_game\_server\_group

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").suspend_game_server_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/suspend_game_server_group.html)

```python
# suspend_game_server_group method definition

await def suspend_game_server_group(
    self,
    *,
    GameServerGroupName: str,
    SuspendActions: Sequence[GameServerGroupActionType],  # (1)
) -> SuspendGameServerGroupOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GameServerGroupActionType](./literals.md#gameservergroupactiontype) 
2. See [:material-code-braces: SuspendGameServerGroupOutputTypeDef](./type_defs.md#suspendgameservergroupoutputtypedef) 


```python
# suspend_game_server_group method usage example with argument unpacking

kwargs: SuspendGameServerGroupInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
    "SuspendActions": ...,
}

parent.suspend_game_server_group(**kwargs)
```

1. See [:material-code-braces: SuspendGameServerGroupInputRequestTypeDef](./type_defs.md#suspendgameservergroupinputrequesttypedef) 

### tag\_resource

Assigns a tag to an Amazon GameLift resource.

Type annotations and code completion for `#!python session.create_client("gamelift").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### terminate\_game\_session

Ends a game session that's currently in progress.

Type annotations and code completion for `#!python session.create_client("gamelift").terminate_game_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/terminate_game_session.html)

```python
# terminate_game_session method definition

await def terminate_game_session(
    self,
    *,
    GameSessionId: str,
    TerminationMode: TerminationModeType,  # (1)
) -> TerminateGameSessionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TerminationModeType](./literals.md#terminationmodetype) 
2. See [:material-code-braces: TerminateGameSessionOutputTypeDef](./type_defs.md#terminategamesessionoutputtypedef) 


```python
# terminate_game_session method usage example with argument unpacking

kwargs: TerminateGameSessionInputRequestTypeDef = {  # (1)
    "GameSessionId": ...,
    "TerminationMode": ...,
}

parent.terminate_game_session(**kwargs)
```

1. See [:material-code-braces: TerminateGameSessionInputRequestTypeDef](./type_defs.md#terminategamesessioninputrequesttypedef) 

### untag\_resource

Removes a tag assigned to a Amazon GameLift resource.

Type annotations and code completion for `#!python session.create_client("gamelift").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_alias

Updates properties for an alias.

Type annotations and code completion for `#!python session.create_client("gamelift").update_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_alias.html)

```python
# update_alias method definition

await def update_alias(
    self,
    *,
    AliasId: str,
    Name: str = ...,
    Description: str = ...,
    RoutingStrategy: RoutingStrategyTypeDef = ...,  # (1)
) -> UpdateAliasOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RoutingStrategyTypeDef](./type_defs.md#routingstrategytypedef) 
2. See [:material-code-braces: UpdateAliasOutputTypeDef](./type_defs.md#updatealiasoutputtypedef) 


```python
# update_alias method usage example with argument unpacking

kwargs: UpdateAliasInputRequestTypeDef = {  # (1)
    "AliasId": ...,
}

parent.update_alias(**kwargs)
```

1. See [:material-code-braces: UpdateAliasInputRequestTypeDef](./type_defs.md#updatealiasinputrequesttypedef) 

### update\_build

Updates metadata in a build resource, including the build name and version.

Type annotations and code completion for `#!python session.create_client("gamelift").update_build` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_build.html)

```python
# update_build method definition

await def update_build(
    self,
    *,
    BuildId: str,
    Name: str = ...,
    Version: str = ...,
) -> UpdateBuildOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateBuildOutputTypeDef](./type_defs.md#updatebuildoutputtypedef) 


```python
# update_build method usage example with argument unpacking

kwargs: UpdateBuildInputRequestTypeDef = {  # (1)
    "BuildId": ...,
}

parent.update_build(**kwargs)
```

1. See [:material-code-braces: UpdateBuildInputRequestTypeDef](./type_defs.md#updatebuildinputrequesttypedef) 

### update\_container\_fleet

Updates the properties of a managed container fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").update_container_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_container_fleet.html)

```python
# update_container_fleet method definition

await def update_container_fleet(
    self,
    *,
    FleetId: str,
    GameServerContainerGroupDefinitionName: str = ...,
    PerInstanceContainerGroupDefinitionName: str = ...,
    GameServerContainerGroupsPerInstance: int = ...,
    InstanceConnectionPortRange: ConnectionPortRangeTypeDef = ...,  # (1)
    InstanceInboundPermissionAuthorizations: Sequence[IpPermissionTypeDef] = ...,  # (2)
    InstanceInboundPermissionRevocations: Sequence[IpPermissionTypeDef] = ...,  # (2)
    DeploymentConfiguration: DeploymentConfigurationTypeDef = ...,  # (4)
    Description: str = ...,
    MetricGroups: Sequence[str] = ...,
    NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,  # (5)
    GameSessionCreationLimitPolicy: GameSessionCreationLimitPolicyTypeDef = ...,  # (6)
    LogConfiguration: LogConfigurationTypeDef = ...,  # (7)
    RemoveAttributes: Sequence[ContainerFleetRemoveAttributeType] = ...,  # (8)
) -> UpdateContainerFleetOutputTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: ConnectionPortRangeTypeDef](./type_defs.md#connectionportrangetypedef) 
2. See [:material-code-braces: IpPermissionTypeDef](./type_defs.md#ippermissiontypedef) 
3. See [:material-code-braces: IpPermissionTypeDef](./type_defs.md#ippermissiontypedef) 
4. See [:material-code-braces: DeploymentConfigurationTypeDef](./type_defs.md#deploymentconfigurationtypedef) 
5. See [:material-code-brackets: ProtectionPolicyType](./literals.md#protectionpolicytype) 
6. See [:material-code-braces: GameSessionCreationLimitPolicyTypeDef](./type_defs.md#gamesessioncreationlimitpolicytypedef) 
7. See [:material-code-braces: LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef) 
8. See [:material-code-brackets: ContainerFleetRemoveAttributeType](./literals.md#containerfleetremoveattributetype) 
9. See [:material-code-braces: UpdateContainerFleetOutputTypeDef](./type_defs.md#updatecontainerfleetoutputtypedef) 


```python
# update_container_fleet method usage example with argument unpacking

kwargs: UpdateContainerFleetInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.update_container_fleet(**kwargs)
```

1. See [:material-code-braces: UpdateContainerFleetInputRequestTypeDef](./type_defs.md#updatecontainerfleetinputrequesttypedef) 

### update\_container\_group\_definition

Updates properties in an existing container group definition.

Type annotations and code completion for `#!python session.create_client("gamelift").update_container_group_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_container_group_definition.html)

```python
# update_container_group_definition method definition

await def update_container_group_definition(
    self,
    *,
    Name: str,
    GameServerContainerDefinition: GameServerContainerDefinitionInputTypeDef = ...,  # (1)
    SupportContainerDefinitions: Sequence[SupportContainerDefinitionInputTypeDef] = ...,  # (2)
    TotalMemoryLimitMebibytes: int = ...,
    TotalVcpuLimit: float = ...,
    VersionDescription: str = ...,
    SourceVersionNumber: int = ...,
    OperatingSystem: ContainerOperatingSystemType = ...,  # (3)
) -> UpdateContainerGroupDefinitionOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: GameServerContainerDefinitionInputTypeDef](./type_defs.md#gameservercontainerdefinitioninputtypedef) 
2. See [:material-code-braces: SupportContainerDefinitionInputTypeDef](./type_defs.md#supportcontainerdefinitioninputtypedef) 
3. See [:material-code-brackets: ContainerOperatingSystemType](./literals.md#containeroperatingsystemtype) 
4. See [:material-code-braces: UpdateContainerGroupDefinitionOutputTypeDef](./type_defs.md#updatecontainergroupdefinitionoutputtypedef) 


```python
# update_container_group_definition method usage example with argument unpacking

kwargs: UpdateContainerGroupDefinitionInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_container_group_definition(**kwargs)
```

1. See [:material-code-braces: UpdateContainerGroupDefinitionInputRequestTypeDef](./type_defs.md#updatecontainergroupdefinitioninputrequesttypedef) 

### update\_fleet\_attributes

Updates a fleet's mutable attributes, such as game session protection and
resource creation limits.

Type annotations and code completion for `#!python session.create_client("gamelift").update_fleet_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_fleet_attributes.html)

```python
# update_fleet_attributes method definition

await def update_fleet_attributes(
    self,
    *,
    FleetId: str,
    Name: str = ...,
    Description: str = ...,
    NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,  # (1)
    ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,  # (2)
    MetricGroups: Sequence[str] = ...,
    AnywhereConfiguration: AnywhereConfigurationTypeDef = ...,  # (3)
) -> UpdateFleetAttributesOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ProtectionPolicyType](./literals.md#protectionpolicytype) 
2. See [:material-code-braces: ResourceCreationLimitPolicyTypeDef](./type_defs.md#resourcecreationlimitpolicytypedef) 
3. See [:material-code-braces: AnywhereConfigurationTypeDef](./type_defs.md#anywhereconfigurationtypedef) 
4. See [:material-code-braces: UpdateFleetAttributesOutputTypeDef](./type_defs.md#updatefleetattributesoutputtypedef) 


```python
# update_fleet_attributes method usage example with argument unpacking

kwargs: UpdateFleetAttributesInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.update_fleet_attributes(**kwargs)
```

1. See [:material-code-braces: UpdateFleetAttributesInputRequestTypeDef](./type_defs.md#updatefleetattributesinputrequesttypedef) 

### update\_fleet\_capacity

Updates capacity settings for a managed EC2 fleet or managed container fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").update_fleet_capacity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_fleet_capacity.html)

```python
# update_fleet_capacity method definition

await def update_fleet_capacity(
    self,
    *,
    FleetId: str,
    DesiredInstances: int = ...,
    MinSize: int = ...,
    MaxSize: int = ...,
    Location: str = ...,
) -> UpdateFleetCapacityOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateFleetCapacityOutputTypeDef](./type_defs.md#updatefleetcapacityoutputtypedef) 


```python
# update_fleet_capacity method usage example with argument unpacking

kwargs: UpdateFleetCapacityInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.update_fleet_capacity(**kwargs)
```

1. See [:material-code-braces: UpdateFleetCapacityInputRequestTypeDef](./type_defs.md#updatefleetcapacityinputrequesttypedef) 

### update\_fleet\_port\_settings

Updates permissions that allow inbound traffic to connect to game sessions in
the fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").update_fleet_port_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_fleet_port_settings.html)

```python
# update_fleet_port_settings method definition

await def update_fleet_port_settings(
    self,
    *,
    FleetId: str,
    InboundPermissionAuthorizations: Sequence[IpPermissionTypeDef] = ...,  # (1)
    InboundPermissionRevocations: Sequence[IpPermissionTypeDef] = ...,  # (1)
) -> UpdateFleetPortSettingsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IpPermissionTypeDef](./type_defs.md#ippermissiontypedef) 
2. See [:material-code-braces: IpPermissionTypeDef](./type_defs.md#ippermissiontypedef) 
3. See [:material-code-braces: UpdateFleetPortSettingsOutputTypeDef](./type_defs.md#updatefleetportsettingsoutputtypedef) 


```python
# update_fleet_port_settings method usage example with argument unpacking

kwargs: UpdateFleetPortSettingsInputRequestTypeDef = {  # (1)
    "FleetId": ...,
}

parent.update_fleet_port_settings(**kwargs)
```

1. See [:material-code-braces: UpdateFleetPortSettingsInputRequestTypeDef](./type_defs.md#updatefleetportsettingsinputrequesttypedef) 

### update\_game\_server

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").update_game_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_game_server.html)

```python
# update_game_server method definition

await def update_game_server(
    self,
    *,
    GameServerGroupName: str,
    GameServerId: str,
    GameServerData: str = ...,
    UtilizationStatus: GameServerUtilizationStatusType = ...,  # (1)
    HealthCheck: GameServerHealthCheckType = ...,  # (2)
) -> UpdateGameServerOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GameServerUtilizationStatusType](./literals.md#gameserverutilizationstatustype) 
2. See [:material-code-brackets: GameServerHealthCheckType](./literals.md#gameserverhealthchecktype) 
3. See [:material-code-braces: UpdateGameServerOutputTypeDef](./type_defs.md#updategameserveroutputtypedef) 


```python
# update_game_server method usage example with argument unpacking

kwargs: UpdateGameServerInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
    "GameServerId": ...,
}

parent.update_game_server(**kwargs)
```

1. See [:material-code-braces: UpdateGameServerInputRequestTypeDef](./type_defs.md#updategameserverinputrequesttypedef) 

### update\_game\_server\_group

<b>This operation is used with the Amazon GameLift FleetIQ solution and game
server groups.</b>.

Type annotations and code completion for `#!python session.create_client("gamelift").update_game_server_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_game_server_group.html)

```python
# update_game_server_group method definition

await def update_game_server_group(
    self,
    *,
    GameServerGroupName: str,
    RoleArn: str = ...,
    InstanceDefinitions: Sequence[InstanceDefinitionTypeDef] = ...,  # (1)
    GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,  # (2)
    BalancingStrategy: BalancingStrategyType = ...,  # (3)
) -> UpdateGameServerGroupOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: InstanceDefinitionTypeDef](./type_defs.md#instancedefinitiontypedef) 
2. See [:material-code-brackets: GameServerProtectionPolicyType](./literals.md#gameserverprotectionpolicytype) 
3. See [:material-code-brackets: BalancingStrategyType](./literals.md#balancingstrategytype) 
4. See [:material-code-braces: UpdateGameServerGroupOutputTypeDef](./type_defs.md#updategameservergroupoutputtypedef) 


```python
# update_game_server_group method usage example with argument unpacking

kwargs: UpdateGameServerGroupInputRequestTypeDef = {  # (1)
    "GameServerGroupName": ...,
}

parent.update_game_server_group(**kwargs)
```

1. See [:material-code-braces: UpdateGameServerGroupInputRequestTypeDef](./type_defs.md#updategameservergroupinputrequesttypedef) 

### update\_game\_session

Updates the mutable properties of a game session.

Type annotations and code completion for `#!python session.create_client("gamelift").update_game_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_game_session.html)

```python
# update_game_session method definition

await def update_game_session(
    self,
    *,
    GameSessionId: str,
    MaximumPlayerSessionCount: int = ...,
    Name: str = ...,
    PlayerSessionCreationPolicy: PlayerSessionCreationPolicyType = ...,  # (1)
    ProtectionPolicy: ProtectionPolicyType = ...,  # (2)
    GameProperties: Sequence[GamePropertyTypeDef] = ...,  # (3)
) -> UpdateGameSessionOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: PlayerSessionCreationPolicyType](./literals.md#playersessioncreationpolicytype) 
2. See [:material-code-brackets: ProtectionPolicyType](./literals.md#protectionpolicytype) 
3. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
4. See [:material-code-braces: UpdateGameSessionOutputTypeDef](./type_defs.md#updategamesessionoutputtypedef) 


```python
# update_game_session method usage example with argument unpacking

kwargs: UpdateGameSessionInputRequestTypeDef = {  # (1)
    "GameSessionId": ...,
}

parent.update_game_session(**kwargs)
```

1. See [:material-code-braces: UpdateGameSessionInputRequestTypeDef](./type_defs.md#updategamesessioninputrequesttypedef) 

### update\_game\_session\_queue

Updates the configuration of a game session queue, which determines how the
queue processes new game session requests.

Type annotations and code completion for `#!python session.create_client("gamelift").update_game_session_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_game_session_queue.html)

```python
# update_game_session_queue method definition

await def update_game_session_queue(
    self,
    *,
    Name: str,
    TimeoutInSeconds: int = ...,
    PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,  # (1)
    Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,  # (2)
    FilterConfiguration: FilterConfigurationTypeDef = ...,  # (3)
    PriorityConfiguration: PriorityConfigurationTypeDef = ...,  # (4)
    CustomEventData: str = ...,
    NotificationTarget: str = ...,
) -> UpdateGameSessionQueueOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: PlayerLatencyPolicyTypeDef](./type_defs.md#playerlatencypolicytypedef) 
2. See [:material-code-braces: GameSessionQueueDestinationTypeDef](./type_defs.md#gamesessionqueuedestinationtypedef) 
3. See [:material-code-braces: FilterConfigurationTypeDef](./type_defs.md#filterconfigurationtypedef) 
4. See [:material-code-braces: PriorityConfigurationTypeDef](./type_defs.md#priorityconfigurationtypedef) 
5. See [:material-code-braces: UpdateGameSessionQueueOutputTypeDef](./type_defs.md#updategamesessionqueueoutputtypedef) 


```python
# update_game_session_queue method usage example with argument unpacking

kwargs: UpdateGameSessionQueueInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_game_session_queue(**kwargs)
```

1. See [:material-code-braces: UpdateGameSessionQueueInputRequestTypeDef](./type_defs.md#updategamesessionqueueinputrequesttypedef) 

### update\_matchmaking\_configuration

Updates settings for a FlexMatch matchmaking configuration.

Type annotations and code completion for `#!python session.create_client("gamelift").update_matchmaking_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_matchmaking_configuration.html)

```python
# update_matchmaking_configuration method definition

await def update_matchmaking_configuration(
    self,
    *,
    Name: str,
    Description: str = ...,
    GameSessionQueueArns: Sequence[str] = ...,
    RequestTimeoutSeconds: int = ...,
    AcceptanceTimeoutSeconds: int = ...,
    AcceptanceRequired: bool = ...,
    RuleSetName: str = ...,
    NotificationTarget: str = ...,
    AdditionalPlayerCount: int = ...,
    CustomEventData: str = ...,
    GameProperties: Sequence[GamePropertyTypeDef] = ...,  # (1)
    GameSessionData: str = ...,
    BackfillMode: BackfillModeType = ...,  # (2)
    FlexMatchMode: FlexMatchModeType = ...,  # (3)
) -> UpdateMatchmakingConfigurationOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
2. See [:material-code-brackets: BackfillModeType](./literals.md#backfillmodetype) 
3. See [:material-code-brackets: FlexMatchModeType](./literals.md#flexmatchmodetype) 
4. See [:material-code-braces: UpdateMatchmakingConfigurationOutputTypeDef](./type_defs.md#updatematchmakingconfigurationoutputtypedef) 


```python
# update_matchmaking_configuration method usage example with argument unpacking

kwargs: UpdateMatchmakingConfigurationInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_matchmaking_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateMatchmakingConfigurationInputRequestTypeDef](./type_defs.md#updatematchmakingconfigurationinputrequesttypedef) 

### update\_runtime\_configuration

Updates the runtime configuration for the specified fleet.

Type annotations and code completion for `#!python session.create_client("gamelift").update_runtime_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_runtime_configuration.html)

```python
# update_runtime_configuration method definition

await def update_runtime_configuration(
    self,
    *,
    FleetId: str,
    RuntimeConfiguration: RuntimeConfigurationTypeDef,  # (1)
) -> UpdateRuntimeConfigurationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RuntimeConfigurationTypeDef](./type_defs.md#runtimeconfigurationtypedef) 
2. See [:material-code-braces: UpdateRuntimeConfigurationOutputTypeDef](./type_defs.md#updateruntimeconfigurationoutputtypedef) 


```python
# update_runtime_configuration method usage example with argument unpacking

kwargs: UpdateRuntimeConfigurationInputRequestTypeDef = {  # (1)
    "FleetId": ...,
    "RuntimeConfiguration": ...,
}

parent.update_runtime_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateRuntimeConfigurationInputRequestTypeDef](./type_defs.md#updateruntimeconfigurationinputrequesttypedef) 

### update\_script

Updates Realtime script metadata and content.

Type annotations and code completion for `#!python session.create_client("gamelift").update_script` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/update_script.html)

```python
# update_script method definition

await def update_script(
    self,
    *,
    ScriptId: str,
    Name: str = ...,
    Version: str = ...,
    StorageLocation: S3LocationTypeDef = ...,  # (1)
    ZipFile: BlobTypeDef = ...,
) -> UpdateScriptOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: UpdateScriptOutputTypeDef](./type_defs.md#updatescriptoutputtypedef) 


```python
# update_script method usage example with argument unpacking

kwargs: UpdateScriptInputRequestTypeDef = {  # (1)
    "ScriptId": ...,
}

parent.update_script(**kwargs)
```

1. See [:material-code-braces: UpdateScriptInputRequestTypeDef](./type_defs.md#updatescriptinputrequesttypedef) 

### validate\_matchmaking\_rule\_set

Validates the syntax of a matchmaking rule or rule set.

Type annotations and code completion for `#!python session.create_client("gamelift").validate_matchmaking_rule_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift/client/validate_matchmaking_rule_set.html)

```python
# validate_matchmaking_rule_set method definition

await def validate_matchmaking_rule_set(
    self,
    *,
    RuleSetBody: str,
) -> ValidateMatchmakingRuleSetOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ValidateMatchmakingRuleSetOutputTypeDef](./type_defs.md#validatematchmakingrulesetoutputtypedef) 


```python
# validate_matchmaking_rule_set method usage example with argument unpacking

kwargs: ValidateMatchmakingRuleSetInputRequestTypeDef = {  # (1)
    "RuleSetBody": ...,
}

parent.validate_matchmaking_rule_set(**kwargs)
```

1. See [:material-code-braces: ValidateMatchmakingRuleSetInputRequestTypeDef](./type_defs.md#validatematchmakingrulesetinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("gamelift").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("gamelift").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("gamelift").get_paginator` method with overloads.

- `client.get_paginator("describe_fleet_attributes")` -> [DescribeFleetAttributesPaginator](./paginators.md#describefleetattributespaginator)
- `client.get_paginator("describe_fleet_capacity")` -> [DescribeFleetCapacityPaginator](./paginators.md#describefleetcapacitypaginator)
- `client.get_paginator("describe_fleet_events")` -> [DescribeFleetEventsPaginator](./paginators.md#describefleeteventspaginator)
- `client.get_paginator("describe_fleet_utilization")` -> [DescribeFleetUtilizationPaginator](./paginators.md#describefleetutilizationpaginator)
- `client.get_paginator("describe_game_server_instances")` -> [DescribeGameServerInstancesPaginator](./paginators.md#describegameserverinstancespaginator)
- `client.get_paginator("describe_game_session_details")` -> [DescribeGameSessionDetailsPaginator](./paginators.md#describegamesessiondetailspaginator)
- `client.get_paginator("describe_game_session_queues")` -> [DescribeGameSessionQueuesPaginator](./paginators.md#describegamesessionqueuespaginator)
- `client.get_paginator("describe_game_sessions")` -> [DescribeGameSessionsPaginator](./paginators.md#describegamesessionspaginator)
- `client.get_paginator("describe_instances")` -> [DescribeInstancesPaginator](./paginators.md#describeinstancespaginator)
- `client.get_paginator("describe_matchmaking_configurations")` -> [DescribeMatchmakingConfigurationsPaginator](./paginators.md#describematchmakingconfigurationspaginator)
- `client.get_paginator("describe_matchmaking_rule_sets")` -> [DescribeMatchmakingRuleSetsPaginator](./paginators.md#describematchmakingrulesetspaginator)
- `client.get_paginator("describe_player_sessions")` -> [DescribePlayerSessionsPaginator](./paginators.md#describeplayersessionspaginator)
- `client.get_paginator("describe_scaling_policies")` -> [DescribeScalingPoliciesPaginator](./paginators.md#describescalingpoliciespaginator)
- `client.get_paginator("list_aliases")` -> [ListAliasesPaginator](./paginators.md#listaliasespaginator)
- `client.get_paginator("list_builds")` -> [ListBuildsPaginator](./paginators.md#listbuildspaginator)
- `client.get_paginator("list_compute")` -> [ListComputePaginator](./paginators.md#listcomputepaginator)
- `client.get_paginator("list_container_fleets")` -> [ListContainerFleetsPaginator](./paginators.md#listcontainerfleetspaginator)
- `client.get_paginator("list_container_group_definition_versions")` -> [ListContainerGroupDefinitionVersionsPaginator](./paginators.md#listcontainergroupdefinitionversionspaginator)
- `client.get_paginator("list_container_group_definitions")` -> [ListContainerGroupDefinitionsPaginator](./paginators.md#listcontainergroupdefinitionspaginator)
- `client.get_paginator("list_fleet_deployments")` -> [ListFleetDeploymentsPaginator](./paginators.md#listfleetdeploymentspaginator)
- `client.get_paginator("list_fleets")` -> [ListFleetsPaginator](./paginators.md#listfleetspaginator)
- `client.get_paginator("list_game_server_groups")` -> [ListGameServerGroupsPaginator](./paginators.md#listgameservergroupspaginator)
- `client.get_paginator("list_game_servers")` -> [ListGameServersPaginator](./paginators.md#listgameserverspaginator)
- `client.get_paginator("list_locations")` -> [ListLocationsPaginator](./paginators.md#listlocationspaginator)
- `client.get_paginator("list_scripts")` -> [ListScriptsPaginator](./paginators.md#listscriptspaginator)
- `client.get_paginator("search_game_sessions")` -> [SearchGameSessionsPaginator](./paginators.md#searchgamesessionspaginator)



