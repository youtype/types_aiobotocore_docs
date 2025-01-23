# Type definitions

> [Index](../README.md) > [Redshift](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Redshift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#redshift)
    type annotations stubs module [types-aiobotocore-redshift](https://pypi.org/project/types-aiobotocore-redshift/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AuthorizedTokenIssuerUnionTypeDef

```python
# AuthorizedTokenIssuerUnionTypeDef definition

AuthorizedTokenIssuerUnionTypeDef = Union[
    AuthorizedTokenIssuerTypeDef,  # (1)
    AuthorizedTokenIssuerOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AuthorizedTokenIssuerTypeDef](./type_defs.md#authorizedtokenissuertypedef) 
2. See [:material-code-braces: AuthorizedTokenIssuerOutputTypeDef](./type_defs.md#authorizedtokenissueroutputtypedef) 

## ServiceIntegrationsUnionUnionTypeDef

```python
# ServiceIntegrationsUnionUnionTypeDef definition

ServiceIntegrationsUnionUnionTypeDef = Union[
    ServiceIntegrationsUnionTypeDef,  # (1)
    ServiceIntegrationsUnionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServiceIntegrationsUnionTypeDef](./type_defs.md#serviceintegrationsuniontypedef) 
2. See [:material-code-braces: ServiceIntegrationsUnionOutputTypeDef](./type_defs.md#serviceintegrationsunionoutputtypedef) 



## AcceptReservedNodeExchangeInputMessageRequestTypeDef

```python
# AcceptReservedNodeExchangeInputMessageRequestTypeDef definition

class AcceptReservedNodeExchangeInputMessageRequestTypeDef(TypedDict):
    ReservedNodeId: str,
    TargetReservedNodeOfferingId: str,
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

## AttributeValueTargetTypeDef

```python
# AttributeValueTargetTypeDef definition

class AttributeValueTargetTypeDef(TypedDict):
    AttributeValue: NotRequired[str],
```

## AccountWithRestoreAccessTypeDef

```python
# AccountWithRestoreAccessTypeDef definition

class AccountWithRestoreAccessTypeDef(TypedDict):
    AccountId: NotRequired[str],
    AccountAlias: NotRequired[str],
```

## AquaConfigurationTypeDef

```python
# AquaConfigurationTypeDef definition

class AquaConfigurationTypeDef(TypedDict):
    AquaStatus: NotRequired[AquaStatusType],  # (1)
    AquaConfigurationStatus: NotRequired[AquaConfigurationStatusType],  # (2)
```

1. See [:material-code-brackets: AquaStatusType](./literals.md#aquastatustype) 
2. See [:material-code-brackets: AquaConfigurationStatusType](./literals.md#aquaconfigurationstatustype) 
## AssociateDataShareConsumerMessageRequestTypeDef

```python
# AssociateDataShareConsumerMessageRequestTypeDef definition

class AssociateDataShareConsumerMessageRequestTypeDef(TypedDict):
    DataShareArn: str,
    AssociateEntireAccount: NotRequired[bool],
    ConsumerArn: NotRequired[str],
    ConsumerRegion: NotRequired[str],
    AllowWrites: NotRequired[bool],
```

## CertificateAssociationTypeDef

```python
# CertificateAssociationTypeDef definition

class CertificateAssociationTypeDef(TypedDict):
    CustomDomainName: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
```

## AuthenticationProfileTypeDef

```python
# AuthenticationProfileTypeDef definition

class AuthenticationProfileTypeDef(TypedDict):
    AuthenticationProfileName: NotRequired[str],
    AuthenticationProfileContent: NotRequired[str],
```

## AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef

```python
# AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef definition

class AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef(TypedDict):
    ClusterSecurityGroupName: str,
    CIDRIP: NotRequired[str],
    EC2SecurityGroupName: NotRequired[str],
    EC2SecurityGroupOwnerId: NotRequired[str],
```

## AuthorizeDataShareMessageRequestTypeDef

```python
# AuthorizeDataShareMessageRequestTypeDef definition

class AuthorizeDataShareMessageRequestTypeDef(TypedDict):
    DataShareArn: str,
    ConsumerIdentifier: str,
    AllowWrites: NotRequired[bool],
```

## AuthorizeEndpointAccessMessageRequestTypeDef

```python
# AuthorizeEndpointAccessMessageRequestTypeDef definition

class AuthorizeEndpointAccessMessageRequestTypeDef(TypedDict):
    Account: str,
    ClusterIdentifier: NotRequired[str],
    VpcIds: NotRequired[Sequence[str]],
```

## AuthorizeSnapshotAccessMessageRequestTypeDef

```python
# AuthorizeSnapshotAccessMessageRequestTypeDef definition

class AuthorizeSnapshotAccessMessageRequestTypeDef(TypedDict):
    AccountWithRestoreAccess: str,
    SnapshotIdentifier: NotRequired[str],
    SnapshotArn: NotRequired[str],
    SnapshotClusterIdentifier: NotRequired[str],
```

## AuthorizedTokenIssuerOutputTypeDef

```python
# AuthorizedTokenIssuerOutputTypeDef definition

class AuthorizedTokenIssuerOutputTypeDef(TypedDict):
    TrustedTokenIssuerArn: NotRequired[str],
    AuthorizedAudiencesList: NotRequired[List[str]],
```

## AuthorizedTokenIssuerTypeDef

```python
# AuthorizedTokenIssuerTypeDef definition

class AuthorizedTokenIssuerTypeDef(TypedDict):
    TrustedTokenIssuerArn: NotRequired[str],
    AuthorizedAudiencesList: NotRequired[Sequence[str]],
```

## SupportedPlatformTypeDef

```python
# SupportedPlatformTypeDef definition

class SupportedPlatformTypeDef(TypedDict):
    Name: NotRequired[str],
```

## DeleteClusterSnapshotMessageTypeDef

```python
# DeleteClusterSnapshotMessageTypeDef definition

class DeleteClusterSnapshotMessageTypeDef(TypedDict):
    SnapshotIdentifier: str,
    SnapshotClusterIdentifier: NotRequired[str],
```

## SnapshotErrorMessageTypeDef

```python
# SnapshotErrorMessageTypeDef definition

class SnapshotErrorMessageTypeDef(TypedDict):
    SnapshotIdentifier: NotRequired[str],
    SnapshotClusterIdentifier: NotRequired[str],
    FailureCode: NotRequired[str],
    FailureReason: NotRequired[str],
```

## BatchModifyClusterSnapshotsMessageRequestTypeDef

```python
# BatchModifyClusterSnapshotsMessageRequestTypeDef definition

class BatchModifyClusterSnapshotsMessageRequestTypeDef(TypedDict):
    SnapshotIdentifierList: Sequence[str],
    ManualSnapshotRetentionPeriod: NotRequired[int],
    Force: NotRequired[bool],
```

## CancelResizeMessageRequestTypeDef

```python
# CancelResizeMessageRequestTypeDef definition

class CancelResizeMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## ClusterAssociatedToScheduleTypeDef

```python
# ClusterAssociatedToScheduleTypeDef definition

class ClusterAssociatedToScheduleTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    ScheduleAssociationState: NotRequired[ScheduleStateType],  # (1)
```

1. See [:material-code-brackets: ScheduleStateType](./literals.md#schedulestatetype) 
## RevisionTargetTypeDef

```python
# RevisionTargetTypeDef definition

class RevisionTargetTypeDef(TypedDict):
    DatabaseRevision: NotRequired[str],
    Description: NotRequired[str],
    DatabaseRevisionReleaseDate: NotRequired[datetime],
```

## ClusterIamRoleTypeDef

```python
# ClusterIamRoleTypeDef definition

class ClusterIamRoleTypeDef(TypedDict):
    IamRoleArn: NotRequired[str],
    ApplyStatus: NotRequired[str],
```

## ClusterNodeTypeDef

```python
# ClusterNodeTypeDef definition

class ClusterNodeTypeDef(TypedDict):
    NodeRole: NotRequired[str],
    PrivateIPAddress: NotRequired[str],
    PublicIPAddress: NotRequired[str],
```

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
    ApplyType: NotRequired[ParameterApplyTypeType],  # (1)
    IsModifiable: NotRequired[bool],
    MinimumEngineVersion: NotRequired[str],
```

1. See [:material-code-brackets: ParameterApplyTypeType](./literals.md#parameterapplytypetype) 
## ClusterParameterStatusTypeDef

```python
# ClusterParameterStatusTypeDef definition

class ClusterParameterStatusTypeDef(TypedDict):
    ParameterName: NotRequired[str],
    ParameterApplyStatus: NotRequired[str],
    ParameterApplyErrorDescription: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ClusterSecurityGroupMembershipTypeDef

```python
# ClusterSecurityGroupMembershipTypeDef definition

class ClusterSecurityGroupMembershipTypeDef(TypedDict):
    ClusterSecurityGroupName: NotRequired[str],
    Status: NotRequired[str],
```

## ClusterSnapshotCopyStatusTypeDef

```python
# ClusterSnapshotCopyStatusTypeDef definition

class ClusterSnapshotCopyStatusTypeDef(TypedDict):
    DestinationRegion: NotRequired[str],
    RetentionPeriod: NotRequired[int],
    ManualSnapshotRetentionPeriod: NotRequired[int],
    SnapshotCopyGrantName: NotRequired[str],
```

## DataTransferProgressTypeDef

```python
# DataTransferProgressTypeDef definition

class DataTransferProgressTypeDef(TypedDict):
    Status: NotRequired[str],
    CurrentRateInMegaBytesPerSecond: NotRequired[float],
    TotalDataInMegaBytes: NotRequired[int],
    DataTransferredInMegaBytes: NotRequired[int],
    EstimatedTimeToCompletionInSeconds: NotRequired[int],
    ElapsedTimeInSeconds: NotRequired[int],
```

## DeferredMaintenanceWindowTypeDef

```python
# DeferredMaintenanceWindowTypeDef definition

class DeferredMaintenanceWindowTypeDef(TypedDict):
    DeferMaintenanceIdentifier: NotRequired[str],
    DeferMaintenanceStartTime: NotRequired[datetime],
    DeferMaintenanceEndTime: NotRequired[datetime],
```

## ElasticIpStatusTypeDef

```python
# ElasticIpStatusTypeDef definition

class ElasticIpStatusTypeDef(TypedDict):
    ElasticIp: NotRequired[str],
    Status: NotRequired[str],
```

## HsmStatusTypeDef

```python
# HsmStatusTypeDef definition

class HsmStatusTypeDef(TypedDict):
    HsmClientCertificateIdentifier: NotRequired[str],
    HsmConfigurationIdentifier: NotRequired[str],
    Status: NotRequired[str],
```

## PendingModifiedValuesTypeDef

```python
# PendingModifiedValuesTypeDef definition

class PendingModifiedValuesTypeDef(TypedDict):
    MasterUserPassword: NotRequired[str],
    NodeType: NotRequired[str],
    NumberOfNodes: NotRequired[int],
    ClusterType: NotRequired[str],
    ClusterVersion: NotRequired[str],
    AutomatedSnapshotRetentionPeriod: NotRequired[int],
    ClusterIdentifier: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    EnhancedVpcRouting: NotRequired[bool],
    MaintenanceTrackName: NotRequired[str],
    EncryptionType: NotRequired[str],
```

## ReservedNodeExchangeStatusTypeDef

```python
# ReservedNodeExchangeStatusTypeDef definition

class ReservedNodeExchangeStatusTypeDef(TypedDict):
    ReservedNodeExchangeRequestId: NotRequired[str],
    Status: NotRequired[ReservedNodeExchangeStatusTypeType],  # (1)
    RequestTime: NotRequired[datetime],
    SourceReservedNodeId: NotRequired[str],
    SourceReservedNodeType: NotRequired[str],
    SourceReservedNodeCount: NotRequired[int],
    TargetReservedNodeOfferingId: NotRequired[str],
    TargetReservedNodeType: NotRequired[str],
    TargetReservedNodeCount: NotRequired[int],
```

1. See [:material-code-brackets: ReservedNodeExchangeStatusTypeType](./literals.md#reservednodeexchangestatustypetype) 
## ResizeInfoTypeDef

```python
# ResizeInfoTypeDef definition

class ResizeInfoTypeDef(TypedDict):
    ResizeType: NotRequired[str],
    AllowCancelResize: NotRequired[bool],
```

## RestoreStatusTypeDef

```python
# RestoreStatusTypeDef definition

class RestoreStatusTypeDef(TypedDict):
    Status: NotRequired[str],
    CurrentRestoreRateInMegaBytesPerSecond: NotRequired[float],
    SnapshotSizeInMegaBytes: NotRequired[int],
    ProgressInMegaBytes: NotRequired[int],
    ElapsedTimeInSeconds: NotRequired[int],
    EstimatedTimeToCompletionInSeconds: NotRequired[int],
```

## VpcSecurityGroupMembershipTypeDef

```python
# VpcSecurityGroupMembershipTypeDef definition

class VpcSecurityGroupMembershipTypeDef(TypedDict):
    VpcSecurityGroupId: NotRequired[str],
    Status: NotRequired[str],
```

## ClusterVersionTypeDef

```python
# ClusterVersionTypeDef definition

class ClusterVersionTypeDef(TypedDict):
    ClusterVersion: NotRequired[str],
    ClusterParameterGroupFamily: NotRequired[str],
    Description: NotRequired[str],
```

## CopyClusterSnapshotMessageRequestTypeDef

```python
# CopyClusterSnapshotMessageRequestTypeDef definition

class CopyClusterSnapshotMessageRequestTypeDef(TypedDict):
    SourceSnapshotIdentifier: str,
    TargetSnapshotIdentifier: str,
    SourceSnapshotClusterIdentifier: NotRequired[str],
    ManualSnapshotRetentionPeriod: NotRequired[int],
```

## CreateAuthenticationProfileMessageRequestTypeDef

```python
# CreateAuthenticationProfileMessageRequestTypeDef definition

class CreateAuthenticationProfileMessageRequestTypeDef(TypedDict):
    AuthenticationProfileName: str,
    AuthenticationProfileContent: str,
```

## CreateCustomDomainAssociationMessageRequestTypeDef

```python
# CreateCustomDomainAssociationMessageRequestTypeDef definition

class CreateCustomDomainAssociationMessageRequestTypeDef(TypedDict):
    CustomDomainName: str,
    CustomDomainCertificateArn: str,
    ClusterIdentifier: str,
```

## CreateEndpointAccessMessageRequestTypeDef

```python
# CreateEndpointAccessMessageRequestTypeDef definition

class CreateEndpointAccessMessageRequestTypeDef(TypedDict):
    EndpointName: str,
    SubnetGroupName: str,
    ClusterIdentifier: NotRequired[str],
    ResourceOwner: NotRequired[str],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
```

## DataShareAssociationTypeDef

```python
# DataShareAssociationTypeDef definition

class DataShareAssociationTypeDef(TypedDict):
    ConsumerIdentifier: NotRequired[str],
    Status: NotRequired[DataShareStatusType],  # (1)
    ConsumerRegion: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    StatusChangeDate: NotRequired[datetime],
    ProducerAllowedWrites: NotRequired[bool],
    ConsumerAcceptedWrites: NotRequired[bool],
```

1. See [:material-code-brackets: DataShareStatusType](./literals.md#datasharestatustype) 
## DeauthorizeDataShareMessageRequestTypeDef

```python
# DeauthorizeDataShareMessageRequestTypeDef definition

class DeauthorizeDataShareMessageRequestTypeDef(TypedDict):
    DataShareArn: str,
    ConsumerIdentifier: str,
```

## DeleteAuthenticationProfileMessageRequestTypeDef

```python
# DeleteAuthenticationProfileMessageRequestTypeDef definition

class DeleteAuthenticationProfileMessageRequestTypeDef(TypedDict):
    AuthenticationProfileName: str,
```

## DeleteClusterMessageRequestTypeDef

```python
# DeleteClusterMessageRequestTypeDef definition

class DeleteClusterMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    SkipFinalClusterSnapshot: NotRequired[bool],
    FinalClusterSnapshotIdentifier: NotRequired[str],
    FinalClusterSnapshotRetentionPeriod: NotRequired[int],
```

## DeleteClusterParameterGroupMessageRequestTypeDef

```python
# DeleteClusterParameterGroupMessageRequestTypeDef definition

class DeleteClusterParameterGroupMessageRequestTypeDef(TypedDict):
    ParameterGroupName: str,
```

## DeleteClusterSecurityGroupMessageRequestTypeDef

```python
# DeleteClusterSecurityGroupMessageRequestTypeDef definition

class DeleteClusterSecurityGroupMessageRequestTypeDef(TypedDict):
    ClusterSecurityGroupName: str,
```

## DeleteClusterSnapshotMessageRequestTypeDef

```python
# DeleteClusterSnapshotMessageRequestTypeDef definition

class DeleteClusterSnapshotMessageRequestTypeDef(TypedDict):
    SnapshotIdentifier: str,
    SnapshotClusterIdentifier: NotRequired[str],
```

## DeleteClusterSubnetGroupMessageRequestTypeDef

```python
# DeleteClusterSubnetGroupMessageRequestTypeDef definition

class DeleteClusterSubnetGroupMessageRequestTypeDef(TypedDict):
    ClusterSubnetGroupName: str,
```

## DeleteCustomDomainAssociationMessageRequestTypeDef

```python
# DeleteCustomDomainAssociationMessageRequestTypeDef definition

class DeleteCustomDomainAssociationMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    CustomDomainName: str,
```

## DeleteEndpointAccessMessageRequestTypeDef

```python
# DeleteEndpointAccessMessageRequestTypeDef definition

class DeleteEndpointAccessMessageRequestTypeDef(TypedDict):
    EndpointName: str,
```

## DeleteEventSubscriptionMessageRequestTypeDef

```python
# DeleteEventSubscriptionMessageRequestTypeDef definition

class DeleteEventSubscriptionMessageRequestTypeDef(TypedDict):
    SubscriptionName: str,
```

## DeleteHsmClientCertificateMessageRequestTypeDef

```python
# DeleteHsmClientCertificateMessageRequestTypeDef definition

class DeleteHsmClientCertificateMessageRequestTypeDef(TypedDict):
    HsmClientCertificateIdentifier: str,
```

## DeleteHsmConfigurationMessageRequestTypeDef

```python
# DeleteHsmConfigurationMessageRequestTypeDef definition

class DeleteHsmConfigurationMessageRequestTypeDef(TypedDict):
    HsmConfigurationIdentifier: str,
```

## DeleteIntegrationMessageRequestTypeDef

```python
# DeleteIntegrationMessageRequestTypeDef definition

class DeleteIntegrationMessageRequestTypeDef(TypedDict):
    IntegrationArn: str,
```

## DeleteRedshiftIdcApplicationMessageRequestTypeDef

```python
# DeleteRedshiftIdcApplicationMessageRequestTypeDef definition

class DeleteRedshiftIdcApplicationMessageRequestTypeDef(TypedDict):
    RedshiftIdcApplicationArn: str,
```

## DeleteResourcePolicyMessageRequestTypeDef

```python
# DeleteResourcePolicyMessageRequestTypeDef definition

class DeleteResourcePolicyMessageRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DeleteScheduledActionMessageRequestTypeDef

```python
# DeleteScheduledActionMessageRequestTypeDef definition

class DeleteScheduledActionMessageRequestTypeDef(TypedDict):
    ScheduledActionName: str,
```

## DeleteSnapshotCopyGrantMessageRequestTypeDef

```python
# DeleteSnapshotCopyGrantMessageRequestTypeDef definition

class DeleteSnapshotCopyGrantMessageRequestTypeDef(TypedDict):
    SnapshotCopyGrantName: str,
```

## DeleteSnapshotScheduleMessageRequestTypeDef

```python
# DeleteSnapshotScheduleMessageRequestTypeDef definition

class DeleteSnapshotScheduleMessageRequestTypeDef(TypedDict):
    ScheduleIdentifier: str,
```

## DeleteTagsMessageRequestTypeDef

```python
# DeleteTagsMessageRequestTypeDef definition

class DeleteTagsMessageRequestTypeDef(TypedDict):
    ResourceName: str,
    TagKeys: Sequence[str],
```

## DeleteUsageLimitMessageRequestTypeDef

```python
# DeleteUsageLimitMessageRequestTypeDef definition

class DeleteUsageLimitMessageRequestTypeDef(TypedDict):
    UsageLimitId: str,
```

## DescribeAccountAttributesMessageRequestTypeDef

```python
# DescribeAccountAttributesMessageRequestTypeDef definition

class DescribeAccountAttributesMessageRequestTypeDef(TypedDict):
    AttributeNames: NotRequired[Sequence[str]],
```

## DescribeAuthenticationProfilesMessageRequestTypeDef

```python
# DescribeAuthenticationProfilesMessageRequestTypeDef definition

class DescribeAuthenticationProfilesMessageRequestTypeDef(TypedDict):
    AuthenticationProfileName: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeClusterDbRevisionsMessageRequestTypeDef

```python
# DescribeClusterDbRevisionsMessageRequestTypeDef definition

class DescribeClusterDbRevisionsMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeClusterParameterGroupsMessageRequestTypeDef

```python
# DescribeClusterParameterGroupsMessageRequestTypeDef definition

class DescribeClusterParameterGroupsMessageRequestTypeDef(TypedDict):
    ParameterGroupName: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
```

## DescribeClusterParametersMessageRequestTypeDef

```python
# DescribeClusterParametersMessageRequestTypeDef definition

class DescribeClusterParametersMessageRequestTypeDef(TypedDict):
    ParameterGroupName: str,
    Source: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeClusterSecurityGroupsMessageRequestTypeDef

```python
# DescribeClusterSecurityGroupsMessageRequestTypeDef definition

class DescribeClusterSecurityGroupsMessageRequestTypeDef(TypedDict):
    ClusterSecurityGroupName: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
```

## SnapshotSortingEntityTypeDef

```python
# SnapshotSortingEntityTypeDef definition

class SnapshotSortingEntityTypeDef(TypedDict):
    Attribute: SnapshotAttributeToSortByType,  # (1)
    SortOrder: NotRequired[SortByOrderType],  # (2)
```

1. See [:material-code-brackets: SnapshotAttributeToSortByType](./literals.md#snapshotattributetosortbytype) 
2. See [:material-code-brackets: SortByOrderType](./literals.md#sortbyordertype) 
## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeClusterSubnetGroupsMessageRequestTypeDef

```python
# DescribeClusterSubnetGroupsMessageRequestTypeDef definition

class DescribeClusterSubnetGroupsMessageRequestTypeDef(TypedDict):
    ClusterSubnetGroupName: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
```

## DescribeClusterTracksMessageRequestTypeDef

```python
# DescribeClusterTracksMessageRequestTypeDef definition

class DescribeClusterTracksMessageRequestTypeDef(TypedDict):
    MaintenanceTrackName: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeClusterVersionsMessageRequestTypeDef

```python
# DescribeClusterVersionsMessageRequestTypeDef definition

class DescribeClusterVersionsMessageRequestTypeDef(TypedDict):
    ClusterVersion: NotRequired[str],
    ClusterParameterGroupFamily: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeClustersMessageRequestTypeDef

```python
# DescribeClustersMessageRequestTypeDef definition

class DescribeClustersMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
```

## DescribeCustomDomainAssociationsMessageRequestTypeDef

```python
# DescribeCustomDomainAssociationsMessageRequestTypeDef definition

class DescribeCustomDomainAssociationsMessageRequestTypeDef(TypedDict):
    CustomDomainName: NotRequired[str],
    CustomDomainCertificateArn: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeDataSharesForConsumerMessageRequestTypeDef

```python
# DescribeDataSharesForConsumerMessageRequestTypeDef definition

class DescribeDataSharesForConsumerMessageRequestTypeDef(TypedDict):
    ConsumerArn: NotRequired[str],
    Status: NotRequired[DataShareStatusForConsumerType],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: DataShareStatusForConsumerType](./literals.md#datasharestatusforconsumertype) 
## DescribeDataSharesForProducerMessageRequestTypeDef

```python
# DescribeDataSharesForProducerMessageRequestTypeDef definition

class DescribeDataSharesForProducerMessageRequestTypeDef(TypedDict):
    ProducerArn: NotRequired[str],
    Status: NotRequired[DataShareStatusForProducerType],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: DataShareStatusForProducerType](./literals.md#datasharestatusforproducertype) 
## DescribeDataSharesMessageRequestTypeDef

```python
# DescribeDataSharesMessageRequestTypeDef definition

class DescribeDataSharesMessageRequestTypeDef(TypedDict):
    DataShareArn: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeDefaultClusterParametersMessageRequestTypeDef

```python
# DescribeDefaultClusterParametersMessageRequestTypeDef definition

class DescribeDefaultClusterParametersMessageRequestTypeDef(TypedDict):
    ParameterGroupFamily: str,
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeEndpointAccessMessageRequestTypeDef

```python
# DescribeEndpointAccessMessageRequestTypeDef definition

class DescribeEndpointAccessMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    ResourceOwner: NotRequired[str],
    EndpointName: NotRequired[str],
    VpcId: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeEndpointAuthorizationMessageRequestTypeDef

```python
# DescribeEndpointAuthorizationMessageRequestTypeDef definition

class DescribeEndpointAuthorizationMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    Account: NotRequired[str],
    Grantee: NotRequired[bool],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeEventCategoriesMessageRequestTypeDef

```python
# DescribeEventCategoriesMessageRequestTypeDef definition

class DescribeEventCategoriesMessageRequestTypeDef(TypedDict):
    SourceType: NotRequired[str],
```

## DescribeEventSubscriptionsMessageRequestTypeDef

```python
# DescribeEventSubscriptionsMessageRequestTypeDef definition

class DescribeEventSubscriptionsMessageRequestTypeDef(TypedDict):
    SubscriptionName: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
```

## DescribeHsmClientCertificatesMessageRequestTypeDef

```python
# DescribeHsmClientCertificatesMessageRequestTypeDef definition

class DescribeHsmClientCertificatesMessageRequestTypeDef(TypedDict):
    HsmClientCertificateIdentifier: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
```

## DescribeHsmConfigurationsMessageRequestTypeDef

```python
# DescribeHsmConfigurationsMessageRequestTypeDef definition

class DescribeHsmConfigurationsMessageRequestTypeDef(TypedDict):
    HsmConfigurationIdentifier: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
```

## DescribeInboundIntegrationsMessageRequestTypeDef

```python
# DescribeInboundIntegrationsMessageRequestTypeDef definition

class DescribeInboundIntegrationsMessageRequestTypeDef(TypedDict):
    IntegrationArn: NotRequired[str],
    TargetArn: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeIntegrationsFilterTypeDef

```python
# DescribeIntegrationsFilterTypeDef definition

class DescribeIntegrationsFilterTypeDef(TypedDict):
    Name: DescribeIntegrationsFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: DescribeIntegrationsFilterNameType](./literals.md#describeintegrationsfilternametype) 
## DescribeLoggingStatusMessageRequestTypeDef

```python
# DescribeLoggingStatusMessageRequestTypeDef definition

class DescribeLoggingStatusMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## NodeConfigurationOptionsFilterTypeDef

```python
# NodeConfigurationOptionsFilterTypeDef definition

class NodeConfigurationOptionsFilterTypeDef(TypedDict):
    Name: NotRequired[NodeConfigurationOptionsFilterNameType],  # (1)
    Operator: NotRequired[OperatorTypeType],  # (2)
    Values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: NodeConfigurationOptionsFilterNameType](./literals.md#nodeconfigurationoptionsfilternametype) 
2. See [:material-code-brackets: OperatorTypeType](./literals.md#operatortypetype) 
## DescribeOrderableClusterOptionsMessageRequestTypeDef

```python
# DescribeOrderableClusterOptionsMessageRequestTypeDef definition

class DescribeOrderableClusterOptionsMessageRequestTypeDef(TypedDict):
    ClusterVersion: NotRequired[str],
    NodeType: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribePartnersInputMessageRequestTypeDef

```python
# DescribePartnersInputMessageRequestTypeDef definition

class DescribePartnersInputMessageRequestTypeDef(TypedDict):
    AccountId: str,
    ClusterIdentifier: str,
    DatabaseName: NotRequired[str],
    PartnerName: NotRequired[str],
```

## PartnerIntegrationInfoTypeDef

```python
# PartnerIntegrationInfoTypeDef definition

class PartnerIntegrationInfoTypeDef(TypedDict):
    DatabaseName: NotRequired[str],
    PartnerName: NotRequired[str],
    Status: NotRequired[PartnerIntegrationStatusType],  # (1)
    StatusMessage: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: PartnerIntegrationStatusType](./literals.md#partnerintegrationstatustype) 
## DescribeRedshiftIdcApplicationsMessageRequestTypeDef

```python
# DescribeRedshiftIdcApplicationsMessageRequestTypeDef definition

class DescribeRedshiftIdcApplicationsMessageRequestTypeDef(TypedDict):
    RedshiftIdcApplicationArn: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef

```python
# DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef definition

class DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef(TypedDict):
    ReservedNodeId: NotRequired[str],
    ReservedNodeExchangeRequestId: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeReservedNodeOfferingsMessageRequestTypeDef

```python
# DescribeReservedNodeOfferingsMessageRequestTypeDef definition

class DescribeReservedNodeOfferingsMessageRequestTypeDef(TypedDict):
    ReservedNodeOfferingId: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeReservedNodesMessageRequestTypeDef

```python
# DescribeReservedNodesMessageRequestTypeDef definition

class DescribeReservedNodesMessageRequestTypeDef(TypedDict):
    ReservedNodeId: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeResizeMessageRequestTypeDef

```python
# DescribeResizeMessageRequestTypeDef definition

class DescribeResizeMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## ScheduledActionFilterTypeDef

```python
# ScheduledActionFilterTypeDef definition

class ScheduledActionFilterTypeDef(TypedDict):
    Name: ScheduledActionFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: ScheduledActionFilterNameType](./literals.md#scheduledactionfilternametype) 
## DescribeSnapshotCopyGrantsMessageRequestTypeDef

```python
# DescribeSnapshotCopyGrantsMessageRequestTypeDef definition

class DescribeSnapshotCopyGrantsMessageRequestTypeDef(TypedDict):
    SnapshotCopyGrantName: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
```

## DescribeSnapshotSchedulesMessageRequestTypeDef

```python
# DescribeSnapshotSchedulesMessageRequestTypeDef definition

class DescribeSnapshotSchedulesMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    ScheduleIdentifier: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

## DescribeTableRestoreStatusMessageRequestTypeDef

```python
# DescribeTableRestoreStatusMessageRequestTypeDef definition

class DescribeTableRestoreStatusMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    TableRestoreRequestId: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeTagsMessageRequestTypeDef

```python
# DescribeTagsMessageRequestTypeDef definition

class DescribeTagsMessageRequestTypeDef(TypedDict):
    ResourceName: NotRequired[str],
    ResourceType: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
```

## DescribeUsageLimitsMessageRequestTypeDef

```python
# DescribeUsageLimitsMessageRequestTypeDef definition

class DescribeUsageLimitsMessageRequestTypeDef(TypedDict):
    UsageLimitId: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
    FeatureType: NotRequired[UsageLimitFeatureTypeType],  # (1)
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: UsageLimitFeatureTypeType](./literals.md#usagelimitfeaturetypetype) 
## DisableLoggingMessageRequestTypeDef

```python
# DisableLoggingMessageRequestTypeDef definition

class DisableLoggingMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## DisableSnapshotCopyMessageRequestTypeDef

```python
# DisableSnapshotCopyMessageRequestTypeDef definition

class DisableSnapshotCopyMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## DisassociateDataShareConsumerMessageRequestTypeDef

```python
# DisassociateDataShareConsumerMessageRequestTypeDef definition

class DisassociateDataShareConsumerMessageRequestTypeDef(TypedDict):
    DataShareArn: str,
    DisassociateEntireAccount: NotRequired[bool],
    ConsumerArn: NotRequired[str],
    ConsumerRegion: NotRequired[str],
```

## EnableLoggingMessageRequestTypeDef

```python
# EnableLoggingMessageRequestTypeDef definition

class EnableLoggingMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    BucketName: NotRequired[str],
    S3KeyPrefix: NotRequired[str],
    LogDestinationType: NotRequired[LogDestinationTypeType],  # (1)
    LogExports: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: LogDestinationTypeType](./literals.md#logdestinationtypetype) 
## EnableSnapshotCopyMessageRequestTypeDef

```python
# EnableSnapshotCopyMessageRequestTypeDef definition

class EnableSnapshotCopyMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    DestinationRegion: str,
    RetentionPeriod: NotRequired[int],
    SnapshotCopyGrantName: NotRequired[str],
    ManualSnapshotRetentionPeriod: NotRequired[int],
```

## EndpointAuthorizationTypeDef

```python
# EndpointAuthorizationTypeDef definition

class EndpointAuthorizationTypeDef(TypedDict):
    Grantor: NotRequired[str],
    Grantee: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
    AuthorizeTime: NotRequired[datetime],
    ClusterStatus: NotRequired[str],
    Status: NotRequired[AuthorizationStatusType],  # (1)
    AllowedAllVPCs: NotRequired[bool],
    AllowedVPCs: NotRequired[List[str]],
    EndpointCount: NotRequired[int],
```

1. See [:material-code-brackets: AuthorizationStatusType](./literals.md#authorizationstatustype) 
## EventInfoMapTypeDef

```python
# EventInfoMapTypeDef definition

class EventInfoMapTypeDef(TypedDict):
    EventId: NotRequired[str],
    EventCategories: NotRequired[List[str]],
    EventDescription: NotRequired[str],
    Severity: NotRequired[str],
```

## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    SourceIdentifier: NotRequired[str],
    SourceType: NotRequired[SourceTypeType],  # (1)
    Message: NotRequired[str],
    EventCategories: NotRequired[List[str]],
    Severity: NotRequired[str],
    Date: NotRequired[datetime],
    EventId: NotRequired[str],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
## FailoverPrimaryComputeInputMessageRequestTypeDef

```python
# FailoverPrimaryComputeInputMessageRequestTypeDef definition

class FailoverPrimaryComputeInputMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## GetClusterCredentialsMessageRequestTypeDef

```python
# GetClusterCredentialsMessageRequestTypeDef definition

class GetClusterCredentialsMessageRequestTypeDef(TypedDict):
    DbUser: str,
    DbName: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
    DurationSeconds: NotRequired[int],
    AutoCreate: NotRequired[bool],
    DbGroups: NotRequired[Sequence[str]],
    CustomDomainName: NotRequired[str],
```

## GetClusterCredentialsWithIAMMessageRequestTypeDef

```python
# GetClusterCredentialsWithIAMMessageRequestTypeDef definition

class GetClusterCredentialsWithIAMMessageRequestTypeDef(TypedDict):
    DbName: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
    DurationSeconds: NotRequired[int],
    CustomDomainName: NotRequired[str],
```

## GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef

```python
# GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef definition

class GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef(TypedDict):
    ActionType: ReservedNodeExchangeActionTypeType,  # (1)
    ClusterIdentifier: NotRequired[str],
    SnapshotIdentifier: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: ReservedNodeExchangeActionTypeType](./literals.md#reservednodeexchangeactiontypetype) 
## GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef

```python
# GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef definition

class GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef(TypedDict):
    ReservedNodeId: str,
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## GetResourcePolicyMessageRequestTypeDef

```python
# GetResourcePolicyMessageRequestTypeDef definition

class GetResourcePolicyMessageRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ResourcePolicyTypeDef

```python
# ResourcePolicyTypeDef definition

class ResourcePolicyTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    Policy: NotRequired[str],
```

## IntegrationErrorTypeDef

```python
# IntegrationErrorTypeDef definition

class IntegrationErrorTypeDef(TypedDict):
    ErrorCode: str,
    ErrorMessage: NotRequired[str],
```

## LakeFormationQueryTypeDef

```python
# LakeFormationQueryTypeDef definition

class LakeFormationQueryTypeDef(TypedDict):
    Authorization: ServiceAuthorizationType,  # (1)
```

1. See [:material-code-brackets: ServiceAuthorizationType](./literals.md#serviceauthorizationtype) 
## ListRecommendationsMessageRequestTypeDef

```python
# ListRecommendationsMessageRequestTypeDef definition

class ListRecommendationsMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    NamespaceArn: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
```

## ModifyAquaInputMessageRequestTypeDef

```python
# ModifyAquaInputMessageRequestTypeDef definition

class ModifyAquaInputMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    AquaConfigurationStatus: NotRequired[AquaConfigurationStatusType],  # (1)
```

1. See [:material-code-brackets: AquaConfigurationStatusType](./literals.md#aquaconfigurationstatustype) 
## ModifyAuthenticationProfileMessageRequestTypeDef

```python
# ModifyAuthenticationProfileMessageRequestTypeDef definition

class ModifyAuthenticationProfileMessageRequestTypeDef(TypedDict):
    AuthenticationProfileName: str,
    AuthenticationProfileContent: str,
```

## ModifyClusterDbRevisionMessageRequestTypeDef

```python
# ModifyClusterDbRevisionMessageRequestTypeDef definition

class ModifyClusterDbRevisionMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    RevisionTarget: str,
```

## ModifyClusterIamRolesMessageRequestTypeDef

```python
# ModifyClusterIamRolesMessageRequestTypeDef definition

class ModifyClusterIamRolesMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    AddIamRoles: NotRequired[Sequence[str]],
    RemoveIamRoles: NotRequired[Sequence[str]],
    DefaultIamRoleArn: NotRequired[str],
```

## ModifyClusterMessageRequestTypeDef

```python
# ModifyClusterMessageRequestTypeDef definition

class ModifyClusterMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    ClusterType: NotRequired[str],
    NodeType: NotRequired[str],
    NumberOfNodes: NotRequired[int],
    ClusterSecurityGroups: NotRequired[Sequence[str]],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    MasterUserPassword: NotRequired[str],
    ClusterParameterGroupName: NotRequired[str],
    AutomatedSnapshotRetentionPeriod: NotRequired[int],
    ManualSnapshotRetentionPeriod: NotRequired[int],
    PreferredMaintenanceWindow: NotRequired[str],
    ClusterVersion: NotRequired[str],
    AllowVersionUpgrade: NotRequired[bool],
    HsmClientCertificateIdentifier: NotRequired[str],
    HsmConfigurationIdentifier: NotRequired[str],
    NewClusterIdentifier: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    ElasticIp: NotRequired[str],
    EnhancedVpcRouting: NotRequired[bool],
    MaintenanceTrackName: NotRequired[str],
    Encrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    AvailabilityZoneRelocation: NotRequired[bool],
    AvailabilityZone: NotRequired[str],
    Port: NotRequired[int],
    ManageMasterPassword: NotRequired[bool],
    MasterPasswordSecretKmsKeyId: NotRequired[str],
    IpAddressType: NotRequired[str],
    MultiAZ: NotRequired[bool],
```

## ModifyClusterSnapshotMessageRequestTypeDef

```python
# ModifyClusterSnapshotMessageRequestTypeDef definition

class ModifyClusterSnapshotMessageRequestTypeDef(TypedDict):
    SnapshotIdentifier: str,
    ManualSnapshotRetentionPeriod: NotRequired[int],
    Force: NotRequired[bool],
```

## ModifyClusterSnapshotScheduleMessageRequestTypeDef

```python
# ModifyClusterSnapshotScheduleMessageRequestTypeDef definition

class ModifyClusterSnapshotScheduleMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    ScheduleIdentifier: NotRequired[str],
    DisassociateSchedule: NotRequired[bool],
```

## ModifyClusterSubnetGroupMessageRequestTypeDef

```python
# ModifyClusterSubnetGroupMessageRequestTypeDef definition

class ModifyClusterSubnetGroupMessageRequestTypeDef(TypedDict):
    ClusterSubnetGroupName: str,
    SubnetIds: Sequence[str],
    Description: NotRequired[str],
```

## ModifyCustomDomainAssociationMessageRequestTypeDef

```python
# ModifyCustomDomainAssociationMessageRequestTypeDef definition

class ModifyCustomDomainAssociationMessageRequestTypeDef(TypedDict):
    CustomDomainName: str,
    CustomDomainCertificateArn: str,
    ClusterIdentifier: str,
```

## ModifyEndpointAccessMessageRequestTypeDef

```python
# ModifyEndpointAccessMessageRequestTypeDef definition

class ModifyEndpointAccessMessageRequestTypeDef(TypedDict):
    EndpointName: str,
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
```

## ModifyEventSubscriptionMessageRequestTypeDef

```python
# ModifyEventSubscriptionMessageRequestTypeDef definition

class ModifyEventSubscriptionMessageRequestTypeDef(TypedDict):
    SubscriptionName: str,
    SnsTopicArn: NotRequired[str],
    SourceType: NotRequired[str],
    SourceIds: NotRequired[Sequence[str]],
    EventCategories: NotRequired[Sequence[str]],
    Severity: NotRequired[str],
    Enabled: NotRequired[bool],
```

## ModifyIntegrationMessageRequestTypeDef

```python
# ModifyIntegrationMessageRequestTypeDef definition

class ModifyIntegrationMessageRequestTypeDef(TypedDict):
    IntegrationArn: str,
    Description: NotRequired[str],
    IntegrationName: NotRequired[str],
```

## ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef

```python
# ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef definition

class ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    RetentionPeriod: int,
    Manual: NotRequired[bool],
```

## ModifySnapshotScheduleMessageRequestTypeDef

```python
# ModifySnapshotScheduleMessageRequestTypeDef definition

class ModifySnapshotScheduleMessageRequestTypeDef(TypedDict):
    ScheduleIdentifier: str,
    ScheduleDefinitions: Sequence[str],
```

## ModifyUsageLimitMessageRequestTypeDef

```python
# ModifyUsageLimitMessageRequestTypeDef definition

class ModifyUsageLimitMessageRequestTypeDef(TypedDict):
    UsageLimitId: str,
    Amount: NotRequired[int],
    BreachAction: NotRequired[UsageLimitBreachActionType],  # (1)
```

1. See [:material-code-brackets: UsageLimitBreachActionType](./literals.md#usagelimitbreachactiontype) 
## ProvisionedIdentifierTypeDef

```python
# ProvisionedIdentifierTypeDef definition

class ProvisionedIdentifierTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## ServerlessIdentifierTypeDef

```python
# ServerlessIdentifierTypeDef definition

class ServerlessIdentifierTypeDef(TypedDict):
    NamespaceIdentifier: str,
    WorkgroupIdentifier: str,
```

## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    NetworkInterfaceId: NotRequired[str],
    SubnetId: NotRequired[str],
    PrivateIpAddress: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    Ipv6Address: NotRequired[str],
```

## NodeConfigurationOptionTypeDef

```python
# NodeConfigurationOptionTypeDef definition

class NodeConfigurationOptionTypeDef(TypedDict):
    NodeType: NotRequired[str],
    NumberOfNodes: NotRequired[int],
    EstimatedDiskUtilizationPercent: NotRequired[float],
    Mode: NotRequired[ModeType],  # (1)
```

1. See [:material-code-brackets: ModeType](./literals.md#modetype) 
## PartnerIntegrationInputMessageRequestTypeDef

```python
# PartnerIntegrationInputMessageRequestTypeDef definition

class PartnerIntegrationInputMessageRequestTypeDef(TypedDict):
    AccountId: str,
    ClusterIdentifier: str,
    DatabaseName: str,
    PartnerName: str,
```

## PauseClusterMessageRequestTypeDef

```python
# PauseClusterMessageRequestTypeDef definition

class PauseClusterMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## PauseClusterMessageTypeDef

```python
# PauseClusterMessageTypeDef definition

class PauseClusterMessageTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## PurchaseReservedNodeOfferingMessageRequestTypeDef

```python
# PurchaseReservedNodeOfferingMessageRequestTypeDef definition

class PurchaseReservedNodeOfferingMessageRequestTypeDef(TypedDict):
    ReservedNodeOfferingId: str,
    NodeCount: NotRequired[int],
```

## PutResourcePolicyMessageRequestTypeDef

```python
# PutResourcePolicyMessageRequestTypeDef definition

class PutResourcePolicyMessageRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
```

## ReadWriteAccessTypeDef

```python
# ReadWriteAccessTypeDef definition

class ReadWriteAccessTypeDef(TypedDict):
    Authorization: ServiceAuthorizationType,  # (1)
```

1. See [:material-code-brackets: ServiceAuthorizationType](./literals.md#serviceauthorizationtype) 
## RebootClusterMessageRequestTypeDef

```python
# RebootClusterMessageRequestTypeDef definition

class RebootClusterMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## RecommendedActionTypeDef

```python
# RecommendedActionTypeDef definition

class RecommendedActionTypeDef(TypedDict):
    Text: NotRequired[str],
    Database: NotRequired[str],
    Command: NotRequired[str],
    Type: NotRequired[RecommendedActionTypeType],  # (1)
```

1. See [:material-code-brackets: RecommendedActionTypeType](./literals.md#recommendedactiontypetype) 
## ReferenceLinkTypeDef

```python
# ReferenceLinkTypeDef definition

class ReferenceLinkTypeDef(TypedDict):
    Text: NotRequired[str],
    Link: NotRequired[str],
```

## RecurringChargeTypeDef

```python
# RecurringChargeTypeDef definition

class RecurringChargeTypeDef(TypedDict):
    RecurringChargeAmount: NotRequired[float],
    RecurringChargeFrequency: NotRequired[str],
```

## RejectDataShareMessageRequestTypeDef

```python
# RejectDataShareMessageRequestTypeDef definition

class RejectDataShareMessageRequestTypeDef(TypedDict):
    DataShareArn: str,
```

## ResizeClusterMessageRequestTypeDef

```python
# ResizeClusterMessageRequestTypeDef definition

class ResizeClusterMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    ClusterType: NotRequired[str],
    NodeType: NotRequired[str],
    NumberOfNodes: NotRequired[int],
    Classic: NotRequired[bool],
    ReservedNodeId: NotRequired[str],
    TargetReservedNodeOfferingId: NotRequired[str],
```

## ResizeClusterMessageTypeDef

```python
# ResizeClusterMessageTypeDef definition

class ResizeClusterMessageTypeDef(TypedDict):
    ClusterIdentifier: str,
    ClusterType: NotRequired[str],
    NodeType: NotRequired[str],
    NumberOfNodes: NotRequired[int],
    Classic: NotRequired[bool],
    ReservedNodeId: NotRequired[str],
    TargetReservedNodeOfferingId: NotRequired[str],
```

## RestoreFromClusterSnapshotMessageRequestTypeDef

```python
# RestoreFromClusterSnapshotMessageRequestTypeDef definition

class RestoreFromClusterSnapshotMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    SnapshotIdentifier: NotRequired[str],
    SnapshotArn: NotRequired[str],
    SnapshotClusterIdentifier: NotRequired[str],
    Port: NotRequired[int],
    AvailabilityZone: NotRequired[str],
    AllowVersionUpgrade: NotRequired[bool],
    ClusterSubnetGroupName: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    OwnerAccount: NotRequired[str],
    HsmClientCertificateIdentifier: NotRequired[str],
    HsmConfigurationIdentifier: NotRequired[str],
    ElasticIp: NotRequired[str],
    ClusterParameterGroupName: NotRequired[str],
    ClusterSecurityGroups: NotRequired[Sequence[str]],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    PreferredMaintenanceWindow: NotRequired[str],
    AutomatedSnapshotRetentionPeriod: NotRequired[int],
    ManualSnapshotRetentionPeriod: NotRequired[int],
    KmsKeyId: NotRequired[str],
    NodeType: NotRequired[str],
    EnhancedVpcRouting: NotRequired[bool],
    AdditionalInfo: NotRequired[str],
    IamRoles: NotRequired[Sequence[str]],
    MaintenanceTrackName: NotRequired[str],
    SnapshotScheduleIdentifier: NotRequired[str],
    NumberOfNodes: NotRequired[int],
    AvailabilityZoneRelocation: NotRequired[bool],
    AquaConfigurationStatus: NotRequired[AquaConfigurationStatusType],  # (1)
    DefaultIamRoleArn: NotRequired[str],
    ReservedNodeId: NotRequired[str],
    TargetReservedNodeOfferingId: NotRequired[str],
    Encrypted: NotRequired[bool],
    ManageMasterPassword: NotRequired[bool],
    MasterPasswordSecretKmsKeyId: NotRequired[str],
    IpAddressType: NotRequired[str],
    MultiAZ: NotRequired[bool],
```

1. See [:material-code-brackets: AquaConfigurationStatusType](./literals.md#aquaconfigurationstatustype) 
## RestoreTableFromClusterSnapshotMessageRequestTypeDef

```python
# RestoreTableFromClusterSnapshotMessageRequestTypeDef definition

class RestoreTableFromClusterSnapshotMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    SnapshotIdentifier: str,
    SourceDatabaseName: str,
    SourceTableName: str,
    NewTableName: str,
    SourceSchemaName: NotRequired[str],
    TargetDatabaseName: NotRequired[str],
    TargetSchemaName: NotRequired[str],
    EnableCaseSensitiveIdentifier: NotRequired[bool],
```

## TableRestoreStatusTypeDef

```python
# TableRestoreStatusTypeDef definition

class TableRestoreStatusTypeDef(TypedDict):
    TableRestoreRequestId: NotRequired[str],
    Status: NotRequired[TableRestoreStatusTypeType],  # (1)
    Message: NotRequired[str],
    RequestTime: NotRequired[datetime],
    ProgressInMegaBytes: NotRequired[int],
    TotalDataInMegaBytes: NotRequired[int],
    ClusterIdentifier: NotRequired[str],
    SnapshotIdentifier: NotRequired[str],
    SourceDatabaseName: NotRequired[str],
    SourceSchemaName: NotRequired[str],
    SourceTableName: NotRequired[str],
    TargetDatabaseName: NotRequired[str],
    TargetSchemaName: NotRequired[str],
    NewTableName: NotRequired[str],
```

1. See [:material-code-brackets: TableRestoreStatusTypeType](./literals.md#tablerestorestatustypetype) 
## ResumeClusterMessageRequestTypeDef

```python
# ResumeClusterMessageRequestTypeDef definition

class ResumeClusterMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## ResumeClusterMessageTypeDef

```python
# ResumeClusterMessageTypeDef definition

class ResumeClusterMessageTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## RevokeClusterSecurityGroupIngressMessageRequestTypeDef

```python
# RevokeClusterSecurityGroupIngressMessageRequestTypeDef definition

class RevokeClusterSecurityGroupIngressMessageRequestTypeDef(TypedDict):
    ClusterSecurityGroupName: str,
    CIDRIP: NotRequired[str],
    EC2SecurityGroupName: NotRequired[str],
    EC2SecurityGroupOwnerId: NotRequired[str],
```

## RevokeEndpointAccessMessageRequestTypeDef

```python
# RevokeEndpointAccessMessageRequestTypeDef definition

class RevokeEndpointAccessMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    Account: NotRequired[str],
    VpcIds: NotRequired[Sequence[str]],
    Force: NotRequired[bool],
```

## RevokeSnapshotAccessMessageRequestTypeDef

```python
# RevokeSnapshotAccessMessageRequestTypeDef definition

class RevokeSnapshotAccessMessageRequestTypeDef(TypedDict):
    AccountWithRestoreAccess: str,
    SnapshotIdentifier: NotRequired[str],
    SnapshotArn: NotRequired[str],
    SnapshotClusterIdentifier: NotRequired[str],
```

## RotateEncryptionKeyMessageRequestTypeDef

```python
# RotateEncryptionKeyMessageRequestTypeDef definition

class RotateEncryptionKeyMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
```

## SupportedOperationTypeDef

```python
# SupportedOperationTypeDef definition

class SupportedOperationTypeDef(TypedDict):
    OperationName: NotRequired[str],
```

## UpdatePartnerStatusInputMessageRequestTypeDef

```python
# UpdatePartnerStatusInputMessageRequestTypeDef definition

class UpdatePartnerStatusInputMessageRequestTypeDef(TypedDict):
    AccountId: str,
    ClusterIdentifier: str,
    DatabaseName: str,
    PartnerName: str,
    Status: PartnerIntegrationStatusType,  # (1)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: PartnerIntegrationStatusType](./literals.md#partnerintegrationstatustype) 
## ClusterCredentialsTypeDef

```python
# ClusterCredentialsTypeDef definition

class ClusterCredentialsTypeDef(TypedDict):
    DbUser: str,
    DbPassword: str,
    Expiration: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterExtendedCredentialsTypeDef

```python
# ClusterExtendedCredentialsTypeDef definition

class ClusterExtendedCredentialsTypeDef(TypedDict):
    DbUser: str,
    DbPassword: str,
    Expiration: datetime,
    NextRefreshTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterParameterGroupNameMessageTypeDef

```python
# ClusterParameterGroupNameMessageTypeDef definition

class ClusterParameterGroupNameMessageTypeDef(TypedDict):
    ParameterGroupName: str,
    ParameterGroupStatus: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAuthenticationProfileResultTypeDef

```python
# CreateAuthenticationProfileResultTypeDef definition

class CreateAuthenticationProfileResultTypeDef(TypedDict):
    AuthenticationProfileName: str,
    AuthenticationProfileContent: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomDomainAssociationResultTypeDef

```python
# CreateCustomDomainAssociationResultTypeDef definition

class CreateCustomDomainAssociationResultTypeDef(TypedDict):
    CustomDomainName: str,
    CustomDomainCertificateArn: str,
    ClusterIdentifier: str,
    CustomDomainCertExpiryTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomerStorageMessageTypeDef

```python
# CustomerStorageMessageTypeDef definition

class CustomerStorageMessageTypeDef(TypedDict):
    TotalBackupSizeInMegaBytes: float,
    TotalProvisionedStorageInMegaBytes: float,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAuthenticationProfileResultTypeDef

```python
# DeleteAuthenticationProfileResultTypeDef definition

class DeleteAuthenticationProfileResultTypeDef(TypedDict):
    AuthenticationProfileName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterNamespaceOutputMessageTypeDef

```python
# DeregisterNamespaceOutputMessageTypeDef definition

class DeregisterNamespaceOutputMessageTypeDef(TypedDict):
    Status: NamespaceRegistrationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: NamespaceRegistrationStatusType](./literals.md#namespaceregistrationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EndpointAuthorizationResponseTypeDef

```python
# EndpointAuthorizationResponseTypeDef definition

class EndpointAuthorizationResponseTypeDef(TypedDict):
    Grantor: str,
    Grantee: str,
    ClusterIdentifier: str,
    AuthorizeTime: datetime,
    ClusterStatus: str,
    Status: AuthorizationStatusType,  # (1)
    AllowedAllVPCs: bool,
    AllowedVPCs: List[str],
    EndpointCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AuthorizationStatusType](./literals.md#authorizationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoggingStatusTypeDef

```python
# LoggingStatusTypeDef definition

class LoggingStatusTypeDef(TypedDict):
    LoggingEnabled: bool,
    BucketName: str,
    S3KeyPrefix: str,
    LastSuccessfulDeliveryTime: datetime,
    LastFailureTime: datetime,
    LastFailureMessage: str,
    LogDestinationType: LogDestinationTypeType,  # (1)
    LogExports: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LogDestinationTypeType](./literals.md#logdestinationtypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyAuthenticationProfileResultTypeDef

```python
# ModifyAuthenticationProfileResultTypeDef definition

class ModifyAuthenticationProfileResultTypeDef(TypedDict):
    AuthenticationProfileName: str,
    AuthenticationProfileContent: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyCustomDomainAssociationResultTypeDef

```python
# ModifyCustomDomainAssociationResultTypeDef definition

class ModifyCustomDomainAssociationResultTypeDef(TypedDict):
    CustomDomainName: str,
    CustomDomainCertificateArn: str,
    ClusterIdentifier: str,
    CustomDomainCertExpiryTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PartnerIntegrationOutputMessageTypeDef

```python
# PartnerIntegrationOutputMessageTypeDef definition

class PartnerIntegrationOutputMessageTypeDef(TypedDict):
    DatabaseName: str,
    PartnerName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterNamespaceOutputMessageTypeDef

```python
# RegisterNamespaceOutputMessageTypeDef definition

class RegisterNamespaceOutputMessageTypeDef(TypedDict):
    Status: NamespaceRegistrationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: NamespaceRegistrationStatusType](./literals.md#namespaceregistrationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResizeProgressMessageTypeDef

```python
# ResizeProgressMessageTypeDef definition

class ResizeProgressMessageTypeDef(TypedDict):
    TargetNodeType: str,
    TargetNumberOfNodes: int,
    TargetClusterType: str,
    Status: str,
    ImportTablesCompleted: List[str],
    ImportTablesInProgress: List[str],
    ImportTablesNotStarted: List[str],
    AvgResizeRateInMegaBytesPerSecond: float,
    TotalResizeDataInMegaBytes: int,
    ProgressInMegaBytes: int,
    ElapsedTimeInSeconds: int,
    EstimatedTimeToCompletionInSeconds: int,
    ResizeType: str,
    Message: str,
    TargetEncryptionType: str,
    DataTransferProgressPercent: float,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AccountAttributeTypeDef

```python
# AccountAttributeTypeDef definition

class AccountAttributeTypeDef(TypedDict):
    AttributeName: NotRequired[str],
    AttributeValues: NotRequired[List[AttributeValueTargetTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeValueTargetTypeDef](./type_defs.md#attributevaluetargettypedef) 
## ModifyAquaOutputMessageTypeDef

```python
# ModifyAquaOutputMessageTypeDef definition

class ModifyAquaOutputMessageTypeDef(TypedDict):
    AquaConfiguration: AquaConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AquaConfigurationTypeDef](./type_defs.md#aquaconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociationTypeDef

```python
# AssociationTypeDef definition

class AssociationTypeDef(TypedDict):
    CustomDomainCertificateArn: NotRequired[str],
    CustomDomainCertificateExpiryDate: NotRequired[datetime],
    CertificateAssociations: NotRequired[List[CertificateAssociationTypeDef]],  # (1)
```

1. See [:material-code-braces: CertificateAssociationTypeDef](./type_defs.md#certificateassociationtypedef) 
## DescribeAuthenticationProfilesResultTypeDef

```python
# DescribeAuthenticationProfilesResultTypeDef definition

class DescribeAuthenticationProfilesResultTypeDef(TypedDict):
    AuthenticationProfiles: List[AuthenticationProfileTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthenticationProfileTypeDef](./type_defs.md#authenticationprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AvailabilityZoneTypeDef

```python
# AvailabilityZoneTypeDef definition

class AvailabilityZoneTypeDef(TypedDict):
    Name: NotRequired[str],
    SupportedPlatforms: NotRequired[List[SupportedPlatformTypeDef]],  # (1)
```

1. See [:material-code-braces: SupportedPlatformTypeDef](./type_defs.md#supportedplatformtypedef) 
## BatchDeleteClusterSnapshotsRequestRequestTypeDef

```python
# BatchDeleteClusterSnapshotsRequestRequestTypeDef definition

class BatchDeleteClusterSnapshotsRequestRequestTypeDef(TypedDict):
    Identifiers: Sequence[DeleteClusterSnapshotMessageTypeDef],  # (1)
```

1. See [:material-code-braces: DeleteClusterSnapshotMessageTypeDef](./type_defs.md#deleteclustersnapshotmessagetypedef) 
## BatchDeleteClusterSnapshotsResultTypeDef

```python
# BatchDeleteClusterSnapshotsResultTypeDef definition

class BatchDeleteClusterSnapshotsResultTypeDef(TypedDict):
    Resources: List[str],
    Errors: List[SnapshotErrorMessageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotErrorMessageTypeDef](./type_defs.md#snapshoterrormessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchModifyClusterSnapshotsOutputMessageTypeDef

```python
# BatchModifyClusterSnapshotsOutputMessageTypeDef definition

class BatchModifyClusterSnapshotsOutputMessageTypeDef(TypedDict):
    Resources: List[str],
    Errors: List[SnapshotErrorMessageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotErrorMessageTypeDef](./type_defs.md#snapshoterrormessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterDbRevisionTypeDef

```python
# ClusterDbRevisionTypeDef definition

class ClusterDbRevisionTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    CurrentDatabaseRevision: NotRequired[str],
    DatabaseRevisionReleaseDate: NotRequired[datetime],
    RevisionTargets: NotRequired[List[RevisionTargetTypeDef]],  # (1)
```

1. See [:material-code-braces: RevisionTargetTypeDef](./type_defs.md#revisiontargettypedef) 
## SecondaryClusterInfoTypeDef

```python
# SecondaryClusterInfoTypeDef definition

class SecondaryClusterInfoTypeDef(TypedDict):
    AvailabilityZone: NotRequired[str],
    ClusterNodes: NotRequired[List[ClusterNodeTypeDef]],  # (1)
```

1. See [:material-code-braces: ClusterNodeTypeDef](./type_defs.md#clusternodetypedef) 
## ClusterParameterGroupDetailsTypeDef

```python
# ClusterParameterGroupDetailsTypeDef definition

class ClusterParameterGroupDetailsTypeDef(TypedDict):
    Parameters: List[ParameterTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DefaultClusterParametersTypeDef

```python
# DefaultClusterParametersTypeDef definition

class DefaultClusterParametersTypeDef(TypedDict):
    ParameterGroupFamily: NotRequired[str],
    Marker: NotRequired[str],
    Parameters: NotRequired[List[ParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## ModifyClusterParameterGroupMessageRequestTypeDef

```python
# ModifyClusterParameterGroupMessageRequestTypeDef definition

class ModifyClusterParameterGroupMessageRequestTypeDef(TypedDict):
    ParameterGroupName: str,
    Parameters: Sequence[ParameterTypeDef],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## ResetClusterParameterGroupMessageRequestTypeDef

```python
# ResetClusterParameterGroupMessageRequestTypeDef definition

class ResetClusterParameterGroupMessageRequestTypeDef(TypedDict):
    ParameterGroupName: str,
    ResetAllParameters: NotRequired[bool],
    Parameters: NotRequired[Sequence[ParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## ClusterParameterGroupStatusTypeDef

```python
# ClusterParameterGroupStatusTypeDef definition

class ClusterParameterGroupStatusTypeDef(TypedDict):
    ParameterGroupName: NotRequired[str],
    ParameterApplyStatus: NotRequired[str],
    ClusterParameterStatusList: NotRequired[List[ClusterParameterStatusTypeDef]],  # (1)
```

1. See [:material-code-braces: ClusterParameterStatusTypeDef](./type_defs.md#clusterparameterstatustypedef) 
## ClusterParameterGroupTypeDef

```python
# ClusterParameterGroupTypeDef definition

class ClusterParameterGroupTypeDef(TypedDict):
    ParameterGroupName: NotRequired[str],
    ParameterGroupFamily: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateClusterMessageRequestTypeDef

```python
# CreateClusterMessageRequestTypeDef definition

class CreateClusterMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    NodeType: str,
    MasterUsername: str,
    DBName: NotRequired[str],
    ClusterType: NotRequired[str],
    MasterUserPassword: NotRequired[str],
    ClusterSecurityGroups: NotRequired[Sequence[str]],
    VpcSecurityGroupIds: NotRequired[Sequence[str]],
    ClusterSubnetGroupName: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    ClusterParameterGroupName: NotRequired[str],
    AutomatedSnapshotRetentionPeriod: NotRequired[int],
    ManualSnapshotRetentionPeriod: NotRequired[int],
    Port: NotRequired[int],
    ClusterVersion: NotRequired[str],
    AllowVersionUpgrade: NotRequired[bool],
    NumberOfNodes: NotRequired[int],
    PubliclyAccessible: NotRequired[bool],
    Encrypted: NotRequired[bool],
    HsmClientCertificateIdentifier: NotRequired[str],
    HsmConfigurationIdentifier: NotRequired[str],
    ElasticIp: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    KmsKeyId: NotRequired[str],
    EnhancedVpcRouting: NotRequired[bool],
    AdditionalInfo: NotRequired[str],
    IamRoles: NotRequired[Sequence[str]],
    MaintenanceTrackName: NotRequired[str],
    SnapshotScheduleIdentifier: NotRequired[str],
    AvailabilityZoneRelocation: NotRequired[bool],
    AquaConfigurationStatus: NotRequired[AquaConfigurationStatusType],  # (2)
    DefaultIamRoleArn: NotRequired[str],
    LoadSampleData: NotRequired[str],
    ManageMasterPassword: NotRequired[bool],
    MasterPasswordSecretKmsKeyId: NotRequired[str],
    IpAddressType: NotRequired[str],
    MultiAZ: NotRequired[bool],
    RedshiftIdcApplicationArn: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: AquaConfigurationStatusType](./literals.md#aquaconfigurationstatustype) 
## CreateClusterParameterGroupMessageRequestTypeDef

```python
# CreateClusterParameterGroupMessageRequestTypeDef definition

class CreateClusterParameterGroupMessageRequestTypeDef(TypedDict):
    ParameterGroupName: str,
    ParameterGroupFamily: str,
    Description: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateClusterSecurityGroupMessageRequestTypeDef

```python
# CreateClusterSecurityGroupMessageRequestTypeDef definition

class CreateClusterSecurityGroupMessageRequestTypeDef(TypedDict):
    ClusterSecurityGroupName: str,
    Description: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateClusterSnapshotMessageRequestTypeDef

```python
# CreateClusterSnapshotMessageRequestTypeDef definition

class CreateClusterSnapshotMessageRequestTypeDef(TypedDict):
    SnapshotIdentifier: str,
    ClusterIdentifier: str,
    ManualSnapshotRetentionPeriod: NotRequired[int],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateClusterSubnetGroupMessageRequestTypeDef

```python
# CreateClusterSubnetGroupMessageRequestTypeDef definition

class CreateClusterSubnetGroupMessageRequestTypeDef(TypedDict):
    ClusterSubnetGroupName: str,
    Description: str,
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
    SourceIds: NotRequired[Sequence[str]],
    EventCategories: NotRequired[Sequence[str]],
    Severity: NotRequired[str],
    Enabled: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateHsmClientCertificateMessageRequestTypeDef

```python
# CreateHsmClientCertificateMessageRequestTypeDef definition

class CreateHsmClientCertificateMessageRequestTypeDef(TypedDict):
    HsmClientCertificateIdentifier: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateHsmConfigurationMessageRequestTypeDef

```python
# CreateHsmConfigurationMessageRequestTypeDef definition

class CreateHsmConfigurationMessageRequestTypeDef(TypedDict):
    HsmConfigurationIdentifier: str,
    Description: str,
    HsmIpAddress: str,
    HsmPartitionName: str,
    HsmPartitionPassword: str,
    HsmServerPublicCertificate: str,
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
    TagList: NotRequired[Sequence[TagTypeDef]],  # (1)
    AdditionalEncryptionContext: NotRequired[Mapping[str, str]],
    Description: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSnapshotCopyGrantMessageRequestTypeDef

```python
# CreateSnapshotCopyGrantMessageRequestTypeDef definition

class CreateSnapshotCopyGrantMessageRequestTypeDef(TypedDict):
    SnapshotCopyGrantName: str,
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSnapshotScheduleMessageRequestTypeDef

```python
# CreateSnapshotScheduleMessageRequestTypeDef definition

class CreateSnapshotScheduleMessageRequestTypeDef(TypedDict):
    ScheduleDefinitions: NotRequired[Sequence[str]],
    ScheduleIdentifier: NotRequired[str],
    ScheduleDescription: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    DryRun: NotRequired[bool],
    NextInvocations: NotRequired[int],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTagsMessageRequestTypeDef

```python
# CreateTagsMessageRequestTypeDef definition

class CreateTagsMessageRequestTypeDef(TypedDict):
    ResourceName: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateUsageLimitMessageRequestTypeDef

```python
# CreateUsageLimitMessageRequestTypeDef definition

class CreateUsageLimitMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    FeatureType: UsageLimitFeatureTypeType,  # (1)
    LimitType: UsageLimitLimitTypeType,  # (2)
    Amount: int,
    Period: NotRequired[UsageLimitPeriodType],  # (3)
    BreachAction: NotRequired[UsageLimitBreachActionType],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-brackets: UsageLimitFeatureTypeType](./literals.md#usagelimitfeaturetypetype) 
2. See [:material-code-brackets: UsageLimitLimitTypeType](./literals.md#usagelimitlimittypetype) 
3. See [:material-code-brackets: UsageLimitPeriodType](./literals.md#usagelimitperiodtype) 
4. See [:material-code-brackets: UsageLimitBreachActionType](./literals.md#usagelimitbreachactiontype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## EC2SecurityGroupTypeDef

```python
# EC2SecurityGroupTypeDef definition

class EC2SecurityGroupTypeDef(TypedDict):
    Status: NotRequired[str],
    EC2SecurityGroupName: NotRequired[str],
    EC2SecurityGroupOwnerId: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## EventSubscriptionTypeDef

```python
# EventSubscriptionTypeDef definition

class EventSubscriptionTypeDef(TypedDict):
    CustomerAwsId: NotRequired[str],
    CustSubscriptionId: NotRequired[str],
    SnsTopicArn: NotRequired[str],
    Status: NotRequired[str],
    SubscriptionCreationTime: NotRequired[datetime],
    SourceType: NotRequired[str],
    SourceIdsList: NotRequired[List[str]],
    EventCategoriesList: NotRequired[List[str]],
    Severity: NotRequired[str],
    Enabled: NotRequired[bool],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## HsmClientCertificateTypeDef

```python
# HsmClientCertificateTypeDef definition

class HsmClientCertificateTypeDef(TypedDict):
    HsmClientCertificateIdentifier: NotRequired[str],
    HsmClientCertificatePublicKey: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## HsmConfigurationTypeDef

```python
# HsmConfigurationTypeDef definition

class HsmConfigurationTypeDef(TypedDict):
    HsmConfigurationIdentifier: NotRequired[str],
    Description: NotRequired[str],
    HsmIpAddress: NotRequired[str],
    HsmPartitionName: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## IPRangeTypeDef

```python
# IPRangeTypeDef definition

class IPRangeTypeDef(TypedDict):
    Status: NotRequired[str],
    CIDRIP: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## SnapshotCopyGrantTypeDef

```python
# SnapshotCopyGrantTypeDef definition

class SnapshotCopyGrantTypeDef(TypedDict):
    SnapshotCopyGrantName: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## SnapshotScheduleResponseTypeDef

```python
# SnapshotScheduleResponseTypeDef definition

class SnapshotScheduleResponseTypeDef(TypedDict):
    ScheduleDefinitions: List[str],
    ScheduleIdentifier: str,
    ScheduleDescription: str,
    Tags: List[TagTypeDef],  # (1)
    NextInvocations: List[datetime],
    AssociatedClusterCount: int,
    AssociatedClusters: List[ClusterAssociatedToScheduleTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ClusterAssociatedToScheduleTypeDef](./type_defs.md#clusterassociatedtoscheduletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SnapshotScheduleTypeDef

```python
# SnapshotScheduleTypeDef definition

class SnapshotScheduleTypeDef(TypedDict):
    ScheduleDefinitions: NotRequired[List[str]],
    ScheduleIdentifier: NotRequired[str],
    ScheduleDescription: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    NextInvocations: NotRequired[List[datetime]],
    AssociatedClusterCount: NotRequired[int],
    AssociatedClusters: NotRequired[List[ClusterAssociatedToScheduleTypeDef]],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ClusterAssociatedToScheduleTypeDef](./type_defs.md#clusterassociatedtoscheduletypedef) 
## SnapshotTypeDef

```python
# SnapshotTypeDef definition

class SnapshotTypeDef(TypedDict):
    SnapshotIdentifier: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
    SnapshotCreateTime: NotRequired[datetime],
    Status: NotRequired[str],
    Port: NotRequired[int],
    AvailabilityZone: NotRequired[str],
    ClusterCreateTime: NotRequired[datetime],
    MasterUsername: NotRequired[str],
    ClusterVersion: NotRequired[str],
    EngineFullVersion: NotRequired[str],
    SnapshotType: NotRequired[str],
    NodeType: NotRequired[str],
    NumberOfNodes: NotRequired[int],
    DBName: NotRequired[str],
    VpcId: NotRequired[str],
    Encrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    EncryptedWithHSM: NotRequired[bool],
    AccountsWithRestoreAccess: NotRequired[List[AccountWithRestoreAccessTypeDef]],  # (1)
    OwnerAccount: NotRequired[str],
    TotalBackupSizeInMegaBytes: NotRequired[float],
    ActualIncrementalBackupSizeInMegaBytes: NotRequired[float],
    BackupProgressInMegaBytes: NotRequired[float],
    CurrentBackupRateInMegaBytesPerSecond: NotRequired[float],
    EstimatedSecondsToCompletion: NotRequired[int],
    ElapsedTimeInSeconds: NotRequired[int],
    SourceRegion: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    RestorableNodeTypes: NotRequired[List[str]],
    EnhancedVpcRouting: NotRequired[bool],
    MaintenanceTrackName: NotRequired[str],
    ManualSnapshotRetentionPeriod: NotRequired[int],
    ManualSnapshotRemainingDays: NotRequired[int],
    SnapshotRetentionStartTime: NotRequired[datetime],
    MasterPasswordSecretArn: NotRequired[str],
    MasterPasswordSecretKmsKeyId: NotRequired[str],
    SnapshotArn: NotRequired[str],
```

1. See [:material-code-braces: AccountWithRestoreAccessTypeDef](./type_defs.md#accountwithrestoreaccesstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TaggedResourceTypeDef

```python
# TaggedResourceTypeDef definition

class TaggedResourceTypeDef(TypedDict):
    Tag: NotRequired[TagTypeDef],  # (1)
    ResourceName: NotRequired[str],
    ResourceType: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UsageLimitResponseTypeDef

```python
# UsageLimitResponseTypeDef definition

class UsageLimitResponseTypeDef(TypedDict):
    UsageLimitId: str,
    ClusterIdentifier: str,
    FeatureType: UsageLimitFeatureTypeType,  # (1)
    LimitType: UsageLimitLimitTypeType,  # (2)
    Amount: int,
    Period: UsageLimitPeriodType,  # (3)
    BreachAction: UsageLimitBreachActionType,  # (4)
    Tags: List[TagTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: UsageLimitFeatureTypeType](./literals.md#usagelimitfeaturetypetype) 
2. See [:material-code-brackets: UsageLimitLimitTypeType](./literals.md#usagelimitlimittypetype) 
3. See [:material-code-brackets: UsageLimitPeriodType](./literals.md#usagelimitperiodtype) 
4. See [:material-code-brackets: UsageLimitBreachActionType](./literals.md#usagelimitbreachactiontype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UsageLimitTypeDef

```python
# UsageLimitTypeDef definition

class UsageLimitTypeDef(TypedDict):
    UsageLimitId: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
    FeatureType: NotRequired[UsageLimitFeatureTypeType],  # (1)
    LimitType: NotRequired[UsageLimitLimitTypeType],  # (2)
    Amount: NotRequired[int],
    Period: NotRequired[UsageLimitPeriodType],  # (3)
    BreachAction: NotRequired[UsageLimitBreachActionType],  # (4)
    Tags: NotRequired[List[TagTypeDef]],  # (5)
```

1. See [:material-code-brackets: UsageLimitFeatureTypeType](./literals.md#usagelimitfeaturetypetype) 
2. See [:material-code-brackets: UsageLimitLimitTypeType](./literals.md#usagelimitlimittypetype) 
3. See [:material-code-brackets: UsageLimitPeriodType](./literals.md#usagelimitperiodtype) 
4. See [:material-code-brackets: UsageLimitBreachActionType](./literals.md#usagelimitbreachactiontype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeReservedNodeExchangeStatusOutputMessageTypeDef

```python
# DescribeReservedNodeExchangeStatusOutputMessageTypeDef definition

class DescribeReservedNodeExchangeStatusOutputMessageTypeDef(TypedDict):
    ReservedNodeExchangeStatusDetails: List[ReservedNodeExchangeStatusTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedNodeExchangeStatusTypeDef](./type_defs.md#reservednodeexchangestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterVersionsMessageTypeDef

```python
# ClusterVersionsMessageTypeDef definition

class ClusterVersionsMessageTypeDef(TypedDict):
    Marker: str,
    ClusterVersions: List[ClusterVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterVersionTypeDef](./type_defs.md#clusterversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## ModifyClusterMaintenanceMessageRequestTypeDef

```python
# ModifyClusterMaintenanceMessageRequestTypeDef definition

class ModifyClusterMaintenanceMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: str,
    DeferMaintenance: NotRequired[bool],
    DeferMaintenanceIdentifier: NotRequired[str],
    DeferMaintenanceStartTime: NotRequired[TimestampTypeDef],
    DeferMaintenanceEndTime: NotRequired[TimestampTypeDef],
    DeferMaintenanceDuration: NotRequired[int],
```

## DataShareResponseTypeDef

```python
# DataShareResponseTypeDef definition

class DataShareResponseTypeDef(TypedDict):
    DataShareArn: str,
    ProducerArn: str,
    AllowPubliclyAccessibleConsumers: bool,
    DataShareAssociations: List[DataShareAssociationTypeDef],  # (1)
    ManagedBy: str,
    DataShareType: DataShareTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DataShareAssociationTypeDef](./type_defs.md#datashareassociationtypedef) 
2. See [:material-code-brackets: DataShareTypeType](./literals.md#datasharetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataShareTypeDef

```python
# DataShareTypeDef definition

class DataShareTypeDef(TypedDict):
    DataShareArn: NotRequired[str],
    ProducerArn: NotRequired[str],
    AllowPubliclyAccessibleConsumers: NotRequired[bool],
    DataShareAssociations: NotRequired[List[DataShareAssociationTypeDef]],  # (1)
    ManagedBy: NotRequired[str],
    DataShareType: NotRequired[DataShareTypeType],  # (2)
```

1. See [:material-code-braces: DataShareAssociationTypeDef](./type_defs.md#datashareassociationtypedef) 
2. See [:material-code-brackets: DataShareTypeType](./literals.md#datasharetypetype) 
## DescribeClusterDbRevisionsMessagePaginateTypeDef

```python
# DescribeClusterDbRevisionsMessagePaginateTypeDef definition

class DescribeClusterDbRevisionsMessagePaginateTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClusterParameterGroupsMessagePaginateTypeDef

```python
# DescribeClusterParameterGroupsMessagePaginateTypeDef definition

class DescribeClusterParameterGroupsMessagePaginateTypeDef(TypedDict):
    ParameterGroupName: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClusterParametersMessagePaginateTypeDef

```python
# DescribeClusterParametersMessagePaginateTypeDef definition

class DescribeClusterParametersMessagePaginateTypeDef(TypedDict):
    ParameterGroupName: str,
    Source: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClusterSecurityGroupsMessagePaginateTypeDef

```python
# DescribeClusterSecurityGroupsMessagePaginateTypeDef definition

class DescribeClusterSecurityGroupsMessagePaginateTypeDef(TypedDict):
    ClusterSecurityGroupName: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClusterSubnetGroupsMessagePaginateTypeDef

```python
# DescribeClusterSubnetGroupsMessagePaginateTypeDef definition

class DescribeClusterSubnetGroupsMessagePaginateTypeDef(TypedDict):
    ClusterSubnetGroupName: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClusterTracksMessagePaginateTypeDef

```python
# DescribeClusterTracksMessagePaginateTypeDef definition

class DescribeClusterTracksMessagePaginateTypeDef(TypedDict):
    MaintenanceTrackName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClusterVersionsMessagePaginateTypeDef

```python
# DescribeClusterVersionsMessagePaginateTypeDef definition

class DescribeClusterVersionsMessagePaginateTypeDef(TypedDict):
    ClusterVersion: NotRequired[str],
    ClusterParameterGroupFamily: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClustersMessagePaginateTypeDef

```python
# DescribeClustersMessagePaginateTypeDef definition

class DescribeClustersMessagePaginateTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeCustomDomainAssociationsMessagePaginateTypeDef

```python
# DescribeCustomDomainAssociationsMessagePaginateTypeDef definition

class DescribeCustomDomainAssociationsMessagePaginateTypeDef(TypedDict):
    CustomDomainName: NotRequired[str],
    CustomDomainCertificateArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDataSharesForConsumerMessagePaginateTypeDef

```python
# DescribeDataSharesForConsumerMessagePaginateTypeDef definition

class DescribeDataSharesForConsumerMessagePaginateTypeDef(TypedDict):
    ConsumerArn: NotRequired[str],
    Status: NotRequired[DataShareStatusForConsumerType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataShareStatusForConsumerType](./literals.md#datasharestatusforconsumertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDataSharesForProducerMessagePaginateTypeDef

```python
# DescribeDataSharesForProducerMessagePaginateTypeDef definition

class DescribeDataSharesForProducerMessagePaginateTypeDef(TypedDict):
    ProducerArn: NotRequired[str],
    Status: NotRequired[DataShareStatusForProducerType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataShareStatusForProducerType](./literals.md#datasharestatusforproducertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDataSharesMessagePaginateTypeDef

```python
# DescribeDataSharesMessagePaginateTypeDef definition

class DescribeDataSharesMessagePaginateTypeDef(TypedDict):
    DataShareArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDefaultClusterParametersMessagePaginateTypeDef

```python
# DescribeDefaultClusterParametersMessagePaginateTypeDef definition

class DescribeDefaultClusterParametersMessagePaginateTypeDef(TypedDict):
    ParameterGroupFamily: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEndpointAccessMessagePaginateTypeDef

```python
# DescribeEndpointAccessMessagePaginateTypeDef definition

class DescribeEndpointAccessMessagePaginateTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    ResourceOwner: NotRequired[str],
    EndpointName: NotRequired[str],
    VpcId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEndpointAuthorizationMessagePaginateTypeDef

```python
# DescribeEndpointAuthorizationMessagePaginateTypeDef definition

class DescribeEndpointAuthorizationMessagePaginateTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    Account: NotRequired[str],
    Grantee: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventSubscriptionsMessagePaginateTypeDef

```python
# DescribeEventSubscriptionsMessagePaginateTypeDef definition

class DescribeEventSubscriptionsMessagePaginateTypeDef(TypedDict):
    SubscriptionName: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
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
## DescribeHsmClientCertificatesMessagePaginateTypeDef

```python
# DescribeHsmClientCertificatesMessagePaginateTypeDef definition

class DescribeHsmClientCertificatesMessagePaginateTypeDef(TypedDict):
    HsmClientCertificateIdentifier: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeHsmConfigurationsMessagePaginateTypeDef

```python
# DescribeHsmConfigurationsMessagePaginateTypeDef definition

class DescribeHsmConfigurationsMessagePaginateTypeDef(TypedDict):
    HsmConfigurationIdentifier: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeInboundIntegrationsMessagePaginateTypeDef

```python
# DescribeInboundIntegrationsMessagePaginateTypeDef definition

class DescribeInboundIntegrationsMessagePaginateTypeDef(TypedDict):
    IntegrationArn: NotRequired[str],
    TargetArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOrderableClusterOptionsMessagePaginateTypeDef

```python
# DescribeOrderableClusterOptionsMessagePaginateTypeDef definition

class DescribeOrderableClusterOptionsMessagePaginateTypeDef(TypedDict):
    ClusterVersion: NotRequired[str],
    NodeType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRedshiftIdcApplicationsMessagePaginateTypeDef

```python
# DescribeRedshiftIdcApplicationsMessagePaginateTypeDef definition

class DescribeRedshiftIdcApplicationsMessagePaginateTypeDef(TypedDict):
    RedshiftIdcApplicationArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReservedNodeExchangeStatusInputMessagePaginateTypeDef

```python
# DescribeReservedNodeExchangeStatusInputMessagePaginateTypeDef definition

class DescribeReservedNodeExchangeStatusInputMessagePaginateTypeDef(TypedDict):
    ReservedNodeId: NotRequired[str],
    ReservedNodeExchangeRequestId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReservedNodeOfferingsMessagePaginateTypeDef

```python
# DescribeReservedNodeOfferingsMessagePaginateTypeDef definition

class DescribeReservedNodeOfferingsMessagePaginateTypeDef(TypedDict):
    ReservedNodeOfferingId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReservedNodesMessagePaginateTypeDef

```python
# DescribeReservedNodesMessagePaginateTypeDef definition

class DescribeReservedNodesMessagePaginateTypeDef(TypedDict):
    ReservedNodeId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSnapshotCopyGrantsMessagePaginateTypeDef

```python
# DescribeSnapshotCopyGrantsMessagePaginateTypeDef definition

class DescribeSnapshotCopyGrantsMessagePaginateTypeDef(TypedDict):
    SnapshotCopyGrantName: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSnapshotSchedulesMessagePaginateTypeDef

```python
# DescribeSnapshotSchedulesMessagePaginateTypeDef definition

class DescribeSnapshotSchedulesMessagePaginateTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    ScheduleIdentifier: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeTableRestoreStatusMessagePaginateTypeDef

```python
# DescribeTableRestoreStatusMessagePaginateTypeDef definition

class DescribeTableRestoreStatusMessagePaginateTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    TableRestoreRequestId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeTagsMessagePaginateTypeDef

```python
# DescribeTagsMessagePaginateTypeDef definition

class DescribeTagsMessagePaginateTypeDef(TypedDict):
    ResourceName: NotRequired[str],
    ResourceType: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeUsageLimitsMessagePaginateTypeDef

```python
# DescribeUsageLimitsMessagePaginateTypeDef definition

class DescribeUsageLimitsMessagePaginateTypeDef(TypedDict):
    UsageLimitId: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
    FeatureType: NotRequired[UsageLimitFeatureTypeType],  # (1)
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: UsageLimitFeatureTypeType](./literals.md#usagelimitfeaturetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetReservedNodeExchangeConfigurationOptionsInputMessagePaginateTypeDef

```python
# GetReservedNodeExchangeConfigurationOptionsInputMessagePaginateTypeDef definition

class GetReservedNodeExchangeConfigurationOptionsInputMessagePaginateTypeDef(TypedDict):
    ActionType: ReservedNodeExchangeActionTypeType,  # (1)
    ClusterIdentifier: NotRequired[str],
    SnapshotIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ReservedNodeExchangeActionTypeType](./literals.md#reservednodeexchangeactiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetReservedNodeExchangeOfferingsInputMessagePaginateTypeDef

```python
# GetReservedNodeExchangeOfferingsInputMessagePaginateTypeDef definition

class GetReservedNodeExchangeOfferingsInputMessagePaginateTypeDef(TypedDict):
    ReservedNodeId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecommendationsMessagePaginateTypeDef

```python
# ListRecommendationsMessagePaginateTypeDef definition

class ListRecommendationsMessagePaginateTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    NamespaceArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClusterSnapshotsMessagePaginateTypeDef

```python
# DescribeClusterSnapshotsMessagePaginateTypeDef definition

class DescribeClusterSnapshotsMessagePaginateTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    SnapshotIdentifier: NotRequired[str],
    SnapshotArn: NotRequired[str],
    SnapshotType: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    OwnerAccount: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    ClusterExists: NotRequired[bool],
    SortingEntities: NotRequired[Sequence[SnapshotSortingEntityTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SnapshotSortingEntityTypeDef](./type_defs.md#snapshotsortingentitytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClusterSnapshotsMessageRequestTypeDef

```python
# DescribeClusterSnapshotsMessageRequestTypeDef definition

class DescribeClusterSnapshotsMessageRequestTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    SnapshotIdentifier: NotRequired[str],
    SnapshotArn: NotRequired[str],
    SnapshotType: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    OwnerAccount: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    ClusterExists: NotRequired[bool],
    SortingEntities: NotRequired[Sequence[SnapshotSortingEntityTypeDef]],  # (1)
```

1. See [:material-code-braces: SnapshotSortingEntityTypeDef](./type_defs.md#snapshotsortingentitytypedef) 
## DescribeClusterSnapshotsMessageWaitTypeDef

```python
# DescribeClusterSnapshotsMessageWaitTypeDef definition

class DescribeClusterSnapshotsMessageWaitTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    SnapshotIdentifier: NotRequired[str],
    SnapshotArn: NotRequired[str],
    SnapshotType: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    OwnerAccount: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    ClusterExists: NotRequired[bool],
    SortingEntities: NotRequired[Sequence[SnapshotSortingEntityTypeDef]],  # (1)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SnapshotSortingEntityTypeDef](./type_defs.md#snapshotsortingentitytypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeClustersMessageWaitTypeDef

```python
# DescribeClustersMessageWaitTypeDef definition

class DescribeClustersMessageWaitTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    TagKeys: NotRequired[Sequence[str]],
    TagValues: NotRequired[Sequence[str]],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeIntegrationsMessagePaginateTypeDef

```python
# DescribeIntegrationsMessagePaginateTypeDef definition

class DescribeIntegrationsMessagePaginateTypeDef(TypedDict):
    IntegrationArn: NotRequired[str],
    Filters: NotRequired[Sequence[DescribeIntegrationsFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeIntegrationsFilterTypeDef](./type_defs.md#describeintegrationsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeIntegrationsMessageRequestTypeDef

```python
# DescribeIntegrationsMessageRequestTypeDef definition

class DescribeIntegrationsMessageRequestTypeDef(TypedDict):
    IntegrationArn: NotRequired[str],
    MaxRecords: NotRequired[int],
    Marker: NotRequired[str],
    Filters: NotRequired[Sequence[DescribeIntegrationsFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: DescribeIntegrationsFilterTypeDef](./type_defs.md#describeintegrationsfiltertypedef) 
## DescribeNodeConfigurationOptionsMessagePaginateTypeDef

```python
# DescribeNodeConfigurationOptionsMessagePaginateTypeDef definition

class DescribeNodeConfigurationOptionsMessagePaginateTypeDef(TypedDict):
    ActionType: ActionTypeType,  # (1)
    ClusterIdentifier: NotRequired[str],
    SnapshotIdentifier: NotRequired[str],
    SnapshotArn: NotRequired[str],
    OwnerAccount: NotRequired[str],
    Filters: NotRequired[Sequence[NodeConfigurationOptionsFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-braces: NodeConfigurationOptionsFilterTypeDef](./type_defs.md#nodeconfigurationoptionsfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeNodeConfigurationOptionsMessageRequestTypeDef

```python
# DescribeNodeConfigurationOptionsMessageRequestTypeDef definition

class DescribeNodeConfigurationOptionsMessageRequestTypeDef(TypedDict):
    ActionType: ActionTypeType,  # (1)
    ClusterIdentifier: NotRequired[str],
    SnapshotIdentifier: NotRequired[str],
    SnapshotArn: NotRequired[str],
    OwnerAccount: NotRequired[str],
    Filters: NotRequired[Sequence[NodeConfigurationOptionsFilterTypeDef]],  # (2)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-braces: NodeConfigurationOptionsFilterTypeDef](./type_defs.md#nodeconfigurationoptionsfiltertypedef) 
## DescribePartnersOutputMessageTypeDef

```python
# DescribePartnersOutputMessageTypeDef definition

class DescribePartnersOutputMessageTypeDef(TypedDict):
    PartnerIntegrationInfoList: List[PartnerIntegrationInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartnerIntegrationInfoTypeDef](./type_defs.md#partnerintegrationinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeScheduledActionsMessagePaginateTypeDef

```python
# DescribeScheduledActionsMessagePaginateTypeDef definition

class DescribeScheduledActionsMessagePaginateTypeDef(TypedDict):
    ScheduledActionName: NotRequired[str],
    TargetActionType: NotRequired[ScheduledActionTypeValuesType],  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Active: NotRequired[bool],
    Filters: NotRequired[Sequence[ScheduledActionFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ScheduledActionTypeValuesType](./literals.md#scheduledactiontypevaluestype) 
2. See [:material-code-braces: ScheduledActionFilterTypeDef](./type_defs.md#scheduledactionfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeScheduledActionsMessageRequestTypeDef

```python
# DescribeScheduledActionsMessageRequestTypeDef definition

class DescribeScheduledActionsMessageRequestTypeDef(TypedDict):
    ScheduledActionName: NotRequired[str],
    TargetActionType: NotRequired[ScheduledActionTypeValuesType],  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Active: NotRequired[bool],
    Filters: NotRequired[Sequence[ScheduledActionFilterTypeDef]],  # (2)
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
```

1. See [:material-code-brackets: ScheduledActionTypeValuesType](./literals.md#scheduledactiontypevaluestype) 
2. See [:material-code-braces: ScheduledActionFilterTypeDef](./type_defs.md#scheduledactionfiltertypedef) 
## EndpointAuthorizationListTypeDef

```python
# EndpointAuthorizationListTypeDef definition

class EndpointAuthorizationListTypeDef(TypedDict):
    EndpointAuthorizationList: List[EndpointAuthorizationTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointAuthorizationTypeDef](./type_defs.md#endpointauthorizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventCategoriesMapTypeDef

```python
# EventCategoriesMapTypeDef definition

class EventCategoriesMapTypeDef(TypedDict):
    SourceType: NotRequired[str],
    Events: NotRequired[List[EventInfoMapTypeDef]],  # (1)
```

1. See [:material-code-braces: EventInfoMapTypeDef](./type_defs.md#eventinfomaptypedef) 
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
## GetResourcePolicyResultTypeDef

```python
# GetResourcePolicyResultTypeDef definition

class GetResourcePolicyResultTypeDef(TypedDict):
    ResourcePolicy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResultTypeDef

```python
# PutResourcePolicyResultTypeDef definition

class PutResourcePolicyResultTypeDef(TypedDict):
    ResourcePolicy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InboundIntegrationTypeDef

```python
# InboundIntegrationTypeDef definition

class InboundIntegrationTypeDef(TypedDict):
    IntegrationArn: NotRequired[str],
    SourceArn: NotRequired[str],
    TargetArn: NotRequired[str],
    Status: NotRequired[ZeroETLIntegrationStatusType],  # (1)
    Errors: NotRequired[List[IntegrationErrorTypeDef]],  # (2)
    CreateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ZeroETLIntegrationStatusType](./literals.md#zeroetlintegrationstatustype) 
2. See [:material-code-braces: IntegrationErrorTypeDef](./type_defs.md#integrationerrortypedef) 
## IntegrationResponseTypeDef

```python
# IntegrationResponseTypeDef definition

class IntegrationResponseTypeDef(TypedDict):
    IntegrationArn: str,
    IntegrationName: str,
    SourceArn: str,
    TargetArn: str,
    Status: ZeroETLIntegrationStatusType,  # (1)
    Errors: List[IntegrationErrorTypeDef],  # (2)
    CreateTime: datetime,
    Description: str,
    KMSKeyId: str,
    AdditionalEncryptionContext: Dict[str, str],
    Tags: List[TagTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ZeroETLIntegrationStatusType](./literals.md#zeroetlintegrationstatustype) 
2. See [:material-code-braces: IntegrationErrorTypeDef](./type_defs.md#integrationerrortypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntegrationTypeDef

```python
# IntegrationTypeDef definition

class IntegrationTypeDef(TypedDict):
    IntegrationArn: NotRequired[str],
    IntegrationName: NotRequired[str],
    SourceArn: NotRequired[str],
    TargetArn: NotRequired[str],
    Status: NotRequired[ZeroETLIntegrationStatusType],  # (1)
    Errors: NotRequired[List[IntegrationErrorTypeDef]],  # (2)
    CreateTime: NotRequired[datetime],
    Description: NotRequired[str],
    KMSKeyId: NotRequired[str],
    AdditionalEncryptionContext: NotRequired[Dict[str, str]],
    Tags: NotRequired[List[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: ZeroETLIntegrationStatusType](./literals.md#zeroetlintegrationstatustype) 
2. See [:material-code-braces: IntegrationErrorTypeDef](./type_defs.md#integrationerrortypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## LakeFormationScopeUnionTypeDef

```python
# LakeFormationScopeUnionTypeDef definition

class LakeFormationScopeUnionTypeDef(TypedDict):
    LakeFormationQuery: NotRequired[LakeFormationQueryTypeDef],  # (1)
```

1. See [:material-code-braces: LakeFormationQueryTypeDef](./type_defs.md#lakeformationquerytypedef) 
## NamespaceIdentifierUnionTypeDef

```python
# NamespaceIdentifierUnionTypeDef definition

class NamespaceIdentifierUnionTypeDef(TypedDict):
    ServerlessIdentifier: NotRequired[ServerlessIdentifierTypeDef],  # (1)
    ProvisionedIdentifier: NotRequired[ProvisionedIdentifierTypeDef],  # (2)
```

1. See [:material-code-braces: ServerlessIdentifierTypeDef](./type_defs.md#serverlessidentifiertypedef) 
2. See [:material-code-braces: ProvisionedIdentifierTypeDef](./type_defs.md#provisionedidentifiertypedef) 
## VpcEndpointTypeDef

```python
# VpcEndpointTypeDef definition

class VpcEndpointTypeDef(TypedDict):
    VpcEndpointId: NotRequired[str],
    VpcId: NotRequired[str],
    NetworkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (1)
```

1. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
## NodeConfigurationOptionsMessageTypeDef

```python
# NodeConfigurationOptionsMessageTypeDef definition

class NodeConfigurationOptionsMessageTypeDef(TypedDict):
    NodeConfigurationOptionList: List[NodeConfigurationOptionTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NodeConfigurationOptionTypeDef](./type_defs.md#nodeconfigurationoptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3AccessGrantsScopeUnionTypeDef

```python
# S3AccessGrantsScopeUnionTypeDef definition

class S3AccessGrantsScopeUnionTypeDef(TypedDict):
    ReadWriteAccess: NotRequired[ReadWriteAccessTypeDef],  # (1)
```

1. See [:material-code-braces: ReadWriteAccessTypeDef](./type_defs.md#readwriteaccesstypedef) 
## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    Id: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
    NamespaceArn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    RecommendationType: NotRequired[str],
    Title: NotRequired[str],
    Description: NotRequired[str],
    Observation: NotRequired[str],
    ImpactRanking: NotRequired[ImpactRankingTypeType],  # (1)
    RecommendationText: NotRequired[str],
    RecommendedActions: NotRequired[List[RecommendedActionTypeDef]],  # (2)
    ReferenceLinks: NotRequired[List[ReferenceLinkTypeDef]],  # (3)
```

1. See [:material-code-brackets: ImpactRankingTypeType](./literals.md#impactrankingtypetype) 
2. See [:material-code-braces: RecommendedActionTypeDef](./type_defs.md#recommendedactiontypedef) 
3. See [:material-code-braces: ReferenceLinkTypeDef](./type_defs.md#referencelinktypedef) 
## ReservedNodeOfferingTypeDef

```python
# ReservedNodeOfferingTypeDef definition

class ReservedNodeOfferingTypeDef(TypedDict):
    ReservedNodeOfferingId: NotRequired[str],
    NodeType: NotRequired[str],
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    UsagePrice: NotRequired[float],
    CurrencyCode: NotRequired[str],
    OfferingType: NotRequired[str],
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (1)
    ReservedNodeOfferingType: NotRequired[ReservedNodeOfferingTypeType],  # (2)
```

1. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
2. See [:material-code-brackets: ReservedNodeOfferingTypeType](./literals.md#reservednodeofferingtypetype) 
## ReservedNodeTypeDef

```python
# ReservedNodeTypeDef definition

class ReservedNodeTypeDef(TypedDict):
    ReservedNodeId: NotRequired[str],
    ReservedNodeOfferingId: NotRequired[str],
    NodeType: NotRequired[str],
    StartTime: NotRequired[datetime],
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    UsagePrice: NotRequired[float],
    CurrencyCode: NotRequired[str],
    NodeCount: NotRequired[int],
    State: NotRequired[str],
    OfferingType: NotRequired[str],
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (1)
    ReservedNodeOfferingType: NotRequired[ReservedNodeOfferingTypeType],  # (2)
```

1. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
2. See [:material-code-brackets: ReservedNodeOfferingTypeType](./literals.md#reservednodeofferingtypetype) 
## RestoreTableFromClusterSnapshotResultTypeDef

```python
# RestoreTableFromClusterSnapshotResultTypeDef definition

class RestoreTableFromClusterSnapshotResultTypeDef(TypedDict):
    TableRestoreStatus: TableRestoreStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableRestoreStatusTypeDef](./type_defs.md#tablerestorestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableRestoreStatusMessageTypeDef

```python
# TableRestoreStatusMessageTypeDef definition

class TableRestoreStatusMessageTypeDef(TypedDict):
    TableRestoreStatusDetails: List[TableRestoreStatusTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableRestoreStatusTypeDef](./type_defs.md#tablerestorestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScheduledActionTypeTypeDef

```python
# ScheduledActionTypeTypeDef definition

class ScheduledActionTypeTypeDef(TypedDict):
    ResizeCluster: NotRequired[ResizeClusterMessageTypeDef],  # (1)
    PauseCluster: NotRequired[PauseClusterMessageTypeDef],  # (2)
    ResumeCluster: NotRequired[ResumeClusterMessageTypeDef],  # (3)
```

1. See [:material-code-braces: ResizeClusterMessageTypeDef](./type_defs.md#resizeclustermessagetypedef) 
2. See [:material-code-braces: PauseClusterMessageTypeDef](./type_defs.md#pauseclustermessagetypedef) 
3. See [:material-code-braces: ResumeClusterMessageTypeDef](./type_defs.md#resumeclustermessagetypedef) 
## UpdateTargetTypeDef

```python
# UpdateTargetTypeDef definition

class UpdateTargetTypeDef(TypedDict):
    MaintenanceTrackName: NotRequired[str],
    DatabaseVersion: NotRequired[str],
    SupportedOperations: NotRequired[List[SupportedOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: SupportedOperationTypeDef](./type_defs.md#supportedoperationtypedef) 
## AccountAttributeListTypeDef

```python
# AccountAttributeListTypeDef definition

class AccountAttributeListTypeDef(TypedDict):
    AccountAttributes: List[AccountAttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAttributeTypeDef](./type_defs.md#accountattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomDomainAssociationsMessageTypeDef

```python
# CustomDomainAssociationsMessageTypeDef definition

class CustomDomainAssociationsMessageTypeDef(TypedDict):
    Marker: str,
    Associations: List[AssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociationTypeDef](./type_defs.md#associationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OrderableClusterOptionTypeDef

```python
# OrderableClusterOptionTypeDef definition

class OrderableClusterOptionTypeDef(TypedDict):
    ClusterVersion: NotRequired[str],
    ClusterType: NotRequired[str],
    NodeType: NotRequired[str],
    AvailabilityZones: NotRequired[List[AvailabilityZoneTypeDef]],  # (1)
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
## ClusterDbRevisionsMessageTypeDef

```python
# ClusterDbRevisionsMessageTypeDef definition

class ClusterDbRevisionsMessageTypeDef(TypedDict):
    Marker: str,
    ClusterDbRevisions: List[ClusterDbRevisionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterDbRevisionTypeDef](./type_defs.md#clusterdbrevisiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDefaultClusterParametersResultTypeDef

```python
# DescribeDefaultClusterParametersResultTypeDef definition

class DescribeDefaultClusterParametersResultTypeDef(TypedDict):
    DefaultClusterParameters: DefaultClusterParametersTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DefaultClusterParametersTypeDef](./type_defs.md#defaultclusterparameterstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterParameterGroupsMessageTypeDef

```python
# ClusterParameterGroupsMessageTypeDef definition

class ClusterParameterGroupsMessageTypeDef(TypedDict):
    Marker: str,
    ParameterGroups: List[ClusterParameterGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterParameterGroupTypeDef](./type_defs.md#clusterparametergrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterParameterGroupResultTypeDef

```python
# CreateClusterParameterGroupResultTypeDef definition

class CreateClusterParameterGroupResultTypeDef(TypedDict):
    ClusterParameterGroup: ClusterParameterGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterParameterGroupTypeDef](./type_defs.md#clusterparametergrouptypedef) 
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
## CreateHsmClientCertificateResultTypeDef

```python
# CreateHsmClientCertificateResultTypeDef definition

class CreateHsmClientCertificateResultTypeDef(TypedDict):
    HsmClientCertificate: HsmClientCertificateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HsmClientCertificateTypeDef](./type_defs.md#hsmclientcertificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HsmClientCertificateMessageTypeDef

```python
# HsmClientCertificateMessageTypeDef definition

class HsmClientCertificateMessageTypeDef(TypedDict):
    Marker: str,
    HsmClientCertificates: List[HsmClientCertificateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HsmClientCertificateTypeDef](./type_defs.md#hsmclientcertificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHsmConfigurationResultTypeDef

```python
# CreateHsmConfigurationResultTypeDef definition

class CreateHsmConfigurationResultTypeDef(TypedDict):
    HsmConfiguration: HsmConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HsmConfigurationTypeDef](./type_defs.md#hsmconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HsmConfigurationMessageTypeDef

```python
# HsmConfigurationMessageTypeDef definition

class HsmConfigurationMessageTypeDef(TypedDict):
    Marker: str,
    HsmConfigurations: List[HsmConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HsmConfigurationTypeDef](./type_defs.md#hsmconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterSecurityGroupTypeDef

```python
# ClusterSecurityGroupTypeDef definition

class ClusterSecurityGroupTypeDef(TypedDict):
    ClusterSecurityGroupName: NotRequired[str],
    Description: NotRequired[str],
    EC2SecurityGroups: NotRequired[List[EC2SecurityGroupTypeDef]],  # (1)
    IPRanges: NotRequired[List[IPRangeTypeDef]],  # (2)
    Tags: NotRequired[List[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: EC2SecurityGroupTypeDef](./type_defs.md#ec2securitygrouptypedef) 
2. See [:material-code-braces: IPRangeTypeDef](./type_defs.md#iprangetypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSnapshotCopyGrantResultTypeDef

```python
# CreateSnapshotCopyGrantResultTypeDef definition

class CreateSnapshotCopyGrantResultTypeDef(TypedDict):
    SnapshotCopyGrant: SnapshotCopyGrantTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotCopyGrantTypeDef](./type_defs.md#snapshotcopygranttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SnapshotCopyGrantMessageTypeDef

```python
# SnapshotCopyGrantMessageTypeDef definition

class SnapshotCopyGrantMessageTypeDef(TypedDict):
    Marker: str,
    SnapshotCopyGrants: List[SnapshotCopyGrantTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotCopyGrantTypeDef](./type_defs.md#snapshotcopygranttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSnapshotSchedulesOutputMessageTypeDef

```python
# DescribeSnapshotSchedulesOutputMessageTypeDef definition

class DescribeSnapshotSchedulesOutputMessageTypeDef(TypedDict):
    SnapshotSchedules: List[SnapshotScheduleTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotScheduleTypeDef](./type_defs.md#snapshotscheduletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AuthorizeSnapshotAccessResultTypeDef

```python
# AuthorizeSnapshotAccessResultTypeDef definition

class AuthorizeSnapshotAccessResultTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyClusterSnapshotResultTypeDef

```python
# CopyClusterSnapshotResultTypeDef definition

class CopyClusterSnapshotResultTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterSnapshotResultTypeDef

```python
# CreateClusterSnapshotResultTypeDef definition

class CreateClusterSnapshotResultTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterSnapshotResultTypeDef

```python
# DeleteClusterSnapshotResultTypeDef definition

class DeleteClusterSnapshotResultTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyClusterSnapshotResultTypeDef

```python
# ModifyClusterSnapshotResultTypeDef definition

class ModifyClusterSnapshotResultTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RevokeSnapshotAccessResultTypeDef

```python
# RevokeSnapshotAccessResultTypeDef definition

class RevokeSnapshotAccessResultTypeDef(TypedDict):
    Snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SnapshotMessageTypeDef

```python
# SnapshotMessageTypeDef definition

class SnapshotMessageTypeDef(TypedDict):
    Marker: str,
    Snapshots: List[SnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TaggedResourceListMessageTypeDef

```python
# TaggedResourceListMessageTypeDef definition

class TaggedResourceListMessageTypeDef(TypedDict):
    TaggedResources: List[TaggedResourceTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaggedResourceTypeDef](./type_defs.md#taggedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UsageLimitListTypeDef

```python
# UsageLimitListTypeDef definition

class UsageLimitListTypeDef(TypedDict):
    UsageLimits: List[UsageLimitTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UsageLimitTypeDef](./type_defs.md#usagelimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataSharesForConsumerResultTypeDef

```python
# DescribeDataSharesForConsumerResultTypeDef definition

class DescribeDataSharesForConsumerResultTypeDef(TypedDict):
    DataShares: List[DataShareTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataShareTypeDef](./type_defs.md#datasharetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataSharesForProducerResultTypeDef

```python
# DescribeDataSharesForProducerResultTypeDef definition

class DescribeDataSharesForProducerResultTypeDef(TypedDict):
    DataShares: List[DataShareTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataShareTypeDef](./type_defs.md#datasharetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataSharesResultTypeDef

```python
# DescribeDataSharesResultTypeDef definition

class DescribeDataSharesResultTypeDef(TypedDict):
    DataShares: List[DataShareTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataShareTypeDef](./type_defs.md#datasharetypedef) 
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
## InboundIntegrationsMessageTypeDef

```python
# InboundIntegrationsMessageTypeDef definition

class InboundIntegrationsMessageTypeDef(TypedDict):
    Marker: str,
    InboundIntegrations: List[InboundIntegrationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InboundIntegrationTypeDef](./type_defs.md#inboundintegrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntegrationsMessageTypeDef

```python
# IntegrationsMessageTypeDef definition

class IntegrationsMessageTypeDef(TypedDict):
    Marker: str,
    Integrations: List[IntegrationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IntegrationTypeDef](./type_defs.md#integrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterNamespaceInputMessageRequestTypeDef

```python
# DeregisterNamespaceInputMessageRequestTypeDef definition

class DeregisterNamespaceInputMessageRequestTypeDef(TypedDict):
    NamespaceIdentifier: NamespaceIdentifierUnionTypeDef,  # (1)
    ConsumerIdentifiers: Sequence[str],
```

1. See [:material-code-braces: NamespaceIdentifierUnionTypeDef](./type_defs.md#namespaceidentifieruniontypedef) 
## RegisterNamespaceInputMessageRequestTypeDef

```python
# RegisterNamespaceInputMessageRequestTypeDef definition

class RegisterNamespaceInputMessageRequestTypeDef(TypedDict):
    NamespaceIdentifier: NamespaceIdentifierUnionTypeDef,  # (1)
    ConsumerIdentifiers: Sequence[str],
```

1. See [:material-code-braces: NamespaceIdentifierUnionTypeDef](./type_defs.md#namespaceidentifieruniontypedef) 
## EndpointAccessResponseTypeDef

```python
# EndpointAccessResponseTypeDef definition

class EndpointAccessResponseTypeDef(TypedDict):
    ClusterIdentifier: str,
    ResourceOwner: str,
    SubnetGroupName: str,
    EndpointStatus: str,
    EndpointName: str,
    EndpointCreateTime: datetime,
    Port: int,
    Address: str,
    VpcSecurityGroups: List[VpcSecurityGroupMembershipTypeDef],  # (1)
    VpcEndpoint: VpcEndpointTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: VpcSecurityGroupMembershipTypeDef](./type_defs.md#vpcsecuritygroupmembershiptypedef) 
2. See [:material-code-braces: VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EndpointAccessTypeDef

```python
# EndpointAccessTypeDef definition

class EndpointAccessTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    ResourceOwner: NotRequired[str],
    SubnetGroupName: NotRequired[str],
    EndpointStatus: NotRequired[str],
    EndpointName: NotRequired[str],
    EndpointCreateTime: NotRequired[datetime],
    Port: NotRequired[int],
    Address: NotRequired[str],
    VpcSecurityGroups: NotRequired[List[VpcSecurityGroupMembershipTypeDef]],  # (1)
    VpcEndpoint: NotRequired[VpcEndpointTypeDef],  # (2)
```

1. See [:material-code-braces: VpcSecurityGroupMembershipTypeDef](./type_defs.md#vpcsecuritygroupmembershiptypedef) 
2. See [:material-code-braces: VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef) 
## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Address: NotRequired[str],
    Port: NotRequired[int],
    VpcEndpoints: NotRequired[List[VpcEndpointTypeDef]],  # (1)
```

1. See [:material-code-braces: VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef) 
## ServiceIntegrationsUnionOutputTypeDef

```python
# ServiceIntegrationsUnionOutputTypeDef definition

class ServiceIntegrationsUnionOutputTypeDef(TypedDict):
    LakeFormation: NotRequired[List[LakeFormationScopeUnionTypeDef]],  # (1)
    S3AccessGrants: NotRequired[List[S3AccessGrantsScopeUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: LakeFormationScopeUnionTypeDef](./type_defs.md#lakeformationscopeuniontypedef) 
2. See [:material-code-braces: S3AccessGrantsScopeUnionTypeDef](./type_defs.md#s3accessgrantsscopeuniontypedef) 
## ServiceIntegrationsUnionTypeDef

```python
# ServiceIntegrationsUnionTypeDef definition

class ServiceIntegrationsUnionTypeDef(TypedDict):
    LakeFormation: NotRequired[Sequence[LakeFormationScopeUnionTypeDef]],  # (1)
    S3AccessGrants: NotRequired[Sequence[S3AccessGrantsScopeUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: LakeFormationScopeUnionTypeDef](./type_defs.md#lakeformationscopeuniontypedef) 
2. See [:material-code-braces: S3AccessGrantsScopeUnionTypeDef](./type_defs.md#s3accessgrantsscopeuniontypedef) 
## ListRecommendationsResultTypeDef

```python
# ListRecommendationsResultTypeDef definition

class ListRecommendationsResultTypeDef(TypedDict):
    Recommendations: List[RecommendationTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReservedNodeExchangeOfferingsOutputMessageTypeDef

```python
# GetReservedNodeExchangeOfferingsOutputMessageTypeDef definition

class GetReservedNodeExchangeOfferingsOutputMessageTypeDef(TypedDict):
    Marker: str,
    ReservedNodeOfferings: List[ReservedNodeOfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedNodeOfferingTypeDef](./type_defs.md#reservednodeofferingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReservedNodeOfferingsMessageTypeDef

```python
# ReservedNodeOfferingsMessageTypeDef definition

class ReservedNodeOfferingsMessageTypeDef(TypedDict):
    Marker: str,
    ReservedNodeOfferings: List[ReservedNodeOfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedNodeOfferingTypeDef](./type_defs.md#reservednodeofferingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AcceptReservedNodeExchangeOutputMessageTypeDef

```python
# AcceptReservedNodeExchangeOutputMessageTypeDef definition

class AcceptReservedNodeExchangeOutputMessageTypeDef(TypedDict):
    ExchangedReservedNode: ReservedNodeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedNodeTypeDef](./type_defs.md#reservednodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PurchaseReservedNodeOfferingResultTypeDef

```python
# PurchaseReservedNodeOfferingResultTypeDef definition

class PurchaseReservedNodeOfferingResultTypeDef(TypedDict):
    ReservedNode: ReservedNodeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedNodeTypeDef](./type_defs.md#reservednodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReservedNodeConfigurationOptionTypeDef

```python
# ReservedNodeConfigurationOptionTypeDef definition

class ReservedNodeConfigurationOptionTypeDef(TypedDict):
    SourceReservedNode: NotRequired[ReservedNodeTypeDef],  # (1)
    TargetReservedNodeCount: NotRequired[int],
    TargetReservedNodeOffering: NotRequired[ReservedNodeOfferingTypeDef],  # (2)
```

1. See [:material-code-braces: ReservedNodeTypeDef](./type_defs.md#reservednodetypedef) 
2. See [:material-code-braces: ReservedNodeOfferingTypeDef](./type_defs.md#reservednodeofferingtypedef) 
## ReservedNodesMessageTypeDef

```python
# ReservedNodesMessageTypeDef definition

class ReservedNodesMessageTypeDef(TypedDict):
    Marker: str,
    ReservedNodes: List[ReservedNodeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedNodeTypeDef](./type_defs.md#reservednodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScheduledActionMessageRequestTypeDef

```python
# CreateScheduledActionMessageRequestTypeDef definition

class CreateScheduledActionMessageRequestTypeDef(TypedDict):
    ScheduledActionName: str,
    TargetAction: ScheduledActionTypeTypeDef,  # (1)
    Schedule: str,
    IamRole: str,
    ScheduledActionDescription: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Enable: NotRequired[bool],
```

1. See [:material-code-braces: ScheduledActionTypeTypeDef](./type_defs.md#scheduledactiontypetypedef) 
## ModifyScheduledActionMessageRequestTypeDef

```python
# ModifyScheduledActionMessageRequestTypeDef definition

class ModifyScheduledActionMessageRequestTypeDef(TypedDict):
    ScheduledActionName: str,
    TargetAction: NotRequired[ScheduledActionTypeTypeDef],  # (1)
    Schedule: NotRequired[str],
    IamRole: NotRequired[str],
    ScheduledActionDescription: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    Enable: NotRequired[bool],
```

1. See [:material-code-braces: ScheduledActionTypeTypeDef](./type_defs.md#scheduledactiontypetypedef) 
## ScheduledActionResponseTypeDef

```python
# ScheduledActionResponseTypeDef definition

class ScheduledActionResponseTypeDef(TypedDict):
    ScheduledActionName: str,
    TargetAction: ScheduledActionTypeTypeDef,  # (1)
    Schedule: str,
    IamRole: str,
    ScheduledActionDescription: str,
    State: ScheduledActionStateType,  # (2)
    NextInvocations: List[datetime],
    StartTime: datetime,
    EndTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ScheduledActionTypeTypeDef](./type_defs.md#scheduledactiontypetypedef) 
2. See [:material-code-brackets: ScheduledActionStateType](./literals.md#scheduledactionstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScheduledActionTypeDef

```python
# ScheduledActionTypeDef definition

class ScheduledActionTypeDef(TypedDict):
    ScheduledActionName: NotRequired[str],
    TargetAction: NotRequired[ScheduledActionTypeTypeDef],  # (1)
    Schedule: NotRequired[str],
    IamRole: NotRequired[str],
    ScheduledActionDescription: NotRequired[str],
    State: NotRequired[ScheduledActionStateType],  # (2)
    NextInvocations: NotRequired[List[datetime]],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-braces: ScheduledActionTypeTypeDef](./type_defs.md#scheduledactiontypetypedef) 
2. See [:material-code-brackets: ScheduledActionStateType](./literals.md#scheduledactionstatetype) 
## MaintenanceTrackTypeDef

```python
# MaintenanceTrackTypeDef definition

class MaintenanceTrackTypeDef(TypedDict):
    MaintenanceTrackName: NotRequired[str],
    DatabaseVersion: NotRequired[str],
    UpdateTargets: NotRequired[List[UpdateTargetTypeDef]],  # (1)
```

1. See [:material-code-braces: UpdateTargetTypeDef](./type_defs.md#updatetargettypedef) 
## OrderableClusterOptionsMessageTypeDef

```python
# OrderableClusterOptionsMessageTypeDef definition

class OrderableClusterOptionsMessageTypeDef(TypedDict):
    OrderableClusterOptions: List[OrderableClusterOptionTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrderableClusterOptionTypeDef](./type_defs.md#orderableclusteroptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterSubnetGroupTypeDef

```python
# ClusterSubnetGroupTypeDef definition

class ClusterSubnetGroupTypeDef(TypedDict):
    ClusterSubnetGroupName: NotRequired[str],
    Description: NotRequired[str],
    VpcId: NotRequired[str],
    SubnetGroupStatus: NotRequired[str],
    Subnets: NotRequired[List[SubnetTypeDef]],  # (1)
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    SupportedClusterIpAddressTypes: NotRequired[List[str]],
```

1. See [:material-code-braces: SubnetTypeDef](./type_defs.md#subnettypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AuthorizeClusterSecurityGroupIngressResultTypeDef

```python
# AuthorizeClusterSecurityGroupIngressResultTypeDef definition

class AuthorizeClusterSecurityGroupIngressResultTypeDef(TypedDict):
    ClusterSecurityGroup: ClusterSecurityGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSecurityGroupTypeDef](./type_defs.md#clustersecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterSecurityGroupMessageTypeDef

```python
# ClusterSecurityGroupMessageTypeDef definition

class ClusterSecurityGroupMessageTypeDef(TypedDict):
    Marker: str,
    ClusterSecurityGroups: List[ClusterSecurityGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSecurityGroupTypeDef](./type_defs.md#clustersecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterSecurityGroupResultTypeDef

```python
# CreateClusterSecurityGroupResultTypeDef definition

class CreateClusterSecurityGroupResultTypeDef(TypedDict):
    ClusterSecurityGroup: ClusterSecurityGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSecurityGroupTypeDef](./type_defs.md#clustersecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RevokeClusterSecurityGroupIngressResultTypeDef

```python
# RevokeClusterSecurityGroupIngressResultTypeDef definition

class RevokeClusterSecurityGroupIngressResultTypeDef(TypedDict):
    ClusterSecurityGroup: ClusterSecurityGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSecurityGroupTypeDef](./type_defs.md#clustersecuritygrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EndpointAccessListTypeDef

```python
# EndpointAccessListTypeDef definition

class EndpointAccessListTypeDef(TypedDict):
    EndpointAccessList: List[EndpointAccessTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointAccessTypeDef](./type_defs.md#endpointaccesstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterTypeDef

```python
# ClusterTypeDef definition

class ClusterTypeDef(TypedDict):
    ClusterIdentifier: NotRequired[str],
    NodeType: NotRequired[str],
    ClusterStatus: NotRequired[str],
    ClusterAvailabilityStatus: NotRequired[str],
    ModifyStatus: NotRequired[str],
    MasterUsername: NotRequired[str],
    DBName: NotRequired[str],
    Endpoint: NotRequired[EndpointTypeDef],  # (1)
    ClusterCreateTime: NotRequired[datetime],
    AutomatedSnapshotRetentionPeriod: NotRequired[int],
    ManualSnapshotRetentionPeriod: NotRequired[int],
    ClusterSecurityGroups: NotRequired[List[ClusterSecurityGroupMembershipTypeDef]],  # (2)
    VpcSecurityGroups: NotRequired[List[VpcSecurityGroupMembershipTypeDef]],  # (3)
    ClusterParameterGroups: NotRequired[List[ClusterParameterGroupStatusTypeDef]],  # (4)
    ClusterSubnetGroupName: NotRequired[str],
    VpcId: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    PendingModifiedValues: NotRequired[PendingModifiedValuesTypeDef],  # (5)
    ClusterVersion: NotRequired[str],
    AllowVersionUpgrade: NotRequired[bool],
    NumberOfNodes: NotRequired[int],
    PubliclyAccessible: NotRequired[bool],
    Encrypted: NotRequired[bool],
    RestoreStatus: NotRequired[RestoreStatusTypeDef],  # (6)
    DataTransferProgress: NotRequired[DataTransferProgressTypeDef],  # (7)
    HsmStatus: NotRequired[HsmStatusTypeDef],  # (8)
    ClusterSnapshotCopyStatus: NotRequired[ClusterSnapshotCopyStatusTypeDef],  # (9)
    ClusterPublicKey: NotRequired[str],
    ClusterNodes: NotRequired[List[ClusterNodeTypeDef]],  # (10)
    ElasticIpStatus: NotRequired[ElasticIpStatusTypeDef],  # (11)
    ClusterRevisionNumber: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (12)
    KmsKeyId: NotRequired[str],
    EnhancedVpcRouting: NotRequired[bool],
    IamRoles: NotRequired[List[ClusterIamRoleTypeDef]],  # (13)
    PendingActions: NotRequired[List[str]],
    MaintenanceTrackName: NotRequired[str],
    ElasticResizeNumberOfNodeOptions: NotRequired[str],
    DeferredMaintenanceWindows: NotRequired[List[DeferredMaintenanceWindowTypeDef]],  # (14)
    SnapshotScheduleIdentifier: NotRequired[str],
    SnapshotScheduleState: NotRequired[ScheduleStateType],  # (15)
    ExpectedNextSnapshotScheduleTime: NotRequired[datetime],
    ExpectedNextSnapshotScheduleTimeStatus: NotRequired[str],
    NextMaintenanceWindowStartTime: NotRequired[datetime],
    ResizeInfo: NotRequired[ResizeInfoTypeDef],  # (16)
    AvailabilityZoneRelocationStatus: NotRequired[str],
    ClusterNamespaceArn: NotRequired[str],
    TotalStorageCapacityInMegaBytes: NotRequired[int],
    AquaConfiguration: NotRequired[AquaConfigurationTypeDef],  # (17)
    DefaultIamRoleArn: NotRequired[str],
    ReservedNodeExchangeStatus: NotRequired[ReservedNodeExchangeStatusTypeDef],  # (18)
    CustomDomainName: NotRequired[str],
    CustomDomainCertificateArn: NotRequired[str],
    CustomDomainCertificateExpiryDate: NotRequired[datetime],
    MasterPasswordSecretArn: NotRequired[str],
    MasterPasswordSecretKmsKeyId: NotRequired[str],
    IpAddressType: NotRequired[str],
    MultiAZ: NotRequired[str],
    MultiAZSecondary: NotRequired[SecondaryClusterInfoTypeDef],  # (19)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ClusterSecurityGroupMembershipTypeDef](./type_defs.md#clustersecuritygroupmembershiptypedef) 
3. See [:material-code-braces: VpcSecurityGroupMembershipTypeDef](./type_defs.md#vpcsecuritygroupmembershiptypedef) 
4. See [:material-code-braces: ClusterParameterGroupStatusTypeDef](./type_defs.md#clusterparametergroupstatustypedef) 
5. See [:material-code-braces: PendingModifiedValuesTypeDef](./type_defs.md#pendingmodifiedvaluestypedef) 
6. See [:material-code-braces: RestoreStatusTypeDef](./type_defs.md#restorestatustypedef) 
7. See [:material-code-braces: DataTransferProgressTypeDef](./type_defs.md#datatransferprogresstypedef) 
8. See [:material-code-braces: HsmStatusTypeDef](./type_defs.md#hsmstatustypedef) 
9. See [:material-code-braces: ClusterSnapshotCopyStatusTypeDef](./type_defs.md#clustersnapshotcopystatustypedef) 
10. See [:material-code-braces: ClusterNodeTypeDef](./type_defs.md#clusternodetypedef) 
11. See [:material-code-braces: ElasticIpStatusTypeDef](./type_defs.md#elasticipstatustypedef) 
12. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
13. See [:material-code-braces: ClusterIamRoleTypeDef](./type_defs.md#clusteriamroletypedef) 
14. See [:material-code-braces: DeferredMaintenanceWindowTypeDef](./type_defs.md#deferredmaintenancewindowtypedef) 
15. See [:material-code-brackets: ScheduleStateType](./literals.md#schedulestatetype) 
16. See [:material-code-braces: ResizeInfoTypeDef](./type_defs.md#resizeinfotypedef) 
17. See [:material-code-braces: AquaConfigurationTypeDef](./type_defs.md#aquaconfigurationtypedef) 
18. See [:material-code-braces: ReservedNodeExchangeStatusTypeDef](./type_defs.md#reservednodeexchangestatustypedef) 
19. See [:material-code-braces: SecondaryClusterInfoTypeDef](./type_defs.md#secondaryclusterinfotypedef) 
## RedshiftIdcApplicationTypeDef

```python
# RedshiftIdcApplicationTypeDef definition

class RedshiftIdcApplicationTypeDef(TypedDict):
    IdcInstanceArn: NotRequired[str],
    RedshiftIdcApplicationName: NotRequired[str],
    RedshiftIdcApplicationArn: NotRequired[str],
    IdentityNamespace: NotRequired[str],
    IdcDisplayName: NotRequired[str],
    IamRoleArn: NotRequired[str],
    IdcManagedApplicationArn: NotRequired[str],
    IdcOnboardStatus: NotRequired[str],
    AuthorizedTokenIssuerList: NotRequired[List[AuthorizedTokenIssuerOutputTypeDef]],  # (1)
    ServiceIntegrations: NotRequired[List[ServiceIntegrationsUnionOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: AuthorizedTokenIssuerOutputTypeDef](./type_defs.md#authorizedtokenissueroutputtypedef) 
2. See [:material-code-braces: ServiceIntegrationsUnionOutputTypeDef](./type_defs.md#serviceintegrationsunionoutputtypedef) 
## ModifyRedshiftIdcApplicationMessageRequestTypeDef

```python
# ModifyRedshiftIdcApplicationMessageRequestTypeDef definition

class ModifyRedshiftIdcApplicationMessageRequestTypeDef(TypedDict):
    RedshiftIdcApplicationArn: str,
    IdentityNamespace: NotRequired[str],
    IamRoleArn: NotRequired[str],
    IdcDisplayName: NotRequired[str],
    AuthorizedTokenIssuerList: NotRequired[Sequence[AuthorizedTokenIssuerTypeDef]],  # (1)
    ServiceIntegrations: NotRequired[Sequence[ServiceIntegrationsUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: AuthorizedTokenIssuerTypeDef](./type_defs.md#authorizedtokenissuertypedef) 
2. See [:material-code-braces: ServiceIntegrationsUnionTypeDef](./type_defs.md#serviceintegrationsuniontypedef) 
## GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef

```python
# GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef definition

class GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef(TypedDict):
    Marker: str,
    ReservedNodeConfigurationOptionList: List[ReservedNodeConfigurationOptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedNodeConfigurationOptionTypeDef](./type_defs.md#reservednodeconfigurationoptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScheduledActionsMessageTypeDef

```python
# ScheduledActionsMessageTypeDef definition

class ScheduledActionsMessageTypeDef(TypedDict):
    Marker: str,
    ScheduledActions: List[ScheduledActionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduledActionTypeDef](./type_defs.md#scheduledactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrackListMessageTypeDef

```python
# TrackListMessageTypeDef definition

class TrackListMessageTypeDef(TypedDict):
    MaintenanceTracks: List[MaintenanceTrackTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MaintenanceTrackTypeDef](./type_defs.md#maintenancetracktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterSubnetGroupMessageTypeDef

```python
# ClusterSubnetGroupMessageTypeDef definition

class ClusterSubnetGroupMessageTypeDef(TypedDict):
    Marker: str,
    ClusterSubnetGroups: List[ClusterSubnetGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSubnetGroupTypeDef](./type_defs.md#clustersubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterSubnetGroupResultTypeDef

```python
# CreateClusterSubnetGroupResultTypeDef definition

class CreateClusterSubnetGroupResultTypeDef(TypedDict):
    ClusterSubnetGroup: ClusterSubnetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSubnetGroupTypeDef](./type_defs.md#clustersubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyClusterSubnetGroupResultTypeDef

```python
# ModifyClusterSubnetGroupResultTypeDef definition

class ModifyClusterSubnetGroupResultTypeDef(TypedDict):
    ClusterSubnetGroup: ClusterSubnetGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSubnetGroupTypeDef](./type_defs.md#clustersubnetgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClustersMessageTypeDef

```python
# ClustersMessageTypeDef definition

class ClustersMessageTypeDef(TypedDict):
    Marker: str,
    Clusters: List[ClusterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterResultTypeDef

```python
# CreateClusterResultTypeDef definition

class CreateClusterResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterResultTypeDef

```python
# DeleteClusterResultTypeDef definition

class DeleteClusterResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableSnapshotCopyResultTypeDef

```python
# DisableSnapshotCopyResultTypeDef definition

class DisableSnapshotCopyResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableSnapshotCopyResultTypeDef

```python
# EnableSnapshotCopyResultTypeDef definition

class EnableSnapshotCopyResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FailoverPrimaryComputeResultTypeDef

```python
# FailoverPrimaryComputeResultTypeDef definition

class FailoverPrimaryComputeResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyClusterDbRevisionResultTypeDef

```python
# ModifyClusterDbRevisionResultTypeDef definition

class ModifyClusterDbRevisionResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyClusterIamRolesResultTypeDef

```python
# ModifyClusterIamRolesResultTypeDef definition

class ModifyClusterIamRolesResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyClusterMaintenanceResultTypeDef

```python
# ModifyClusterMaintenanceResultTypeDef definition

class ModifyClusterMaintenanceResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyClusterResultTypeDef

```python
# ModifyClusterResultTypeDef definition

class ModifyClusterResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifySnapshotCopyRetentionPeriodResultTypeDef

```python
# ModifySnapshotCopyRetentionPeriodResultTypeDef definition

class ModifySnapshotCopyRetentionPeriodResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PauseClusterResultTypeDef

```python
# PauseClusterResultTypeDef definition

class PauseClusterResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RebootClusterResultTypeDef

```python
# RebootClusterResultTypeDef definition

class RebootClusterResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResizeClusterResultTypeDef

```python
# ResizeClusterResultTypeDef definition

class ResizeClusterResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreFromClusterSnapshotResultTypeDef

```python
# RestoreFromClusterSnapshotResultTypeDef definition

class RestoreFromClusterSnapshotResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResumeClusterResultTypeDef

```python
# ResumeClusterResultTypeDef definition

class ResumeClusterResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RotateEncryptionKeyResultTypeDef

```python
# RotateEncryptionKeyResultTypeDef definition

class RotateEncryptionKeyResultTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRedshiftIdcApplicationResultTypeDef

```python
# CreateRedshiftIdcApplicationResultTypeDef definition

class CreateRedshiftIdcApplicationResultTypeDef(TypedDict):
    RedshiftIdcApplication: RedshiftIdcApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RedshiftIdcApplicationTypeDef](./type_defs.md#redshiftidcapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRedshiftIdcApplicationsResultTypeDef

```python
# DescribeRedshiftIdcApplicationsResultTypeDef definition

class DescribeRedshiftIdcApplicationsResultTypeDef(TypedDict):
    RedshiftIdcApplications: List[RedshiftIdcApplicationTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RedshiftIdcApplicationTypeDef](./type_defs.md#redshiftidcapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyRedshiftIdcApplicationResultTypeDef

```python
# ModifyRedshiftIdcApplicationResultTypeDef definition

class ModifyRedshiftIdcApplicationResultTypeDef(TypedDict):
    RedshiftIdcApplication: RedshiftIdcApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RedshiftIdcApplicationTypeDef](./type_defs.md#redshiftidcapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRedshiftIdcApplicationMessageRequestTypeDef

```python
# CreateRedshiftIdcApplicationMessageRequestTypeDef definition

class CreateRedshiftIdcApplicationMessageRequestTypeDef(TypedDict):
    IdcInstanceArn: str,
    RedshiftIdcApplicationName: str,
    IdcDisplayName: str,
    IamRoleArn: str,
    IdentityNamespace: NotRequired[str],
    AuthorizedTokenIssuerList: NotRequired[Sequence[AuthorizedTokenIssuerUnionTypeDef]],  # (1)
    ServiceIntegrations: NotRequired[Sequence[ServiceIntegrationsUnionUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: AuthorizedTokenIssuerTypeDef](./type_defs.md#authorizedtokenissuertypedef) [:material-code-braces: AuthorizedTokenIssuerOutputTypeDef](./type_defs.md#authorizedtokenissueroutputtypedef) 
2. See [:material-code-braces: ServiceIntegrationsUnionTypeDef](./type_defs.md#serviceintegrationsuniontypedef) [:material-code-braces: ServiceIntegrationsUnionOutputTypeDef](./type_defs.md#serviceintegrationsunionoutputtypedef) 
