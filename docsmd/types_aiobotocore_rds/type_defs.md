# Type definitions

> [Index](../README.md) > [RDS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RDS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#rds)
    type annotations stubs module [types-aiobotocore-rds](https://pypi.org/project/types-aiobotocore-rds/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ParameterUnionTypeDef

```python
# ParameterUnionTypeDef definition

ParameterUnionTypeDef = Union[
    ParameterTypeDef,  # (1)
    ParameterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ParameterOutputTypeDef](./type_defs.md#parameteroutputtypedef) 



## AccountQuotaTypeDef

```python
# AccountQuotaTypeDef definition

class AccountQuotaTypeDef(TypedDict):
    AccountQuotaName: NotRequired[str],
    Used: NotRequired[int],
    Max: NotRequired[int],
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

## AddRoleToDBClusterMessageRequestTypeDef

```python
# AddRoleToDBClusterMessageRequestTypeDef definition

class AddRoleToDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    RoleArn: str,
    FeatureName: NotRequired[str],
```

## AddRoleToDBInstanceMessageRequestTypeDef

```python
# AddRoleToDBInstanceMessageRequestTypeDef definition

class AddRoleToDBInstanceMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    RoleArn: str,
    FeatureName: str,
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

## AuthorizeDBSecurityGroupIngressMessageRequestTypeDef

```python
# AuthorizeDBSecurityGroupIngressMessageRequestTypeDef definition

class AuthorizeDBSecurityGroupIngressMessageRequestTypeDef(TypedDict):
    DBSecurityGroupName: str,
    CIDRIP: NotRequired[str],
    EC2SecurityGroupName: NotRequired[str],
    EC2SecurityGroupId: NotRequired[str],
    EC2SecurityGroupOwnerId: NotRequired[str],
```

## AvailabilityZoneTypeDef

```python
# AvailabilityZoneTypeDef definition

class AvailabilityZoneTypeDef(TypedDict):
    Name: NotRequired[str],
```

## AvailableProcessorFeatureTypeDef

```python
# AvailableProcessorFeatureTypeDef definition

class AvailableProcessorFeatureTypeDef(TypedDict):
    Name: NotRequired[str],
    DefaultValue: NotRequired[str],
    AllowedValues: NotRequired[str],
```

## BlueGreenDeploymentTaskTypeDef

```python
# BlueGreenDeploymentTaskTypeDef definition

class BlueGreenDeploymentTaskTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[str],
```

## SwitchoverDetailTypeDef

```python
# SwitchoverDetailTypeDef definition

class SwitchoverDetailTypeDef(TypedDict):
    SourceMember: NotRequired[str],
    TargetMember: NotRequired[str],
    Status: NotRequired[str],
```

## CancelExportTaskMessageRequestTypeDef

```python
# CancelExportTaskMessageRequestTypeDef definition

class CancelExportTaskMessageRequestTypeDef(TypedDict):
    ExportTaskIdentifier: str,
```

## CertificateDetailsTypeDef

```python
# CertificateDetailsTypeDef definition

class CertificateDetailsTypeDef(TypedDict):
    CAIdentifier: NotRequired[str],
    ValidTill: NotRequired[datetime],
```

## CertificateTypeDef

```python
# CertificateTypeDef definition

class CertificateTypeDef(TypedDict):
    CertificateIdentifier: NotRequired[str],
    CertificateType: NotRequired[str],
    Thumbprint: NotRequired[str],
    ValidFrom: NotRequired[datetime],
    ValidTill: NotRequired[datetime],
    CertificateArn: NotRequired[str],
    CustomerOverride: NotRequired[bool],
    CustomerOverrideValidTill: NotRequired[datetime],
```

## CharacterSetTypeDef

```python
# CharacterSetTypeDef definition

class CharacterSetTypeDef(TypedDict):
    CharacterSetName: NotRequired[str],
    CharacterSetDescription: NotRequired[str],
```

## ClientGenerateDbAuthTokenRequestTypeDef

```python
# ClientGenerateDbAuthTokenRequestTypeDef definition

class ClientGenerateDbAuthTokenRequestTypeDef(TypedDict):
    DBHostname: str,
    Port: int,
    DBUsername: str,
    Region: NotRequired[Union[str, None]],
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

## RdsCustomClusterConfigurationTypeDef

```python
# RdsCustomClusterConfigurationTypeDef definition

class RdsCustomClusterConfigurationTypeDef(TypedDict):
    InterconnectSubnetId: NotRequired[str],
    TransitGatewayMulticastDomainId: NotRequired[str],
    ReplicaMode: NotRequired[ReplicaModeType],  # (1)
```

1. See [:material-code-brackets: ReplicaModeType](./literals.md#replicamodetype) 
## ConnectionPoolConfigurationInfoTypeDef

```python
# ConnectionPoolConfigurationInfoTypeDef definition

class ConnectionPoolConfigurationInfoTypeDef(TypedDict):
    MaxConnectionsPercent: NotRequired[int],
    MaxIdleConnectionsPercent: NotRequired[int],
    ConnectionBorrowTimeout: NotRequired[int],
    SessionPinningFilters: NotRequired[List[str]],
    InitQuery: NotRequired[str],
```

## ConnectionPoolConfigurationTypeDef

```python
# ConnectionPoolConfigurationTypeDef definition

class ConnectionPoolConfigurationTypeDef(TypedDict):
    MaxConnectionsPercent: NotRequired[int],
    MaxIdleConnectionsPercent: NotRequired[int],
    ConnectionBorrowTimeout: NotRequired[int],
    SessionPinningFilters: NotRequired[Sequence[str]],
    InitQuery: NotRequired[str],
```

## ContextAttributeTypeDef

```python
# ContextAttributeTypeDef definition

class ContextAttributeTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
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

## DBParameterGroupTypeDef

```python
# DBParameterGroupTypeDef definition

class DBParameterGroupTypeDef(TypedDict):
    DBParameterGroupName: NotRequired[str],
    DBParameterGroupFamily: NotRequired[str],
    Description: NotRequired[str],
    DBParameterGroupArn: NotRequired[str],
```

## ScalingConfigurationTypeDef

```python
# ScalingConfigurationTypeDef definition

class ScalingConfigurationTypeDef(TypedDict):
    MinCapacity: NotRequired[int],
    MaxCapacity: NotRequired[int],
    AutoPause: NotRequired[bool],
    SecondsUntilAutoPause: NotRequired[int],
    TimeoutAction: NotRequired[str],
    SecondsBeforeTimeout: NotRequired[int],
```

## ServerlessV2ScalingConfigurationTypeDef

```python
# ServerlessV2ScalingConfigurationTypeDef definition

class ServerlessV2ScalingConfigurationTypeDef(TypedDict):
    MinCapacity: NotRequired[float],
    MaxCapacity: NotRequired[float],
    SecondsUntilAutoPause: NotRequired[int],
```

## ProcessorFeatureTypeDef

```python
# ProcessorFeatureTypeDef definition

class ProcessorFeatureTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## DBProxyEndpointTypeDef

```python
# DBProxyEndpointTypeDef definition

class DBProxyEndpointTypeDef(TypedDict):
    DBProxyEndpointName: NotRequired[str],
    DBProxyEndpointArn: NotRequired[str],
    DBProxyName: NotRequired[str],
    Status: NotRequired[DBProxyEndpointStatusType],  # (1)
    VpcId: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[List[str]],
    VpcSubnetIds: NotRequired[List[str]],
    Endpoint: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    TargetRole: NotRequired[DBProxyEndpointTargetRoleType],  # (2)
    IsDefault: NotRequired[bool],
```

1. See [:material-code-brackets: DBProxyEndpointStatusType](./literals.md#dbproxyendpointstatustype) 
2. See [:material-code-brackets: DBProxyEndpointTargetRoleType](./literals.md#dbproxyendpointtargetroletype) 
## UserAuthConfigTypeDef

```python
# UserAuthConfigTypeDef definition

class UserAuthConfigTypeDef(TypedDict):
    Description: NotRequired[str],
    UserName: NotRequired[str],
    AuthScheme: NotRequired[AuthSchemeType],  # (1)
    SecretArn: NotRequired[str],
    IAMAuth: NotRequired[IAMAuthModeType],  # (2)
    ClientPasswordAuthType: NotRequired[ClientPasswordAuthTypeType],  # (3)
```

1. See [:material-code-brackets: AuthSchemeType](./literals.md#authschemetype) 
2. See [:material-code-brackets: IAMAuthModeType](./literals.md#iamauthmodetype) 
3. See [:material-code-brackets: ClientPasswordAuthTypeType](./literals.md#clientpasswordauthtypetype) 
## CustomDBEngineVersionAMITypeDef

```python
# CustomDBEngineVersionAMITypeDef definition

class CustomDBEngineVersionAMITypeDef(TypedDict):
    ImageId: NotRequired[str],
    Status: NotRequired[str],
```

## RestoreWindowTypeDef

```python
# RestoreWindowTypeDef definition

class RestoreWindowTypeDef(TypedDict):
    EarliestTime: NotRequired[datetime],
    LatestTime: NotRequired[datetime],
```

## DBClusterBacktrackTypeDef

```python
# DBClusterBacktrackTypeDef definition

class DBClusterBacktrackTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    BacktrackIdentifier: NotRequired[str],
    BacktrackTo: NotRequired[datetime],
    BacktrackedFrom: NotRequired[datetime],
    BacktrackRequestCreationTime: NotRequired[datetime],
    Status: NotRequired[str],
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

## ParameterOutputTypeDef

```python
# ParameterOutputTypeDef definition

class ParameterOutputTypeDef(TypedDict):
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
    SupportedEngineModes: NotRequired[List[str]],
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

## DBClusterStatusInfoTypeDef

```python
# DBClusterStatusInfoTypeDef definition

class DBClusterStatusInfoTypeDef(TypedDict):
    StatusType: NotRequired[str],
    Normal: NotRequired[bool],
    Status: NotRequired[str],
    Message: NotRequired[str],
```

## DomainMembershipTypeDef

```python
# DomainMembershipTypeDef definition

class DomainMembershipTypeDef(TypedDict):
    Domain: NotRequired[str],
    Status: NotRequired[str],
    FQDN: NotRequired[str],
    IAMRoleName: NotRequired[str],
    OU: NotRequired[str],
    AuthSecretArn: NotRequired[str],
    DnsIps: NotRequired[List[str]],
```

## LimitlessDatabaseTypeDef

```python
# LimitlessDatabaseTypeDef definition

class LimitlessDatabaseTypeDef(TypedDict):
    Status: NotRequired[LimitlessDatabaseStatusType],  # (1)
    MinRequiredACU: NotRequired[float],
```

1. See [:material-code-brackets: LimitlessDatabaseStatusType](./literals.md#limitlessdatabasestatustype) 
## MasterUserSecretTypeDef

```python
# MasterUserSecretTypeDef definition

class MasterUserSecretTypeDef(TypedDict):
    SecretArn: NotRequired[str],
    SecretStatus: NotRequired[str],
    KmsKeyId: NotRequired[str],
```

## ScalingConfigurationInfoTypeDef

```python
# ScalingConfigurationInfoTypeDef definition

class ScalingConfigurationInfoTypeDef(TypedDict):
    MinCapacity: NotRequired[int],
    MaxCapacity: NotRequired[int],
    AutoPause: NotRequired[bool],
    SecondsUntilAutoPause: NotRequired[int],
    TimeoutAction: NotRequired[str],
    SecondsBeforeTimeout: NotRequired[int],
```

## ServerlessV2ScalingConfigurationInfoTypeDef

```python
# ServerlessV2ScalingConfigurationInfoTypeDef definition

class ServerlessV2ScalingConfigurationInfoTypeDef(TypedDict):
    MinCapacity: NotRequired[float],
    MaxCapacity: NotRequired[float],
    SecondsUntilAutoPause: NotRequired[int],
```

## VpcSecurityGroupMembershipTypeDef

```python
# VpcSecurityGroupMembershipTypeDef definition

class VpcSecurityGroupMembershipTypeDef(TypedDict):
    VpcSecurityGroupId: NotRequired[str],
    Status: NotRequired[str],
```

## ServerlessV2FeaturesSupportTypeDef

```python
# ServerlessV2FeaturesSupportTypeDef definition

class ServerlessV2FeaturesSupportTypeDef(TypedDict):
    MinCapacity: NotRequired[float],
    MaxCapacity: NotRequired[float],
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
    SupportedEngineModes: NotRequired[List[str]],
    SupportsParallelQuery: NotRequired[bool],
    SupportsGlobalDatabases: NotRequired[bool],
    SupportsBabelfish: NotRequired[bool],
    SupportsLimitlessDatabase: NotRequired[bool],
    SupportsLocalWriteForwarding: NotRequired[bool],
    SupportsIntegrations: NotRequired[bool],
```

## DBInstanceAutomatedBackupsReplicationTypeDef

```python
# DBInstanceAutomatedBackupsReplicationTypeDef definition

class DBInstanceAutomatedBackupsReplicationTypeDef(TypedDict):
    DBInstanceAutomatedBackupsArn: NotRequired[str],
```

## DBInstanceRoleTypeDef

```python
# DBInstanceRoleTypeDef definition

class DBInstanceRoleTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    FeatureName: NotRequired[str],
    Status: NotRequired[str],
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

## TargetHealthTypeDef

```python
# TargetHealthTypeDef definition

class TargetHealthTypeDef(TypedDict):
    State: NotRequired[TargetStateType],  # (1)
    Reason: NotRequired[TargetHealthReasonType],  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: TargetStateType](./literals.md#targetstatetype) 
2. See [:material-code-brackets: TargetHealthReasonType](./literals.md#targethealthreasontype) 
## UserAuthConfigInfoTypeDef

```python
# UserAuthConfigInfoTypeDef definition

class UserAuthConfigInfoTypeDef(TypedDict):
    Description: NotRequired[str],
    UserName: NotRequired[str],
    AuthScheme: NotRequired[AuthSchemeType],  # (1)
    SecretArn: NotRequired[str],
    IAMAuth: NotRequired[IAMAuthModeType],  # (2)
    ClientPasswordAuthType: NotRequired[ClientPasswordAuthTypeType],  # (3)
```

1. See [:material-code-brackets: AuthSchemeType](./literals.md#authschemetype) 
2. See [:material-code-brackets: IAMAuthModeType](./literals.md#iamauthmodetype) 
3. See [:material-code-brackets: ClientPasswordAuthTypeType](./literals.md#clientpasswordauthtypetype) 
## DocLinkTypeDef

```python
# DocLinkTypeDef definition

class DocLinkTypeDef(TypedDict):
    Text: NotRequired[str],
    Url: NotRequired[str],
```

## EC2SecurityGroupTypeDef

```python
# EC2SecurityGroupTypeDef definition

class EC2SecurityGroupTypeDef(TypedDict):
    Status: NotRequired[str],
    EC2SecurityGroupName: NotRequired[str],
    EC2SecurityGroupId: NotRequired[str],
    EC2SecurityGroupOwnerId: NotRequired[str],
```

## IPRangeTypeDef

```python
# IPRangeTypeDef definition

class IPRangeTypeDef(TypedDict):
    Status: NotRequired[str],
    CIDRIP: NotRequired[str],
```

## DBSnapshotAttributeTypeDef

```python
# DBSnapshotAttributeTypeDef definition

class DBSnapshotAttributeTypeDef(TypedDict):
    AttributeName: NotRequired[str],
    AttributeValues: NotRequired[List[str]],
```

## DeleteBlueGreenDeploymentRequestRequestTypeDef

```python
# DeleteBlueGreenDeploymentRequestRequestTypeDef definition

class DeleteBlueGreenDeploymentRequestRequestTypeDef(TypedDict):
    BlueGreenDeploymentIdentifier: str,
    DeleteTarget: NotRequired[bool],
```

## DeleteCustomDBEngineVersionMessageRequestTypeDef

```python
# DeleteCustomDBEngineVersionMessageRequestTypeDef definition

class DeleteCustomDBEngineVersionMessageRequestTypeDef(TypedDict):
    Engine: str,
    EngineVersion: str,
```

## DeleteDBClusterAutomatedBackupMessageRequestTypeDef

```python
# DeleteDBClusterAutomatedBackupMessageRequestTypeDef definition

class DeleteDBClusterAutomatedBackupMessageRequestTypeDef(TypedDict):
    DbClusterResourceId: str,
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
    DeleteAutomatedBackups: NotRequired[bool],
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

## DeleteDBInstanceAutomatedBackupMessageRequestTypeDef

```python
# DeleteDBInstanceAutomatedBackupMessageRequestTypeDef definition

class DeleteDBInstanceAutomatedBackupMessageRequestTypeDef(TypedDict):
    DbiResourceId: NotRequired[str],
    DBInstanceAutomatedBackupsArn: NotRequired[str],
```

## DeleteDBInstanceMessageRequestTypeDef

```python
# DeleteDBInstanceMessageRequestTypeDef definition

class DeleteDBInstanceMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    SkipFinalSnapshot: NotRequired[bool],
    FinalDBSnapshotIdentifier: NotRequired[str],
    DeleteAutomatedBackups: NotRequired[bool],
```

## DeleteDBParameterGroupMessageRequestTypeDef

```python
# DeleteDBParameterGroupMessageRequestTypeDef definition

class DeleteDBParameterGroupMessageRequestTypeDef(TypedDict):
    DBParameterGroupName: str,
```

## DeleteDBProxyEndpointRequestRequestTypeDef

```python
# DeleteDBProxyEndpointRequestRequestTypeDef definition

class DeleteDBProxyEndpointRequestRequestTypeDef(TypedDict):
    DBProxyEndpointName: str,
```

## DeleteDBProxyRequestRequestTypeDef

```python
# DeleteDBProxyRequestRequestTypeDef definition

class DeleteDBProxyRequestRequestTypeDef(TypedDict):
    DBProxyName: str,
```

## DeleteDBSecurityGroupMessageRequestTypeDef

```python
# DeleteDBSecurityGroupMessageRequestTypeDef definition

class DeleteDBSecurityGroupMessageRequestTypeDef(TypedDict):
    DBSecurityGroupName: str,
```

## DeleteDBShardGroupMessageRequestTypeDef

```python
# DeleteDBShardGroupMessageRequestTypeDef definition

class DeleteDBShardGroupMessageRequestTypeDef(TypedDict):
    DBShardGroupIdentifier: str,
```

## DeleteDBSnapshotMessageRequestTypeDef

```python
# DeleteDBSnapshotMessageRequestTypeDef definition

class DeleteDBSnapshotMessageRequestTypeDef(TypedDict):
    DBSnapshotIdentifier: str,
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

## DeleteIntegrationMessageRequestTypeDef

```python
# DeleteIntegrationMessageRequestTypeDef definition

class DeleteIntegrationMessageRequestTypeDef(TypedDict):
    IntegrationIdentifier: str,
```

## DeleteOptionGroupMessageRequestTypeDef

```python
# DeleteOptionGroupMessageRequestTypeDef definition

class DeleteOptionGroupMessageRequestTypeDef(TypedDict):
    OptionGroupName: str,
```

## DeleteTenantDatabaseMessageRequestTypeDef

```python
# DeleteTenantDatabaseMessageRequestTypeDef definition

class DeleteTenantDatabaseMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    TenantDBName: str,
    SkipFinalSnapshot: NotRequired[bool],
    FinalDBSnapshotIdentifier: NotRequired[str],
```

## DeregisterDBProxyTargetsRequestRequestTypeDef

```python
# DeregisterDBProxyTargetsRequestRequestTypeDef definition

class DeregisterDBProxyTargetsRequestRequestTypeDef(TypedDict):
    DBProxyName: str,
    TargetGroupName: NotRequired[str],
    DBInstanceIdentifiers: NotRequired[Sequence[str]],
    DBClusterIdentifiers: NotRequired[Sequence[str]],
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

## DescribeDBLogFilesDetailsTypeDef

```python
# DescribeDBLogFilesDetailsTypeDef definition

class DescribeDBLogFilesDetailsTypeDef(TypedDict):
    LogFileName: NotRequired[str],
    LastWritten: NotRequired[int],
    Size: NotRequired[int],
```

## DescribeDBSnapshotAttributesMessageRequestTypeDef

```python
# DescribeDBSnapshotAttributesMessageRequestTypeDef definition

class DescribeDBSnapshotAttributesMessageRequestTypeDef(TypedDict):
    DBSnapshotIdentifier: str,
```

## DescribeValidDBInstanceModificationsMessageRequestTypeDef

```python
# DescribeValidDBInstanceModificationsMessageRequestTypeDef definition

class DescribeValidDBInstanceModificationsMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
```

## DisableHttpEndpointRequestRequestTypeDef

```python
# DisableHttpEndpointRequestRequestTypeDef definition

class DisableHttpEndpointRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DoubleRangeTypeDef

```python
# DoubleRangeTypeDef definition

class DoubleRangeTypeDef(TypedDict):
    From: NotRequired[float],
    To: NotRequired[float],
```

## DownloadDBLogFilePortionMessageRequestTypeDef

```python
# DownloadDBLogFilePortionMessageRequestTypeDef definition

class DownloadDBLogFilePortionMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    LogFileName: str,
    Marker: NotRequired[str],
    NumberOfLines: NotRequired[int],
```

## EnableHttpEndpointRequestRequestTypeDef

```python
# EnableHttpEndpointRequestRequestTypeDef definition

class EnableHttpEndpointRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
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
## ExportTaskTypeDef

```python
# ExportTaskTypeDef definition

class ExportTaskTypeDef(TypedDict):
    ExportTaskIdentifier: NotRequired[str],
    SourceArn: NotRequired[str],
    ExportOnly: NotRequired[List[str]],
    SnapshotTime: NotRequired[datetime],
    TaskStartTime: NotRequired[datetime],
    TaskEndTime: NotRequired[datetime],
    S3Bucket: NotRequired[str],
    S3Prefix: NotRequired[str],
    IamRoleArn: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Status: NotRequired[str],
    PercentProgress: NotRequired[int],
    TotalExtractedDataInGB: NotRequired[int],
    FailureCause: NotRequired[str],
    WarningMessage: NotRequired[str],
    SourceType: NotRequired[ExportSourceTypeType],  # (1)
```

1. See [:material-code-brackets: ExportSourceTypeType](./literals.md#exportsourcetypetype) 
## FailoverDBClusterMessageRequestTypeDef

```python
# FailoverDBClusterMessageRequestTypeDef definition

class FailoverDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    TargetDBInstanceIdentifier: NotRequired[str],
```

## FailoverGlobalClusterMessageRequestTypeDef

```python
# FailoverGlobalClusterMessageRequestTypeDef definition

class FailoverGlobalClusterMessageRequestTypeDef(TypedDict):
    GlobalClusterIdentifier: str,
    TargetDbClusterIdentifier: str,
    AllowDataLoss: NotRequired[bool],
    Switchover: NotRequired[bool],
```

## FailoverStateTypeDef

```python
# FailoverStateTypeDef definition

class FailoverStateTypeDef(TypedDict):
    Status: NotRequired[FailoverStatusType],  # (1)
    FromDbClusterArn: NotRequired[str],
    ToDbClusterArn: NotRequired[str],
    IsDataLossAllowed: NotRequired[bool],
```

1. See [:material-code-brackets: FailoverStatusType](./literals.md#failoverstatustype) 
## GlobalClusterMemberTypeDef

```python
# GlobalClusterMemberTypeDef definition

class GlobalClusterMemberTypeDef(TypedDict):
    DBClusterArn: NotRequired[str],
    Readers: NotRequired[List[str]],
    IsWriter: NotRequired[bool],
    GlobalWriteForwardingStatus: NotRequired[WriteForwardingStatusType],  # (1)
    SynchronizationStatus: NotRequired[GlobalClusterMemberSynchronizationStatusType],  # (2)
```

1. See [:material-code-brackets: WriteForwardingStatusType](./literals.md#writeforwardingstatustype) 
2. See [:material-code-brackets: GlobalClusterMemberSynchronizationStatusType](./literals.md#globalclustermembersynchronizationstatustype) 
## IntegrationErrorTypeDef

```python
# IntegrationErrorTypeDef definition

class IntegrationErrorTypeDef(TypedDict):
    ErrorCode: str,
    ErrorMessage: NotRequired[str],
```

## MinimumEngineVersionPerAllowedValueTypeDef

```python
# MinimumEngineVersionPerAllowedValueTypeDef definition

class MinimumEngineVersionPerAllowedValueTypeDef(TypedDict):
    AllowedValue: NotRequired[str],
    MinimumEngineVersion: NotRequired[str],
```

## ModifyActivityStreamRequestRequestTypeDef

```python
# ModifyActivityStreamRequestRequestTypeDef definition

class ModifyActivityStreamRequestRequestTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    AuditPolicyState: NotRequired[AuditPolicyStateType],  # (1)
```

1. See [:material-code-brackets: AuditPolicyStateType](./literals.md#auditpolicystatetype) 
## ModifyCertificatesMessageRequestTypeDef

```python
# ModifyCertificatesMessageRequestTypeDef definition

class ModifyCertificatesMessageRequestTypeDef(TypedDict):
    CertificateIdentifier: NotRequired[str],
    RemoveCustomerOverride: NotRequired[bool],
```

## ModifyCurrentDBClusterCapacityMessageRequestTypeDef

```python
# ModifyCurrentDBClusterCapacityMessageRequestTypeDef definition

class ModifyCurrentDBClusterCapacityMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    Capacity: NotRequired[int],
    SecondsBeforeTimeout: NotRequired[int],
    TimeoutAction: NotRequired[str],
```

## ModifyCustomDBEngineVersionMessageRequestTypeDef

```python
# ModifyCustomDBEngineVersionMessageRequestTypeDef definition

class ModifyCustomDBEngineVersionMessageRequestTypeDef(TypedDict):
    Engine: str,
    EngineVersion: str,
    Description: NotRequired[str],
    Status: NotRequired[CustomEngineVersionStatusType],  # (1)
```

1. See [:material-code-brackets: CustomEngineVersionStatusType](./literals.md#customengineversionstatustype) 
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
    SupportedEngineModes: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ApplyMethodType](./literals.md#applymethodtype) 
## ModifyDBProxyEndpointRequestRequestTypeDef

```python
# ModifyDBProxyEndpointRequestRequestTypeDef definition

class ModifyDBProxyEndpointRequestRequestTypeDef(TypedDict):
    DBProxyEndpointName: str,
    NewDBProxyEndpointName: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
```

## RecommendedActionUpdateTypeDef

```python
# RecommendedActionUpdateTypeDef definition

class RecommendedActionUpdateTypeDef(TypedDict):
    ActionId: str,
    Status: str,
```

## ModifyDBShardGroupMessageRequestTypeDef

```python
# ModifyDBShardGroupMessageRequestTypeDef definition

class ModifyDBShardGroupMessageRequestTypeDef(TypedDict):
    DBShardGroupIdentifier: str,
    MaxACU: NotRequired[float],
    MinACU: NotRequired[float],
    ComputeRedundancy: NotRequired[int],
```

## ModifyDBSnapshotAttributeMessageRequestTypeDef

```python
# ModifyDBSnapshotAttributeMessageRequestTypeDef definition

class ModifyDBSnapshotAttributeMessageRequestTypeDef(TypedDict):
    DBSnapshotIdentifier: str,
    AttributeName: str,
    ValuesToAdd: NotRequired[Sequence[str]],
    ValuesToRemove: NotRequired[Sequence[str]],
```

## ModifyDBSnapshotMessageRequestTypeDef

```python
# ModifyDBSnapshotMessageRequestTypeDef definition

class ModifyDBSnapshotMessageRequestTypeDef(TypedDict):
    DBSnapshotIdentifier: str,
    EngineVersion: NotRequired[str],
    OptionGroupName: NotRequired[str],
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
    GlobalClusterIdentifier: NotRequired[str],
    NewGlobalClusterIdentifier: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    EngineVersion: NotRequired[str],
    AllowMajorVersionUpgrade: NotRequired[bool],
```

## ModifyIntegrationMessageRequestTypeDef

```python
# ModifyIntegrationMessageRequestTypeDef definition

class ModifyIntegrationMessageRequestTypeDef(TypedDict):
    IntegrationIdentifier: str,
    IntegrationName: NotRequired[str],
    DataFilter: NotRequired[str],
    Description: NotRequired[str],
```

## ModifyTenantDatabaseMessageRequestTypeDef

```python
# ModifyTenantDatabaseMessageRequestTypeDef definition

class ModifyTenantDatabaseMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    TenantDBName: str,
    MasterUserPassword: NotRequired[str],
    NewTenantDBName: NotRequired[str],
```

## OptionSettingTypeDef

```python
# OptionSettingTypeDef definition

class OptionSettingTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
    DefaultValue: NotRequired[str],
    Description: NotRequired[str],
    ApplyType: NotRequired[str],
    DataType: NotRequired[str],
    AllowedValues: NotRequired[str],
    IsModifiable: NotRequired[bool],
    IsCollection: NotRequired[bool],
```

## OptionVersionTypeDef

```python
# OptionVersionTypeDef definition

class OptionVersionTypeDef(TypedDict):
    Version: NotRequired[str],
    IsDefault: NotRequired[bool],
```

## OutpostTypeDef

```python
# OutpostTypeDef definition

class OutpostTypeDef(TypedDict):
    Arn: NotRequired[str],
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

## PerformanceInsightsMetricDimensionGroupTypeDef

```python
# PerformanceInsightsMetricDimensionGroupTypeDef definition

class PerformanceInsightsMetricDimensionGroupTypeDef(TypedDict):
    Dimensions: NotRequired[List[str]],
    Group: NotRequired[str],
    Limit: NotRequired[int],
```

## PromoteReadReplicaDBClusterMessageRequestTypeDef

```python
# PromoteReadReplicaDBClusterMessageRequestTypeDef definition

class PromoteReadReplicaDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
```

## PromoteReadReplicaMessageRequestTypeDef

```python
# PromoteReadReplicaMessageRequestTypeDef definition

class PromoteReadReplicaMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    BackupRetentionPeriod: NotRequired[int],
    PreferredBackupWindow: NotRequired[str],
```

## RangeTypeDef

```python
# RangeTypeDef definition

class RangeTypeDef(TypedDict):
    From: NotRequired[int],
    To: NotRequired[int],
    Step: NotRequired[int],
```

## RebootDBClusterMessageRequestTypeDef

```python
# RebootDBClusterMessageRequestTypeDef definition

class RebootDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
```

## RebootDBInstanceMessageRequestTypeDef

```python
# RebootDBInstanceMessageRequestTypeDef definition

class RebootDBInstanceMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    ForceFailover: NotRequired[bool],
```

## RebootDBShardGroupMessageRequestTypeDef

```python
# RebootDBShardGroupMessageRequestTypeDef definition

class RebootDBShardGroupMessageRequestTypeDef(TypedDict):
    DBShardGroupIdentifier: str,
```

## RecommendedActionParameterTypeDef

```python
# RecommendedActionParameterTypeDef definition

class RecommendedActionParameterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## RecurringChargeTypeDef

```python
# RecurringChargeTypeDef definition

class RecurringChargeTypeDef(TypedDict):
    RecurringChargeAmount: NotRequired[float],
    RecurringChargeFrequency: NotRequired[str],
```

## ScalarReferenceDetailsTypeDef

```python
# ScalarReferenceDetailsTypeDef definition

class ScalarReferenceDetailsTypeDef(TypedDict):
    Value: NotRequired[float],
```

## RegisterDBProxyTargetsRequestRequestTypeDef

```python
# RegisterDBProxyTargetsRequestRequestTypeDef definition

class RegisterDBProxyTargetsRequestRequestTypeDef(TypedDict):
    DBProxyName: str,
    TargetGroupName: NotRequired[str],
    DBInstanceIdentifiers: NotRequired[Sequence[str]],
    DBClusterIdentifiers: NotRequired[Sequence[str]],
```

## RemoveFromGlobalClusterMessageRequestTypeDef

```python
# RemoveFromGlobalClusterMessageRequestTypeDef definition

class RemoveFromGlobalClusterMessageRequestTypeDef(TypedDict):
    GlobalClusterIdentifier: NotRequired[str],
    DbClusterIdentifier: NotRequired[str],
```

## RemoveRoleFromDBClusterMessageRequestTypeDef

```python
# RemoveRoleFromDBClusterMessageRequestTypeDef definition

class RemoveRoleFromDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    RoleArn: str,
    FeatureName: NotRequired[str],
```

## RemoveRoleFromDBInstanceMessageRequestTypeDef

```python
# RemoveRoleFromDBInstanceMessageRequestTypeDef definition

class RemoveRoleFromDBInstanceMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    RoleArn: str,
    FeatureName: str,
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

## RevokeDBSecurityGroupIngressMessageRequestTypeDef

```python
# RevokeDBSecurityGroupIngressMessageRequestTypeDef definition

class RevokeDBSecurityGroupIngressMessageRequestTypeDef(TypedDict):
    DBSecurityGroupName: str,
    CIDRIP: NotRequired[str],
    EC2SecurityGroupName: NotRequired[str],
    EC2SecurityGroupId: NotRequired[str],
    EC2SecurityGroupOwnerId: NotRequired[str],
```

## SourceRegionTypeDef

```python
# SourceRegionTypeDef definition

class SourceRegionTypeDef(TypedDict):
    RegionName: NotRequired[str],
    Endpoint: NotRequired[str],
    Status: NotRequired[str],
    SupportsDBInstanceAutomatedBackupsReplication: NotRequired[bool],
```

## StartActivityStreamRequestRequestTypeDef

```python
# StartActivityStreamRequestRequestTypeDef definition

class StartActivityStreamRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Mode: ActivityStreamModeType,  # (1)
    KmsKeyId: str,
    ApplyImmediately: NotRequired[bool],
    EngineNativeAuditFieldsIncluded: NotRequired[bool],
```

1. See [:material-code-brackets: ActivityStreamModeType](./literals.md#activitystreammodetype) 
## StartDBClusterMessageRequestTypeDef

```python
# StartDBClusterMessageRequestTypeDef definition

class StartDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
```

## StartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef

```python
# StartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef definition

class StartDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef(TypedDict):
    SourceDBInstanceArn: str,
    BackupRetentionPeriod: NotRequired[int],
    KmsKeyId: NotRequired[str],
    PreSignedUrl: NotRequired[str],
    SourceRegion: NotRequired[str],
```

## StartDBInstanceMessageRequestTypeDef

```python
# StartDBInstanceMessageRequestTypeDef definition

class StartDBInstanceMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
```

## StartExportTaskMessageRequestTypeDef

```python
# StartExportTaskMessageRequestTypeDef definition

class StartExportTaskMessageRequestTypeDef(TypedDict):
    ExportTaskIdentifier: str,
    SourceArn: str,
    S3BucketName: str,
    IamRoleArn: str,
    KmsKeyId: str,
    S3Prefix: NotRequired[str],
    ExportOnly: NotRequired[Sequence[str]],
```

## StopActivityStreamRequestRequestTypeDef

```python
# StopActivityStreamRequestRequestTypeDef definition

class StopActivityStreamRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    ApplyImmediately: NotRequired[bool],
```

## StopDBClusterMessageRequestTypeDef

```python
# StopDBClusterMessageRequestTypeDef definition

class StopDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
```

## StopDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef

```python
# StopDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef definition

class StopDBInstanceAutomatedBackupsReplicationMessageRequestTypeDef(TypedDict):
    SourceDBInstanceArn: str,
```

## StopDBInstanceMessageRequestTypeDef

```python
# StopDBInstanceMessageRequestTypeDef definition

class StopDBInstanceMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    DBSnapshotIdentifier: NotRequired[str],
```

## SwitchoverBlueGreenDeploymentRequestRequestTypeDef

```python
# SwitchoverBlueGreenDeploymentRequestRequestTypeDef definition

class SwitchoverBlueGreenDeploymentRequestRequestTypeDef(TypedDict):
    BlueGreenDeploymentIdentifier: str,
    SwitchoverTimeout: NotRequired[int],
```

## SwitchoverGlobalClusterMessageRequestTypeDef

```python
# SwitchoverGlobalClusterMessageRequestTypeDef definition

class SwitchoverGlobalClusterMessageRequestTypeDef(TypedDict):
    GlobalClusterIdentifier: str,
    TargetDbClusterIdentifier: str,
```

## SwitchoverReadReplicaMessageRequestTypeDef

```python
# SwitchoverReadReplicaMessageRequestTypeDef definition

class SwitchoverReadReplicaMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
```

## TenantDatabasePendingModifiedValuesTypeDef

```python
# TenantDatabasePendingModifiedValuesTypeDef definition

class TenantDatabasePendingModifiedValuesTypeDef(TypedDict):
    MasterUserPassword: NotRequired[str],
    TenantDBName: NotRequired[str],
```

## AccountAttributesMessageTypeDef

```python
# AccountAttributesMessageTypeDef definition

class AccountAttributesMessageTypeDef(TypedDict):
    AccountQuotas: List[AccountQuotaTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountQuotaTypeDef](./type_defs.md#accountquotatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBClusterBacktrackResponseTypeDef

```python
# DBClusterBacktrackResponseTypeDef definition

class DBClusterBacktrackResponseTypeDef(TypedDict):
    DBClusterIdentifier: str,
    BacktrackIdentifier: str,
    BacktrackTo: datetime,
    BacktrackedFrom: datetime,
    BacktrackRequestCreationTime: datetime,
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBClusterCapacityInfoTypeDef

```python
# DBClusterCapacityInfoTypeDef definition

class DBClusterCapacityInfoTypeDef(TypedDict):
    DBClusterIdentifier: str,
    PendingCapacity: int,
    CurrentCapacity: int,
    SecondsBeforeTimeout: int,
    TimeoutAction: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBClusterEndpointResponseTypeDef

```python
# DBClusterEndpointResponseTypeDef definition

class DBClusterEndpointResponseTypeDef(TypedDict):
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
## DisableHttpEndpointResponseTypeDef

```python
# DisableHttpEndpointResponseTypeDef definition

class DisableHttpEndpointResponseTypeDef(TypedDict):
    ResourceArn: str,
    HttpEndpointEnabled: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DownloadDBLogFilePortionDetailsTypeDef

```python
# DownloadDBLogFilePortionDetailsTypeDef definition

class DownloadDBLogFilePortionDetailsTypeDef(TypedDict):
    LogFileData: str,
    Marker: str,
    AdditionalDataPending: bool,
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
## EnableHttpEndpointResponseTypeDef

```python
# EnableHttpEndpointResponseTypeDef definition

class EnableHttpEndpointResponseTypeDef(TypedDict):
    ResourceArn: str,
    HttpEndpointEnabled: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportTaskResponseTypeDef

```python
# ExportTaskResponseTypeDef definition

class ExportTaskResponseTypeDef(TypedDict):
    ExportTaskIdentifier: str,
    SourceArn: str,
    ExportOnly: List[str],
    SnapshotTime: datetime,
    TaskStartTime: datetime,
    TaskEndTime: datetime,
    S3Bucket: str,
    S3Prefix: str,
    IamRoleArn: str,
    KmsKeyId: str,
    Status: str,
    PercentProgress: int,
    TotalExtractedDataInGB: int,
    FailureCause: str,
    WarningMessage: str,
    SourceType: ExportSourceTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ExportSourceTypeType](./literals.md#exportsourcetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyActivityStreamResponseTypeDef

```python
# ModifyActivityStreamResponseTypeDef definition

class ModifyActivityStreamResponseTypeDef(TypedDict):
    KmsKeyId: str,
    KinesisStreamName: str,
    Status: ActivityStreamStatusType,  # (1)
    Mode: ActivityStreamModeType,  # (2)
    EngineNativeAuditFieldsIncluded: bool,
    PolicyStatus: ActivityStreamPolicyStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ActivityStreamStatusType](./literals.md#activitystreamstatustype) 
2. See [:material-code-brackets: ActivityStreamModeType](./literals.md#activitystreammodetype) 
3. See [:material-code-brackets: ActivityStreamPolicyStatusType](./literals.md#activitystreampolicystatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartActivityStreamResponseTypeDef

```python
# StartActivityStreamResponseTypeDef definition

class StartActivityStreamResponseTypeDef(TypedDict):
    KmsKeyId: str,
    KinesisStreamName: str,
    Status: ActivityStreamStatusType,  # (1)
    Mode: ActivityStreamModeType,  # (2)
    ApplyImmediately: bool,
    EngineNativeAuditFieldsIncluded: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ActivityStreamStatusType](./literals.md#activitystreamstatustype) 
2. See [:material-code-brackets: ActivityStreamModeType](./literals.md#activitystreammodetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopActivityStreamResponseTypeDef

```python
# StopActivityStreamResponseTypeDef definition

class StopActivityStreamResponseTypeDef(TypedDict):
    KmsKeyId: str,
    KinesisStreamName: str,
    Status: ActivityStreamStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ActivityStreamStatusType](./literals.md#activitystreamstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddSourceIdentifierToSubscriptionResultTypeDef

```python
# AddSourceIdentifierToSubscriptionResultTypeDef definition

class AddSourceIdentifierToSubscriptionResultTypeDef(TypedDict):
    EventSubscription: EventSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEventSubscriptionResultTypeDef

```python
# CreateEventSubscriptionResultTypeDef definition

class CreateEventSubscriptionResultTypeDef(TypedDict):
    EventSubscription: EventSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEventSubscriptionResultTypeDef

```python
# DeleteEventSubscriptionResultTypeDef definition

class DeleteEventSubscriptionResultTypeDef(TypedDict):
    EventSubscription: EventSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSubscriptionTypeDef](./type_defs.md#eventsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## CopyDBSnapshotMessageRequestTypeDef

```python
# CopyDBSnapshotMessageRequestTypeDef definition

class CopyDBSnapshotMessageRequestTypeDef(TypedDict):
    SourceDBSnapshotIdentifier: str,
    TargetDBSnapshotIdentifier: str,
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    CopyTags: NotRequired[bool],
    PreSignedUrl: NotRequired[str],
    OptionGroupName: NotRequired[str],
    TargetCustomAvailabilityZone: NotRequired[str],
    CopyOptionGroup: NotRequired[bool],
    SourceRegion: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CopyOptionGroupMessageRequestTypeDef

```python
# CopyOptionGroupMessageRequestTypeDef definition

class CopyOptionGroupMessageRequestTypeDef(TypedDict):
    SourceOptionGroupIdentifier: str,
    TargetOptionGroupIdentifier: str,
    TargetOptionGroupDescription: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateBlueGreenDeploymentRequestRequestTypeDef

```python
# CreateBlueGreenDeploymentRequestRequestTypeDef definition

class CreateBlueGreenDeploymentRequestRequestTypeDef(TypedDict):
    BlueGreenDeploymentName: str,
    Source: str,
    TargetEngineVersion: NotRequired[str],
    TargetDBParameterGroupName: NotRequired[str],
    TargetDBClusterParameterGroupName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    TargetDBInstanceClass: NotRequired[str],
    UpgradeTargetStorageConfig: NotRequired[bool],
    TargetIops: NotRequired[int],
    TargetStorageType: NotRequired[str],
    TargetAllocatedStorage: NotRequired[int],
    TargetStorageThroughput: NotRequired[int],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCustomDBEngineVersionMessageRequestTypeDef

```python
# CreateCustomDBEngineVersionMessageRequestTypeDef definition

class CreateCustomDBEngineVersionMessageRequestTypeDef(TypedDict):
    Engine: str,
    EngineVersion: str,
    DatabaseInstallationFilesS3BucketName: NotRequired[str],
    DatabaseInstallationFilesS3Prefix: NotRequired[str],
    ImageId: NotRequired[str],
    KMSKeyId: NotRequired[str],
    Description: NotRequired[str],
    Manifest: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    SourceCustomDbEngineVersionIdentifier: NotRequired[str],
    UseAwsProvidedLatestImage: NotRequired[bool],
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
## CreateDBProxyEndpointRequestRequestTypeDef

```python
# CreateDBProxyEndpointRequestRequestTypeDef definition

class CreateDBProxyEndpointRequestRequestTypeDef(TypedDict):
    DBProxyName: str,
    DBProxyEndpointName: str,
    VpcSubnetIds: Sequence[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    TargetRole: NotRequired[DBProxyEndpointTargetRoleType],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: DBProxyEndpointTargetRoleType](./literals.md#dbproxyendpointtargetroletype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDBSecurityGroupMessageRequestTypeDef

```python
# CreateDBSecurityGroupMessageRequestTypeDef definition

class CreateDBSecurityGroupMessageRequestTypeDef(TypedDict):
    DBSecurityGroupName: str,
    DBSecurityGroupDescription: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDBShardGroupMessageRequestTypeDef

```python
# CreateDBShardGroupMessageRequestTypeDef definition

class CreateDBShardGroupMessageRequestTypeDef(TypedDict):
    DBShardGroupIdentifier: str,
    DBClusterIdentifier: str,
    MaxACU: float,
    ComputeRedundancy: NotRequired[int],
    MinACU: NotRequired[float],
    PubliclyAccessible: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDBSnapshotMessageRequestTypeDef

```python
# CreateDBSnapshotMessageRequestTypeDef definition

class CreateDBSnapshotMessageRequestTypeDef(TypedDict):
    DBSnapshotIdentifier: str,
    DBInstanceIdentifier: str,
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
## CreateGlobalClusterMessageRequestTypeDef

```python
# CreateGlobalClusterMessageRequestTypeDef definition

class CreateGlobalClusterMessageRequestTypeDef(TypedDict):
    GlobalClusterIdentifier: NotRequired[str],
    SourceDBClusterIdentifier: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    EngineLifecycleSupport: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    DatabaseName: NotRequired[str],
    StorageEncrypted: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateIntegrationMessageRequestTypeDef

```python
# CreateIntegrationMessageRequestTypeDef definition

class CreateIntegrationMessageRequestTypeDef(TypedDict):
    SourceArn: str,
    TargetArn: str,
    IntegrationName: str,
    KMSKeyId: NotRequired[str],
    AdditionalEncryptionContext: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    DataFilter: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateOptionGroupMessageRequestTypeDef

```python
# CreateOptionGroupMessageRequestTypeDef definition

class CreateOptionGroupMessageRequestTypeDef(TypedDict):
    OptionGroupName: str,
    EngineName: str,
    MajorEngineVersion: str,
    OptionGroupDescription: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTenantDatabaseMessageRequestTypeDef

```python
# CreateTenantDatabaseMessageRequestTypeDef definition

class CreateTenantDatabaseMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    TenantDBName: str,
    MasterUsername: str,
    MasterUserPassword: str,
    CharacterSetName: NotRequired[str],
    NcharCharacterSetName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DBClusterSnapshotTypeDef

```python
# DBClusterSnapshotTypeDef definition

class DBClusterSnapshotTypeDef(TypedDict):
    AvailabilityZones: NotRequired[List[str]],
    DBClusterSnapshotIdentifier: NotRequired[str],
    DBClusterIdentifier: NotRequired[str],
    SnapshotCreateTime: NotRequired[datetime],
    Engine: NotRequired[str],
    EngineMode: NotRequired[str],
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
    TagList: NotRequired[List[TagTypeDef]],  # (1)
    DBSystemId: NotRequired[str],
    StorageType: NotRequired[str],
    DbClusterResourceId: NotRequired[str],
    StorageThroughput: NotRequired[int],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DBShardGroupResponseTypeDef

```python
# DBShardGroupResponseTypeDef definition

class DBShardGroupResponseTypeDef(TypedDict):
    DBShardGroupResourceId: str,
    DBShardGroupIdentifier: str,
    DBClusterIdentifier: str,
    MaxACU: float,
    MinACU: float,
    ComputeRedundancy: int,
    Status: str,
    PubliclyAccessible: bool,
    Endpoint: str,
    DBShardGroupArn: str,
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBShardGroupTypeDef

```python
# DBShardGroupTypeDef definition

class DBShardGroupTypeDef(TypedDict):
    DBShardGroupResourceId: NotRequired[str],
    DBShardGroupIdentifier: NotRequired[str],
    DBClusterIdentifier: NotRequired[str],
    MaxACU: NotRequired[float],
    MinACU: NotRequired[float],
    ComputeRedundancy: NotRequired[int],
    Status: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    Endpoint: NotRequired[str],
    DBShardGroupArn: NotRequired[str],
    TagList: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DBSnapshotTenantDatabaseTypeDef

```python
# DBSnapshotTenantDatabaseTypeDef definition

class DBSnapshotTenantDatabaseTypeDef(TypedDict):
    DBSnapshotIdentifier: NotRequired[str],
    DBInstanceIdentifier: NotRequired[str],
    DbiResourceId: NotRequired[str],
    EngineName: NotRequired[str],
    SnapshotType: NotRequired[str],
    TenantDatabaseCreateTime: NotRequired[datetime],
    TenantDBName: NotRequired[str],
    MasterUsername: NotRequired[str],
    TenantDatabaseResourceId: NotRequired[str],
    CharacterSetName: NotRequired[str],
    DBSnapshotTenantDatabaseARN: NotRequired[str],
    NcharCharacterSetName: NotRequired[str],
    TagList: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PurchaseReservedDBInstancesOfferingMessageRequestTypeDef

```python
# PurchaseReservedDBInstancesOfferingMessageRequestTypeDef definition

class PurchaseReservedDBInstancesOfferingMessageRequestTypeDef(TypedDict):
    ReservedDBInstancesOfferingId: str,
    ReservedDBInstanceId: NotRequired[str],
    DBInstanceCount: NotRequired[int],
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
    AvailabilityZoneGroup: NotRequired[str],
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
    AvailableProcessorFeatures: NotRequired[List[AvailableProcessorFeatureTypeDef]],  # (2)
    SupportedEngineModes: NotRequired[List[str]],
    SupportsStorageAutoscaling: NotRequired[bool],
    SupportsKerberosAuthentication: NotRequired[bool],
    OutpostCapable: NotRequired[bool],
    SupportedActivityStreamModes: NotRequired[List[str]],
    SupportsGlobalDatabases: NotRequired[bool],
    SupportsClusters: NotRequired[bool],
    SupportedNetworkTypes: NotRequired[List[str]],
    SupportsStorageThroughput: NotRequired[bool],
    MinStorageThroughputPerDbInstance: NotRequired[int],
    MaxStorageThroughputPerDbInstance: NotRequired[int],
    MinStorageThroughputPerIops: NotRequired[float],
    MaxStorageThroughputPerIops: NotRequired[float],
    SupportsDedicatedLogVolume: NotRequired[bool],
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
2. See [:material-code-braces: AvailableProcessorFeatureTypeDef](./type_defs.md#availableprocessorfeaturetypedef) 
## BacktrackDBClusterMessageRequestTypeDef

```python
# BacktrackDBClusterMessageRequestTypeDef definition

class BacktrackDBClusterMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    BacktrackTo: TimestampTypeDef,
    Force: NotRequired[bool],
    UseEarliestTimeOnPointInTimeUnavailable: NotRequired[bool],
```

## BlueGreenDeploymentTypeDef

```python
# BlueGreenDeploymentTypeDef definition

class BlueGreenDeploymentTypeDef(TypedDict):
    BlueGreenDeploymentIdentifier: NotRequired[str],
    BlueGreenDeploymentName: NotRequired[str],
    Source: NotRequired[str],
    Target: NotRequired[str],
    SwitchoverDetails: NotRequired[List[SwitchoverDetailTypeDef]],  # (1)
    Tasks: NotRequired[List[BlueGreenDeploymentTaskTypeDef]],  # (2)
    Status: NotRequired[str],
    StatusDetails: NotRequired[str],
    CreateTime: NotRequired[datetime],
    DeleteTime: NotRequired[datetime],
    TagList: NotRequired[List[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: SwitchoverDetailTypeDef](./type_defs.md#switchoverdetailtypedef) 
2. See [:material-code-braces: BlueGreenDeploymentTaskTypeDef](./type_defs.md#bluegreendeploymenttasktypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CertificateMessageTypeDef

```python
# CertificateMessageTypeDef definition

class CertificateMessageTypeDef(TypedDict):
    DefaultCertificateForNewLaunches: str,
    Certificates: List[CertificateTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyCertificatesResultTypeDef

```python
# ModifyCertificatesResultTypeDef definition

class ModifyCertificatesResultTypeDef(TypedDict):
    Certificate: CertificateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterPendingModifiedValuesTypeDef

```python
# ClusterPendingModifiedValuesTypeDef definition

class ClusterPendingModifiedValuesTypeDef(TypedDict):
    PendingCloudwatchLogsExports: NotRequired[PendingCloudwatchLogsExportsTypeDef],  # (1)
    DBClusterIdentifier: NotRequired[str],
    MasterUserPassword: NotRequired[str],
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    EngineVersion: NotRequired[str],
    BackupRetentionPeriod: NotRequired[int],
    AllocatedStorage: NotRequired[int],
    RdsCustomClusterConfiguration: NotRequired[RdsCustomClusterConfigurationTypeDef],  # (2)
    Iops: NotRequired[int],
    StorageType: NotRequired[str],
    CertificateDetails: NotRequired[CertificateDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: PendingCloudwatchLogsExportsTypeDef](./type_defs.md#pendingcloudwatchlogsexportstypedef) 
2. See [:material-code-braces: RdsCustomClusterConfigurationTypeDef](./type_defs.md#rdscustomclusterconfigurationtypedef) 
3. See [:material-code-braces: CertificateDetailsTypeDef](./type_defs.md#certificatedetailstypedef) 
## DBProxyTargetGroupTypeDef

```python
# DBProxyTargetGroupTypeDef definition

class DBProxyTargetGroupTypeDef(TypedDict):
    DBProxyName: NotRequired[str],
    TargetGroupName: NotRequired[str],
    TargetGroupArn: NotRequired[str],
    IsDefault: NotRequired[bool],
    Status: NotRequired[str],
    ConnectionPoolConfig: NotRequired[ConnectionPoolConfigurationInfoTypeDef],  # (1)
    CreatedDate: NotRequired[datetime],
    UpdatedDate: NotRequired[datetime],
```

1. See [:material-code-braces: ConnectionPoolConfigurationInfoTypeDef](./type_defs.md#connectionpoolconfigurationinfotypedef) 
## ModifyDBProxyTargetGroupRequestRequestTypeDef

```python
# ModifyDBProxyTargetGroupRequestRequestTypeDef definition

class ModifyDBProxyTargetGroupRequestRequestTypeDef(TypedDict):
    TargetGroupName: str,
    DBProxyName: str,
    ConnectionPoolConfig: NotRequired[ConnectionPoolConfigurationTypeDef],  # (1)
    NewName: NotRequired[str],
```

1. See [:material-code-braces: ConnectionPoolConfigurationTypeDef](./type_defs.md#connectionpoolconfigurationtypedef) 
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
    BacktrackWindow: NotRequired[int],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    EngineMode: NotRequired[str],
    ScalingConfiguration: NotRequired[ScalingConfigurationTypeDef],  # (2)
    RdsCustomClusterConfiguration: NotRequired[RdsCustomClusterConfigurationTypeDef],  # (3)
    DeletionProtection: NotRequired[bool],
    GlobalClusterIdentifier: NotRequired[str],
    EnableHttpEndpoint: NotRequired[bool],
    CopyTagsToSnapshot: NotRequired[bool],
    Domain: NotRequired[str],
    DomainIAMRoleName: NotRequired[str],
    EnableGlobalWriteForwarding: NotRequired[bool],
    DBClusterInstanceClass: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    StorageType: NotRequired[str],
    Iops: NotRequired[int],
    PubliclyAccessible: NotRequired[bool],
    AutoMinorVersionUpgrade: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    MonitoringRoleArn: NotRequired[str],
    DatabaseInsightsMode: NotRequired[DatabaseInsightsModeType],  # (4)
    EnablePerformanceInsights: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    PerformanceInsightsRetentionPeriod: NotRequired[int],
    EnableLimitlessDatabase: NotRequired[bool],
    ServerlessV2ScalingConfiguration: NotRequired[ServerlessV2ScalingConfigurationTypeDef],  # (5)
    NetworkType: NotRequired[str],
    ClusterScalabilityType: NotRequired[ClusterScalabilityTypeType],  # (6)
    DBSystemId: NotRequired[str],
    ManageMasterUserPassword: NotRequired[bool],
    MasterUserSecretKmsKeyId: NotRequired[str],
    EnableLocalWriteForwarding: NotRequired[bool],
    CACertificateIdentifier: NotRequired[str],
    EngineLifecycleSupport: NotRequired[str],
    SourceRegion: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ScalingConfigurationTypeDef](./type_defs.md#scalingconfigurationtypedef) 
3. See [:material-code-braces: RdsCustomClusterConfigurationTypeDef](./type_defs.md#rdscustomclusterconfigurationtypedef) 
4. See [:material-code-brackets: DatabaseInsightsModeType](./literals.md#databaseinsightsmodetype) 
5. See [:material-code-braces: ServerlessV2ScalingConfigurationTypeDef](./type_defs.md#serverlessv2scalingconfigurationtypedef) 
6. See [:material-code-brackets: ClusterScalabilityTypeType](./literals.md#clusterscalabilitytypetype) 
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
    BacktrackWindow: NotRequired[int],
    CloudwatchLogsExportConfiguration: NotRequired[CloudwatchLogsExportConfigurationTypeDef],  # (1)
    EngineVersion: NotRequired[str],
    AllowMajorVersionUpgrade: NotRequired[bool],
    DBInstanceParameterGroupName: NotRequired[str],
    Domain: NotRequired[str],
    DomainIAMRoleName: NotRequired[str],
    ScalingConfiguration: NotRequired[ScalingConfigurationTypeDef],  # (2)
    DeletionProtection: NotRequired[bool],
    EnableHttpEndpoint: NotRequired[bool],
    CopyTagsToSnapshot: NotRequired[bool],
    EnableGlobalWriteForwarding: NotRequired[bool],
    DBClusterInstanceClass: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    StorageType: NotRequired[str],
    Iops: NotRequired[int],
    AutoMinorVersionUpgrade: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    MonitoringRoleArn: NotRequired[str],
    DatabaseInsightsMode: NotRequired[DatabaseInsightsModeType],  # (3)
    EnablePerformanceInsights: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    PerformanceInsightsRetentionPeriod: NotRequired[int],
    ServerlessV2ScalingConfiguration: NotRequired[ServerlessV2ScalingConfigurationTypeDef],  # (4)
    NetworkType: NotRequired[str],
    ManageMasterUserPassword: NotRequired[bool],
    RotateMasterUserPassword: NotRequired[bool],
    MasterUserSecretKmsKeyId: NotRequired[str],
    EngineMode: NotRequired[str],
    AllowEngineModeChange: NotRequired[bool],
    EnableLocalWriteForwarding: NotRequired[bool],
    AwsBackupRecoveryPointArn: NotRequired[str],
    EnableLimitlessDatabase: NotRequired[bool],
    CACertificateIdentifier: NotRequired[str],
```

1. See [:material-code-braces: CloudwatchLogsExportConfigurationTypeDef](./type_defs.md#cloudwatchlogsexportconfigurationtypedef) 
2. See [:material-code-braces: ScalingConfigurationTypeDef](./type_defs.md#scalingconfigurationtypedef) 
3. See [:material-code-brackets: DatabaseInsightsModeType](./literals.md#databaseinsightsmodetype) 
4. See [:material-code-braces: ServerlessV2ScalingConfigurationTypeDef](./type_defs.md#serverlessv2scalingconfigurationtypedef) 
## RestoreDBClusterFromS3MessageRequestTypeDef

```python
# RestoreDBClusterFromS3MessageRequestTypeDef definition

class RestoreDBClusterFromS3MessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    Engine: str,
    MasterUsername: str,
    SourceEngine: str,
    SourceEngineVersion: str,
    S3BucketName: str,
    S3IngestionRoleArn: str,
    AvailabilityZones: NotRequired[Sequence[str]],
    BackupRetentionPeriod: NotRequired[int],
    CharacterSetName: NotRequired[str],
    DatabaseName: NotRequired[str],
    DBClusterParameterGroupName: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    DBSubnetGroupName: NotRequired[str],
    EngineVersion: NotRequired[str],
    Port: NotRequired[int],
    MasterUserPassword: NotRequired[str],
    OptionGroupName: NotRequired[str],
    PreferredBackupWindow: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    S3Prefix: NotRequired[str],
    BacktrackWindow: NotRequired[int],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    DeletionProtection: NotRequired[bool],
    CopyTagsToSnapshot: NotRequired[bool],
    Domain: NotRequired[str],
    DomainIAMRoleName: NotRequired[str],
    ServerlessV2ScalingConfiguration: NotRequired[ServerlessV2ScalingConfigurationTypeDef],  # (2)
    NetworkType: NotRequired[str],
    ManageMasterUserPassword: NotRequired[bool],
    MasterUserSecretKmsKeyId: NotRequired[str],
    StorageType: NotRequired[str],
    EngineLifecycleSupport: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
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
    BacktrackWindow: NotRequired[int],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    EngineMode: NotRequired[str],
    ScalingConfiguration: NotRequired[ScalingConfigurationTypeDef],  # (2)
    DBClusterParameterGroupName: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    CopyTagsToSnapshot: NotRequired[bool],
    Domain: NotRequired[str],
    DomainIAMRoleName: NotRequired[str],
    DBClusterInstanceClass: NotRequired[str],
    StorageType: NotRequired[str],
    Iops: NotRequired[int],
    PubliclyAccessible: NotRequired[bool],
    ServerlessV2ScalingConfiguration: NotRequired[ServerlessV2ScalingConfigurationTypeDef],  # (3)
    NetworkType: NotRequired[str],
    RdsCustomClusterConfiguration: NotRequired[RdsCustomClusterConfigurationTypeDef],  # (4)
    MonitoringInterval: NotRequired[int],
    MonitoringRoleArn: NotRequired[str],
    EnablePerformanceInsights: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    PerformanceInsightsRetentionPeriod: NotRequired[int],
    EngineLifecycleSupport: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ScalingConfigurationTypeDef](./type_defs.md#scalingconfigurationtypedef) 
3. See [:material-code-braces: ServerlessV2ScalingConfigurationTypeDef](./type_defs.md#serverlessv2scalingconfigurationtypedef) 
4. See [:material-code-braces: RdsCustomClusterConfigurationTypeDef](./type_defs.md#rdscustomclusterconfigurationtypedef) 
## RestoreDBClusterToPointInTimeMessageRequestTypeDef

```python
# RestoreDBClusterToPointInTimeMessageRequestTypeDef definition

class RestoreDBClusterToPointInTimeMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    RestoreType: NotRequired[str],
    SourceDBClusterIdentifier: NotRequired[str],
    RestoreToTime: NotRequired[TimestampTypeDef],
    UseLatestRestorableTime: NotRequired[bool],
    Port: NotRequired[int],
    DBSubnetGroupName: NotRequired[str],
    OptionGroupName: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    KmsKeyId: NotRequired[str],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    BacktrackWindow: NotRequired[int],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    DBClusterParameterGroupName: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    CopyTagsToSnapshot: NotRequired[bool],
    Domain: NotRequired[str],
    DomainIAMRoleName: NotRequired[str],
    ScalingConfiguration: NotRequired[ScalingConfigurationTypeDef],  # (2)
    EngineMode: NotRequired[str],
    DBClusterInstanceClass: NotRequired[str],
    StorageType: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    Iops: NotRequired[int],
    ServerlessV2ScalingConfiguration: NotRequired[ServerlessV2ScalingConfigurationTypeDef],  # (3)
    NetworkType: NotRequired[str],
    SourceDbClusterResourceId: NotRequired[str],
    RdsCustomClusterConfiguration: NotRequired[RdsCustomClusterConfigurationTypeDef],  # (4)
    MonitoringInterval: NotRequired[int],
    MonitoringRoleArn: NotRequired[str],
    EnablePerformanceInsights: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    PerformanceInsightsRetentionPeriod: NotRequired[int],
    EngineLifecycleSupport: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ScalingConfigurationTypeDef](./type_defs.md#scalingconfigurationtypedef) 
3. See [:material-code-braces: ServerlessV2ScalingConfigurationTypeDef](./type_defs.md#serverlessv2scalingconfigurationtypedef) 
4. See [:material-code-braces: RdsCustomClusterConfigurationTypeDef](./type_defs.md#rdscustomclusterconfigurationtypedef) 
## CreateDBInstanceMessageRequestTypeDef

```python
# CreateDBInstanceMessageRequestTypeDef definition

class CreateDBInstanceMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    DBInstanceClass: str,
    Engine: str,
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
    NcharCharacterSetName: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    DBClusterIdentifier: NotRequired[str],
    StorageType: NotRequired[str],
    TdeCredentialArn: NotRequired[str],
    TdeCredentialPassword: NotRequired[str],
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    Domain: NotRequired[str],
    DomainFqdn: NotRequired[str],
    DomainOu: NotRequired[str],
    DomainAuthSecretArn: NotRequired[str],
    DomainDnsIps: NotRequired[Sequence[str]],
    CopyTagsToSnapshot: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    MonitoringRoleArn: NotRequired[str],
    DomainIAMRoleName: NotRequired[str],
    PromotionTier: NotRequired[int],
    Timezone: NotRequired[str],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    DatabaseInsightsMode: NotRequired[DatabaseInsightsModeType],  # (2)
    EnablePerformanceInsights: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    PerformanceInsightsRetentionPeriod: NotRequired[int],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    ProcessorFeatures: NotRequired[Sequence[ProcessorFeatureTypeDef]],  # (3)
    DeletionProtection: NotRequired[bool],
    MaxAllocatedStorage: NotRequired[int],
    EnableCustomerOwnedIp: NotRequired[bool],
    CustomIamInstanceProfile: NotRequired[str],
    BackupTarget: NotRequired[str],
    NetworkType: NotRequired[str],
    StorageThroughput: NotRequired[int],
    ManageMasterUserPassword: NotRequired[bool],
    MasterUserSecretKmsKeyId: NotRequired[str],
    CACertificateIdentifier: NotRequired[str],
    DBSystemId: NotRequired[str],
    DedicatedLogVolume: NotRequired[bool],
    MultiTenant: NotRequired[bool],
    EngineLifecycleSupport: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: DatabaseInsightsModeType](./literals.md#databaseinsightsmodetype) 
3. See [:material-code-braces: ProcessorFeatureTypeDef](./type_defs.md#processorfeaturetypedef) 
## CreateDBInstanceReadReplicaMessageRequestTypeDef

```python
# CreateDBInstanceReadReplicaMessageRequestTypeDef definition

class CreateDBInstanceReadReplicaMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    SourceDBInstanceIdentifier: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    Port: NotRequired[int],
    MultiAZ: NotRequired[bool],
    AutoMinorVersionUpgrade: NotRequired[bool],
    Iops: NotRequired[int],
    OptionGroupName: NotRequired[str],
    DBParameterGroupName: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    DBSubnetGroupName: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    StorageType: NotRequired[str],
    CopyTagsToSnapshot: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    MonitoringRoleArn: NotRequired[str],
    KmsKeyId: NotRequired[str],
    PreSignedUrl: NotRequired[str],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    DatabaseInsightsMode: NotRequired[DatabaseInsightsModeType],  # (2)
    EnablePerformanceInsights: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    PerformanceInsightsRetentionPeriod: NotRequired[int],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    ProcessorFeatures: NotRequired[Sequence[ProcessorFeatureTypeDef]],  # (3)
    UseDefaultProcessorFeatures: NotRequired[bool],
    DeletionProtection: NotRequired[bool],
    Domain: NotRequired[str],
    DomainIAMRoleName: NotRequired[str],
    DomainFqdn: NotRequired[str],
    DomainOu: NotRequired[str],
    DomainAuthSecretArn: NotRequired[str],
    DomainDnsIps: NotRequired[Sequence[str]],
    ReplicaMode: NotRequired[ReplicaModeType],  # (4)
    MaxAllocatedStorage: NotRequired[int],
    CustomIamInstanceProfile: NotRequired[str],
    NetworkType: NotRequired[str],
    StorageThroughput: NotRequired[int],
    EnableCustomerOwnedIp: NotRequired[bool],
    AllocatedStorage: NotRequired[int],
    SourceDBClusterIdentifier: NotRequired[str],
    DedicatedLogVolume: NotRequired[bool],
    UpgradeStorageConfig: NotRequired[bool],
    CACertificateIdentifier: NotRequired[str],
    SourceRegion: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: DatabaseInsightsModeType](./literals.md#databaseinsightsmodetype) 
3. See [:material-code-braces: ProcessorFeatureTypeDef](./type_defs.md#processorfeaturetypedef) 
4. See [:material-code-brackets: ReplicaModeType](./literals.md#replicamodetype) 
## DBSnapshotTypeDef

```python
# DBSnapshotTypeDef definition

class DBSnapshotTypeDef(TypedDict):
    DBSnapshotIdentifier: NotRequired[str],
    DBInstanceIdentifier: NotRequired[str],
    SnapshotCreateTime: NotRequired[datetime],
    Engine: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    Status: NotRequired[str],
    Port: NotRequired[int],
    AvailabilityZone: NotRequired[str],
    VpcId: NotRequired[str],
    InstanceCreateTime: NotRequired[datetime],
    MasterUsername: NotRequired[str],
    EngineVersion: NotRequired[str],
    LicenseModel: NotRequired[str],
    SnapshotType: NotRequired[str],
    Iops: NotRequired[int],
    OptionGroupName: NotRequired[str],
    PercentProgress: NotRequired[int],
    SourceRegion: NotRequired[str],
    SourceDBSnapshotIdentifier: NotRequired[str],
    StorageType: NotRequired[str],
    TdeCredentialArn: NotRequired[str],
    Encrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    DBSnapshotArn: NotRequired[str],
    Timezone: NotRequired[str],
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    ProcessorFeatures: NotRequired[List[ProcessorFeatureTypeDef]],  # (1)
    DbiResourceId: NotRequired[str],
    TagList: NotRequired[List[TagTypeDef]],  # (2)
    OriginalSnapshotCreateTime: NotRequired[datetime],
    SnapshotDatabaseTime: NotRequired[datetime],
    SnapshotTarget: NotRequired[str],
    StorageThroughput: NotRequired[int],
    DBSystemId: NotRequired[str],
    DedicatedLogVolume: NotRequired[bool],
    MultiTenant: NotRequired[bool],
```

1. See [:material-code-braces: ProcessorFeatureTypeDef](./type_defs.md#processorfeaturetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
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
    DomainFqdn: NotRequired[str],
    DomainOu: NotRequired[str],
    DomainAuthSecretArn: NotRequired[str],
    DomainDnsIps: NotRequired[Sequence[str]],
    CopyTagsToSnapshot: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    DBPortNumber: NotRequired[int],
    PubliclyAccessible: NotRequired[bool],
    MonitoringRoleArn: NotRequired[str],
    DomainIAMRoleName: NotRequired[str],
    DisableDomain: NotRequired[bool],
    PromotionTier: NotRequired[int],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    DatabaseInsightsMode: NotRequired[DatabaseInsightsModeType],  # (1)
    EnablePerformanceInsights: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    PerformanceInsightsRetentionPeriod: NotRequired[int],
    CloudwatchLogsExportConfiguration: NotRequired[CloudwatchLogsExportConfigurationTypeDef],  # (2)
    ProcessorFeatures: NotRequired[Sequence[ProcessorFeatureTypeDef]],  # (3)
    UseDefaultProcessorFeatures: NotRequired[bool],
    DeletionProtection: NotRequired[bool],
    MaxAllocatedStorage: NotRequired[int],
    CertificateRotationRestart: NotRequired[bool],
    ReplicaMode: NotRequired[ReplicaModeType],  # (4)
    EnableCustomerOwnedIp: NotRequired[bool],
    AwsBackupRecoveryPointArn: NotRequired[str],
    AutomationMode: NotRequired[AutomationModeType],  # (5)
    ResumeFullAutomationModeMinutes: NotRequired[int],
    NetworkType: NotRequired[str],
    StorageThroughput: NotRequired[int],
    ManageMasterUserPassword: NotRequired[bool],
    RotateMasterUserPassword: NotRequired[bool],
    MasterUserSecretKmsKeyId: NotRequired[str],
    Engine: NotRequired[str],
    DedicatedLogVolume: NotRequired[bool],
    MultiTenant: NotRequired[bool],
```

1. See [:material-code-brackets: DatabaseInsightsModeType](./literals.md#databaseinsightsmodetype) 
2. See [:material-code-braces: CloudwatchLogsExportConfigurationTypeDef](./type_defs.md#cloudwatchlogsexportconfigurationtypedef) 
3. See [:material-code-braces: ProcessorFeatureTypeDef](./type_defs.md#processorfeaturetypedef) 
4. See [:material-code-brackets: ReplicaModeType](./literals.md#replicamodetype) 
5. See [:material-code-brackets: AutomationModeType](./literals.md#automationmodetype) 
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
    ProcessorFeatures: NotRequired[List[ProcessorFeatureTypeDef]],  # (2)
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    AutomationMode: NotRequired[AutomationModeType],  # (3)
    ResumeFullAutomationModeTime: NotRequired[datetime],
    StorageThroughput: NotRequired[int],
    Engine: NotRequired[str],
    DedicatedLogVolume: NotRequired[bool],
    MultiTenant: NotRequired[bool],
```

1. See [:material-code-braces: PendingCloudwatchLogsExportsTypeDef](./type_defs.md#pendingcloudwatchlogsexportstypedef) 
2. See [:material-code-braces: ProcessorFeatureTypeDef](./type_defs.md#processorfeaturetypedef) 
3. See [:material-code-brackets: AutomationModeType](./literals.md#automationmodetype) 
## RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef

```python
# RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef definition

class RestoreDBInstanceFromDBSnapshotMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    DBSnapshotIdentifier: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    Port: NotRequired[int],
    AvailabilityZone: NotRequired[str],
    DBSubnetGroupName: NotRequired[str],
    MultiAZ: NotRequired[bool],
    PubliclyAccessible: NotRequired[bool],
    AutoMinorVersionUpgrade: NotRequired[bool],
    LicenseModel: NotRequired[str],
    DBName: NotRequired[str],
    Engine: NotRequired[str],
    Iops: NotRequired[int],
    OptionGroupName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    StorageType: NotRequired[str],
    TdeCredentialArn: NotRequired[str],
    TdeCredentialPassword: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    Domain: NotRequired[str],
    DomainFqdn: NotRequired[str],
    DomainOu: NotRequired[str],
    DomainAuthSecretArn: NotRequired[str],
    DomainDnsIps: NotRequired[Sequence[str]],
    CopyTagsToSnapshot: NotRequired[bool],
    DomainIAMRoleName: NotRequired[str],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    ProcessorFeatures: NotRequired[Sequence[ProcessorFeatureTypeDef]],  # (2)
    UseDefaultProcessorFeatures: NotRequired[bool],
    DBParameterGroupName: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    EnableCustomerOwnedIp: NotRequired[bool],
    CustomIamInstanceProfile: NotRequired[str],
    BackupTarget: NotRequired[str],
    NetworkType: NotRequired[str],
    StorageThroughput: NotRequired[int],
    DBClusterSnapshotIdentifier: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    DedicatedLogVolume: NotRequired[bool],
    CACertificateIdentifier: NotRequired[str],
    EngineLifecycleSupport: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ProcessorFeatureTypeDef](./type_defs.md#processorfeaturetypedef) 
## RestoreDBInstanceFromS3MessageRequestTypeDef

```python
# RestoreDBInstanceFromS3MessageRequestTypeDef definition

class RestoreDBInstanceFromS3MessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    DBInstanceClass: str,
    Engine: str,
    SourceEngine: str,
    SourceEngineVersion: str,
    S3BucketName: str,
    S3IngestionRoleArn: str,
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
    PubliclyAccessible: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    StorageType: NotRequired[str],
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    CopyTagsToSnapshot: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    MonitoringRoleArn: NotRequired[str],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    S3Prefix: NotRequired[str],
    DatabaseInsightsMode: NotRequired[DatabaseInsightsModeType],  # (2)
    EnablePerformanceInsights: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    PerformanceInsightsRetentionPeriod: NotRequired[int],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    ProcessorFeatures: NotRequired[Sequence[ProcessorFeatureTypeDef]],  # (3)
    UseDefaultProcessorFeatures: NotRequired[bool],
    DeletionProtection: NotRequired[bool],
    MaxAllocatedStorage: NotRequired[int],
    NetworkType: NotRequired[str],
    StorageThroughput: NotRequired[int],
    ManageMasterUserPassword: NotRequired[bool],
    MasterUserSecretKmsKeyId: NotRequired[str],
    DedicatedLogVolume: NotRequired[bool],
    CACertificateIdentifier: NotRequired[str],
    EngineLifecycleSupport: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: DatabaseInsightsModeType](./literals.md#databaseinsightsmodetype) 
3. See [:material-code-braces: ProcessorFeatureTypeDef](./type_defs.md#processorfeaturetypedef) 
## RestoreDBInstanceToPointInTimeMessageRequestTypeDef

```python
# RestoreDBInstanceToPointInTimeMessageRequestTypeDef definition

class RestoreDBInstanceToPointInTimeMessageRequestTypeDef(TypedDict):
    TargetDBInstanceIdentifier: str,
    SourceDBInstanceIdentifier: NotRequired[str],
    RestoreTime: NotRequired[TimestampTypeDef],
    UseLatestRestorableTime: NotRequired[bool],
    DBInstanceClass: NotRequired[str],
    Port: NotRequired[int],
    AvailabilityZone: NotRequired[str],
    DBSubnetGroupName: NotRequired[str],
    MultiAZ: NotRequired[bool],
    PubliclyAccessible: NotRequired[bool],
    AutoMinorVersionUpgrade: NotRequired[bool],
    LicenseModel: NotRequired[str],
    DBName: NotRequired[str],
    Engine: NotRequired[str],
    Iops: NotRequired[int],
    OptionGroupName: NotRequired[str],
    CopyTagsToSnapshot: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    StorageType: NotRequired[str],
    TdeCredentialArn: NotRequired[str],
    TdeCredentialPassword: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    Domain: NotRequired[str],
    DomainIAMRoleName: NotRequired[str],
    DomainFqdn: NotRequired[str],
    DomainOu: NotRequired[str],
    DomainAuthSecretArn: NotRequired[str],
    DomainDnsIps: NotRequired[Sequence[str]],
    EnableIAMDatabaseAuthentication: NotRequired[bool],
    EnableCloudwatchLogsExports: NotRequired[Sequence[str]],
    ProcessorFeatures: NotRequired[Sequence[ProcessorFeatureTypeDef]],  # (2)
    UseDefaultProcessorFeatures: NotRequired[bool],
    DBParameterGroupName: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    SourceDbiResourceId: NotRequired[str],
    MaxAllocatedStorage: NotRequired[int],
    SourceDBInstanceAutomatedBackupsArn: NotRequired[str],
    EnableCustomerOwnedIp: NotRequired[bool],
    CustomIamInstanceProfile: NotRequired[str],
    BackupTarget: NotRequired[str],
    NetworkType: NotRequired[str],
    StorageThroughput: NotRequired[int],
    AllocatedStorage: NotRequired[int],
    DedicatedLogVolume: NotRequired[bool],
    CACertificateIdentifier: NotRequired[str],
    EngineLifecycleSupport: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ProcessorFeatureTypeDef](./type_defs.md#processorfeaturetypedef) 
## CreateDBProxyEndpointResponseTypeDef

```python
# CreateDBProxyEndpointResponseTypeDef definition

class CreateDBProxyEndpointResponseTypeDef(TypedDict):
    DBProxyEndpoint: DBProxyEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyEndpointTypeDef](./type_defs.md#dbproxyendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDBProxyEndpointResponseTypeDef

```python
# DeleteDBProxyEndpointResponseTypeDef definition

class DeleteDBProxyEndpointResponseTypeDef(TypedDict):
    DBProxyEndpoint: DBProxyEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyEndpointTypeDef](./type_defs.md#dbproxyendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDBProxyEndpointsResponseTypeDef

```python
# DescribeDBProxyEndpointsResponseTypeDef definition

class DescribeDBProxyEndpointsResponseTypeDef(TypedDict):
    DBProxyEndpoints: List[DBProxyEndpointTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyEndpointTypeDef](./type_defs.md#dbproxyendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDBProxyEndpointResponseTypeDef

```python
# ModifyDBProxyEndpointResponseTypeDef definition

class ModifyDBProxyEndpointResponseTypeDef(TypedDict):
    DBProxyEndpoint: DBProxyEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyEndpointTypeDef](./type_defs.md#dbproxyendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDBProxyRequestRequestTypeDef

```python
# CreateDBProxyRequestRequestTypeDef definition

class CreateDBProxyRequestRequestTypeDef(TypedDict):
    DBProxyName: str,
    EngineFamily: EngineFamilyType,  # (1)
    Auth: Sequence[UserAuthConfigTypeDef],  # (2)
    RoleArn: str,
    VpcSubnetIds: Sequence[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    RequireTLS: NotRequired[bool],
    IdleClientTimeout: NotRequired[int],
    DebugLogging: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: EngineFamilyType](./literals.md#enginefamilytype) 
2. See [:material-code-braces: UserAuthConfigTypeDef](./type_defs.md#userauthconfigtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ModifyDBProxyRequestRequestTypeDef

```python
# ModifyDBProxyRequestRequestTypeDef definition

class ModifyDBProxyRequestRequestTypeDef(TypedDict):
    DBProxyName: str,
    NewDBProxyName: NotRequired[str],
    Auth: NotRequired[Sequence[UserAuthConfigTypeDef]],  # (1)
    RequireTLS: NotRequired[bool],
    IdleClientTimeout: NotRequired[int],
    DebugLogging: NotRequired[bool],
    RoleArn: NotRequired[str],
    SecurityGroups: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: UserAuthConfigTypeDef](./type_defs.md#userauthconfigtypedef) 
## DBClusterAutomatedBackupTypeDef

```python
# DBClusterAutomatedBackupTypeDef definition

class DBClusterAutomatedBackupTypeDef(TypedDict):
    Engine: NotRequired[str],
    VpcId: NotRequired[str],
    DBClusterAutomatedBackupsArn: NotRequired[str],
    DBClusterIdentifier: NotRequired[str],
    RestoreWindow: NotRequired[RestoreWindowTypeDef],  # (1)
    MasterUsername: NotRequired[str],
    DbClusterResourceId: NotRequired[str],
    Region: NotRequired[str],
    LicenseModel: NotRequired[str],
    Status: NotRequired[str],
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    ClusterCreateTime: NotRequired[datetime],
    StorageEncrypted: NotRequired[bool],
    AllocatedStorage: NotRequired[int],
    EngineVersion: NotRequired[str],
    DBClusterArn: NotRequired[str],
    BackupRetentionPeriod: NotRequired[int],
    EngineMode: NotRequired[str],
    AvailabilityZones: NotRequired[List[str]],
    Port: NotRequired[int],
    KmsKeyId: NotRequired[str],
    StorageType: NotRequired[str],
    Iops: NotRequired[int],
    AwsBackupRecoveryPointArn: NotRequired[str],
    StorageThroughput: NotRequired[int],
```

1. See [:material-code-braces: RestoreWindowTypeDef](./type_defs.md#restorewindowtypedef) 
## DBClusterBacktrackMessageTypeDef

```python
# DBClusterBacktrackMessageTypeDef definition

class DBClusterBacktrackMessageTypeDef(TypedDict):
    Marker: str,
    DBClusterBacktracks: List[DBClusterBacktrackTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterBacktrackTypeDef](./type_defs.md#dbclusterbacktracktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    Parameters: List[ParameterOutputTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterOutputTypeDef](./type_defs.md#parameteroutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBParameterGroupDetailsTypeDef

```python
# DBParameterGroupDetailsTypeDef definition

class DBParameterGroupDetailsTypeDef(TypedDict):
    Parameters: List[ParameterOutputTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterOutputTypeDef](./type_defs.md#parameteroutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EngineDefaultsTypeDef

```python
# EngineDefaultsTypeDef definition

class EngineDefaultsTypeDef(TypedDict):
    DBParameterGroupFamily: NotRequired[str],
    Marker: NotRequired[str],
    Parameters: NotRequired[List[ParameterOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterOutputTypeDef](./type_defs.md#parameteroutputtypedef) 
## DBClusterSnapshotAttributesResultTypeDef

```python
# DBClusterSnapshotAttributesResultTypeDef definition

class DBClusterSnapshotAttributesResultTypeDef(TypedDict):
    DBClusterSnapshotIdentifier: NotRequired[str],
    DBClusterSnapshotAttributes: NotRequired[List[DBClusterSnapshotAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: DBClusterSnapshotAttributeTypeDef](./type_defs.md#dbclustersnapshotattributetypedef) 
## DBEngineVersionResponseTypeDef

```python
# DBEngineVersionResponseTypeDef definition

class DBEngineVersionResponseTypeDef(TypedDict):
    Engine: str,
    EngineVersion: str,
    DBParameterGroupFamily: str,
    DBEngineDescription: str,
    DBEngineVersionDescription: str,
    DefaultCharacterSet: CharacterSetTypeDef,  # (1)
    Image: CustomDBEngineVersionAMITypeDef,  # (2)
    DBEngineMediaType: str,
    SupportedCharacterSets: List[CharacterSetTypeDef],  # (3)
    SupportedNcharCharacterSets: List[CharacterSetTypeDef],  # (3)
    ValidUpgradeTarget: List[UpgradeTargetTypeDef],  # (5)
    SupportedTimezones: List[TimezoneTypeDef],  # (6)
    ExportableLogTypes: List[str],
    SupportsLogExportsToCloudwatchLogs: bool,
    SupportsReadReplica: bool,
    SupportedEngineModes: List[str],
    SupportedFeatureNames: List[str],
    Status: str,
    SupportsParallelQuery: bool,
    SupportsGlobalDatabases: bool,
    MajorEngineVersion: str,
    DatabaseInstallationFilesS3BucketName: str,
    DatabaseInstallationFilesS3Prefix: str,
    DBEngineVersionArn: str,
    KMSKeyId: str,
    CreateTime: datetime,
    TagList: List[TagTypeDef],  # (7)
    SupportsBabelfish: bool,
    CustomDBEngineVersionManifest: str,
    SupportsLimitlessDatabase: bool,
    SupportsCertificateRotationWithoutRestart: bool,
    SupportedCACertificateIdentifiers: List[str],
    SupportsLocalWriteForwarding: bool,
    SupportsIntegrations: bool,
    ServerlessV2FeaturesSupport: ServerlessV2FeaturesSupportTypeDef,  # (8)
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-braces: CharacterSetTypeDef](./type_defs.md#charactersettypedef) 
2. See [:material-code-braces: CustomDBEngineVersionAMITypeDef](./type_defs.md#customdbengineversionamitypedef) 
3. See [:material-code-braces: CharacterSetTypeDef](./type_defs.md#charactersettypedef) 
4. See [:material-code-braces: CharacterSetTypeDef](./type_defs.md#charactersettypedef) 
5. See [:material-code-braces: UpgradeTargetTypeDef](./type_defs.md#upgradetargettypedef) 
6. See [:material-code-braces: TimezoneTypeDef](./type_defs.md#timezonetypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: ServerlessV2FeaturesSupportTypeDef](./type_defs.md#serverlessv2featuressupporttypedef) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    Image: NotRequired[CustomDBEngineVersionAMITypeDef],  # (2)
    DBEngineMediaType: NotRequired[str],
    SupportedCharacterSets: NotRequired[List[CharacterSetTypeDef]],  # (3)
    SupportedNcharCharacterSets: NotRequired[List[CharacterSetTypeDef]],  # (3)
    ValidUpgradeTarget: NotRequired[List[UpgradeTargetTypeDef]],  # (5)
    SupportedTimezones: NotRequired[List[TimezoneTypeDef]],  # (6)
    ExportableLogTypes: NotRequired[List[str]],
    SupportsLogExportsToCloudwatchLogs: NotRequired[bool],
    SupportsReadReplica: NotRequired[bool],
    SupportedEngineModes: NotRequired[List[str]],
    SupportedFeatureNames: NotRequired[List[str]],
    Status: NotRequired[str],
    SupportsParallelQuery: NotRequired[bool],
    SupportsGlobalDatabases: NotRequired[bool],
    MajorEngineVersion: NotRequired[str],
    DatabaseInstallationFilesS3BucketName: NotRequired[str],
    DatabaseInstallationFilesS3Prefix: NotRequired[str],
    DBEngineVersionArn: NotRequired[str],
    KMSKeyId: NotRequired[str],
    CreateTime: NotRequired[datetime],
    TagList: NotRequired[List[TagTypeDef]],  # (7)
    SupportsBabelfish: NotRequired[bool],
    CustomDBEngineVersionManifest: NotRequired[str],
    SupportsLimitlessDatabase: NotRequired[bool],
    SupportsCertificateRotationWithoutRestart: NotRequired[bool],
    SupportedCACertificateIdentifiers: NotRequired[List[str]],
    SupportsLocalWriteForwarding: NotRequired[bool],
    SupportsIntegrations: NotRequired[bool],
    ServerlessV2FeaturesSupport: NotRequired[ServerlessV2FeaturesSupportTypeDef],  # (8)
```

1. See [:material-code-braces: CharacterSetTypeDef](./type_defs.md#charactersettypedef) 
2. See [:material-code-braces: CustomDBEngineVersionAMITypeDef](./type_defs.md#customdbengineversionamitypedef) 
3. See [:material-code-braces: CharacterSetTypeDef](./type_defs.md#charactersettypedef) 
4. See [:material-code-braces: CharacterSetTypeDef](./type_defs.md#charactersettypedef) 
5. See [:material-code-braces: UpgradeTargetTypeDef](./type_defs.md#upgradetargettypedef) 
6. See [:material-code-braces: TimezoneTypeDef](./type_defs.md#timezonetypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: ServerlessV2FeaturesSupportTypeDef](./type_defs.md#serverlessv2featuressupporttypedef) 
## DBInstanceAutomatedBackupTypeDef

```python
# DBInstanceAutomatedBackupTypeDef definition

class DBInstanceAutomatedBackupTypeDef(TypedDict):
    DBInstanceArn: NotRequired[str],
    DbiResourceId: NotRequired[str],
    Region: NotRequired[str],
    DBInstanceIdentifier: NotRequired[str],
    RestoreWindow: NotRequired[RestoreWindowTypeDef],  # (1)
    AllocatedStorage: NotRequired[int],
    Status: NotRequired[str],
    Port: NotRequired[int],
    AvailabilityZone: NotRequired[str],
    VpcId: NotRequired[str],
    InstanceCreateTime: NotRequired[datetime],
    MasterUsername: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    LicenseModel: NotRequired[str],
    Iops: NotRequired[int],
    OptionGroupName: NotRequired[str],
    TdeCredentialArn: NotRequired[str],
    Encrypted: NotRequired[bool],
    StorageType: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Timezone: NotRequired[str],
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    BackupRetentionPeriod: NotRequired[int],
    DBInstanceAutomatedBackupsArn: NotRequired[str],
    DBInstanceAutomatedBackupsReplications: NotRequired[List[DBInstanceAutomatedBackupsReplicationTypeDef]],  # (2)
    BackupTarget: NotRequired[str],
    StorageThroughput: NotRequired[int],
    AwsBackupRecoveryPointArn: NotRequired[str],
    DedicatedLogVolume: NotRequired[bool],
    MultiTenant: NotRequired[bool],
```

1. See [:material-code-braces: RestoreWindowTypeDef](./type_defs.md#restorewindowtypedef) 
2. See [:material-code-braces: DBInstanceAutomatedBackupsReplicationTypeDef](./type_defs.md#dbinstanceautomatedbackupsreplicationtypedef) 
## DBProxyTargetTypeDef

```python
# DBProxyTargetTypeDef definition

class DBProxyTargetTypeDef(TypedDict):
    TargetArn: NotRequired[str],
    Endpoint: NotRequired[str],
    TrackedClusterId: NotRequired[str],
    RdsResourceId: NotRequired[str],
    Port: NotRequired[int],
    Type: NotRequired[TargetTypeType],  # (1)
    Role: NotRequired[TargetRoleType],  # (2)
    TargetHealth: NotRequired[TargetHealthTypeDef],  # (3)
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
2. See [:material-code-brackets: TargetRoleType](./literals.md#targetroletype) 
3. See [:material-code-braces: TargetHealthTypeDef](./type_defs.md#targethealthtypedef) 
## DBProxyTypeDef

```python
# DBProxyTypeDef definition

class DBProxyTypeDef(TypedDict):
    DBProxyName: NotRequired[str],
    DBProxyArn: NotRequired[str],
    Status: NotRequired[DBProxyStatusType],  # (1)
    EngineFamily: NotRequired[str],
    VpcId: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[List[str]],
    VpcSubnetIds: NotRequired[List[str]],
    Auth: NotRequired[List[UserAuthConfigInfoTypeDef]],  # (2)
    RoleArn: NotRequired[str],
    Endpoint: NotRequired[str],
    RequireTLS: NotRequired[bool],
    IdleClientTimeout: NotRequired[int],
    DebugLogging: NotRequired[bool],
    CreatedDate: NotRequired[datetime],
    UpdatedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: DBProxyStatusType](./literals.md#dbproxystatustype) 
2. See [:material-code-braces: UserAuthConfigInfoTypeDef](./type_defs.md#userauthconfiginfotypedef) 
## DBSecurityGroupTypeDef

```python
# DBSecurityGroupTypeDef definition

class DBSecurityGroupTypeDef(TypedDict):
    OwnerId: NotRequired[str],
    DBSecurityGroupName: NotRequired[str],
    DBSecurityGroupDescription: NotRequired[str],
    VpcId: NotRequired[str],
    EC2SecurityGroups: NotRequired[List[EC2SecurityGroupTypeDef]],  # (1)
    IPRanges: NotRequired[List[IPRangeTypeDef]],  # (2)
    DBSecurityGroupArn: NotRequired[str],
```

1. See [:material-code-braces: EC2SecurityGroupTypeDef](./type_defs.md#ec2securitygrouptypedef) 
2. See [:material-code-braces: IPRangeTypeDef](./type_defs.md#iprangetypedef) 
## DBSnapshotAttributesResultTypeDef

```python
# DBSnapshotAttributesResultTypeDef definition

class DBSnapshotAttributesResultTypeDef(TypedDict):
    DBSnapshotIdentifier: NotRequired[str],
    DBSnapshotAttributes: NotRequired[List[DBSnapshotAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: DBSnapshotAttributeTypeDef](./type_defs.md#dbsnapshotattributetypedef) 
## DescribeBlueGreenDeploymentsRequestRequestTypeDef

```python
# DescribeBlueGreenDeploymentsRequestRequestTypeDef definition

class DescribeBlueGreenDeploymentsRequestRequestTypeDef(TypedDict):
    BlueGreenDeploymentIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeCertificatesMessageRequestTypeDef

```python
# DescribeCertificatesMessageRequestTypeDef definition

class DescribeCertificatesMessageRequestTypeDef(TypedDict):
    CertificateIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBClusterAutomatedBackupsMessageRequestTypeDef

```python
# DescribeDBClusterAutomatedBackupsMessageRequestTypeDef definition

class DescribeDBClusterAutomatedBackupsMessageRequestTypeDef(TypedDict):
    DbClusterResourceId: NotRequired[str],
    DBClusterIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBClusterBacktracksMessageRequestTypeDef

```python
# DescribeDBClusterBacktracksMessageRequestTypeDef definition

class DescribeDBClusterBacktracksMessageRequestTypeDef(TypedDict):
    DBClusterIdentifier: str,
    BacktrackIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
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
    DbClusterResourceId: NotRequired[str],
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
    IncludeShared: NotRequired[bool],
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
    IncludeAll: NotRequired[bool],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBInstanceAutomatedBackupsMessageRequestTypeDef

```python
# DescribeDBInstanceAutomatedBackupsMessageRequestTypeDef definition

class DescribeDBInstanceAutomatedBackupsMessageRequestTypeDef(TypedDict):
    DbiResourceId: NotRequired[str],
    DBInstanceIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    DBInstanceAutomatedBackupsArn: NotRequired[str],
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
## DescribeDBLogFilesMessageRequestTypeDef

```python
# DescribeDBLogFilesMessageRequestTypeDef definition

class DescribeDBLogFilesMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    FilenameContains: NotRequired[str],
    FileLastWritten: NotRequired[int],
    FileSize: NotRequired[int],
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
## DescribeDBProxiesRequestRequestTypeDef

```python
# DescribeDBProxiesRequestRequestTypeDef definition

class DescribeDBProxiesRequestRequestTypeDef(TypedDict):
    DBProxyName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBProxyEndpointsRequestRequestTypeDef

```python
# DescribeDBProxyEndpointsRequestRequestTypeDef definition

class DescribeDBProxyEndpointsRequestRequestTypeDef(TypedDict):
    DBProxyName: NotRequired[str],
    DBProxyEndpointName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBProxyTargetGroupsRequestRequestTypeDef

```python
# DescribeDBProxyTargetGroupsRequestRequestTypeDef definition

class DescribeDBProxyTargetGroupsRequestRequestTypeDef(TypedDict):
    DBProxyName: str,
    TargetGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBProxyTargetsRequestRequestTypeDef

```python
# DescribeDBProxyTargetsRequestRequestTypeDef definition

class DescribeDBProxyTargetsRequestRequestTypeDef(TypedDict):
    DBProxyName: str,
    TargetGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBRecommendationsMessageRequestTypeDef

```python
# DescribeDBRecommendationsMessageRequestTypeDef definition

class DescribeDBRecommendationsMessageRequestTypeDef(TypedDict):
    LastUpdatedAfter: NotRequired[TimestampTypeDef],
    LastUpdatedBefore: NotRequired[TimestampTypeDef],
    Locale: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBSecurityGroupsMessageRequestTypeDef

```python
# DescribeDBSecurityGroupsMessageRequestTypeDef definition

class DescribeDBSecurityGroupsMessageRequestTypeDef(TypedDict):
    DBSecurityGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBShardGroupsMessageRequestTypeDef

```python
# DescribeDBShardGroupsMessageRequestTypeDef definition

class DescribeDBShardGroupsMessageRequestTypeDef(TypedDict):
    DBShardGroupIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBSnapshotTenantDatabasesMessageRequestTypeDef

```python
# DescribeDBSnapshotTenantDatabasesMessageRequestTypeDef definition

class DescribeDBSnapshotTenantDatabasesMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    DBSnapshotIdentifier: NotRequired[str],
    SnapshotType: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    DbiResourceId: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeDBSnapshotsMessageRequestTypeDef

```python
# DescribeDBSnapshotsMessageRequestTypeDef definition

class DescribeDBSnapshotsMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    DBSnapshotIdentifier: NotRequired[str],
    SnapshotType: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    IncludeShared: NotRequired[bool],
    IncludePublic: NotRequired[bool],
    DbiResourceId: NotRequired[str],
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
## DescribeExportTasksMessageRequestTypeDef

```python
# DescribeExportTasksMessageRequestTypeDef definition

class DescribeExportTasksMessageRequestTypeDef(TypedDict):
    ExportTaskIdentifier: NotRequired[str],
    SourceArn: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
    SourceType: NotRequired[ExportSourceTypeType],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: ExportSourceTypeType](./literals.md#exportsourcetypetype) 
## DescribeGlobalClustersMessageRequestTypeDef

```python
# DescribeGlobalClustersMessageRequestTypeDef definition

class DescribeGlobalClustersMessageRequestTypeDef(TypedDict):
    GlobalClusterIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeIntegrationsMessageRequestTypeDef

```python
# DescribeIntegrationsMessageRequestTypeDef definition

class DescribeIntegrationsMessageRequestTypeDef(TypedDict):
    IntegrationIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeOptionGroupOptionsMessageRequestTypeDef

```python
# DescribeOptionGroupOptionsMessageRequestTypeDef definition

class DescribeOptionGroupOptionsMessageRequestTypeDef(TypedDict):
    EngineName: str,
    MajorEngineVersion: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeOptionGroupsMessageRequestTypeDef

```python
# DescribeOptionGroupsMessageRequestTypeDef definition

class DescribeOptionGroupsMessageRequestTypeDef(TypedDict):
    OptionGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
    EngineName: NotRequired[str],
    MajorEngineVersion: NotRequired[str],
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
    AvailabilityZoneGroup: NotRequired[str],
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
## DescribeReservedDBInstancesMessageRequestTypeDef

```python
# DescribeReservedDBInstancesMessageRequestTypeDef definition

class DescribeReservedDBInstancesMessageRequestTypeDef(TypedDict):
    ReservedDBInstanceId: NotRequired[str],
    ReservedDBInstancesOfferingId: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    Duration: NotRequired[str],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    MultiAZ: NotRequired[bool],
    LeaseId: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeReservedDBInstancesOfferingsMessageRequestTypeDef

```python
# DescribeReservedDBInstancesOfferingsMessageRequestTypeDef definition

class DescribeReservedDBInstancesOfferingsMessageRequestTypeDef(TypedDict):
    ReservedDBInstancesOfferingId: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    Duration: NotRequired[str],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    MultiAZ: NotRequired[bool],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeSourceRegionsMessageRequestTypeDef

```python
# DescribeSourceRegionsMessageRequestTypeDef definition

class DescribeSourceRegionsMessageRequestTypeDef(TypedDict):
    RegionName: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeTenantDatabasesMessageRequestTypeDef

```python
# DescribeTenantDatabasesMessageRequestTypeDef definition

class DescribeTenantDatabasesMessageRequestTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    TenantDBName: NotRequired[str],
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
## DescribeBlueGreenDeploymentsRequestPaginateTypeDef

```python
# DescribeBlueGreenDeploymentsRequestPaginateTypeDef definition

class DescribeBlueGreenDeploymentsRequestPaginateTypeDef(TypedDict):
    BlueGreenDeploymentIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeCertificatesMessagePaginateTypeDef

```python
# DescribeCertificatesMessagePaginateTypeDef definition

class DescribeCertificatesMessagePaginateTypeDef(TypedDict):
    CertificateIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClusterAutomatedBackupsMessagePaginateTypeDef

```python
# DescribeDBClusterAutomatedBackupsMessagePaginateTypeDef definition

class DescribeDBClusterAutomatedBackupsMessagePaginateTypeDef(TypedDict):
    DbClusterResourceId: NotRequired[str],
    DBClusterIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClusterBacktracksMessagePaginateTypeDef

```python
# DescribeDBClusterBacktracksMessagePaginateTypeDef definition

class DescribeDBClusterBacktracksMessagePaginateTypeDef(TypedDict):
    DBClusterIdentifier: str,
    BacktrackIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClusterEndpointsMessagePaginateTypeDef

```python
# DescribeDBClusterEndpointsMessagePaginateTypeDef definition

class DescribeDBClusterEndpointsMessagePaginateTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    DBClusterEndpointIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClusterParameterGroupsMessagePaginateTypeDef

```python
# DescribeDBClusterParameterGroupsMessagePaginateTypeDef definition

class DescribeDBClusterParameterGroupsMessagePaginateTypeDef(TypedDict):
    DBClusterParameterGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClusterParametersMessagePaginateTypeDef

```python
# DescribeDBClusterParametersMessagePaginateTypeDef definition

class DescribeDBClusterParametersMessagePaginateTypeDef(TypedDict):
    DBClusterParameterGroupName: str,
    Source: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClusterSnapshotsMessagePaginateTypeDef

```python
# DescribeDBClusterSnapshotsMessagePaginateTypeDef definition

class DescribeDBClusterSnapshotsMessagePaginateTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    DBClusterSnapshotIdentifier: NotRequired[str],
    SnapshotType: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    IncludeShared: NotRequired[bool],
    IncludePublic: NotRequired[bool],
    DbClusterResourceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClustersMessagePaginateTypeDef

```python
# DescribeDBClustersMessagePaginateTypeDef definition

class DescribeDBClustersMessagePaginateTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    IncludeShared: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBEngineVersionsMessagePaginateTypeDef

```python
# DescribeDBEngineVersionsMessagePaginateTypeDef definition

class DescribeDBEngineVersionsMessagePaginateTypeDef(TypedDict):
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    DBParameterGroupFamily: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    DefaultOnly: NotRequired[bool],
    ListSupportedCharacterSets: NotRequired[bool],
    ListSupportedTimezones: NotRequired[bool],
    IncludeAll: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBInstanceAutomatedBackupsMessagePaginateTypeDef

```python
# DescribeDBInstanceAutomatedBackupsMessagePaginateTypeDef definition

class DescribeDBInstanceAutomatedBackupsMessagePaginateTypeDef(TypedDict):
    DbiResourceId: NotRequired[str],
    DBInstanceIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    DBInstanceAutomatedBackupsArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBInstancesMessagePaginateTypeDef

```python
# DescribeDBInstancesMessagePaginateTypeDef definition

class DescribeDBInstancesMessagePaginateTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBLogFilesMessagePaginateTypeDef

```python
# DescribeDBLogFilesMessagePaginateTypeDef definition

class DescribeDBLogFilesMessagePaginateTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    FilenameContains: NotRequired[str],
    FileLastWritten: NotRequired[int],
    FileSize: NotRequired[int],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBParameterGroupsMessagePaginateTypeDef

```python
# DescribeDBParameterGroupsMessagePaginateTypeDef definition

class DescribeDBParameterGroupsMessagePaginateTypeDef(TypedDict):
    DBParameterGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBParametersMessagePaginateTypeDef

```python
# DescribeDBParametersMessagePaginateTypeDef definition

class DescribeDBParametersMessagePaginateTypeDef(TypedDict):
    DBParameterGroupName: str,
    Source: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBProxiesRequestPaginateTypeDef

```python
# DescribeDBProxiesRequestPaginateTypeDef definition

class DescribeDBProxiesRequestPaginateTypeDef(TypedDict):
    DBProxyName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBProxyEndpointsRequestPaginateTypeDef

```python
# DescribeDBProxyEndpointsRequestPaginateTypeDef definition

class DescribeDBProxyEndpointsRequestPaginateTypeDef(TypedDict):
    DBProxyName: NotRequired[str],
    DBProxyEndpointName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBProxyTargetGroupsRequestPaginateTypeDef

```python
# DescribeDBProxyTargetGroupsRequestPaginateTypeDef definition

class DescribeDBProxyTargetGroupsRequestPaginateTypeDef(TypedDict):
    DBProxyName: str,
    TargetGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBProxyTargetsRequestPaginateTypeDef

```python
# DescribeDBProxyTargetsRequestPaginateTypeDef definition

class DescribeDBProxyTargetsRequestPaginateTypeDef(TypedDict):
    DBProxyName: str,
    TargetGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBRecommendationsMessagePaginateTypeDef

```python
# DescribeDBRecommendationsMessagePaginateTypeDef definition

class DescribeDBRecommendationsMessagePaginateTypeDef(TypedDict):
    LastUpdatedAfter: NotRequired[TimestampTypeDef],
    LastUpdatedBefore: NotRequired[TimestampTypeDef],
    Locale: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBSecurityGroupsMessagePaginateTypeDef

```python
# DescribeDBSecurityGroupsMessagePaginateTypeDef definition

class DescribeDBSecurityGroupsMessagePaginateTypeDef(TypedDict):
    DBSecurityGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBSnapshotTenantDatabasesMessagePaginateTypeDef

```python
# DescribeDBSnapshotTenantDatabasesMessagePaginateTypeDef definition

class DescribeDBSnapshotTenantDatabasesMessagePaginateTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    DBSnapshotIdentifier: NotRequired[str],
    SnapshotType: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    DbiResourceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBSnapshotsMessagePaginateTypeDef

```python
# DescribeDBSnapshotsMessagePaginateTypeDef definition

class DescribeDBSnapshotsMessagePaginateTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    DBSnapshotIdentifier: NotRequired[str],
    SnapshotType: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    IncludeShared: NotRequired[bool],
    IncludePublic: NotRequired[bool],
    DbiResourceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBSubnetGroupsMessagePaginateTypeDef

```python
# DescribeDBSubnetGroupsMessagePaginateTypeDef definition

class DescribeDBSubnetGroupsMessagePaginateTypeDef(TypedDict):
    DBSubnetGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEngineDefaultClusterParametersMessagePaginateTypeDef

```python
# DescribeEngineDefaultClusterParametersMessagePaginateTypeDef definition

class DescribeEngineDefaultClusterParametersMessagePaginateTypeDef(TypedDict):
    DBParameterGroupFamily: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEngineDefaultParametersMessagePaginateTypeDef

```python
# DescribeEngineDefaultParametersMessagePaginateTypeDef definition

class DescribeEngineDefaultParametersMessagePaginateTypeDef(TypedDict):
    DBParameterGroupFamily: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventSubscriptionsMessagePaginateTypeDef

```python
# DescribeEventSubscriptionsMessagePaginateTypeDef definition

class DescribeEventSubscriptionsMessagePaginateTypeDef(TypedDict):
    SubscriptionName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsMessagePaginateTypeDef

```python
# DescribeEventsMessagePaginateTypeDef definition

class DescribeEventsMessagePaginateTypeDef(TypedDict):
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
## DescribeExportTasksMessagePaginateTypeDef

```python
# DescribeExportTasksMessagePaginateTypeDef definition

class DescribeExportTasksMessagePaginateTypeDef(TypedDict):
    ExportTaskIdentifier: NotRequired[str],
    SourceArn: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SourceType: NotRequired[ExportSourceTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: ExportSourceTypeType](./literals.md#exportsourcetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeGlobalClustersMessagePaginateTypeDef

```python
# DescribeGlobalClustersMessagePaginateTypeDef definition

class DescribeGlobalClustersMessagePaginateTypeDef(TypedDict):
    GlobalClusterIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeIntegrationsMessagePaginateTypeDef

```python
# DescribeIntegrationsMessagePaginateTypeDef definition

class DescribeIntegrationsMessagePaginateTypeDef(TypedDict):
    IntegrationIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOptionGroupOptionsMessagePaginateTypeDef

```python
# DescribeOptionGroupOptionsMessagePaginateTypeDef definition

class DescribeOptionGroupOptionsMessagePaginateTypeDef(TypedDict):
    EngineName: str,
    MajorEngineVersion: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOptionGroupsMessagePaginateTypeDef

```python
# DescribeOptionGroupsMessagePaginateTypeDef definition

class DescribeOptionGroupsMessagePaginateTypeDef(TypedDict):
    OptionGroupName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    EngineName: NotRequired[str],
    MajorEngineVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOrderableDBInstanceOptionsMessagePaginateTypeDef

```python
# DescribeOrderableDBInstanceOptionsMessagePaginateTypeDef definition

class DescribeOrderableDBInstanceOptionsMessagePaginateTypeDef(TypedDict):
    Engine: str,
    EngineVersion: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    LicenseModel: NotRequired[str],
    AvailabilityZoneGroup: NotRequired[str],
    Vpc: NotRequired[bool],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePendingMaintenanceActionsMessagePaginateTypeDef

```python
# DescribePendingMaintenanceActionsMessagePaginateTypeDef definition

class DescribePendingMaintenanceActionsMessagePaginateTypeDef(TypedDict):
    ResourceIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReservedDBInstancesMessagePaginateTypeDef

```python
# DescribeReservedDBInstancesMessagePaginateTypeDef definition

class DescribeReservedDBInstancesMessagePaginateTypeDef(TypedDict):
    ReservedDBInstanceId: NotRequired[str],
    ReservedDBInstancesOfferingId: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    Duration: NotRequired[str],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    MultiAZ: NotRequired[bool],
    LeaseId: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReservedDBInstancesOfferingsMessagePaginateTypeDef

```python
# DescribeReservedDBInstancesOfferingsMessagePaginateTypeDef definition

class DescribeReservedDBInstancesOfferingsMessagePaginateTypeDef(TypedDict):
    ReservedDBInstancesOfferingId: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    Duration: NotRequired[str],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    MultiAZ: NotRequired[bool],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSourceRegionsMessagePaginateTypeDef

```python
# DescribeSourceRegionsMessagePaginateTypeDef definition

class DescribeSourceRegionsMessagePaginateTypeDef(TypedDict):
    RegionName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeTenantDatabasesMessagePaginateTypeDef

```python
# DescribeTenantDatabasesMessagePaginateTypeDef definition

class DescribeTenantDatabasesMessagePaginateTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    TenantDBName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DownloadDBLogFilePortionMessagePaginateTypeDef

```python
# DownloadDBLogFilePortionMessagePaginateTypeDef definition

class DownloadDBLogFilePortionMessagePaginateTypeDef(TypedDict):
    DBInstanceIdentifier: str,
    LogFileName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDBClusterSnapshotsMessageWaitTypeDef

```python
# DescribeDBClusterSnapshotsMessageWaitTypeDef definition

class DescribeDBClusterSnapshotsMessageWaitTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    DBClusterSnapshotIdentifier: NotRequired[str],
    SnapshotType: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    IncludeShared: NotRequired[bool],
    IncludePublic: NotRequired[bool],
    DbClusterResourceId: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeDBClustersMessageWaitTypeDef

```python
# DescribeDBClustersMessageWaitTypeDef definition

class DescribeDBClustersMessageWaitTypeDef(TypedDict):
    DBClusterIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    IncludeShared: NotRequired[bool],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeDBInstancesMessageWaitTypeDef

```python
# DescribeDBInstancesMessageWaitTypeDef definition

class DescribeDBInstancesMessageWaitTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeDBSnapshotsMessageWaitTypeDef

```python
# DescribeDBSnapshotsMessageWaitTypeDef definition

class DescribeDBSnapshotsMessageWaitTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    DBSnapshotIdentifier: NotRequired[str],
    SnapshotType: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    IncludeShared: NotRequired[bool],
    IncludePublic: NotRequired[bool],
    DbiResourceId: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTenantDatabasesMessageWaitTypeDef

```python
# DescribeTenantDatabasesMessageWaitTypeDef definition

class DescribeTenantDatabasesMessageWaitTypeDef(TypedDict):
    DBInstanceIdentifier: NotRequired[str],
    TenantDBName: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeDBLogFilesResponseTypeDef

```python
# DescribeDBLogFilesResponseTypeDef definition

class DescribeDBLogFilesResponseTypeDef(TypedDict):
    DescribeDBLogFiles: List[DescribeDBLogFilesDetailsTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DescribeDBLogFilesDetailsTypeDef](./type_defs.md#describedblogfilesdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## ExportTasksMessageTypeDef

```python
# ExportTasksMessageTypeDef definition

class ExportTasksMessageTypeDef(TypedDict):
    Marker: str,
    ExportTasks: List[ExportTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportTaskTypeDef](./type_defs.md#exporttasktypedef) 
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
    EngineLifecycleSupport: NotRequired[str],
    DatabaseName: NotRequired[str],
    StorageEncrypted: NotRequired[bool],
    DeletionProtection: NotRequired[bool],
    GlobalClusterMembers: NotRequired[List[GlobalClusterMemberTypeDef]],  # (1)
    Endpoint: NotRequired[str],
    FailoverState: NotRequired[FailoverStateTypeDef],  # (2)
    TagList: NotRequired[List[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: GlobalClusterMemberTypeDef](./type_defs.md#globalclustermembertypedef) 
2. See [:material-code-braces: FailoverStateTypeDef](./type_defs.md#failoverstatetypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## IntegrationResponseTypeDef

```python
# IntegrationResponseTypeDef definition

class IntegrationResponseTypeDef(TypedDict):
    SourceArn: str,
    TargetArn: str,
    IntegrationName: str,
    IntegrationArn: str,
    KMSKeyId: str,
    AdditionalEncryptionContext: Dict[str, str],
    Status: IntegrationStatusType,  # (1)
    Tags: List[TagTypeDef],  # (2)
    CreateTime: datetime,
    Errors: List[IntegrationErrorTypeDef],  # (3)
    DataFilter: str,
    Description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: IntegrationStatusType](./literals.md#integrationstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: IntegrationErrorTypeDef](./type_defs.md#integrationerrortypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntegrationTypeDef

```python
# IntegrationTypeDef definition

class IntegrationTypeDef(TypedDict):
    SourceArn: NotRequired[str],
    TargetArn: NotRequired[str],
    IntegrationName: NotRequired[str],
    IntegrationArn: NotRequired[str],
    KMSKeyId: NotRequired[str],
    AdditionalEncryptionContext: NotRequired[Dict[str, str]],
    Status: NotRequired[IntegrationStatusType],  # (1)
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    CreateTime: NotRequired[datetime],
    Errors: NotRequired[List[IntegrationErrorTypeDef]],  # (3)
    DataFilter: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: IntegrationStatusType](./literals.md#integrationstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: IntegrationErrorTypeDef](./type_defs.md#integrationerrortypedef) 
## OptionGroupOptionSettingTypeDef

```python
# OptionGroupOptionSettingTypeDef definition

class OptionGroupOptionSettingTypeDef(TypedDict):
    SettingName: NotRequired[str],
    SettingDescription: NotRequired[str],
    DefaultValue: NotRequired[str],
    ApplyType: NotRequired[str],
    AllowedValues: NotRequired[str],
    IsModifiable: NotRequired[bool],
    IsRequired: NotRequired[bool],
    MinimumEngineVersionPerAllowedValue: NotRequired[List[MinimumEngineVersionPerAllowedValueTypeDef]],  # (1)
```

1. See [:material-code-braces: MinimumEngineVersionPerAllowedValueTypeDef](./type_defs.md#minimumengineversionperallowedvaluetypedef) 
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
## ModifyDBRecommendationMessageRequestTypeDef

```python
# ModifyDBRecommendationMessageRequestTypeDef definition

class ModifyDBRecommendationMessageRequestTypeDef(TypedDict):
    RecommendationId: str,
    Locale: NotRequired[str],
    Status: NotRequired[str],
    RecommendedActionUpdates: NotRequired[Sequence[RecommendedActionUpdateTypeDef]],  # (1)
```

1. See [:material-code-braces: RecommendedActionUpdateTypeDef](./type_defs.md#recommendedactionupdatetypedef) 
## OptionConfigurationTypeDef

```python
# OptionConfigurationTypeDef definition

class OptionConfigurationTypeDef(TypedDict):
    OptionName: str,
    Port: NotRequired[int],
    OptionVersion: NotRequired[str],
    DBSecurityGroupMemberships: NotRequired[Sequence[str]],
    VpcSecurityGroupMemberships: NotRequired[Sequence[str]],
    OptionSettings: NotRequired[Sequence[OptionSettingTypeDef]],  # (1)
```

1. See [:material-code-braces: OptionSettingTypeDef](./type_defs.md#optionsettingtypedef) 
## OptionTypeDef

```python
# OptionTypeDef definition

class OptionTypeDef(TypedDict):
    OptionName: NotRequired[str],
    OptionDescription: NotRequired[str],
    Persistent: NotRequired[bool],
    Permanent: NotRequired[bool],
    Port: NotRequired[int],
    OptionVersion: NotRequired[str],
    OptionSettings: NotRequired[List[OptionSettingTypeDef]],  # (1)
    DBSecurityGroupMemberships: NotRequired[List[DBSecurityGroupMembershipTypeDef]],  # (2)
    VpcSecurityGroupMemberships: NotRequired[List[VpcSecurityGroupMembershipTypeDef]],  # (3)
```

1. See [:material-code-braces: OptionSettingTypeDef](./type_defs.md#optionsettingtypedef) 
2. See [:material-code-braces: DBSecurityGroupMembershipTypeDef](./type_defs.md#dbsecuritygroupmembershiptypedef) 
3. See [:material-code-braces: VpcSecurityGroupMembershipTypeDef](./type_defs.md#vpcsecuritygroupmembershiptypedef) 
## SubnetTypeDef

```python
# SubnetTypeDef definition

class SubnetTypeDef(TypedDict):
    SubnetIdentifier: NotRequired[str],
    SubnetAvailabilityZone: NotRequired[AvailabilityZoneTypeDef],  # (1)
    SubnetOutpost: NotRequired[OutpostTypeDef],  # (2)
    SubnetStatus: NotRequired[str],
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
2. See [:material-code-braces: OutpostTypeDef](./type_defs.md#outposttypedef) 
## ResourcePendingMaintenanceActionsTypeDef

```python
# ResourcePendingMaintenanceActionsTypeDef definition

class ResourcePendingMaintenanceActionsTypeDef(TypedDict):
    ResourceIdentifier: NotRequired[str],
    PendingMaintenanceActionDetails: NotRequired[List[PendingMaintenanceActionTypeDef]],  # (1)
```

1. See [:material-code-braces: PendingMaintenanceActionTypeDef](./type_defs.md#pendingmaintenanceactiontypedef) 
## PerformanceInsightsMetricQueryTypeDef

```python
# PerformanceInsightsMetricQueryTypeDef definition

class PerformanceInsightsMetricQueryTypeDef(TypedDict):
    GroupBy: NotRequired[PerformanceInsightsMetricDimensionGroupTypeDef],  # (1)
    Metric: NotRequired[str],
```

1. See [:material-code-braces: PerformanceInsightsMetricDimensionGroupTypeDef](./type_defs.md#performanceinsightsmetricdimensiongrouptypedef) 
## ValidStorageOptionsTypeDef

```python
# ValidStorageOptionsTypeDef definition

class ValidStorageOptionsTypeDef(TypedDict):
    StorageType: NotRequired[str],
    StorageSize: NotRequired[List[RangeTypeDef]],  # (1)
    ProvisionedIops: NotRequired[List[RangeTypeDef]],  # (1)
    IopsToStorageRatio: NotRequired[List[DoubleRangeTypeDef]],  # (3)
    SupportsStorageAutoscaling: NotRequired[bool],
    ProvisionedStorageThroughput: NotRequired[List[RangeTypeDef]],  # (1)
    StorageThroughputToIopsRatio: NotRequired[List[DoubleRangeTypeDef]],  # (3)
```

1. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
2. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
3. See [:material-code-braces: DoubleRangeTypeDef](./type_defs.md#doublerangetypedef) 
4. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
5. See [:material-code-braces: DoubleRangeTypeDef](./type_defs.md#doublerangetypedef) 
## ReservedDBInstanceTypeDef

```python
# ReservedDBInstanceTypeDef definition

class ReservedDBInstanceTypeDef(TypedDict):
    ReservedDBInstanceId: NotRequired[str],
    ReservedDBInstancesOfferingId: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    StartTime: NotRequired[datetime],
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    UsagePrice: NotRequired[float],
    CurrencyCode: NotRequired[str],
    DBInstanceCount: NotRequired[int],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    MultiAZ: NotRequired[bool],
    State: NotRequired[str],
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (1)
    ReservedDBInstanceArn: NotRequired[str],
    LeaseId: NotRequired[str],
```

1. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
## ReservedDBInstancesOfferingTypeDef

```python
# ReservedDBInstancesOfferingTypeDef definition

class ReservedDBInstancesOfferingTypeDef(TypedDict):
    ReservedDBInstancesOfferingId: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    UsagePrice: NotRequired[float],
    CurrencyCode: NotRequired[str],
    ProductDescription: NotRequired[str],
    OfferingType: NotRequired[str],
    MultiAZ: NotRequired[bool],
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (1)
```

1. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
## ReferenceDetailsTypeDef

```python
# ReferenceDetailsTypeDef definition

class ReferenceDetailsTypeDef(TypedDict):
    ScalarReferenceDetails: NotRequired[ScalarReferenceDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: ScalarReferenceDetailsTypeDef](./type_defs.md#scalarreferencedetailstypedef) 
## SourceRegionMessageTypeDef

```python
# SourceRegionMessageTypeDef definition

class SourceRegionMessageTypeDef(TypedDict):
    Marker: str,
    SourceRegions: List[SourceRegionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceRegionTypeDef](./type_defs.md#sourceregiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TenantDatabaseTypeDef

```python
# TenantDatabaseTypeDef definition

class TenantDatabaseTypeDef(TypedDict):
    TenantDatabaseCreateTime: NotRequired[datetime],
    DBInstanceIdentifier: NotRequired[str],
    TenantDBName: NotRequired[str],
    Status: NotRequired[str],
    MasterUsername: NotRequired[str],
    DbiResourceId: NotRequired[str],
    TenantDatabaseResourceId: NotRequired[str],
    TenantDatabaseARN: NotRequired[str],
    CharacterSetName: NotRequired[str],
    NcharCharacterSetName: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    PendingModifiedValues: NotRequired[TenantDatabasePendingModifiedValuesTypeDef],  # (1)
    TagList: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: TenantDatabasePendingModifiedValuesTypeDef](./type_defs.md#tenantdatabasependingmodifiedvaluestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
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
## DescribeDBShardGroupsResponseTypeDef

```python
# DescribeDBShardGroupsResponseTypeDef definition

class DescribeDBShardGroupsResponseTypeDef(TypedDict):
    DBShardGroups: List[DBShardGroupTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBShardGroupTypeDef](./type_defs.md#dbshardgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBSnapshotTenantDatabasesMessageTypeDef

```python
# DBSnapshotTenantDatabasesMessageTypeDef definition

class DBSnapshotTenantDatabasesMessageTypeDef(TypedDict):
    Marker: str,
    DBSnapshotTenantDatabases: List[DBSnapshotTenantDatabaseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSnapshotTenantDatabaseTypeDef](./type_defs.md#dbsnapshottenantdatabasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## CreateBlueGreenDeploymentResponseTypeDef

```python
# CreateBlueGreenDeploymentResponseTypeDef definition

class CreateBlueGreenDeploymentResponseTypeDef(TypedDict):
    BlueGreenDeployment: BlueGreenDeploymentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueGreenDeploymentTypeDef](./type_defs.md#bluegreendeploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBlueGreenDeploymentResponseTypeDef

```python
# DeleteBlueGreenDeploymentResponseTypeDef definition

class DeleteBlueGreenDeploymentResponseTypeDef(TypedDict):
    BlueGreenDeployment: BlueGreenDeploymentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueGreenDeploymentTypeDef](./type_defs.md#bluegreendeploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBlueGreenDeploymentsResponseTypeDef

```python
# DescribeBlueGreenDeploymentsResponseTypeDef definition

class DescribeBlueGreenDeploymentsResponseTypeDef(TypedDict):
    BlueGreenDeployments: List[BlueGreenDeploymentTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueGreenDeploymentTypeDef](./type_defs.md#bluegreendeploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SwitchoverBlueGreenDeploymentResponseTypeDef

```python
# SwitchoverBlueGreenDeploymentResponseTypeDef definition

class SwitchoverBlueGreenDeploymentResponseTypeDef(TypedDict):
    BlueGreenDeployment: BlueGreenDeploymentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueGreenDeploymentTypeDef](./type_defs.md#bluegreendeploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    AutomaticRestartTime: NotRequired[datetime],
    PercentProgress: NotRequired[str],
    EarliestRestorableTime: NotRequired[datetime],
    Endpoint: NotRequired[str],
    ReaderEndpoint: NotRequired[str],
    CustomEndpoints: NotRequired[List[str]],
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
    StatusInfos: NotRequired[List[DBClusterStatusInfoTypeDef]],  # (2)
    DBClusterMembers: NotRequired[List[DBClusterMemberTypeDef]],  # (3)
    VpcSecurityGroups: NotRequired[List[VpcSecurityGroupMembershipTypeDef]],  # (4)
    HostedZoneId: NotRequired[str],
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    DbClusterResourceId: NotRequired[str],
    DBClusterArn: NotRequired[str],
    AssociatedRoles: NotRequired[List[DBClusterRoleTypeDef]],  # (5)
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    CloneGroupId: NotRequired[str],
    ClusterCreateTime: NotRequired[datetime],
    EarliestBacktrackTime: NotRequired[datetime],
    BacktrackWindow: NotRequired[int],
    BacktrackConsumedChangeRecords: NotRequired[int],
    EnabledCloudwatchLogsExports: NotRequired[List[str]],
    Capacity: NotRequired[int],
    EngineMode: NotRequired[str],
    ScalingConfigurationInfo: NotRequired[ScalingConfigurationInfoTypeDef],  # (6)
    RdsCustomClusterConfiguration: NotRequired[RdsCustomClusterConfigurationTypeDef],  # (7)
    DeletionProtection: NotRequired[bool],
    HttpEndpointEnabled: NotRequired[bool],
    ActivityStreamMode: NotRequired[ActivityStreamModeType],  # (8)
    ActivityStreamStatus: NotRequired[ActivityStreamStatusType],  # (9)
    ActivityStreamKmsKeyId: NotRequired[str],
    ActivityStreamKinesisStreamName: NotRequired[str],
    CopyTagsToSnapshot: NotRequired[bool],
    CrossAccountClone: NotRequired[bool],
    DomainMemberships: NotRequired[List[DomainMembershipTypeDef]],  # (10)
    TagList: NotRequired[List[TagTypeDef]],  # (11)
    GlobalWriteForwardingStatus: NotRequired[WriteForwardingStatusType],  # (12)
    GlobalWriteForwardingRequested: NotRequired[bool],
    PendingModifiedValues: NotRequired[ClusterPendingModifiedValuesTypeDef],  # (13)
    DBClusterInstanceClass: NotRequired[str],
    StorageType: NotRequired[str],
    Iops: NotRequired[int],
    PubliclyAccessible: NotRequired[bool],
    AutoMinorVersionUpgrade: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    MonitoringRoleArn: NotRequired[str],
    DatabaseInsightsMode: NotRequired[DatabaseInsightsModeType],  # (14)
    PerformanceInsightsEnabled: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    PerformanceInsightsRetentionPeriod: NotRequired[int],
    ServerlessV2ScalingConfiguration: NotRequired[ServerlessV2ScalingConfigurationInfoTypeDef],  # (15)
    NetworkType: NotRequired[str],
    DBSystemId: NotRequired[str],
    MasterUserSecret: NotRequired[MasterUserSecretTypeDef],  # (16)
    IOOptimizedNextAllowedModificationTime: NotRequired[datetime],
    LocalWriteForwardingStatus: NotRequired[LocalWriteForwardingStatusType],  # (17)
    AwsBackupRecoveryPointArn: NotRequired[str],
    LimitlessDatabase: NotRequired[LimitlessDatabaseTypeDef],  # (18)
    StorageThroughput: NotRequired[int],
    ClusterScalabilityType: NotRequired[ClusterScalabilityTypeType],  # (19)
    CertificateDetails: NotRequired[CertificateDetailsTypeDef],  # (20)
    EngineLifecycleSupport: NotRequired[str],
```

1. See [:material-code-braces: DBClusterOptionGroupStatusTypeDef](./type_defs.md#dbclusteroptiongroupstatustypedef) 
2. See [:material-code-braces: DBClusterStatusInfoTypeDef](./type_defs.md#dbclusterstatusinfotypedef) 
3. See [:material-code-braces: DBClusterMemberTypeDef](./type_defs.md#dbclustermembertypedef) 
4. See [:material-code-braces: VpcSecurityGroupMembershipTypeDef](./type_defs.md#vpcsecuritygroupmembershiptypedef) 
5. See [:material-code-braces: DBClusterRoleTypeDef](./type_defs.md#dbclusterroletypedef) 
6. See [:material-code-braces: ScalingConfigurationInfoTypeDef](./type_defs.md#scalingconfigurationinfotypedef) 
7. See [:material-code-braces: RdsCustomClusterConfigurationTypeDef](./type_defs.md#rdscustomclusterconfigurationtypedef) 
8. See [:material-code-brackets: ActivityStreamModeType](./literals.md#activitystreammodetype) 
9. See [:material-code-brackets: ActivityStreamStatusType](./literals.md#activitystreamstatustype) 
10. See [:material-code-braces: DomainMembershipTypeDef](./type_defs.md#domainmembershiptypedef) 
11. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
12. See [:material-code-brackets: WriteForwardingStatusType](./literals.md#writeforwardingstatustype) 
13. See [:material-code-braces: ClusterPendingModifiedValuesTypeDef](./type_defs.md#clusterpendingmodifiedvaluestypedef) 
14. See [:material-code-brackets: DatabaseInsightsModeType](./literals.md#databaseinsightsmodetype) 
15. See [:material-code-braces: ServerlessV2ScalingConfigurationInfoTypeDef](./type_defs.md#serverlessv2scalingconfigurationinfotypedef) 
16. See [:material-code-braces: MasterUserSecretTypeDef](./type_defs.md#masterusersecrettypedef) 
17. See [:material-code-brackets: LocalWriteForwardingStatusType](./literals.md#localwriteforwardingstatustype) 
18. See [:material-code-braces: LimitlessDatabaseTypeDef](./type_defs.md#limitlessdatabasetypedef) 
19. See [:material-code-brackets: ClusterScalabilityTypeType](./literals.md#clusterscalabilitytypetype) 
20. See [:material-code-braces: CertificateDetailsTypeDef](./type_defs.md#certificatedetailstypedef) 
## DescribeDBProxyTargetGroupsResponseTypeDef

```python
# DescribeDBProxyTargetGroupsResponseTypeDef definition

class DescribeDBProxyTargetGroupsResponseTypeDef(TypedDict):
    TargetGroups: List[DBProxyTargetGroupTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyTargetGroupTypeDef](./type_defs.md#dbproxytargetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDBProxyTargetGroupResponseTypeDef

```python
# ModifyDBProxyTargetGroupResponseTypeDef definition

class ModifyDBProxyTargetGroupResponseTypeDef(TypedDict):
    DBProxyTargetGroup: DBProxyTargetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyTargetGroupTypeDef](./type_defs.md#dbproxytargetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyDBSnapshotResultTypeDef

```python
# CopyDBSnapshotResultTypeDef definition

class CopyDBSnapshotResultTypeDef(TypedDict):
    DBSnapshot: DBSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSnapshotTypeDef](./type_defs.md#dbsnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDBSnapshotResultTypeDef

```python
# CreateDBSnapshotResultTypeDef definition

class CreateDBSnapshotResultTypeDef(TypedDict):
    DBSnapshot: DBSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSnapshotTypeDef](./type_defs.md#dbsnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBSnapshotMessageTypeDef

```python
# DBSnapshotMessageTypeDef definition

class DBSnapshotMessageTypeDef(TypedDict):
    Marker: str,
    DBSnapshots: List[DBSnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSnapshotTypeDef](./type_defs.md#dbsnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDBSnapshotResultTypeDef

```python
# DeleteDBSnapshotResultTypeDef definition

class DeleteDBSnapshotResultTypeDef(TypedDict):
    DBSnapshot: DBSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSnapshotTypeDef](./type_defs.md#dbsnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDBSnapshotResultTypeDef

```python
# ModifyDBSnapshotResultTypeDef definition

class ModifyDBSnapshotResultTypeDef(TypedDict):
    DBSnapshot: DBSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSnapshotTypeDef](./type_defs.md#dbsnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBClusterAutomatedBackupMessageTypeDef

```python
# DBClusterAutomatedBackupMessageTypeDef definition

class DBClusterAutomatedBackupMessageTypeDef(TypedDict):
    Marker: str,
    DBClusterAutomatedBackups: List[DBClusterAutomatedBackupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterAutomatedBackupTypeDef](./type_defs.md#dbclusterautomatedbackuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDBClusterAutomatedBackupResultTypeDef

```python
# DeleteDBClusterAutomatedBackupResultTypeDef definition

class DeleteDBClusterAutomatedBackupResultTypeDef(TypedDict):
    DBClusterAutomatedBackup: DBClusterAutomatedBackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterAutomatedBackupTypeDef](./type_defs.md#dbclusterautomatedbackuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## DBInstanceAutomatedBackupMessageTypeDef

```python
# DBInstanceAutomatedBackupMessageTypeDef definition

class DBInstanceAutomatedBackupMessageTypeDef(TypedDict):
    Marker: str,
    DBInstanceAutomatedBackups: List[DBInstanceAutomatedBackupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceAutomatedBackupTypeDef](./type_defs.md#dbinstanceautomatedbackuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDBInstanceAutomatedBackupResultTypeDef

```python
# DeleteDBInstanceAutomatedBackupResultTypeDef definition

class DeleteDBInstanceAutomatedBackupResultTypeDef(TypedDict):
    DBInstanceAutomatedBackup: DBInstanceAutomatedBackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceAutomatedBackupTypeDef](./type_defs.md#dbinstanceautomatedbackuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDBInstanceAutomatedBackupsReplicationResultTypeDef

```python
# StartDBInstanceAutomatedBackupsReplicationResultTypeDef definition

class StartDBInstanceAutomatedBackupsReplicationResultTypeDef(TypedDict):
    DBInstanceAutomatedBackup: DBInstanceAutomatedBackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceAutomatedBackupTypeDef](./type_defs.md#dbinstanceautomatedbackuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopDBInstanceAutomatedBackupsReplicationResultTypeDef

```python
# StopDBInstanceAutomatedBackupsReplicationResultTypeDef definition

class StopDBInstanceAutomatedBackupsReplicationResultTypeDef(TypedDict):
    DBInstanceAutomatedBackup: DBInstanceAutomatedBackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceAutomatedBackupTypeDef](./type_defs.md#dbinstanceautomatedbackuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDBProxyTargetsResponseTypeDef

```python
# DescribeDBProxyTargetsResponseTypeDef definition

class DescribeDBProxyTargetsResponseTypeDef(TypedDict):
    Targets: List[DBProxyTargetTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyTargetTypeDef](./type_defs.md#dbproxytargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterDBProxyTargetsResponseTypeDef

```python
# RegisterDBProxyTargetsResponseTypeDef definition

class RegisterDBProxyTargetsResponseTypeDef(TypedDict):
    DBProxyTargets: List[DBProxyTargetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyTargetTypeDef](./type_defs.md#dbproxytargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDBProxyResponseTypeDef

```python
# CreateDBProxyResponseTypeDef definition

class CreateDBProxyResponseTypeDef(TypedDict):
    DBProxy: DBProxyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyTypeDef](./type_defs.md#dbproxytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDBProxyResponseTypeDef

```python
# DeleteDBProxyResponseTypeDef definition

class DeleteDBProxyResponseTypeDef(TypedDict):
    DBProxy: DBProxyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyTypeDef](./type_defs.md#dbproxytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDBProxiesResponseTypeDef

```python
# DescribeDBProxiesResponseTypeDef definition

class DescribeDBProxiesResponseTypeDef(TypedDict):
    DBProxies: List[DBProxyTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyTypeDef](./type_defs.md#dbproxytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDBProxyResponseTypeDef

```python
# ModifyDBProxyResponseTypeDef definition

class ModifyDBProxyResponseTypeDef(TypedDict):
    DBProxy: DBProxyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBProxyTypeDef](./type_defs.md#dbproxytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AuthorizeDBSecurityGroupIngressResultTypeDef

```python
# AuthorizeDBSecurityGroupIngressResultTypeDef definition

class AuthorizeDBSecurityGroupIngressResultTypeDef(TypedDict):
    DBSecurityGroup: DBSecurityGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSecurityGroupTypeDef](./type_defs.md#dbsecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDBSecurityGroupResultTypeDef

```python
# CreateDBSecurityGroupResultTypeDef definition

class CreateDBSecurityGroupResultTypeDef(TypedDict):
    DBSecurityGroup: DBSecurityGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSecurityGroupTypeDef](./type_defs.md#dbsecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBSecurityGroupMessageTypeDef

```python
# DBSecurityGroupMessageTypeDef definition

class DBSecurityGroupMessageTypeDef(TypedDict):
    Marker: str,
    DBSecurityGroups: List[DBSecurityGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSecurityGroupTypeDef](./type_defs.md#dbsecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RevokeDBSecurityGroupIngressResultTypeDef

```python
# RevokeDBSecurityGroupIngressResultTypeDef definition

class RevokeDBSecurityGroupIngressResultTypeDef(TypedDict):
    DBSecurityGroup: DBSecurityGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSecurityGroupTypeDef](./type_defs.md#dbsecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDBSnapshotAttributesResultTypeDef

```python
# DescribeDBSnapshotAttributesResultTypeDef definition

class DescribeDBSnapshotAttributesResultTypeDef(TypedDict):
    DBSnapshotAttributesResult: DBSnapshotAttributesResultTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSnapshotAttributesResultTypeDef](./type_defs.md#dbsnapshotattributesresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyDBSnapshotAttributeResultTypeDef

```python
# ModifyDBSnapshotAttributeResultTypeDef definition

class ModifyDBSnapshotAttributeResultTypeDef(TypedDict):
    DBSnapshotAttributesResult: DBSnapshotAttributesResultTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBSnapshotAttributesResultTypeDef](./type_defs.md#dbsnapshotattributesresulttypedef) 
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
## SwitchoverGlobalClusterResultTypeDef

```python
# SwitchoverGlobalClusterResultTypeDef definition

class SwitchoverGlobalClusterResultTypeDef(TypedDict):
    GlobalCluster: GlobalClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalClusterTypeDef](./type_defs.md#globalclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeIntegrationsResponseTypeDef

```python
# DescribeIntegrationsResponseTypeDef definition

class DescribeIntegrationsResponseTypeDef(TypedDict):
    Marker: str,
    Integrations: List[IntegrationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IntegrationTypeDef](./type_defs.md#integrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OptionGroupOptionTypeDef

```python
# OptionGroupOptionTypeDef definition

class OptionGroupOptionTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    EngineName: NotRequired[str],
    MajorEngineVersion: NotRequired[str],
    MinimumRequiredMinorEngineVersion: NotRequired[str],
    PortRequired: NotRequired[bool],
    DefaultPort: NotRequired[int],
    OptionsDependedOn: NotRequired[List[str]],
    OptionsConflictsWith: NotRequired[List[str]],
    Persistent: NotRequired[bool],
    Permanent: NotRequired[bool],
    RequiresAutoMinorEngineVersionUpgrade: NotRequired[bool],
    VpcOnly: NotRequired[bool],
    SupportsOptionVersionDowngrade: NotRequired[bool],
    OptionGroupOptionSettings: NotRequired[List[OptionGroupOptionSettingTypeDef]],  # (1)
    OptionGroupOptionVersions: NotRequired[List[OptionVersionTypeDef]],  # (2)
    CopyableCrossAccount: NotRequired[bool],
```

1. See [:material-code-braces: OptionGroupOptionSettingTypeDef](./type_defs.md#optiongroupoptionsettingtypedef) 
2. See [:material-code-braces: OptionVersionTypeDef](./type_defs.md#optionversiontypedef) 
## ModifyDBClusterParameterGroupMessageRequestTypeDef

```python
# ModifyDBClusterParameterGroupMessageRequestTypeDef definition

class ModifyDBClusterParameterGroupMessageRequestTypeDef(TypedDict):
    DBClusterParameterGroupName: str,
    Parameters: Sequence[ParameterUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) [:material-code-braces: ParameterOutputTypeDef](./type_defs.md#parameteroutputtypedef) 
## ModifyOptionGroupMessageRequestTypeDef

```python
# ModifyOptionGroupMessageRequestTypeDef definition

class ModifyOptionGroupMessageRequestTypeDef(TypedDict):
    OptionGroupName: str,
    OptionsToInclude: NotRequired[Sequence[OptionConfigurationTypeDef]],  # (1)
    OptionsToRemove: NotRequired[Sequence[str]],
    ApplyImmediately: NotRequired[bool],
```

1. See [:material-code-braces: OptionConfigurationTypeDef](./type_defs.md#optionconfigurationtypedef) 
## OptionGroupTypeDef

```python
# OptionGroupTypeDef definition

class OptionGroupTypeDef(TypedDict):
    OptionGroupName: NotRequired[str],
    OptionGroupDescription: NotRequired[str],
    EngineName: NotRequired[str],
    MajorEngineVersion: NotRequired[str],
    Options: NotRequired[List[OptionTypeDef]],  # (1)
    AllowsVpcAndNonVpcInstanceMemberships: NotRequired[bool],
    VpcId: NotRequired[str],
    OptionGroupArn: NotRequired[str],
    SourceOptionGroup: NotRequired[str],
    SourceAccountId: NotRequired[str],
    CopyTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
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
    SupportedNetworkTypes: NotRequired[List[str]],
```

1. See [:material-code-braces: SubnetTypeDef](./type_defs.md#subnettypedef) 
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
## MetricQueryTypeDef

```python
# MetricQueryTypeDef definition

class MetricQueryTypeDef(TypedDict):
    PerformanceInsightsMetricQuery: NotRequired[PerformanceInsightsMetricQueryTypeDef],  # (1)
```

1. See [:material-code-braces: PerformanceInsightsMetricQueryTypeDef](./type_defs.md#performanceinsightsmetricquerytypedef) 
## ValidDBInstanceModificationsMessageTypeDef

```python
# ValidDBInstanceModificationsMessageTypeDef definition

class ValidDBInstanceModificationsMessageTypeDef(TypedDict):
    Storage: NotRequired[List[ValidStorageOptionsTypeDef]],  # (1)
    ValidProcessorFeatures: NotRequired[List[AvailableProcessorFeatureTypeDef]],  # (2)
    SupportsDedicatedLogVolume: NotRequired[bool],
```

1. See [:material-code-braces: ValidStorageOptionsTypeDef](./type_defs.md#validstorageoptionstypedef) 
2. See [:material-code-braces: AvailableProcessorFeatureTypeDef](./type_defs.md#availableprocessorfeaturetypedef) 
## PurchaseReservedDBInstancesOfferingResultTypeDef

```python
# PurchaseReservedDBInstancesOfferingResultTypeDef definition

class PurchaseReservedDBInstancesOfferingResultTypeDef(TypedDict):
    ReservedDBInstance: ReservedDBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedDBInstanceTypeDef](./type_defs.md#reserveddbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReservedDBInstanceMessageTypeDef

```python
# ReservedDBInstanceMessageTypeDef definition

class ReservedDBInstanceMessageTypeDef(TypedDict):
    Marker: str,
    ReservedDBInstances: List[ReservedDBInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedDBInstanceTypeDef](./type_defs.md#reserveddbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReservedDBInstancesOfferingMessageTypeDef

```python
# ReservedDBInstancesOfferingMessageTypeDef definition

class ReservedDBInstancesOfferingMessageTypeDef(TypedDict):
    Marker: str,
    ReservedDBInstancesOfferings: List[ReservedDBInstancesOfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedDBInstancesOfferingTypeDef](./type_defs.md#reserveddbinstancesofferingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricReferenceTypeDef

```python
# MetricReferenceTypeDef definition

class MetricReferenceTypeDef(TypedDict):
    Name: NotRequired[str],
    ReferenceDetails: NotRequired[ReferenceDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: ReferenceDetailsTypeDef](./type_defs.md#referencedetailstypedef) 
## CreateTenantDatabaseResultTypeDef

```python
# CreateTenantDatabaseResultTypeDef definition

class CreateTenantDatabaseResultTypeDef(TypedDict):
    TenantDatabase: TenantDatabaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TenantDatabaseTypeDef](./type_defs.md#tenantdatabasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTenantDatabaseResultTypeDef

```python
# DeleteTenantDatabaseResultTypeDef definition

class DeleteTenantDatabaseResultTypeDef(TypedDict):
    TenantDatabase: TenantDatabaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TenantDatabaseTypeDef](./type_defs.md#tenantdatabasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyTenantDatabaseResultTypeDef

```python
# ModifyTenantDatabaseResultTypeDef definition

class ModifyTenantDatabaseResultTypeDef(TypedDict):
    TenantDatabase: TenantDatabaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TenantDatabaseTypeDef](./type_defs.md#tenantdatabasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TenantDatabasesMessageTypeDef

```python
# TenantDatabasesMessageTypeDef definition

class TenantDatabasesMessageTypeDef(TypedDict):
    Marker: str,
    TenantDatabases: List[TenantDatabaseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TenantDatabaseTypeDef](./type_defs.md#tenantdatabasetypedef) 
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
## RebootDBClusterResultTypeDef

```python
# RebootDBClusterResultTypeDef definition

class RebootDBClusterResultTypeDef(TypedDict):
    DBCluster: DBClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBClusterTypeDef](./type_defs.md#dbclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreDBClusterFromS3ResultTypeDef

```python
# RestoreDBClusterFromS3ResultTypeDef definition

class RestoreDBClusterFromS3ResultTypeDef(TypedDict):
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
## OptionGroupOptionsMessageTypeDef

```python
# OptionGroupOptionsMessageTypeDef definition

class OptionGroupOptionsMessageTypeDef(TypedDict):
    OptionGroupOptions: List[OptionGroupOptionTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OptionGroupOptionTypeDef](./type_defs.md#optiongroupoptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyOptionGroupResultTypeDef

```python
# CopyOptionGroupResultTypeDef definition

class CopyOptionGroupResultTypeDef(TypedDict):
    OptionGroup: OptionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OptionGroupTypeDef](./type_defs.md#optiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOptionGroupResultTypeDef

```python
# CreateOptionGroupResultTypeDef definition

class CreateOptionGroupResultTypeDef(TypedDict):
    OptionGroup: OptionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OptionGroupTypeDef](./type_defs.md#optiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyOptionGroupResultTypeDef

```python
# ModifyOptionGroupResultTypeDef definition

class ModifyOptionGroupResultTypeDef(TypedDict):
    OptionGroup: OptionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OptionGroupTypeDef](./type_defs.md#optiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OptionGroupsTypeDef

```python
# OptionGroupsTypeDef definition

class OptionGroupsTypeDef(TypedDict):
    OptionGroupsList: List[OptionGroupTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OptionGroupTypeDef](./type_defs.md#optiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    AutomaticRestartTime: NotRequired[datetime],
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
    ReplicaMode: NotRequired[ReplicaModeType],  # (7)
    LicenseModel: NotRequired[str],
    Iops: NotRequired[int],
    OptionGroupMemberships: NotRequired[List[OptionGroupMembershipTypeDef]],  # (8)
    CharacterSetName: NotRequired[str],
    NcharCharacterSetName: NotRequired[str],
    SecondaryAvailabilityZone: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    StatusInfos: NotRequired[List[DBInstanceStatusInfoTypeDef]],  # (9)
    StorageType: NotRequired[str],
    TdeCredentialArn: NotRequired[str],
    DbInstancePort: NotRequired[int],
    DBClusterIdentifier: NotRequired[str],
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    DbiResourceId: NotRequired[str],
    CACertificateIdentifier: NotRequired[str],
    DomainMemberships: NotRequired[List[DomainMembershipTypeDef]],  # (10)
    CopyTagsToSnapshot: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    EnhancedMonitoringResourceArn: NotRequired[str],
    MonitoringRoleArn: NotRequired[str],
    PromotionTier: NotRequired[int],
    DBInstanceArn: NotRequired[str],
    Timezone: NotRequired[str],
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    DatabaseInsightsMode: NotRequired[DatabaseInsightsModeType],  # (11)
    PerformanceInsightsEnabled: NotRequired[bool],
    PerformanceInsightsKMSKeyId: NotRequired[str],
    PerformanceInsightsRetentionPeriod: NotRequired[int],
    EnabledCloudwatchLogsExports: NotRequired[List[str]],
    ProcessorFeatures: NotRequired[List[ProcessorFeatureTypeDef]],  # (12)
    DeletionProtection: NotRequired[bool],
    AssociatedRoles: NotRequired[List[DBInstanceRoleTypeDef]],  # (13)
    ListenerEndpoint: NotRequired[EndpointTypeDef],  # (1)
    MaxAllocatedStorage: NotRequired[int],
    TagList: NotRequired[List[TagTypeDef]],  # (15)
    DBInstanceAutomatedBackupsReplications: NotRequired[List[DBInstanceAutomatedBackupsReplicationTypeDef]],  # (16)
    CustomerOwnedIpEnabled: NotRequired[bool],
    AwsBackupRecoveryPointArn: NotRequired[str],
    ActivityStreamStatus: NotRequired[ActivityStreamStatusType],  # (17)
    ActivityStreamKmsKeyId: NotRequired[str],
    ActivityStreamKinesisStreamName: NotRequired[str],
    ActivityStreamMode: NotRequired[ActivityStreamModeType],  # (18)
    ActivityStreamEngineNativeAuditFieldsIncluded: NotRequired[bool],
    AutomationMode: NotRequired[AutomationModeType],  # (19)
    ResumeFullAutomationModeTime: NotRequired[datetime],
    CustomIamInstanceProfile: NotRequired[str],
    BackupTarget: NotRequired[str],
    NetworkType: NotRequired[str],
    ActivityStreamPolicyStatus: NotRequired[ActivityStreamPolicyStatusType],  # (20)
    StorageThroughput: NotRequired[int],
    DBSystemId: NotRequired[str],
    MasterUserSecret: NotRequired[MasterUserSecretTypeDef],  # (21)
    CertificateDetails: NotRequired[CertificateDetailsTypeDef],  # (22)
    ReadReplicaSourceDBClusterIdentifier: NotRequired[str],
    PercentProgress: NotRequired[str],
    DedicatedLogVolume: NotRequired[bool],
    IsStorageConfigUpgradeAvailable: NotRequired[bool],
    MultiTenant: NotRequired[bool],
    EngineLifecycleSupport: NotRequired[str],
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: DBSecurityGroupMembershipTypeDef](./type_defs.md#dbsecuritygroupmembershiptypedef) 
3. See [:material-code-braces: VpcSecurityGroupMembershipTypeDef](./type_defs.md#vpcsecuritygroupmembershiptypedef) 
4. See [:material-code-braces: DBParameterGroupStatusTypeDef](./type_defs.md#dbparametergroupstatustypedef) 
5. See [:material-code-braces: DBSubnetGroupTypeDef](./type_defs.md#dbsubnetgrouptypedef) 
6. See [:material-code-braces: PendingModifiedValuesTypeDef](./type_defs.md#pendingmodifiedvaluestypedef) 
7. See [:material-code-brackets: ReplicaModeType](./literals.md#replicamodetype) 
8. See [:material-code-braces: OptionGroupMembershipTypeDef](./type_defs.md#optiongroupmembershiptypedef) 
9. See [:material-code-braces: DBInstanceStatusInfoTypeDef](./type_defs.md#dbinstancestatusinfotypedef) 
10. See [:material-code-braces: DomainMembershipTypeDef](./type_defs.md#domainmembershiptypedef) 
11. See [:material-code-brackets: DatabaseInsightsModeType](./literals.md#databaseinsightsmodetype) 
12. See [:material-code-braces: ProcessorFeatureTypeDef](./type_defs.md#processorfeaturetypedef) 
13. See [:material-code-braces: DBInstanceRoleTypeDef](./type_defs.md#dbinstanceroletypedef) 
14. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
15. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
16. See [:material-code-braces: DBInstanceAutomatedBackupsReplicationTypeDef](./type_defs.md#dbinstanceautomatedbackupsreplicationtypedef) 
17. See [:material-code-brackets: ActivityStreamStatusType](./literals.md#activitystreamstatustype) 
18. See [:material-code-brackets: ActivityStreamModeType](./literals.md#activitystreammodetype) 
19. See [:material-code-brackets: AutomationModeType](./literals.md#automationmodetype) 
20. See [:material-code-brackets: ActivityStreamPolicyStatusType](./literals.md#activitystreampolicystatustype) 
21. See [:material-code-braces: MasterUserSecretTypeDef](./type_defs.md#masterusersecrettypedef) 
22. See [:material-code-braces: CertificateDetailsTypeDef](./type_defs.md#certificatedetailstypedef) 
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
## DescribeValidDBInstanceModificationsResultTypeDef

```python
# DescribeValidDBInstanceModificationsResultTypeDef definition

class DescribeValidDBInstanceModificationsResultTypeDef(TypedDict):
    ValidDBInstanceModificationsMessage: ValidDBInstanceModificationsMessageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidDBInstanceModificationsMessageTypeDef](./type_defs.md#validdbinstancemodificationsmessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricTypeDef

```python
# MetricTypeDef definition

class MetricTypeDef(TypedDict):
    Name: NotRequired[str],
    References: NotRequired[List[MetricReferenceTypeDef]],  # (1)
    StatisticsDetails: NotRequired[str],
    MetricQuery: NotRequired[MetricQueryTypeDef],  # (2)
```

1. See [:material-code-braces: MetricReferenceTypeDef](./type_defs.md#metricreferencetypedef) 
2. See [:material-code-braces: MetricQueryTypeDef](./type_defs.md#metricquerytypedef) 
## CreateDBInstanceReadReplicaResultTypeDef

```python
# CreateDBInstanceReadReplicaResultTypeDef definition

class CreateDBInstanceReadReplicaResultTypeDef(TypedDict):
    DBInstance: DBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
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
## PromoteReadReplicaResultTypeDef

```python
# PromoteReadReplicaResultTypeDef definition

class PromoteReadReplicaResultTypeDef(TypedDict):
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
## RestoreDBInstanceFromDBSnapshotResultTypeDef

```python
# RestoreDBInstanceFromDBSnapshotResultTypeDef definition

class RestoreDBInstanceFromDBSnapshotResultTypeDef(TypedDict):
    DBInstance: DBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreDBInstanceFromS3ResultTypeDef

```python
# RestoreDBInstanceFromS3ResultTypeDef definition

class RestoreDBInstanceFromS3ResultTypeDef(TypedDict):
    DBInstance: DBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreDBInstanceToPointInTimeResultTypeDef

```python
# RestoreDBInstanceToPointInTimeResultTypeDef definition

class RestoreDBInstanceToPointInTimeResultTypeDef(TypedDict):
    DBInstance: DBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDBInstanceResultTypeDef

```python
# StartDBInstanceResultTypeDef definition

class StartDBInstanceResultTypeDef(TypedDict):
    DBInstance: DBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopDBInstanceResultTypeDef

```python
# StopDBInstanceResultTypeDef definition

class StopDBInstanceResultTypeDef(TypedDict):
    DBInstance: DBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SwitchoverReadReplicaResultTypeDef

```python
# SwitchoverReadReplicaResultTypeDef definition

class SwitchoverReadReplicaResultTypeDef(TypedDict):
    DBInstance: DBInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBInstanceTypeDef](./type_defs.md#dbinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PerformanceIssueDetailsTypeDef

```python
# PerformanceIssueDetailsTypeDef definition

class PerformanceIssueDetailsTypeDef(TypedDict):
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Metrics: NotRequired[List[MetricTypeDef]],  # (1)
    Analysis: NotRequired[str],
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
## IssueDetailsTypeDef

```python
# IssueDetailsTypeDef definition

class IssueDetailsTypeDef(TypedDict):
    PerformanceIssueDetails: NotRequired[PerformanceIssueDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: PerformanceIssueDetailsTypeDef](./type_defs.md#performanceissuedetailstypedef) 
## RecommendedActionTypeDef

```python
# RecommendedActionTypeDef definition

class RecommendedActionTypeDef(TypedDict):
    ActionId: NotRequired[str],
    Title: NotRequired[str],
    Description: NotRequired[str],
    Operation: NotRequired[str],
    Parameters: NotRequired[List[RecommendedActionParameterTypeDef]],  # (1)
    ApplyModes: NotRequired[List[str]],
    Status: NotRequired[str],
    IssueDetails: NotRequired[IssueDetailsTypeDef],  # (2)
    ContextAttributes: NotRequired[List[ContextAttributeTypeDef]],  # (3)
```

1. See [:material-code-braces: RecommendedActionParameterTypeDef](./type_defs.md#recommendedactionparametertypedef) 
2. See [:material-code-braces: IssueDetailsTypeDef](./type_defs.md#issuedetailstypedef) 
3. See [:material-code-braces: ContextAttributeTypeDef](./type_defs.md#contextattributetypedef) 
## DBRecommendationTypeDef

```python
# DBRecommendationTypeDef definition

class DBRecommendationTypeDef(TypedDict):
    RecommendationId: NotRequired[str],
    TypeId: NotRequired[str],
    Severity: NotRequired[str],
    ResourceArn: NotRequired[str],
    Status: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    UpdatedTime: NotRequired[datetime],
    Detection: NotRequired[str],
    Recommendation: NotRequired[str],
    Description: NotRequired[str],
    Reason: NotRequired[str],
    RecommendedActions: NotRequired[List[RecommendedActionTypeDef]],  # (1)
    Category: NotRequired[str],
    Source: NotRequired[str],
    TypeDetection: NotRequired[str],
    TypeRecommendation: NotRequired[str],
    Impact: NotRequired[str],
    AdditionalInfo: NotRequired[str],
    Links: NotRequired[List[DocLinkTypeDef]],  # (2)
    IssueDetails: NotRequired[IssueDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: RecommendedActionTypeDef](./type_defs.md#recommendedactiontypedef) 
2. See [:material-code-braces: DocLinkTypeDef](./type_defs.md#doclinktypedef) 
3. See [:material-code-braces: IssueDetailsTypeDef](./type_defs.md#issuedetailstypedef) 
## DBRecommendationMessageTypeDef

```python
# DBRecommendationMessageTypeDef definition

class DBRecommendationMessageTypeDef(TypedDict):
    DBRecommendation: DBRecommendationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBRecommendationTypeDef](./type_defs.md#dbrecommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DBRecommendationsMessageTypeDef

```python
# DBRecommendationsMessageTypeDef definition

class DBRecommendationsMessageTypeDef(TypedDict):
    DBRecommendations: List[DBRecommendationTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DBRecommendationTypeDef](./type_defs.md#dbrecommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
