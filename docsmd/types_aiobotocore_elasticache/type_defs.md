# Type definitions

> [Index](../README.md) > [ElastiCache](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ElastiCache](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#elasticache)
    type annotations stubs module [types-aiobotocore-elasticache](https://pypi.org/project/types-aiobotocore-elasticache/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## NodeGroupConfigurationUnionTypeDef

```python
# NodeGroupConfigurationUnionTypeDef definition

NodeGroupConfigurationUnionTypeDef = Union[
    NodeGroupConfigurationTypeDef,  # (1)
    NodeGroupConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NodeGroupConfigurationTypeDef](./type_defs.md#nodegroupconfigurationtypedef) 
2. See [:material-code-braces: NodeGroupConfigurationOutputTypeDef](./type_defs.md#nodegroupconfigurationoutputtypedef) 



## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

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

## AuthenticationModeTypeDef

```python
# AuthenticationModeTypeDef definition

class AuthenticationModeTypeDef(TypedDict):
    Type: NotRequired[InputAuthenticationTypeType],  # (1)
    Passwords: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: InputAuthenticationTypeType](./literals.md#inputauthenticationtypetype) 
## AuthenticationTypeDef

```python
# AuthenticationTypeDef definition

class AuthenticationTypeDef(TypedDict):
    Type: NotRequired[AuthenticationTypeType],  # (1)
    PasswordCount: NotRequired[int],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
## AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef

```python
# AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef definition

class AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef(TypedDict):
    CacheSecurityGroupName: str,
    EC2SecurityGroupName: str,
    EC2SecurityGroupOwnerId: str,
```

## AvailabilityZoneTypeDef

```python
# AvailabilityZoneTypeDef definition

class AvailabilityZoneTypeDef(TypedDict):
    Name: NotRequired[str],
```

## BatchApplyUpdateActionMessageRequestTypeDef

```python
# BatchApplyUpdateActionMessageRequestTypeDef definition

class BatchApplyUpdateActionMessageRequestTypeDef(TypedDict):
    ServiceUpdateName: str,
    ReplicationGroupIds: NotRequired[Sequence[str]],
    CacheClusterIds: NotRequired[Sequence[str]],
```

## BatchStopUpdateActionMessageRequestTypeDef

```python
# BatchStopUpdateActionMessageRequestTypeDef definition

class BatchStopUpdateActionMessageRequestTypeDef(TypedDict):
    ServiceUpdateName: str,
    ReplicationGroupIds: NotRequired[Sequence[str]],
    CacheClusterIds: NotRequired[Sequence[str]],
```

## CacheParameterGroupStatusTypeDef

```python
# CacheParameterGroupStatusTypeDef definition

class CacheParameterGroupStatusTypeDef(TypedDict):
    CacheParameterGroupName: NotRequired[str],
    ParameterApplyStatus: NotRequired[str],
    CacheNodeIdsToReboot: NotRequired[List[str]],
```

## CacheSecurityGroupMembershipTypeDef

```python
# CacheSecurityGroupMembershipTypeDef definition

class CacheSecurityGroupMembershipTypeDef(TypedDict):
    CacheSecurityGroupName: NotRequired[str],
    Status: NotRequired[str],
```

## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Address: NotRequired[str],
    Port: NotRequired[int],
```

## NotificationConfigurationTypeDef

```python
# NotificationConfigurationTypeDef definition

class NotificationConfigurationTypeDef(TypedDict):
    TopicArn: NotRequired[str],
    TopicStatus: NotRequired[str],
```

## SecurityGroupMembershipTypeDef

```python
# SecurityGroupMembershipTypeDef definition

class SecurityGroupMembershipTypeDef(TypedDict):
    SecurityGroupId: NotRequired[str],
    Status: NotRequired[str],
```

## CacheEngineVersionTypeDef

```python
# CacheEngineVersionTypeDef definition

class CacheEngineVersionTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    CacheParameterGroupFamily: NotRequired[str],
    CacheEngineDescription: NotRequired[str],
    CacheEngineVersionDescription: NotRequired[str],
```

## CacheNodeTypeSpecificValueTypeDef

```python
# CacheNodeTypeSpecificValueTypeDef definition

class CacheNodeTypeSpecificValueTypeDef(TypedDict):
    CacheNodeType: NotRequired[str],
    Value: NotRequired[str],
```

## CacheNodeUpdateStatusTypeDef

```python
# CacheNodeUpdateStatusTypeDef definition

class CacheNodeUpdateStatusTypeDef(TypedDict):
    CacheNodeId: NotRequired[str],
    NodeUpdateStatus: NotRequired[NodeUpdateStatusType],  # (1)
    NodeDeletionDate: NotRequired[datetime],
    NodeUpdateStartDate: NotRequired[datetime],
    NodeUpdateEndDate: NotRequired[datetime],
    NodeUpdateInitiatedBy: NotRequired[NodeUpdateInitiatedByType],  # (2)
    NodeUpdateInitiatedDate: NotRequired[datetime],
    NodeUpdateStatusModifiedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: NodeUpdateStatusType](./literals.md#nodeupdatestatustype) 
2. See [:material-code-brackets: NodeUpdateInitiatedByType](./literals.md#nodeupdateinitiatedbytype) 
## ParameterTypeDef

```python
# ParameterTypeDef definition

class ParameterTypeDef(TypedDict):
    ParameterName: NotRequired[str],
    ParameterValue: NotRequired[str],
    Description: NotRequired[str],
    Source: NotRequired[str],
    DataType: NotRequired[str],
    AllowedValues: NotRequired[str],
    IsModifiable: NotRequired[bool],
    MinimumEngineVersion: NotRequired[str],
    ChangeType: NotRequired[ChangeTypeType],  # (1)
```

1. See [:material-code-brackets: ChangeTypeType](./literals.md#changetypetype) 
## CacheParameterGroupTypeDef

```python
# CacheParameterGroupTypeDef definition

class CacheParameterGroupTypeDef(TypedDict):
    CacheParameterGroupName: NotRequired[str],
    CacheParameterGroupFamily: NotRequired[str],
    Description: NotRequired[str],
    IsGlobal: NotRequired[bool],
    ARN: NotRequired[str],
```

## EC2SecurityGroupTypeDef

```python
# EC2SecurityGroupTypeDef definition

class EC2SecurityGroupTypeDef(TypedDict):
    Status: NotRequired[str],
    EC2SecurityGroupName: NotRequired[str],
    EC2SecurityGroupOwnerId: NotRequired[str],
```

## DataStorageTypeDef

```python
# DataStorageTypeDef definition

class DataStorageTypeDef(TypedDict):
    Unit: DataStorageUnitType,  # (1)
    Maximum: NotRequired[int],
    Minimum: NotRequired[int],
```

1. See [:material-code-brackets: DataStorageUnitType](./literals.md#datastorageunittype) 
## ECPUPerSecondTypeDef

```python
# ECPUPerSecondTypeDef definition

class ECPUPerSecondTypeDef(TypedDict):
    Maximum: NotRequired[int],
    Minimum: NotRequired[int],
```

## CloudWatchLogsDestinationDetailsTypeDef

```python
# CloudWatchLogsDestinationDetailsTypeDef definition

class CloudWatchLogsDestinationDetailsTypeDef(TypedDict):
    LogGroup: NotRequired[str],
```

## CompleteMigrationMessageRequestTypeDef

```python
# CompleteMigrationMessageRequestTypeDef definition

class CompleteMigrationMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: str,
    Force: NotRequired[bool],
```

## ConfigureShardTypeDef

```python
# ConfigureShardTypeDef definition

class ConfigureShardTypeDef(TypedDict):
    NodeGroupId: str,
    NewReplicaCount: int,
    PreferredAvailabilityZones: NotRequired[Sequence[str]],
    PreferredOutpostArns: NotRequired[Sequence[str]],
```

## CreateGlobalReplicationGroupMessageRequestTypeDef

```python
# CreateGlobalReplicationGroupMessageRequestTypeDef definition

class CreateGlobalReplicationGroupMessageRequestTypeDef(TypedDict):
    GlobalReplicationGroupIdSuffix: str,
    PrimaryReplicationGroupId: str,
    GlobalReplicationGroupDescription: NotRequired[str],
```

## CustomerNodeEndpointTypeDef

```python
# CustomerNodeEndpointTypeDef definition

class CustomerNodeEndpointTypeDef(TypedDict):
    Address: NotRequired[str],
    Port: NotRequired[int],
```

## DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef

```python
# DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef definition

class DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(TypedDict):
    GlobalReplicationGroupId: str,
    NodeGroupCount: int,
    ApplyImmediately: bool,
    GlobalNodeGroupsToRemove: NotRequired[Sequence[str]],
    GlobalNodeGroupsToRetain: NotRequired[Sequence[str]],
```

## DeleteCacheClusterMessageRequestTypeDef

```python
# DeleteCacheClusterMessageRequestTypeDef definition

class DeleteCacheClusterMessageRequestTypeDef(TypedDict):
    CacheClusterId: str,
    FinalSnapshotIdentifier: NotRequired[str],
```

## DeleteCacheParameterGroupMessageRequestTypeDef

```python
# DeleteCacheParameterGroupMessageRequestTypeDef definition

class DeleteCacheParameterGroupMessageRequestTypeDef(TypedDict):
    CacheParameterGroupName: str,
```

## DeleteCacheSecurityGroupMessageRequestTypeDef

```python
# DeleteCacheSecurityGroupMessageRequestTypeDef definition

class DeleteCacheSecurityGroupMessageRequestTypeDef(TypedDict):
    CacheSecurityGroupName: str,
```

## DeleteCacheSubnetGroupMessageRequestTypeDef

```python
# DeleteCacheSubnetGroupMessageRequestTypeDef definition

class DeleteCacheSubnetGroupMessageRequestTypeDef(TypedDict):
    CacheSubnetGroupName: str,
```

## DeleteGlobalReplicationGroupMessageRequestTypeDef

```python
# DeleteGlobalReplicationGroupMessageRequestTypeDef definition

class DeleteGlobalReplicationGroupMessageRequestTypeDef(TypedDict):
    GlobalReplicationGroupId: str,
    RetainPrimaryReplicationGroup: bool,
```

## DeleteReplicationGroupMessageRequestTypeDef

```python
# DeleteReplicationGroupMessageRequestTypeDef definition

class DeleteReplicationGroupMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: str,
    RetainPrimaryCluster: NotRequired[bool],
    FinalSnapshotIdentifier: NotRequired[str],
```

## DeleteServerlessCacheRequestRequestTypeDef

```python
# DeleteServerlessCacheRequestRequestTypeDef definition

class DeleteServerlessCacheRequestRequestTypeDef(TypedDict):
    ServerlessCacheName: str,
    FinalSnapshotName: NotRequired[str],
```

## DeleteServerlessCacheSnapshotRequestRequestTypeDef

```python
# DeleteServerlessCacheSnapshotRequestRequestTypeDef definition

class DeleteServerlessCacheSnapshotRequestRequestTypeDef(TypedDict):
    ServerlessCacheSnapshotName: str,
```

## DeleteSnapshotMessageRequestTypeDef

```python
# DeleteSnapshotMessageRequestTypeDef definition

class DeleteSnapshotMessageRequestTypeDef(TypedDict):
    SnapshotName: str,
```

## DeleteUserGroupMessageRequestTypeDef

```python
# DeleteUserGroupMessageRequestTypeDef definition

class DeleteUserGroupMessageRequestTypeDef(TypedDict):
    UserGroupId: str,
```

## DeleteUserMessageRequestTypeDef

```python
# DeleteUserMessageRequestTypeDef definition

class DeleteUserMessageRequestTypeDef(TypedDict):
    UserId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeCacheClustersMessageRequestTypeDef

```python
# DescribeCacheClustersMessageRequestTypeDef definition

class DescribeCacheClustersMessageRequestTypeDef(TypedDict):
    CacheClusterId: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    ShowCacheNodeInfo: NotRequired[bool],
    ShowCacheClustersNotInReplicationGroups: NotRequired[bool],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeCacheEngineVersionsMessageRequestTypeDef

```python
# DescribeCacheEngineVersionsMessageRequestTypeDef definition

class DescribeCacheEngineVersionsMessageRequestTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    CacheParameterGroupFamily: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    DefaultOnly: NotRequired[bool],
```

## DescribeCacheParameterGroupsMessageRequestTypeDef

```python
# DescribeCacheParameterGroupsMessageRequestTypeDef definition

class DescribeCacheParameterGroupsMessageRequestTypeDef(TypedDict):
    CacheParameterGroupName: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeCacheParametersMessageRequestTypeDef

```python
# DescribeCacheParametersMessageRequestTypeDef definition

class DescribeCacheParametersMessageRequestTypeDef(TypedDict):
    CacheParameterGroupName: str,
    Source: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeCacheSecurityGroupsMessageRequestTypeDef

```python
# DescribeCacheSecurityGroupsMessageRequestTypeDef definition

class DescribeCacheSecurityGroupsMessageRequestTypeDef(TypedDict):
    CacheSecurityGroupName: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeCacheSubnetGroupsMessageRequestTypeDef

```python
# DescribeCacheSubnetGroupsMessageRequestTypeDef definition

class DescribeCacheSubnetGroupsMessageRequestTypeDef(TypedDict):
    CacheSubnetGroupName: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeEngineDefaultParametersMessageRequestTypeDef

```python
# DescribeEngineDefaultParametersMessageRequestTypeDef definition

class DescribeEngineDefaultParametersMessageRequestTypeDef(TypedDict):
    CacheParameterGroupFamily: str,
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeGlobalReplicationGroupsMessageRequestTypeDef

```python
# DescribeGlobalReplicationGroupsMessageRequestTypeDef definition

class DescribeGlobalReplicationGroupsMessageRequestTypeDef(TypedDict):
    GlobalReplicationGroupId: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    ShowMemberInfo: NotRequired[bool],
```

## DescribeReplicationGroupsMessageRequestTypeDef

```python
# DescribeReplicationGroupsMessageRequestTypeDef definition

class DescribeReplicationGroupsMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeReservedCacheNodesMessageRequestTypeDef

```python
# DescribeReservedCacheNodesMessageRequestTypeDef definition

class DescribeReservedCacheNodesMessageRequestTypeDef(TypedDict):
    ReservedCacheNodeId: NotRequired[str],
    ReservedCacheNodesOfferingId: NotRequired[str],
    CacheNodeType: NotRequired[str],
    Duration: NotRequired[str],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeReservedCacheNodesOfferingsMessageRequestTypeDef

```python
# DescribeReservedCacheNodesOfferingsMessageRequestTypeDef definition

class DescribeReservedCacheNodesOfferingsMessageRequestTypeDef(TypedDict):
    ReservedCacheNodesOfferingId: NotRequired[str],
    CacheNodeType: NotRequired[str],
    Duration: NotRequired[str],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeServerlessCacheSnapshotsRequestRequestTypeDef

```python
# DescribeServerlessCacheSnapshotsRequestRequestTypeDef definition

class DescribeServerlessCacheSnapshotsRequestRequestTypeDef(TypedDict):
    ServerlessCacheName: NotRequired[str],
    ServerlessCacheSnapshotName: NotRequired[str],
    SnapshotType: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeServerlessCachesRequestRequestTypeDef

```python
# DescribeServerlessCachesRequestRequestTypeDef definition

class DescribeServerlessCachesRequestRequestTypeDef(TypedDict):
    ServerlessCacheName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeServiceUpdatesMessageRequestTypeDef

```python
# DescribeServiceUpdatesMessageRequestTypeDef definition

class DescribeServiceUpdatesMessageRequestTypeDef(TypedDict):
    ServiceUpdateName: NotRequired[str],
    ServiceUpdateStatus: NotRequired[Sequence[ServiceUpdateStatusType]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
## DescribeSnapshotsMessageRequestTypeDef

```python
# DescribeSnapshotsMessageRequestTypeDef definition

class DescribeSnapshotsMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: NotRequired[str],
    CacheClusterId: NotRequired[str],
    SnapshotName: NotRequired[str],
    SnapshotSource: NotRequired[str],
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
    ShowNodeGroupConfig: NotRequired[bool],
```

## DescribeUserGroupsMessageRequestTypeDef

```python
# DescribeUserGroupsMessageRequestTypeDef definition

class DescribeUserGroupsMessageRequestTypeDef(TypedDict):
    UserGroupId: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: str,
    Values: Sequence[str],
```

## KinesisFirehoseDestinationDetailsTypeDef

```python
# KinesisFirehoseDestinationDetailsTypeDef definition

class KinesisFirehoseDestinationDetailsTypeDef(TypedDict):
    DeliveryStream: NotRequired[str],
```

## DisassociateGlobalReplicationGroupMessageRequestTypeDef

```python
# DisassociateGlobalReplicationGroupMessageRequestTypeDef definition

class DisassociateGlobalReplicationGroupMessageRequestTypeDef(TypedDict):
    GlobalReplicationGroupId: str,
    ReplicationGroupId: str,
    ReplicationGroupRegion: str,
```

## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    SourceIdentifier: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    Message: NotRequired[str],
    Date: NotRequired[datetime],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## ExportServerlessCacheSnapshotRequestRequestTypeDef

```python
# ExportServerlessCacheSnapshotRequestRequestTypeDef definition

class ExportServerlessCacheSnapshotRequestRequestTypeDef(TypedDict):
    ServerlessCacheSnapshotName: str,
    S3BucketName: str,
```

## FailoverGlobalReplicationGroupMessageRequestTypeDef

```python
# FailoverGlobalReplicationGroupMessageRequestTypeDef definition

class FailoverGlobalReplicationGroupMessageRequestTypeDef(TypedDict):
    GlobalReplicationGroupId: str,
    PrimaryRegion: str,
    PrimaryReplicationGroupId: str,
```

## GlobalNodeGroupTypeDef

```python
# GlobalNodeGroupTypeDef definition

class GlobalNodeGroupTypeDef(TypedDict):
    GlobalNodeGroupId: NotRequired[str],
    Slots: NotRequired[str],
```

## GlobalReplicationGroupInfoTypeDef

```python
# GlobalReplicationGroupInfoTypeDef definition

class GlobalReplicationGroupInfoTypeDef(TypedDict):
    GlobalReplicationGroupId: NotRequired[str],
    GlobalReplicationGroupMemberRole: NotRequired[str],
```

## GlobalReplicationGroupMemberTypeDef

```python
# GlobalReplicationGroupMemberTypeDef definition

class GlobalReplicationGroupMemberTypeDef(TypedDict):
    ReplicationGroupId: NotRequired[str],
    ReplicationGroupRegion: NotRequired[str],
    Role: NotRequired[str],
    AutomaticFailover: NotRequired[AutomaticFailoverStatusType],  # (1)
    Status: NotRequired[str],
```

1. See [:material-code-brackets: AutomaticFailoverStatusType](./literals.md#automaticfailoverstatustype) 
## ListAllowedNodeTypeModificationsMessageRequestTypeDef

```python
# ListAllowedNodeTypeModificationsMessageRequestTypeDef definition

class ListAllowedNodeTypeModificationsMessageRequestTypeDef(TypedDict):
    CacheClusterId: NotRequired[str],
    ReplicationGroupId: NotRequired[str],
```

## ListTagsForResourceMessageRequestTypeDef

```python
# ListTagsForResourceMessageRequestTypeDef definition

class ListTagsForResourceMessageRequestTypeDef(TypedDict):
    ResourceName: str,
```

## ParameterNameValueTypeDef

```python
# ParameterNameValueTypeDef definition

class ParameterNameValueTypeDef(TypedDict):
    ParameterName: NotRequired[str],
    ParameterValue: NotRequired[str],
```

## ModifyCacheSubnetGroupMessageRequestTypeDef

```python
# ModifyCacheSubnetGroupMessageRequestTypeDef definition

class ModifyCacheSubnetGroupMessageRequestTypeDef(TypedDict):
    CacheSubnetGroupName: str,
    CacheSubnetGroupDescription: NotRequired[str],
    SubnetIds: NotRequired[Sequence[str]],
```

## ModifyGlobalReplicationGroupMessageRequestTypeDef

```python
# ModifyGlobalReplicationGroupMessageRequestTypeDef definition

class ModifyGlobalReplicationGroupMessageRequestTypeDef(TypedDict):
    GlobalReplicationGroupId: str,
    ApplyImmediately: bool,
    CacheNodeType: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    CacheParameterGroupName: NotRequired[str],
    GlobalReplicationGroupDescription: NotRequired[str],
    AutomaticFailoverEnabled: NotRequired[bool],
```

## ReshardingConfigurationTypeDef

```python
# ReshardingConfigurationTypeDef definition

class ReshardingConfigurationTypeDef(TypedDict):
    NodeGroupId: NotRequired[str],
    PreferredAvailabilityZones: NotRequired[Sequence[str]],
```

## ModifyUserGroupMessageRequestTypeDef

```python
# ModifyUserGroupMessageRequestTypeDef definition

class ModifyUserGroupMessageRequestTypeDef(TypedDict):
    UserGroupId: str,
    UserIdsToAdd: NotRequired[Sequence[str]],
    UserIdsToRemove: NotRequired[Sequence[str]],
    Engine: NotRequired[str],
```

## NodeGroupConfigurationOutputTypeDef

```python
# NodeGroupConfigurationOutputTypeDef definition

class NodeGroupConfigurationOutputTypeDef(TypedDict):
    NodeGroupId: NotRequired[str],
    Slots: NotRequired[str],
    ReplicaCount: NotRequired[int],
    PrimaryAvailabilityZone: NotRequired[str],
    ReplicaAvailabilityZones: NotRequired[List[str]],
    PrimaryOutpostArn: NotRequired[str],
    ReplicaOutpostArns: NotRequired[List[str]],
```

## NodeGroupConfigurationTypeDef

```python
# NodeGroupConfigurationTypeDef definition

class NodeGroupConfigurationTypeDef(TypedDict):
    NodeGroupId: NotRequired[str],
    Slots: NotRequired[str],
    ReplicaCount: NotRequired[int],
    PrimaryAvailabilityZone: NotRequired[str],
    ReplicaAvailabilityZones: NotRequired[Sequence[str]],
    PrimaryOutpostArn: NotRequired[str],
    ReplicaOutpostArns: NotRequired[Sequence[str]],
```

## NodeGroupMemberUpdateStatusTypeDef

```python
# NodeGroupMemberUpdateStatusTypeDef definition

class NodeGroupMemberUpdateStatusTypeDef(TypedDict):
    CacheClusterId: NotRequired[str],
    CacheNodeId: NotRequired[str],
    NodeUpdateStatus: NotRequired[NodeUpdateStatusType],  # (1)
    NodeDeletionDate: NotRequired[datetime],
    NodeUpdateStartDate: NotRequired[datetime],
    NodeUpdateEndDate: NotRequired[datetime],
    NodeUpdateInitiatedBy: NotRequired[NodeUpdateInitiatedByType],  # (2)
    NodeUpdateInitiatedDate: NotRequired[datetime],
    NodeUpdateStatusModifiedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: NodeUpdateStatusType](./literals.md#nodeupdatestatustype) 
2. See [:material-code-brackets: NodeUpdateInitiatedByType](./literals.md#nodeupdateinitiatedbytype) 
## ProcessedUpdateActionTypeDef

```python
# ProcessedUpdateActionTypeDef definition

class ProcessedUpdateActionTypeDef(TypedDict):
    ReplicationGroupId: NotRequired[str],
    CacheClusterId: NotRequired[str],
    ServiceUpdateName: NotRequired[str],
    UpdateActionStatus: NotRequired[UpdateActionStatusType],  # (1)
```

1. See [:material-code-brackets: UpdateActionStatusType](./literals.md#updateactionstatustype) 
## RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef

```python
# RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef definition

class RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef(TypedDict):
    GlobalReplicationGroupId: str,
    ApplyImmediately: bool,
```

## RebootCacheClusterMessageRequestTypeDef

```python
# RebootCacheClusterMessageRequestTypeDef definition

class RebootCacheClusterMessageRequestTypeDef(TypedDict):
    CacheClusterId: str,
    CacheNodeIdsToReboot: Sequence[str],
```

## RecurringChargeTypeDef

```python
# RecurringChargeTypeDef definition

class RecurringChargeTypeDef(TypedDict):
    RecurringChargeAmount: NotRequired[float],
    RecurringChargeFrequency: NotRequired[str],
```

## RemoveTagsFromResourceMessageRequestTypeDef

```python
# RemoveTagsFromResourceMessageRequestTypeDef definition

class RemoveTagsFromResourceMessageRequestTypeDef(TypedDict):
    ResourceName: str,
    TagKeys: Sequence[str],
```

## UserGroupsUpdateStatusTypeDef

```python
# UserGroupsUpdateStatusTypeDef definition

class UserGroupsUpdateStatusTypeDef(TypedDict):
    UserGroupIdsToAdd: NotRequired[List[str]],
    UserGroupIdsToRemove: NotRequired[List[str]],
```

## SlotMigrationTypeDef

```python
# SlotMigrationTypeDef definition

class SlotMigrationTypeDef(TypedDict):
    ProgressPercentage: NotRequired[float],
```

## RevokeCacheSecurityGroupIngressMessageRequestTypeDef

```python
# RevokeCacheSecurityGroupIngressMessageRequestTypeDef definition

class RevokeCacheSecurityGroupIngressMessageRequestTypeDef(TypedDict):
    CacheSecurityGroupName: str,
    EC2SecurityGroupName: str,
    EC2SecurityGroupOwnerId: str,
```

## ServerlessCacheConfigurationTypeDef

```python
# ServerlessCacheConfigurationTypeDef definition

class ServerlessCacheConfigurationTypeDef(TypedDict):
    ServerlessCacheName: NotRequired[str],
    Engine: NotRequired[str],
    MajorEngineVersion: NotRequired[str],
```

## ServiceUpdateTypeDef

```python
# ServiceUpdateTypeDef definition

class ServiceUpdateTypeDef(TypedDict):
    ServiceUpdateName: NotRequired[str],
    ServiceUpdateReleaseDate: NotRequired[datetime],
    ServiceUpdateEndDate: NotRequired[datetime],
    ServiceUpdateSeverity: NotRequired[ServiceUpdateSeverityType],  # (1)
    ServiceUpdateRecommendedApplyByDate: NotRequired[datetime],
    ServiceUpdateStatus: NotRequired[ServiceUpdateStatusType],  # (2)
    ServiceUpdateDescription: NotRequired[str],
    ServiceUpdateType: NotRequired[ServiceUpdateTypeType],  # (3)
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    AutoUpdateAfterRecommendedApplyByDate: NotRequired[bool],
    EstimatedUpdateTime: NotRequired[str],
```

1. See [:material-code-brackets: ServiceUpdateSeverityType](./literals.md#serviceupdateseveritytype) 
2. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
3. See [:material-code-brackets: ServiceUpdateTypeType](./literals.md#serviceupdatetypetype) 
## SubnetOutpostTypeDef

```python
# SubnetOutpostTypeDef definition

class SubnetOutpostTypeDef(TypedDict):
    SubnetOutpostArn: NotRequired[str],
```

## TestFailoverMessageRequestTypeDef

```python
# TestFailoverMessageRequestTypeDef definition

class TestFailoverMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: str,
    NodeGroupId: str,
```

## UnprocessedUpdateActionTypeDef

```python
# UnprocessedUpdateActionTypeDef definition

class UnprocessedUpdateActionTypeDef(TypedDict):
    ReplicationGroupId: NotRequired[str],
    CacheClusterId: NotRequired[str],
    ServiceUpdateName: NotRequired[str],
    ErrorType: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## UserGroupPendingChangesTypeDef

```python
# UserGroupPendingChangesTypeDef definition

class UserGroupPendingChangesTypeDef(TypedDict):
    UserIdsToRemove: NotRequired[List[str]],
    UserIdsToAdd: NotRequired[List[str]],
```

## AddTagsToResourceMessageRequestTypeDef

```python
# AddTagsToResourceMessageRequestTypeDef definition

class AddTagsToResourceMessageRequestTypeDef(TypedDict):
    ResourceName: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CopyServerlessCacheSnapshotRequestRequestTypeDef

```python
# CopyServerlessCacheSnapshotRequestRequestTypeDef definition

class CopyServerlessCacheSnapshotRequestRequestTypeDef(TypedDict):
    SourceServerlessCacheSnapshotName: str,
    TargetServerlessCacheSnapshotName: str,
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CopySnapshotMessageRequestTypeDef

```python
# CopySnapshotMessageRequestTypeDef definition

class CopySnapshotMessageRequestTypeDef(TypedDict):
    SourceSnapshotName: str,
    TargetSnapshotName: str,
    TargetBucket: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCacheParameterGroupMessageRequestTypeDef

```python
# CreateCacheParameterGroupMessageRequestTypeDef definition

class CreateCacheParameterGroupMessageRequestTypeDef(TypedDict):
    CacheParameterGroupName: str,
    CacheParameterGroupFamily: str,
    Description: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCacheSecurityGroupMessageRequestTypeDef

```python
# CreateCacheSecurityGroupMessageRequestTypeDef definition

class CreateCacheSecurityGroupMessageRequestTypeDef(TypedDict):
    CacheSecurityGroupName: str,
    Description: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCacheSubnetGroupMessageRequestTypeDef

```python
# CreateCacheSubnetGroupMessageRequestTypeDef definition

class CreateCacheSubnetGroupMessageRequestTypeDef(TypedDict):
    CacheSubnetGroupName: str,
    CacheSubnetGroupDescription: str,
    SubnetIds: Sequence[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateServerlessCacheSnapshotRequestRequestTypeDef

```python
# CreateServerlessCacheSnapshotRequestRequestTypeDef definition

class CreateServerlessCacheSnapshotRequestRequestTypeDef(TypedDict):
    ServerlessCacheSnapshotName: str,
    ServerlessCacheName: str,
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSnapshotMessageRequestTypeDef

```python
# CreateSnapshotMessageRequestTypeDef definition

class CreateSnapshotMessageRequestTypeDef(TypedDict):
    SnapshotName: str,
    ReplicationGroupId: NotRequired[str],
    CacheClusterId: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateUserGroupMessageRequestTypeDef

```python
# CreateUserGroupMessageRequestTypeDef definition

class CreateUserGroupMessageRequestTypeDef(TypedDict):
    UserGroupId: str,
    Engine: str,
    UserIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PurchaseReservedCacheNodesOfferingMessageRequestTypeDef

```python
# PurchaseReservedCacheNodesOfferingMessageRequestTypeDef definition

class PurchaseReservedCacheNodesOfferingMessageRequestTypeDef(TypedDict):
    ReservedCacheNodesOfferingId: str,
    ReservedCacheNodeId: NotRequired[str],
    CacheNodeCount: NotRequired[int],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AllowedNodeTypeModificationsMessageTypeDef

```python
# AllowedNodeTypeModificationsMessageTypeDef definition

class AllowedNodeTypeModificationsMessageTypeDef(TypedDict):
    ScaleUpModifications: List[str],
    ScaleDownModifications: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CacheParameterGroupNameMessageTypeDef

```python
# CacheParameterGroupNameMessageTypeDef definition

class CacheParameterGroupNameMessageTypeDef(TypedDict):
    CacheParameterGroupName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagListMessageTypeDef

```python
# TagListMessageTypeDef definition

class TagListMessageTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserMessageRequestTypeDef

```python
# CreateUserMessageRequestTypeDef definition

class CreateUserMessageRequestTypeDef(TypedDict):
    UserId: str,
    UserName: str,
    Engine: str,
    AccessString: str,
    Passwords: NotRequired[Sequence[str]],
    NoPasswordRequired: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    AuthenticationMode: NotRequired[AuthenticationModeTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: AuthenticationModeTypeDef](./type_defs.md#authenticationmodetypedef) 
## ModifyUserMessageRequestTypeDef

```python
# ModifyUserMessageRequestTypeDef definition

class ModifyUserMessageRequestTypeDef(TypedDict):
    UserId: str,
    AccessString: NotRequired[str],
    AppendAccessString: NotRequired[str],
    Passwords: NotRequired[Sequence[str]],
    NoPasswordRequired: NotRequired[bool],
    AuthenticationMode: NotRequired[AuthenticationModeTypeDef],  # (1)
    Engine: NotRequired[str],
```

1. See [:material-code-braces: AuthenticationModeTypeDef](./type_defs.md#authenticationmodetypedef) 
## UserResponseTypeDef

```python
# UserResponseTypeDef definition

class UserResponseTypeDef(TypedDict):
    UserId: str,
    UserName: str,
    Status: str,
    Engine: str,
    MinimumEngineVersion: str,
    AccessString: str,
    UserGroupIds: List[str],
    Authentication: AuthenticationTypeDef,  # (1)
    ARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthenticationTypeDef](./type_defs.md#authenticationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    UserId: NotRequired[str],
    UserName: NotRequired[str],
    Status: NotRequired[str],
    Engine: NotRequired[str],
    MinimumEngineVersion: NotRequired[str],
    AccessString: NotRequired[str],
    UserGroupIds: NotRequired[List[str]],
    Authentication: NotRequired[AuthenticationTypeDef],  # (1)
    ARN: NotRequired[str],
```

1. See [:material-code-braces: AuthenticationTypeDef](./type_defs.md#authenticationtypedef) 
## CacheNodeTypeDef

```python
# CacheNodeTypeDef definition

class CacheNodeTypeDef(TypedDict):
    CacheNodeId: NotRequired[str],
    CacheNodeStatus: NotRequired[str],
    CacheNodeCreateTime: NotRequired[datetime],
    Endpoint: NotRequired[EndpointTypeDef],  # (1)
    ParameterGroupStatus: NotRequired[str],
    SourceCacheNodeId: NotRequired[str],
    CustomerAvailabilityZone: NotRequired[str],
    CustomerOutpostArn: NotRequired[str],
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
## NodeGroupMemberTypeDef

```python
# NodeGroupMemberTypeDef definition

class NodeGroupMemberTypeDef(TypedDict):
    CacheClusterId: NotRequired[str],
    CacheNodeId: NotRequired[str],
    ReadEndpoint: NotRequired[EndpointTypeDef],  # (1)
    PreferredAvailabilityZone: NotRequired[str],
    PreferredOutpostArn: NotRequired[str],
    CurrentRole: NotRequired[str],
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
## CacheEngineVersionMessageTypeDef

```python
# CacheEngineVersionMessageTypeDef definition

class CacheEngineVersionMessageTypeDef(TypedDict):
    Marker: str,
    CacheEngineVersions: List[CacheEngineVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheEngineVersionTypeDef](./type_defs.md#cacheengineversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CacheNodeTypeSpecificParameterTypeDef

```python
# CacheNodeTypeSpecificParameterTypeDef definition

class CacheNodeTypeSpecificParameterTypeDef(TypedDict):
    ParameterName: NotRequired[str],
    Description: NotRequired[str],
    Source: NotRequired[str],
    DataType: NotRequired[str],
    AllowedValues: NotRequired[str],
    IsModifiable: NotRequired[bool],
    MinimumEngineVersion: NotRequired[str],
    CacheNodeTypeSpecificValues: NotRequired[List[CacheNodeTypeSpecificValueTypeDef]],  # (1)
    ChangeType: NotRequired[ChangeTypeType],  # (2)
```

1. See [:material-code-braces: CacheNodeTypeSpecificValueTypeDef](./type_defs.md#cachenodetypespecificvaluetypedef) 
2. See [:material-code-brackets: ChangeTypeType](./literals.md#changetypetype) 
## CacheParameterGroupsMessageTypeDef

```python
# CacheParameterGroupsMessageTypeDef definition

class CacheParameterGroupsMessageTypeDef(TypedDict):
    Marker: str,
    CacheParameterGroups: List[CacheParameterGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheParameterGroupTypeDef](./type_defs.md#cacheparametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCacheParameterGroupResultTypeDef

```python
# CreateCacheParameterGroupResultTypeDef definition

class CreateCacheParameterGroupResultTypeDef(TypedDict):
    CacheParameterGroup: CacheParameterGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheParameterGroupTypeDef](./type_defs.md#cacheparametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CacheSecurityGroupTypeDef

```python
# CacheSecurityGroupTypeDef definition

class CacheSecurityGroupTypeDef(TypedDict):
    OwnerId: NotRequired[str],
    CacheSecurityGroupName: NotRequired[str],
    Description: NotRequired[str],
    EC2SecurityGroups: NotRequired[List[EC2SecurityGroupTypeDef]],  # (1)
    ARN: NotRequired[str],
```

1. See [:material-code-braces: EC2SecurityGroupTypeDef](./type_defs.md#ec2securitygrouptypedef) 
## CacheUsageLimitsTypeDef

```python
# CacheUsageLimitsTypeDef definition

class CacheUsageLimitsTypeDef(TypedDict):
    DataStorage: NotRequired[DataStorageTypeDef],  # (1)
    ECPUPerSecond: NotRequired[ECPUPerSecondTypeDef],  # (2)
```

1. See [:material-code-braces: DataStorageTypeDef](./type_defs.md#datastoragetypedef) 
2. See [:material-code-braces: ECPUPerSecondTypeDef](./type_defs.md#ecpupersecondtypedef) 
## DecreaseReplicaCountMessageRequestTypeDef

```python
# DecreaseReplicaCountMessageRequestTypeDef definition

class DecreaseReplicaCountMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: str,
    ApplyImmediately: bool,
    NewReplicaCount: NotRequired[int],
    ReplicaConfiguration: NotRequired[Sequence[ConfigureShardTypeDef]],  # (1)
    ReplicasToRemove: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ConfigureShardTypeDef](./type_defs.md#configureshardtypedef) 
## IncreaseReplicaCountMessageRequestTypeDef

```python
# IncreaseReplicaCountMessageRequestTypeDef definition

class IncreaseReplicaCountMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: str,
    ApplyImmediately: bool,
    NewReplicaCount: NotRequired[int],
    ReplicaConfiguration: NotRequired[Sequence[ConfigureShardTypeDef]],  # (1)
```

1. See [:material-code-braces: ConfigureShardTypeDef](./type_defs.md#configureshardtypedef) 
## StartMigrationMessageRequestTypeDef

```python
# StartMigrationMessageRequestTypeDef definition

class StartMigrationMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: str,
    CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef],  # (1)
```

1. See [:material-code-braces: CustomerNodeEndpointTypeDef](./type_defs.md#customernodeendpointtypedef) 
## TestMigrationMessageRequestTypeDef

```python
# TestMigrationMessageRequestTypeDef definition

class TestMigrationMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: str,
    CustomerNodeEndpointList: Sequence[CustomerNodeEndpointTypeDef],  # (1)
```

1. See [:material-code-braces: CustomerNodeEndpointTypeDef](./type_defs.md#customernodeendpointtypedef) 
## DescribeCacheClustersMessagePaginateTypeDef

```python
# DescribeCacheClustersMessagePaginateTypeDef definition

class DescribeCacheClustersMessagePaginateTypeDef(TypedDict):
    CacheClusterId: NotRequired[str],
    ShowCacheNodeInfo: NotRequired[bool],
    ShowCacheClustersNotInReplicationGroups: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeCacheEngineVersionsMessagePaginateTypeDef

```python
# DescribeCacheEngineVersionsMessagePaginateTypeDef definition

class DescribeCacheEngineVersionsMessagePaginateTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    CacheParameterGroupFamily: NotRequired[str],
    DefaultOnly: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeCacheParameterGroupsMessagePaginateTypeDef

```python
# DescribeCacheParameterGroupsMessagePaginateTypeDef definition

class DescribeCacheParameterGroupsMessagePaginateTypeDef(TypedDict):
    CacheParameterGroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeCacheParametersMessagePaginateTypeDef

```python
# DescribeCacheParametersMessagePaginateTypeDef definition

class DescribeCacheParametersMessagePaginateTypeDef(TypedDict):
    CacheParameterGroupName: str,
    Source: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeCacheSecurityGroupsMessagePaginateTypeDef

```python
# DescribeCacheSecurityGroupsMessagePaginateTypeDef definition

class DescribeCacheSecurityGroupsMessagePaginateTypeDef(TypedDict):
    CacheSecurityGroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeCacheSubnetGroupsMessagePaginateTypeDef

```python
# DescribeCacheSubnetGroupsMessagePaginateTypeDef definition

class DescribeCacheSubnetGroupsMessagePaginateTypeDef(TypedDict):
    CacheSubnetGroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEngineDefaultParametersMessagePaginateTypeDef

```python
# DescribeEngineDefaultParametersMessagePaginateTypeDef definition

class DescribeEngineDefaultParametersMessagePaginateTypeDef(TypedDict):
    CacheParameterGroupFamily: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeGlobalReplicationGroupsMessagePaginateTypeDef

```python
# DescribeGlobalReplicationGroupsMessagePaginateTypeDef definition

class DescribeGlobalReplicationGroupsMessagePaginateTypeDef(TypedDict):
    GlobalReplicationGroupId: NotRequired[str],
    ShowMemberInfo: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReplicationGroupsMessagePaginateTypeDef

```python
# DescribeReplicationGroupsMessagePaginateTypeDef definition

class DescribeReplicationGroupsMessagePaginateTypeDef(TypedDict):
    ReplicationGroupId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReservedCacheNodesMessagePaginateTypeDef

```python
# DescribeReservedCacheNodesMessagePaginateTypeDef definition

class DescribeReservedCacheNodesMessagePaginateTypeDef(TypedDict):
    ReservedCacheNodeId: NotRequired[str],
    ReservedCacheNodesOfferingId: NotRequired[str],
    CacheNodeType: NotRequired[str],
    Duration: NotRequired[str],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReservedCacheNodesOfferingsMessagePaginateTypeDef

```python
# DescribeReservedCacheNodesOfferingsMessagePaginateTypeDef definition

class DescribeReservedCacheNodesOfferingsMessagePaginateTypeDef(TypedDict):
    ReservedCacheNodesOfferingId: NotRequired[str],
    CacheNodeType: NotRequired[str],
    Duration: NotRequired[str],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeServerlessCacheSnapshotsRequestPaginateTypeDef

```python
# DescribeServerlessCacheSnapshotsRequestPaginateTypeDef definition

class DescribeServerlessCacheSnapshotsRequestPaginateTypeDef(TypedDict):
    ServerlessCacheName: NotRequired[str],
    ServerlessCacheSnapshotName: NotRequired[str],
    SnapshotType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeServerlessCachesRequestPaginateTypeDef

```python
# DescribeServerlessCachesRequestPaginateTypeDef definition

class DescribeServerlessCachesRequestPaginateTypeDef(TypedDict):
    ServerlessCacheName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeServiceUpdatesMessagePaginateTypeDef

```python
# DescribeServiceUpdatesMessagePaginateTypeDef definition

class DescribeServiceUpdatesMessagePaginateTypeDef(TypedDict):
    ServiceUpdateName: NotRequired[str],
    ServiceUpdateStatus: NotRequired[Sequence[ServiceUpdateStatusType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSnapshotsMessagePaginateTypeDef

```python
# DescribeSnapshotsMessagePaginateTypeDef definition

class DescribeSnapshotsMessagePaginateTypeDef(TypedDict):
    ReplicationGroupId: NotRequired[str],
    CacheClusterId: NotRequired[str],
    SnapshotName: NotRequired[str],
    SnapshotSource: NotRequired[str],
    ShowNodeGroupConfig: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeUserGroupsMessagePaginateTypeDef

```python
# DescribeUserGroupsMessagePaginateTypeDef definition

class DescribeUserGroupsMessagePaginateTypeDef(TypedDict):
    UserGroupId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeCacheClustersMessageWaitTypeDef

```python
# DescribeCacheClustersMessageWaitTypeDef definition

class DescribeCacheClustersMessageWaitTypeDef(TypedDict):
    CacheClusterId: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    ShowCacheNodeInfo: NotRequired[bool],
    ShowCacheClustersNotInReplicationGroups: NotRequired[bool],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeReplicationGroupsMessageWaitTypeDef

```python
# DescribeReplicationGroupsMessageWaitTypeDef definition

class DescribeReplicationGroupsMessageWaitTypeDef(TypedDict):
    ReplicationGroupId: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEventsMessagePaginateTypeDef

```python
# DescribeEventsMessagePaginateTypeDef definition

class DescribeEventsMessagePaginateTypeDef(TypedDict):
    SourceIdentifier: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Duration: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsMessageRequestTypeDef

```python
# DescribeEventsMessageRequestTypeDef definition

class DescribeEventsMessageRequestTypeDef(TypedDict):
    SourceIdentifier: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Duration: NotRequired[int],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## TimeRangeFilterTypeDef

```python
# TimeRangeFilterTypeDef definition

class TimeRangeFilterTypeDef(TypedDict):
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
```

## DescribeUsersMessagePaginateTypeDef

```python
# DescribeUsersMessagePaginateTypeDef definition

class DescribeUsersMessagePaginateTypeDef(TypedDict):
    Engine: NotRequired[str],
    UserId: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeUsersMessageRequestTypeDef

```python
# DescribeUsersMessageRequestTypeDef definition

class DescribeUsersMessageRequestTypeDef(TypedDict):
    Engine: NotRequired[str],
    UserId: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DestinationDetailsTypeDef

```python
# DestinationDetailsTypeDef definition

class DestinationDetailsTypeDef(TypedDict):
    CloudWatchLogsDetails: NotRequired[CloudWatchLogsDestinationDetailsTypeDef],  # (1)
    KinesisFirehoseDetails: NotRequired[KinesisFirehoseDestinationDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: CloudWatchLogsDestinationDetailsTypeDef](./type_defs.md#cloudwatchlogsdestinationdetailstypedef) 
2. See [:material-code-braces: KinesisFirehoseDestinationDetailsTypeDef](./type_defs.md#kinesisfirehosedestinationdetailstypedef) 
## EventsMessageTypeDef

```python
# EventsMessageTypeDef definition

class EventsMessageTypeDef(TypedDict):
    Marker: str,
    Events: List[EventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GlobalReplicationGroupTypeDef

```python
# GlobalReplicationGroupTypeDef definition

class GlobalReplicationGroupTypeDef(TypedDict):
    GlobalReplicationGroupId: NotRequired[str],
    GlobalReplicationGroupDescription: NotRequired[str],
    Status: NotRequired[str],
    CacheNodeType: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    Members: NotRequired[List[GlobalReplicationGroupMemberTypeDef]],  # (1)
    ClusterEnabled: NotRequired[bool],
    GlobalNodeGroups: NotRequired[List[GlobalNodeGroupTypeDef]],  # (2)
    AuthTokenEnabled: NotRequired[bool],
    TransitEncryptionEnabled: NotRequired[bool],
    AtRestEncryptionEnabled: NotRequired[bool],
    ARN: NotRequired[str],
```

1. See [:material-code-braces: GlobalReplicationGroupMemberTypeDef](./type_defs.md#globalreplicationgroupmembertypedef) 
2. See [:material-code-braces: GlobalNodeGroupTypeDef](./type_defs.md#globalnodegrouptypedef) 
## ModifyCacheParameterGroupMessageRequestTypeDef

```python
# ModifyCacheParameterGroupMessageRequestTypeDef definition

class ModifyCacheParameterGroupMessageRequestTypeDef(TypedDict):
    CacheParameterGroupName: str,
    ParameterNameValues: Sequence[ParameterNameValueTypeDef],  # (1)
```

1. See [:material-code-braces: ParameterNameValueTypeDef](./type_defs.md#parameternamevaluetypedef) 
## ResetCacheParameterGroupMessageRequestTypeDef

```python
# ResetCacheParameterGroupMessageRequestTypeDef definition

class ResetCacheParameterGroupMessageRequestTypeDef(TypedDict):
    CacheParameterGroupName: str,
    ResetAllParameters: NotRequired[bool],
    ParameterNameValues: NotRequired[Sequence[ParameterNameValueTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterNameValueTypeDef](./type_defs.md#parameternamevaluetypedef) 
## ModifyReplicationGroupShardConfigurationMessageRequestTypeDef

```python
# ModifyReplicationGroupShardConfigurationMessageRequestTypeDef definition

class ModifyReplicationGroupShardConfigurationMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: str,
    NodeGroupCount: int,
    ApplyImmediately: bool,
    ReshardingConfiguration: NotRequired[Sequence[ReshardingConfigurationTypeDef]],  # (1)
    NodeGroupsToRemove: NotRequired[Sequence[str]],
    NodeGroupsToRetain: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ReshardingConfigurationTypeDef](./type_defs.md#reshardingconfigurationtypedef) 
## RegionalConfigurationTypeDef

```python
# RegionalConfigurationTypeDef definition

class RegionalConfigurationTypeDef(TypedDict):
    ReplicationGroupId: str,
    ReplicationGroupRegion: str,
    ReshardingConfiguration: Sequence[ReshardingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ReshardingConfigurationTypeDef](./type_defs.md#reshardingconfigurationtypedef) 
## NodeSnapshotTypeDef

```python
# NodeSnapshotTypeDef definition

class NodeSnapshotTypeDef(TypedDict):
    CacheClusterId: NotRequired[str],
    NodeGroupId: NotRequired[str],
    CacheNodeId: NotRequired[str],
    NodeGroupConfiguration: NotRequired[NodeGroupConfigurationOutputTypeDef],  # (1)
    CacheSize: NotRequired[str],
    CacheNodeCreateTime: NotRequired[datetime],
    SnapshotCreateTime: NotRequired[datetime],
```

1. See [:material-code-braces: NodeGroupConfigurationOutputTypeDef](./type_defs.md#nodegroupconfigurationoutputtypedef) 
## NodeGroupUpdateStatusTypeDef

```python
# NodeGroupUpdateStatusTypeDef definition

class NodeGroupUpdateStatusTypeDef(TypedDict):
    NodeGroupId: NotRequired[str],
    NodeGroupMemberUpdateStatus: NotRequired[List[NodeGroupMemberUpdateStatusTypeDef]],  # (1)
```

1. See [:material-code-braces: NodeGroupMemberUpdateStatusTypeDef](./type_defs.md#nodegroupmemberupdatestatustypedef) 
## ReservedCacheNodeTypeDef

```python
# ReservedCacheNodeTypeDef definition

class ReservedCacheNodeTypeDef(TypedDict):
    ReservedCacheNodeId: NotRequired[str],
    ReservedCacheNodesOfferingId: NotRequired[str],
    CacheNodeType: NotRequired[str],
    StartTime: NotRequired[datetime],
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    UsagePrice: NotRequired[float],
    CacheNodeCount: NotRequired[int],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    State: NotRequired[str],
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (1)
    ReservationARN: NotRequired[str],
```

1. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
## ReservedCacheNodesOfferingTypeDef

```python
# ReservedCacheNodesOfferingTypeDef definition

class ReservedCacheNodesOfferingTypeDef(TypedDict):
    ReservedCacheNodesOfferingId: NotRequired[str],
    CacheNodeType: NotRequired[str],
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    UsagePrice: NotRequired[float],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (1)
```

1. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
## ReshardingStatusTypeDef

```python
# ReshardingStatusTypeDef definition

class ReshardingStatusTypeDef(TypedDict):
    SlotMigration: NotRequired[SlotMigrationTypeDef],  # (1)
```

1. See [:material-code-braces: SlotMigrationTypeDef](./type_defs.md#slotmigrationtypedef) 
## ServerlessCacheSnapshotTypeDef

```python
# ServerlessCacheSnapshotTypeDef definition

class ServerlessCacheSnapshotTypeDef(TypedDict):
    ServerlessCacheSnapshotName: NotRequired[str],
    ARN: NotRequired[str],
    KmsKeyId: NotRequired[str],
    SnapshotType: NotRequired[str],
    Status: NotRequired[str],
    CreateTime: NotRequired[datetime],
    ExpiryTime: NotRequired[datetime],
    BytesUsedForCache: NotRequired[str],
    ServerlessCacheConfiguration: NotRequired[ServerlessCacheConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ServerlessCacheConfigurationTypeDef](./type_defs.md#serverlesscacheconfigurationtypedef) 
## ServiceUpdatesMessageTypeDef

```python
# ServiceUpdatesMessageTypeDef definition

class ServiceUpdatesMessageTypeDef(TypedDict):
    Marker: str,
    ServiceUpdates: List[ServiceUpdateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceUpdateTypeDef](./type_defs.md#serviceupdatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubnetTypeDef

```python
# SubnetTypeDef definition

class SubnetTypeDef(TypedDict):
    SubnetIdentifier: NotRequired[str],
    SubnetAvailabilityZone: NotRequired[AvailabilityZoneTypeDef],  # (1)
    SubnetOutpost: NotRequired[SubnetOutpostTypeDef],  # (2)
    SupportedNetworkTypes: NotRequired[List[NetworkTypeType]],  # (3)
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
2. See [:material-code-braces: SubnetOutpostTypeDef](./type_defs.md#subnetoutposttypedef) 
3. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
## UpdateActionResultsMessageTypeDef

```python
# UpdateActionResultsMessageTypeDef definition

class UpdateActionResultsMessageTypeDef(TypedDict):
    ProcessedUpdateActions: List[ProcessedUpdateActionTypeDef],  # (1)
    UnprocessedUpdateActions: List[UnprocessedUpdateActionTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProcessedUpdateActionTypeDef](./type_defs.md#processedupdateactiontypedef) 
2. See [:material-code-braces: UnprocessedUpdateActionTypeDef](./type_defs.md#unprocessedupdateactiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UserGroupResponseTypeDef

```python
# UserGroupResponseTypeDef definition

class UserGroupResponseTypeDef(TypedDict):
    UserGroupId: str,
    Status: str,
    Engine: str,
    UserIds: List[str],
    MinimumEngineVersion: str,
    PendingChanges: UserGroupPendingChangesTypeDef,  # (1)
    ReplicationGroups: List[str],
    ServerlessCaches: List[str],
    ARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserGroupPendingChangesTypeDef](./type_defs.md#usergrouppendingchangestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UserGroupTypeDef

```python
# UserGroupTypeDef definition

class UserGroupTypeDef(TypedDict):
    UserGroupId: NotRequired[str],
    Status: NotRequired[str],
    Engine: NotRequired[str],
    UserIds: NotRequired[List[str]],
    MinimumEngineVersion: NotRequired[str],
    PendingChanges: NotRequired[UserGroupPendingChangesTypeDef],  # (1)
    ReplicationGroups: NotRequired[List[str]],
    ServerlessCaches: NotRequired[List[str]],
    ARN: NotRequired[str],
```

1. See [:material-code-braces: UserGroupPendingChangesTypeDef](./type_defs.md#usergrouppendingchangestypedef) 
## DescribeUsersResultTypeDef

```python
# DescribeUsersResultTypeDef definition

class DescribeUsersResultTypeDef(TypedDict):
    Users: List[UserTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NodeGroupTypeDef

```python
# NodeGroupTypeDef definition

class NodeGroupTypeDef(TypedDict):
    NodeGroupId: NotRequired[str],
    Status: NotRequired[str],
    PrimaryEndpoint: NotRequired[EndpointTypeDef],  # (1)
    ReaderEndpoint: NotRequired[EndpointTypeDef],  # (1)
    Slots: NotRequired[str],
    NodeGroupMembers: NotRequired[List[NodeGroupMemberTypeDef]],  # (3)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
3. See [:material-code-braces: NodeGroupMemberTypeDef](./type_defs.md#nodegroupmembertypedef) 
## CacheParameterGroupDetailsTypeDef

```python
# CacheParameterGroupDetailsTypeDef definition

class CacheParameterGroupDetailsTypeDef(TypedDict):
    Marker: str,
    Parameters: List[ParameterTypeDef],  # (1)
    CacheNodeTypeSpecificParameters: List[CacheNodeTypeSpecificParameterTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: CacheNodeTypeSpecificParameterTypeDef](./type_defs.md#cachenodetypespecificparametertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EngineDefaultsTypeDef

```python
# EngineDefaultsTypeDef definition

class EngineDefaultsTypeDef(TypedDict):
    CacheParameterGroupFamily: NotRequired[str],
    Marker: NotRequired[str],
    Parameters: NotRequired[List[ParameterTypeDef]],  # (1)
    CacheNodeTypeSpecificParameters: NotRequired[List[CacheNodeTypeSpecificParameterTypeDef]],  # (2)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: CacheNodeTypeSpecificParameterTypeDef](./type_defs.md#cachenodetypespecificparametertypedef) 
## AuthorizeCacheSecurityGroupIngressResultTypeDef

```python
# AuthorizeCacheSecurityGroupIngressResultTypeDef definition

class AuthorizeCacheSecurityGroupIngressResultTypeDef(TypedDict):
    CacheSecurityGroup: CacheSecurityGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheSecurityGroupTypeDef](./type_defs.md#cachesecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CacheSecurityGroupMessageTypeDef

```python
# CacheSecurityGroupMessageTypeDef definition

class CacheSecurityGroupMessageTypeDef(TypedDict):
    Marker: str,
    CacheSecurityGroups: List[CacheSecurityGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheSecurityGroupTypeDef](./type_defs.md#cachesecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCacheSecurityGroupResultTypeDef

```python
# CreateCacheSecurityGroupResultTypeDef definition

class CreateCacheSecurityGroupResultTypeDef(TypedDict):
    CacheSecurityGroup: CacheSecurityGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheSecurityGroupTypeDef](./type_defs.md#cachesecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RevokeCacheSecurityGroupIngressResultTypeDef

```python
# RevokeCacheSecurityGroupIngressResultTypeDef definition

class RevokeCacheSecurityGroupIngressResultTypeDef(TypedDict):
    CacheSecurityGroup: CacheSecurityGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheSecurityGroupTypeDef](./type_defs.md#cachesecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServerlessCacheRequestRequestTypeDef

```python
# CreateServerlessCacheRequestRequestTypeDef definition

class CreateServerlessCacheRequestRequestTypeDef(TypedDict):
    ServerlessCacheName: str,
    Engine: str,
    Description: NotRequired[str],
    MajorEngineVersion: NotRequired[str],
    CacheUsageLimits: NotRequired[CacheUsageLimitsTypeDef],  # (1)
    KmsKeyId: NotRequired[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    SnapshotArnsToRestore: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    UserGroupId: NotRequired[str],
    SubnetIds: NotRequired[Sequence[str]],
    SnapshotRetentionLimit: NotRequired[int],
    DailySnapshotTime: NotRequired[str],
```

1. See [:material-code-braces: CacheUsageLimitsTypeDef](./type_defs.md#cacheusagelimitstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ModifyServerlessCacheRequestRequestTypeDef

```python
# ModifyServerlessCacheRequestRequestTypeDef definition

class ModifyServerlessCacheRequestRequestTypeDef(TypedDict):
    ServerlessCacheName: str,
    Description: NotRequired[str],
    CacheUsageLimits: NotRequired[CacheUsageLimitsTypeDef],  # (1)
    RemoveUserGroup: NotRequired[bool],
    UserGroupId: NotRequired[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    SnapshotRetentionLimit: NotRequired[int],
    DailySnapshotTime: NotRequired[str],
    Engine: NotRequired[str],
    MajorEngineVersion: NotRequired[str],
```

1. See [:material-code-braces: CacheUsageLimitsTypeDef](./type_defs.md#cacheusagelimitstypedef) 
## ServerlessCacheTypeDef

```python
# ServerlessCacheTypeDef definition

class ServerlessCacheTypeDef(TypedDict):
    ServerlessCacheName: NotRequired[str],
    Description: NotRequired[str],
    CreateTime: NotRequired[datetime],
    Status: NotRequired[str],
    Engine: NotRequired[str],
    MajorEngineVersion: NotRequired[str],
    FullEngineVersion: NotRequired[str],
    CacheUsageLimits: NotRequired[CacheUsageLimitsTypeDef],  # (1)
    KmsKeyId: NotRequired[str],
    SecurityGroupIds: NotRequired[List[str]],
    Endpoint: NotRequired[EndpointTypeDef],  # (2)
    ReaderEndpoint: NotRequired[EndpointTypeDef],  # (2)
    ARN: NotRequired[str],
    UserGroupId: NotRequired[str],
    SubnetIds: NotRequired[List[str]],
    SnapshotRetentionLimit: NotRequired[int],
    DailySnapshotTime: NotRequired[str],
```

1. See [:material-code-braces: CacheUsageLimitsTypeDef](./type_defs.md#cacheusagelimitstypedef) 
2. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
3. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
## DescribeUpdateActionsMessagePaginateTypeDef

```python
# DescribeUpdateActionsMessagePaginateTypeDef definition

class DescribeUpdateActionsMessagePaginateTypeDef(TypedDict):
    ServiceUpdateName: NotRequired[str],
    ReplicationGroupIds: NotRequired[Sequence[str]],
    CacheClusterIds: NotRequired[Sequence[str]],
    Engine: NotRequired[str],
    ServiceUpdateStatus: NotRequired[Sequence[ServiceUpdateStatusType]],  # (1)
    ServiceUpdateTimeRange: NotRequired[TimeRangeFilterTypeDef],  # (2)
    UpdateActionStatus: NotRequired[Sequence[UpdateActionStatusType]],  # (3)
    ShowNodeLevelUpdateStatus: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
2. See [:material-code-braces: TimeRangeFilterTypeDef](./type_defs.md#timerangefiltertypedef) 
3. See [:material-code-brackets: UpdateActionStatusType](./literals.md#updateactionstatustype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeUpdateActionsMessageRequestTypeDef

```python
# DescribeUpdateActionsMessageRequestTypeDef definition

class DescribeUpdateActionsMessageRequestTypeDef(TypedDict):
    ServiceUpdateName: NotRequired[str],
    ReplicationGroupIds: NotRequired[Sequence[str]],
    CacheClusterIds: NotRequired[Sequence[str]],
    Engine: NotRequired[str],
    ServiceUpdateStatus: NotRequired[Sequence[ServiceUpdateStatusType]],  # (1)
    ServiceUpdateTimeRange: NotRequired[TimeRangeFilterTypeDef],  # (2)
    UpdateActionStatus: NotRequired[Sequence[UpdateActionStatusType]],  # (3)
    ShowNodeLevelUpdateStatus: NotRequired[bool],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
2. See [:material-code-braces: TimeRangeFilterTypeDef](./type_defs.md#timerangefiltertypedef) 
3. See [:material-code-brackets: UpdateActionStatusType](./literals.md#updateactionstatustype) 
## LogDeliveryConfigurationRequestTypeDef

```python
# LogDeliveryConfigurationRequestTypeDef definition

class LogDeliveryConfigurationRequestTypeDef(TypedDict):
    LogType: NotRequired[LogTypeType],  # (1)
    DestinationType: NotRequired[DestinationTypeType],  # (2)
    DestinationDetails: NotRequired[DestinationDetailsTypeDef],  # (3)
    LogFormat: NotRequired[LogFormatType],  # (4)
    Enabled: NotRequired[bool],
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype) 
3. See [:material-code-braces: DestinationDetailsTypeDef](./type_defs.md#destinationdetailstypedef) 
4. See [:material-code-brackets: LogFormatType](./literals.md#logformattype) 
## LogDeliveryConfigurationTypeDef

```python
# LogDeliveryConfigurationTypeDef definition

class LogDeliveryConfigurationTypeDef(TypedDict):
    LogType: NotRequired[LogTypeType],  # (1)
    DestinationType: NotRequired[DestinationTypeType],  # (2)
    DestinationDetails: NotRequired[DestinationDetailsTypeDef],  # (3)
    LogFormat: NotRequired[LogFormatType],  # (4)
    Status: NotRequired[LogDeliveryConfigurationStatusType],  # (5)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype) 
3. See [:material-code-braces: DestinationDetailsTypeDef](./type_defs.md#destinationdetailstypedef) 
4. See [:material-code-brackets: LogFormatType](./literals.md#logformattype) 
5. See [:material-code-brackets: LogDeliveryConfigurationStatusType](./literals.md#logdeliveryconfigurationstatustype) 
## PendingLogDeliveryConfigurationTypeDef

```python
# PendingLogDeliveryConfigurationTypeDef definition

class PendingLogDeliveryConfigurationTypeDef(TypedDict):
    LogType: NotRequired[LogTypeType],  # (1)
    DestinationType: NotRequired[DestinationTypeType],  # (2)
    DestinationDetails: NotRequired[DestinationDetailsTypeDef],  # (3)
    LogFormat: NotRequired[LogFormatType],  # (4)
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype) 
3. See [:material-code-braces: DestinationDetailsTypeDef](./type_defs.md#destinationdetailstypedef) 
4. See [:material-code-brackets: LogFormatType](./literals.md#logformattype) 
## CreateGlobalReplicationGroupResultTypeDef

```python
# CreateGlobalReplicationGroupResultTypeDef definition

class CreateGlobalReplicationGroupResultTypeDef(TypedDict):
    GlobalReplicationGroup: GlobalReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalReplicationGroupTypeDef](./type_defs.md#globalreplicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef

```python
# DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef definition

class DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef(TypedDict):
    GlobalReplicationGroup: GlobalReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalReplicationGroupTypeDef](./type_defs.md#globalreplicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGlobalReplicationGroupResultTypeDef

```python
# DeleteGlobalReplicationGroupResultTypeDef definition

class DeleteGlobalReplicationGroupResultTypeDef(TypedDict):
    GlobalReplicationGroup: GlobalReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalReplicationGroupTypeDef](./type_defs.md#globalreplicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGlobalReplicationGroupsResultTypeDef

```python
# DescribeGlobalReplicationGroupsResultTypeDef definition

class DescribeGlobalReplicationGroupsResultTypeDef(TypedDict):
    Marker: str,
    GlobalReplicationGroups: List[GlobalReplicationGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalReplicationGroupTypeDef](./type_defs.md#globalreplicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateGlobalReplicationGroupResultTypeDef

```python
# DisassociateGlobalReplicationGroupResultTypeDef definition

class DisassociateGlobalReplicationGroupResultTypeDef(TypedDict):
    GlobalReplicationGroup: GlobalReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalReplicationGroupTypeDef](./type_defs.md#globalreplicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FailoverGlobalReplicationGroupResultTypeDef

```python
# FailoverGlobalReplicationGroupResultTypeDef definition

class FailoverGlobalReplicationGroupResultTypeDef(TypedDict):
    GlobalReplicationGroup: GlobalReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalReplicationGroupTypeDef](./type_defs.md#globalreplicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef

```python
# IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef definition

class IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef(TypedDict):
    GlobalReplicationGroup: GlobalReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalReplicationGroupTypeDef](./type_defs.md#globalreplicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyGlobalReplicationGroupResultTypeDef

```python
# ModifyGlobalReplicationGroupResultTypeDef definition

class ModifyGlobalReplicationGroupResultTypeDef(TypedDict):
    GlobalReplicationGroup: GlobalReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalReplicationGroupTypeDef](./type_defs.md#globalreplicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RebalanceSlotsInGlobalReplicationGroupResultTypeDef

```python
# RebalanceSlotsInGlobalReplicationGroupResultTypeDef definition

class RebalanceSlotsInGlobalReplicationGroupResultTypeDef(TypedDict):
    GlobalReplicationGroup: GlobalReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalReplicationGroupTypeDef](./type_defs.md#globalreplicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef

```python
# IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef definition

class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(TypedDict):
    GlobalReplicationGroupId: str,
    NodeGroupCount: int,
    ApplyImmediately: bool,
    RegionalConfigurations: NotRequired[Sequence[RegionalConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: RegionalConfigurationTypeDef](./type_defs.md#regionalconfigurationtypedef) 
## SnapshotTypeDef

```python
# SnapshotTypeDef definition

class SnapshotTypeDef(TypedDict):
    SnapshotName: NotRequired[str],
    ReplicationGroupId: NotRequired[str],
    ReplicationGroupDescription: NotRequired[str],
    CacheClusterId: NotRequired[str],
    SnapshotStatus: NotRequired[str],
    SnapshotSource: NotRequired[str],
    CacheNodeType: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    NumCacheNodes: NotRequired[int],
    PreferredAvailabilityZone: NotRequired[str],
    PreferredOutpostArn: NotRequired[str],
    CacheClusterCreateTime: NotRequired[datetime],
    PreferredMaintenanceWindow: NotRequired[str],
    TopicArn: NotRequired[str],
    Port: NotRequired[int],
    CacheParameterGroupName: NotRequired[str],
    CacheSubnetGroupName: NotRequired[str],
    VpcId: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    SnapshotRetentionLimit: NotRequired[int],
    SnapshotWindow: NotRequired[str],
    NumNodeGroups: NotRequired[int],
    AutomaticFailover: NotRequired[AutomaticFailoverStatusType],  # (1)
    NodeSnapshots: NotRequired[List[NodeSnapshotTypeDef]],  # (2)
    KmsKeyId: NotRequired[str],
    ARN: NotRequired[str],
    DataTiering: NotRequired[DataTieringStatusType],  # (3)
```

1. See [:material-code-brackets: AutomaticFailoverStatusType](./literals.md#automaticfailoverstatustype) 
2. See [:material-code-braces: NodeSnapshotTypeDef](./type_defs.md#nodesnapshottypedef) 
3. See [:material-code-brackets: DataTieringStatusType](./literals.md#datatieringstatustype) 
## UpdateActionTypeDef

```python
# UpdateActionTypeDef definition

class UpdateActionTypeDef(TypedDict):
    ReplicationGroupId: NotRequired[str],
    CacheClusterId: NotRequired[str],
    ServiceUpdateName: NotRequired[str],
    ServiceUpdateReleaseDate: NotRequired[datetime],
    ServiceUpdateSeverity: NotRequired[ServiceUpdateSeverityType],  # (1)
    ServiceUpdateStatus: NotRequired[ServiceUpdateStatusType],  # (2)
    ServiceUpdateRecommendedApplyByDate: NotRequired[datetime],
    ServiceUpdateType: NotRequired[ServiceUpdateTypeType],  # (3)
    UpdateActionAvailableDate: NotRequired[datetime],
    UpdateActionStatus: NotRequired[UpdateActionStatusType],  # (4)
    NodesUpdated: NotRequired[str],
    UpdateActionStatusModifiedDate: NotRequired[datetime],
    SlaMet: NotRequired[SlaMetType],  # (5)
    NodeGroupUpdateStatus: NotRequired[List[NodeGroupUpdateStatusTypeDef]],  # (6)
    CacheNodeUpdateStatus: NotRequired[List[CacheNodeUpdateStatusTypeDef]],  # (7)
    EstimatedUpdateTime: NotRequired[str],
    Engine: NotRequired[str],
```

1. See [:material-code-brackets: ServiceUpdateSeverityType](./literals.md#serviceupdateseveritytype) 
2. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
3. See [:material-code-brackets: ServiceUpdateTypeType](./literals.md#serviceupdatetypetype) 
4. See [:material-code-brackets: UpdateActionStatusType](./literals.md#updateactionstatustype) 
5. See [:material-code-brackets: SlaMetType](./literals.md#slamettype) 
6. See [:material-code-braces: NodeGroupUpdateStatusTypeDef](./type_defs.md#nodegroupupdatestatustypedef) 
7. See [:material-code-braces: CacheNodeUpdateStatusTypeDef](./type_defs.md#cachenodeupdatestatustypedef) 
## PurchaseReservedCacheNodesOfferingResultTypeDef

```python
# PurchaseReservedCacheNodesOfferingResultTypeDef definition

class PurchaseReservedCacheNodesOfferingResultTypeDef(TypedDict):
    ReservedCacheNode: ReservedCacheNodeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedCacheNodeTypeDef](./type_defs.md#reservedcachenodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReservedCacheNodeMessageTypeDef

```python
# ReservedCacheNodeMessageTypeDef definition

class ReservedCacheNodeMessageTypeDef(TypedDict):
    Marker: str,
    ReservedCacheNodes: List[ReservedCacheNodeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedCacheNodeTypeDef](./type_defs.md#reservedcachenodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReservedCacheNodesOfferingMessageTypeDef

```python
# ReservedCacheNodesOfferingMessageTypeDef definition

class ReservedCacheNodesOfferingMessageTypeDef(TypedDict):
    Marker: str,
    ReservedCacheNodesOfferings: List[ReservedCacheNodesOfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedCacheNodesOfferingTypeDef](./type_defs.md#reservedcachenodesofferingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyServerlessCacheSnapshotResponseTypeDef

```python
# CopyServerlessCacheSnapshotResponseTypeDef definition

class CopyServerlessCacheSnapshotResponseTypeDef(TypedDict):
    ServerlessCacheSnapshot: ServerlessCacheSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerlessCacheSnapshotTypeDef](./type_defs.md#serverlesscachesnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServerlessCacheSnapshotResponseTypeDef

```python
# CreateServerlessCacheSnapshotResponseTypeDef definition

class CreateServerlessCacheSnapshotResponseTypeDef(TypedDict):
    ServerlessCacheSnapshot: ServerlessCacheSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerlessCacheSnapshotTypeDef](./type_defs.md#serverlesscachesnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServerlessCacheSnapshotResponseTypeDef

```python
# DeleteServerlessCacheSnapshotResponseTypeDef definition

class DeleteServerlessCacheSnapshotResponseTypeDef(TypedDict):
    ServerlessCacheSnapshot: ServerlessCacheSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerlessCacheSnapshotTypeDef](./type_defs.md#serverlesscachesnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeServerlessCacheSnapshotsResponseTypeDef

```python
# DescribeServerlessCacheSnapshotsResponseTypeDef definition

class DescribeServerlessCacheSnapshotsResponseTypeDef(TypedDict):
    ServerlessCacheSnapshots: List[ServerlessCacheSnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServerlessCacheSnapshotTypeDef](./type_defs.md#serverlesscachesnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportServerlessCacheSnapshotResponseTypeDef

```python
# ExportServerlessCacheSnapshotResponseTypeDef definition

class ExportServerlessCacheSnapshotResponseTypeDef(TypedDict):
    ServerlessCacheSnapshot: ServerlessCacheSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerlessCacheSnapshotTypeDef](./type_defs.md#serverlesscachesnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CacheSubnetGroupTypeDef

```python
# CacheSubnetGroupTypeDef definition

class CacheSubnetGroupTypeDef(TypedDict):
    CacheSubnetGroupName: NotRequired[str],
    CacheSubnetGroupDescription: NotRequired[str],
    VpcId: NotRequired[str],
    Subnets: NotRequired[List[SubnetTypeDef]],  # (1)
    ARN: NotRequired[str],
    SupportedNetworkTypes: NotRequired[List[NetworkTypeType]],  # (2)
```

1. See [:material-code-braces: SubnetTypeDef](./type_defs.md#subnettypedef) 
2. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
## DescribeUserGroupsResultTypeDef

```python
# DescribeUserGroupsResultTypeDef definition

class DescribeUserGroupsResultTypeDef(TypedDict):
    UserGroups: List[UserGroupTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserGroupTypeDef](./type_defs.md#usergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEngineDefaultParametersResultTypeDef

```python
# DescribeEngineDefaultParametersResultTypeDef definition

class DescribeEngineDefaultParametersResultTypeDef(TypedDict):
    EngineDefaults: EngineDefaultsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EngineDefaultsTypeDef](./type_defs.md#enginedefaultstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServerlessCacheResponseTypeDef

```python
# CreateServerlessCacheResponseTypeDef definition

class CreateServerlessCacheResponseTypeDef(TypedDict):
    ServerlessCache: ServerlessCacheTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerlessCacheTypeDef](./type_defs.md#serverlesscachetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServerlessCacheResponseTypeDef

```python
# DeleteServerlessCacheResponseTypeDef definition

class DeleteServerlessCacheResponseTypeDef(TypedDict):
    ServerlessCache: ServerlessCacheTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerlessCacheTypeDef](./type_defs.md#serverlesscachetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeServerlessCachesResponseTypeDef

```python
# DescribeServerlessCachesResponseTypeDef definition

class DescribeServerlessCachesResponseTypeDef(TypedDict):
    ServerlessCaches: List[ServerlessCacheTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServerlessCacheTypeDef](./type_defs.md#serverlesscachetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyServerlessCacheResponseTypeDef

```python
# ModifyServerlessCacheResponseTypeDef definition

class ModifyServerlessCacheResponseTypeDef(TypedDict):
    ServerlessCache: ServerlessCacheTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerlessCacheTypeDef](./type_defs.md#serverlesscachetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCacheClusterMessageRequestTypeDef

```python
# CreateCacheClusterMessageRequestTypeDef definition

class CreateCacheClusterMessageRequestTypeDef(TypedDict):
    CacheClusterId: str,
    ReplicationGroupId: NotRequired[str],
    AZMode: NotRequired[AZModeType],  # (1)
    PreferredAvailabilityZone: NotRequired[str],
    PreferredAvailabilityZones: NotRequired[Sequence[str]],
    NumCacheNodes: NotRequired[int],
    CacheNodeType: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    CacheParameterGroupName: NotRequired[str],
    CacheSubnetGroupName: NotRequired[str],
    CacheSecurityGroupNames: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    SnapshotArns: NotRequired[Sequence[str]],
    SnapshotName: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    Port: NotRequired[int],
    NotificationTopicArn: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    SnapshotRetentionLimit: NotRequired[int],
    SnapshotWindow: NotRequired[str],
    AuthToken: NotRequired[str],
    OutpostMode: NotRequired[OutpostModeType],  # (3)
    PreferredOutpostArn: NotRequired[str],
    PreferredOutpostArns: NotRequired[Sequence[str]],
    LogDeliveryConfigurations: NotRequired[Sequence[LogDeliveryConfigurationRequestTypeDef]],  # (4)
    TransitEncryptionEnabled: NotRequired[bool],
    NetworkType: NotRequired[NetworkTypeType],  # (5)
    IpDiscovery: NotRequired[IpDiscoveryType],  # (6)
```

1. See [:material-code-brackets: AZModeType](./literals.md#azmodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: OutpostModeType](./literals.md#outpostmodetype) 
4. See [:material-code-braces: LogDeliveryConfigurationRequestTypeDef](./type_defs.md#logdeliveryconfigurationrequesttypedef) 
5. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
6. See [:material-code-brackets: IpDiscoveryType](./literals.md#ipdiscoverytype) 
## CreateReplicationGroupMessageRequestTypeDef

```python
# CreateReplicationGroupMessageRequestTypeDef definition

class CreateReplicationGroupMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: str,
    ReplicationGroupDescription: str,
    GlobalReplicationGroupId: NotRequired[str],
    PrimaryClusterId: NotRequired[str],
    AutomaticFailoverEnabled: NotRequired[bool],
    MultiAZEnabled: NotRequired[bool],
    NumCacheClusters: NotRequired[int],
    PreferredCacheClusterAZs: NotRequired[Sequence[str]],
    NumNodeGroups: NotRequired[int],
    ReplicasPerNodeGroup: NotRequired[int],
    NodeGroupConfiguration: NotRequired[Sequence[NodeGroupConfigurationUnionTypeDef]],  # (1)
    CacheNodeType: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    CacheParameterGroupName: NotRequired[str],
    CacheSubnetGroupName: NotRequired[str],
    CacheSecurityGroupNames: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    SnapshotArns: NotRequired[Sequence[str]],
    SnapshotName: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    Port: NotRequired[int],
    NotificationTopicArn: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    SnapshotRetentionLimit: NotRequired[int],
    SnapshotWindow: NotRequired[str],
    AuthToken: NotRequired[str],
    TransitEncryptionEnabled: NotRequired[bool],
    AtRestEncryptionEnabled: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    UserGroupIds: NotRequired[Sequence[str]],
    LogDeliveryConfigurations: NotRequired[Sequence[LogDeliveryConfigurationRequestTypeDef]],  # (3)
    DataTieringEnabled: NotRequired[bool],
    NetworkType: NotRequired[NetworkTypeType],  # (4)
    IpDiscovery: NotRequired[IpDiscoveryType],  # (5)
    TransitEncryptionMode: NotRequired[TransitEncryptionModeType],  # (6)
    ClusterMode: NotRequired[ClusterModeType],  # (7)
    ServerlessCacheSnapshotName: NotRequired[str],
```

1. See [:material-code-braces: NodeGroupConfigurationTypeDef](./type_defs.md#nodegroupconfigurationtypedef) [:material-code-braces: NodeGroupConfigurationOutputTypeDef](./type_defs.md#nodegroupconfigurationoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: LogDeliveryConfigurationRequestTypeDef](./type_defs.md#logdeliveryconfigurationrequesttypedef) 
4. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
5. See [:material-code-brackets: IpDiscoveryType](./literals.md#ipdiscoverytype) 
6. See [:material-code-brackets: TransitEncryptionModeType](./literals.md#transitencryptionmodetype) 
7. See [:material-code-brackets: ClusterModeType](./literals.md#clustermodetype) 
## ModifyCacheClusterMessageRequestTypeDef

```python
# ModifyCacheClusterMessageRequestTypeDef definition

class ModifyCacheClusterMessageRequestTypeDef(TypedDict):
    CacheClusterId: str,
    NumCacheNodes: NotRequired[int],
    CacheNodeIdsToRemove: NotRequired[Sequence[str]],
    AZMode: NotRequired[AZModeType],  # (1)
    NewAvailabilityZones: NotRequired[Sequence[str]],
    CacheSecurityGroupNames: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
    PreferredMaintenanceWindow: NotRequired[str],
    NotificationTopicArn: NotRequired[str],
    CacheParameterGroupName: NotRequired[str],
    NotificationTopicStatus: NotRequired[str],
    ApplyImmediately: NotRequired[bool],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    SnapshotRetentionLimit: NotRequired[int],
    SnapshotWindow: NotRequired[str],
    CacheNodeType: NotRequired[str],
    AuthToken: NotRequired[str],
    AuthTokenUpdateStrategy: NotRequired[AuthTokenUpdateStrategyTypeType],  # (2)
    LogDeliveryConfigurations: NotRequired[Sequence[LogDeliveryConfigurationRequestTypeDef]],  # (3)
    IpDiscovery: NotRequired[IpDiscoveryType],  # (4)
```

1. See [:material-code-brackets: AZModeType](./literals.md#azmodetype) 
2. See [:material-code-brackets: AuthTokenUpdateStrategyTypeType](./literals.md#authtokenupdatestrategytypetype) 
3. See [:material-code-braces: LogDeliveryConfigurationRequestTypeDef](./type_defs.md#logdeliveryconfigurationrequesttypedef) 
4. See [:material-code-brackets: IpDiscoveryType](./literals.md#ipdiscoverytype) 
## ModifyReplicationGroupMessageRequestTypeDef

```python
# ModifyReplicationGroupMessageRequestTypeDef definition

class ModifyReplicationGroupMessageRequestTypeDef(TypedDict):
    ReplicationGroupId: str,
    ReplicationGroupDescription: NotRequired[str],
    PrimaryClusterId: NotRequired[str],
    SnapshottingClusterId: NotRequired[str],
    AutomaticFailoverEnabled: NotRequired[bool],
    MultiAZEnabled: NotRequired[bool],
    NodeGroupId: NotRequired[str],
    CacheSecurityGroupNames: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
    PreferredMaintenanceWindow: NotRequired[str],
    NotificationTopicArn: NotRequired[str],
    CacheParameterGroupName: NotRequired[str],
    NotificationTopicStatus: NotRequired[str],
    ApplyImmediately: NotRequired[bool],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    SnapshotRetentionLimit: NotRequired[int],
    SnapshotWindow: NotRequired[str],
    CacheNodeType: NotRequired[str],
    AuthToken: NotRequired[str],
    AuthTokenUpdateStrategy: NotRequired[AuthTokenUpdateStrategyTypeType],  # (1)
    UserGroupIdsToAdd: NotRequired[Sequence[str]],
    UserGroupIdsToRemove: NotRequired[Sequence[str]],
    RemoveUserGroups: NotRequired[bool],
    LogDeliveryConfigurations: NotRequired[Sequence[LogDeliveryConfigurationRequestTypeDef]],  # (2)
    IpDiscovery: NotRequired[IpDiscoveryType],  # (3)
    TransitEncryptionEnabled: NotRequired[bool],
    TransitEncryptionMode: NotRequired[TransitEncryptionModeType],  # (4)
    ClusterMode: NotRequired[ClusterModeType],  # (5)
```

1. See [:material-code-brackets: AuthTokenUpdateStrategyTypeType](./literals.md#authtokenupdatestrategytypetype) 
2. See [:material-code-braces: LogDeliveryConfigurationRequestTypeDef](./type_defs.md#logdeliveryconfigurationrequesttypedef) 
3. See [:material-code-brackets: IpDiscoveryType](./literals.md#ipdiscoverytype) 
4. See [:material-code-brackets: TransitEncryptionModeType](./literals.md#transitencryptionmodetype) 
5. See [:material-code-brackets: ClusterModeType](./literals.md#clustermodetype) 
## PendingModifiedValuesTypeDef

```python
# PendingModifiedValuesTypeDef definition

class PendingModifiedValuesTypeDef(TypedDict):
    NumCacheNodes: NotRequired[int],
    CacheNodeIdsToRemove: NotRequired[List[str]],
    EngineVersion: NotRequired[str],
    CacheNodeType: NotRequired[str],
    AuthTokenStatus: NotRequired[AuthTokenUpdateStatusType],  # (1)
    LogDeliveryConfigurations: NotRequired[List[PendingLogDeliveryConfigurationTypeDef]],  # (2)
    TransitEncryptionEnabled: NotRequired[bool],
    TransitEncryptionMode: NotRequired[TransitEncryptionModeType],  # (3)
```

1. See [:material-code-brackets: AuthTokenUpdateStatusType](./literals.md#authtokenupdatestatustype) 
2. See [:material-code-braces: PendingLogDeliveryConfigurationTypeDef](./type_defs.md#pendinglogdeliveryconfigurationtypedef) 
3. See [:material-code-brackets: TransitEncryptionModeType](./literals.md#transitencryptionmodetype) 
## ReplicationGroupPendingModifiedValuesTypeDef

```python
# ReplicationGroupPendingModifiedValuesTypeDef definition

class ReplicationGroupPendingModifiedValuesTypeDef(TypedDict):
    PrimaryClusterId: NotRequired[str],
    AutomaticFailoverStatus: NotRequired[PendingAutomaticFailoverStatusType],  # (1)
    Resharding: NotRequired[ReshardingStatusTypeDef],  # (2)
    AuthTokenStatus: NotRequired[AuthTokenUpdateStatusType],  # (3)
    UserGroups: NotRequired[UserGroupsUpdateStatusTypeDef],  # (4)
    LogDeliveryConfigurations: NotRequired[List[PendingLogDeliveryConfigurationTypeDef]],  # (5)
    TransitEncryptionEnabled: NotRequired[bool],
    TransitEncryptionMode: NotRequired[TransitEncryptionModeType],  # (6)
    ClusterMode: NotRequired[ClusterModeType],  # (7)
```

1. See [:material-code-brackets: PendingAutomaticFailoverStatusType](./literals.md#pendingautomaticfailoverstatustype) 
2. See [:material-code-braces: ReshardingStatusTypeDef](./type_defs.md#reshardingstatustypedef) 
3. See [:material-code-brackets: AuthTokenUpdateStatusType](./literals.md#authtokenupdatestatustype) 
4. See [:material-code-braces: UserGroupsUpdateStatusTypeDef](./type_defs.md#usergroupsupdatestatustypedef) 
5. See [:material-code-braces: PendingLogDeliveryConfigurationTypeDef](./type_defs.md#pendinglogdeliveryconfigurationtypedef) 
6. See [:material-code-brackets: TransitEncryptionModeType](./literals.md#transitencryptionmodetype) 
7. See [:material-code-brackets: ClusterModeType](./literals.md#clustermodetype) 
## CopySnapshotResultTypeDef

```python
# CopySnapshotResultTypeDef definition

class CopySnapshotResultTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSnapshotResultTypeDef

```python
# CreateSnapshotResultTypeDef definition

class CreateSnapshotResultTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSnapshotResultTypeDef

```python
# DeleteSnapshotResultTypeDef definition

class DeleteSnapshotResultTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSnapshotsListMessageTypeDef

```python
# DescribeSnapshotsListMessageTypeDef definition

class DescribeSnapshotsListMessageTypeDef(TypedDict):
    Marker: str,
    Snapshots: List[SnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateActionsMessageTypeDef

```python
# UpdateActionsMessageTypeDef definition

class UpdateActionsMessageTypeDef(TypedDict):
    Marker: str,
    UpdateActions: List[UpdateActionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateActionTypeDef](./type_defs.md#updateactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CacheSubnetGroupMessageTypeDef

```python
# CacheSubnetGroupMessageTypeDef definition

class CacheSubnetGroupMessageTypeDef(TypedDict):
    Marker: str,
    CacheSubnetGroups: List[CacheSubnetGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheSubnetGroupTypeDef](./type_defs.md#cachesubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCacheSubnetGroupResultTypeDef

```python
# CreateCacheSubnetGroupResultTypeDef definition

class CreateCacheSubnetGroupResultTypeDef(TypedDict):
    CacheSubnetGroup: CacheSubnetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheSubnetGroupTypeDef](./type_defs.md#cachesubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyCacheSubnetGroupResultTypeDef

```python
# ModifyCacheSubnetGroupResultTypeDef definition

class ModifyCacheSubnetGroupResultTypeDef(TypedDict):
    CacheSubnetGroup: CacheSubnetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheSubnetGroupTypeDef](./type_defs.md#cachesubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CacheClusterTypeDef

```python
# CacheClusterTypeDef definition

class CacheClusterTypeDef(TypedDict):
    CacheClusterId: NotRequired[str],
    ConfigurationEndpoint: NotRequired[EndpointTypeDef],  # (1)
    ClientDownloadLandingPage: NotRequired[str],
    CacheNodeType: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    CacheClusterStatus: NotRequired[str],
    NumCacheNodes: NotRequired[int],
    PreferredAvailabilityZone: NotRequired[str],
    PreferredOutpostArn: NotRequired[str],
    CacheClusterCreateTime: NotRequired[datetime],
    PreferredMaintenanceWindow: NotRequired[str],
    PendingModifiedValues: NotRequired[PendingModifiedValuesTypeDef],  # (2)
    NotificationConfiguration: NotRequired[NotificationConfigurationTypeDef],  # (3)
    CacheSecurityGroups: NotRequired[List[CacheSecurityGroupMembershipTypeDef]],  # (4)
    CacheParameterGroup: NotRequired[CacheParameterGroupStatusTypeDef],  # (5)
    CacheSubnetGroupName: NotRequired[str],
    CacheNodes: NotRequired[List[CacheNodeTypeDef]],  # (6)
    AutoMinorVersionUpgrade: NotRequired[bool],
    SecurityGroups: NotRequired[List[SecurityGroupMembershipTypeDef]],  # (7)
    ReplicationGroupId: NotRequired[str],
    SnapshotRetentionLimit: NotRequired[int],
    SnapshotWindow: NotRequired[str],
    AuthTokenEnabled: NotRequired[bool],
    AuthTokenLastModifiedDate: NotRequired[datetime],
    TransitEncryptionEnabled: NotRequired[bool],
    AtRestEncryptionEnabled: NotRequired[bool],
    ARN: NotRequired[str],
    ReplicationGroupLogDeliveryEnabled: NotRequired[bool],
    LogDeliveryConfigurations: NotRequired[List[LogDeliveryConfigurationTypeDef]],  # (8)
    NetworkType: NotRequired[NetworkTypeType],  # (9)
    IpDiscovery: NotRequired[IpDiscoveryType],  # (10)
    TransitEncryptionMode: NotRequired[TransitEncryptionModeType],  # (11)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: PendingModifiedValuesTypeDef](./type_defs.md#pendingmodifiedvaluestypedef) 
3. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
4. See [:material-code-braces: CacheSecurityGroupMembershipTypeDef](./type_defs.md#cachesecuritygroupmembershiptypedef) 
5. See [:material-code-braces: CacheParameterGroupStatusTypeDef](./type_defs.md#cacheparametergroupstatustypedef) 
6. See [:material-code-braces: CacheNodeTypeDef](./type_defs.md#cachenodetypedef) 
7. See [:material-code-braces: SecurityGroupMembershipTypeDef](./type_defs.md#securitygroupmembershiptypedef) 
8. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
9. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
10. See [:material-code-brackets: IpDiscoveryType](./literals.md#ipdiscoverytype) 
11. See [:material-code-brackets: TransitEncryptionModeType](./literals.md#transitencryptionmodetype) 
## ReplicationGroupTypeDef

```python
# ReplicationGroupTypeDef definition

class ReplicationGroupTypeDef(TypedDict):
    ReplicationGroupId: NotRequired[str],
    Description: NotRequired[str],
    GlobalReplicationGroupInfo: NotRequired[GlobalReplicationGroupInfoTypeDef],  # (1)
    Status: NotRequired[str],
    PendingModifiedValues: NotRequired[ReplicationGroupPendingModifiedValuesTypeDef],  # (2)
    MemberClusters: NotRequired[List[str]],
    NodeGroups: NotRequired[List[NodeGroupTypeDef]],  # (3)
    SnapshottingClusterId: NotRequired[str],
    AutomaticFailover: NotRequired[AutomaticFailoverStatusType],  # (4)
    MultiAZ: NotRequired[MultiAZStatusType],  # (5)
    ConfigurationEndpoint: NotRequired[EndpointTypeDef],  # (6)
    SnapshotRetentionLimit: NotRequired[int],
    SnapshotWindow: NotRequired[str],
    ClusterEnabled: NotRequired[bool],
    CacheNodeType: NotRequired[str],
    AuthTokenEnabled: NotRequired[bool],
    AuthTokenLastModifiedDate: NotRequired[datetime],
    TransitEncryptionEnabled: NotRequired[bool],
    AtRestEncryptionEnabled: NotRequired[bool],
    MemberClustersOutpostArns: NotRequired[List[str]],
    KmsKeyId: NotRequired[str],
    ARN: NotRequired[str],
    UserGroupIds: NotRequired[List[str]],
    LogDeliveryConfigurations: NotRequired[List[LogDeliveryConfigurationTypeDef]],  # (7)
    ReplicationGroupCreateTime: NotRequired[datetime],
    DataTiering: NotRequired[DataTieringStatusType],  # (8)
    AutoMinorVersionUpgrade: NotRequired[bool],
    NetworkType: NotRequired[NetworkTypeType],  # (9)
    IpDiscovery: NotRequired[IpDiscoveryType],  # (10)
    TransitEncryptionMode: NotRequired[TransitEncryptionModeType],  # (11)
    ClusterMode: NotRequired[ClusterModeType],  # (12)
    Engine: NotRequired[str],
```

1. See [:material-code-braces: GlobalReplicationGroupInfoTypeDef](./type_defs.md#globalreplicationgroupinfotypedef) 
2. See [:material-code-braces: ReplicationGroupPendingModifiedValuesTypeDef](./type_defs.md#replicationgrouppendingmodifiedvaluestypedef) 
3. See [:material-code-braces: NodeGroupTypeDef](./type_defs.md#nodegrouptypedef) 
4. See [:material-code-brackets: AutomaticFailoverStatusType](./literals.md#automaticfailoverstatustype) 
5. See [:material-code-brackets: MultiAZStatusType](./literals.md#multiazstatustype) 
6. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
7. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
8. See [:material-code-brackets: DataTieringStatusType](./literals.md#datatieringstatustype) 
9. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
10. See [:material-code-brackets: IpDiscoveryType](./literals.md#ipdiscoverytype) 
11. See [:material-code-brackets: TransitEncryptionModeType](./literals.md#transitencryptionmodetype) 
12. See [:material-code-brackets: ClusterModeType](./literals.md#clustermodetype) 
## CacheClusterMessageTypeDef

```python
# CacheClusterMessageTypeDef definition

class CacheClusterMessageTypeDef(TypedDict):
    Marker: str,
    CacheClusters: List[CacheClusterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheClusterTypeDef](./type_defs.md#cacheclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCacheClusterResultTypeDef

```python
# CreateCacheClusterResultTypeDef definition

class CreateCacheClusterResultTypeDef(TypedDict):
    CacheCluster: CacheClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheClusterTypeDef](./type_defs.md#cacheclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCacheClusterResultTypeDef

```python
# DeleteCacheClusterResultTypeDef definition

class DeleteCacheClusterResultTypeDef(TypedDict):
    CacheCluster: CacheClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheClusterTypeDef](./type_defs.md#cacheclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyCacheClusterResultTypeDef

```python
# ModifyCacheClusterResultTypeDef definition

class ModifyCacheClusterResultTypeDef(TypedDict):
    CacheCluster: CacheClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheClusterTypeDef](./type_defs.md#cacheclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RebootCacheClusterResultTypeDef

```python
# RebootCacheClusterResultTypeDef definition

class RebootCacheClusterResultTypeDef(TypedDict):
    CacheCluster: CacheClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CacheClusterTypeDef](./type_defs.md#cacheclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CompleteMigrationResponseTypeDef

```python
# CompleteMigrationResponseTypeDef definition

class CompleteMigrationResponseTypeDef(TypedDict):
    ReplicationGroup: ReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationGroupTypeDef](./type_defs.md#replicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReplicationGroupResultTypeDef

```python
# CreateReplicationGroupResultTypeDef definition

class CreateReplicationGroupResultTypeDef(TypedDict):
    ReplicationGroup: ReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationGroupTypeDef](./type_defs.md#replicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DecreaseReplicaCountResultTypeDef

```python
# DecreaseReplicaCountResultTypeDef definition

class DecreaseReplicaCountResultTypeDef(TypedDict):
    ReplicationGroup: ReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationGroupTypeDef](./type_defs.md#replicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteReplicationGroupResultTypeDef

```python
# DeleteReplicationGroupResultTypeDef definition

class DeleteReplicationGroupResultTypeDef(TypedDict):
    ReplicationGroup: ReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationGroupTypeDef](./type_defs.md#replicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IncreaseReplicaCountResultTypeDef

```python
# IncreaseReplicaCountResultTypeDef definition

class IncreaseReplicaCountResultTypeDef(TypedDict):
    ReplicationGroup: ReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationGroupTypeDef](./type_defs.md#replicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyReplicationGroupResultTypeDef

```python
# ModifyReplicationGroupResultTypeDef definition

class ModifyReplicationGroupResultTypeDef(TypedDict):
    ReplicationGroup: ReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationGroupTypeDef](./type_defs.md#replicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyReplicationGroupShardConfigurationResultTypeDef

```python
# ModifyReplicationGroupShardConfigurationResultTypeDef definition

class ModifyReplicationGroupShardConfigurationResultTypeDef(TypedDict):
    ReplicationGroup: ReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationGroupTypeDef](./type_defs.md#replicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicationGroupMessageTypeDef

```python
# ReplicationGroupMessageTypeDef definition

class ReplicationGroupMessageTypeDef(TypedDict):
    Marker: str,
    ReplicationGroups: List[ReplicationGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationGroupTypeDef](./type_defs.md#replicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMigrationResponseTypeDef

```python
# StartMigrationResponseTypeDef definition

class StartMigrationResponseTypeDef(TypedDict):
    ReplicationGroup: ReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationGroupTypeDef](./type_defs.md#replicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestFailoverResultTypeDef

```python
# TestFailoverResultTypeDef definition

class TestFailoverResultTypeDef(TypedDict):
    ReplicationGroup: ReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationGroupTypeDef](./type_defs.md#replicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestMigrationResponseTypeDef

```python
# TestMigrationResponseTypeDef definition

class TestMigrationResponseTypeDef(TypedDict):
    ReplicationGroup: ReplicationGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationGroupTypeDef](./type_defs.md#replicationgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
