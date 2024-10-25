# Type definitions

> [Index](../README.md) > [GameLift](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [GameLift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
    type annotations stubs module [types-aiobotocore-gamelift](https://pypi.org/project/types-aiobotocore-gamelift/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AttributeValueUnionTypeDef

```python
# AttributeValueUnionTypeDef definition

AttributeValueUnionTypeDef = Union[
    AttributeValueTypeDef,  # (1)
    AttributeValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 

## ContainerHealthCheckUnionTypeDef

```python
# ContainerHealthCheckUnionTypeDef definition

ContainerHealthCheckUnionTypeDef = Union[
    ContainerHealthCheckTypeDef,  # (1)
    ContainerHealthCheckOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ContainerHealthCheckTypeDef](./type_defs.md#containerhealthchecktypedef) 
2. See [:material-code-braces: ContainerHealthCheckOutputTypeDef](./type_defs.md#containerhealthcheckoutputtypedef) 

## ContainerPortConfigurationUnionTypeDef

```python
# ContainerPortConfigurationUnionTypeDef definition

ContainerPortConfigurationUnionTypeDef = Union[
    ContainerPortConfigurationTypeDef,  # (1)
    ContainerPortConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ContainerPortConfigurationTypeDef](./type_defs.md#containerportconfigurationtypedef) 
2. See [:material-code-braces: ContainerPortConfigurationOutputTypeDef](./type_defs.md#containerportconfigurationoutputtypedef) 

## PlayerUnionTypeDef

```python
# PlayerUnionTypeDef definition

PlayerUnionTypeDef = Union[
    PlayerTypeDef,  # (1)
    PlayerOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PlayerTypeDef](./type_defs.md#playertypedef) 
2. See [:material-code-braces: PlayerOutputTypeDef](./type_defs.md#playeroutputtypedef) 



## AcceptMatchInputRequestTypeDef

```python
# AcceptMatchInputRequestTypeDef definition

class AcceptMatchInputRequestTypeDef(TypedDict):
    TicketId: str,
    PlayerIds: Sequence[str],
    AcceptanceType: AcceptanceTypeType,  # (1)
```

1. See [:material-code-brackets: AcceptanceTypeType](./literals.md#acceptancetypetype) 
## RoutingStrategyTypeDef

```python
# RoutingStrategyTypeDef definition

class RoutingStrategyTypeDef(TypedDict):
    Type: NotRequired[RoutingStrategyTypeType],  # (1)
    FleetId: NotRequired[str],
    Message: NotRequired[str],
```

1. See [:material-code-brackets: RoutingStrategyTypeType](./literals.md#routingstrategytypetype) 
## AnywhereConfigurationTypeDef

```python
# AnywhereConfigurationTypeDef definition

class AnywhereConfigurationTypeDef(TypedDict):
    Cost: str,
```

## AttributeValueOutputTypeDef

```python
# AttributeValueOutputTypeDef definition

class AttributeValueOutputTypeDef(TypedDict):
    S: NotRequired[str],
    N: NotRequired[float],
    SL: NotRequired[List[str]],
    SDM: NotRequired[Dict[str, float]],
```

## AttributeValueTypeDef

```python
# AttributeValueTypeDef definition

class AttributeValueTypeDef(TypedDict):
    S: NotRequired[str],
    N: NotRequired[float],
    SL: NotRequired[Sequence[str]],
    SDM: NotRequired[Mapping[str, float]],
```

## AwsCredentialsTypeDef

```python
# AwsCredentialsTypeDef definition

class AwsCredentialsTypeDef(TypedDict):
    AccessKeyId: NotRequired[str],
    SecretAccessKey: NotRequired[str],
    SessionToken: NotRequired[str],
```

## BuildTypeDef

```python
# BuildTypeDef definition

class BuildTypeDef(TypedDict):
    BuildId: NotRequired[str],
    BuildArn: NotRequired[str],
    Name: NotRequired[str],
    Version: NotRequired[str],
    Status: NotRequired[BuildStatusType],  # (1)
    SizeOnDisk: NotRequired[int],
    OperatingSystem: NotRequired[OperatingSystemType],  # (2)
    CreationTime: NotRequired[datetime],
    ServerSdkVersion: NotRequired[str],
```

1. See [:material-code-brackets: BuildStatusType](./literals.md#buildstatustype) 
2. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
## CertificateConfigurationTypeDef

```python
# CertificateConfigurationTypeDef definition

class CertificateConfigurationTypeDef(TypedDict):
    CertificateType: CertificateTypeType,  # (1)
```

1. See [:material-code-brackets: CertificateTypeType](./literals.md#certificatetypetype) 
## ClaimFilterOptionTypeDef

```python
# ClaimFilterOptionTypeDef definition

class ClaimFilterOptionTypeDef(TypedDict):
    InstanceStatuses: NotRequired[Sequence[FilterInstanceStatusType]],  # (1)
```

1. See [:material-code-brackets: FilterInstanceStatusType](./literals.md#filterinstancestatustype) 
## GameServerTypeDef

```python
# GameServerTypeDef definition

class GameServerTypeDef(TypedDict):
    GameServerGroupName: NotRequired[str],
    GameServerGroupArn: NotRequired[str],
    GameServerId: NotRequired[str],
    InstanceId: NotRequired[str],
    ConnectionInfo: NotRequired[str],
    GameServerData: NotRequired[str],
    ClaimStatus: NotRequired[GameServerClaimStatusType],  # (1)
    UtilizationStatus: NotRequired[GameServerUtilizationStatusType],  # (2)
    RegistrationTime: NotRequired[datetime],
    LastClaimTime: NotRequired[datetime],
    LastHealthCheckTime: NotRequired[datetime],
```

1. See [:material-code-brackets: GameServerClaimStatusType](./literals.md#gameserverclaimstatustype) 
2. See [:material-code-brackets: GameServerUtilizationStatusType](./literals.md#gameserverutilizationstatustype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ConnectionPortRangeTypeDef

```python
# ConnectionPortRangeTypeDef definition

class ConnectionPortRangeTypeDef(TypedDict):
    FromPort: int,
    ToPort: int,
```

## ContainerPortMappingTypeDef

```python
# ContainerPortMappingTypeDef definition

class ContainerPortMappingTypeDef(TypedDict):
    ContainerPort: NotRequired[int],
    ConnectionPort: NotRequired[int],
    Protocol: NotRequired[IpProtocolType],  # (1)
```

1. See [:material-code-brackets: IpProtocolType](./literals.md#ipprotocoltype) 
## ContainerDependencyTypeDef

```python
# ContainerDependencyTypeDef definition

class ContainerDependencyTypeDef(TypedDict):
    ContainerName: str,
    Condition: ContainerDependencyConditionType,  # (1)
```

1. See [:material-code-brackets: ContainerDependencyConditionType](./literals.md#containerdependencyconditiontype) 
## ContainerEnvironmentTypeDef

```python
# ContainerEnvironmentTypeDef definition

class ContainerEnvironmentTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## ContainerMemoryLimitsTypeDef

```python
# ContainerMemoryLimitsTypeDef definition

class ContainerMemoryLimitsTypeDef(TypedDict):
    SoftLimit: NotRequired[int],
    HardLimit: NotRequired[int],
```

## ContainerHealthCheckOutputTypeDef

```python
# ContainerHealthCheckOutputTypeDef definition

class ContainerHealthCheckOutputTypeDef(TypedDict):
    Command: List[str],
    Interval: NotRequired[int],
    Timeout: NotRequired[int],
    Retries: NotRequired[int],
    StartPeriod: NotRequired[int],
```

## ContainerGroupDefinitionPropertyTypeDef

```python
# ContainerGroupDefinitionPropertyTypeDef definition

class ContainerGroupDefinitionPropertyTypeDef(TypedDict):
    SchedulingStrategy: NotRequired[ContainerSchedulingStrategyType],  # (1)
    ContainerGroupDefinitionName: NotRequired[str],
```

1. See [:material-code-brackets: ContainerSchedulingStrategyType](./literals.md#containerschedulingstrategytype) 
## ContainerGroupsPerInstanceTypeDef

```python
# ContainerGroupsPerInstanceTypeDef definition

class ContainerGroupsPerInstanceTypeDef(TypedDict):
    DesiredReplicaContainerGroupsPerInstance: NotRequired[int],
    MaxReplicaContainerGroupsPerInstance: NotRequired[int],
```

## ContainerHealthCheckTypeDef

```python
# ContainerHealthCheckTypeDef definition

class ContainerHealthCheckTypeDef(TypedDict):
    Command: Sequence[str],
    Interval: NotRequired[int],
    Timeout: NotRequired[int],
    Retries: NotRequired[int],
    StartPeriod: NotRequired[int],
```

## ContainerPortRangeTypeDef

```python
# ContainerPortRangeTypeDef definition

class ContainerPortRangeTypeDef(TypedDict):
    FromPort: int,
    ToPort: int,
    Protocol: IpProtocolType,  # (1)
```

1. See [:material-code-brackets: IpProtocolType](./literals.md#ipprotocoltype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Key: NotRequired[str],
    RoleArn: NotRequired[str],
    ObjectVersion: NotRequired[str],
```

## IpPermissionTypeDef

```python
# IpPermissionTypeDef definition

class IpPermissionTypeDef(TypedDict):
    FromPort: int,
    ToPort: int,
    IpRange: str,
    Protocol: IpProtocolType,  # (1)
```

1. See [:material-code-brackets: IpProtocolType](./literals.md#ipprotocoltype) 
## LocationConfigurationTypeDef

```python
# LocationConfigurationTypeDef definition

class LocationConfigurationTypeDef(TypedDict):
    Location: str,
```

## ResourceCreationLimitPolicyTypeDef

```python
# ResourceCreationLimitPolicyTypeDef definition

class ResourceCreationLimitPolicyTypeDef(TypedDict):
    NewGameSessionsPerCreator: NotRequired[int],
    PolicyPeriodInMinutes: NotRequired[int],
```

## LocationStateTypeDef

```python
# LocationStateTypeDef definition

class LocationStateTypeDef(TypedDict):
    Location: NotRequired[str],
    Status: NotRequired[FleetStatusType],  # (1)
```

1. See [:material-code-brackets: FleetStatusType](./literals.md#fleetstatustype) 
## InstanceDefinitionTypeDef

```python
# InstanceDefinitionTypeDef definition

class InstanceDefinitionTypeDef(TypedDict):
    InstanceType: GameServerGroupInstanceTypeType,  # (1)
    WeightedCapacity: NotRequired[str],
```

1. See [:material-code-brackets: GameServerGroupInstanceTypeType](./literals.md#gameservergroupinstancetypetype) 
## LaunchTemplateSpecificationTypeDef

```python
# LaunchTemplateSpecificationTypeDef definition

class LaunchTemplateSpecificationTypeDef(TypedDict):
    LaunchTemplateId: NotRequired[str],
    LaunchTemplateName: NotRequired[str],
    Version: NotRequired[str],
```

## GamePropertyTypeDef

```python
# GamePropertyTypeDef definition

class GamePropertyTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## FilterConfigurationTypeDef

```python
# FilterConfigurationTypeDef definition

class FilterConfigurationTypeDef(TypedDict):
    AllowedLocations: NotRequired[Sequence[str]],
```

## GameSessionQueueDestinationTypeDef

```python
# GameSessionQueueDestinationTypeDef definition

class GameSessionQueueDestinationTypeDef(TypedDict):
    DestinationArn: NotRequired[str],
```

## PlayerLatencyPolicyTypeDef

```python
# PlayerLatencyPolicyTypeDef definition

class PlayerLatencyPolicyTypeDef(TypedDict):
    MaximumIndividualPlayerLatencyMilliseconds: NotRequired[int],
    PolicyDurationSeconds: NotRequired[int],
```

## PriorityConfigurationTypeDef

```python
# PriorityConfigurationTypeDef definition

class PriorityConfigurationTypeDef(TypedDict):
    PriorityOrder: NotRequired[Sequence[PriorityTypeType]],  # (1)
    LocationOrder: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: PriorityTypeType](./literals.md#prioritytypetype) 
## LocationModelTypeDef

```python
# LocationModelTypeDef definition

class LocationModelTypeDef(TypedDict):
    LocationName: NotRequired[str],
    LocationArn: NotRequired[str],
```

## MatchmakingRuleSetTypeDef

```python
# MatchmakingRuleSetTypeDef definition

class MatchmakingRuleSetTypeDef(TypedDict):
    RuleSetBody: str,
    RuleSetName: NotRequired[str],
    RuleSetArn: NotRequired[str],
    CreationTime: NotRequired[datetime],
```

## CreatePlayerSessionInputRequestTypeDef

```python
# CreatePlayerSessionInputRequestTypeDef definition

class CreatePlayerSessionInputRequestTypeDef(TypedDict):
    GameSessionId: str,
    PlayerId: str,
    PlayerData: NotRequired[str],
```

## PlayerSessionTypeDef

```python
# PlayerSessionTypeDef definition

class PlayerSessionTypeDef(TypedDict):
    PlayerSessionId: NotRequired[str],
    PlayerId: NotRequired[str],
    GameSessionId: NotRequired[str],
    FleetId: NotRequired[str],
    FleetArn: NotRequired[str],
    CreationTime: NotRequired[datetime],
    TerminationTime: NotRequired[datetime],
    Status: NotRequired[PlayerSessionStatusType],  # (1)
    IpAddress: NotRequired[str],
    DnsName: NotRequired[str],
    Port: NotRequired[int],
    PlayerData: NotRequired[str],
```

1. See [:material-code-brackets: PlayerSessionStatusType](./literals.md#playersessionstatustype) 
## CreatePlayerSessionsInputRequestTypeDef

```python
# CreatePlayerSessionsInputRequestTypeDef definition

class CreatePlayerSessionsInputRequestTypeDef(TypedDict):
    GameSessionId: str,
    PlayerIds: Sequence[str],
    PlayerDataMap: NotRequired[Mapping[str, str]],
```

## CreateVpcPeeringAuthorizationInputRequestTypeDef

```python
# CreateVpcPeeringAuthorizationInputRequestTypeDef definition

class CreateVpcPeeringAuthorizationInputRequestTypeDef(TypedDict):
    GameLiftAwsAccountId: str,
    PeerVpcId: str,
```

## VpcPeeringAuthorizationTypeDef

```python
# VpcPeeringAuthorizationTypeDef definition

class VpcPeeringAuthorizationTypeDef(TypedDict):
    GameLiftAwsAccountId: NotRequired[str],
    PeerVpcAwsAccountId: NotRequired[str],
    PeerVpcId: NotRequired[str],
    CreationTime: NotRequired[datetime],
    ExpirationTime: NotRequired[datetime],
```

## CreateVpcPeeringConnectionInputRequestTypeDef

```python
# CreateVpcPeeringConnectionInputRequestTypeDef definition

class CreateVpcPeeringConnectionInputRequestTypeDef(TypedDict):
    FleetId: str,
    PeerVpcAwsAccountId: str,
    PeerVpcId: str,
```

## DeleteAliasInputRequestTypeDef

```python
# DeleteAliasInputRequestTypeDef definition

class DeleteAliasInputRequestTypeDef(TypedDict):
    AliasId: str,
```

## DeleteBuildInputRequestTypeDef

```python
# DeleteBuildInputRequestTypeDef definition

class DeleteBuildInputRequestTypeDef(TypedDict):
    BuildId: str,
```

## DeleteContainerGroupDefinitionInputRequestTypeDef

```python
# DeleteContainerGroupDefinitionInputRequestTypeDef definition

class DeleteContainerGroupDefinitionInputRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteFleetInputRequestTypeDef

```python
# DeleteFleetInputRequestTypeDef definition

class DeleteFleetInputRequestTypeDef(TypedDict):
    FleetId: str,
```

## DeleteFleetLocationsInputRequestTypeDef

```python
# DeleteFleetLocationsInputRequestTypeDef definition

class DeleteFleetLocationsInputRequestTypeDef(TypedDict):
    FleetId: str,
    Locations: Sequence[str],
```

## DeleteGameServerGroupInputRequestTypeDef

```python
# DeleteGameServerGroupInputRequestTypeDef definition

class DeleteGameServerGroupInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    DeleteOption: NotRequired[GameServerGroupDeleteOptionType],  # (1)
```

1. See [:material-code-brackets: GameServerGroupDeleteOptionType](./literals.md#gameservergroupdeleteoptiontype) 
## DeleteGameSessionQueueInputRequestTypeDef

```python
# DeleteGameSessionQueueInputRequestTypeDef definition

class DeleteGameSessionQueueInputRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteLocationInputRequestTypeDef

```python
# DeleteLocationInputRequestTypeDef definition

class DeleteLocationInputRequestTypeDef(TypedDict):
    LocationName: str,
```

## DeleteMatchmakingConfigurationInputRequestTypeDef

```python
# DeleteMatchmakingConfigurationInputRequestTypeDef definition

class DeleteMatchmakingConfigurationInputRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteMatchmakingRuleSetInputRequestTypeDef

```python
# DeleteMatchmakingRuleSetInputRequestTypeDef definition

class DeleteMatchmakingRuleSetInputRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteScalingPolicyInputRequestTypeDef

```python
# DeleteScalingPolicyInputRequestTypeDef definition

class DeleteScalingPolicyInputRequestTypeDef(TypedDict):
    Name: str,
    FleetId: str,
```

## DeleteScriptInputRequestTypeDef

```python
# DeleteScriptInputRequestTypeDef definition

class DeleteScriptInputRequestTypeDef(TypedDict):
    ScriptId: str,
```

## DeleteVpcPeeringAuthorizationInputRequestTypeDef

```python
# DeleteVpcPeeringAuthorizationInputRequestTypeDef definition

class DeleteVpcPeeringAuthorizationInputRequestTypeDef(TypedDict):
    GameLiftAwsAccountId: str,
    PeerVpcId: str,
```

## DeleteVpcPeeringConnectionInputRequestTypeDef

```python
# DeleteVpcPeeringConnectionInputRequestTypeDef definition

class DeleteVpcPeeringConnectionInputRequestTypeDef(TypedDict):
    FleetId: str,
    VpcPeeringConnectionId: str,
```

## DeregisterComputeInputRequestTypeDef

```python
# DeregisterComputeInputRequestTypeDef definition

class DeregisterComputeInputRequestTypeDef(TypedDict):
    FleetId: str,
    ComputeName: str,
```

## DeregisterGameServerInputRequestTypeDef

```python
# DeregisterGameServerInputRequestTypeDef definition

class DeregisterGameServerInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    GameServerId: str,
```

## DescribeAliasInputRequestTypeDef

```python
# DescribeAliasInputRequestTypeDef definition

class DescribeAliasInputRequestTypeDef(TypedDict):
    AliasId: str,
```

## DescribeBuildInputRequestTypeDef

```python
# DescribeBuildInputRequestTypeDef definition

class DescribeBuildInputRequestTypeDef(TypedDict):
    BuildId: str,
```

## DescribeComputeInputRequestTypeDef

```python
# DescribeComputeInputRequestTypeDef definition

class DescribeComputeInputRequestTypeDef(TypedDict):
    FleetId: str,
    ComputeName: str,
```

## DescribeContainerGroupDefinitionInputRequestTypeDef

```python
# DescribeContainerGroupDefinitionInputRequestTypeDef definition

class DescribeContainerGroupDefinitionInputRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeEC2InstanceLimitsInputRequestTypeDef

```python
# DescribeEC2InstanceLimitsInputRequestTypeDef definition

class DescribeEC2InstanceLimitsInputRequestTypeDef(TypedDict):
    EC2InstanceType: NotRequired[EC2InstanceTypeType],  # (1)
    Location: NotRequired[str],
```

1. See [:material-code-brackets: EC2InstanceTypeType](./literals.md#ec2instancetypetype) 
## EC2InstanceLimitTypeDef

```python
# EC2InstanceLimitTypeDef definition

class EC2InstanceLimitTypeDef(TypedDict):
    EC2InstanceType: NotRequired[EC2InstanceTypeType],  # (1)
    CurrentInstances: NotRequired[int],
    InstanceLimit: NotRequired[int],
    Location: NotRequired[str],
```

1. See [:material-code-brackets: EC2InstanceTypeType](./literals.md#ec2instancetypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeFleetAttributesInputRequestTypeDef

```python
# DescribeFleetAttributesInputRequestTypeDef definition

class DescribeFleetAttributesInputRequestTypeDef(TypedDict):
    FleetIds: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeFleetCapacityInputRequestTypeDef

```python
# DescribeFleetCapacityInputRequestTypeDef definition

class DescribeFleetCapacityInputRequestTypeDef(TypedDict):
    FleetIds: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    EventId: NotRequired[str],
    ResourceId: NotRequired[str],
    EventCode: NotRequired[EventCodeType],  # (1)
    Message: NotRequired[str],
    EventTime: NotRequired[datetime],
    PreSignedLogUrl: NotRequired[str],
    Count: NotRequired[int],
```

1. See [:material-code-brackets: EventCodeType](./literals.md#eventcodetype) 
## DescribeFleetLocationAttributesInputRequestTypeDef

```python
# DescribeFleetLocationAttributesInputRequestTypeDef definition

class DescribeFleetLocationAttributesInputRequestTypeDef(TypedDict):
    FleetId: str,
    Locations: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeFleetLocationCapacityInputRequestTypeDef

```python
# DescribeFleetLocationCapacityInputRequestTypeDef definition

class DescribeFleetLocationCapacityInputRequestTypeDef(TypedDict):
    FleetId: str,
    Location: str,
```

## DescribeFleetLocationUtilizationInputRequestTypeDef

```python
# DescribeFleetLocationUtilizationInputRequestTypeDef definition

class DescribeFleetLocationUtilizationInputRequestTypeDef(TypedDict):
    FleetId: str,
    Location: str,
```

## FleetUtilizationTypeDef

```python
# FleetUtilizationTypeDef definition

class FleetUtilizationTypeDef(TypedDict):
    FleetId: NotRequired[str],
    FleetArn: NotRequired[str],
    ActiveServerProcessCount: NotRequired[int],
    ActiveGameSessionCount: NotRequired[int],
    CurrentPlayerSessionCount: NotRequired[int],
    MaximumPlayerSessionCount: NotRequired[int],
    Location: NotRequired[str],
```

## DescribeFleetPortSettingsInputRequestTypeDef

```python
# DescribeFleetPortSettingsInputRequestTypeDef definition

class DescribeFleetPortSettingsInputRequestTypeDef(TypedDict):
    FleetId: str,
    Location: NotRequired[str],
```

## DescribeFleetUtilizationInputRequestTypeDef

```python
# DescribeFleetUtilizationInputRequestTypeDef definition

class DescribeFleetUtilizationInputRequestTypeDef(TypedDict):
    FleetIds: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeGameServerGroupInputRequestTypeDef

```python
# DescribeGameServerGroupInputRequestTypeDef definition

class DescribeGameServerGroupInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
```

## DescribeGameServerInputRequestTypeDef

```python
# DescribeGameServerInputRequestTypeDef definition

class DescribeGameServerInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    GameServerId: str,
```

## DescribeGameServerInstancesInputRequestTypeDef

```python
# DescribeGameServerInstancesInputRequestTypeDef definition

class DescribeGameServerInstancesInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    InstanceIds: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## GameServerInstanceTypeDef

```python
# GameServerInstanceTypeDef definition

class GameServerInstanceTypeDef(TypedDict):
    GameServerGroupName: NotRequired[str],
    GameServerGroupArn: NotRequired[str],
    InstanceId: NotRequired[str],
    InstanceStatus: NotRequired[GameServerInstanceStatusType],  # (1)
```

1. See [:material-code-brackets: GameServerInstanceStatusType](./literals.md#gameserverinstancestatustype) 
## DescribeGameSessionDetailsInputRequestTypeDef

```python
# DescribeGameSessionDetailsInputRequestTypeDef definition

class DescribeGameSessionDetailsInputRequestTypeDef(TypedDict):
    FleetId: NotRequired[str],
    GameSessionId: NotRequired[str],
    AliasId: NotRequired[str],
    Location: NotRequired[str],
    StatusFilter: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeGameSessionPlacementInputRequestTypeDef

```python
# DescribeGameSessionPlacementInputRequestTypeDef definition

class DescribeGameSessionPlacementInputRequestTypeDef(TypedDict):
    PlacementId: str,
```

## DescribeGameSessionQueuesInputRequestTypeDef

```python
# DescribeGameSessionQueuesInputRequestTypeDef definition

class DescribeGameSessionQueuesInputRequestTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeGameSessionsInputRequestTypeDef

```python
# DescribeGameSessionsInputRequestTypeDef definition

class DescribeGameSessionsInputRequestTypeDef(TypedDict):
    FleetId: NotRequired[str],
    GameSessionId: NotRequired[str],
    AliasId: NotRequired[str],
    Location: NotRequired[str],
    StatusFilter: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeInstancesInputRequestTypeDef

```python
# DescribeInstancesInputRequestTypeDef definition

class DescribeInstancesInputRequestTypeDef(TypedDict):
    FleetId: str,
    InstanceId: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
    Location: NotRequired[str],
```

## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    FleetId: NotRequired[str],
    FleetArn: NotRequired[str],
    InstanceId: NotRequired[str],
    IpAddress: NotRequired[str],
    DnsName: NotRequired[str],
    OperatingSystem: NotRequired[OperatingSystemType],  # (1)
    Type: NotRequired[EC2InstanceTypeType],  # (2)
    Status: NotRequired[InstanceStatusType],  # (3)
    CreationTime: NotRequired[datetime],
    Location: NotRequired[str],
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-brackets: EC2InstanceTypeType](./literals.md#ec2instancetypetype) 
3. See [:material-code-brackets: InstanceStatusType](./literals.md#instancestatustype) 
## DescribeMatchmakingConfigurationsInputRequestTypeDef

```python
# DescribeMatchmakingConfigurationsInputRequestTypeDef definition

class DescribeMatchmakingConfigurationsInputRequestTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    RuleSetName: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeMatchmakingInputRequestTypeDef

```python
# DescribeMatchmakingInputRequestTypeDef definition

class DescribeMatchmakingInputRequestTypeDef(TypedDict):
    TicketIds: Sequence[str],
```

## DescribeMatchmakingRuleSetsInputRequestTypeDef

```python
# DescribeMatchmakingRuleSetsInputRequestTypeDef definition

class DescribeMatchmakingRuleSetsInputRequestTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribePlayerSessionsInputRequestTypeDef

```python
# DescribePlayerSessionsInputRequestTypeDef definition

class DescribePlayerSessionsInputRequestTypeDef(TypedDict):
    GameSessionId: NotRequired[str],
    PlayerId: NotRequired[str],
    PlayerSessionId: NotRequired[str],
    PlayerSessionStatusFilter: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeRuntimeConfigurationInputRequestTypeDef

```python
# DescribeRuntimeConfigurationInputRequestTypeDef definition

class DescribeRuntimeConfigurationInputRequestTypeDef(TypedDict):
    FleetId: str,
```

## DescribeScalingPoliciesInputRequestTypeDef

```python
# DescribeScalingPoliciesInputRequestTypeDef definition

class DescribeScalingPoliciesInputRequestTypeDef(TypedDict):
    FleetId: str,
    StatusFilter: NotRequired[ScalingStatusTypeType],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
    Location: NotRequired[str],
```

1. See [:material-code-brackets: ScalingStatusTypeType](./literals.md#scalingstatustypetype) 
## DescribeScriptInputRequestTypeDef

```python
# DescribeScriptInputRequestTypeDef definition

class DescribeScriptInputRequestTypeDef(TypedDict):
    ScriptId: str,
```

## DescribeVpcPeeringConnectionsInputRequestTypeDef

```python
# DescribeVpcPeeringConnectionsInputRequestTypeDef definition

class DescribeVpcPeeringConnectionsInputRequestTypeDef(TypedDict):
    FleetId: NotRequired[str],
```

## DesiredPlayerSessionTypeDef

```python
# DesiredPlayerSessionTypeDef definition

class DesiredPlayerSessionTypeDef(TypedDict):
    PlayerId: NotRequired[str],
    PlayerData: NotRequired[str],
```

## EC2InstanceCountsTypeDef

```python
# EC2InstanceCountsTypeDef definition

class EC2InstanceCountsTypeDef(TypedDict):
    DESIRED: NotRequired[int],
    MINIMUM: NotRequired[int],
    MAXIMUM: NotRequired[int],
    PENDING: NotRequired[int],
    ACTIVE: NotRequired[int],
    IDLE: NotRequired[int],
    TERMINATING: NotRequired[int],
```

## FilterConfigurationOutputTypeDef

```python
# FilterConfigurationOutputTypeDef definition

class FilterConfigurationOutputTypeDef(TypedDict):
    AllowedLocations: NotRequired[List[str]],
```

## ReplicaContainerGroupCountsTypeDef

```python
# ReplicaContainerGroupCountsTypeDef definition

class ReplicaContainerGroupCountsTypeDef(TypedDict):
    PENDING: NotRequired[int],
    ACTIVE: NotRequired[int],
    IDLE: NotRequired[int],
    TERMINATING: NotRequired[int],
```

## TargetTrackingConfigurationTypeDef

```python
# TargetTrackingConfigurationTypeDef definition

class TargetTrackingConfigurationTypeDef(TypedDict):
    TargetValue: float,
```

## MatchedPlayerSessionTypeDef

```python
# MatchedPlayerSessionTypeDef definition

class MatchedPlayerSessionTypeDef(TypedDict):
    PlayerId: NotRequired[str],
    PlayerSessionId: NotRequired[str],
```

## PlacedPlayerSessionTypeDef

```python
# PlacedPlayerSessionTypeDef definition

class PlacedPlayerSessionTypeDef(TypedDict):
    PlayerId: NotRequired[str],
    PlayerSessionId: NotRequired[str],
```

## PlayerLatencyTypeDef

```python
# PlayerLatencyTypeDef definition

class PlayerLatencyTypeDef(TypedDict):
    PlayerId: NotRequired[str],
    RegionIdentifier: NotRequired[str],
    LatencyInMilliseconds: NotRequired[float],
```

## PriorityConfigurationOutputTypeDef

```python
# PriorityConfigurationOutputTypeDef definition

class PriorityConfigurationOutputTypeDef(TypedDict):
    PriorityOrder: NotRequired[List[PriorityTypeType]],  # (1)
    LocationOrder: NotRequired[List[str]],
```

1. See [:material-code-brackets: PriorityTypeType](./literals.md#prioritytypetype) 
## GetComputeAccessInputRequestTypeDef

```python
# GetComputeAccessInputRequestTypeDef definition

class GetComputeAccessInputRequestTypeDef(TypedDict):
    FleetId: str,
    ComputeName: str,
```

## GetComputeAuthTokenInputRequestTypeDef

```python
# GetComputeAuthTokenInputRequestTypeDef definition

class GetComputeAuthTokenInputRequestTypeDef(TypedDict):
    FleetId: str,
    ComputeName: str,
```

## GetGameSessionLogUrlInputRequestTypeDef

```python
# GetGameSessionLogUrlInputRequestTypeDef definition

class GetGameSessionLogUrlInputRequestTypeDef(TypedDict):
    GameSessionId: str,
```

## GetInstanceAccessInputRequestTypeDef

```python
# GetInstanceAccessInputRequestTypeDef definition

class GetInstanceAccessInputRequestTypeDef(TypedDict):
    FleetId: str,
    InstanceId: str,
```

## InstanceCredentialsTypeDef

```python
# InstanceCredentialsTypeDef definition

class InstanceCredentialsTypeDef(TypedDict):
    UserName: NotRequired[str],
    Secret: NotRequired[str],
```

## ListAliasesInputRequestTypeDef

```python
# ListAliasesInputRequestTypeDef definition

class ListAliasesInputRequestTypeDef(TypedDict):
    RoutingStrategyType: NotRequired[RoutingStrategyTypeType],  # (1)
    Name: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RoutingStrategyTypeType](./literals.md#routingstrategytypetype) 
## ListBuildsInputRequestTypeDef

```python
# ListBuildsInputRequestTypeDef definition

class ListBuildsInputRequestTypeDef(TypedDict):
    Status: NotRequired[BuildStatusType],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: BuildStatusType](./literals.md#buildstatustype) 
## ListComputeInputRequestTypeDef

```python
# ListComputeInputRequestTypeDef definition

class ListComputeInputRequestTypeDef(TypedDict):
    FleetId: str,
    Location: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListContainerGroupDefinitionsInputRequestTypeDef

```python
# ListContainerGroupDefinitionsInputRequestTypeDef definition

class ListContainerGroupDefinitionsInputRequestTypeDef(TypedDict):
    SchedulingStrategy: NotRequired[ContainerSchedulingStrategyType],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ContainerSchedulingStrategyType](./literals.md#containerschedulingstrategytype) 
## ListFleetsInputRequestTypeDef

```python
# ListFleetsInputRequestTypeDef definition

class ListFleetsInputRequestTypeDef(TypedDict):
    BuildId: NotRequired[str],
    ScriptId: NotRequired[str],
    ContainerGroupDefinitionName: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListGameServerGroupsInputRequestTypeDef

```python
# ListGameServerGroupsInputRequestTypeDef definition

class ListGameServerGroupsInputRequestTypeDef(TypedDict):
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListGameServersInputRequestTypeDef

```python
# ListGameServersInputRequestTypeDef definition

class ListGameServersInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    SortOrder: NotRequired[SortOrderType],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListLocationsInputRequestTypeDef

```python
# ListLocationsInputRequestTypeDef definition

class ListLocationsInputRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[LocationFilterType]],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: LocationFilterType](./literals.md#locationfiltertype) 
## ListScriptsInputRequestTypeDef

```python
# ListScriptsInputRequestTypeDef definition

class ListScriptsInputRequestTypeDef(TypedDict):
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## TargetConfigurationTypeDef

```python
# TargetConfigurationTypeDef definition

class TargetConfigurationTypeDef(TypedDict):
    TargetValue: float,
```

## RegisterComputeInputRequestTypeDef

```python
# RegisterComputeInputRequestTypeDef definition

class RegisterComputeInputRequestTypeDef(TypedDict):
    FleetId: str,
    ComputeName: str,
    CertificatePath: NotRequired[str],
    DnsName: NotRequired[str],
    IpAddress: NotRequired[str],
    Location: NotRequired[str],
```

## RegisterGameServerInputRequestTypeDef

```python
# RegisterGameServerInputRequestTypeDef definition

class RegisterGameServerInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    GameServerId: str,
    InstanceId: str,
    ConnectionInfo: NotRequired[str],
    GameServerData: NotRequired[str],
```

## RequestUploadCredentialsInputRequestTypeDef

```python
# RequestUploadCredentialsInputRequestTypeDef definition

class RequestUploadCredentialsInputRequestTypeDef(TypedDict):
    BuildId: str,
```

## ResolveAliasInputRequestTypeDef

```python
# ResolveAliasInputRequestTypeDef definition

class ResolveAliasInputRequestTypeDef(TypedDict):
    AliasId: str,
```

## ResumeGameServerGroupInputRequestTypeDef

```python
# ResumeGameServerGroupInputRequestTypeDef definition

class ResumeGameServerGroupInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    ResumeActions: Sequence[GameServerGroupActionType],  # (1)
```

1. See [:material-code-brackets: GameServerGroupActionType](./literals.md#gameservergroupactiontype) 
## ServerProcessTypeDef

```python
# ServerProcessTypeDef definition

class ServerProcessTypeDef(TypedDict):
    LaunchPath: str,
    ConcurrentExecutions: int,
    Parameters: NotRequired[str],
```

## SearchGameSessionsInputRequestTypeDef

```python
# SearchGameSessionsInputRequestTypeDef definition

class SearchGameSessionsInputRequestTypeDef(TypedDict):
    FleetId: NotRequired[str],
    AliasId: NotRequired[str],
    Location: NotRequired[str],
    FilterExpression: NotRequired[str],
    SortExpression: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## StartFleetActionsInputRequestTypeDef

```python
# StartFleetActionsInputRequestTypeDef definition

class StartFleetActionsInputRequestTypeDef(TypedDict):
    FleetId: str,
    Actions: Sequence[FleetActionType],  # (1)
    Location: NotRequired[str],
```

1. See [:material-code-brackets: FleetActionType](./literals.md#fleetactiontype) 
## StopFleetActionsInputRequestTypeDef

```python
# StopFleetActionsInputRequestTypeDef definition

class StopFleetActionsInputRequestTypeDef(TypedDict):
    FleetId: str,
    Actions: Sequence[FleetActionType],  # (1)
    Location: NotRequired[str],
```

1. See [:material-code-brackets: FleetActionType](./literals.md#fleetactiontype) 
## StopGameSessionPlacementInputRequestTypeDef

```python
# StopGameSessionPlacementInputRequestTypeDef definition

class StopGameSessionPlacementInputRequestTypeDef(TypedDict):
    PlacementId: str,
```

## StopMatchmakingInputRequestTypeDef

```python
# StopMatchmakingInputRequestTypeDef definition

class StopMatchmakingInputRequestTypeDef(TypedDict):
    TicketId: str,
```

## SuspendGameServerGroupInputRequestTypeDef

```python
# SuspendGameServerGroupInputRequestTypeDef definition

class SuspendGameServerGroupInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    SuspendActions: Sequence[GameServerGroupActionType],  # (1)
```

1. See [:material-code-brackets: GameServerGroupActionType](./literals.md#gameservergroupactiontype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateBuildInputRequestTypeDef

```python
# UpdateBuildInputRequestTypeDef definition

class UpdateBuildInputRequestTypeDef(TypedDict):
    BuildId: str,
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## UpdateFleetCapacityInputRequestTypeDef

```python
# UpdateFleetCapacityInputRequestTypeDef definition

class UpdateFleetCapacityInputRequestTypeDef(TypedDict):
    FleetId: str,
    DesiredInstances: NotRequired[int],
    MinSize: NotRequired[int],
    MaxSize: NotRequired[int],
    Location: NotRequired[str],
```

## UpdateGameServerInputRequestTypeDef

```python
# UpdateGameServerInputRequestTypeDef definition

class UpdateGameServerInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    GameServerId: str,
    GameServerData: NotRequired[str],
    UtilizationStatus: NotRequired[GameServerUtilizationStatusType],  # (1)
    HealthCheck: NotRequired[GameServerHealthCheckType],  # (2)
```

1. See [:material-code-brackets: GameServerUtilizationStatusType](./literals.md#gameserverutilizationstatustype) 
2. See [:material-code-brackets: GameServerHealthCheckType](./literals.md#gameserverhealthchecktype) 
## ValidateMatchmakingRuleSetInputRequestTypeDef

```python
# ValidateMatchmakingRuleSetInputRequestTypeDef definition

class ValidateMatchmakingRuleSetInputRequestTypeDef(TypedDict):
    RuleSetBody: str,
```

## VpcPeeringConnectionStatusTypeDef

```python
# VpcPeeringConnectionStatusTypeDef definition

class VpcPeeringConnectionStatusTypeDef(TypedDict):
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## AliasTypeDef

```python
# AliasTypeDef definition

class AliasTypeDef(TypedDict):
    AliasId: NotRequired[str],
    Name: NotRequired[str],
    AliasArn: NotRequired[str],
    Description: NotRequired[str],
    RoutingStrategy: NotRequired[RoutingStrategyTypeDef],  # (1)
    CreationTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-braces: RoutingStrategyTypeDef](./type_defs.md#routingstrategytypedef) 
## UpdateAliasInputRequestTypeDef

```python
# UpdateAliasInputRequestTypeDef definition

class UpdateAliasInputRequestTypeDef(TypedDict):
    AliasId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    RoutingStrategy: NotRequired[RoutingStrategyTypeDef],  # (1)
```

1. See [:material-code-braces: RoutingStrategyTypeDef](./type_defs.md#routingstrategytypedef) 
## PlayerOutputTypeDef

```python
# PlayerOutputTypeDef definition

class PlayerOutputTypeDef(TypedDict):
    PlayerId: NotRequired[str],
    PlayerAttributes: NotRequired[Dict[str, AttributeValueOutputTypeDef]],  # (1)
    Team: NotRequired[str],
    LatencyInMs: NotRequired[Dict[str, int]],
```

1. See [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 
## ClaimGameServerInputRequestTypeDef

```python
# ClaimGameServerInputRequestTypeDef definition

class ClaimGameServerInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    GameServerId: NotRequired[str],
    GameServerData: NotRequired[str],
    FilterOption: NotRequired[ClaimFilterOptionTypeDef],  # (1)
```

1. See [:material-code-braces: ClaimFilterOptionTypeDef](./type_defs.md#claimfilteroptiontypedef) 
## ClaimGameServerOutputTypeDef

```python
# ClaimGameServerOutputTypeDef definition

class ClaimGameServerOutputTypeDef(TypedDict):
    GameServer: GameServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameServerTypeDef](./type_defs.md#gameservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBuildOutputTypeDef

```python
# DescribeBuildOutputTypeDef definition

class DescribeBuildOutputTypeDef(TypedDict):
    Build: BuildTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildTypeDef](./type_defs.md#buildtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGameServerOutputTypeDef

```python
# DescribeGameServerOutputTypeDef definition

class DescribeGameServerOutputTypeDef(TypedDict):
    GameServer: GameServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameServerTypeDef](./type_defs.md#gameservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComputeAccessOutputTypeDef

```python
# GetComputeAccessOutputTypeDef definition

class GetComputeAccessOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    ComputeName: str,
    ComputeArn: str,
    Credentials: AwsCredentialsTypeDef,  # (1)
    Target: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComputeAuthTokenOutputTypeDef

```python
# GetComputeAuthTokenOutputTypeDef definition

class GetComputeAuthTokenOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    ComputeName: str,
    ComputeArn: str,
    AuthToken: str,
    ExpirationTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGameSessionLogUrlOutputTypeDef

```python
# GetGameSessionLogUrlOutputTypeDef definition

class GetGameSessionLogUrlOutputTypeDef(TypedDict):
    PreSignedUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBuildsOutputTypeDef

```python
# ListBuildsOutputTypeDef definition

class ListBuildsOutputTypeDef(TypedDict):
    Builds: List[BuildTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BuildTypeDef](./type_defs.md#buildtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFleetsOutputTypeDef

```python
# ListFleetsOutputTypeDef definition

class ListFleetsOutputTypeDef(TypedDict):
    FleetIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGameServersOutputTypeDef

```python
# ListGameServersOutputTypeDef definition

class ListGameServersOutputTypeDef(TypedDict):
    GameServers: List[GameServerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GameServerTypeDef](./type_defs.md#gameservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutScalingPolicyOutputTypeDef

```python
# PutScalingPolicyOutputTypeDef definition

class PutScalingPolicyOutputTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterGameServerOutputTypeDef

```python
# RegisterGameServerOutputTypeDef definition

class RegisterGameServerOutputTypeDef(TypedDict):
    GameServer: GameServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameServerTypeDef](./type_defs.md#gameservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResolveAliasOutputTypeDef

```python
# ResolveAliasOutputTypeDef definition

class ResolveAliasOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartFleetActionsOutputTypeDef

```python
# StartFleetActionsOutputTypeDef definition

class StartFleetActionsOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopFleetActionsOutputTypeDef

```python
# StopFleetActionsOutputTypeDef definition

class StopFleetActionsOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBuildOutputTypeDef

```python
# UpdateBuildOutputTypeDef definition

class UpdateBuildOutputTypeDef(TypedDict):
    Build: BuildTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildTypeDef](./type_defs.md#buildtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFleetAttributesOutputTypeDef

```python
# UpdateFleetAttributesOutputTypeDef definition

class UpdateFleetAttributesOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFleetCapacityOutputTypeDef

```python
# UpdateFleetCapacityOutputTypeDef definition

class UpdateFleetCapacityOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFleetPortSettingsOutputTypeDef

```python
# UpdateFleetPortSettingsOutputTypeDef definition

class UpdateFleetPortSettingsOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGameServerOutputTypeDef

```python
# UpdateGameServerOutputTypeDef definition

class UpdateGameServerOutputTypeDef(TypedDict):
    GameServer: GameServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameServerTypeDef](./type_defs.md#gameservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ValidateMatchmakingRuleSetOutputTypeDef

```python
# ValidateMatchmakingRuleSetOutputTypeDef definition

class ValidateMatchmakingRuleSetOutputTypeDef(TypedDict):
    Valid: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContainerGroupsConfigurationTypeDef

```python
# ContainerGroupsConfigurationTypeDef definition

class ContainerGroupsConfigurationTypeDef(TypedDict):
    ContainerGroupDefinitionNames: Sequence[str],
    ConnectionPortRange: ConnectionPortRangeTypeDef,  # (1)
    DesiredReplicaContainerGroupsPerInstance: NotRequired[int],
```

1. See [:material-code-braces: ConnectionPortRangeTypeDef](./type_defs.md#connectionportrangetypedef) 
## ContainerAttributesTypeDef

```python
# ContainerAttributesTypeDef definition

class ContainerAttributesTypeDef(TypedDict):
    ContainerPortMappings: NotRequired[List[ContainerPortMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: ContainerPortMappingTypeDef](./type_defs.md#containerportmappingtypedef) 
## ContainerGroupsAttributesTypeDef

```python
# ContainerGroupsAttributesTypeDef definition

class ContainerGroupsAttributesTypeDef(TypedDict):
    ContainerGroupDefinitionProperties: NotRequired[List[ContainerGroupDefinitionPropertyTypeDef]],  # (1)
    ConnectionPortRange: NotRequired[ConnectionPortRangeTypeDef],  # (2)
    ContainerGroupsPerInstance: NotRequired[ContainerGroupsPerInstanceTypeDef],  # (3)
```

1. See [:material-code-braces: ContainerGroupDefinitionPropertyTypeDef](./type_defs.md#containergroupdefinitionpropertytypedef) 
2. See [:material-code-braces: ConnectionPortRangeTypeDef](./type_defs.md#connectionportrangetypedef) 
3. See [:material-code-braces: ContainerGroupsPerInstanceTypeDef](./type_defs.md#containergroupsperinstancetypedef) 
## ContainerPortConfigurationOutputTypeDef

```python
# ContainerPortConfigurationOutputTypeDef definition

class ContainerPortConfigurationOutputTypeDef(TypedDict):
    ContainerPortRanges: List[ContainerPortRangeTypeDef],  # (1)
```

1. See [:material-code-braces: ContainerPortRangeTypeDef](./type_defs.md#containerportrangetypedef) 
## ContainerPortConfigurationTypeDef

```python
# ContainerPortConfigurationTypeDef definition

class ContainerPortConfigurationTypeDef(TypedDict):
    ContainerPortRanges: Sequence[ContainerPortRangeTypeDef],  # (1)
```

1. See [:material-code-braces: ContainerPortRangeTypeDef](./type_defs.md#containerportrangetypedef) 
## CreateAliasInputRequestTypeDef

```python
# CreateAliasInputRequestTypeDef definition

class CreateAliasInputRequestTypeDef(TypedDict):
    Name: str,
    RoutingStrategy: RoutingStrategyTypeDef,  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: RoutingStrategyTypeDef](./type_defs.md#routingstrategytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateLocationInputRequestTypeDef

```python
# CreateLocationInputRequestTypeDef definition

class CreateLocationInputRequestTypeDef(TypedDict):
    LocationName: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateMatchmakingRuleSetInputRequestTypeDef

```python
# CreateMatchmakingRuleSetInputRequestTypeDef definition

class CreateMatchmakingRuleSetInputRequestTypeDef(TypedDict):
    Name: str,
    RuleSetBody: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateBuildInputRequestTypeDef

```python
# CreateBuildInputRequestTypeDef definition

class CreateBuildInputRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
    StorageLocation: NotRequired[S3LocationTypeDef],  # (1)
    OperatingSystem: NotRequired[OperatingSystemType],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    ServerSdkVersion: NotRequired[str],
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateBuildOutputTypeDef

```python
# CreateBuildOutputTypeDef definition

class CreateBuildOutputTypeDef(TypedDict):
    Build: BuildTypeDef,  # (1)
    UploadCredentials: AwsCredentialsTypeDef,  # (2)
    StorageLocation: S3LocationTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: BuildTypeDef](./type_defs.md#buildtypedef) 
2. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScriptInputRequestTypeDef

```python
# CreateScriptInputRequestTypeDef definition

class CreateScriptInputRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
    StorageLocation: NotRequired[S3LocationTypeDef],  # (1)
    ZipFile: NotRequired[BlobTypeDef],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RequestUploadCredentialsOutputTypeDef

```python
# RequestUploadCredentialsOutputTypeDef definition

class RequestUploadCredentialsOutputTypeDef(TypedDict):
    UploadCredentials: AwsCredentialsTypeDef,  # (1)
    StorageLocation: S3LocationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScriptTypeDef

```python
# ScriptTypeDef definition

class ScriptTypeDef(TypedDict):
    ScriptId: NotRequired[str],
    ScriptArn: NotRequired[str],
    Name: NotRequired[str],
    Version: NotRequired[str],
    SizeOnDisk: NotRequired[int],
    CreationTime: NotRequired[datetime],
    StorageLocation: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## UpdateScriptInputRequestTypeDef

```python
# UpdateScriptInputRequestTypeDef definition

class UpdateScriptInputRequestTypeDef(TypedDict):
    ScriptId: str,
    Name: NotRequired[str],
    Version: NotRequired[str],
    StorageLocation: NotRequired[S3LocationTypeDef],  # (1)
    ZipFile: NotRequired[BlobTypeDef],
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## DescribeFleetPortSettingsOutputTypeDef

```python
# DescribeFleetPortSettingsOutputTypeDef definition

class DescribeFleetPortSettingsOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    InboundPermissions: List[IpPermissionTypeDef],  # (1)
    UpdateStatus: LocationUpdateStatusType,  # (2)
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: IpPermissionTypeDef](./type_defs.md#ippermissiontypedef) 
2. See [:material-code-brackets: LocationUpdateStatusType](./literals.md#locationupdatestatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFleetPortSettingsInputRequestTypeDef

```python
# UpdateFleetPortSettingsInputRequestTypeDef definition

class UpdateFleetPortSettingsInputRequestTypeDef(TypedDict):
    FleetId: str,
    InboundPermissionAuthorizations: NotRequired[Sequence[IpPermissionTypeDef]],  # (1)
    InboundPermissionRevocations: NotRequired[Sequence[IpPermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: IpPermissionTypeDef](./type_defs.md#ippermissiontypedef) 
2. See [:material-code-braces: IpPermissionTypeDef](./type_defs.md#ippermissiontypedef) 
## CreateFleetLocationsInputRequestTypeDef

```python
# CreateFleetLocationsInputRequestTypeDef definition

class CreateFleetLocationsInputRequestTypeDef(TypedDict):
    FleetId: str,
    Locations: Sequence[LocationConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: LocationConfigurationTypeDef](./type_defs.md#locationconfigurationtypedef) 
## UpdateFleetAttributesInputRequestTypeDef

```python
# UpdateFleetAttributesInputRequestTypeDef definition

class UpdateFleetAttributesInputRequestTypeDef(TypedDict):
    FleetId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    NewGameSessionProtectionPolicy: NotRequired[ProtectionPolicyType],  # (1)
    ResourceCreationLimitPolicy: NotRequired[ResourceCreationLimitPolicyTypeDef],  # (2)
    MetricGroups: NotRequired[Sequence[str]],
    AnywhereConfiguration: NotRequired[AnywhereConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: ProtectionPolicyType](./literals.md#protectionpolicytype) 
2. See [:material-code-braces: ResourceCreationLimitPolicyTypeDef](./type_defs.md#resourcecreationlimitpolicytypedef) 
3. See [:material-code-braces: AnywhereConfigurationTypeDef](./type_defs.md#anywhereconfigurationtypedef) 
## CreateFleetLocationsOutputTypeDef

```python
# CreateFleetLocationsOutputTypeDef definition

class CreateFleetLocationsOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    LocationStates: List[LocationStateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LocationStateTypeDef](./type_defs.md#locationstatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFleetLocationsOutputTypeDef

```python
# DeleteFleetLocationsOutputTypeDef definition

class DeleteFleetLocationsOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    LocationStates: List[LocationStateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LocationStateTypeDef](./type_defs.md#locationstatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LocationAttributesTypeDef

```python
# LocationAttributesTypeDef definition

class LocationAttributesTypeDef(TypedDict):
    LocationState: NotRequired[LocationStateTypeDef],  # (1)
    StoppedActions: NotRequired[List[FleetActionType]],  # (2)
    UpdateStatus: NotRequired[LocationUpdateStatusType],  # (3)
```

1. See [:material-code-braces: LocationStateTypeDef](./type_defs.md#locationstatetypedef) 
2. See [:material-code-brackets: FleetActionType](./literals.md#fleetactiontype) 
3. See [:material-code-brackets: LocationUpdateStatusType](./literals.md#locationupdatestatustype) 
## GameServerGroupTypeDef

```python
# GameServerGroupTypeDef definition

class GameServerGroupTypeDef(TypedDict):
    GameServerGroupName: NotRequired[str],
    GameServerGroupArn: NotRequired[str],
    RoleArn: NotRequired[str],
    InstanceDefinitions: NotRequired[List[InstanceDefinitionTypeDef]],  # (1)
    BalancingStrategy: NotRequired[BalancingStrategyType],  # (2)
    GameServerProtectionPolicy: NotRequired[GameServerProtectionPolicyType],  # (3)
    AutoScalingGroupArn: NotRequired[str],
    Status: NotRequired[GameServerGroupStatusType],  # (4)
    StatusReason: NotRequired[str],
    SuspendedActions: NotRequired[List[GameServerGroupActionType]],  # (5)
    CreationTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-braces: InstanceDefinitionTypeDef](./type_defs.md#instancedefinitiontypedef) 
2. See [:material-code-brackets: BalancingStrategyType](./literals.md#balancingstrategytype) 
3. See [:material-code-brackets: GameServerProtectionPolicyType](./literals.md#gameserverprotectionpolicytype) 
4. See [:material-code-brackets: GameServerGroupStatusType](./literals.md#gameservergroupstatustype) 
5. See [:material-code-brackets: GameServerGroupActionType](./literals.md#gameservergroupactiontype) 
## UpdateGameServerGroupInputRequestTypeDef

```python
# UpdateGameServerGroupInputRequestTypeDef definition

class UpdateGameServerGroupInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    RoleArn: NotRequired[str],
    InstanceDefinitions: NotRequired[Sequence[InstanceDefinitionTypeDef]],  # (1)
    GameServerProtectionPolicy: NotRequired[GameServerProtectionPolicyType],  # (2)
    BalancingStrategy: NotRequired[BalancingStrategyType],  # (3)
```

1. See [:material-code-braces: InstanceDefinitionTypeDef](./type_defs.md#instancedefinitiontypedef) 
2. See [:material-code-brackets: GameServerProtectionPolicyType](./literals.md#gameserverprotectionpolicytype) 
3. See [:material-code-brackets: BalancingStrategyType](./literals.md#balancingstrategytype) 
## CreateGameSessionInputRequestTypeDef

```python
# CreateGameSessionInputRequestTypeDef definition

class CreateGameSessionInputRequestTypeDef(TypedDict):
    MaximumPlayerSessionCount: int,
    FleetId: NotRequired[str],
    AliasId: NotRequired[str],
    Name: NotRequired[str],
    GameProperties: NotRequired[Sequence[GamePropertyTypeDef]],  # (1)
    CreatorId: NotRequired[str],
    GameSessionId: NotRequired[str],
    IdempotencyToken: NotRequired[str],
    GameSessionData: NotRequired[str],
    Location: NotRequired[str],
```

1. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
## CreateMatchmakingConfigurationInputRequestTypeDef

```python
# CreateMatchmakingConfigurationInputRequestTypeDef definition

class CreateMatchmakingConfigurationInputRequestTypeDef(TypedDict):
    Name: str,
    RequestTimeoutSeconds: int,
    AcceptanceRequired: bool,
    RuleSetName: str,
    Description: NotRequired[str],
    GameSessionQueueArns: NotRequired[Sequence[str]],
    AcceptanceTimeoutSeconds: NotRequired[int],
    NotificationTarget: NotRequired[str],
    AdditionalPlayerCount: NotRequired[int],
    CustomEventData: NotRequired[str],
    GameProperties: NotRequired[Sequence[GamePropertyTypeDef]],  # (1)
    GameSessionData: NotRequired[str],
    BackfillMode: NotRequired[BackfillModeType],  # (2)
    FlexMatchMode: NotRequired[FlexMatchModeType],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
2. See [:material-code-brackets: BackfillModeType](./literals.md#backfillmodetype) 
3. See [:material-code-brackets: FlexMatchModeType](./literals.md#flexmatchmodetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GameSessionTypeDef

```python
# GameSessionTypeDef definition

class GameSessionTypeDef(TypedDict):
    GameSessionId: NotRequired[str],
    Name: NotRequired[str],
    FleetId: NotRequired[str],
    FleetArn: NotRequired[str],
    CreationTime: NotRequired[datetime],
    TerminationTime: NotRequired[datetime],
    CurrentPlayerSessionCount: NotRequired[int],
    MaximumPlayerSessionCount: NotRequired[int],
    Status: NotRequired[GameSessionStatusType],  # (1)
    StatusReason: NotRequired[GameSessionStatusReasonType],  # (2)
    GameProperties: NotRequired[List[GamePropertyTypeDef]],  # (3)
    IpAddress: NotRequired[str],
    DnsName: NotRequired[str],
    Port: NotRequired[int],
    PlayerSessionCreationPolicy: NotRequired[PlayerSessionCreationPolicyType],  # (4)
    CreatorId: NotRequired[str],
    GameSessionData: NotRequired[str],
    MatchmakerData: NotRequired[str],
    Location: NotRequired[str],
```

1. See [:material-code-brackets: GameSessionStatusType](./literals.md#gamesessionstatustype) 
2. See [:material-code-brackets: GameSessionStatusReasonType](./literals.md#gamesessionstatusreasontype) 
3. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
4. See [:material-code-brackets: PlayerSessionCreationPolicyType](./literals.md#playersessioncreationpolicytype) 
## MatchmakingConfigurationTypeDef

```python
# MatchmakingConfigurationTypeDef definition

class MatchmakingConfigurationTypeDef(TypedDict):
    Name: NotRequired[str],
    ConfigurationArn: NotRequired[str],
    Description: NotRequired[str],
    GameSessionQueueArns: NotRequired[List[str]],
    RequestTimeoutSeconds: NotRequired[int],
    AcceptanceTimeoutSeconds: NotRequired[int],
    AcceptanceRequired: NotRequired[bool],
    RuleSetName: NotRequired[str],
    RuleSetArn: NotRequired[str],
    NotificationTarget: NotRequired[str],
    AdditionalPlayerCount: NotRequired[int],
    CustomEventData: NotRequired[str],
    CreationTime: NotRequired[datetime],
    GameProperties: NotRequired[List[GamePropertyTypeDef]],  # (1)
    GameSessionData: NotRequired[str],
    BackfillMode: NotRequired[BackfillModeType],  # (2)
    FlexMatchMode: NotRequired[FlexMatchModeType],  # (3)
```

1. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
2. See [:material-code-brackets: BackfillModeType](./literals.md#backfillmodetype) 
3. See [:material-code-brackets: FlexMatchModeType](./literals.md#flexmatchmodetype) 
## UpdateGameSessionInputRequestTypeDef

```python
# UpdateGameSessionInputRequestTypeDef definition

class UpdateGameSessionInputRequestTypeDef(TypedDict):
    GameSessionId: str,
    MaximumPlayerSessionCount: NotRequired[int],
    Name: NotRequired[str],
    PlayerSessionCreationPolicy: NotRequired[PlayerSessionCreationPolicyType],  # (1)
    ProtectionPolicy: NotRequired[ProtectionPolicyType],  # (2)
    GameProperties: NotRequired[Sequence[GamePropertyTypeDef]],  # (3)
```

1. See [:material-code-brackets: PlayerSessionCreationPolicyType](./literals.md#playersessioncreationpolicytype) 
2. See [:material-code-brackets: ProtectionPolicyType](./literals.md#protectionpolicytype) 
3. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
## UpdateMatchmakingConfigurationInputRequestTypeDef

```python
# UpdateMatchmakingConfigurationInputRequestTypeDef definition

class UpdateMatchmakingConfigurationInputRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    GameSessionQueueArns: NotRequired[Sequence[str]],
    RequestTimeoutSeconds: NotRequired[int],
    AcceptanceTimeoutSeconds: NotRequired[int],
    AcceptanceRequired: NotRequired[bool],
    RuleSetName: NotRequired[str],
    NotificationTarget: NotRequired[str],
    AdditionalPlayerCount: NotRequired[int],
    CustomEventData: NotRequired[str],
    GameProperties: NotRequired[Sequence[GamePropertyTypeDef]],  # (1)
    GameSessionData: NotRequired[str],
    BackfillMode: NotRequired[BackfillModeType],  # (2)
    FlexMatchMode: NotRequired[FlexMatchModeType],  # (3)
```

1. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
2. See [:material-code-brackets: BackfillModeType](./literals.md#backfillmodetype) 
3. See [:material-code-brackets: FlexMatchModeType](./literals.md#flexmatchmodetype) 
## CreateGameSessionQueueInputRequestTypeDef

```python
# CreateGameSessionQueueInputRequestTypeDef definition

class CreateGameSessionQueueInputRequestTypeDef(TypedDict):
    Name: str,
    TimeoutInSeconds: NotRequired[int],
    PlayerLatencyPolicies: NotRequired[Sequence[PlayerLatencyPolicyTypeDef]],  # (1)
    Destinations: NotRequired[Sequence[GameSessionQueueDestinationTypeDef]],  # (2)
    FilterConfiguration: NotRequired[FilterConfigurationTypeDef],  # (3)
    PriorityConfiguration: NotRequired[PriorityConfigurationTypeDef],  # (4)
    CustomEventData: NotRequired[str],
    NotificationTarget: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: PlayerLatencyPolicyTypeDef](./type_defs.md#playerlatencypolicytypedef) 
2. See [:material-code-braces: GameSessionQueueDestinationTypeDef](./type_defs.md#gamesessionqueuedestinationtypedef) 
3. See [:material-code-braces: FilterConfigurationTypeDef](./type_defs.md#filterconfigurationtypedef) 
4. See [:material-code-braces: PriorityConfigurationTypeDef](./type_defs.md#priorityconfigurationtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateGameSessionQueueInputRequestTypeDef

```python
# UpdateGameSessionQueueInputRequestTypeDef definition

class UpdateGameSessionQueueInputRequestTypeDef(TypedDict):
    Name: str,
    TimeoutInSeconds: NotRequired[int],
    PlayerLatencyPolicies: NotRequired[Sequence[PlayerLatencyPolicyTypeDef]],  # (1)
    Destinations: NotRequired[Sequence[GameSessionQueueDestinationTypeDef]],  # (2)
    FilterConfiguration: NotRequired[FilterConfigurationTypeDef],  # (3)
    PriorityConfiguration: NotRequired[PriorityConfigurationTypeDef],  # (4)
    CustomEventData: NotRequired[str],
    NotificationTarget: NotRequired[str],
```

1. See [:material-code-braces: PlayerLatencyPolicyTypeDef](./type_defs.md#playerlatencypolicytypedef) 
2. See [:material-code-braces: GameSessionQueueDestinationTypeDef](./type_defs.md#gamesessionqueuedestinationtypedef) 
3. See [:material-code-braces: FilterConfigurationTypeDef](./type_defs.md#filterconfigurationtypedef) 
4. See [:material-code-braces: PriorityConfigurationTypeDef](./type_defs.md#priorityconfigurationtypedef) 
## CreateLocationOutputTypeDef

```python
# CreateLocationOutputTypeDef definition

class CreateLocationOutputTypeDef(TypedDict):
    Location: LocationModelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LocationModelTypeDef](./type_defs.md#locationmodeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLocationsOutputTypeDef

```python
# ListLocationsOutputTypeDef definition

class ListLocationsOutputTypeDef(TypedDict):
    Locations: List[LocationModelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LocationModelTypeDef](./type_defs.md#locationmodeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMatchmakingRuleSetOutputTypeDef

```python
# CreateMatchmakingRuleSetOutputTypeDef definition

class CreateMatchmakingRuleSetOutputTypeDef(TypedDict):
    RuleSet: MatchmakingRuleSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MatchmakingRuleSetTypeDef](./type_defs.md#matchmakingrulesettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMatchmakingRuleSetsOutputTypeDef

```python
# DescribeMatchmakingRuleSetsOutputTypeDef definition

class DescribeMatchmakingRuleSetsOutputTypeDef(TypedDict):
    RuleSets: List[MatchmakingRuleSetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MatchmakingRuleSetTypeDef](./type_defs.md#matchmakingrulesettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePlayerSessionOutputTypeDef

```python
# CreatePlayerSessionOutputTypeDef definition

class CreatePlayerSessionOutputTypeDef(TypedDict):
    PlayerSession: PlayerSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlayerSessionTypeDef](./type_defs.md#playersessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePlayerSessionsOutputTypeDef

```python
# CreatePlayerSessionsOutputTypeDef definition

class CreatePlayerSessionsOutputTypeDef(TypedDict):
    PlayerSessions: List[PlayerSessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlayerSessionTypeDef](./type_defs.md#playersessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePlayerSessionsOutputTypeDef

```python
# DescribePlayerSessionsOutputTypeDef definition

class DescribePlayerSessionsOutputTypeDef(TypedDict):
    PlayerSessions: List[PlayerSessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PlayerSessionTypeDef](./type_defs.md#playersessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVpcPeeringAuthorizationOutputTypeDef

```python
# CreateVpcPeeringAuthorizationOutputTypeDef definition

class CreateVpcPeeringAuthorizationOutputTypeDef(TypedDict):
    VpcPeeringAuthorization: VpcPeeringAuthorizationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VpcPeeringAuthorizationTypeDef](./type_defs.md#vpcpeeringauthorizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVpcPeeringAuthorizationsOutputTypeDef

```python
# DescribeVpcPeeringAuthorizationsOutputTypeDef definition

class DescribeVpcPeeringAuthorizationsOutputTypeDef(TypedDict):
    VpcPeeringAuthorizations: List[VpcPeeringAuthorizationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VpcPeeringAuthorizationTypeDef](./type_defs.md#vpcpeeringauthorizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEC2InstanceLimitsOutputTypeDef

```python
# DescribeEC2InstanceLimitsOutputTypeDef definition

class DescribeEC2InstanceLimitsOutputTypeDef(TypedDict):
    EC2InstanceLimits: List[EC2InstanceLimitTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EC2InstanceLimitTypeDef](./type_defs.md#ec2instancelimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetAttributesInputDescribeFleetAttributesPaginateTypeDef

```python
# DescribeFleetAttributesInputDescribeFleetAttributesPaginateTypeDef definition

class DescribeFleetAttributesInputDescribeFleetAttributesPaginateTypeDef(TypedDict):
    FleetIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeFleetCapacityInputDescribeFleetCapacityPaginateTypeDef

```python
# DescribeFleetCapacityInputDescribeFleetCapacityPaginateTypeDef definition

class DescribeFleetCapacityInputDescribeFleetCapacityPaginateTypeDef(TypedDict):
    FleetIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef

```python
# DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef definition

class DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef(TypedDict):
    FleetIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef

```python
# DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef definition

class DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef(TypedDict):
    GameServerGroupName: str,
    InstanceIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeGameSessionDetailsInputDescribeGameSessionDetailsPaginateTypeDef

```python
# DescribeGameSessionDetailsInputDescribeGameSessionDetailsPaginateTypeDef definition

class DescribeGameSessionDetailsInputDescribeGameSessionDetailsPaginateTypeDef(TypedDict):
    FleetId: NotRequired[str],
    GameSessionId: NotRequired[str],
    AliasId: NotRequired[str],
    Location: NotRequired[str],
    StatusFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeGameSessionQueuesInputDescribeGameSessionQueuesPaginateTypeDef

```python
# DescribeGameSessionQueuesInputDescribeGameSessionQueuesPaginateTypeDef definition

class DescribeGameSessionQueuesInputDescribeGameSessionQueuesPaginateTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeGameSessionsInputDescribeGameSessionsPaginateTypeDef

```python
# DescribeGameSessionsInputDescribeGameSessionsPaginateTypeDef definition

class DescribeGameSessionsInputDescribeGameSessionsPaginateTypeDef(TypedDict):
    FleetId: NotRequired[str],
    GameSessionId: NotRequired[str],
    AliasId: NotRequired[str],
    Location: NotRequired[str],
    StatusFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInstancesInputDescribeInstancesPaginateTypeDef

```python
# DescribeInstancesInputDescribeInstancesPaginateTypeDef definition

class DescribeInstancesInputDescribeInstancesPaginateTypeDef(TypedDict):
    FleetId: str,
    InstanceId: NotRequired[str],
    Location: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef

```python
# DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef definition

class DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    RuleSetName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMatchmakingRuleSetsInputDescribeMatchmakingRuleSetsPaginateTypeDef

```python
# DescribeMatchmakingRuleSetsInputDescribeMatchmakingRuleSetsPaginateTypeDef definition

class DescribeMatchmakingRuleSetsInputDescribeMatchmakingRuleSetsPaginateTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePlayerSessionsInputDescribePlayerSessionsPaginateTypeDef

```python
# DescribePlayerSessionsInputDescribePlayerSessionsPaginateTypeDef definition

class DescribePlayerSessionsInputDescribePlayerSessionsPaginateTypeDef(TypedDict):
    GameSessionId: NotRequired[str],
    PlayerId: NotRequired[str],
    PlayerSessionId: NotRequired[str],
    PlayerSessionStatusFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef

```python
# DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef definition

class DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef(TypedDict):
    FleetId: str,
    StatusFilter: NotRequired[ScalingStatusTypeType],  # (1)
    Location: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ScalingStatusTypeType](./literals.md#scalingstatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAliasesInputListAliasesPaginateTypeDef

```python
# ListAliasesInputListAliasesPaginateTypeDef definition

class ListAliasesInputListAliasesPaginateTypeDef(TypedDict):
    RoutingStrategyType: NotRequired[RoutingStrategyTypeType],  # (1)
    Name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: RoutingStrategyTypeType](./literals.md#routingstrategytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBuildsInputListBuildsPaginateTypeDef

```python
# ListBuildsInputListBuildsPaginateTypeDef definition

class ListBuildsInputListBuildsPaginateTypeDef(TypedDict):
    Status: NotRequired[BuildStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: BuildStatusType](./literals.md#buildstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComputeInputListComputePaginateTypeDef

```python
# ListComputeInputListComputePaginateTypeDef definition

class ListComputeInputListComputePaginateTypeDef(TypedDict):
    FleetId: str,
    Location: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContainerGroupDefinitionsInputListContainerGroupDefinitionsPaginateTypeDef

```python
# ListContainerGroupDefinitionsInputListContainerGroupDefinitionsPaginateTypeDef definition

class ListContainerGroupDefinitionsInputListContainerGroupDefinitionsPaginateTypeDef(TypedDict):
    SchedulingStrategy: NotRequired[ContainerSchedulingStrategyType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ContainerSchedulingStrategyType](./literals.md#containerschedulingstrategytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFleetsInputListFleetsPaginateTypeDef

```python
# ListFleetsInputListFleetsPaginateTypeDef definition

class ListFleetsInputListFleetsPaginateTypeDef(TypedDict):
    BuildId: NotRequired[str],
    ScriptId: NotRequired[str],
    ContainerGroupDefinitionName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef

```python
# ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef definition

class ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGameServersInputListGameServersPaginateTypeDef

```python
# ListGameServersInputListGameServersPaginateTypeDef definition

class ListGameServersInputListGameServersPaginateTypeDef(TypedDict):
    GameServerGroupName: str,
    SortOrder: NotRequired[SortOrderType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLocationsInputListLocationsPaginateTypeDef

```python
# ListLocationsInputListLocationsPaginateTypeDef definition

class ListLocationsInputListLocationsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[LocationFilterType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LocationFilterType](./literals.md#locationfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListScriptsInputListScriptsPaginateTypeDef

```python
# ListScriptsInputListScriptsPaginateTypeDef definition

class ListScriptsInputListScriptsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchGameSessionsInputSearchGameSessionsPaginateTypeDef

```python
# SearchGameSessionsInputSearchGameSessionsPaginateTypeDef definition

class SearchGameSessionsInputSearchGameSessionsPaginateTypeDef(TypedDict):
    FleetId: NotRequired[str],
    AliasId: NotRequired[str],
    Location: NotRequired[str],
    FilterExpression: NotRequired[str],
    SortExpression: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef

```python
# DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef definition

class DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef(TypedDict):
    FleetId: str,
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeFleetEventsInputRequestTypeDef

```python
# DescribeFleetEventsInputRequestTypeDef definition

class DescribeFleetEventsInputRequestTypeDef(TypedDict):
    FleetId: str,
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeFleetEventsOutputTypeDef

```python
# DescribeFleetEventsOutputTypeDef definition

class DescribeFleetEventsOutputTypeDef(TypedDict):
    Events: List[EventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetLocationUtilizationOutputTypeDef

```python
# DescribeFleetLocationUtilizationOutputTypeDef definition

class DescribeFleetLocationUtilizationOutputTypeDef(TypedDict):
    FleetUtilization: FleetUtilizationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FleetUtilizationTypeDef](./type_defs.md#fleetutilizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetUtilizationOutputTypeDef

```python
# DescribeFleetUtilizationOutputTypeDef definition

class DescribeFleetUtilizationOutputTypeDef(TypedDict):
    FleetUtilization: List[FleetUtilizationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetUtilizationTypeDef](./type_defs.md#fleetutilizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGameServerInstancesOutputTypeDef

```python
# DescribeGameServerInstancesOutputTypeDef definition

class DescribeGameServerInstancesOutputTypeDef(TypedDict):
    GameServerInstances: List[GameServerInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GameServerInstanceTypeDef](./type_defs.md#gameserverinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInstancesOutputTypeDef

```python
# DescribeInstancesOutputTypeDef definition

class DescribeInstancesOutputTypeDef(TypedDict):
    Instances: List[InstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FleetCapacityTypeDef

```python
# FleetCapacityTypeDef definition

class FleetCapacityTypeDef(TypedDict):
    FleetId: NotRequired[str],
    FleetArn: NotRequired[str],
    InstanceType: NotRequired[EC2InstanceTypeType],  # (1)
    InstanceCounts: NotRequired[EC2InstanceCountsTypeDef],  # (2)
    Location: NotRequired[str],
    ReplicaContainerGroupCounts: NotRequired[ReplicaContainerGroupCountsTypeDef],  # (3)
```

1. See [:material-code-brackets: EC2InstanceTypeType](./literals.md#ec2instancetypetype) 
2. See [:material-code-braces: EC2InstanceCountsTypeDef](./type_defs.md#ec2instancecountstypedef) 
3. See [:material-code-braces: ReplicaContainerGroupCountsTypeDef](./type_defs.md#replicacontainergroupcountstypedef) 
## GameServerGroupAutoScalingPolicyTypeDef

```python
# GameServerGroupAutoScalingPolicyTypeDef definition

class GameServerGroupAutoScalingPolicyTypeDef(TypedDict):
    TargetTrackingConfiguration: TargetTrackingConfigurationTypeDef,  # (1)
    EstimatedInstanceWarmup: NotRequired[int],
```

1. See [:material-code-braces: TargetTrackingConfigurationTypeDef](./type_defs.md#targettrackingconfigurationtypedef) 
## GameSessionConnectionInfoTypeDef

```python
# GameSessionConnectionInfoTypeDef definition

class GameSessionConnectionInfoTypeDef(TypedDict):
    GameSessionArn: NotRequired[str],
    IpAddress: NotRequired[str],
    DnsName: NotRequired[str],
    Port: NotRequired[int],
    MatchedPlayerSessions: NotRequired[List[MatchedPlayerSessionTypeDef]],  # (1)
```

1. See [:material-code-braces: MatchedPlayerSessionTypeDef](./type_defs.md#matchedplayersessiontypedef) 
## GameSessionPlacementTypeDef

```python
# GameSessionPlacementTypeDef definition

class GameSessionPlacementTypeDef(TypedDict):
    PlacementId: NotRequired[str],
    GameSessionQueueName: NotRequired[str],
    Status: NotRequired[GameSessionPlacementStateType],  # (1)
    GameProperties: NotRequired[List[GamePropertyTypeDef]],  # (2)
    MaximumPlayerSessionCount: NotRequired[int],
    GameSessionName: NotRequired[str],
    GameSessionId: NotRequired[str],
    GameSessionArn: NotRequired[str],
    GameSessionRegion: NotRequired[str],
    PlayerLatencies: NotRequired[List[PlayerLatencyTypeDef]],  # (3)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    IpAddress: NotRequired[str],
    DnsName: NotRequired[str],
    Port: NotRequired[int],
    PlacedPlayerSessions: NotRequired[List[PlacedPlayerSessionTypeDef]],  # (4)
    GameSessionData: NotRequired[str],
    MatchmakerData: NotRequired[str],
```

1. See [:material-code-brackets: GameSessionPlacementStateType](./literals.md#gamesessionplacementstatetype) 
2. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
3. See [:material-code-braces: PlayerLatencyTypeDef](./type_defs.md#playerlatencytypedef) 
4. See [:material-code-braces: PlacedPlayerSessionTypeDef](./type_defs.md#placedplayersessiontypedef) 
## StartGameSessionPlacementInputRequestTypeDef

```python
# StartGameSessionPlacementInputRequestTypeDef definition

class StartGameSessionPlacementInputRequestTypeDef(TypedDict):
    PlacementId: str,
    GameSessionQueueName: str,
    MaximumPlayerSessionCount: int,
    GameProperties: NotRequired[Sequence[GamePropertyTypeDef]],  # (1)
    GameSessionName: NotRequired[str],
    PlayerLatencies: NotRequired[Sequence[PlayerLatencyTypeDef]],  # (2)
    DesiredPlayerSessions: NotRequired[Sequence[DesiredPlayerSessionTypeDef]],  # (3)
    GameSessionData: NotRequired[str],
```

1. See [:material-code-braces: GamePropertyTypeDef](./type_defs.md#gamepropertytypedef) 
2. See [:material-code-braces: PlayerLatencyTypeDef](./type_defs.md#playerlatencytypedef) 
3. See [:material-code-braces: DesiredPlayerSessionTypeDef](./type_defs.md#desiredplayersessiontypedef) 
## GameSessionQueueTypeDef

```python
# GameSessionQueueTypeDef definition

class GameSessionQueueTypeDef(TypedDict):
    Name: NotRequired[str],
    GameSessionQueueArn: NotRequired[str],
    TimeoutInSeconds: NotRequired[int],
    PlayerLatencyPolicies: NotRequired[List[PlayerLatencyPolicyTypeDef]],  # (1)
    Destinations: NotRequired[List[GameSessionQueueDestinationTypeDef]],  # (2)
    FilterConfiguration: NotRequired[FilterConfigurationOutputTypeDef],  # (3)
    PriorityConfiguration: NotRequired[PriorityConfigurationOutputTypeDef],  # (4)
    CustomEventData: NotRequired[str],
    NotificationTarget: NotRequired[str],
```

1. See [:material-code-braces: PlayerLatencyPolicyTypeDef](./type_defs.md#playerlatencypolicytypedef) 
2. See [:material-code-braces: GameSessionQueueDestinationTypeDef](./type_defs.md#gamesessionqueuedestinationtypedef) 
3. See [:material-code-braces: FilterConfigurationOutputTypeDef](./type_defs.md#filterconfigurationoutputtypedef) 
4. See [:material-code-braces: PriorityConfigurationOutputTypeDef](./type_defs.md#priorityconfigurationoutputtypedef) 
## InstanceAccessTypeDef

```python
# InstanceAccessTypeDef definition

class InstanceAccessTypeDef(TypedDict):
    FleetId: NotRequired[str],
    InstanceId: NotRequired[str],
    IpAddress: NotRequired[str],
    OperatingSystem: NotRequired[OperatingSystemType],  # (1)
    Credentials: NotRequired[InstanceCredentialsTypeDef],  # (2)
```

1. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
2. See [:material-code-braces: InstanceCredentialsTypeDef](./type_defs.md#instancecredentialstypedef) 
## PutScalingPolicyInputRequestTypeDef

```python
# PutScalingPolicyInputRequestTypeDef definition

class PutScalingPolicyInputRequestTypeDef(TypedDict):
    Name: str,
    FleetId: str,
    MetricName: MetricNameType,  # (1)
    ScalingAdjustment: NotRequired[int],
    ScalingAdjustmentType: NotRequired[ScalingAdjustmentTypeType],  # (2)
    Threshold: NotRequired[float],
    ComparisonOperator: NotRequired[ComparisonOperatorTypeType],  # (3)
    EvaluationPeriods: NotRequired[int],
    PolicyType: NotRequired[PolicyTypeType],  # (4)
    TargetConfiguration: NotRequired[TargetConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: MetricNameType](./literals.md#metricnametype) 
2. See [:material-code-brackets: ScalingAdjustmentTypeType](./literals.md#scalingadjustmenttypetype) 
3. See [:material-code-brackets: ComparisonOperatorTypeType](./literals.md#comparisonoperatortypetype) 
4. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
5. See [:material-code-braces: TargetConfigurationTypeDef](./type_defs.md#targetconfigurationtypedef) 
## ScalingPolicyTypeDef

```python
# ScalingPolicyTypeDef definition

class ScalingPolicyTypeDef(TypedDict):
    FleetId: NotRequired[str],
    FleetArn: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ScalingStatusTypeType],  # (1)
    ScalingAdjustment: NotRequired[int],
    ScalingAdjustmentType: NotRequired[ScalingAdjustmentTypeType],  # (2)
    ComparisonOperator: NotRequired[ComparisonOperatorTypeType],  # (3)
    Threshold: NotRequired[float],
    EvaluationPeriods: NotRequired[int],
    MetricName: NotRequired[MetricNameType],  # (4)
    PolicyType: NotRequired[PolicyTypeType],  # (5)
    TargetConfiguration: NotRequired[TargetConfigurationTypeDef],  # (6)
    UpdateStatus: NotRequired[LocationUpdateStatusType],  # (7)
    Location: NotRequired[str],
```

1. See [:material-code-brackets: ScalingStatusTypeType](./literals.md#scalingstatustypetype) 
2. See [:material-code-brackets: ScalingAdjustmentTypeType](./literals.md#scalingadjustmenttypetype) 
3. See [:material-code-brackets: ComparisonOperatorTypeType](./literals.md#comparisonoperatortypetype) 
4. See [:material-code-brackets: MetricNameType](./literals.md#metricnametype) 
5. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
6. See [:material-code-braces: TargetConfigurationTypeDef](./type_defs.md#targetconfigurationtypedef) 
7. See [:material-code-brackets: LocationUpdateStatusType](./literals.md#locationupdatestatustype) 
## RuntimeConfigurationOutputTypeDef

```python
# RuntimeConfigurationOutputTypeDef definition

class RuntimeConfigurationOutputTypeDef(TypedDict):
    ServerProcesses: NotRequired[List[ServerProcessTypeDef]],  # (1)
    MaxConcurrentGameSessionActivations: NotRequired[int],
    GameSessionActivationTimeoutSeconds: NotRequired[int],
```

1. See [:material-code-braces: ServerProcessTypeDef](./type_defs.md#serverprocesstypedef) 
## RuntimeConfigurationTypeDef

```python
# RuntimeConfigurationTypeDef definition

class RuntimeConfigurationTypeDef(TypedDict):
    ServerProcesses: NotRequired[Sequence[ServerProcessTypeDef]],  # (1)
    MaxConcurrentGameSessionActivations: NotRequired[int],
    GameSessionActivationTimeoutSeconds: NotRequired[int],
```

1. See [:material-code-braces: ServerProcessTypeDef](./type_defs.md#serverprocesstypedef) 
## VpcPeeringConnectionTypeDef

```python
# VpcPeeringConnectionTypeDef definition

class VpcPeeringConnectionTypeDef(TypedDict):
    FleetId: NotRequired[str],
    FleetArn: NotRequired[str],
    IpV4CidrBlock: NotRequired[str],
    VpcPeeringConnectionId: NotRequired[str],
    Status: NotRequired[VpcPeeringConnectionStatusTypeDef],  # (1)
    PeerVpcId: NotRequired[str],
    GameLiftVpcId: NotRequired[str],
```

1. See [:material-code-braces: VpcPeeringConnectionStatusTypeDef](./type_defs.md#vpcpeeringconnectionstatustypedef) 
## CreateAliasOutputTypeDef

```python
# CreateAliasOutputTypeDef definition

class CreateAliasOutputTypeDef(TypedDict):
    Alias: AliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAliasOutputTypeDef

```python
# DescribeAliasOutputTypeDef definition

class DescribeAliasOutputTypeDef(TypedDict):
    Alias: AliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAliasesOutputTypeDef

```python
# ListAliasesOutputTypeDef definition

class ListAliasesOutputTypeDef(TypedDict):
    Aliases: List[AliasTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAliasOutputTypeDef

```python
# UpdateAliasOutputTypeDef definition

class UpdateAliasOutputTypeDef(TypedDict):
    Alias: AliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PlayerTypeDef

```python
# PlayerTypeDef definition

class PlayerTypeDef(TypedDict):
    PlayerId: NotRequired[str],
    PlayerAttributes: NotRequired[Mapping[str, AttributeValueUnionTypeDef]],  # (1)
    Team: NotRequired[str],
    LatencyInMs: NotRequired[Mapping[str, int]],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 
## ComputeTypeDef

```python
# ComputeTypeDef definition

class ComputeTypeDef(TypedDict):
    FleetId: NotRequired[str],
    FleetArn: NotRequired[str],
    ComputeName: NotRequired[str],
    ComputeArn: NotRequired[str],
    IpAddress: NotRequired[str],
    DnsName: NotRequired[str],
    ComputeStatus: NotRequired[ComputeStatusType],  # (1)
    Location: NotRequired[str],
    CreationTime: NotRequired[datetime],
    OperatingSystem: NotRequired[OperatingSystemType],  # (2)
    Type: NotRequired[EC2InstanceTypeType],  # (3)
    GameLiftServiceSdkEndpoint: NotRequired[str],
    GameLiftAgentEndpoint: NotRequired[str],
    InstanceId: NotRequired[str],
    ContainerAttributes: NotRequired[ContainerAttributesTypeDef],  # (4)
```

1. See [:material-code-brackets: ComputeStatusType](./literals.md#computestatustype) 
2. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
3. See [:material-code-brackets: EC2InstanceTypeType](./literals.md#ec2instancetypetype) 
4. See [:material-code-braces: ContainerAttributesTypeDef](./type_defs.md#containerattributestypedef) 
## FleetAttributesTypeDef

```python
# FleetAttributesTypeDef definition

class FleetAttributesTypeDef(TypedDict):
    FleetId: NotRequired[str],
    FleetArn: NotRequired[str],
    FleetType: NotRequired[FleetTypeType],  # (1)
    InstanceType: NotRequired[EC2InstanceTypeType],  # (2)
    Description: NotRequired[str],
    Name: NotRequired[str],
    CreationTime: NotRequired[datetime],
    TerminationTime: NotRequired[datetime],
    Status: NotRequired[FleetStatusType],  # (3)
    BuildId: NotRequired[str],
    BuildArn: NotRequired[str],
    ScriptId: NotRequired[str],
    ScriptArn: NotRequired[str],
    ServerLaunchPath: NotRequired[str],
    ServerLaunchParameters: NotRequired[str],
    LogPaths: NotRequired[List[str]],
    NewGameSessionProtectionPolicy: NotRequired[ProtectionPolicyType],  # (4)
    OperatingSystem: NotRequired[OperatingSystemType],  # (5)
    ResourceCreationLimitPolicy: NotRequired[ResourceCreationLimitPolicyTypeDef],  # (6)
    MetricGroups: NotRequired[List[str]],
    StoppedActions: NotRequired[List[FleetActionType]],  # (7)
    InstanceRoleArn: NotRequired[str],
    CertificateConfiguration: NotRequired[CertificateConfigurationTypeDef],  # (8)
    ComputeType: NotRequired[ComputeTypeType],  # (9)
    AnywhereConfiguration: NotRequired[AnywhereConfigurationTypeDef],  # (10)
    InstanceRoleCredentialsProvider: NotRequired[InstanceRoleCredentialsProviderType],  # (11)
    ContainerGroupsAttributes: NotRequired[ContainerGroupsAttributesTypeDef],  # (12)
```

1. See [:material-code-brackets: FleetTypeType](./literals.md#fleettypetype) 
2. See [:material-code-brackets: EC2InstanceTypeType](./literals.md#ec2instancetypetype) 
3. See [:material-code-brackets: FleetStatusType](./literals.md#fleetstatustype) 
4. See [:material-code-brackets: ProtectionPolicyType](./literals.md#protectionpolicytype) 
5. See [:material-code-brackets: OperatingSystemType](./literals.md#operatingsystemtype) 
6. See [:material-code-braces: ResourceCreationLimitPolicyTypeDef](./type_defs.md#resourcecreationlimitpolicytypedef) 
7. See [:material-code-brackets: FleetActionType](./literals.md#fleetactiontype) 
8. See [:material-code-braces: CertificateConfigurationTypeDef](./type_defs.md#certificateconfigurationtypedef) 
9. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
10. See [:material-code-braces: AnywhereConfigurationTypeDef](./type_defs.md#anywhereconfigurationtypedef) 
11. See [:material-code-brackets: InstanceRoleCredentialsProviderType](./literals.md#instancerolecredentialsprovidertype) 
12. See [:material-code-braces: ContainerGroupsAttributesTypeDef](./type_defs.md#containergroupsattributestypedef) 
## ContainerDefinitionTypeDef

```python
# ContainerDefinitionTypeDef definition

class ContainerDefinitionTypeDef(TypedDict):
    ContainerName: str,
    ImageUri: str,
    ResolvedImageDigest: NotRequired[str],
    MemoryLimits: NotRequired[ContainerMemoryLimitsTypeDef],  # (1)
    PortConfiguration: NotRequired[ContainerPortConfigurationOutputTypeDef],  # (2)
    Cpu: NotRequired[int],
    HealthCheck: NotRequired[ContainerHealthCheckOutputTypeDef],  # (3)
    Command: NotRequired[List[str]],
    Essential: NotRequired[bool],
    EntryPoint: NotRequired[List[str]],
    WorkingDirectory: NotRequired[str],
    Environment: NotRequired[List[ContainerEnvironmentTypeDef]],  # (4)
    DependsOn: NotRequired[List[ContainerDependencyTypeDef]],  # (5)
```

1. See [:material-code-braces: ContainerMemoryLimitsTypeDef](./type_defs.md#containermemorylimitstypedef) 
2. See [:material-code-braces: ContainerPortConfigurationOutputTypeDef](./type_defs.md#containerportconfigurationoutputtypedef) 
3. See [:material-code-braces: ContainerHealthCheckOutputTypeDef](./type_defs.md#containerhealthcheckoutputtypedef) 
4. See [:material-code-braces: ContainerEnvironmentTypeDef](./type_defs.md#containerenvironmenttypedef) 
5. See [:material-code-braces: ContainerDependencyTypeDef](./type_defs.md#containerdependencytypedef) 
## CreateScriptOutputTypeDef

```python
# CreateScriptOutputTypeDef definition

class CreateScriptOutputTypeDef(TypedDict):
    Script: ScriptTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScriptTypeDef](./type_defs.md#scripttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScriptOutputTypeDef

```python
# DescribeScriptOutputTypeDef definition

class DescribeScriptOutputTypeDef(TypedDict):
    Script: ScriptTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScriptTypeDef](./type_defs.md#scripttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListScriptsOutputTypeDef

```python
# ListScriptsOutputTypeDef definition

class ListScriptsOutputTypeDef(TypedDict):
    Scripts: List[ScriptTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScriptTypeDef](./type_defs.md#scripttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateScriptOutputTypeDef

```python
# UpdateScriptOutputTypeDef definition

class UpdateScriptOutputTypeDef(TypedDict):
    Script: ScriptTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScriptTypeDef](./type_defs.md#scripttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetLocationAttributesOutputTypeDef

```python
# DescribeFleetLocationAttributesOutputTypeDef definition

class DescribeFleetLocationAttributesOutputTypeDef(TypedDict):
    FleetId: str,
    FleetArn: str,
    LocationAttributes: List[LocationAttributesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LocationAttributesTypeDef](./type_defs.md#locationattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGameServerGroupOutputTypeDef

```python
# CreateGameServerGroupOutputTypeDef definition

class CreateGameServerGroupOutputTypeDef(TypedDict):
    GameServerGroup: GameServerGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameServerGroupTypeDef](./type_defs.md#gameservergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGameServerGroupOutputTypeDef

```python
# DeleteGameServerGroupOutputTypeDef definition

class DeleteGameServerGroupOutputTypeDef(TypedDict):
    GameServerGroup: GameServerGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameServerGroupTypeDef](./type_defs.md#gameservergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGameServerGroupOutputTypeDef

```python
# DescribeGameServerGroupOutputTypeDef definition

class DescribeGameServerGroupOutputTypeDef(TypedDict):
    GameServerGroup: GameServerGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameServerGroupTypeDef](./type_defs.md#gameservergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGameServerGroupsOutputTypeDef

```python
# ListGameServerGroupsOutputTypeDef definition

class ListGameServerGroupsOutputTypeDef(TypedDict):
    GameServerGroups: List[GameServerGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GameServerGroupTypeDef](./type_defs.md#gameservergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResumeGameServerGroupOutputTypeDef

```python
# ResumeGameServerGroupOutputTypeDef definition

class ResumeGameServerGroupOutputTypeDef(TypedDict):
    GameServerGroup: GameServerGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameServerGroupTypeDef](./type_defs.md#gameservergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SuspendGameServerGroupOutputTypeDef

```python
# SuspendGameServerGroupOutputTypeDef definition

class SuspendGameServerGroupOutputTypeDef(TypedDict):
    GameServerGroup: GameServerGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameServerGroupTypeDef](./type_defs.md#gameservergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGameServerGroupOutputTypeDef

```python
# UpdateGameServerGroupOutputTypeDef definition

class UpdateGameServerGroupOutputTypeDef(TypedDict):
    GameServerGroup: GameServerGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameServerGroupTypeDef](./type_defs.md#gameservergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGameSessionOutputTypeDef

```python
# CreateGameSessionOutputTypeDef definition

class CreateGameSessionOutputTypeDef(TypedDict):
    GameSession: GameSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameSessionTypeDef](./type_defs.md#gamesessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGameSessionsOutputTypeDef

```python
# DescribeGameSessionsOutputTypeDef definition

class DescribeGameSessionsOutputTypeDef(TypedDict):
    GameSessions: List[GameSessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GameSessionTypeDef](./type_defs.md#gamesessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GameSessionDetailTypeDef

```python
# GameSessionDetailTypeDef definition

class GameSessionDetailTypeDef(TypedDict):
    GameSession: NotRequired[GameSessionTypeDef],  # (1)
    ProtectionPolicy: NotRequired[ProtectionPolicyType],  # (2)
```

1. See [:material-code-braces: GameSessionTypeDef](./type_defs.md#gamesessiontypedef) 
2. See [:material-code-brackets: ProtectionPolicyType](./literals.md#protectionpolicytype) 
## SearchGameSessionsOutputTypeDef

```python
# SearchGameSessionsOutputTypeDef definition

class SearchGameSessionsOutputTypeDef(TypedDict):
    GameSessions: List[GameSessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GameSessionTypeDef](./type_defs.md#gamesessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGameSessionOutputTypeDef

```python
# UpdateGameSessionOutputTypeDef definition

class UpdateGameSessionOutputTypeDef(TypedDict):
    GameSession: GameSessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameSessionTypeDef](./type_defs.md#gamesessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMatchmakingConfigurationOutputTypeDef

```python
# CreateMatchmakingConfigurationOutputTypeDef definition

class CreateMatchmakingConfigurationOutputTypeDef(TypedDict):
    Configuration: MatchmakingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MatchmakingConfigurationTypeDef](./type_defs.md#matchmakingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMatchmakingConfigurationsOutputTypeDef

```python
# DescribeMatchmakingConfigurationsOutputTypeDef definition

class DescribeMatchmakingConfigurationsOutputTypeDef(TypedDict):
    Configurations: List[MatchmakingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MatchmakingConfigurationTypeDef](./type_defs.md#matchmakingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMatchmakingConfigurationOutputTypeDef

```python
# UpdateMatchmakingConfigurationOutputTypeDef definition

class UpdateMatchmakingConfigurationOutputTypeDef(TypedDict):
    Configuration: MatchmakingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MatchmakingConfigurationTypeDef](./type_defs.md#matchmakingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetCapacityOutputTypeDef

```python
# DescribeFleetCapacityOutputTypeDef definition

class DescribeFleetCapacityOutputTypeDef(TypedDict):
    FleetCapacity: List[FleetCapacityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetCapacityTypeDef](./type_defs.md#fleetcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetLocationCapacityOutputTypeDef

```python
# DescribeFleetLocationCapacityOutputTypeDef definition

class DescribeFleetLocationCapacityOutputTypeDef(TypedDict):
    FleetCapacity: FleetCapacityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FleetCapacityTypeDef](./type_defs.md#fleetcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGameServerGroupInputRequestTypeDef

```python
# CreateGameServerGroupInputRequestTypeDef definition

class CreateGameServerGroupInputRequestTypeDef(TypedDict):
    GameServerGroupName: str,
    RoleArn: str,
    MinSize: int,
    MaxSize: int,
    LaunchTemplate: LaunchTemplateSpecificationTypeDef,  # (1)
    InstanceDefinitions: Sequence[InstanceDefinitionTypeDef],  # (2)
    AutoScalingPolicy: NotRequired[GameServerGroupAutoScalingPolicyTypeDef],  # (3)
    BalancingStrategy: NotRequired[BalancingStrategyType],  # (4)
    GameServerProtectionPolicy: NotRequired[GameServerProtectionPolicyType],  # (5)
    VpcSubnets: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (6)
```

1. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
2. See [:material-code-braces: InstanceDefinitionTypeDef](./type_defs.md#instancedefinitiontypedef) 
3. See [:material-code-braces: GameServerGroupAutoScalingPolicyTypeDef](./type_defs.md#gameservergroupautoscalingpolicytypedef) 
4. See [:material-code-brackets: BalancingStrategyType](./literals.md#balancingstrategytype) 
5. See [:material-code-brackets: GameServerProtectionPolicyType](./literals.md#gameserverprotectionpolicytype) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## MatchmakingTicketTypeDef

```python
# MatchmakingTicketTypeDef definition

class MatchmakingTicketTypeDef(TypedDict):
    TicketId: NotRequired[str],
    ConfigurationName: NotRequired[str],
    ConfigurationArn: NotRequired[str],
    Status: NotRequired[MatchmakingConfigurationStatusType],  # (1)
    StatusReason: NotRequired[str],
    StatusMessage: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Players: NotRequired[List[PlayerOutputTypeDef]],  # (2)
    GameSessionConnectionInfo: NotRequired[GameSessionConnectionInfoTypeDef],  # (3)
    EstimatedWaitTime: NotRequired[int],
```

1. See [:material-code-brackets: MatchmakingConfigurationStatusType](./literals.md#matchmakingconfigurationstatustype) 
2. See [:material-code-braces: PlayerOutputTypeDef](./type_defs.md#playeroutputtypedef) 
3. See [:material-code-braces: GameSessionConnectionInfoTypeDef](./type_defs.md#gamesessionconnectioninfotypedef) 
## DescribeGameSessionPlacementOutputTypeDef

```python
# DescribeGameSessionPlacementOutputTypeDef definition

class DescribeGameSessionPlacementOutputTypeDef(TypedDict):
    GameSessionPlacement: GameSessionPlacementTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameSessionPlacementTypeDef](./type_defs.md#gamesessionplacementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartGameSessionPlacementOutputTypeDef

```python
# StartGameSessionPlacementOutputTypeDef definition

class StartGameSessionPlacementOutputTypeDef(TypedDict):
    GameSessionPlacement: GameSessionPlacementTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameSessionPlacementTypeDef](./type_defs.md#gamesessionplacementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopGameSessionPlacementOutputTypeDef

```python
# StopGameSessionPlacementOutputTypeDef definition

class StopGameSessionPlacementOutputTypeDef(TypedDict):
    GameSessionPlacement: GameSessionPlacementTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameSessionPlacementTypeDef](./type_defs.md#gamesessionplacementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGameSessionQueueOutputTypeDef

```python
# CreateGameSessionQueueOutputTypeDef definition

class CreateGameSessionQueueOutputTypeDef(TypedDict):
    GameSessionQueue: GameSessionQueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameSessionQueueTypeDef](./type_defs.md#gamesessionqueuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGameSessionQueuesOutputTypeDef

```python
# DescribeGameSessionQueuesOutputTypeDef definition

class DescribeGameSessionQueuesOutputTypeDef(TypedDict):
    GameSessionQueues: List[GameSessionQueueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GameSessionQueueTypeDef](./type_defs.md#gamesessionqueuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGameSessionQueueOutputTypeDef

```python
# UpdateGameSessionQueueOutputTypeDef definition

class UpdateGameSessionQueueOutputTypeDef(TypedDict):
    GameSessionQueue: GameSessionQueueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameSessionQueueTypeDef](./type_defs.md#gamesessionqueuetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstanceAccessOutputTypeDef

```python
# GetInstanceAccessOutputTypeDef definition

class GetInstanceAccessOutputTypeDef(TypedDict):
    InstanceAccess: InstanceAccessTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceAccessTypeDef](./type_defs.md#instanceaccesstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScalingPoliciesOutputTypeDef

```python
# DescribeScalingPoliciesOutputTypeDef definition

class DescribeScalingPoliciesOutputTypeDef(TypedDict):
    ScalingPolicies: List[ScalingPolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScalingPolicyTypeDef](./type_defs.md#scalingpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRuntimeConfigurationOutputTypeDef

```python
# DescribeRuntimeConfigurationOutputTypeDef definition

class DescribeRuntimeConfigurationOutputTypeDef(TypedDict):
    RuntimeConfiguration: RuntimeConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuntimeConfigurationOutputTypeDef](./type_defs.md#runtimeconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRuntimeConfigurationOutputTypeDef

```python
# UpdateRuntimeConfigurationOutputTypeDef definition

class UpdateRuntimeConfigurationOutputTypeDef(TypedDict):
    RuntimeConfiguration: RuntimeConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuntimeConfigurationOutputTypeDef](./type_defs.md#runtimeconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetInputRequestTypeDef

```python
# CreateFleetInputRequestTypeDef definition

class CreateFleetInputRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    BuildId: NotRequired[str],
    ScriptId: NotRequired[str],
    ServerLaunchPath: NotRequired[str],
    ServerLaunchParameters: NotRequired[str],
    LogPaths: NotRequired[Sequence[str]],
    EC2InstanceType: NotRequired[EC2InstanceTypeType],  # (1)
    EC2InboundPermissions: NotRequired[Sequence[IpPermissionTypeDef]],  # (2)
    NewGameSessionProtectionPolicy: NotRequired[ProtectionPolicyType],  # (3)
    RuntimeConfiguration: NotRequired[RuntimeConfigurationTypeDef],  # (4)
    ResourceCreationLimitPolicy: NotRequired[ResourceCreationLimitPolicyTypeDef],  # (5)
    MetricGroups: NotRequired[Sequence[str]],
    PeerVpcAwsAccountId: NotRequired[str],
    PeerVpcId: NotRequired[str],
    FleetType: NotRequired[FleetTypeType],  # (6)
    InstanceRoleArn: NotRequired[str],
    CertificateConfiguration: NotRequired[CertificateConfigurationTypeDef],  # (7)
    Locations: NotRequired[Sequence[LocationConfigurationTypeDef]],  # (8)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (9)
    ComputeType: NotRequired[ComputeTypeType],  # (10)
    AnywhereConfiguration: NotRequired[AnywhereConfigurationTypeDef],  # (11)
    InstanceRoleCredentialsProvider: NotRequired[InstanceRoleCredentialsProviderType],  # (12)
    ContainerGroupsConfiguration: NotRequired[ContainerGroupsConfigurationTypeDef],  # (13)
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
13. See [:material-code-braces: ContainerGroupsConfigurationTypeDef](./type_defs.md#containergroupsconfigurationtypedef) 
## UpdateRuntimeConfigurationInputRequestTypeDef

```python
# UpdateRuntimeConfigurationInputRequestTypeDef definition

class UpdateRuntimeConfigurationInputRequestTypeDef(TypedDict):
    FleetId: str,
    RuntimeConfiguration: RuntimeConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: RuntimeConfigurationTypeDef](./type_defs.md#runtimeconfigurationtypedef) 
## DescribeVpcPeeringConnectionsOutputTypeDef

```python
# DescribeVpcPeeringConnectionsOutputTypeDef definition

class DescribeVpcPeeringConnectionsOutputTypeDef(TypedDict):
    VpcPeeringConnections: List[VpcPeeringConnectionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VpcPeeringConnectionTypeDef](./type_defs.md#vpcpeeringconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMatchmakingInputRequestTypeDef

```python
# StartMatchmakingInputRequestTypeDef definition

class StartMatchmakingInputRequestTypeDef(TypedDict):
    ConfigurationName: str,
    Players: Sequence[PlayerTypeDef],  # (1)
    TicketId: NotRequired[str],
```

1. See [:material-code-braces: PlayerTypeDef](./type_defs.md#playertypedef) 
## DescribeComputeOutputTypeDef

```python
# DescribeComputeOutputTypeDef definition

class DescribeComputeOutputTypeDef(TypedDict):
    Compute: ComputeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComputeTypeDef](./type_defs.md#computetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListComputeOutputTypeDef

```python
# ListComputeOutputTypeDef definition

class ListComputeOutputTypeDef(TypedDict):
    ComputeList: List[ComputeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ComputeTypeDef](./type_defs.md#computetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterComputeOutputTypeDef

```python
# RegisterComputeOutputTypeDef definition

class RegisterComputeOutputTypeDef(TypedDict):
    Compute: ComputeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComputeTypeDef](./type_defs.md#computetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetOutputTypeDef

```python
# CreateFleetOutputTypeDef definition

class CreateFleetOutputTypeDef(TypedDict):
    FleetAttributes: FleetAttributesTypeDef,  # (1)
    LocationStates: List[LocationStateTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FleetAttributesTypeDef](./type_defs.md#fleetattributestypedef) 
2. See [:material-code-braces: LocationStateTypeDef](./type_defs.md#locationstatetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetAttributesOutputTypeDef

```python
# DescribeFleetAttributesOutputTypeDef definition

class DescribeFleetAttributesOutputTypeDef(TypedDict):
    FleetAttributes: List[FleetAttributesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetAttributesTypeDef](./type_defs.md#fleetattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContainerGroupDefinitionTypeDef

```python
# ContainerGroupDefinitionTypeDef definition

class ContainerGroupDefinitionTypeDef(TypedDict):
    ContainerGroupDefinitionArn: NotRequired[str],
    CreationTime: NotRequired[datetime],
    OperatingSystem: NotRequired[ContainerOperatingSystemType],  # (1)
    Name: NotRequired[str],
    SchedulingStrategy: NotRequired[ContainerSchedulingStrategyType],  # (2)
    TotalMemoryLimit: NotRequired[int],
    TotalCpuLimit: NotRequired[int],
    ContainerDefinitions: NotRequired[List[ContainerDefinitionTypeDef]],  # (3)
    Status: NotRequired[ContainerGroupDefinitionStatusType],  # (4)
    StatusReason: NotRequired[str],
```

1. See [:material-code-brackets: ContainerOperatingSystemType](./literals.md#containeroperatingsystemtype) 
2. See [:material-code-brackets: ContainerSchedulingStrategyType](./literals.md#containerschedulingstrategytype) 
3. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) 
4. See [:material-code-brackets: ContainerGroupDefinitionStatusType](./literals.md#containergroupdefinitionstatustype) 
## ContainerDefinitionInputTypeDef

```python
# ContainerDefinitionInputTypeDef definition

class ContainerDefinitionInputTypeDef(TypedDict):
    ContainerName: str,
    ImageUri: str,
    MemoryLimits: NotRequired[ContainerMemoryLimitsTypeDef],  # (1)
    PortConfiguration: NotRequired[ContainerPortConfigurationUnionTypeDef],  # (2)
    Cpu: NotRequired[int],
    HealthCheck: NotRequired[ContainerHealthCheckUnionTypeDef],  # (3)
    Command: NotRequired[Sequence[str]],
    Essential: NotRequired[bool],
    EntryPoint: NotRequired[Sequence[str]],
    WorkingDirectory: NotRequired[str],
    Environment: NotRequired[Sequence[ContainerEnvironmentTypeDef]],  # (4)
    DependsOn: NotRequired[Sequence[ContainerDependencyTypeDef]],  # (5)
```

1. See [:material-code-braces: ContainerMemoryLimitsTypeDef](./type_defs.md#containermemorylimitstypedef) 
2. See [:material-code-braces: ContainerPortConfigurationTypeDef](./type_defs.md#containerportconfigurationtypedef) [:material-code-braces: ContainerPortConfigurationOutputTypeDef](./type_defs.md#containerportconfigurationoutputtypedef) 
3. See [:material-code-braces: ContainerHealthCheckTypeDef](./type_defs.md#containerhealthchecktypedef) [:material-code-braces: ContainerHealthCheckOutputTypeDef](./type_defs.md#containerhealthcheckoutputtypedef) 
4. See [:material-code-braces: ContainerEnvironmentTypeDef](./type_defs.md#containerenvironmenttypedef) 
5. See [:material-code-braces: ContainerDependencyTypeDef](./type_defs.md#containerdependencytypedef) 
## DescribeGameSessionDetailsOutputTypeDef

```python
# DescribeGameSessionDetailsOutputTypeDef definition

class DescribeGameSessionDetailsOutputTypeDef(TypedDict):
    GameSessionDetails: List[GameSessionDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GameSessionDetailTypeDef](./type_defs.md#gamesessiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMatchmakingOutputTypeDef

```python
# DescribeMatchmakingOutputTypeDef definition

class DescribeMatchmakingOutputTypeDef(TypedDict):
    TicketList: List[MatchmakingTicketTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MatchmakingTicketTypeDef](./type_defs.md#matchmakingtickettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMatchBackfillOutputTypeDef

```python
# StartMatchBackfillOutputTypeDef definition

class StartMatchBackfillOutputTypeDef(TypedDict):
    MatchmakingTicket: MatchmakingTicketTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MatchmakingTicketTypeDef](./type_defs.md#matchmakingtickettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMatchmakingOutputTypeDef

```python
# StartMatchmakingOutputTypeDef definition

class StartMatchmakingOutputTypeDef(TypedDict):
    MatchmakingTicket: MatchmakingTicketTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MatchmakingTicketTypeDef](./type_defs.md#matchmakingtickettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMatchBackfillInputRequestTypeDef

```python
# StartMatchBackfillInputRequestTypeDef definition

class StartMatchBackfillInputRequestTypeDef(TypedDict):
    ConfigurationName: str,
    Players: Sequence[PlayerUnionTypeDef],  # (1)
    TicketId: NotRequired[str],
    GameSessionArn: NotRequired[str],
```

1. See [:material-code-braces: PlayerTypeDef](./type_defs.md#playertypedef) [:material-code-braces: PlayerOutputTypeDef](./type_defs.md#playeroutputtypedef) 
## CreateContainerGroupDefinitionOutputTypeDef

```python
# CreateContainerGroupDefinitionOutputTypeDef definition

class CreateContainerGroupDefinitionOutputTypeDef(TypedDict):
    ContainerGroupDefinition: ContainerGroupDefinitionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerGroupDefinitionTypeDef](./type_defs.md#containergroupdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContainerGroupDefinitionOutputTypeDef

```python
# DescribeContainerGroupDefinitionOutputTypeDef definition

class DescribeContainerGroupDefinitionOutputTypeDef(TypedDict):
    ContainerGroupDefinition: ContainerGroupDefinitionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerGroupDefinitionTypeDef](./type_defs.md#containergroupdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContainerGroupDefinitionsOutputTypeDef

```python
# ListContainerGroupDefinitionsOutputTypeDef definition

class ListContainerGroupDefinitionsOutputTypeDef(TypedDict):
    ContainerGroupDefinitions: List[ContainerGroupDefinitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContainerGroupDefinitionTypeDef](./type_defs.md#containergroupdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContainerGroupDefinitionInputRequestTypeDef

```python
# CreateContainerGroupDefinitionInputRequestTypeDef definition

class CreateContainerGroupDefinitionInputRequestTypeDef(TypedDict):
    Name: str,
    TotalMemoryLimit: int,
    TotalCpuLimit: int,
    ContainerDefinitions: Sequence[ContainerDefinitionInputTypeDef],  # (1)
    OperatingSystem: ContainerOperatingSystemType,  # (2)
    SchedulingStrategy: NotRequired[ContainerSchedulingStrategyType],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: ContainerDefinitionInputTypeDef](./type_defs.md#containerdefinitioninputtypedef) 
2. See [:material-code-brackets: ContainerOperatingSystemType](./literals.md#containeroperatingsystemtype) 
3. See [:material-code-brackets: ContainerSchedulingStrategyType](./literals.md#containerschedulingstrategytype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
