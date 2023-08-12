# Type definitions

> [Index](../README.md) > [OpenSearchService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [OpenSearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
    type annotations stubs module [types-aiobotocore-opensearch](https://pypi.org/project/types-aiobotocore-opensearch/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AWSDomainInformationTypeDef

```python
# AWSDomainInformationTypeDef definition

class AWSDomainInformationTypeDef(TypedDict):
    DomainName: str,
    OwnerId: NotRequired[str],
    Region: NotRequired[str],
```

## AcceptInboundConnectionRequestRequestTypeDef

```python
# AcceptInboundConnectionRequestRequestTypeDef definition

class AcceptInboundConnectionRequestRequestTypeDef(TypedDict):
    ConnectionId: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## OptionStatusTypeDef

```python
# OptionStatusTypeDef definition

class OptionStatusTypeDef(TypedDict):
    CreationDate: datetime,
    UpdateDate: datetime,
    State: OptionStateType,  # (1)
    UpdateVersion: NotRequired[int],
    PendingDeletion: NotRequired[bool],
```

1. See [:material-code-brackets: OptionStateType](./literals.md#optionstatetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## AdditionalLimitTypeDef

```python
# AdditionalLimitTypeDef definition

class AdditionalLimitTypeDef(TypedDict):
    LimitName: NotRequired[str],
    LimitValues: NotRequired[List[str]],
```

## MasterUserOptionsTypeDef

```python
# MasterUserOptionsTypeDef definition

class MasterUserOptionsTypeDef(TypedDict):
    MasterUserARN: NotRequired[str],
    MasterUserName: NotRequired[str],
    MasterUserPassword: NotRequired[str],
```

## AssociatePackageRequestRequestTypeDef

```python
# AssociatePackageRequestRequestTypeDef definition

class AssociatePackageRequestRequestTypeDef(TypedDict):
    PackageID: str,
    DomainName: str,
```

## AuthorizeVpcEndpointAccessRequestRequestTypeDef

```python
# AuthorizeVpcEndpointAccessRequestRequestTypeDef definition

class AuthorizeVpcEndpointAccessRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Account: str,
```

## AuthorizedPrincipalTypeDef

```python
# AuthorizedPrincipalTypeDef definition

class AuthorizedPrincipalTypeDef(TypedDict):
    PrincipalType: NotRequired[PrincipalTypeType],  # (1)
    Principal: NotRequired[str],
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## ScheduledAutoTuneDetailsTypeDef

```python
# ScheduledAutoTuneDetailsTypeDef definition

class ScheduledAutoTuneDetailsTypeDef(TypedDict):
    Date: NotRequired[datetime],
    ActionType: NotRequired[ScheduledAutoTuneActionTypeType],  # (1)
    Action: NotRequired[str],
    Severity: NotRequired[ScheduledAutoTuneSeverityTypeType],  # (2)
```

1. See [:material-code-brackets: ScheduledAutoTuneActionTypeType](./literals.md#scheduledautotuneactiontypetype) 
2. See [:material-code-brackets: ScheduledAutoTuneSeverityTypeType](./literals.md#scheduledautotuneseveritytypetype) 
## DurationTypeDef

```python
# DurationTypeDef definition

class DurationTypeDef(TypedDict):
    Value: NotRequired[int],
    Unit: NotRequired[TimeUnitType],  # (1)
```

1. See [:material-code-brackets: TimeUnitType](./literals.md#timeunittype) 
## AutoTuneOptionsOutputTypeDef

```python
# AutoTuneOptionsOutputTypeDef definition

class AutoTuneOptionsOutputTypeDef(TypedDict):
    State: NotRequired[AutoTuneStateType],  # (1)
    ErrorMessage: NotRequired[str],
    UseOffPeakWindow: NotRequired[bool],
```

1. See [:material-code-brackets: AutoTuneStateType](./literals.md#autotunestatetype) 
## AutoTuneStatusTypeDef

```python
# AutoTuneStatusTypeDef definition

class AutoTuneStatusTypeDef(TypedDict):
    CreationDate: datetime,
    UpdateDate: datetime,
    State: AutoTuneStateType,  # (1)
    UpdateVersion: NotRequired[int],
    ErrorMessage: NotRequired[str],
    PendingDeletion: NotRequired[bool],
```

1. See [:material-code-brackets: AutoTuneStateType](./literals.md#autotunestatetype) 
## AvailabilityZoneInfoTypeDef

```python
# AvailabilityZoneInfoTypeDef definition

class AvailabilityZoneInfoTypeDef(TypedDict):
    AvailabilityZoneName: NotRequired[str],
    ZoneStatus: NotRequired[ZoneStatusType],  # (1)
    ConfiguredDataNodeCount: NotRequired[str],
    AvailableDataNodeCount: NotRequired[str],
    TotalShards: NotRequired[str],
    TotalUnAssignedShards: NotRequired[str],
```

1. See [:material-code-brackets: ZoneStatusType](./literals.md#zonestatustype) 
## CancelServiceSoftwareUpdateRequestRequestTypeDef

```python
# CancelServiceSoftwareUpdateRequestRequestTypeDef definition

class CancelServiceSoftwareUpdateRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## ServiceSoftwareOptionsTypeDef

```python
# ServiceSoftwareOptionsTypeDef definition

class ServiceSoftwareOptionsTypeDef(TypedDict):
    CurrentVersion: NotRequired[str],
    NewVersion: NotRequired[str],
    UpdateAvailable: NotRequired[bool],
    Cancellable: NotRequired[bool],
    UpdateStatus: NotRequired[DeploymentStatusType],  # (1)
    Description: NotRequired[str],
    AutomatedUpdateDate: NotRequired[datetime],
    OptionalDeployment: NotRequired[bool],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
## ChangeProgressDetailsTypeDef

```python
# ChangeProgressDetailsTypeDef definition

class ChangeProgressDetailsTypeDef(TypedDict):
    ChangeId: NotRequired[str],
    Message: NotRequired[str],
```

## ChangeProgressStageTypeDef

```python
# ChangeProgressStageTypeDef definition

class ChangeProgressStageTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[str],
    Description: NotRequired[str],
    LastUpdated: NotRequired[datetime],
```

## ColdStorageOptionsTypeDef

```python
# ColdStorageOptionsTypeDef definition

class ColdStorageOptionsTypeDef(TypedDict):
    Enabled: bool,
```

## ZoneAwarenessConfigTypeDef

```python
# ZoneAwarenessConfigTypeDef definition

class ZoneAwarenessConfigTypeDef(TypedDict):
    AvailabilityZoneCount: NotRequired[int],
```

## CognitoOptionsTypeDef

```python
# CognitoOptionsTypeDef definition

class CognitoOptionsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    UserPoolId: NotRequired[str],
    IdentityPoolId: NotRequired[str],
    RoleArn: NotRequired[str],
```

## CompatibleVersionsMapTypeDef

```python
# CompatibleVersionsMapTypeDef definition

class CompatibleVersionsMapTypeDef(TypedDict):
    SourceVersion: NotRequired[str],
    TargetVersions: NotRequired[List[str]],
```

## CrossClusterSearchConnectionPropertiesTypeDef

```python
# CrossClusterSearchConnectionPropertiesTypeDef definition

class CrossClusterSearchConnectionPropertiesTypeDef(TypedDict):
    SkipUnavailable: NotRequired[SkipUnavailableStatusType],  # (1)
```

1. See [:material-code-brackets: SkipUnavailableStatusType](./literals.md#skipunavailablestatustype) 
## DomainEndpointOptionsTypeDef

```python
# DomainEndpointOptionsTypeDef definition

class DomainEndpointOptionsTypeDef(TypedDict):
    EnforceHTTPS: NotRequired[bool],
    TLSSecurityPolicy: NotRequired[TLSSecurityPolicyType],  # (1)
    CustomEndpointEnabled: NotRequired[bool],
    CustomEndpoint: NotRequired[str],
    CustomEndpointCertificateArn: NotRequired[str],
```

1. See [:material-code-brackets: TLSSecurityPolicyType](./literals.md#tlssecuritypolicytype) 
## EBSOptionsTypeDef

```python
# EBSOptionsTypeDef definition

class EBSOptionsTypeDef(TypedDict):
    EBSEnabled: NotRequired[bool],
    VolumeType: NotRequired[VolumeTypeType],  # (1)
    VolumeSize: NotRequired[int],
    Iops: NotRequired[int],
    Throughput: NotRequired[int],
```

1. See [:material-code-brackets: VolumeTypeType](./literals.md#volumetypetype) 
## EncryptionAtRestOptionsTypeDef

```python
# EncryptionAtRestOptionsTypeDef definition

class EncryptionAtRestOptionsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    KmsKeyId: NotRequired[str],
```

## LogPublishingOptionTypeDef

```python
# LogPublishingOptionTypeDef definition

class LogPublishingOptionTypeDef(TypedDict):
    CloudWatchLogsLogGroupArn: NotRequired[str],
    Enabled: NotRequired[bool],
```

## NodeToNodeEncryptionOptionsTypeDef

```python
# NodeToNodeEncryptionOptionsTypeDef definition

class NodeToNodeEncryptionOptionsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## SnapshotOptionsTypeDef

```python
# SnapshotOptionsTypeDef definition

class SnapshotOptionsTypeDef(TypedDict):
    AutomatedSnapshotStartHour: NotRequired[int],
```

## SoftwareUpdateOptionsTypeDef

```python
# SoftwareUpdateOptionsTypeDef definition

class SoftwareUpdateOptionsTypeDef(TypedDict):
    AutoSoftwareUpdateEnabled: NotRequired[bool],
```

## VPCOptionsTypeDef

```python
# VPCOptionsTypeDef definition

class VPCOptionsTypeDef(TypedDict):
    SubnetIds: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
```

## OutboundConnectionStatusTypeDef

```python
# OutboundConnectionStatusTypeDef definition

class OutboundConnectionStatusTypeDef(TypedDict):
    StatusCode: NotRequired[OutboundConnectionStatusCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: OutboundConnectionStatusCodeType](./literals.md#outboundconnectionstatuscodetype) 
## PackageSourceTypeDef

```python
# PackageSourceTypeDef definition

class PackageSourceTypeDef(TypedDict):
    S3BucketName: NotRequired[str],
    S3Key: NotRequired[str],
```

## DeleteDomainRequestRequestTypeDef

```python
# DeleteDomainRequestRequestTypeDef definition

class DeleteDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DeleteInboundConnectionRequestRequestTypeDef

```python
# DeleteInboundConnectionRequestRequestTypeDef definition

class DeleteInboundConnectionRequestRequestTypeDef(TypedDict):
    ConnectionId: str,
```

## DeleteOutboundConnectionRequestRequestTypeDef

```python
# DeleteOutboundConnectionRequestRequestTypeDef definition

class DeleteOutboundConnectionRequestRequestTypeDef(TypedDict):
    ConnectionId: str,
```

## DeletePackageRequestRequestTypeDef

```python
# DeletePackageRequestRequestTypeDef definition

class DeletePackageRequestRequestTypeDef(TypedDict):
    PackageID: str,
```

## DeleteVpcEndpointRequestRequestTypeDef

```python
# DeleteVpcEndpointRequestRequestTypeDef definition

class DeleteVpcEndpointRequestRequestTypeDef(TypedDict):
    VpcEndpointId: str,
```

## VpcEndpointSummaryTypeDef

```python
# VpcEndpointSummaryTypeDef definition

class VpcEndpointSummaryTypeDef(TypedDict):
    VpcEndpointId: NotRequired[str],
    VpcEndpointOwner: NotRequired[str],
    DomainArn: NotRequired[str],
    Status: NotRequired[VpcEndpointStatusType],  # (1)
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## DescribeDomainAutoTunesRequestRequestTypeDef

```python
# DescribeDomainAutoTunesRequestRequestTypeDef definition

class DescribeDomainAutoTunesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeDomainChangeProgressRequestRequestTypeDef

```python
# DescribeDomainChangeProgressRequestRequestTypeDef definition

class DescribeDomainChangeProgressRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ChangeId: NotRequired[str],
```

## DescribeDomainConfigRequestRequestTypeDef

```python
# DescribeDomainConfigRequestRequestTypeDef definition

class DescribeDomainConfigRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DescribeDomainHealthRequestRequestTypeDef

```python
# DescribeDomainHealthRequestRequestTypeDef definition

class DescribeDomainHealthRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DescribeDomainNodesRequestRequestTypeDef

```python
# DescribeDomainNodesRequestRequestTypeDef definition

class DescribeDomainNodesRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DomainNodesStatusTypeDef

```python
# DomainNodesStatusTypeDef definition

class DomainNodesStatusTypeDef(TypedDict):
    NodeId: NotRequired[str],
    NodeType: NotRequired[NodeTypeType],  # (1)
    AvailabilityZone: NotRequired[str],
    InstanceType: NotRequired[OpenSearchPartitionInstanceTypeType],  # (2)
    NodeStatus: NotRequired[NodeStatusType],  # (3)
    StorageType: NotRequired[str],
    StorageVolumeType: NotRequired[VolumeTypeType],  # (4)
    StorageSize: NotRequired[str],
```

1. See [:material-code-brackets: NodeTypeType](./literals.md#nodetypetype) 
2. See [:material-code-brackets: OpenSearchPartitionInstanceTypeType](./literals.md#opensearchpartitioninstancetypetype) 
3. See [:material-code-brackets: NodeStatusType](./literals.md#nodestatustype) 
4. See [:material-code-brackets: VolumeTypeType](./literals.md#volumetypetype) 
## DescribeDomainRequestRequestTypeDef

```python
# DescribeDomainRequestRequestTypeDef definition

class DescribeDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DescribeDomainsRequestRequestTypeDef

```python
# DescribeDomainsRequestRequestTypeDef definition

class DescribeDomainsRequestRequestTypeDef(TypedDict):
    DomainNames: Sequence[str],
```

## DescribeDryRunProgressRequestRequestTypeDef

```python
# DescribeDryRunProgressRequestRequestTypeDef definition

class DescribeDryRunProgressRequestRequestTypeDef(TypedDict):
    DomainName: str,
    DryRunId: NotRequired[str],
    LoadDryRunConfig: NotRequired[bool],
```

## DryRunResultsTypeDef

```python
# DryRunResultsTypeDef definition

class DryRunResultsTypeDef(TypedDict):
    DeploymentType: NotRequired[str],
    Message: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## DescribeInstanceTypeLimitsRequestRequestTypeDef

```python
# DescribeInstanceTypeLimitsRequestRequestTypeDef definition

class DescribeInstanceTypeLimitsRequestRequestTypeDef(TypedDict):
    InstanceType: OpenSearchPartitionInstanceTypeType,  # (1)
    EngineVersion: str,
    DomainName: NotRequired[str],
```

1. See [:material-code-brackets: OpenSearchPartitionInstanceTypeType](./literals.md#opensearchpartitioninstancetypetype) 
## DescribePackagesFilterTypeDef

```python
# DescribePackagesFilterTypeDef definition

class DescribePackagesFilterTypeDef(TypedDict):
    Name: NotRequired[DescribePackagesFilterNameType],  # (1)
    Value: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: DescribePackagesFilterNameType](./literals.md#describepackagesfilternametype) 
## DescribeReservedInstanceOfferingsRequestRequestTypeDef

```python
# DescribeReservedInstanceOfferingsRequestRequestTypeDef definition

class DescribeReservedInstanceOfferingsRequestRequestTypeDef(TypedDict):
    ReservedInstanceOfferingId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeReservedInstancesRequestRequestTypeDef

```python
# DescribeReservedInstancesRequestRequestTypeDef definition

class DescribeReservedInstancesRequestRequestTypeDef(TypedDict):
    ReservedInstanceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeVpcEndpointsRequestRequestTypeDef

```python
# DescribeVpcEndpointsRequestRequestTypeDef definition

class DescribeVpcEndpointsRequestRequestTypeDef(TypedDict):
    VpcEndpointIds: Sequence[str],
```

## VpcEndpointErrorTypeDef

```python
# VpcEndpointErrorTypeDef definition

class VpcEndpointErrorTypeDef(TypedDict):
    VpcEndpointId: NotRequired[str],
    ErrorCode: NotRequired[VpcEndpointErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: VpcEndpointErrorCodeType](./literals.md#vpcendpointerrorcodetype) 
## DissociatePackageRequestRequestTypeDef

```python
# DissociatePackageRequestRequestTypeDef definition

class DissociatePackageRequestRequestTypeDef(TypedDict):
    PackageID: str,
    DomainName: str,
```

## DomainInfoTypeDef

```python
# DomainInfoTypeDef definition

class DomainInfoTypeDef(TypedDict):
    DomainName: NotRequired[str],
    EngineType: NotRequired[EngineTypeType],  # (1)
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    ErrorType: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## VPCDerivedInfoTypeDef

```python
# VPCDerivedInfoTypeDef definition

class VPCDerivedInfoTypeDef(TypedDict):
    VPCId: NotRequired[str],
    SubnetIds: NotRequired[List[str]],
    AvailabilityZones: NotRequired[List[str]],
    SecurityGroupIds: NotRequired[List[str]],
```

## ValidationFailureTypeDef

```python
# ValidationFailureTypeDef definition

class ValidationFailureTypeDef(TypedDict):
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## GetCompatibleVersionsRequestRequestTypeDef

```python
# GetCompatibleVersionsRequestRequestTypeDef definition

class GetCompatibleVersionsRequestRequestTypeDef(TypedDict):
    DomainName: NotRequired[str],
```

## GetPackageVersionHistoryRequestRequestTypeDef

```python
# GetPackageVersionHistoryRequestRequestTypeDef definition

class GetPackageVersionHistoryRequestRequestTypeDef(TypedDict):
    PackageID: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PackageVersionHistoryTypeDef

```python
# PackageVersionHistoryTypeDef definition

class PackageVersionHistoryTypeDef(TypedDict):
    PackageVersion: NotRequired[str],
    CommitMessage: NotRequired[str],
    CreatedAt: NotRequired[datetime],
```

## GetUpgradeHistoryRequestRequestTypeDef

```python
# GetUpgradeHistoryRequestRequestTypeDef definition

class GetUpgradeHistoryRequestRequestTypeDef(TypedDict):
    DomainName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetUpgradeStatusRequestRequestTypeDef

```python
# GetUpgradeStatusRequestRequestTypeDef definition

class GetUpgradeStatusRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## InboundConnectionStatusTypeDef

```python
# InboundConnectionStatusTypeDef definition

class InboundConnectionStatusTypeDef(TypedDict):
    StatusCode: NotRequired[InboundConnectionStatusCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: InboundConnectionStatusCodeType](./literals.md#inboundconnectionstatuscodetype) 
## InstanceCountLimitsTypeDef

```python
# InstanceCountLimitsTypeDef definition

class InstanceCountLimitsTypeDef(TypedDict):
    MinimumInstanceCount: NotRequired[int],
    MaximumInstanceCount: NotRequired[int],
```

## InstanceTypeDetailsTypeDef

```python
# InstanceTypeDetailsTypeDef definition

class InstanceTypeDetailsTypeDef(TypedDict):
    InstanceType: NotRequired[OpenSearchPartitionInstanceTypeType],  # (1)
    EncryptionEnabled: NotRequired[bool],
    CognitoEnabled: NotRequired[bool],
    AppLogsEnabled: NotRequired[bool],
    AdvancedSecurityEnabled: NotRequired[bool],
    WarmEnabled: NotRequired[bool],
    InstanceRole: NotRequired[List[str]],
    AvailabilityZones: NotRequired[List[str]],
```

1. See [:material-code-brackets: OpenSearchPartitionInstanceTypeType](./literals.md#opensearchpartitioninstancetypetype) 
## ListDomainNamesRequestRequestTypeDef

```python
# ListDomainNamesRequestRequestTypeDef definition

class ListDomainNamesRequestRequestTypeDef(TypedDict):
    EngineType: NotRequired[EngineTypeType],  # (1)
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
## ListDomainsForPackageRequestRequestTypeDef

```python
# ListDomainsForPackageRequestRequestTypeDef definition

class ListDomainsForPackageRequestRequestTypeDef(TypedDict):
    PackageID: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListInstanceTypeDetailsRequestRequestTypeDef

```python
# ListInstanceTypeDetailsRequestRequestTypeDef definition

class ListInstanceTypeDetailsRequestRequestTypeDef(TypedDict):
    EngineVersion: str,
    DomainName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    RetrieveAZs: NotRequired[bool],
    InstanceType: NotRequired[str],
```

## ListPackagesForDomainRequestRequestTypeDef

```python
# ListPackagesForDomainRequestRequestTypeDef definition

class ListPackagesForDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListScheduledActionsRequestRequestTypeDef

```python
# ListScheduledActionsRequestRequestTypeDef definition

class ListScheduledActionsRequestRequestTypeDef(TypedDict):
    DomainName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ScheduledActionTypeDef

```python
# ScheduledActionTypeDef definition

class ScheduledActionTypeDef(TypedDict):
    Id: str,
    Type: ActionTypeType,  # (1)
    Severity: ActionSeverityType,  # (2)
    ScheduledTime: int,
    Description: NotRequired[str],
    ScheduledBy: NotRequired[ScheduledByType],  # (3)
    Status: NotRequired[ActionStatusType],  # (4)
    Mandatory: NotRequired[bool],
    Cancellable: NotRequired[bool],
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-brackets: ActionSeverityType](./literals.md#actionseveritytype) 
3. See [:material-code-brackets: ScheduledByType](./literals.md#scheduledbytype) 
4. See [:material-code-brackets: ActionStatusType](./literals.md#actionstatustype) 
## ListTagsRequestRequestTypeDef

```python
# ListTagsRequestRequestTypeDef definition

class ListTagsRequestRequestTypeDef(TypedDict):
    ARN: str,
```

## ListVersionsRequestRequestTypeDef

```python
# ListVersionsRequestRequestTypeDef definition

class ListVersionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListVpcEndpointAccessRequestRequestTypeDef

```python
# ListVpcEndpointAccessRequestRequestTypeDef definition

class ListVpcEndpointAccessRequestRequestTypeDef(TypedDict):
    DomainName: str,
    NextToken: NotRequired[str],
```

## ListVpcEndpointsForDomainRequestRequestTypeDef

```python
# ListVpcEndpointsForDomainRequestRequestTypeDef definition

class ListVpcEndpointsForDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    NextToken: NotRequired[str],
```

## ListVpcEndpointsRequestRequestTypeDef

```python
# ListVpcEndpointsRequestRequestTypeDef definition

class ListVpcEndpointsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## WindowStartTimeTypeDef

```python
# WindowStartTimeTypeDef definition

class WindowStartTimeTypeDef(TypedDict):
    Hours: int,
    Minutes: int,
```

## PurchaseReservedInstanceOfferingRequestRequestTypeDef

```python
# PurchaseReservedInstanceOfferingRequestRequestTypeDef definition

class PurchaseReservedInstanceOfferingRequestRequestTypeDef(TypedDict):
    ReservedInstanceOfferingId: str,
    ReservationName: str,
    InstanceCount: NotRequired[int],
```

## RecurringChargeTypeDef

```python
# RecurringChargeTypeDef definition

class RecurringChargeTypeDef(TypedDict):
    RecurringChargeAmount: NotRequired[float],
    RecurringChargeFrequency: NotRequired[str],
```

## RejectInboundConnectionRequestRequestTypeDef

```python
# RejectInboundConnectionRequestRequestTypeDef definition

class RejectInboundConnectionRequestRequestTypeDef(TypedDict):
    ConnectionId: str,
```

## RemoveTagsRequestRequestTypeDef

```python
# RemoveTagsRequestRequestTypeDef definition

class RemoveTagsRequestRequestTypeDef(TypedDict):
    ARN: str,
    TagKeys: Sequence[str],
```

## RevokeVpcEndpointAccessRequestRequestTypeDef

```python
# RevokeVpcEndpointAccessRequestRequestTypeDef definition

class RevokeVpcEndpointAccessRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Account: str,
```

## SAMLIdpTypeDef

```python
# SAMLIdpTypeDef definition

class SAMLIdpTypeDef(TypedDict):
    MetadataContent: str,
    EntityId: str,
```

## StartServiceSoftwareUpdateRequestRequestTypeDef

```python
# StartServiceSoftwareUpdateRequestRequestTypeDef definition

class StartServiceSoftwareUpdateRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ScheduleAt: NotRequired[ScheduleAtType],  # (1)
    DesiredStartTime: NotRequired[int],
```

1. See [:material-code-brackets: ScheduleAtType](./literals.md#scheduleattype) 
## StorageTypeLimitTypeDef

```python
# StorageTypeLimitTypeDef definition

class StorageTypeLimitTypeDef(TypedDict):
    LimitName: NotRequired[str],
    LimitValues: NotRequired[List[str]],
```

## UpdateScheduledActionRequestRequestTypeDef

```python
# UpdateScheduledActionRequestRequestTypeDef definition

class UpdateScheduledActionRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ActionID: str,
    ActionType: ActionTypeType,  # (1)
    ScheduleAt: ScheduleAtType,  # (2)
    DesiredStartTime: NotRequired[int],
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-brackets: ScheduleAtType](./literals.md#scheduleattype) 
## UpgradeDomainRequestRequestTypeDef

```python
# UpgradeDomainRequestRequestTypeDef definition

class UpgradeDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    TargetVersion: str,
    PerformCheckOnly: NotRequired[bool],
    AdvancedOptions: NotRequired[Mapping[str, str]],
```

## UpgradeStepItemTypeDef

```python
# UpgradeStepItemTypeDef definition

class UpgradeStepItemTypeDef(TypedDict):
    UpgradeStep: NotRequired[UpgradeStepType],  # (1)
    UpgradeStepStatus: NotRequired[UpgradeStatusType],  # (2)
    Issues: NotRequired[List[str]],
    ProgressPercent: NotRequired[float],
```

1. See [:material-code-brackets: UpgradeStepType](./literals.md#upgradesteptype) 
2. See [:material-code-brackets: UpgradeStatusType](./literals.md#upgradestatustype) 
## DomainInformationContainerTypeDef

```python
# DomainInformationContainerTypeDef definition

class DomainInformationContainerTypeDef(TypedDict):
    AWSDomainInformation: NotRequired[AWSDomainInformationTypeDef],  # (1)
```

1. See [:material-code-braces: AWSDomainInformationTypeDef](./type_defs.md#awsdomaininformationtypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUpgradeStatusResponseTypeDef

```python
# GetUpgradeStatusResponseTypeDef definition

class GetUpgradeStatusResponseTypeDef(TypedDict):
    UpgradeStep: UpgradeStepType,  # (1)
    StepStatus: UpgradeStatusType,  # (2)
    UpgradeName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: UpgradeStepType](./literals.md#upgradesteptype) 
2. See [:material-code-brackets: UpgradeStatusType](./literals.md#upgradestatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVersionsResponseTypeDef

```python
# ListVersionsResponseTypeDef definition

class ListVersionsResponseTypeDef(TypedDict):
    Versions: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PurchaseReservedInstanceOfferingResponseTypeDef

```python
# PurchaseReservedInstanceOfferingResponseTypeDef definition

class PurchaseReservedInstanceOfferingResponseTypeDef(TypedDict):
    ReservedInstanceId: str,
    ReservationName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AccessPoliciesStatusTypeDef

```python
# AccessPoliciesStatusTypeDef definition

class AccessPoliciesStatusTypeDef(TypedDict):
    Options: str,
    Status: OptionStatusTypeDef,  # (1)
```

1. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## AdvancedOptionsStatusTypeDef

```python
# AdvancedOptionsStatusTypeDef definition

class AdvancedOptionsStatusTypeDef(TypedDict):
    Options: Dict[str, str],
    Status: OptionStatusTypeDef,  # (1)
```

1. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## VersionStatusTypeDef

```python
# VersionStatusTypeDef definition

class VersionStatusTypeDef(TypedDict):
    Options: str,
    Status: OptionStatusTypeDef,  # (1)
```

1. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## AddTagsRequestRequestTypeDef

```python
# AddTagsRequestRequestTypeDef definition

class AddTagsRequestRequestTypeDef(TypedDict):
    ARN: str,
    TagList: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsResponseTypeDef

```python
# ListTagsResponseTypeDef definition

class ListTagsResponseTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AuthorizeVpcEndpointAccessResponseTypeDef

```python
# AuthorizeVpcEndpointAccessResponseTypeDef definition

class AuthorizeVpcEndpointAccessResponseTypeDef(TypedDict):
    AuthorizedPrincipal: AuthorizedPrincipalTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthorizedPrincipalTypeDef](./type_defs.md#authorizedprincipaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVpcEndpointAccessResponseTypeDef

```python
# ListVpcEndpointAccessResponseTypeDef definition

class ListVpcEndpointAccessResponseTypeDef(TypedDict):
    AuthorizedPrincipalList: List[AuthorizedPrincipalTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthorizedPrincipalTypeDef](./type_defs.md#authorizedprincipaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoTuneDetailsTypeDef

```python
# AutoTuneDetailsTypeDef definition

class AutoTuneDetailsTypeDef(TypedDict):
    ScheduledAutoTuneDetails: NotRequired[ScheduledAutoTuneDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: ScheduledAutoTuneDetailsTypeDef](./type_defs.md#scheduledautotunedetailstypedef) 
## AutoTuneMaintenanceScheduleTypeDef

```python
# AutoTuneMaintenanceScheduleTypeDef definition

class AutoTuneMaintenanceScheduleTypeDef(TypedDict):
    StartAt: NotRequired[Union[datetime, str]],
    Duration: NotRequired[DurationTypeDef],  # (1)
    CronExpressionForRecurrence: NotRequired[str],
```

1. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
## EnvironmentInfoTypeDef

```python
# EnvironmentInfoTypeDef definition

class EnvironmentInfoTypeDef(TypedDict):
    AvailabilityZoneInformation: NotRequired[List[AvailabilityZoneInfoTypeDef]],  # (1)
```

1. See [:material-code-braces: AvailabilityZoneInfoTypeDef](./type_defs.md#availabilityzoneinfotypedef) 
## CancelServiceSoftwareUpdateResponseTypeDef

```python
# CancelServiceSoftwareUpdateResponseTypeDef definition

class CancelServiceSoftwareUpdateResponseTypeDef(TypedDict):
    ServiceSoftwareOptions: ServiceSoftwareOptionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSoftwareOptionsTypeDef](./type_defs.md#servicesoftwareoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartServiceSoftwareUpdateResponseTypeDef

```python
# StartServiceSoftwareUpdateResponseTypeDef definition

class StartServiceSoftwareUpdateResponseTypeDef(TypedDict):
    ServiceSoftwareOptions: ServiceSoftwareOptionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSoftwareOptionsTypeDef](./type_defs.md#servicesoftwareoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpgradeDomainResponseTypeDef

```python
# UpgradeDomainResponseTypeDef definition

class UpgradeDomainResponseTypeDef(TypedDict):
    UpgradeId: str,
    DomainName: str,
    TargetVersion: str,
    PerformCheckOnly: bool,
    AdvancedOptions: Dict[str, str],
    ChangeProgressDetails: ChangeProgressDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeProgressDetailsTypeDef](./type_defs.md#changeprogressdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChangeProgressStatusDetailsTypeDef

```python
# ChangeProgressStatusDetailsTypeDef definition

class ChangeProgressStatusDetailsTypeDef(TypedDict):
    ChangeId: NotRequired[str],
    StartTime: NotRequired[datetime],
    Status: NotRequired[OverallChangeStatusType],  # (1)
    PendingProperties: NotRequired[List[str]],
    CompletedProperties: NotRequired[List[str]],
    TotalNumberOfStages: NotRequired[int],
    ChangeProgressStages: NotRequired[List[ChangeProgressStageTypeDef]],  # (2)
```

1. See [:material-code-brackets: OverallChangeStatusType](./literals.md#overallchangestatustype) 
2. See [:material-code-braces: ChangeProgressStageTypeDef](./type_defs.md#changeprogressstagetypedef) 
## ClusterConfigTypeDef

```python
# ClusterConfigTypeDef definition

class ClusterConfigTypeDef(TypedDict):
    InstanceType: NotRequired[OpenSearchPartitionInstanceTypeType],  # (1)
    InstanceCount: NotRequired[int],
    DedicatedMasterEnabled: NotRequired[bool],
    ZoneAwarenessEnabled: NotRequired[bool],
    ZoneAwarenessConfig: NotRequired[ZoneAwarenessConfigTypeDef],  # (2)
    DedicatedMasterType: NotRequired[OpenSearchPartitionInstanceTypeType],  # (1)
    DedicatedMasterCount: NotRequired[int],
    WarmEnabled: NotRequired[bool],
    WarmType: NotRequired[OpenSearchWarmPartitionInstanceTypeType],  # (4)
    WarmCount: NotRequired[int],
    ColdStorageOptions: NotRequired[ColdStorageOptionsTypeDef],  # (5)
    MultiAZWithStandbyEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: OpenSearchPartitionInstanceTypeType](./literals.md#opensearchpartitioninstancetypetype) 
2. See [:material-code-braces: ZoneAwarenessConfigTypeDef](./type_defs.md#zoneawarenessconfigtypedef) 
3. See [:material-code-brackets: OpenSearchPartitionInstanceTypeType](./literals.md#opensearchpartitioninstancetypetype) 
4. See [:material-code-brackets: OpenSearchWarmPartitionInstanceTypeType](./literals.md#opensearchwarmpartitioninstancetypetype) 
5. See [:material-code-braces: ColdStorageOptionsTypeDef](./type_defs.md#coldstorageoptionstypedef) 
## CognitoOptionsStatusTypeDef

```python
# CognitoOptionsStatusTypeDef definition

class CognitoOptionsStatusTypeDef(TypedDict):
    Options: CognitoOptionsTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: CognitoOptionsTypeDef](./type_defs.md#cognitooptionstypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## GetCompatibleVersionsResponseTypeDef

```python
# GetCompatibleVersionsResponseTypeDef definition

class GetCompatibleVersionsResponseTypeDef(TypedDict):
    CompatibleVersions: List[CompatibleVersionsMapTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompatibleVersionsMapTypeDef](./type_defs.md#compatibleversionsmaptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionPropertiesTypeDef

```python
# ConnectionPropertiesTypeDef definition

class ConnectionPropertiesTypeDef(TypedDict):
    Endpoint: NotRequired[str],
    CrossClusterSearch: NotRequired[CrossClusterSearchConnectionPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: CrossClusterSearchConnectionPropertiesTypeDef](./type_defs.md#crossclustersearchconnectionpropertiestypedef) 
## DomainEndpointOptionsStatusTypeDef

```python
# DomainEndpointOptionsStatusTypeDef definition

class DomainEndpointOptionsStatusTypeDef(TypedDict):
    Options: DomainEndpointOptionsTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: DomainEndpointOptionsTypeDef](./type_defs.md#domainendpointoptionstypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## EBSOptionsStatusTypeDef

```python
# EBSOptionsStatusTypeDef definition

class EBSOptionsStatusTypeDef(TypedDict):
    Options: EBSOptionsTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: EBSOptionsTypeDef](./type_defs.md#ebsoptionstypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## EncryptionAtRestOptionsStatusTypeDef

```python
# EncryptionAtRestOptionsStatusTypeDef definition

class EncryptionAtRestOptionsStatusTypeDef(TypedDict):
    Options: EncryptionAtRestOptionsTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## LogPublishingOptionsStatusTypeDef

```python
# LogPublishingOptionsStatusTypeDef definition

class LogPublishingOptionsStatusTypeDef(TypedDict):
    Options: NotRequired[Dict[LogTypeType, LogPublishingOptionTypeDef]],  # (1)
    Status: NotRequired[OptionStatusTypeDef],  # (2)
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) [:material-code-braces: LogPublishingOptionTypeDef](./type_defs.md#logpublishingoptiontypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## NodeToNodeEncryptionOptionsStatusTypeDef

```python
# NodeToNodeEncryptionOptionsStatusTypeDef definition

class NodeToNodeEncryptionOptionsStatusTypeDef(TypedDict):
    Options: NodeToNodeEncryptionOptionsTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: NodeToNodeEncryptionOptionsTypeDef](./type_defs.md#nodetonodeencryptionoptionstypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## SnapshotOptionsStatusTypeDef

```python
# SnapshotOptionsStatusTypeDef definition

class SnapshotOptionsStatusTypeDef(TypedDict):
    Options: SnapshotOptionsTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotOptionsTypeDef](./type_defs.md#snapshotoptionstypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## SoftwareUpdateOptionsStatusTypeDef

```python
# SoftwareUpdateOptionsStatusTypeDef definition

class SoftwareUpdateOptionsStatusTypeDef(TypedDict):
    Options: NotRequired[SoftwareUpdateOptionsTypeDef],  # (1)
    Status: NotRequired[OptionStatusTypeDef],  # (2)
```

1. See [:material-code-braces: SoftwareUpdateOptionsTypeDef](./type_defs.md#softwareupdateoptionstypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## CreateVpcEndpointRequestRequestTypeDef

```python
# CreateVpcEndpointRequestRequestTypeDef definition

class CreateVpcEndpointRequestRequestTypeDef(TypedDict):
    DomainArn: str,
    VpcOptions: VPCOptionsTypeDef,  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: VPCOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
## UpdateVpcEndpointRequestRequestTypeDef

```python
# UpdateVpcEndpointRequestRequestTypeDef definition

class UpdateVpcEndpointRequestRequestTypeDef(TypedDict):
    VpcEndpointId: str,
    VpcOptions: VPCOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: VPCOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
## CreatePackageRequestRequestTypeDef

```python
# CreatePackageRequestRequestTypeDef definition

class CreatePackageRequestRequestTypeDef(TypedDict):
    PackageName: str,
    PackageType: PackageTypeType,  # (1)
    PackageSource: PackageSourceTypeDef,  # (2)
    PackageDescription: NotRequired[str],
```

1. See [:material-code-brackets: PackageTypeType](./literals.md#packagetypetype) 
2. See [:material-code-braces: PackageSourceTypeDef](./type_defs.md#packagesourcetypedef) 
## UpdatePackageRequestRequestTypeDef

```python
# UpdatePackageRequestRequestTypeDef definition

class UpdatePackageRequestRequestTypeDef(TypedDict):
    PackageID: str,
    PackageSource: PackageSourceTypeDef,  # (1)
    PackageDescription: NotRequired[str],
    CommitMessage: NotRequired[str],
```

1. See [:material-code-braces: PackageSourceTypeDef](./type_defs.md#packagesourcetypedef) 
## DeleteVpcEndpointResponseTypeDef

```python
# DeleteVpcEndpointResponseTypeDef definition

class DeleteVpcEndpointResponseTypeDef(TypedDict):
    VpcEndpointSummary: VpcEndpointSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VpcEndpointSummaryTypeDef](./type_defs.md#vpcendpointsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVpcEndpointsForDomainResponseTypeDef

```python
# ListVpcEndpointsForDomainResponseTypeDef definition

class ListVpcEndpointsForDomainResponseTypeDef(TypedDict):
    VpcEndpointSummaryList: List[VpcEndpointSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VpcEndpointSummaryTypeDef](./type_defs.md#vpcendpointsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVpcEndpointsResponseTypeDef

```python
# ListVpcEndpointsResponseTypeDef definition

class ListVpcEndpointsResponseTypeDef(TypedDict):
    VpcEndpointSummaryList: List[VpcEndpointSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VpcEndpointSummaryTypeDef](./type_defs.md#vpcendpointsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDomainNodesResponseTypeDef

```python
# DescribeDomainNodesResponseTypeDef definition

class DescribeDomainNodesResponseTypeDef(TypedDict):
    DomainNodesStatusList: List[DomainNodesStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainNodesStatusTypeDef](./type_defs.md#domainnodesstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInboundConnectionsRequestRequestTypeDef

```python
# DescribeInboundConnectionsRequestRequestTypeDef definition

class DescribeInboundConnectionsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeOutboundConnectionsRequestRequestTypeDef

```python
# DescribeOutboundConnectionsRequestRequestTypeDef definition

class DescribeOutboundConnectionsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribePackagesRequestRequestTypeDef

```python
# DescribePackagesRequestRequestTypeDef definition

class DescribePackagesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[DescribePackagesFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribePackagesFilterTypeDef](./type_defs.md#describepackagesfiltertypedef) 
## ListDomainNamesResponseTypeDef

```python
# ListDomainNamesResponseTypeDef definition

class ListDomainNamesResponseTypeDef(TypedDict):
    DomainNames: List[DomainInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainInfoTypeDef](./type_defs.md#domaininfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainPackageDetailsTypeDef

```python
# DomainPackageDetailsTypeDef definition

class DomainPackageDetailsTypeDef(TypedDict):
    PackageID: NotRequired[str],
    PackageName: NotRequired[str],
    PackageType: NotRequired[PackageTypeType],  # (1)
    LastUpdated: NotRequired[datetime],
    DomainName: NotRequired[str],
    DomainPackageStatus: NotRequired[DomainPackageStatusType],  # (2)
    PackageVersion: NotRequired[str],
    ReferencePath: NotRequired[str],
    ErrorDetails: NotRequired[ErrorDetailsTypeDef],  # (3)
```

1. See [:material-code-brackets: PackageTypeType](./literals.md#packagetypetype) 
2. See [:material-code-brackets: DomainPackageStatusType](./literals.md#domainpackagestatustype) 
3. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## PackageDetailsTypeDef

```python
# PackageDetailsTypeDef definition

class PackageDetailsTypeDef(TypedDict):
    PackageID: NotRequired[str],
    PackageName: NotRequired[str],
    PackageType: NotRequired[PackageTypeType],  # (1)
    PackageDescription: NotRequired[str],
    PackageStatus: NotRequired[PackageStatusType],  # (2)
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    AvailablePackageVersion: NotRequired[str],
    ErrorDetails: NotRequired[ErrorDetailsTypeDef],  # (3)
```

1. See [:material-code-brackets: PackageTypeType](./literals.md#packagetypetype) 
2. See [:material-code-brackets: PackageStatusType](./literals.md#packagestatustype) 
3. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## VPCDerivedInfoStatusTypeDef

```python
# VPCDerivedInfoStatusTypeDef definition

class VPCDerivedInfoStatusTypeDef(TypedDict):
    Options: VPCDerivedInfoTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: VPCDerivedInfoTypeDef](./type_defs.md#vpcderivedinfotypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## VpcEndpointTypeDef

```python
# VpcEndpointTypeDef definition

class VpcEndpointTypeDef(TypedDict):
    VpcEndpointId: NotRequired[str],
    VpcEndpointOwner: NotRequired[str],
    DomainArn: NotRequired[str],
    VpcOptions: NotRequired[VPCDerivedInfoTypeDef],  # (1)
    Status: NotRequired[VpcEndpointStatusType],  # (2)
    Endpoint: NotRequired[str],
```

1. See [:material-code-braces: VPCDerivedInfoTypeDef](./type_defs.md#vpcderivedinfotypedef) 
2. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## DryRunProgressStatusTypeDef

```python
# DryRunProgressStatusTypeDef definition

class DryRunProgressStatusTypeDef(TypedDict):
    DryRunId: str,
    DryRunStatus: str,
    CreationDate: str,
    UpdateDate: str,
    ValidationFailures: NotRequired[List[ValidationFailureTypeDef]],  # (1)
```

1. See [:material-code-braces: ValidationFailureTypeDef](./type_defs.md#validationfailuretypedef) 
## GetPackageVersionHistoryResponseTypeDef

```python
# GetPackageVersionHistoryResponseTypeDef definition

class GetPackageVersionHistoryResponseTypeDef(TypedDict):
    PackageID: str,
    PackageVersionHistoryList: List[PackageVersionHistoryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageVersionHistoryTypeDef](./type_defs.md#packageversionhistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceLimitsTypeDef

```python
# InstanceLimitsTypeDef definition

class InstanceLimitsTypeDef(TypedDict):
    InstanceCountLimits: NotRequired[InstanceCountLimitsTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceCountLimitsTypeDef](./type_defs.md#instancecountlimitstypedef) 
## ListInstanceTypeDetailsResponseTypeDef

```python
# ListInstanceTypeDetailsResponseTypeDef definition

class ListInstanceTypeDetailsResponseTypeDef(TypedDict):
    InstanceTypeDetails: List[InstanceTypeDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDetailsTypeDef](./type_defs.md#instancetypedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListScheduledActionsResponseTypeDef

```python
# ListScheduledActionsResponseTypeDef definition

class ListScheduledActionsResponseTypeDef(TypedDict):
    ScheduledActions: List[ScheduledActionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduledActionTypeDef](./type_defs.md#scheduledactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateScheduledActionResponseTypeDef

```python
# UpdateScheduledActionResponseTypeDef definition

class UpdateScheduledActionResponseTypeDef(TypedDict):
    ScheduledAction: ScheduledActionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduledActionTypeDef](./type_defs.md#scheduledactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OffPeakWindowTypeDef

```python
# OffPeakWindowTypeDef definition

class OffPeakWindowTypeDef(TypedDict):
    WindowStartTime: NotRequired[WindowStartTimeTypeDef],  # (1)
```

1. See [:material-code-braces: WindowStartTimeTypeDef](./type_defs.md#windowstarttimetypedef) 
## ReservedInstanceOfferingTypeDef

```python
# ReservedInstanceOfferingTypeDef definition

class ReservedInstanceOfferingTypeDef(TypedDict):
    ReservedInstanceOfferingId: NotRequired[str],
    InstanceType: NotRequired[OpenSearchPartitionInstanceTypeType],  # (1)
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    UsagePrice: NotRequired[float],
    CurrencyCode: NotRequired[str],
    PaymentOption: NotRequired[ReservedInstancePaymentOptionType],  # (2)
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (3)
```

1. See [:material-code-brackets: OpenSearchPartitionInstanceTypeType](./literals.md#opensearchpartitioninstancetypetype) 
2. See [:material-code-brackets: ReservedInstancePaymentOptionType](./literals.md#reservedinstancepaymentoptiontype) 
3. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
## ReservedInstanceTypeDef

```python
# ReservedInstanceTypeDef definition

class ReservedInstanceTypeDef(TypedDict):
    ReservationName: NotRequired[str],
    ReservedInstanceId: NotRequired[str],
    BillingSubscriptionId: NotRequired[int],
    ReservedInstanceOfferingId: NotRequired[str],
    InstanceType: NotRequired[OpenSearchPartitionInstanceTypeType],  # (1)
    StartTime: NotRequired[datetime],
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    UsagePrice: NotRequired[float],
    CurrencyCode: NotRequired[str],
    InstanceCount: NotRequired[int],
    State: NotRequired[str],
    PaymentOption: NotRequired[ReservedInstancePaymentOptionType],  # (2)
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (3)
```

1. See [:material-code-brackets: OpenSearchPartitionInstanceTypeType](./literals.md#opensearchpartitioninstancetypetype) 
2. See [:material-code-brackets: ReservedInstancePaymentOptionType](./literals.md#reservedinstancepaymentoptiontype) 
3. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
## SAMLOptionsInputTypeDef

```python
# SAMLOptionsInputTypeDef definition

class SAMLOptionsInputTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    Idp: NotRequired[SAMLIdpTypeDef],  # (1)
    MasterUserName: NotRequired[str],
    MasterBackendRole: NotRequired[str],
    SubjectKey: NotRequired[str],
    RolesKey: NotRequired[str],
    SessionTimeoutMinutes: NotRequired[int],
```

1. See [:material-code-braces: SAMLIdpTypeDef](./type_defs.md#samlidptypedef) 
## SAMLOptionsOutputTypeDef

```python
# SAMLOptionsOutputTypeDef definition

class SAMLOptionsOutputTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    Idp: NotRequired[SAMLIdpTypeDef],  # (1)
    SubjectKey: NotRequired[str],
    RolesKey: NotRequired[str],
    SessionTimeoutMinutes: NotRequired[int],
```

1. See [:material-code-braces: SAMLIdpTypeDef](./type_defs.md#samlidptypedef) 
## StorageTypeTypeDef

```python
# StorageTypeTypeDef definition

class StorageTypeTypeDef(TypedDict):
    StorageTypeName: NotRequired[str],
    StorageSubTypeName: NotRequired[str],
    StorageTypeLimits: NotRequired[List[StorageTypeLimitTypeDef]],  # (1)
```

1. See [:material-code-braces: StorageTypeLimitTypeDef](./type_defs.md#storagetypelimittypedef) 
## UpgradeHistoryTypeDef

```python
# UpgradeHistoryTypeDef definition

class UpgradeHistoryTypeDef(TypedDict):
    UpgradeName: NotRequired[str],
    StartTimestamp: NotRequired[datetime],
    UpgradeStatus: NotRequired[UpgradeStatusType],  # (1)
    StepsList: NotRequired[List[UpgradeStepItemTypeDef]],  # (2)
```

1. See [:material-code-brackets: UpgradeStatusType](./literals.md#upgradestatustype) 
2. See [:material-code-braces: UpgradeStepItemTypeDef](./type_defs.md#upgradestepitemtypedef) 
## InboundConnectionTypeDef

```python
# InboundConnectionTypeDef definition

class InboundConnectionTypeDef(TypedDict):
    LocalDomainInfo: NotRequired[DomainInformationContainerTypeDef],  # (1)
    RemoteDomainInfo: NotRequired[DomainInformationContainerTypeDef],  # (1)
    ConnectionId: NotRequired[str],
    ConnectionStatus: NotRequired[InboundConnectionStatusTypeDef],  # (3)
    ConnectionMode: NotRequired[ConnectionModeType],  # (4)
```

1. See [:material-code-braces: DomainInformationContainerTypeDef](./type_defs.md#domaininformationcontainertypedef) 
2. See [:material-code-braces: DomainInformationContainerTypeDef](./type_defs.md#domaininformationcontainertypedef) 
3. See [:material-code-braces: InboundConnectionStatusTypeDef](./type_defs.md#inboundconnectionstatustypedef) 
4. See [:material-code-brackets: ConnectionModeType](./literals.md#connectionmodetype) 
## AutoTuneTypeDef

```python
# AutoTuneTypeDef definition

class AutoTuneTypeDef(TypedDict):
    AutoTuneType: NotRequired[AutoTuneTypeType],  # (1)
    AutoTuneDetails: NotRequired[AutoTuneDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: AutoTuneTypeType](./literals.md#autotunetypetype) 
2. See [:material-code-braces: AutoTuneDetailsTypeDef](./type_defs.md#autotunedetailstypedef) 
## AutoTuneOptionsInputTypeDef

```python
# AutoTuneOptionsInputTypeDef definition

class AutoTuneOptionsInputTypeDef(TypedDict):
    DesiredState: NotRequired[AutoTuneDesiredStateType],  # (1)
    MaintenanceSchedules: NotRequired[Sequence[AutoTuneMaintenanceScheduleTypeDef]],  # (2)
    UseOffPeakWindow: NotRequired[bool],
```

1. See [:material-code-brackets: AutoTuneDesiredStateType](./literals.md#autotunedesiredstatetype) 
2. See [:material-code-braces: AutoTuneMaintenanceScheduleTypeDef](./type_defs.md#autotunemaintenancescheduletypedef) 
## AutoTuneOptionsTypeDef

```python
# AutoTuneOptionsTypeDef definition

class AutoTuneOptionsTypeDef(TypedDict):
    DesiredState: NotRequired[AutoTuneDesiredStateType],  # (1)
    RollbackOnDisable: NotRequired[RollbackOnDisableType],  # (2)
    MaintenanceSchedules: NotRequired[List[AutoTuneMaintenanceScheduleTypeDef]],  # (3)
    UseOffPeakWindow: NotRequired[bool],
```

1. See [:material-code-brackets: AutoTuneDesiredStateType](./literals.md#autotunedesiredstatetype) 
2. See [:material-code-brackets: RollbackOnDisableType](./literals.md#rollbackondisabletype) 
3. See [:material-code-braces: AutoTuneMaintenanceScheduleTypeDef](./type_defs.md#autotunemaintenancescheduletypedef) 
## DescribeDomainHealthResponseTypeDef

```python
# DescribeDomainHealthResponseTypeDef definition

class DescribeDomainHealthResponseTypeDef(TypedDict):
    DomainState: DomainStateType,  # (1)
    AvailabilityZoneCount: str,
    ActiveAvailabilityZoneCount: str,
    StandByAvailabilityZoneCount: str,
    DataNodeCount: str,
    DedicatedMaster: bool,
    MasterEligibleNodeCount: str,
    WarmNodeCount: str,
    MasterNode: MasterNodeStatusType,  # (2)
    ClusterHealth: DomainHealthType,  # (3)
    TotalShards: str,
    TotalUnAssignedShards: str,
    EnvironmentInformation: List[EnvironmentInfoTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: DomainStateType](./literals.md#domainstatetype) 
2. See [:material-code-brackets: MasterNodeStatusType](./literals.md#masternodestatustype) 
3. See [:material-code-brackets: DomainHealthType](./literals.md#domainhealthtype) 
4. See [:material-code-braces: EnvironmentInfoTypeDef](./type_defs.md#environmentinfotypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDomainChangeProgressResponseTypeDef

```python
# DescribeDomainChangeProgressResponseTypeDef definition

class DescribeDomainChangeProgressResponseTypeDef(TypedDict):
    ChangeProgressStatus: ChangeProgressStatusDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeProgressStatusDetailsTypeDef](./type_defs.md#changeprogressstatusdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClusterConfigStatusTypeDef

```python
# ClusterConfigStatusTypeDef definition

class ClusterConfigStatusTypeDef(TypedDict):
    Options: ClusterConfigTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterConfigTypeDef](./type_defs.md#clusterconfigtypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## CreateOutboundConnectionRequestRequestTypeDef

```python
# CreateOutboundConnectionRequestRequestTypeDef definition

class CreateOutboundConnectionRequestRequestTypeDef(TypedDict):
    LocalDomainInfo: DomainInformationContainerTypeDef,  # (1)
    RemoteDomainInfo: DomainInformationContainerTypeDef,  # (1)
    ConnectionAlias: str,
    ConnectionMode: NotRequired[ConnectionModeType],  # (3)
    ConnectionProperties: NotRequired[ConnectionPropertiesTypeDef],  # (4)
```

1. See [:material-code-braces: DomainInformationContainerTypeDef](./type_defs.md#domaininformationcontainertypedef) 
2. See [:material-code-braces: DomainInformationContainerTypeDef](./type_defs.md#domaininformationcontainertypedef) 
3. See [:material-code-brackets: ConnectionModeType](./literals.md#connectionmodetype) 
4. See [:material-code-braces: ConnectionPropertiesTypeDef](./type_defs.md#connectionpropertiestypedef) 
## CreateOutboundConnectionResponseTypeDef

```python
# CreateOutboundConnectionResponseTypeDef definition

class CreateOutboundConnectionResponseTypeDef(TypedDict):
    LocalDomainInfo: DomainInformationContainerTypeDef,  # (1)
    RemoteDomainInfo: DomainInformationContainerTypeDef,  # (1)
    ConnectionAlias: str,
    ConnectionStatus: OutboundConnectionStatusTypeDef,  # (3)
    ConnectionId: str,
    ConnectionMode: ConnectionModeType,  # (4)
    ConnectionProperties: ConnectionPropertiesTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: DomainInformationContainerTypeDef](./type_defs.md#domaininformationcontainertypedef) 
2. See [:material-code-braces: DomainInformationContainerTypeDef](./type_defs.md#domaininformationcontainertypedef) 
3. See [:material-code-braces: OutboundConnectionStatusTypeDef](./type_defs.md#outboundconnectionstatustypedef) 
4. See [:material-code-brackets: ConnectionModeType](./literals.md#connectionmodetype) 
5. See [:material-code-braces: ConnectionPropertiesTypeDef](./type_defs.md#connectionpropertiestypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OutboundConnectionTypeDef

```python
# OutboundConnectionTypeDef definition

class OutboundConnectionTypeDef(TypedDict):
    LocalDomainInfo: NotRequired[DomainInformationContainerTypeDef],  # (1)
    RemoteDomainInfo: NotRequired[DomainInformationContainerTypeDef],  # (1)
    ConnectionId: NotRequired[str],
    ConnectionAlias: NotRequired[str],
    ConnectionStatus: NotRequired[OutboundConnectionStatusTypeDef],  # (3)
    ConnectionMode: NotRequired[ConnectionModeType],  # (4)
    ConnectionProperties: NotRequired[ConnectionPropertiesTypeDef],  # (5)
```

1. See [:material-code-braces: DomainInformationContainerTypeDef](./type_defs.md#domaininformationcontainertypedef) 
2. See [:material-code-braces: DomainInformationContainerTypeDef](./type_defs.md#domaininformationcontainertypedef) 
3. See [:material-code-braces: OutboundConnectionStatusTypeDef](./type_defs.md#outboundconnectionstatustypedef) 
4. See [:material-code-brackets: ConnectionModeType](./literals.md#connectionmodetype) 
5. See [:material-code-braces: ConnectionPropertiesTypeDef](./type_defs.md#connectionpropertiestypedef) 
## AssociatePackageResponseTypeDef

```python
# AssociatePackageResponseTypeDef definition

class AssociatePackageResponseTypeDef(TypedDict):
    DomainPackageDetails: DomainPackageDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainPackageDetailsTypeDef](./type_defs.md#domainpackagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DissociatePackageResponseTypeDef

```python
# DissociatePackageResponseTypeDef definition

class DissociatePackageResponseTypeDef(TypedDict):
    DomainPackageDetails: DomainPackageDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainPackageDetailsTypeDef](./type_defs.md#domainpackagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainsForPackageResponseTypeDef

```python
# ListDomainsForPackageResponseTypeDef definition

class ListDomainsForPackageResponseTypeDef(TypedDict):
    DomainPackageDetailsList: List[DomainPackageDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainPackageDetailsTypeDef](./type_defs.md#domainpackagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPackagesForDomainResponseTypeDef

```python
# ListPackagesForDomainResponseTypeDef definition

class ListPackagesForDomainResponseTypeDef(TypedDict):
    DomainPackageDetailsList: List[DomainPackageDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainPackageDetailsTypeDef](./type_defs.md#domainpackagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePackageResponseTypeDef

```python
# CreatePackageResponseTypeDef definition

class CreatePackageResponseTypeDef(TypedDict):
    PackageDetails: PackageDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageDetailsTypeDef](./type_defs.md#packagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePackageResponseTypeDef

```python
# DeletePackageResponseTypeDef definition

class DeletePackageResponseTypeDef(TypedDict):
    PackageDetails: PackageDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageDetailsTypeDef](./type_defs.md#packagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePackagesResponseTypeDef

```python
# DescribePackagesResponseTypeDef definition

class DescribePackagesResponseTypeDef(TypedDict):
    PackageDetailsList: List[PackageDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageDetailsTypeDef](./type_defs.md#packagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePackageResponseTypeDef

```python
# UpdatePackageResponseTypeDef definition

class UpdatePackageResponseTypeDef(TypedDict):
    PackageDetails: PackageDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageDetailsTypeDef](./type_defs.md#packagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVpcEndpointResponseTypeDef

```python
# CreateVpcEndpointResponseTypeDef definition

class CreateVpcEndpointResponseTypeDef(TypedDict):
    VpcEndpoint: VpcEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVpcEndpointsResponseTypeDef

```python
# DescribeVpcEndpointsResponseTypeDef definition

class DescribeVpcEndpointsResponseTypeDef(TypedDict):
    VpcEndpoints: List[VpcEndpointTypeDef],  # (1)
    VpcEndpointErrors: List[VpcEndpointErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef) 
2. See [:material-code-braces: VpcEndpointErrorTypeDef](./type_defs.md#vpcendpointerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVpcEndpointResponseTypeDef

```python
# UpdateVpcEndpointResponseTypeDef definition

class UpdateVpcEndpointResponseTypeDef(TypedDict):
    VpcEndpoint: VpcEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OffPeakWindowOptionsTypeDef

```python
# OffPeakWindowOptionsTypeDef definition

class OffPeakWindowOptionsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    OffPeakWindow: NotRequired[OffPeakWindowTypeDef],  # (1)
```

1. See [:material-code-braces: OffPeakWindowTypeDef](./type_defs.md#offpeakwindowtypedef) 
## DescribeReservedInstanceOfferingsResponseTypeDef

```python
# DescribeReservedInstanceOfferingsResponseTypeDef definition

class DescribeReservedInstanceOfferingsResponseTypeDef(TypedDict):
    NextToken: str,
    ReservedInstanceOfferings: List[ReservedInstanceOfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedInstanceOfferingTypeDef](./type_defs.md#reservedinstanceofferingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReservedInstancesResponseTypeDef

```python
# DescribeReservedInstancesResponseTypeDef definition

class DescribeReservedInstancesResponseTypeDef(TypedDict):
    NextToken: str,
    ReservedInstances: List[ReservedInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReservedInstanceTypeDef](./type_defs.md#reservedinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AdvancedSecurityOptionsInputTypeDef

```python
# AdvancedSecurityOptionsInputTypeDef definition

class AdvancedSecurityOptionsInputTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    InternalUserDatabaseEnabled: NotRequired[bool],
    MasterUserOptions: NotRequired[MasterUserOptionsTypeDef],  # (1)
    SAMLOptions: NotRequired[SAMLOptionsInputTypeDef],  # (2)
    AnonymousAuthEnabled: NotRequired[bool],
```

1. See [:material-code-braces: MasterUserOptionsTypeDef](./type_defs.md#masteruseroptionstypedef) 
2. See [:material-code-braces: SAMLOptionsInputTypeDef](./type_defs.md#samloptionsinputtypedef) 
## AdvancedSecurityOptionsTypeDef

```python
# AdvancedSecurityOptionsTypeDef definition

class AdvancedSecurityOptionsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    InternalUserDatabaseEnabled: NotRequired[bool],
    SAMLOptions: NotRequired[SAMLOptionsOutputTypeDef],  # (1)
    AnonymousAuthDisableDate: NotRequired[datetime],
    AnonymousAuthEnabled: NotRequired[bool],
```

1. See [:material-code-braces: SAMLOptionsOutputTypeDef](./type_defs.md#samloptionsoutputtypedef) 
## LimitsTypeDef

```python
# LimitsTypeDef definition

class LimitsTypeDef(TypedDict):
    StorageTypes: NotRequired[List[StorageTypeTypeDef]],  # (1)
    InstanceLimits: NotRequired[InstanceLimitsTypeDef],  # (2)
    AdditionalLimits: NotRequired[List[AdditionalLimitTypeDef]],  # (3)
```

1. See [:material-code-braces: StorageTypeTypeDef](./type_defs.md#storagetypetypedef) 
2. See [:material-code-braces: InstanceLimitsTypeDef](./type_defs.md#instancelimitstypedef) 
3. See [:material-code-braces: AdditionalLimitTypeDef](./type_defs.md#additionallimittypedef) 
## GetUpgradeHistoryResponseTypeDef

```python
# GetUpgradeHistoryResponseTypeDef definition

class GetUpgradeHistoryResponseTypeDef(TypedDict):
    UpgradeHistories: List[UpgradeHistoryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpgradeHistoryTypeDef](./type_defs.md#upgradehistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AcceptInboundConnectionResponseTypeDef

```python
# AcceptInboundConnectionResponseTypeDef definition

class AcceptInboundConnectionResponseTypeDef(TypedDict):
    Connection: InboundConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InboundConnectionTypeDef](./type_defs.md#inboundconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInboundConnectionResponseTypeDef

```python
# DeleteInboundConnectionResponseTypeDef definition

class DeleteInboundConnectionResponseTypeDef(TypedDict):
    Connection: InboundConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InboundConnectionTypeDef](./type_defs.md#inboundconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInboundConnectionsResponseTypeDef

```python
# DescribeInboundConnectionsResponseTypeDef definition

class DescribeInboundConnectionsResponseTypeDef(TypedDict):
    Connections: List[InboundConnectionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InboundConnectionTypeDef](./type_defs.md#inboundconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RejectInboundConnectionResponseTypeDef

```python
# RejectInboundConnectionResponseTypeDef definition

class RejectInboundConnectionResponseTypeDef(TypedDict):
    Connection: InboundConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InboundConnectionTypeDef](./type_defs.md#inboundconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDomainAutoTunesResponseTypeDef

```python
# DescribeDomainAutoTunesResponseTypeDef definition

class DescribeDomainAutoTunesResponseTypeDef(TypedDict):
    AutoTunes: List[AutoTuneTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoTuneTypeDef](./type_defs.md#autotunetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoTuneOptionsStatusTypeDef

```python
# AutoTuneOptionsStatusTypeDef definition

class AutoTuneOptionsStatusTypeDef(TypedDict):
    Options: NotRequired[AutoTuneOptionsTypeDef],  # (1)
    Status: NotRequired[AutoTuneStatusTypeDef],  # (2)
```

1. See [:material-code-braces: AutoTuneOptionsTypeDef](./type_defs.md#autotuneoptionstypedef) 
2. See [:material-code-braces: AutoTuneStatusTypeDef](./type_defs.md#autotunestatustypedef) 
## DeleteOutboundConnectionResponseTypeDef

```python
# DeleteOutboundConnectionResponseTypeDef definition

class DeleteOutboundConnectionResponseTypeDef(TypedDict):
    Connection: OutboundConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutboundConnectionTypeDef](./type_defs.md#outboundconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOutboundConnectionsResponseTypeDef

```python
# DescribeOutboundConnectionsResponseTypeDef definition

class DescribeOutboundConnectionsResponseTypeDef(TypedDict):
    Connections: List[OutboundConnectionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutboundConnectionTypeDef](./type_defs.md#outboundconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OffPeakWindowOptionsStatusTypeDef

```python
# OffPeakWindowOptionsStatusTypeDef definition

class OffPeakWindowOptionsStatusTypeDef(TypedDict):
    Options: NotRequired[OffPeakWindowOptionsTypeDef],  # (1)
    Status: NotRequired[OptionStatusTypeDef],  # (2)
```

1. See [:material-code-braces: OffPeakWindowOptionsTypeDef](./type_defs.md#offpeakwindowoptionstypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## CreateDomainRequestRequestTypeDef

```python
# CreateDomainRequestRequestTypeDef definition

class CreateDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    EngineVersion: NotRequired[str],
    ClusterConfig: NotRequired[ClusterConfigTypeDef],  # (1)
    EBSOptions: NotRequired[EBSOptionsTypeDef],  # (2)
    AccessPolicies: NotRequired[str],
    SnapshotOptions: NotRequired[SnapshotOptionsTypeDef],  # (3)
    VPCOptions: NotRequired[VPCOptionsTypeDef],  # (4)
    CognitoOptions: NotRequired[CognitoOptionsTypeDef],  # (5)
    EncryptionAtRestOptions: NotRequired[EncryptionAtRestOptionsTypeDef],  # (6)
    NodeToNodeEncryptionOptions: NotRequired[NodeToNodeEncryptionOptionsTypeDef],  # (7)
    AdvancedOptions: NotRequired[Mapping[str, str]],
    LogPublishingOptions: NotRequired[Mapping[LogTypeType, LogPublishingOptionTypeDef]],  # (8)
    DomainEndpointOptions: NotRequired[DomainEndpointOptionsTypeDef],  # (9)
    AdvancedSecurityOptions: NotRequired[AdvancedSecurityOptionsInputTypeDef],  # (10)
    TagList: NotRequired[Sequence[TagTypeDef]],  # (11)
    AutoTuneOptions: NotRequired[AutoTuneOptionsInputTypeDef],  # (12)
    OffPeakWindowOptions: NotRequired[OffPeakWindowOptionsTypeDef],  # (13)
    SoftwareUpdateOptions: NotRequired[SoftwareUpdateOptionsTypeDef],  # (14)
```

1. See [:material-code-braces: ClusterConfigTypeDef](./type_defs.md#clusterconfigtypedef) 
2. See [:material-code-braces: EBSOptionsTypeDef](./type_defs.md#ebsoptionstypedef) 
3. See [:material-code-braces: SnapshotOptionsTypeDef](./type_defs.md#snapshotoptionstypedef) 
4. See [:material-code-braces: VPCOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
5. See [:material-code-braces: CognitoOptionsTypeDef](./type_defs.md#cognitooptionstypedef) 
6. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef) 
7. See [:material-code-braces: NodeToNodeEncryptionOptionsTypeDef](./type_defs.md#nodetonodeencryptionoptionstypedef) 
8. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) [:material-code-braces: LogPublishingOptionTypeDef](./type_defs.md#logpublishingoptiontypedef) 
9. See [:material-code-braces: DomainEndpointOptionsTypeDef](./type_defs.md#domainendpointoptionstypedef) 
10. See [:material-code-braces: AdvancedSecurityOptionsInputTypeDef](./type_defs.md#advancedsecurityoptionsinputtypedef) 
11. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
12. See [:material-code-braces: AutoTuneOptionsInputTypeDef](./type_defs.md#autotuneoptionsinputtypedef) 
13. See [:material-code-braces: OffPeakWindowOptionsTypeDef](./type_defs.md#offpeakwindowoptionstypedef) 
14. See [:material-code-braces: SoftwareUpdateOptionsTypeDef](./type_defs.md#softwareupdateoptionstypedef) 
## UpdateDomainConfigRequestRequestTypeDef

```python
# UpdateDomainConfigRequestRequestTypeDef definition

class UpdateDomainConfigRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ClusterConfig: NotRequired[ClusterConfigTypeDef],  # (1)
    EBSOptions: NotRequired[EBSOptionsTypeDef],  # (2)
    SnapshotOptions: NotRequired[SnapshotOptionsTypeDef],  # (3)
    VPCOptions: NotRequired[VPCOptionsTypeDef],  # (4)
    CognitoOptions: NotRequired[CognitoOptionsTypeDef],  # (5)
    AdvancedOptions: NotRequired[Mapping[str, str]],
    AccessPolicies: NotRequired[str],
    LogPublishingOptions: NotRequired[Mapping[LogTypeType, LogPublishingOptionTypeDef]],  # (6)
    EncryptionAtRestOptions: NotRequired[EncryptionAtRestOptionsTypeDef],  # (7)
    DomainEndpointOptions: NotRequired[DomainEndpointOptionsTypeDef],  # (8)
    NodeToNodeEncryptionOptions: NotRequired[NodeToNodeEncryptionOptionsTypeDef],  # (9)
    AdvancedSecurityOptions: NotRequired[AdvancedSecurityOptionsInputTypeDef],  # (10)
    AutoTuneOptions: NotRequired[AutoTuneOptionsTypeDef],  # (11)
    DryRun: NotRequired[bool],
    DryRunMode: NotRequired[DryRunModeType],  # (12)
    OffPeakWindowOptions: NotRequired[OffPeakWindowOptionsTypeDef],  # (13)
    SoftwareUpdateOptions: NotRequired[SoftwareUpdateOptionsTypeDef],  # (14)
```

1. See [:material-code-braces: ClusterConfigTypeDef](./type_defs.md#clusterconfigtypedef) 
2. See [:material-code-braces: EBSOptionsTypeDef](./type_defs.md#ebsoptionstypedef) 
3. See [:material-code-braces: SnapshotOptionsTypeDef](./type_defs.md#snapshotoptionstypedef) 
4. See [:material-code-braces: VPCOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
5. See [:material-code-braces: CognitoOptionsTypeDef](./type_defs.md#cognitooptionstypedef) 
6. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) [:material-code-braces: LogPublishingOptionTypeDef](./type_defs.md#logpublishingoptiontypedef) 
7. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef) 
8. See [:material-code-braces: DomainEndpointOptionsTypeDef](./type_defs.md#domainendpointoptionstypedef) 
9. See [:material-code-braces: NodeToNodeEncryptionOptionsTypeDef](./type_defs.md#nodetonodeencryptionoptionstypedef) 
10. See [:material-code-braces: AdvancedSecurityOptionsInputTypeDef](./type_defs.md#advancedsecurityoptionsinputtypedef) 
11. See [:material-code-braces: AutoTuneOptionsTypeDef](./type_defs.md#autotuneoptionstypedef) 
12. See [:material-code-brackets: DryRunModeType](./literals.md#dryrunmodetype) 
13. See [:material-code-braces: OffPeakWindowOptionsTypeDef](./type_defs.md#offpeakwindowoptionstypedef) 
14. See [:material-code-braces: SoftwareUpdateOptionsTypeDef](./type_defs.md#softwareupdateoptionstypedef) 
## AdvancedSecurityOptionsStatusTypeDef

```python
# AdvancedSecurityOptionsStatusTypeDef definition

class AdvancedSecurityOptionsStatusTypeDef(TypedDict):
    Options: AdvancedSecurityOptionsTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: AdvancedSecurityOptionsTypeDef](./type_defs.md#advancedsecurityoptionstypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## DomainStatusTypeDef

```python
# DomainStatusTypeDef definition

class DomainStatusTypeDef(TypedDict):
    DomainId: str,
    DomainName: str,
    ARN: str,
    ClusterConfig: ClusterConfigTypeDef,  # (1)
    Created: NotRequired[bool],
    Deleted: NotRequired[bool],
    Endpoint: NotRequired[str],
    Endpoints: NotRequired[Dict[str, str]],
    Processing: NotRequired[bool],
    UpgradeProcessing: NotRequired[bool],
    EngineVersion: NotRequired[str],
    EBSOptions: NotRequired[EBSOptionsTypeDef],  # (2)
    AccessPolicies: NotRequired[str],
    SnapshotOptions: NotRequired[SnapshotOptionsTypeDef],  # (3)
    VPCOptions: NotRequired[VPCDerivedInfoTypeDef],  # (4)
    CognitoOptions: NotRequired[CognitoOptionsTypeDef],  # (5)
    EncryptionAtRestOptions: NotRequired[EncryptionAtRestOptionsTypeDef],  # (6)
    NodeToNodeEncryptionOptions: NotRequired[NodeToNodeEncryptionOptionsTypeDef],  # (7)
    AdvancedOptions: NotRequired[Dict[str, str]],
    LogPublishingOptions: NotRequired[Dict[LogTypeType, LogPublishingOptionTypeDef]],  # (8)
    ServiceSoftwareOptions: NotRequired[ServiceSoftwareOptionsTypeDef],  # (9)
    DomainEndpointOptions: NotRequired[DomainEndpointOptionsTypeDef],  # (10)
    AdvancedSecurityOptions: NotRequired[AdvancedSecurityOptionsTypeDef],  # (11)
    AutoTuneOptions: NotRequired[AutoTuneOptionsOutputTypeDef],  # (12)
    ChangeProgressDetails: NotRequired[ChangeProgressDetailsTypeDef],  # (13)
    OffPeakWindowOptions: NotRequired[OffPeakWindowOptionsTypeDef],  # (14)
    SoftwareUpdateOptions: NotRequired[SoftwareUpdateOptionsTypeDef],  # (15)
```

1. See [:material-code-braces: ClusterConfigTypeDef](./type_defs.md#clusterconfigtypedef) 
2. See [:material-code-braces: EBSOptionsTypeDef](./type_defs.md#ebsoptionstypedef) 
3. See [:material-code-braces: SnapshotOptionsTypeDef](./type_defs.md#snapshotoptionstypedef) 
4. See [:material-code-braces: VPCDerivedInfoTypeDef](./type_defs.md#vpcderivedinfotypedef) 
5. See [:material-code-braces: CognitoOptionsTypeDef](./type_defs.md#cognitooptionstypedef) 
6. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef) 
7. See [:material-code-braces: NodeToNodeEncryptionOptionsTypeDef](./type_defs.md#nodetonodeencryptionoptionstypedef) 
8. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) [:material-code-braces: LogPublishingOptionTypeDef](./type_defs.md#logpublishingoptiontypedef) 
9. See [:material-code-braces: ServiceSoftwareOptionsTypeDef](./type_defs.md#servicesoftwareoptionstypedef) 
10. See [:material-code-braces: DomainEndpointOptionsTypeDef](./type_defs.md#domainendpointoptionstypedef) 
11. See [:material-code-braces: AdvancedSecurityOptionsTypeDef](./type_defs.md#advancedsecurityoptionstypedef) 
12. See [:material-code-braces: AutoTuneOptionsOutputTypeDef](./type_defs.md#autotuneoptionsoutputtypedef) 
13. See [:material-code-braces: ChangeProgressDetailsTypeDef](./type_defs.md#changeprogressdetailstypedef) 
14. See [:material-code-braces: OffPeakWindowOptionsTypeDef](./type_defs.md#offpeakwindowoptionstypedef) 
15. See [:material-code-braces: SoftwareUpdateOptionsTypeDef](./type_defs.md#softwareupdateoptionstypedef) 
## DescribeInstanceTypeLimitsResponseTypeDef

```python
# DescribeInstanceTypeLimitsResponseTypeDef definition

class DescribeInstanceTypeLimitsResponseTypeDef(TypedDict):
    LimitsByRole: Dict[str, LimitsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LimitsTypeDef](./type_defs.md#limitstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainConfigTypeDef

```python
# DomainConfigTypeDef definition

class DomainConfigTypeDef(TypedDict):
    EngineVersion: NotRequired[VersionStatusTypeDef],  # (1)
    ClusterConfig: NotRequired[ClusterConfigStatusTypeDef],  # (2)
    EBSOptions: NotRequired[EBSOptionsStatusTypeDef],  # (3)
    AccessPolicies: NotRequired[AccessPoliciesStatusTypeDef],  # (4)
    SnapshotOptions: NotRequired[SnapshotOptionsStatusTypeDef],  # (5)
    VPCOptions: NotRequired[VPCDerivedInfoStatusTypeDef],  # (6)
    CognitoOptions: NotRequired[CognitoOptionsStatusTypeDef],  # (7)
    EncryptionAtRestOptions: NotRequired[EncryptionAtRestOptionsStatusTypeDef],  # (8)
    NodeToNodeEncryptionOptions: NotRequired[NodeToNodeEncryptionOptionsStatusTypeDef],  # (9)
    AdvancedOptions: NotRequired[AdvancedOptionsStatusTypeDef],  # (10)
    LogPublishingOptions: NotRequired[LogPublishingOptionsStatusTypeDef],  # (11)
    DomainEndpointOptions: NotRequired[DomainEndpointOptionsStatusTypeDef],  # (12)
    AdvancedSecurityOptions: NotRequired[AdvancedSecurityOptionsStatusTypeDef],  # (13)
    AutoTuneOptions: NotRequired[AutoTuneOptionsStatusTypeDef],  # (14)
    ChangeProgressDetails: NotRequired[ChangeProgressDetailsTypeDef],  # (15)
    OffPeakWindowOptions: NotRequired[OffPeakWindowOptionsStatusTypeDef],  # (16)
    SoftwareUpdateOptions: NotRequired[SoftwareUpdateOptionsStatusTypeDef],  # (17)
```

1. See [:material-code-braces: VersionStatusTypeDef](./type_defs.md#versionstatustypedef) 
2. See [:material-code-braces: ClusterConfigStatusTypeDef](./type_defs.md#clusterconfigstatustypedef) 
3. See [:material-code-braces: EBSOptionsStatusTypeDef](./type_defs.md#ebsoptionsstatustypedef) 
4. See [:material-code-braces: AccessPoliciesStatusTypeDef](./type_defs.md#accesspoliciesstatustypedef) 
5. See [:material-code-braces: SnapshotOptionsStatusTypeDef](./type_defs.md#snapshotoptionsstatustypedef) 
6. See [:material-code-braces: VPCDerivedInfoStatusTypeDef](./type_defs.md#vpcderivedinfostatustypedef) 
7. See [:material-code-braces: CognitoOptionsStatusTypeDef](./type_defs.md#cognitooptionsstatustypedef) 
8. See [:material-code-braces: EncryptionAtRestOptionsStatusTypeDef](./type_defs.md#encryptionatrestoptionsstatustypedef) 
9. See [:material-code-braces: NodeToNodeEncryptionOptionsStatusTypeDef](./type_defs.md#nodetonodeencryptionoptionsstatustypedef) 
10. See [:material-code-braces: AdvancedOptionsStatusTypeDef](./type_defs.md#advancedoptionsstatustypedef) 
11. See [:material-code-braces: LogPublishingOptionsStatusTypeDef](./type_defs.md#logpublishingoptionsstatustypedef) 
12. See [:material-code-braces: DomainEndpointOptionsStatusTypeDef](./type_defs.md#domainendpointoptionsstatustypedef) 
13. See [:material-code-braces: AdvancedSecurityOptionsStatusTypeDef](./type_defs.md#advancedsecurityoptionsstatustypedef) 
14. See [:material-code-braces: AutoTuneOptionsStatusTypeDef](./type_defs.md#autotuneoptionsstatustypedef) 
15. See [:material-code-braces: ChangeProgressDetailsTypeDef](./type_defs.md#changeprogressdetailstypedef) 
16. See [:material-code-braces: OffPeakWindowOptionsStatusTypeDef](./type_defs.md#offpeakwindowoptionsstatustypedef) 
17. See [:material-code-braces: SoftwareUpdateOptionsStatusTypeDef](./type_defs.md#softwareupdateoptionsstatustypedef) 
## CreateDomainResponseTypeDef

```python
# CreateDomainResponseTypeDef definition

class CreateDomainResponseTypeDef(TypedDict):
    DomainStatus: DomainStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainStatusTypeDef](./type_defs.md#domainstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDomainResponseTypeDef

```python
# DeleteDomainResponseTypeDef definition

class DeleteDomainResponseTypeDef(TypedDict):
    DomainStatus: DomainStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainStatusTypeDef](./type_defs.md#domainstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDomainResponseTypeDef

```python
# DescribeDomainResponseTypeDef definition

class DescribeDomainResponseTypeDef(TypedDict):
    DomainStatus: DomainStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainStatusTypeDef](./type_defs.md#domainstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDomainsResponseTypeDef

```python
# DescribeDomainsResponseTypeDef definition

class DescribeDomainsResponseTypeDef(TypedDict):
    DomainStatusList: List[DomainStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainStatusTypeDef](./type_defs.md#domainstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDryRunProgressResponseTypeDef

```python
# DescribeDryRunProgressResponseTypeDef definition

class DescribeDryRunProgressResponseTypeDef(TypedDict):
    DryRunProgressStatus: DryRunProgressStatusTypeDef,  # (1)
    DryRunConfig: DomainStatusTypeDef,  # (2)
    DryRunResults: DryRunResultsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DryRunProgressStatusTypeDef](./type_defs.md#dryrunprogressstatustypedef) 
2. See [:material-code-braces: DomainStatusTypeDef](./type_defs.md#domainstatustypedef) 
3. See [:material-code-braces: DryRunResultsTypeDef](./type_defs.md#dryrunresultstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDomainConfigResponseTypeDef

```python
# DescribeDomainConfigResponseTypeDef definition

class DescribeDomainConfigResponseTypeDef(TypedDict):
    DomainConfig: DomainConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainConfigTypeDef](./type_defs.md#domainconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainConfigResponseTypeDef

```python
# UpdateDomainConfigResponseTypeDef definition

class UpdateDomainConfigResponseTypeDef(TypedDict):
    DomainConfig: DomainConfigTypeDef,  # (1)
    DryRunResults: DryRunResultsTypeDef,  # (2)
    DryRunProgressStatus: DryRunProgressStatusTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DomainConfigTypeDef](./type_defs.md#domainconfigtypedef) 
2. See [:material-code-braces: DryRunResultsTypeDef](./type_defs.md#dryrunresultstypedef) 
3. See [:material-code-braces: DryRunProgressStatusTypeDef](./type_defs.md#dryrunprogressstatustypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
