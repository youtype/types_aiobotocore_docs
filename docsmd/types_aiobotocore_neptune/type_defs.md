# Type definitions

> [Index](../README.md) > [Neptune](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Neptune](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
    type annotations stubs module [types-aiobotocore-neptune](https://pypi.org/project/types-aiobotocore-neptune/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AddRoleToDBClusterMessageRequestTypeDef

```python
# AddRoleToDBClusterMessageRequestTypeDef definition

class AddRoleToDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    RoleArn: str,
    FeatureName: NotRequired[str],
```

## AddSourceIdentifierToSubscriptionMessageRequestTypeDef

```python
# AddSourceIdentifierToSubscriptionMessageRequestTypeDef definition

class AddSourceIdentifierToSubscriptionMessageRequestTypeDef(TypedDict):
    SubscriptionName: str,
    SourceIdentifier: str,
```

## EventSubscriptionTypeDef

```python
# EventSubscriptionTypeDef definition

class EventSubscriptionTypeDef(TypedDict):
    CustomerAwsId: NotRequired[str],
    CustSubscriptionId: NotRequired[str],
    SnsTopicArn: NotRequired[str],
    Status: NotRequired[str],
    SubscriptionCreationTime: NotRequired[str],
    SourceType: NotRequired[str],
    SourceIdsList: NotRequired[List[str]],
    EventCategoriesList: NotRequired[List[str]],
    Enabled: NotRequired[bool],
    EventSubscriptionArn: NotRequired[str],
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

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ApplyPendingMaintenanceActionMessageRequestTypeDef

```python
# ApplyPendingMaintenanceActionMessageRequestTypeDef definition

class ApplyPendingMaintenanceActionMessageRequestTypeDef(TypedDict):
    ResourceIdentifier: str,
    ApplyAction: str,
    OptInType: str,
```

## AvailabilityZoneTypeDef

```python
# AvailabilityZoneTypeDef definition

class AvailabilityZoneTypeDef(TypedDict):
    Name: NotRequired[str],
```

## CharacterSetTypeDef

```python
# CharacterSetTypeDef definition

class CharacterSetTypeDef(TypedDict):
    CharacterSetName: NotRequired[str],
    CharacterSetDescription: NotRequired[str],
```

## CloudwatchLogsExportConfigurationTypeDef

```python
# CloudwatchLogsExportConfigurationTypeDef definition

class CloudwatchLogsExportConfigurationTypeDef(TypedDict):
    EnableLogTypes: NotRequired[Sequence[str]],
    DisableLogTypes: NotRequired[Sequence[str]],
```

## PendingCloudwatchLogsExportsTypeDef

```python
# PendingCloudwatchLogsExportsTypeDef definition

class PendingCloudwatchLogsExportsTypeDef(TypedDict):
    LogTypesToEnable: NotRequired[List[str]],
    LogTypesToDisable: NotRequired[List[str]],
```

## DBClusterParameterGroupTypeDef

```python
# DBClusterParameterGroupTypeDef definition

class DBClusterParameterGroupTypeDef(TypedDict):
    DBClusterParameterGroupName: NotRequired[str],
    DBParameterGroupFamily: NotRequired[str],
    Description: NotRequired[str],
    DBClusterParameterGroupArn: NotRequired[str],
```

## DBClusterSnapshotTypeDef

```python
# DBClusterSnapshotTypeDef definition

class DBClusterSnapshotTypeDef(TypedDict):
    AvailabilityZones: NotRequired[List[str]],
    DBClusterSnapshotIdentifier: NotRequired[str],
    DBClusterIdentifier: NotRequired[str],
    SnapshotCreateTime: NotRequired[datetime],
    Engine: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    Status: NotRequired[str],
    Port: NotRequired[int],
    VpcId: NotRequired[str],
    ClusterCreateTime: NotRequired[datetime],
    MasterUsername: NotRequired[str],
    EngineVersion: NotRequired[str],
    LicenseModel: NotRequired[str],
    SnapshotType: NotRequired[str],
    PercentProgress: NotRequired[int],
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    DBClusterSnapshotArn: NotRequired[str],
    SourceDBClusterSnapshotArn: NotRequired[str],
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    StorageType: NotRequired[str],
```

## DBParameterGroupTypeDef

```python
# DBParameterGroupTypeDef definition

class DBParameterGroupTypeDef(TypedDict):
    DBParameterGroupName: NotRequired[str],
    DBParameterGroupFamily: NotRequired[str],
    Description: NotRequired[str],
    DBParameterGroupArn: NotRequired[str],
```

## ServerlessV2ScalingConfigurationTypeDef

```python
# ServerlessV2ScalingConfigurationTypeDef definition

class ServerlessV2ScalingConfigurationTypeDef(TypedDict):
    MinCapacity: NotRequired[float],
    MaxCapacity: NotRequired[float],
```

## CreateGlobalClusterMessageRequestTypeDef

```python
# CreateGlobalClusterMessageRequestTypeDef definition

class CreateGlobalClusterMessageRequestTypeDef(TypedDict):
    GlobalClusterIdentifier: str,
    SourceDBClusterIdentifier: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    StorageEncrypted: NotRequired[bool],
```

## DBClusterEndpointTypeDef

```python
# DBClusterEndpointTypeDef definition

class DBClusterEndpointTypeDef(TypedDict):
    DBClusterEndpointIdentifier: NotRequired[str],
    DBClusterIdentifier: NotRequired[str],
    DBClusterEndpointResourceIdentifier: NotRequired[str],
    Endpoint: NotRequired[str],
    Status: NotRequired[str],
    EndpointType: NotRequired[str],
    CustomEndpointType: NotRequired[str],
    StaticMembers: NotRequired[List[str]],
    ExcludedMembers: NotRequired[List[str]],
    DBClusterEndpointArn: NotRequired[str],
```

## DBClusterMemberTypeDef

```python
# DBClusterMemberTypeDef definition

class DBClusterMemberTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    IsClusterWriter: NotRequired[bool],
    DBClusterParameterGroupStatus: NotRequired[str],
    PromotionTier: NotRequired[int],
```

## DBClusterOptionGroupStatusTypeDef

```python
# DBClusterOptionGroupStatusTypeDef definition

class DBClusterOptionGroupStatusTypeDef(TypedDict):
    DBClusterOptionGroupName: NotRequired[str],
    Status: NotRequired[str],
```

## ParameterTypeDef

```python
# ParameterTypeDef definition

class ParameterTypeDef(TypedDict):
    ParameterName: NotRequired[str],
    ParameterValue: NotRequired[str],
    Description: NotRequired[str],
    Source: NotRequired[str],
    ApplyType: NotRequired[str],
    DataType: NotRequired[str],
    AllowedValues: NotRequired[str],
    IsModifiable: NotRequired[bool],
    MinimumEngineVersion: NotRequired[str],
    ApplyMethod: NotRequired[ApplyMethodType],  # (1)
```

1. See [:material-code-brackets: ApplyMethodType](./literals.md#applymethodtype) 
## DBClusterRoleTypeDef

```python
# DBClusterRoleTypeDef definition

class DBClusterRoleTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    Status: NotRequired[str],
    FeatureName: NotRequired[str],
```

## DBClusterSnapshotAttributeTypeDef

```python
# DBClusterSnapshotAttributeTypeDef definition

class DBClusterSnapshotAttributeTypeDef(TypedDict):
    AttributeName: NotRequired[str],
    AttributeValues: NotRequired[List[str]],
```

## ServerlessV2ScalingConfigurationInfoTypeDef

```python
# ServerlessV2ScalingConfigurationInfoTypeDef definition

class ServerlessV2ScalingConfigurationInfoTypeDef(TypedDict):
    MinCapacity: NotRequired[float],
    MaxCapacity: NotRequired[float],
```

## VpcSecurityGroupMembershipTypeDef

```python
# VpcSecurityGroupMembershipTypeDef definition

class VpcSecurityGroupMembershipTypeDef(TypedDict):
    VpcSecurityGroupId: NotRequired[str],
    Status: NotRequired[str],
```

## TimezoneTypeDef

```python
# TimezoneTypeDef definition

class TimezoneTypeDef(TypedDict):
    TimezoneName: NotRequired[str],
```

## UpgradeTargetTypeDef

```python
# UpgradeTargetTypeDef definition

class UpgradeTargetTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    Description: NotRequired[str],
    AutoUpgrade: NotRequired[bool],
    IsMajorVersionUpgrade: NotRequired[bool],
    SupportsGlobalDatabases: NotRequired[bool],
```

## DBInstanceStatusInfoTypeDef

```python
# DBInstanceStatusInfoTypeDef definition

class DBInstanceStatusInfoTypeDef(TypedDict):
    StatusType: NotRequired[str],
    Normal: NotRequired[bool],
    Status: NotRequired[str],
    Message: NotRequired[str],
```

## DBParameterGroupStatusTypeDef

```python
# DBParameterGroupStatusTypeDef definition

class DBParameterGroupStatusTypeDef(TypedDict):
    DBParameterGroupName: NotRequired[str],
    ParameterApplyStatus: NotRequired[str],
```

## DBSecurityGroupMembershipTypeDef

```python
# DBSecurityGroupMembershipTypeDef definition

class DBSecurityGroupMembershipTypeDef(TypedDict):
    DBSecurityGroupName: NotRequired[str],
    Status: NotRequired[str],
```

## DomainMembershipTypeDef

```python
# DomainMembershipTypeDef definition

class DomainMembershipTypeDef(TypedDict):
    Domain: NotRequired[str],
    Status: NotRequired[str],
    FQDN: NotRequired[str],
    IAMRoleName: NotRequired[str],
```

## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Address: NotRequired[str],
    Port: NotRequired[int],
    HostedZoneId: NotRequired[str],
```

## OptionGroupMembershipTypeDef

```python
# OptionGroupMembershipTypeDef definition

class OptionGroupMembershipTypeDef(TypedDict):
    OptionGroupName: NotRequired[str],
    Status: NotRequired[str],
```

## DeleteDBClusterEndpointMessageRequestTypeDef

```python
# DeleteDBClusterEndpointMessageRequestTypeDef definition

class DeleteDBClusterEndpointMessageRequestTypeDef(TypedDict):
    DBClusterEndpointIdentifier: str,
```

## DeleteDBClusterMessageRequestTypeDef

```python
# DeleteDBClusterMessageRequestTypeDef definition

class DeleteDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    SkipFinalSnapshot: NotRequired[bool],
    FinalDBSnapshotIdentifier: NotRequired[str],
```

## DeleteDBClusterParameterGroupMessageRequestTypeDef

```python
# DeleteDBClusterParameterGroupMessageRequestTypeDef definition

class DeleteDBClusterParameterGroupMessageRequestTypeDef(TypedDict):
    DBClusterParameterGroupName: str,
```

## DeleteDBClusterSnapshotMessageRequestTypeDef

```python
# DeleteDBClusterSnapshotMessageRequestTypeDef definition

class DeleteDBClusterSnapshotMessageRequestTypeDef(TypedDict):
    DBClusterSnapshotIdentifier: str,
```

## DeleteDBInstanceMessageRequestTypeDef

```python
# DeleteDBInstanceMessageRequestTypeDef definition

class DeleteDBInstanceMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    SkipFinalSnapshot: NotRequired[bool],
    FinalDBSnapshotIdentifier: NotRequired[str],
```

## DeleteDBParameterGroupMessageRequestTypeDef

```python
# DeleteDBParameterGroupMessageRequestTypeDef definition

class DeleteDBParameterGroupMessageRequestTypeDef(TypedDict):
    DBParameterGroupName: str,
```

## DeleteDBSubnetGroupMessageRequestTypeDef

```python
# DeleteDBSubnetGroupMessageRequestTypeDef definition

class DeleteDBSubnetGroupMessageRequestTypeDef(TypedDict):
    DBSubnetGroupName: str,
```

## DeleteEventSubscriptionMessageRequestTypeDef

```python
# DeleteEventSubscriptionMessageRequestTypeDef definition

class DeleteEventSubscriptionMessageRequestTypeDef(TypedDict):
    SubscriptionName: str,
```

## DeleteGlobalClusterMessageRequestTypeDef

```python
# DeleteGlobalClusterMessageRequestTypeDef definition

class DeleteGlobalClusterMessageRequestTypeDef(TypedDict):
    GlobalClusterIdentifier: str,
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: str,
    Values: Sequence[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeDBClusterSnapshotAttributesMessageRequestTypeDef

```python
# DescribeDBClusterSnapshotAttributesMessageRequestTypeDef definition

class DescribeDBClusterSnapshotAttributesMessageRequestTypeDef(TypedDict):
    DBClusterSnapshotIdentifier: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeGlobalClustersMessageRequestTypeDef

```python
# DescribeGlobalClustersMessageRequestTypeDef definition

class DescribeGlobalClustersMessageRequestTypeDef(TypedDict):
    GlobalClusterIdentifier: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeValidDBInstanceModificationsMessageRequestTypeDef

```python
# DescribeValidDBInstanceModificationsMessageRequestTypeDef definition

class DescribeValidDBInstanceModificationsMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
```

## DoubleRangeTypeDef

```python
# DoubleRangeTypeDef definition

class DoubleRangeTypeDef(TypedDict):
    From: NotRequired[float],
    To: NotRequired[float],
```

## EventCategoriesMapTypeDef

```python
# EventCategoriesMapTypeDef definition

class EventCategoriesMapTypeDef(TypedDict):
    SourceType: NotRequired[str],
    EventCategories: NotRequired[List[str]],
```

## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    SourceIdentifier: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    Message: NotRequired[str],
    EventCategories: NotRequired[List[str]],
    Date: NotRequired[datetime],
    SourceArn: NotRequired[str],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## FailoverDBClusterMessageRequestTypeDef

```python
# FailoverDBClusterMessageRequestTypeDef definition

class FailoverDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    TargetDBInstanceIdentifier: NotRequired[str],
```

## FailoverGlobalClusterMessageRequestTypeDef

```python
# FailoverGlobalClusterMessageRequestTypeDef definition

class FailoverGlobalClusterMessageRequestTypeDef(TypedDict):
    GlobalClusterIdentifier: str,
    TargetDbClusterIdentifier: str,
```

## GlobalClusterMemberTypeDef

```python
# GlobalClusterMemberTypeDef definition

class GlobalClusterMemberTypeDef(TypedDict):
    DBClusterArn: NotRequired[str],
    Readers: NotRequired[List[str]],
    IsWriter: NotRequired[bool],
```

## ModifyDBClusterEndpointMessageRequestTypeDef

```python
# ModifyDBClusterEndpointMessageRequestTypeDef definition

class ModifyDBClusterEndpointMessageRequestTypeDef(TypedDict):
    DBClusterEndpointIdentifier: str,
    EndpointType: NotRequired[str],
    StaticMembers: NotRequired[Sequence[str]],
    ExcludedMembers: NotRequired[Sequence[str]],
```

## ModifyDBClusterSnapshotAttributeMessageRequestTypeDef

```python
# ModifyDBClusterSnapshotAttributeMessageRequestTypeDef definition

class ModifyDBClusterSnapshotAttributeMessageRequestTypeDef(TypedDict):
    DBClusterSnapshotIdentifier: str,
    AttributeName: str,
    ValuesToAdd: NotRequired[Sequence[str]],
    ValuesToRemove: NotRequired[Sequence[str]],
```

## ModifyDBSubnetGroupMessageRequestTypeDef

```python
# ModifyDBSubnetGroupMessageRequestTypeDef definition

class ModifyDBSubnetGroupMessageRequestTypeDef(TypedDict):
    DBSubnetGroupName: str,
    SubnetIds: Sequence[str],
    DBSubnetGroupDescription: NotRequired[str],
```

## ModifyEventSubscriptionMessageRequestTypeDef

```python
# ModifyEventSubscriptionMessageRequestTypeDef definition

class ModifyEventSubscriptionMessageRequestTypeDef(TypedDict):
    SubscriptionName: str,
    SnsTopicArn: NotRequired[str],
    SourceType: NotRequired[str],
    EventCategories: NotRequired[Sequence[str]],
    Enabled: NotRequired[bool],
```

## ModifyGlobalClusterMessageRequestTypeDef

```python
# ModifyGlobalClusterMessageRequestTypeDef definition

class ModifyGlobalClusterMessageRequestTypeDef(TypedDict):
    GlobalClusterIdentifier: str,
    NewGlobalClusterIdentifier: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    EngineVersion: NotRequired[str],
    AllowMajorVersionUpgrade: NotRequired[bool],
```

## PendingMaintenanceActionTypeDef

```python
# PendingMaintenanceActionTypeDef definition

class PendingMaintenanceActionTypeDef(TypedDict):
    Action: NotRequired[str],
    AutoAppliedAfterDate: NotRequired[datetime],
    ForcedApplyDate: NotRequired[datetime],
    OptInStatus: NotRequired[str],
    CurrentApplyDate: NotRequired[datetime],
    Description: NotRequired[str],
```

## PromoteReadReplicaDBClusterMessageRequestTypeDef

```python
# PromoteReadReplicaDBClusterMessageRequestTypeDef definition

class PromoteReadReplicaDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
```

## RangeTypeDef

```python
# RangeTypeDef definition

class RangeTypeDef(TypedDict):
    From: NotRequired[int],
    To: NotRequired[int],
    Step: NotRequired[int],
```

## RebootDBInstanceMessageRequestTypeDef

```python
# RebootDBInstanceMessageRequestTypeDef definition

class RebootDBInstanceMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    ForceFailover: NotRequired[bool],
```

## RemoveFromGlobalClusterMessageRequestTypeDef

```python
# RemoveFromGlobalClusterMessageRequestTypeDef definition

class RemoveFromGlobalClusterMessageRequestTypeDef(TypedDict):
    GlobalClusterIdentifier: str,
    DbClusterIdentifier: str,
```

## RemoveRoleFromDBClusterMessageRequestTypeDef

```python
# RemoveRoleFromDBClusterMessageRequestTypeDef definition

class RemoveRoleFromDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    RoleArn: str,
    FeatureName: NotRequired[str],
```

## RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef

```python
# RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef definition

class RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef(TypedDict):
    SubscriptionName: str,
    SourceIdentifier: str,
```

## RemoveTagsFromResourceMessageRequestTypeDef

```python
# RemoveTagsFromResourceMessageRequestTypeDef definition

class RemoveTagsFromResourceMessageRequestTypeDef(TypedDict):
    ResourceName: str,
    TagKeys: Sequence[str],
```

## StartDBClusterMessageRequestTypeDef

```python
# StartDBClusterMessageRequestTypeDef definition

class StartDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
```

## StopDBClusterMessageRequestTypeDef

```python
# StopDBClusterMessageRequestTypeDef definition

class StopDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
```

## AddSourceIdentifierToSubscriptionResultTypeDef

```python
# AddSourceIdentifierToSubscriptionResultTypeDef definition

class AddSourceIdentifierToSubscriptionResultTypeDef(TypedDict):
    EventSubscription: EventSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDBClusterEndpointOutputTypeDef

```python
# CreateDBClusterEndpointOutputTypeDef definition

class CreateDBClusterEndpointOutputTypeDef(TypedDict):
    DBClusterEndpointIdentifier: str,
    DBClusterIdentifier: str,
    DBClusterEndpointResourceIdentifier: str,
    Endpoint: str,
    Status: str,
    EndpointType: str,
    CustomEndpointType: str,
    StaticMembers: List[str],
    ExcludedMembers: List[str],
    DBClusterEndpointArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEventSubscriptionResultTypeDef

```python
# CreateEventSubscriptionResultTypeDef definition

class CreateEventSubscriptionResultTypeDef(TypedDict):
    EventSubscription: EventSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBClusterParameterGroupNameMessageTypeDef

```python
# DBClusterParameterGroupNameMessageTypeDef definition

class DBClusterParameterGroupNameMessageTypeDef(TypedDict):
    DBClusterParameterGroupName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBParameterGroupNameMessageTypeDef

```python
# DBParameterGroupNameMessageTypeDef definition

class DBParameterGroupNameMessageTypeDef(TypedDict):
    DBParameterGroupName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDBClusterEndpointOutputTypeDef

```python
# DeleteDBClusterEndpointOutputTypeDef definition

class DeleteDBClusterEndpointOutputTypeDef(TypedDict):
    DBClusterEndpointIdentifier: str,
    DBClusterIdentifier: str,
    DBClusterEndpointResourceIdentifier: str,
    Endpoint: str,
    Status: str,
    EndpointType: str,
    CustomEndpointType: str,
    StaticMembers: List[str],
    ExcludedMembers: List[str],
    DBClusterEndpointArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEventSubscriptionResultTypeDef

```python
# DeleteEventSubscriptionResultTypeDef definition

class DeleteEventSubscriptionResultTypeDef(TypedDict):
    EventSubscription: EventSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventSubscriptionsMessageTypeDef

```python
# EventSubscriptionsMessageTypeDef definition

class EventSubscriptionsMessageTypeDef(TypedDict):
    Marker: str,
    EventSubscriptionsList: List[EventSubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDBClusterEndpointOutputTypeDef

```python
# ModifyDBClusterEndpointOutputTypeDef definition

class ModifyDBClusterEndpointOutputTypeDef(TypedDict):
    DBClusterEndpointIdentifier: str,
    DBClusterIdentifier: str,
    DBClusterEndpointResourceIdentifier: str,
    Endpoint: str,
    Status: str,
    EndpointType: str,
    CustomEndpointType: str,
    StaticMembers: List[str],
    ExcludedMembers: List[str],
    DBClusterEndpointArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyEventSubscriptionResultTypeDef

```python
# ModifyEventSubscriptionResultTypeDef definition

class ModifyEventSubscriptionResultTypeDef(TypedDict):
    EventSubscription: EventSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveSourceIdentifierFromSubscriptionResultTypeDef

```python
# RemoveSourceIdentifierFromSubscriptionResultTypeDef definition

class RemoveSourceIdentifierFromSubscriptionResultTypeDef(TypedDict):
    EventSubscription: EventSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddTagsToResourceMessageRequestTypeDef

```python
# AddTagsToResourceMessageRequestTypeDef definition

class AddTagsToResourceMessageRequestTypeDef(TypedDict):
    ResourceName: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CopyDBClusterParameterGroupMessageRequestTypeDef

```python
# CopyDBClusterParameterGroupMessageRequestTypeDef definition

class CopyDBClusterParameterGroupMessageRequestTypeDef(TypedDict):
    SourceDBClusterParameterGroupIdentifier: str,
    TargetDBClusterParameterGroupIdentifier: str,
    TargetDBClusterParameterGroupDescription: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CopyDBClusterSnapshotMessageRequestTypeDef

```python
# CopyDBClusterSnapshotMessageRequestTypeDef definition

class CopyDBClusterSnapshotMessageRequestTypeDef(TypedDict):
    SourceDBClusterSnapshotIdentifier: str,
    TargetDBClusterSnapshotIdentifier: str,
    KmsKeyId: NotRequired[str],
    PreSignedUrl: NotRequired[str],
    CopyTags: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    SourceRegion: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CopyDBParameterGroupMessageRequestTypeDef

```python
# CopyDBParameterGroupMessageRequestTypeDef definition

class CopyDBParameterGroupMessageRequestTypeDef(TypedDict):
    SourceDBParameterGroupIdentifier: str,
    TargetDBParameterGroupIdentifier: str,
    TargetDBParameterGroupDescription: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDBClusterEndpointMessageRequestTypeDef

```python
# CreateDBClusterEndpointMessageRequestTypeDef definition

class CreateDBClusterEndpointMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    DBClusterEndpointIdentifier: str,
    EndpointType: str,
    StaticMembers: NotRequired[Sequence[str]],
    ExcludedMembers: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDBClusterParameterGroupMessageRequestTypeDef

```python
# CreateDBClusterParameterGroupMessageRequestTypeDef definition

class CreateDBClusterParameterGroupMessageRequestTypeDef(TypedDict):
    DBClusterParameterGroupName: str,
    DBParameterGroupFamily: str,
    Description: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDBClusterSnapshotMessageRequestTypeDef

```python
# CreateDBClusterSnapshotMessageRequestTypeDef definition

class CreateDBClusterSnapshotMessageRequestTypeDef(TypedDict):
    DBClusterSnapshotIdentifier: str,
    DBClusterIdentifier: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDBInstanceMessageRequestTypeDef

```python
# CreateDBInstanceMessageRequestTypeDef definition

class CreateDBInstanceMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    DBInstanceClass: str,
    Engine: str,
    DBClusterIdentifier: str,
    DBName: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    MasterUsername: NotRequired[str],
    MasterUserPassword: NotRequired[str],
    DBSecurityGroups: NotRequired[Sequence[str]],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    AvailabilityZone: NotRequired[str],
    DBSubnetGroupName: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    DBParameterGroupName: NotRequired[str],
    BackupRetentionPeriod: NotRequired[int],
    PreferredBackupWindow: NotRequired[str],
    Port: NotRequired[int],
    MultiAZ: NotRequired[bool],
    EngineVersion: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    LicenseModel: NotRequired[str],
    Iops: NotRequired[int],
    OptionGroupName: NotRequired[str],
    CharacterSetName: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    StorageType: NotRequired[str],
    TdeCredentialArn: NotRequired[str],
    TdeCredentialPassword: NotRequired[str],
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    Domain: NotRequired[str],
    CopyTagsToSnapshot: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    MonitoringRoleArn: NotRequired[str],
    DomainIAMRoleName: NotRequired[str],
    PromotionTier: NotRequired[int],
    Timezone: NotRequired[str],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    EnablePerformanceInsights: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    DeletionProtection: NotRequired[bool],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDBParameterGroupMessageRequestTypeDef

```python
# CreateDBParameterGroupMessageRequestTypeDef definition

class CreateDBParameterGroupMessageRequestTypeDef(TypedDict):
    DBParameterGroupName: str,
    DBParameterGroupFamily: str,
    Description: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDBSubnetGroupMessageRequestTypeDef

```python
# CreateDBSubnetGroupMessageRequestTypeDef definition

class CreateDBSubnetGroupMessageRequestTypeDef(TypedDict):
    DBSubnetGroupName: str,
    DBSubnetGroupDescription: str,
    SubnetIds: Sequence[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEventSubscriptionMessageRequestTypeDef

```python
# CreateEventSubscriptionMessageRequestTypeDef definition

class CreateEventSubscriptionMessageRequestTypeDef(TypedDict):
    SubscriptionName: str,
    SnsTopicArn: str,
    SourceType: NotRequired[str],
    EventCategories: NotRequired[Sequence[str]],
    SourceIds: NotRequired[Sequence[str]],
    Enabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagListMessageTypeDef

```python
# TagListMessageTypeDef definition

class TagListMessageTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OrderableDBInstanceOptionTypeDef

```python
# OrderableDBInstanceOptionTypeDef definition

class OrderableDBInstanceOptionTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    LicenseModel: NotRequired[str],
    AvailabilityZones: NotRequired[List[AvailabilityZoneTypeDef]],  # (1)
    MultiAZCapable: NotRequired[bool],
    ReadReplicaCapable: NotRequired[bool],
    Vpc: NotRequired[bool],
    SupportsStorageEncryption: NotRequired[bool],
    StorageType: NotRequired[str],
    SupportsIops: NotRequired[bool],
    SupportsEnhancedMonitoring: NotRequired[bool],
    SupportsIAMDatabaseAuthentication: NotRequired[bool],
    SupportsPerformanceInsights: NotRequired[bool],
    MinStorageSize: NotRequired[int],
    MaxStorageSize: NotRequired[int],
    MinIopsPerDbInstance: NotRequired[int],
    MaxIopsPerDbInstance: NotRequired[int],
    MinIopsPerGib: NotRequired[float],
    MaxIopsPerGib: NotRequired[float],
    SupportsGlobalDatabases: NotRequired[bool],
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
## SubnetTypeDef

```python
# SubnetTypeDef definition

class SubnetTypeDef(TypedDict):
    SubnetIdentifier: NotRequired[str],
    SubnetAvailabilityZone: NotRequired[AvailabilityZoneTypeDef],  # (1)
    SubnetStatus: NotRequired[str],
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
## ModifyDBInstanceMessageRequestTypeDef

```python
# ModifyDBInstanceMessageRequestTypeDef definition

class ModifyDBInstanceMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    AllocatedStorage: NotRequired[int],
    DBInstanceClass: NotRequired[str],
    DBSubnetGroupName: NotRequired[str],
    DBSecurityGroups: NotRequired[Sequence[str]],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    ApplyImmediately: NotRequired[bool],
    MasterUserPassword: NotRequired[str],
    DBParameterGroupName: NotRequired[str],
    BackupRetentionPeriod: NotRequired[int],
    PreferredBackupWindow: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    MultiAZ: NotRequired[bool],
    EngineVersion: NotRequired[str],
    AllowMajorVersionUpgrade: NotRequired[bool],
    AutoMinorVersionUpgrade: NotRequired[bool],
    LicenseModel: NotRequired[str],
    Iops: NotRequired[int],
    OptionGroupName: NotRequired[str],
    NewDBInstanceIdentifier: NotRequired[str],
    StorageType: NotRequired[str],
    TdeCredentialArn: NotRequired[str],
    TdeCredentialPassword: NotRequired[str],
    CACertificateIdentifier: NotRequired[str],
    Domain: NotRequired[str],
    CopyTagsToSnapshot: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    DBPortNumber: NotRequired[int],
    PubliclyAccessible: NotRequired[bool],
    MonitoringRoleArn: NotRequired[str],
    DomainIAMRoleName: NotRequired[str],
    PromotionTier: NotRequired[int],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    EnablePerformanceInsights: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    CloudwatchLogsExportConfiguration: NotRequired[CloudwatchLogsExportConfigurationTypeDef],  # (1)
    DeletionProtection: NotRequired[bool],
```

1. See [:material-code-braces: CloudwatchLogsExportConfigurationTypeDef](./type_defs.md#cloudwatchlogsexportconfigurationtypedef) 
## ClusterPendingModifiedValuesTypeDef

```python
# ClusterPendingModifiedValuesTypeDef definition

class ClusterPendingModifiedValuesTypeDef(TypedDict):
    PendingCloudwatchLogsExports: NotRequired[PendingCloudwatchLogsExportsTypeDef],  # (1)
    DBClusterIdentifier: NotRequired[str],
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    EngineVersion: NotRequired[str],
    BackupRetentionPeriod: NotRequired[int],
    StorageType: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    Iops: NotRequired[int],
```

1. See [:material-code-braces: PendingCloudwatchLogsExportsTypeDef](./type_defs.md#pendingcloudwatchlogsexportstypedef) 
## PendingModifiedValuesTypeDef

```python
# PendingModifiedValuesTypeDef definition

class PendingModifiedValuesTypeDef(TypedDict):
    DBInstanceClass: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    MasterUserPassword: NotRequired[str],
    Port: NotRequired[int],
    BackupRetentionPeriod: NotRequired[int],
    MultiAZ: NotRequired[bool],
    EngineVersion: NotRequired[str],
    LicenseModel: NotRequired[str],
    Iops: NotRequired[int],
    DBInstanceIdentifier: NotRequired[str],
    StorageType: NotRequired[str],
    CACertificateIdentifier: NotRequired[str],
    DBSubnetGroupName: NotRequired[str],
    PendingCloudwatchLogsExports: NotRequired[PendingCloudwatchLogsExportsTypeDef],  # (1)
```

1. See [:material-code-braces: PendingCloudwatchLogsExportsTypeDef](./type_defs.md#pendingcloudwatchlogsexportstypedef) 
## CopyDBClusterParameterGroupResultTypeDef

```python
# CopyDBClusterParameterGroupResultTypeDef definition

class CopyDBClusterParameterGroupResultTypeDef(TypedDict):
    DBClusterParameterGroup: DBClusterParameterGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterParameterGroupTypeDef](./type_defs.md#dbclusterparametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDBClusterParameterGroupResultTypeDef

```python
# CreateDBClusterParameterGroupResultTypeDef definition

class CreateDBClusterParameterGroupResultTypeDef(TypedDict):
    DBClusterParameterGroup: DBClusterParameterGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterParameterGroupTypeDef](./type_defs.md#dbclusterparametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBClusterParameterGroupsMessageTypeDef

```python
# DBClusterParameterGroupsMessageTypeDef definition

class DBClusterParameterGroupsMessageTypeDef(TypedDict):
    Marker: str,
    DBClusterParameterGroups: List[DBClusterParameterGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterParameterGroupTypeDef](./type_defs.md#dbclusterparametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyDBClusterSnapshotResultTypeDef

```python
# CopyDBClusterSnapshotResultTypeDef definition

class CopyDBClusterSnapshotResultTypeDef(TypedDict):
    DBClusterSnapshot: DBClusterSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterSnapshotTypeDef](./type_defs.md#dbclustersnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDBClusterSnapshotResultTypeDef

```python
# CreateDBClusterSnapshotResultTypeDef definition

class CreateDBClusterSnapshotResultTypeDef(TypedDict):
    DBClusterSnapshot: DBClusterSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterSnapshotTypeDef](./type_defs.md#dbclustersnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBClusterSnapshotMessageTypeDef

```python
# DBClusterSnapshotMessageTypeDef definition

class DBClusterSnapshotMessageTypeDef(TypedDict):
    Marker: str,
    DBClusterSnapshots: List[DBClusterSnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterSnapshotTypeDef](./type_defs.md#dbclustersnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDBClusterSnapshotResultTypeDef

```python
# DeleteDBClusterSnapshotResultTypeDef definition

class DeleteDBClusterSnapshotResultTypeDef(TypedDict):
    DBClusterSnapshot: DBClusterSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterSnapshotTypeDef](./type_defs.md#dbclustersnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyDBParameterGroupResultTypeDef

```python
# CopyDBParameterGroupResultTypeDef definition

class CopyDBParameterGroupResultTypeDef(TypedDict):
    DBParameterGroup: DBParameterGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBParameterGroupTypeDef](./type_defs.md#dbparametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDBParameterGroupResultTypeDef

```python
# CreateDBParameterGroupResultTypeDef definition

class CreateDBParameterGroupResultTypeDef(TypedDict):
    DBParameterGroup: DBParameterGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBParameterGroupTypeDef](./type_defs.md#dbparametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBParameterGroupsMessageTypeDef

```python
# DBParameterGroupsMessageTypeDef definition

class DBParameterGroupsMessageTypeDef(TypedDict):
    Marker: str,
    DBParameterGroups: List[DBParameterGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBParameterGroupTypeDef](./type_defs.md#dbparametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDBClusterMessageRequestTypeDef

```python
# CreateDBClusterMessageRequestTypeDef definition

class CreateDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    Engine: str,
    AvailabilityZones: NotRequired[Sequence[str]],
    BackupRetentionPeriod: NotRequired[int],
    CharacterSetName: NotRequired[str],
    CopyTagsToSnapshot: NotRequired[bool],
    DatabaseName: NotRequired[str],
    DBClusterParameterGroupName: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    DBSubnetGroupName: NotRequired[str],
    EngineVersion: NotRequired[str],
    Port: NotRequired[int],
    MasterUsername: NotRequired[str],
    MasterUserPassword: NotRequired[str],
    OptionGroupName: NotRequired[str],
    PreferredBackupWindow: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    ReplicationSourceIdentifier: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    PreSignedUrl: NotRequired[str],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    DeletionProtection: NotRequired[bool],
    ServerlessV2ScalingConfiguration: NotRequired[ServerlessV2ScalingConfigurationTypeDef],  # (2)
    GlobalClusterIdentifier: NotRequired[str],
    StorageType: NotRequired[str],
    SourceRegion: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ServerlessV2ScalingConfigurationTypeDef](./type_defs.md#serverlessv2scalingconfigurationtypedef) 
## ModifyDBClusterMessageRequestTypeDef

```python
# ModifyDBClusterMessageRequestTypeDef definition

class ModifyDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    NewDBClusterIdentifier: NotRequired[str],
    ApplyImmediately: NotRequired[bool],
    BackupRetentionPeriod: NotRequired[int],
    DBClusterParameterGroupName: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    Port: NotRequired[int],
    MasterUserPassword: NotRequired[str],
    OptionGroupName: NotRequired[str],
    PreferredBackupWindow: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    CloudwatchLogsExportConfiguration: NotRequired[CloudwatchLogsExportConfigurationTypeDef],  # (1)
    EngineVersion: NotRequired[str],
    AllowMajorVersionUpgrade: NotRequired[bool],
    DBInstanceParameterGroupName: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    CopyTagsToSnapshot: NotRequired[bool],
    ServerlessV2ScalingConfiguration: NotRequired[ServerlessV2ScalingConfigurationTypeDef],  # (2)
    StorageType: NotRequired[str],
```

1. See [:material-code-braces: CloudwatchLogsExportConfigurationTypeDef](./type_defs.md#cloudwatchlogsexportconfigurationtypedef) 
2. See [:material-code-braces: ServerlessV2ScalingConfigurationTypeDef](./type_defs.md#serverlessv2scalingconfigurationtypedef) 
## RestoreDBClusterFromSnapshotMessageRequestTypeDef

```python
# RestoreDBClusterFromSnapshotMessageRequestTypeDef definition

class RestoreDBClusterFromSnapshotMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    SnapshotIdentifier: str,
    Engine: str,
    AvailabilityZones: NotRequired[Sequence[str]],
    EngineVersion: NotRequired[str],
    Port: NotRequired[int],
    DBSubnetGroupName: NotRequired[str],
    DatabaseName: NotRequired[str],
    OptionGroupName: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    KmsKeyId: NotRequired[str],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    DBClusterParameterGroupName: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    CopyTagsToSnapshot: NotRequired[bool],
    ServerlessV2ScalingConfiguration: NotRequired[ServerlessV2ScalingConfigurationTypeDef],  # (2)
    StorageType: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ServerlessV2ScalingConfigurationTypeDef](./type_defs.md#serverlessv2scalingconfigurationtypedef) 
## DBClusterEndpointMessageTypeDef

```python
# DBClusterEndpointMessageTypeDef definition

class DBClusterEndpointMessageTypeDef(TypedDict):
    Marker: str,
    DBClusterEndpoints: List[DBClusterEndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterEndpointTypeDef](./type_defs.md#dbclusterendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBClusterParameterGroupDetailsTypeDef

```python
# DBClusterParameterGroupDetailsTypeDef definition

class DBClusterParameterGroupDetailsTypeDef(TypedDict):
    Parameters: List[ParameterTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBParameterGroupDetailsTypeDef

```python
# DBParameterGroupDetailsTypeDef definition

class DBParameterGroupDetailsTypeDef(TypedDict):
    Parameters: List[ParameterTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EngineDefaultsTypeDef

```python
# EngineDefaultsTypeDef definition

class EngineDefaultsTypeDef(TypedDict):
    DBParameterGroupFamily: NotRequired[str],
    Marker: NotRequired[str],
    Parameters: NotRequired[List[ParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## ModifyDBClusterParameterGroupMessageRequestTypeDef

```python
# ModifyDBClusterParameterGroupMessageRequestTypeDef definition

class ModifyDBClusterParameterGroupMessageRequestTypeDef(TypedDict):
    DBClusterParameterGroupName: str,
    Parameters: Sequence[ParameterTypeDef],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## ModifyDBParameterGroupMessageRequestTypeDef

```python
# ModifyDBParameterGroupMessageRequestTypeDef definition

class ModifyDBParameterGroupMessageRequestTypeDef(TypedDict):
    DBParameterGroupName: str,
    Parameters: Sequence[ParameterTypeDef],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## ResetDBClusterParameterGroupMessageRequestTypeDef

```python
# ResetDBClusterParameterGroupMessageRequestTypeDef definition

class ResetDBClusterParameterGroupMessageRequestTypeDef(TypedDict):
    DBClusterParameterGroupName: str,
    ResetAllParameters: NotRequired[bool],
    Parameters: NotRequired[Sequence[ParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## ResetDBParameterGroupMessageRequestTypeDef

```python
# ResetDBParameterGroupMessageRequestTypeDef definition

class ResetDBParameterGroupMessageRequestTypeDef(TypedDict):
    DBParameterGroupName: str,
    ResetAllParameters: NotRequired[bool],
    Parameters: NotRequired[Sequence[ParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## DBClusterSnapshotAttributesResultTypeDef

```python
# DBClusterSnapshotAttributesResultTypeDef definition

class DBClusterSnapshotAttributesResultTypeDef(TypedDict):
    DBClusterSnapshotIdentifier: NotRequired[str],
    DBClusterSnapshotAttributes: NotRequired[List[DBClusterSnapshotAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: DBClusterSnapshotAttributeTypeDef](./type_defs.md#dbclustersnapshotattributetypedef) 
## DBEngineVersionTypeDef

```python
# DBEngineVersionTypeDef definition

class DBEngineVersionTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    DBParameterGroupFamily: NotRequired[str],
    DBEngineDescription: NotRequired[str],
    DBEngineVersionDescription: NotRequired[str],
    DefaultCharacterSet: NotRequired[CharacterSetTypeDef],  # (1)
    SupportedCharacterSets: NotRequired[List[CharacterSetTypeDef]],  # (2)
    ValidUpgradeTarget: NotRequired[List[UpgradeTargetTypeDef]],  # (3)
    SupportedTimezones: NotRequired[List[TimezoneTypeDef]],  # (4)
    ExportableLogTypes: NotRequired[List[str]],
    SupportsLogExportsToCloudwatchLogs: NotRequired[bool],
    SupportsReadReplica: NotRequired[bool],
    SupportsGlobalDatabases: NotRequired[bool],
```

1. See [:material-code-braces: CharacterSetTypeDef](./type_defs.md#charactersettypedef) 
2. See [:material-code-braces: CharacterSetTypeDef](./type_defs.md#charactersettypedef) 
3. See [:material-code-braces: UpgradeTargetTypeDef](./type_defs.md#upgradetargettypedef) 
4. See [:material-code-braces: TimezoneTypeDef](./type_defs.md#timezonetypedef) 
## DescribeDBClusterEndpointsMessageRequestTypeDef

```python
# DescribeDBClusterEndpointsMessageRequestTypeDef definition

class DescribeDBClusterEndpointsMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    DBClusterEndpointIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBClusterParameterGroupsMessageRequestTypeDef

```python
# DescribeDBClusterParameterGroupsMessageRequestTypeDef definition

class DescribeDBClusterParameterGroupsMessageRequestTypeDef(TypedDict):
    DBClusterParameterGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBClusterParametersMessageRequestTypeDef

```python
# DescribeDBClusterParametersMessageRequestTypeDef definition

class DescribeDBClusterParametersMessageRequestTypeDef(TypedDict):
    DBClusterParameterGroupName: str,
    Source: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBClusterSnapshotsMessageRequestTypeDef

```python
# DescribeDBClusterSnapshotsMessageRequestTypeDef definition

class DescribeDBClusterSnapshotsMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    DBClusterSnapshotIdentifier: NotRequired[str],
    SnapshotType: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    IncludeShared: NotRequired[bool],
    IncludePublic: NotRequired[bool],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBClustersMessageRequestTypeDef

```python
# DescribeDBClustersMessageRequestTypeDef definition

class DescribeDBClustersMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBEngineVersionsMessageRequestTypeDef

```python
# DescribeDBEngineVersionsMessageRequestTypeDef definition

class DescribeDBEngineVersionsMessageRequestTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    DBParameterGroupFamily: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    DefaultOnly: NotRequired[bool],
    ListSupportedCharacterSets: NotRequired[bool],
    ListSupportedTimezones: NotRequired[bool],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBInstancesMessageRequestTypeDef

```python
# DescribeDBInstancesMessageRequestTypeDef definition

class DescribeDBInstancesMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBParameterGroupsMessageRequestTypeDef

```python
# DescribeDBParameterGroupsMessageRequestTypeDef definition

class DescribeDBParameterGroupsMessageRequestTypeDef(TypedDict):
    DBParameterGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBParametersMessageRequestTypeDef

```python
# DescribeDBParametersMessageRequestTypeDef definition

class DescribeDBParametersMessageRequestTypeDef(TypedDict):
    DBParameterGroupName: str,
    Source: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBSubnetGroupsMessageRequestTypeDef

```python
# DescribeDBSubnetGroupsMessageRequestTypeDef definition

class DescribeDBSubnetGroupsMessageRequestTypeDef(TypedDict):
    DBSubnetGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeEngineDefaultClusterParametersMessageRequestTypeDef

```python
# DescribeEngineDefaultClusterParametersMessageRequestTypeDef definition

class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(TypedDict):
    DBParameterGroupFamily: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeEngineDefaultParametersMessageRequestTypeDef

```python
# DescribeEngineDefaultParametersMessageRequestTypeDef definition

class DescribeEngineDefaultParametersMessageRequestTypeDef(TypedDict):
    DBParameterGroupFamily: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeEventCategoriesMessageRequestTypeDef

```python
# DescribeEventCategoriesMessageRequestTypeDef definition

class DescribeEventCategoriesMessageRequestTypeDef(TypedDict):
    SourceType: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeEventSubscriptionsMessageRequestTypeDef

```python
# DescribeEventSubscriptionsMessageRequestTypeDef definition

class DescribeEventSubscriptionsMessageRequestTypeDef(TypedDict):
    SubscriptionName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeOrderableDBInstanceOptionsMessageRequestTypeDef

```python
# DescribeOrderableDBInstanceOptionsMessageRequestTypeDef definition

class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(TypedDict):
    Engine: str,
    EngineVersion: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    LicenseModel: NotRequired[str],
    Vpc: NotRequired[bool],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribePendingMaintenanceActionsMessageRequestTypeDef

```python
# DescribePendingMaintenanceActionsMessageRequestTypeDef definition

class DescribePendingMaintenanceActionsMessageRequestTypeDef(TypedDict):
    ResourceIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListTagsForResourceMessageRequestTypeDef

```python
# ListTagsForResourceMessageRequestTypeDef definition

class ListTagsForResourceMessageRequestTypeDef(TypedDict):
    ResourceName: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef

```python
# DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef definition

class DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    DBClusterEndpointIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef

```python
# DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef definition

class DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef(TypedDict):
    DBClusterParameterGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef

```python
# DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef definition

class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(TypedDict):
    DBClusterParameterGroupName: str,
    Source: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef

```python
# DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef definition

class DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    DBClusterSnapshotIdentifier: NotRequired[str],
    SnapshotType: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    IncludeShared: NotRequired[bool],
    IncludePublic: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef

```python
# DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef definition

class DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef

```python
# DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef definition

class DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    DBParameterGroupFamily: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    DefaultOnly: NotRequired[bool],
    ListSupportedCharacterSets: NotRequired[bool],
    ListSupportedTimezones: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef

```python
# DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef definition

class DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef

```python
# DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef definition

class DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef(TypedDict):
    DBParameterGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef

```python
# DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef definition

class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(TypedDict):
    DBParameterGroupName: str,
    Source: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef

```python
# DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef definition

class DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef(TypedDict):
    DBSubnetGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef

```python
# DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef definition

class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(TypedDict):
    DBParameterGroupFamily: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef

```python
# DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef definition

class DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef(TypedDict):
    SubscriptionName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef

```python
# DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef definition

class DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef(TypedDict):
    GlobalClusterIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef

```python
# DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef definition

class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(TypedDict):
    Engine: str,
    EngineVersion: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    LicenseModel: NotRequired[str],
    Vpc: NotRequired[bool],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef

```python
# DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef definition

class DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef(TypedDict):
    ResourceIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef

```python
# DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef definition

class DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef

```python
# DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef definition

class DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEventsMessageDescribeEventsPaginateTypeDef

```python
# DescribeEventsMessageDescribeEventsPaginateTypeDef definition

class DescribeEventsMessageDescribeEventsPaginateTypeDef(TypedDict):
    SourceIdentifier: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Duration: NotRequired[int],
    EventCategories: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsMessageRequestTypeDef

```python
# DescribeEventsMessageRequestTypeDef definition

class DescribeEventsMessageRequestTypeDef(TypedDict):
    SourceIdentifier: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Duration: NotRequired[int],
    EventCategories: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## RestoreDBClusterToPointInTimeMessageRequestTypeDef

```python
# RestoreDBClusterToPointInTimeMessageRequestTypeDef definition

class RestoreDBClusterToPointInTimeMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    SourceDBClusterIdentifier: str,
    RestoreType: NotRequired[str],
    RestoreToTime: NotRequired[TimestampTypeDef],
    UseLatestRestorableTime: NotRequired[bool],
    Port: NotRequired[int],
    DBSubnetGroupName: NotRequired[str],
    OptionGroupName: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    KmsKeyId: NotRequired[str],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    DBClusterParameterGroupName: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    ServerlessV2ScalingConfiguration: NotRequired[ServerlessV2ScalingConfigurationTypeDef],  # (2)
    StorageType: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ServerlessV2ScalingConfigurationTypeDef](./type_defs.md#serverlessv2scalingconfigurationtypedef) 
## EventCategoriesMessageTypeDef

```python
# EventCategoriesMessageTypeDef definition

class EventCategoriesMessageTypeDef(TypedDict):
    EventCategoriesMapList: List[EventCategoriesMapTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventCategoriesMapTypeDef](./type_defs.md#eventcategoriesmaptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## GlobalClusterTypeDef

```python
# GlobalClusterTypeDef definition

class GlobalClusterTypeDef(TypedDict):
    GlobalClusterIdentifier: NotRequired[str],
    GlobalClusterResourceId: NotRequired[str],
    GlobalClusterArn: NotRequired[str],
    Status: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    StorageEncrypted: NotRequired[bool],
    DeletionProtection: NotRequired[bool],
    GlobalClusterMembers: NotRequired[List[GlobalClusterMemberTypeDef]],  # (1)
```

1. See [:material-code-braces: GlobalClusterMemberTypeDef](./type_defs.md#globalclustermembertypedef) 
## ResourcePendingMaintenanceActionsTypeDef

```python
# ResourcePendingMaintenanceActionsTypeDef definition

class ResourcePendingMaintenanceActionsTypeDef(TypedDict):
    ResourceIdentifier: NotRequired[str],
    PendingMaintenanceActionDetails: NotRequired[List[PendingMaintenanceActionTypeDef]],  # (1)
```

1. See [:material-code-braces: PendingMaintenanceActionTypeDef](./type_defs.md#pendingmaintenanceactiontypedef) 
## ValidStorageOptionsTypeDef

```python
# ValidStorageOptionsTypeDef definition

class ValidStorageOptionsTypeDef(TypedDict):
    StorageType: NotRequired[str],
    StorageSize: NotRequired[List[RangeTypeDef]],  # (1)
    ProvisionedIops: NotRequired[List[RangeTypeDef]],  # (1)
    IopsToStorageRatio: NotRequired[List[DoubleRangeTypeDef]],  # (3)
```

1. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
2. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
3. See [:material-code-braces: DoubleRangeTypeDef](./type_defs.md#doublerangetypedef) 
## OrderableDBInstanceOptionsMessageTypeDef

```python
# OrderableDBInstanceOptionsMessageTypeDef definition

class OrderableDBInstanceOptionsMessageTypeDef(TypedDict):
    OrderableDBInstanceOptions: List[OrderableDBInstanceOptionTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrderableDBInstanceOptionTypeDef](./type_defs.md#orderabledbinstanceoptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBSubnetGroupTypeDef

```python
# DBSubnetGroupTypeDef definition

class DBSubnetGroupTypeDef(TypedDict):
    DBSubnetGroupName: NotRequired[str],
    DBSubnetGroupDescription: NotRequired[str],
    VpcId: NotRequired[str],
    SubnetGroupStatus: NotRequired[str],
    Subnets: NotRequired[List[SubnetTypeDef]],  # (1)
    DBSubnetGroupArn: NotRequired[str],
```

1. See [:material-code-braces: SubnetTypeDef](./type_defs.md#subnettypedef) 
## DBClusterTypeDef

```python
# DBClusterTypeDef definition

class DBClusterTypeDef(TypedDict):
    AllocatedStorage: NotRequired[int],
    AvailabilityZones: NotRequired[List[str]],
    BackupRetentionPeriod: NotRequired[int],
    CharacterSetName: NotRequired[str],
    DatabaseName: NotRequired[str],
    DBClusterIdentifier: NotRequired[str],
    DBClusterParameterGroup: NotRequired[str],
    DBSubnetGroup: NotRequired[str],
    Status: NotRequired[str],
    PercentProgress: NotRequired[str],
    EarliestRestorableTime: NotRequired[datetime],
    Endpoint: NotRequired[str],
    ReaderEndpoint: NotRequired[str],
    MultiAZ: NotRequired[bool],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    LatestRestorableTime: NotRequired[datetime],
    Port: NotRequired[int],
    MasterUsername: NotRequired[str],
    DBClusterOptionGroupMemberships: NotRequired[List[DBClusterOptionGroupStatusTypeDef]],  # (1)
    PreferredBackupWindow: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    ReplicationSourceIdentifier: NotRequired[str],
    ReadReplicaIdentifiers: NotRequired[List[str]],
    DBClusterMembers: NotRequired[List[DBClusterMemberTypeDef]],  # (2)
    VpcSecurityGroups: NotRequired[List[VpcSecurityGroupMembershipTypeDef]],  # (3)
    HostedZoneId: NotRequired[str],
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    DbClusterResourceId: NotRequired[str],
    DBClusterArn: NotRequired[str],
    AssociatedRoles: NotRequired[List[DBClusterRoleTypeDef]],  # (4)
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    CloneGroupId: NotRequired[str],
    ClusterCreateTime: NotRequired[datetime],
    CopyTagsToSnapshot: NotRequired[bool],
    EnabledCloudwatchLogsExports: NotRequired[List[str]],
    PendingModifiedValues: NotRequired[ClusterPendingModifiedValuesTypeDef],  # (5)
    DeletionProtection: NotRequired[bool],
    CrossAccountClone: NotRequired[bool],
    AutomaticRestartTime: NotRequired[datetime],
    ServerlessV2ScalingConfiguration: NotRequired[ServerlessV2ScalingConfigurationInfoTypeDef],  # (6)
    GlobalClusterIdentifier: NotRequired[str],
    IOOptimizedNextAllowedModificationTime: NotRequired[datetime],
    StorageType: NotRequired[str],
```

1. See [:material-code-braces: DBClusterOptionGroupStatusTypeDef](./type_defs.md#dbclusteroptiongroupstatustypedef) 
2. See [:material-code-braces: DBClusterMemberTypeDef](./type_defs.md#dbclustermembertypedef) 
3. See [:material-code-braces: VpcSecurityGroupMembershipTypeDef](./type_defs.md#vpcsecuritygroupmembershiptypedef) 
4. See [:material-code-braces: DBClusterRoleTypeDef](./type_defs.md#dbclusterroletypedef) 
5. See [:material-code-braces: ClusterPendingModifiedValuesTypeDef](./type_defs.md#clusterpendingmodifiedvaluestypedef) 
6. See [:material-code-braces: ServerlessV2ScalingConfigurationInfoTypeDef](./type_defs.md#serverlessv2scalingconfigurationinfotypedef) 
## DescribeEngineDefaultClusterParametersResultTypeDef

```python
# DescribeEngineDefaultClusterParametersResultTypeDef definition

class DescribeEngineDefaultClusterParametersResultTypeDef(TypedDict):
    EngineDefaults: EngineDefaultsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EngineDefaultsTypeDef](./type_defs.md#enginedefaultstypedef) 
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
## DescribeDBClusterSnapshotAttributesResultTypeDef

```python
# DescribeDBClusterSnapshotAttributesResultTypeDef definition

class DescribeDBClusterSnapshotAttributesResultTypeDef(TypedDict):
    DBClusterSnapshotAttributesResult: DBClusterSnapshotAttributesResultTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterSnapshotAttributesResultTypeDef](./type_defs.md#dbclustersnapshotattributesresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDBClusterSnapshotAttributeResultTypeDef

```python
# ModifyDBClusterSnapshotAttributeResultTypeDef definition

class ModifyDBClusterSnapshotAttributeResultTypeDef(TypedDict):
    DBClusterSnapshotAttributesResult: DBClusterSnapshotAttributesResultTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterSnapshotAttributesResultTypeDef](./type_defs.md#dbclustersnapshotattributesresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBEngineVersionMessageTypeDef

```python
# DBEngineVersionMessageTypeDef definition

class DBEngineVersionMessageTypeDef(TypedDict):
    Marker: str,
    DBEngineVersions: List[DBEngineVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBEngineVersionTypeDef](./type_defs.md#dbengineversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGlobalClusterResultTypeDef

```python
# CreateGlobalClusterResultTypeDef definition

class CreateGlobalClusterResultTypeDef(TypedDict):
    GlobalCluster: GlobalClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalClusterTypeDef](./type_defs.md#globalclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGlobalClusterResultTypeDef

```python
# DeleteGlobalClusterResultTypeDef definition

class DeleteGlobalClusterResultTypeDef(TypedDict):
    GlobalCluster: GlobalClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalClusterTypeDef](./type_defs.md#globalclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FailoverGlobalClusterResultTypeDef

```python
# FailoverGlobalClusterResultTypeDef definition

class FailoverGlobalClusterResultTypeDef(TypedDict):
    GlobalCluster: GlobalClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalClusterTypeDef](./type_defs.md#globalclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GlobalClustersMessageTypeDef

```python
# GlobalClustersMessageTypeDef definition

class GlobalClustersMessageTypeDef(TypedDict):
    Marker: str,
    GlobalClusters: List[GlobalClusterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalClusterTypeDef](./type_defs.md#globalclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyGlobalClusterResultTypeDef

```python
# ModifyGlobalClusterResultTypeDef definition

class ModifyGlobalClusterResultTypeDef(TypedDict):
    GlobalCluster: GlobalClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalClusterTypeDef](./type_defs.md#globalclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveFromGlobalClusterResultTypeDef

```python
# RemoveFromGlobalClusterResultTypeDef definition

class RemoveFromGlobalClusterResultTypeDef(TypedDict):
    GlobalCluster: GlobalClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalClusterTypeDef](./type_defs.md#globalclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplyPendingMaintenanceActionResultTypeDef

```python
# ApplyPendingMaintenanceActionResultTypeDef definition

class ApplyPendingMaintenanceActionResultTypeDef(TypedDict):
    ResourcePendingMaintenanceActions: ResourcePendingMaintenanceActionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePendingMaintenanceActionsTypeDef](./type_defs.md#resourcependingmaintenanceactionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PendingMaintenanceActionsMessageTypeDef

```python
# PendingMaintenanceActionsMessageTypeDef definition

class PendingMaintenanceActionsMessageTypeDef(TypedDict):
    PendingMaintenanceActions: List[ResourcePendingMaintenanceActionsTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePendingMaintenanceActionsTypeDef](./type_defs.md#resourcependingmaintenanceactionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ValidDBInstanceModificationsMessageTypeDef

```python
# ValidDBInstanceModificationsMessageTypeDef definition

class ValidDBInstanceModificationsMessageTypeDef(TypedDict):
    Storage: NotRequired[List[ValidStorageOptionsTypeDef]],  # (1)
```

1. See [:material-code-braces: ValidStorageOptionsTypeDef](./type_defs.md#validstorageoptionstypedef) 
## CreateDBSubnetGroupResultTypeDef

```python
# CreateDBSubnetGroupResultTypeDef definition

class CreateDBSubnetGroupResultTypeDef(TypedDict):
    DBSubnetGroup: DBSubnetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSubnetGroupTypeDef](./type_defs.md#dbsubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBInstanceTypeDef

```python
# DBInstanceTypeDef definition

class DBInstanceTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    Engine: NotRequired[str],
    DBInstanceStatus: NotRequired[str],
    MasterUsername: NotRequired[str],
    DBName: NotRequired[str],
    Endpoint: NotRequired[EndpointTypeDef],  # (1)
    AllocatedStorage: NotRequired[int],
    InstanceCreateTime: NotRequired[datetime],
    PreferredBackupWindow: NotRequired[str],
    BackupRetentionPeriod: NotRequired[int],
    DBSecurityGroups: NotRequired[List[DBSecurityGroupMembershipTypeDef]],  # (2)
    VpcSecurityGroups: NotRequired[List[VpcSecurityGroupMembershipTypeDef]],  # (3)
    DBParameterGroups: NotRequired[List[DBParameterGroupStatusTypeDef]],  # (4)
    AvailabilityZone: NotRequired[str],
    DBSubnetGroup: NotRequired[DBSubnetGroupTypeDef],  # (5)
    PreferredMaintenanceWindow: NotRequired[str],
    PendingModifiedValues: NotRequired[PendingModifiedValuesTypeDef],  # (6)
    LatestRestorableTime: NotRequired[datetime],
    MultiAZ: NotRequired[bool],
    EngineVersion: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    ReadReplicaSourceDBInstanceIdentifier: NotRequired[str],
    ReadReplicaDBInstanceIdentifiers: NotRequired[List[str]],
    ReadReplicaDBClusterIdentifiers: NotRequired[List[str]],
    LicenseModel: NotRequired[str],
    Iops: NotRequired[int],
    OptionGroupMemberships: NotRequired[List[OptionGroupMembershipTypeDef]],  # (7)
    CharacterSetName: NotRequired[str],
    SecondaryAvailabilityZone: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    StatusInfos: NotRequired[List[DBInstanceStatusInfoTypeDef]],  # (8)
    StorageType: NotRequired[str],
    TdeCredentialArn: NotRequired[str],
    DbInstancePort: NotRequired[int],
    DBClusterIdentifier: NotRequired[str],
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    DbiResourceId: NotRequired[str],
    CACertificateIdentifier: NotRequired[str],
    DomainMemberships: NotRequired[List[DomainMembershipTypeDef]],  # (9)
    CopyTagsToSnapshot: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    EnhancedMonitoringResourceArn: NotRequired[str],
    MonitoringRoleArn: NotRequired[str],
    PromotionTier: NotRequired[int],
    DBInstanceArn: NotRequired[str],
    Timezone: NotRequired[str],
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    PerformanceInsightsEnabled: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    EnabledCloudwatchLogsExports: NotRequired[List[str]],
    DeletionProtection: NotRequired[bool],
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: DBSecurityGroupMembershipTypeDef](./type_defs.md#dbsecuritygroupmembershiptypedef) 
3. See [:material-code-braces: VpcSecurityGroupMembershipTypeDef](./type_defs.md#vpcsecuritygroupmembershiptypedef) 
4. See [:material-code-braces: DBParameterGroupStatusTypeDef](./type_defs.md#dbparametergroupstatustypedef) 
5. See [:material-code-braces: DBSubnetGroupTypeDef](./type_defs.md#dbsubnetgrouptypedef) 
6. See [:material-code-braces: PendingModifiedValuesTypeDef](./type_defs.md#pendingmodifiedvaluestypedef) 
7. See [:material-code-braces: OptionGroupMembershipTypeDef](./type_defs.md#optiongroupmembershiptypedef) 
8. See [:material-code-braces: DBInstanceStatusInfoTypeDef](./type_defs.md#dbinstancestatusinfotypedef) 
9. See [:material-code-braces: DomainMembershipTypeDef](./type_defs.md#domainmembershiptypedef) 
## DBSubnetGroupMessageTypeDef

```python
# DBSubnetGroupMessageTypeDef definition

class DBSubnetGroupMessageTypeDef(TypedDict):
    Marker: str,
    DBSubnetGroups: List[DBSubnetGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSubnetGroupTypeDef](./type_defs.md#dbsubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDBSubnetGroupResultTypeDef

```python
# ModifyDBSubnetGroupResultTypeDef definition

class ModifyDBSubnetGroupResultTypeDef(TypedDict):
    DBSubnetGroup: DBSubnetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSubnetGroupTypeDef](./type_defs.md#dbsubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDBClusterResultTypeDef

```python
# CreateDBClusterResultTypeDef definition

class CreateDBClusterResultTypeDef(TypedDict):
    DBCluster: DBClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterTypeDef](./type_defs.md#dbclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBClusterMessageTypeDef

```python
# DBClusterMessageTypeDef definition

class DBClusterMessageTypeDef(TypedDict):
    Marker: str,
    DBClusters: List[DBClusterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterTypeDef](./type_defs.md#dbclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDBClusterResultTypeDef

```python
# DeleteDBClusterResultTypeDef definition

class DeleteDBClusterResultTypeDef(TypedDict):
    DBCluster: DBClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterTypeDef](./type_defs.md#dbclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FailoverDBClusterResultTypeDef

```python
# FailoverDBClusterResultTypeDef definition

class FailoverDBClusterResultTypeDef(TypedDict):
    DBCluster: DBClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterTypeDef](./type_defs.md#dbclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDBClusterResultTypeDef

```python
# ModifyDBClusterResultTypeDef definition

class ModifyDBClusterResultTypeDef(TypedDict):
    DBCluster: DBClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterTypeDef](./type_defs.md#dbclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PromoteReadReplicaDBClusterResultTypeDef

```python
# PromoteReadReplicaDBClusterResultTypeDef definition

class PromoteReadReplicaDBClusterResultTypeDef(TypedDict):
    DBCluster: DBClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterTypeDef](./type_defs.md#dbclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreDBClusterFromSnapshotResultTypeDef

```python
# RestoreDBClusterFromSnapshotResultTypeDef definition

class RestoreDBClusterFromSnapshotResultTypeDef(TypedDict):
    DBCluster: DBClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterTypeDef](./type_defs.md#dbclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreDBClusterToPointInTimeResultTypeDef

```python
# RestoreDBClusterToPointInTimeResultTypeDef definition

class RestoreDBClusterToPointInTimeResultTypeDef(TypedDict):
    DBCluster: DBClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterTypeDef](./type_defs.md#dbclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDBClusterResultTypeDef

```python
# StartDBClusterResultTypeDef definition

class StartDBClusterResultTypeDef(TypedDict):
    DBCluster: DBClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterTypeDef](./type_defs.md#dbclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopDBClusterResultTypeDef

```python
# StopDBClusterResultTypeDef definition

class StopDBClusterResultTypeDef(TypedDict):
    DBCluster: DBClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterTypeDef](./type_defs.md#dbclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeValidDBInstanceModificationsResultTypeDef

```python
# DescribeValidDBInstanceModificationsResultTypeDef definition

class DescribeValidDBInstanceModificationsResultTypeDef(TypedDict):
    ValidDBInstanceModificationsMessage: ValidDBInstanceModificationsMessageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidDBInstanceModificationsMessageTypeDef](./type_defs.md#validdbinstancemodificationsmessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDBInstanceResultTypeDef

```python
# CreateDBInstanceResultTypeDef definition

class CreateDBInstanceResultTypeDef(TypedDict):
    DBInstance: DBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBInstanceMessageTypeDef

```python
# DBInstanceMessageTypeDef definition

class DBInstanceMessageTypeDef(TypedDict):
    Marker: str,
    DBInstances: List[DBInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDBInstanceResultTypeDef

```python
# DeleteDBInstanceResultTypeDef definition

class DeleteDBInstanceResultTypeDef(TypedDict):
    DBInstance: DBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDBInstanceResultTypeDef

```python
# ModifyDBInstanceResultTypeDef definition

class ModifyDBInstanceResultTypeDef(TypedDict):
    DBInstance: DBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RebootDBInstanceResultTypeDef

```python
# RebootDBInstanceResultTypeDef definition

class RebootDBInstanceResultTypeDef(TypedDict):
    DBInstance: DBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
