# Literals

> [Index](../README.md) > [GameLift](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [GameLift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
    type annotations stubs module [types-aiobotocore-gamelift](https://pypi.org/project/types-aiobotocore-gamelift/).

## AcceptanceTypeType

```python
# AcceptanceTypeType usage example

from types_aiobotocore_gamelift.literals import AcceptanceTypeType

def get_value() -> AcceptanceTypeType:
    return "ACCEPT"
```

```python
# AcceptanceTypeType definition

AcceptanceTypeType = Literal[
    "ACCEPT",
    "REJECT",
]
```
## BackfillModeType

```python
# BackfillModeType usage example

from types_aiobotocore_gamelift.literals import BackfillModeType

def get_value() -> BackfillModeType:
    return "AUTOMATIC"
```

```python
# BackfillModeType definition

BackfillModeType = Literal[
    "AUTOMATIC",
    "MANUAL",
]
```
## BalancingStrategyType

```python
# BalancingStrategyType usage example

from types_aiobotocore_gamelift.literals import BalancingStrategyType

def get_value() -> BalancingStrategyType:
    return "ON_DEMAND_ONLY"
```

```python
# BalancingStrategyType definition

BalancingStrategyType = Literal[
    "ON_DEMAND_ONLY",
    "SPOT_ONLY",
    "SPOT_PREFERRED",
]
```
## BuildStatusType

```python
# BuildStatusType usage example

from types_aiobotocore_gamelift.literals import BuildStatusType

def get_value() -> BuildStatusType:
    return "FAILED"
```

```python
# BuildStatusType definition

BuildStatusType = Literal[
    "FAILED",
    "INITIALIZED",
    "READY",
]
```
## CertificateTypeType

```python
# CertificateTypeType usage example

from types_aiobotocore_gamelift.literals import CertificateTypeType

def get_value() -> CertificateTypeType:
    return "DISABLED"
```

```python
# CertificateTypeType definition

CertificateTypeType = Literal[
    "DISABLED",
    "GENERATED",
]
```
## ComparisonOperatorTypeType

```python
# ComparisonOperatorTypeType usage example

from types_aiobotocore_gamelift.literals import ComparisonOperatorTypeType

def get_value() -> ComparisonOperatorTypeType:
    return "GreaterThanOrEqualToThreshold"
```

```python
# ComparisonOperatorTypeType definition

ComparisonOperatorTypeType = Literal[
    "GreaterThanOrEqualToThreshold",
    "GreaterThanThreshold",
    "LessThanOrEqualToThreshold",
    "LessThanThreshold",
]
```
## ComputeStatusType

```python
# ComputeStatusType usage example

from types_aiobotocore_gamelift.literals import ComputeStatusType

def get_value() -> ComputeStatusType:
    return "ACTIVE"
```

```python
# ComputeStatusType definition

ComputeStatusType = Literal[
    "ACTIVE",
    "PENDING",
    "TERMINATING",
]
```
## ComputeTypeType

```python
# ComputeTypeType usage example

from types_aiobotocore_gamelift.literals import ComputeTypeType

def get_value() -> ComputeTypeType:
    return "ANYWHERE"
```

```python
# ComputeTypeType definition

ComputeTypeType = Literal[
    "ANYWHERE",
    "EC2",
]
```
## DescribeFleetAttributesPaginatorName

```python
# DescribeFleetAttributesPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeFleetAttributesPaginatorName

def get_value() -> DescribeFleetAttributesPaginatorName:
    return "describe_fleet_attributes"
```

```python
# DescribeFleetAttributesPaginatorName definition

DescribeFleetAttributesPaginatorName = Literal[
    "describe_fleet_attributes",
]
```
## DescribeFleetCapacityPaginatorName

```python
# DescribeFleetCapacityPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeFleetCapacityPaginatorName

def get_value() -> DescribeFleetCapacityPaginatorName:
    return "describe_fleet_capacity"
```

```python
# DescribeFleetCapacityPaginatorName definition

DescribeFleetCapacityPaginatorName = Literal[
    "describe_fleet_capacity",
]
```
## DescribeFleetEventsPaginatorName

```python
# DescribeFleetEventsPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeFleetEventsPaginatorName

def get_value() -> DescribeFleetEventsPaginatorName:
    return "describe_fleet_events"
```

```python
# DescribeFleetEventsPaginatorName definition

DescribeFleetEventsPaginatorName = Literal[
    "describe_fleet_events",
]
```
## DescribeFleetUtilizationPaginatorName

```python
# DescribeFleetUtilizationPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeFleetUtilizationPaginatorName

def get_value() -> DescribeFleetUtilizationPaginatorName:
    return "describe_fleet_utilization"
```

```python
# DescribeFleetUtilizationPaginatorName definition

DescribeFleetUtilizationPaginatorName = Literal[
    "describe_fleet_utilization",
]
```
## DescribeGameServerInstancesPaginatorName

```python
# DescribeGameServerInstancesPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeGameServerInstancesPaginatorName

def get_value() -> DescribeGameServerInstancesPaginatorName:
    return "describe_game_server_instances"
```

```python
# DescribeGameServerInstancesPaginatorName definition

DescribeGameServerInstancesPaginatorName = Literal[
    "describe_game_server_instances",
]
```
## DescribeGameSessionDetailsPaginatorName

```python
# DescribeGameSessionDetailsPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeGameSessionDetailsPaginatorName

def get_value() -> DescribeGameSessionDetailsPaginatorName:
    return "describe_game_session_details"
```

```python
# DescribeGameSessionDetailsPaginatorName definition

DescribeGameSessionDetailsPaginatorName = Literal[
    "describe_game_session_details",
]
```
## DescribeGameSessionQueuesPaginatorName

```python
# DescribeGameSessionQueuesPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeGameSessionQueuesPaginatorName

def get_value() -> DescribeGameSessionQueuesPaginatorName:
    return "describe_game_session_queues"
```

```python
# DescribeGameSessionQueuesPaginatorName definition

DescribeGameSessionQueuesPaginatorName = Literal[
    "describe_game_session_queues",
]
```
## DescribeGameSessionsPaginatorName

```python
# DescribeGameSessionsPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeGameSessionsPaginatorName

def get_value() -> DescribeGameSessionsPaginatorName:
    return "describe_game_sessions"
```

```python
# DescribeGameSessionsPaginatorName definition

DescribeGameSessionsPaginatorName = Literal[
    "describe_game_sessions",
]
```
## DescribeInstancesPaginatorName

```python
# DescribeInstancesPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeInstancesPaginatorName

def get_value() -> DescribeInstancesPaginatorName:
    return "describe_instances"
```

```python
# DescribeInstancesPaginatorName definition

DescribeInstancesPaginatorName = Literal[
    "describe_instances",
]
```
## DescribeMatchmakingConfigurationsPaginatorName

```python
# DescribeMatchmakingConfigurationsPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeMatchmakingConfigurationsPaginatorName

def get_value() -> DescribeMatchmakingConfigurationsPaginatorName:
    return "describe_matchmaking_configurations"
```

```python
# DescribeMatchmakingConfigurationsPaginatorName definition

DescribeMatchmakingConfigurationsPaginatorName = Literal[
    "describe_matchmaking_configurations",
]
```
## DescribeMatchmakingRuleSetsPaginatorName

```python
# DescribeMatchmakingRuleSetsPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeMatchmakingRuleSetsPaginatorName

def get_value() -> DescribeMatchmakingRuleSetsPaginatorName:
    return "describe_matchmaking_rule_sets"
```

```python
# DescribeMatchmakingRuleSetsPaginatorName definition

DescribeMatchmakingRuleSetsPaginatorName = Literal[
    "describe_matchmaking_rule_sets",
]
```
## DescribePlayerSessionsPaginatorName

```python
# DescribePlayerSessionsPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribePlayerSessionsPaginatorName

def get_value() -> DescribePlayerSessionsPaginatorName:
    return "describe_player_sessions"
```

```python
# DescribePlayerSessionsPaginatorName definition

DescribePlayerSessionsPaginatorName = Literal[
    "describe_player_sessions",
]
```
## DescribeScalingPoliciesPaginatorName

```python
# DescribeScalingPoliciesPaginatorName usage example

from types_aiobotocore_gamelift.literals import DescribeScalingPoliciesPaginatorName

def get_value() -> DescribeScalingPoliciesPaginatorName:
    return "describe_scaling_policies"
```

```python
# DescribeScalingPoliciesPaginatorName definition

DescribeScalingPoliciesPaginatorName = Literal[
    "describe_scaling_policies",
]
```
## EC2InstanceTypeType

```python
# EC2InstanceTypeType usage example

from types_aiobotocore_gamelift.literals import EC2InstanceTypeType

def get_value() -> EC2InstanceTypeType:
    return "c3.2xlarge"
```

```python
# EC2InstanceTypeType definition

EC2InstanceTypeType = Literal[
    "c3.2xlarge",
    "c3.4xlarge",
    "c3.8xlarge",
    "c3.large",
    "c3.xlarge",
    "c4.2xlarge",
    "c4.4xlarge",
    "c4.8xlarge",
    "c4.large",
    "c4.xlarge",
    "c5.12xlarge",
    "c5.18xlarge",
    "c5.24xlarge",
    "c5.2xlarge",
    "c5.4xlarge",
    "c5.9xlarge",
    "c5.large",
    "c5.xlarge",
    "c5a.12xlarge",
    "c5a.16xlarge",
    "c5a.24xlarge",
    "c5a.2xlarge",
    "c5a.4xlarge",
    "c5a.8xlarge",
    "c5a.large",
    "c5a.xlarge",
    "c5d.12xlarge",
    "c5d.18xlarge",
    "c5d.24xlarge",
    "c5d.2xlarge",
    "c5d.4xlarge",
    "c5d.9xlarge",
    "c5d.large",
    "c5d.xlarge",
    "c6a.12xlarge",
    "c6a.16xlarge",
    "c6a.24xlarge",
    "c6a.2xlarge",
    "c6a.4xlarge",
    "c6a.8xlarge",
    "c6a.large",
    "c6a.xlarge",
    "c6i.12xlarge",
    "c6i.16xlarge",
    "c6i.24xlarge",
    "c6i.2xlarge",
    "c6i.4xlarge",
    "c6i.8xlarge",
    "c6i.large",
    "c6i.xlarge",
    "m3.2xlarge",
    "m3.large",
    "m3.medium",
    "m3.xlarge",
    "m4.10xlarge",
    "m4.2xlarge",
    "m4.4xlarge",
    "m4.large",
    "m4.xlarge",
    "m5.12xlarge",
    "m5.16xlarge",
    "m5.24xlarge",
    "m5.2xlarge",
    "m5.4xlarge",
    "m5.8xlarge",
    "m5.large",
    "m5.xlarge",
    "m5a.12xlarge",
    "m5a.16xlarge",
    "m5a.24xlarge",
    "m5a.2xlarge",
    "m5a.4xlarge",
    "m5a.8xlarge",
    "m5a.large",
    "m5a.xlarge",
    "r3.2xlarge",
    "r3.4xlarge",
    "r3.8xlarge",
    "r3.large",
    "r3.xlarge",
    "r4.16xlarge",
    "r4.2xlarge",
    "r4.4xlarge",
    "r4.8xlarge",
    "r4.large",
    "r4.xlarge",
    "r5.12xlarge",
    "r5.16xlarge",
    "r5.24xlarge",
    "r5.2xlarge",
    "r5.4xlarge",
    "r5.8xlarge",
    "r5.large",
    "r5.xlarge",
    "r5a.12xlarge",
    "r5a.16xlarge",
    "r5a.24xlarge",
    "r5a.2xlarge",
    "r5a.4xlarge",
    "r5a.8xlarge",
    "r5a.large",
    "r5a.xlarge",
    "r5d.12xlarge",
    "r5d.16xlarge",
    "r5d.24xlarge",
    "r5d.2xlarge",
    "r5d.4xlarge",
    "r5d.8xlarge",
    "r5d.large",
    "r5d.xlarge",
    "t2.large",
    "t2.medium",
    "t2.micro",
    "t2.small",
]
```
## EventCodeType

```python
# EventCodeType usage example

from types_aiobotocore_gamelift.literals import EventCodeType

def get_value() -> EventCodeType:
    return "FLEET_ACTIVATION_FAILED"
```

```python
# EventCodeType definition

EventCodeType = Literal[
    "FLEET_ACTIVATION_FAILED",
    "FLEET_ACTIVATION_FAILED_NO_INSTANCES",
    "FLEET_BINARY_DOWNLOAD_FAILED",
    "FLEET_CREATED",
    "FLEET_CREATION_EXTRACTING_BUILD",
    "FLEET_CREATION_RUNNING_INSTALLER",
    "FLEET_CREATION_VALIDATING_RUNTIME_CONFIG",
    "FLEET_DELETED",
    "FLEET_INITIALIZATION_FAILED",
    "FLEET_NEW_GAME_SESSION_PROTECTION_POLICY_UPDATED",
    "FLEET_SCALING_EVENT",
    "FLEET_STATE_ACTIVATING",
    "FLEET_STATE_ACTIVE",
    "FLEET_STATE_BUILDING",
    "FLEET_STATE_DOWNLOADING",
    "FLEET_STATE_ERROR",
    "FLEET_STATE_VALIDATING",
    "FLEET_VALIDATION_EXECUTABLE_RUNTIME_FAILURE",
    "FLEET_VALIDATION_LAUNCH_PATH_NOT_FOUND",
    "FLEET_VALIDATION_TIMED_OUT",
    "FLEET_VPC_PEERING_DELETED",
    "FLEET_VPC_PEERING_FAILED",
    "FLEET_VPC_PEERING_SUCCEEDED",
    "GAME_SESSION_ACTIVATION_TIMEOUT",
    "GENERIC_EVENT",
    "INSTANCE_INTERRUPTED",
    "INSTANCE_RECYCLED",
    "SERVER_PROCESS_CRASHED",
    "SERVER_PROCESS_FORCE_TERMINATED",
    "SERVER_PROCESS_INVALID_PATH",
    "SERVER_PROCESS_PROCESS_EXIT_TIMEOUT",
    "SERVER_PROCESS_PROCESS_READY_TIMEOUT",
    "SERVER_PROCESS_SDK_INITIALIZATION_TIMEOUT",
    "SERVER_PROCESS_TERMINATED_UNHEALTHY",
]
```
## FilterInstanceStatusType

```python
# FilterInstanceStatusType usage example

from types_aiobotocore_gamelift.literals import FilterInstanceStatusType

def get_value() -> FilterInstanceStatusType:
    return "ACTIVE"
```

```python
# FilterInstanceStatusType definition

FilterInstanceStatusType = Literal[
    "ACTIVE",
    "DRAINING",
]
```
## FleetActionType

```python
# FleetActionType usage example

from types_aiobotocore_gamelift.literals import FleetActionType

def get_value() -> FleetActionType:
    return "AUTO_SCALING"
```

```python
# FleetActionType definition

FleetActionType = Literal[
    "AUTO_SCALING",
]
```
## FleetStatusType

```python
# FleetStatusType usage example

from types_aiobotocore_gamelift.literals import FleetStatusType

def get_value() -> FleetStatusType:
    return "ACTIVATING"
```

```python
# FleetStatusType definition

FleetStatusType = Literal[
    "ACTIVATING",
    "ACTIVE",
    "BUILDING",
    "DELETING",
    "DOWNLOADING",
    "ERROR",
    "NEW",
    "NOT_FOUND",
    "TERMINATED",
    "VALIDATING",
]
```
## FleetTypeType

```python
# FleetTypeType usage example

from types_aiobotocore_gamelift.literals import FleetTypeType

def get_value() -> FleetTypeType:
    return "ON_DEMAND"
```

```python
# FleetTypeType definition

FleetTypeType = Literal[
    "ON_DEMAND",
    "SPOT",
]
```
## FlexMatchModeType

```python
# FlexMatchModeType usage example

from types_aiobotocore_gamelift.literals import FlexMatchModeType

def get_value() -> FlexMatchModeType:
    return "STANDALONE"
```

```python
# FlexMatchModeType definition

FlexMatchModeType = Literal[
    "STANDALONE",
    "WITH_QUEUE",
]
```
## GameServerClaimStatusType

```python
# GameServerClaimStatusType usage example

from types_aiobotocore_gamelift.literals import GameServerClaimStatusType

def get_value() -> GameServerClaimStatusType:
    return "CLAIMED"
```

```python
# GameServerClaimStatusType definition

GameServerClaimStatusType = Literal[
    "CLAIMED",
]
```
## GameServerGroupActionType

```python
# GameServerGroupActionType usage example

from types_aiobotocore_gamelift.literals import GameServerGroupActionType

def get_value() -> GameServerGroupActionType:
    return "REPLACE_INSTANCE_TYPES"
```

```python
# GameServerGroupActionType definition

GameServerGroupActionType = Literal[
    "REPLACE_INSTANCE_TYPES",
]
```
## GameServerGroupDeleteOptionType

```python
# GameServerGroupDeleteOptionType usage example

from types_aiobotocore_gamelift.literals import GameServerGroupDeleteOptionType

def get_value() -> GameServerGroupDeleteOptionType:
    return "FORCE_DELETE"
```

```python
# GameServerGroupDeleteOptionType definition

GameServerGroupDeleteOptionType = Literal[
    "FORCE_DELETE",
    "RETAIN",
    "SAFE_DELETE",
]
```
## GameServerGroupInstanceTypeType

```python
# GameServerGroupInstanceTypeType usage example

from types_aiobotocore_gamelift.literals import GameServerGroupInstanceTypeType

def get_value() -> GameServerGroupInstanceTypeType:
    return "c4.2xlarge"
```

```python
# GameServerGroupInstanceTypeType definition

GameServerGroupInstanceTypeType = Literal[
    "c4.2xlarge",
    "c4.4xlarge",
    "c4.8xlarge",
    "c4.large",
    "c4.xlarge",
    "c5.12xlarge",
    "c5.18xlarge",
    "c5.24xlarge",
    "c5.2xlarge",
    "c5.4xlarge",
    "c5.9xlarge",
    "c5.large",
    "c5.xlarge",
    "c5a.12xlarge",
    "c5a.16xlarge",
    "c5a.24xlarge",
    "c5a.2xlarge",
    "c5a.4xlarge",
    "c5a.8xlarge",
    "c5a.large",
    "c5a.xlarge",
    "c6g.12xlarge",
    "c6g.16xlarge",
    "c6g.2xlarge",
    "c6g.4xlarge",
    "c6g.8xlarge",
    "c6g.large",
    "c6g.medium",
    "c6g.xlarge",
    "m4.10xlarge",
    "m4.2xlarge",
    "m4.4xlarge",
    "m4.large",
    "m4.xlarge",
    "m5.12xlarge",
    "m5.16xlarge",
    "m5.24xlarge",
    "m5.2xlarge",
    "m5.4xlarge",
    "m5.8xlarge",
    "m5.large",
    "m5.xlarge",
    "m5a.12xlarge",
    "m5a.16xlarge",
    "m5a.24xlarge",
    "m5a.2xlarge",
    "m5a.4xlarge",
    "m5a.8xlarge",
    "m5a.large",
    "m5a.xlarge",
    "m6g.12xlarge",
    "m6g.16xlarge",
    "m6g.2xlarge",
    "m6g.4xlarge",
    "m6g.8xlarge",
    "m6g.large",
    "m6g.medium",
    "m6g.xlarge",
    "r4.16xlarge",
    "r4.2xlarge",
    "r4.4xlarge",
    "r4.8xlarge",
    "r4.large",
    "r4.xlarge",
    "r5.12xlarge",
    "r5.16xlarge",
    "r5.24xlarge",
    "r5.2xlarge",
    "r5.4xlarge",
    "r5.8xlarge",
    "r5.large",
    "r5.xlarge",
    "r5a.12xlarge",
    "r5a.16xlarge",
    "r5a.24xlarge",
    "r5a.2xlarge",
    "r5a.4xlarge",
    "r5a.8xlarge",
    "r5a.large",
    "r5a.xlarge",
    "r6g.12xlarge",
    "r6g.16xlarge",
    "r6g.2xlarge",
    "r6g.4xlarge",
    "r6g.8xlarge",
    "r6g.large",
    "r6g.medium",
    "r6g.xlarge",
]
```
## GameServerGroupStatusType

```python
# GameServerGroupStatusType usage example

from types_aiobotocore_gamelift.literals import GameServerGroupStatusType

def get_value() -> GameServerGroupStatusType:
    return "ACTIVATING"
```

```python
# GameServerGroupStatusType definition

GameServerGroupStatusType = Literal[
    "ACTIVATING",
    "ACTIVE",
    "DELETE_SCHEDULED",
    "DELETED",
    "DELETING",
    "ERROR",
    "NEW",
]
```
## GameServerHealthCheckType

```python
# GameServerHealthCheckType usage example

from types_aiobotocore_gamelift.literals import GameServerHealthCheckType

def get_value() -> GameServerHealthCheckType:
    return "HEALTHY"
```

```python
# GameServerHealthCheckType definition

GameServerHealthCheckType = Literal[
    "HEALTHY",
]
```
## GameServerInstanceStatusType

```python
# GameServerInstanceStatusType usage example

from types_aiobotocore_gamelift.literals import GameServerInstanceStatusType

def get_value() -> GameServerInstanceStatusType:
    return "ACTIVE"
```

```python
# GameServerInstanceStatusType definition

GameServerInstanceStatusType = Literal[
    "ACTIVE",
    "DRAINING",
    "SPOT_TERMINATING",
]
```
## GameServerProtectionPolicyType

```python
# GameServerProtectionPolicyType usage example

from types_aiobotocore_gamelift.literals import GameServerProtectionPolicyType

def get_value() -> GameServerProtectionPolicyType:
    return "FULL_PROTECTION"
```

```python
# GameServerProtectionPolicyType definition

GameServerProtectionPolicyType = Literal[
    "FULL_PROTECTION",
    "NO_PROTECTION",
]
```
## GameServerUtilizationStatusType

```python
# GameServerUtilizationStatusType usage example

from types_aiobotocore_gamelift.literals import GameServerUtilizationStatusType

def get_value() -> GameServerUtilizationStatusType:
    return "AVAILABLE"
```

```python
# GameServerUtilizationStatusType definition

GameServerUtilizationStatusType = Literal[
    "AVAILABLE",
    "UTILIZED",
]
```
## GameSessionPlacementStateType

```python
# GameSessionPlacementStateType usage example

from types_aiobotocore_gamelift.literals import GameSessionPlacementStateType

def get_value() -> GameSessionPlacementStateType:
    return "CANCELLED"
```

```python
# GameSessionPlacementStateType definition

GameSessionPlacementStateType = Literal[
    "CANCELLED",
    "FAILED",
    "FULFILLED",
    "PENDING",
    "TIMED_OUT",
]
```
## GameSessionStatusReasonType

```python
# GameSessionStatusReasonType usage example

from types_aiobotocore_gamelift.literals import GameSessionStatusReasonType

def get_value() -> GameSessionStatusReasonType:
    return "INTERRUPTED"
```

```python
# GameSessionStatusReasonType definition

GameSessionStatusReasonType = Literal[
    "INTERRUPTED",
]
```
## GameSessionStatusType

```python
# GameSessionStatusType usage example

from types_aiobotocore_gamelift.literals import GameSessionStatusType

def get_value() -> GameSessionStatusType:
    return "ACTIVATING"
```

```python
# GameSessionStatusType definition

GameSessionStatusType = Literal[
    "ACTIVATING",
    "ACTIVE",
    "ERROR",
    "TERMINATED",
    "TERMINATING",
]
```
## InstanceStatusType

```python
# InstanceStatusType usage example

from types_aiobotocore_gamelift.literals import InstanceStatusType

def get_value() -> InstanceStatusType:
    return "ACTIVE"
```

```python
# InstanceStatusType definition

InstanceStatusType = Literal[
    "ACTIVE",
    "PENDING",
    "TERMINATING",
]
```
## IpProtocolType

```python
# IpProtocolType usage example

from types_aiobotocore_gamelift.literals import IpProtocolType

def get_value() -> IpProtocolType:
    return "TCP"
```

```python
# IpProtocolType definition

IpProtocolType = Literal[
    "TCP",
    "UDP",
]
```
## ListAliasesPaginatorName

```python
# ListAliasesPaginatorName usage example

from types_aiobotocore_gamelift.literals import ListAliasesPaginatorName

def get_value() -> ListAliasesPaginatorName:
    return "list_aliases"
```

```python
# ListAliasesPaginatorName definition

ListAliasesPaginatorName = Literal[
    "list_aliases",
]
```
## ListBuildsPaginatorName

```python
# ListBuildsPaginatorName usage example

from types_aiobotocore_gamelift.literals import ListBuildsPaginatorName

def get_value() -> ListBuildsPaginatorName:
    return "list_builds"
```

```python
# ListBuildsPaginatorName definition

ListBuildsPaginatorName = Literal[
    "list_builds",
]
```
## ListComputePaginatorName

```python
# ListComputePaginatorName usage example

from types_aiobotocore_gamelift.literals import ListComputePaginatorName

def get_value() -> ListComputePaginatorName:
    return "list_compute"
```

```python
# ListComputePaginatorName definition

ListComputePaginatorName = Literal[
    "list_compute",
]
```
## ListFleetsPaginatorName

```python
# ListFleetsPaginatorName usage example

from types_aiobotocore_gamelift.literals import ListFleetsPaginatorName

def get_value() -> ListFleetsPaginatorName:
    return "list_fleets"
```

```python
# ListFleetsPaginatorName definition

ListFleetsPaginatorName = Literal[
    "list_fleets",
]
```
## ListGameServerGroupsPaginatorName

```python
# ListGameServerGroupsPaginatorName usage example

from types_aiobotocore_gamelift.literals import ListGameServerGroupsPaginatorName

def get_value() -> ListGameServerGroupsPaginatorName:
    return "list_game_server_groups"
```

```python
# ListGameServerGroupsPaginatorName definition

ListGameServerGroupsPaginatorName = Literal[
    "list_game_server_groups",
]
```
## ListGameServersPaginatorName

```python
# ListGameServersPaginatorName usage example

from types_aiobotocore_gamelift.literals import ListGameServersPaginatorName

def get_value() -> ListGameServersPaginatorName:
    return "list_game_servers"
```

```python
# ListGameServersPaginatorName definition

ListGameServersPaginatorName = Literal[
    "list_game_servers",
]
```
## ListLocationsPaginatorName

```python
# ListLocationsPaginatorName usage example

from types_aiobotocore_gamelift.literals import ListLocationsPaginatorName

def get_value() -> ListLocationsPaginatorName:
    return "list_locations"
```

```python
# ListLocationsPaginatorName definition

ListLocationsPaginatorName = Literal[
    "list_locations",
]
```
## ListScriptsPaginatorName

```python
# ListScriptsPaginatorName usage example

from types_aiobotocore_gamelift.literals import ListScriptsPaginatorName

def get_value() -> ListScriptsPaginatorName:
    return "list_scripts"
```

```python
# ListScriptsPaginatorName definition

ListScriptsPaginatorName = Literal[
    "list_scripts",
]
```
## LocationFilterType

```python
# LocationFilterType usage example

from types_aiobotocore_gamelift.literals import LocationFilterType

def get_value() -> LocationFilterType:
    return "AWS"
```

```python
# LocationFilterType definition

LocationFilterType = Literal[
    "AWS",
    "CUSTOM",
]
```
## LocationUpdateStatusType

```python
# LocationUpdateStatusType usage example

from types_aiobotocore_gamelift.literals import LocationUpdateStatusType

def get_value() -> LocationUpdateStatusType:
    return "PENDING_UPDATE"
```

```python
# LocationUpdateStatusType definition

LocationUpdateStatusType = Literal[
    "PENDING_UPDATE",
]
```
## MatchmakingConfigurationStatusType

```python
# MatchmakingConfigurationStatusType usage example

from types_aiobotocore_gamelift.literals import MatchmakingConfigurationStatusType

def get_value() -> MatchmakingConfigurationStatusType:
    return "CANCELLED"
```

```python
# MatchmakingConfigurationStatusType definition

MatchmakingConfigurationStatusType = Literal[
    "CANCELLED",
    "COMPLETED",
    "FAILED",
    "PLACING",
    "QUEUED",
    "REQUIRES_ACCEPTANCE",
    "SEARCHING",
    "TIMED_OUT",
]
```
## MetricNameType

```python
# MetricNameType usage example

from types_aiobotocore_gamelift.literals import MetricNameType

def get_value() -> MetricNameType:
    return "ActivatingGameSessions"
```

```python
# MetricNameType definition

MetricNameType = Literal[
    "ActivatingGameSessions",
    "ActiveGameSessions",
    "ActiveInstances",
    "AvailableGameSessions",
    "AvailablePlayerSessions",
    "ConcurrentActivatableGameSessions",
    "CurrentPlayerSessions",
    "IdleInstances",
    "PercentAvailableGameSessions",
    "PercentIdleInstances",
    "QueueDepth",
    "WaitTime",
]
```
## OperatingSystemType

```python
# OperatingSystemType usage example

from types_aiobotocore_gamelift.literals import OperatingSystemType

def get_value() -> OperatingSystemType:
    return "AMAZON_LINUX"
```

```python
# OperatingSystemType definition

OperatingSystemType = Literal[
    "AMAZON_LINUX",
    "AMAZON_LINUX_2",
    "AMAZON_LINUX_2023",
    "WINDOWS_2012",
    "WINDOWS_2016",
]
```
## PlayerSessionCreationPolicyType

```python
# PlayerSessionCreationPolicyType usage example

from types_aiobotocore_gamelift.literals import PlayerSessionCreationPolicyType

def get_value() -> PlayerSessionCreationPolicyType:
    return "ACCEPT_ALL"
```

```python
# PlayerSessionCreationPolicyType definition

PlayerSessionCreationPolicyType = Literal[
    "ACCEPT_ALL",
    "DENY_ALL",
]
```
## PlayerSessionStatusType

```python
# PlayerSessionStatusType usage example

from types_aiobotocore_gamelift.literals import PlayerSessionStatusType

def get_value() -> PlayerSessionStatusType:
    return "ACTIVE"
```

```python
# PlayerSessionStatusType definition

PlayerSessionStatusType = Literal[
    "ACTIVE",
    "COMPLETED",
    "RESERVED",
    "TIMEDOUT",
]
```
## PolicyTypeType

```python
# PolicyTypeType usage example

from types_aiobotocore_gamelift.literals import PolicyTypeType

def get_value() -> PolicyTypeType:
    return "RuleBased"
```

```python
# PolicyTypeType definition

PolicyTypeType = Literal[
    "RuleBased",
    "TargetBased",
]
```
## PriorityTypeType

```python
# PriorityTypeType usage example

from types_aiobotocore_gamelift.literals import PriorityTypeType

def get_value() -> PriorityTypeType:
    return "COST"
```

```python
# PriorityTypeType definition

PriorityTypeType = Literal[
    "COST",
    "DESTINATION",
    "LATENCY",
    "LOCATION",
]
```
## ProtectionPolicyType

```python
# ProtectionPolicyType usage example

from types_aiobotocore_gamelift.literals import ProtectionPolicyType

def get_value() -> ProtectionPolicyType:
    return "FullProtection"
```

```python
# ProtectionPolicyType definition

ProtectionPolicyType = Literal[
    "FullProtection",
    "NoProtection",
]
```
## RoutingStrategyTypeType

```python
# RoutingStrategyTypeType usage example

from types_aiobotocore_gamelift.literals import RoutingStrategyTypeType

def get_value() -> RoutingStrategyTypeType:
    return "SIMPLE"
```

```python
# RoutingStrategyTypeType definition

RoutingStrategyTypeType = Literal[
    "SIMPLE",
    "TERMINAL",
]
```
## ScalingAdjustmentTypeType

```python
# ScalingAdjustmentTypeType usage example

from types_aiobotocore_gamelift.literals import ScalingAdjustmentTypeType

def get_value() -> ScalingAdjustmentTypeType:
    return "ChangeInCapacity"
```

```python
# ScalingAdjustmentTypeType definition

ScalingAdjustmentTypeType = Literal[
    "ChangeInCapacity",
    "ExactCapacity",
    "PercentChangeInCapacity",
]
```
## ScalingStatusTypeType

```python
# ScalingStatusTypeType usage example

from types_aiobotocore_gamelift.literals import ScalingStatusTypeType

def get_value() -> ScalingStatusTypeType:
    return "ACTIVE"
```

```python
# ScalingStatusTypeType definition

ScalingStatusTypeType = Literal[
    "ACTIVE",
    "DELETE_REQUESTED",
    "DELETED",
    "DELETING",
    "ERROR",
    "UPDATE_REQUESTED",
    "UPDATING",
]
```
## SearchGameSessionsPaginatorName

```python
# SearchGameSessionsPaginatorName usage example

from types_aiobotocore_gamelift.literals import SearchGameSessionsPaginatorName

def get_value() -> SearchGameSessionsPaginatorName:
    return "search_game_sessions"
```

```python
# SearchGameSessionsPaginatorName definition

SearchGameSessionsPaginatorName = Literal[
    "search_game_sessions",
]
```
## SortOrderType

```python
# SortOrderType usage example

from types_aiobotocore_gamelift.literals import SortOrderType

def get_value() -> SortOrderType:
    return "ASCENDING"
```

```python
# SortOrderType definition

SortOrderType = Literal[
    "ASCENDING",
    "DESCENDING",
]
```
## GameLiftServiceName

```python
# GameLiftServiceName usage example

from types_aiobotocore_gamelift.literals import GameLiftServiceName

def get_value() -> GameLiftServiceName:
    return "gamelift"
```

```python
# GameLiftServiceName definition

GameLiftServiceName = Literal[
    "gamelift",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_gamelift.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition

ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "alexaforbusiness",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-zonal-shift",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcases",
    "connectparticipant",
    "controltower",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "fsx",
    "gamelift",
    "gamesparks",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
    "internetmonitor",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-roborunner",
    "iot1click-devices",
    "iot1click-projects",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "m2",
    "machinelearning",
    "macie",
    "macie2",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-catalog",
    "marketplace-entitlement",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
    "oam",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "payment-cryptography",
    "payment-cryptography-data",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "privatenetworks",
    "proton",
    "qldb",
    "qldb-session",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_gamelift.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition

ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example

from types_aiobotocore_gamelift.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_fleet_attributes"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_fleet_attributes",
    "describe_fleet_capacity",
    "describe_fleet_events",
    "describe_fleet_utilization",
    "describe_game_server_instances",
    "describe_game_session_details",
    "describe_game_session_queues",
    "describe_game_sessions",
    "describe_instances",
    "describe_matchmaking_configurations",
    "describe_matchmaking_rule_sets",
    "describe_player_sessions",
    "describe_scaling_policies",
    "list_aliases",
    "list_builds",
    "list_compute",
    "list_fleets",
    "list_game_server_groups",
    "list_game_servers",
    "list_locations",
    "list_scripts",
    "search_game_sessions",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_gamelift.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition

RegionName = Literal[
    "af-south-1",
    "ap-east-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-northeast-3",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-south-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
