# Type definitions

> [Index](../README.md) > [ElasticsearchService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ElasticsearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
    type annotations stubs module [types-aiobotocore-es](https://pypi.org/project/types-aiobotocore-es/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AutoTuneMaintenanceScheduleUnionTypeDef

```python
# AutoTuneMaintenanceScheduleUnionTypeDef definition

AutoTuneMaintenanceScheduleUnionTypeDef = Union[
    AutoTuneMaintenanceScheduleTypeDef,  # (1)
    AutoTuneMaintenanceScheduleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AutoTuneMaintenanceScheduleTypeDef](./type_defs.md#autotunemaintenancescheduletypedef) 
2. See [:material-code-braces: AutoTuneMaintenanceScheduleOutputTypeDef](./type_defs.md#autotunemaintenancescheduleoutputtypedef) 



## AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef

```python
# AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef definition

class AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef(TypedDict):
    CrossClusterSearchConnectionId: str,
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
## CancelDomainConfigChangeRequestRequestTypeDef

```python
# CancelDomainConfigChangeRequestRequestTypeDef definition

class CancelDomainConfigChangeRequestRequestTypeDef(TypedDict):
    DomainName: str,
    DryRun: NotRequired[bool],
```

## CancelledChangePropertyTypeDef

```python
# CancelledChangePropertyTypeDef definition

class CancelledChangePropertyTypeDef(TypedDict):
    PropertyName: NotRequired[str],
    CancelledValue: NotRequired[str],
    ActiveValue: NotRequired[str],
```

## CancelElasticsearchServiceSoftwareUpdateRequestRequestTypeDef

```python
# CancelElasticsearchServiceSoftwareUpdateRequestRequestTypeDef definition

class CancelElasticsearchServiceSoftwareUpdateRequestRequestTypeDef(TypedDict):
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
    ConfigChangeStatus: NotRequired[ConfigChangeStatusType],  # (1)
    StartTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    InitiatedBy: NotRequired[InitiatedByType],  # (2)
```

1. See [:material-code-brackets: ConfigChangeStatusType](./literals.md#configchangestatustype) 
2. See [:material-code-brackets: InitiatedByType](./literals.md#initiatedbytype) 
## ChangeProgressStageTypeDef

```python
# ChangeProgressStageTypeDef definition

class ChangeProgressStageTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[str],
    Description: NotRequired[str],
    LastUpdated: NotRequired[datetime],
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

## ColdStorageOptionsTypeDef

```python
# ColdStorageOptionsTypeDef definition

class ColdStorageOptionsTypeDef(TypedDict):
    Enabled: bool,
```

## CompatibleVersionsMapTypeDef

```python
# CompatibleVersionsMapTypeDef definition

class CompatibleVersionsMapTypeDef(TypedDict):
    SourceVersion: NotRequired[str],
    TargetVersions: NotRequired[List[str]],
```

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

## VPCOptionsTypeDef

```python
# VPCOptionsTypeDef definition

class VPCOptionsTypeDef(TypedDict):
    SubnetIds: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
```

## DomainInformationTypeDef

```python
# DomainInformationTypeDef definition

class DomainInformationTypeDef(TypedDict):
    DomainName: str,
    OwnerId: NotRequired[str],
    Region: NotRequired[str],
```

## OutboundCrossClusterSearchConnectionStatusTypeDef

```python
# OutboundCrossClusterSearchConnectionStatusTypeDef definition

class OutboundCrossClusterSearchConnectionStatusTypeDef(TypedDict):
    StatusCode: NotRequired[OutboundCrossClusterSearchConnectionStatusCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: OutboundCrossClusterSearchConnectionStatusCodeType](./literals.md#outboundcrossclustersearchconnectionstatuscodetype) 
## PackageSourceTypeDef

```python
# PackageSourceTypeDef definition

class PackageSourceTypeDef(TypedDict):
    S3BucketName: NotRequired[str],
    S3Key: NotRequired[str],
```

## DeleteElasticsearchDomainRequestRequestTypeDef

```python
# DeleteElasticsearchDomainRequestRequestTypeDef definition

class DeleteElasticsearchDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DeleteInboundCrossClusterSearchConnectionRequestRequestTypeDef

```python
# DeleteInboundCrossClusterSearchConnectionRequestRequestTypeDef definition

class DeleteInboundCrossClusterSearchConnectionRequestRequestTypeDef(TypedDict):
    CrossClusterSearchConnectionId: str,
```

## DeleteOutboundCrossClusterSearchConnectionRequestRequestTypeDef

```python
# DeleteOutboundCrossClusterSearchConnectionRequestRequestTypeDef definition

class DeleteOutboundCrossClusterSearchConnectionRequestRequestTypeDef(TypedDict):
    CrossClusterSearchConnectionId: str,
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

## DescribeElasticsearchDomainConfigRequestRequestTypeDef

```python
# DescribeElasticsearchDomainConfigRequestRequestTypeDef definition

class DescribeElasticsearchDomainConfigRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DescribeElasticsearchDomainRequestRequestTypeDef

```python
# DescribeElasticsearchDomainRequestRequestTypeDef definition

class DescribeElasticsearchDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DescribeElasticsearchDomainsRequestRequestTypeDef

```python
# DescribeElasticsearchDomainsRequestRequestTypeDef definition

class DescribeElasticsearchDomainsRequestRequestTypeDef(TypedDict):
    DomainNames: Sequence[str],
```

## DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef

```python
# DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef definition

class DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef(TypedDict):
    InstanceType: ESPartitionInstanceTypeType,  # (1)
    ElasticsearchVersion: str,
    DomainName: NotRequired[str],
```

1. See [:material-code-brackets: ESPartitionInstanceTypeType](./literals.md#espartitioninstancetypetype) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## DescribePackagesFilterTypeDef

```python
# DescribePackagesFilterTypeDef definition

class DescribePackagesFilterTypeDef(TypedDict):
    Name: NotRequired[DescribePackagesFilterNameType],  # (1)
    Value: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: DescribePackagesFilterNameType](./literals.md#describepackagesfilternametype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef

```python
# DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef definition

class DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef(TypedDict):
    ReservedElasticsearchInstanceOfferingId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeReservedElasticsearchInstancesRequestRequestTypeDef

```python
# DescribeReservedElasticsearchInstancesRequestRequestTypeDef definition

class DescribeReservedElasticsearchInstancesRequestRequestTypeDef(TypedDict):
    ReservedElasticsearchInstanceId: NotRequired[str],
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

## DryRunResultsTypeDef

```python
# DryRunResultsTypeDef definition

class DryRunResultsTypeDef(TypedDict):
    DeploymentType: NotRequired[str],
    Message: NotRequired[str],
```

## ZoneAwarenessConfigTypeDef

```python
# ZoneAwarenessConfigTypeDef definition

class ZoneAwarenessConfigTypeDef(TypedDict):
    AvailabilityZoneCount: NotRequired[int],
```

## ModifyingPropertiesTypeDef

```python
# ModifyingPropertiesTypeDef definition

class ModifyingPropertiesTypeDef(TypedDict):
    Name: NotRequired[str],
    ActiveValue: NotRequired[str],
    PendingValue: NotRequired[str],
    ValueType: NotRequired[PropertyValueTypeType],  # (1)
```

1. See [:material-code-brackets: PropertyValueTypeType](./literals.md#propertyvaluetypetype) 
## VPCDerivedInfoTypeDef

```python
# VPCDerivedInfoTypeDef definition

class VPCDerivedInfoTypeDef(TypedDict):
    VPCId: NotRequired[str],
    SubnetIds: NotRequired[List[str]],
    AvailabilityZones: NotRequired[List[str]],
    SecurityGroupIds: NotRequired[List[str]],
```

## GetCompatibleElasticsearchVersionsRequestRequestTypeDef

```python
# GetCompatibleElasticsearchVersionsRequestRequestTypeDef definition

class GetCompatibleElasticsearchVersionsRequestRequestTypeDef(TypedDict):
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

## InboundCrossClusterSearchConnectionStatusTypeDef

```python
# InboundCrossClusterSearchConnectionStatusTypeDef definition

class InboundCrossClusterSearchConnectionStatusTypeDef(TypedDict):
    StatusCode: NotRequired[InboundCrossClusterSearchConnectionStatusCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: InboundCrossClusterSearchConnectionStatusCodeType](./literals.md#inboundcrossclustersearchconnectionstatuscodetype) 
## InstanceCountLimitsTypeDef

```python
# InstanceCountLimitsTypeDef definition

class InstanceCountLimitsTypeDef(TypedDict):
    MinimumInstanceCount: NotRequired[int],
    MaximumInstanceCount: NotRequired[int],
```

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

## ListElasticsearchInstanceTypesRequestRequestTypeDef

```python
# ListElasticsearchInstanceTypesRequestRequestTypeDef definition

class ListElasticsearchInstanceTypesRequestRequestTypeDef(TypedDict):
    ElasticsearchVersion: str,
    DomainName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListElasticsearchVersionsRequestRequestTypeDef

```python
# ListElasticsearchVersionsRequestRequestTypeDef definition

class ListElasticsearchVersionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListPackagesForDomainRequestRequestTypeDef

```python
# ListPackagesForDomainRequestRequestTypeDef definition

class ListPackagesForDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsRequestRequestTypeDef

```python
# ListTagsRequestRequestTypeDef definition

class ListTagsRequestRequestTypeDef(TypedDict):
    ARN: str,
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

## PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef

```python
# PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef definition

class PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef(TypedDict):
    ReservedElasticsearchInstanceOfferingId: str,
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

## RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef

```python
# RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef definition

class RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef(TypedDict):
    CrossClusterSearchConnectionId: str,
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

## StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef

```python
# StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef definition

class StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## StorageTypeLimitTypeDef

```python
# StorageTypeLimitTypeDef definition

class StorageTypeLimitTypeDef(TypedDict):
    LimitName: NotRequired[str],
    LimitValues: NotRequired[List[str]],
```

## UpgradeElasticsearchDomainRequestRequestTypeDef

```python
# UpgradeElasticsearchDomainRequestRequestTypeDef definition

class UpgradeElasticsearchDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    TargetVersion: str,
    PerformCheckOnly: NotRequired[bool],
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
## ListElasticsearchInstanceTypesResponseTypeDef

```python
# ListElasticsearchInstanceTypesResponseTypeDef definition

class ListElasticsearchInstanceTypesResponseTypeDef(TypedDict):
    ElasticsearchInstanceTypes: List[ESPartitionInstanceTypeType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ESPartitionInstanceTypeType](./literals.md#espartitioninstancetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListElasticsearchVersionsResponseTypeDef

```python
# ListElasticsearchVersionsResponseTypeDef definition

class ListElasticsearchVersionsResponseTypeDef(TypedDict):
    ElasticsearchVersions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef

```python
# PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef definition

class PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef(TypedDict):
    ReservedElasticsearchInstanceId: str,
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
## ElasticsearchVersionStatusTypeDef

```python
# ElasticsearchVersionStatusTypeDef definition

class ElasticsearchVersionStatusTypeDef(TypedDict):
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
## AutoTuneMaintenanceScheduleOutputTypeDef

```python
# AutoTuneMaintenanceScheduleOutputTypeDef definition

class AutoTuneMaintenanceScheduleOutputTypeDef(TypedDict):
    StartAt: NotRequired[datetime],
    Duration: NotRequired[DurationTypeDef],  # (1)
    CronExpressionForRecurrence: NotRequired[str],
```

1. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
## AutoTuneMaintenanceScheduleTypeDef

```python
# AutoTuneMaintenanceScheduleTypeDef definition

class AutoTuneMaintenanceScheduleTypeDef(TypedDict):
    StartAt: NotRequired[TimestampTypeDef],
    Duration: NotRequired[DurationTypeDef],  # (1)
    CronExpressionForRecurrence: NotRequired[str],
```

1. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
## CancelDomainConfigChangeResponseTypeDef

```python
# CancelDomainConfigChangeResponseTypeDef definition

class CancelDomainConfigChangeResponseTypeDef(TypedDict):
    DryRun: bool,
    CancelledChangeIds: List[str],
    CancelledChangeProperties: List[CancelledChangePropertyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CancelledChangePropertyTypeDef](./type_defs.md#cancelledchangepropertytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelElasticsearchServiceSoftwareUpdateResponseTypeDef

```python
# CancelElasticsearchServiceSoftwareUpdateResponseTypeDef definition

class CancelElasticsearchServiceSoftwareUpdateResponseTypeDef(TypedDict):
    ServiceSoftwareOptions: ServiceSoftwareOptionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSoftwareOptionsTypeDef](./type_defs.md#servicesoftwareoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartElasticsearchServiceSoftwareUpdateResponseTypeDef

```python
# StartElasticsearchServiceSoftwareUpdateResponseTypeDef definition

class StartElasticsearchServiceSoftwareUpdateResponseTypeDef(TypedDict):
    ServiceSoftwareOptions: ServiceSoftwareOptionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSoftwareOptionsTypeDef](./type_defs.md#servicesoftwareoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpgradeElasticsearchDomainResponseTypeDef

```python
# UpgradeElasticsearchDomainResponseTypeDef definition

class UpgradeElasticsearchDomainResponseTypeDef(TypedDict):
    DomainName: str,
    TargetVersion: str,
    PerformCheckOnly: bool,
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
    ConfigChangeStatus: NotRequired[ConfigChangeStatusType],  # (3)
    LastUpdatedTime: NotRequired[datetime],
    InitiatedBy: NotRequired[InitiatedByType],  # (4)
```

1. See [:material-code-brackets: OverallChangeStatusType](./literals.md#overallchangestatustype) 
2. See [:material-code-braces: ChangeProgressStageTypeDef](./type_defs.md#changeprogressstagetypedef) 
3. See [:material-code-brackets: ConfigChangeStatusType](./literals.md#configchangestatustype) 
4. See [:material-code-brackets: InitiatedByType](./literals.md#initiatedbytype) 
## CognitoOptionsStatusTypeDef

```python
# CognitoOptionsStatusTypeDef definition

class CognitoOptionsStatusTypeDef(TypedDict):
    Options: CognitoOptionsTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: CognitoOptionsTypeDef](./type_defs.md#cognitooptionstypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## GetCompatibleElasticsearchVersionsResponseTypeDef

```python
# GetCompatibleElasticsearchVersionsResponseTypeDef definition

class GetCompatibleElasticsearchVersionsResponseTypeDef(TypedDict):
    CompatibleElasticsearchVersions: List[CompatibleVersionsMapTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompatibleVersionsMapTypeDef](./type_defs.md#compatibleversionsmaptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## CreateOutboundCrossClusterSearchConnectionRequestRequestTypeDef

```python
# CreateOutboundCrossClusterSearchConnectionRequestRequestTypeDef definition

class CreateOutboundCrossClusterSearchConnectionRequestRequestTypeDef(TypedDict):
    SourceDomainInfo: DomainInformationTypeDef,  # (1)
    DestinationDomainInfo: DomainInformationTypeDef,  # (1)
    ConnectionAlias: str,
```

1. See [:material-code-braces: DomainInformationTypeDef](./type_defs.md#domaininformationtypedef) 
2. See [:material-code-braces: DomainInformationTypeDef](./type_defs.md#domaininformationtypedef) 
## CreateOutboundCrossClusterSearchConnectionResponseTypeDef

```python
# CreateOutboundCrossClusterSearchConnectionResponseTypeDef definition

class CreateOutboundCrossClusterSearchConnectionResponseTypeDef(TypedDict):
    SourceDomainInfo: DomainInformationTypeDef,  # (1)
    DestinationDomainInfo: DomainInformationTypeDef,  # (1)
    ConnectionAlias: str,
    ConnectionStatus: OutboundCrossClusterSearchConnectionStatusTypeDef,  # (3)
    CrossClusterSearchConnectionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DomainInformationTypeDef](./type_defs.md#domaininformationtypedef) 
2. See [:material-code-braces: DomainInformationTypeDef](./type_defs.md#domaininformationtypedef) 
3. See [:material-code-braces: OutboundCrossClusterSearchConnectionStatusTypeDef](./type_defs.md#outboundcrossclustersearchconnectionstatustypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OutboundCrossClusterSearchConnectionTypeDef

```python
# OutboundCrossClusterSearchConnectionTypeDef definition

class OutboundCrossClusterSearchConnectionTypeDef(TypedDict):
    SourceDomainInfo: NotRequired[DomainInformationTypeDef],  # (1)
    DestinationDomainInfo: NotRequired[DomainInformationTypeDef],  # (1)
    CrossClusterSearchConnectionId: NotRequired[str],
    ConnectionAlias: NotRequired[str],
    ConnectionStatus: NotRequired[OutboundCrossClusterSearchConnectionStatusTypeDef],  # (3)
```

1. See [:material-code-braces: DomainInformationTypeDef](./type_defs.md#domaininformationtypedef) 
2. See [:material-code-braces: DomainInformationTypeDef](./type_defs.md#domaininformationtypedef) 
3. See [:material-code-braces: OutboundCrossClusterSearchConnectionStatusTypeDef](./type_defs.md#outboundcrossclustersearchconnectionstatustypedef) 
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
## DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef

```python
# DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef definition

class DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef

```python
# DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef definition

class DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef(TypedDict):
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
## DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef

```python
# DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef definition

class DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef(TypedDict):
    ReservedElasticsearchInstanceOfferingId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef

```python
# DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef definition

class DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef(TypedDict):
    ReservedElasticsearchInstanceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef

```python
# GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef definition

class GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef(TypedDict):
    DomainName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef

```python
# ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef definition

class ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef(TypedDict):
    ElasticsearchVersion: str,
    DomainName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef

```python
# ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef definition

class ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
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
## ElasticsearchClusterConfigTypeDef

```python
# ElasticsearchClusterConfigTypeDef definition

class ElasticsearchClusterConfigTypeDef(TypedDict):
    InstanceType: NotRequired[ESPartitionInstanceTypeType],  # (1)
    InstanceCount: NotRequired[int],
    DedicatedMasterEnabled: NotRequired[bool],
    ZoneAwarenessEnabled: NotRequired[bool],
    ZoneAwarenessConfig: NotRequired[ZoneAwarenessConfigTypeDef],  # (2)
    DedicatedMasterType: NotRequired[ESPartitionInstanceTypeType],  # (1)
    DedicatedMasterCount: NotRequired[int],
    WarmEnabled: NotRequired[bool],
    WarmType: NotRequired[ESWarmPartitionInstanceTypeType],  # (4)
    WarmCount: NotRequired[int],
    ColdStorageOptions: NotRequired[ColdStorageOptionsTypeDef],  # (5)
```

1. See [:material-code-brackets: ESPartitionInstanceTypeType](./literals.md#espartitioninstancetypetype) 
2. See [:material-code-braces: ZoneAwarenessConfigTypeDef](./type_defs.md#zoneawarenessconfigtypedef) 
3. See [:material-code-brackets: ESPartitionInstanceTypeType](./literals.md#espartitioninstancetypetype) 
4. See [:material-code-brackets: ESWarmPartitionInstanceTypeType](./literals.md#eswarmpartitioninstancetypetype) 
5. See [:material-code-braces: ColdStorageOptionsTypeDef](./type_defs.md#coldstorageoptionstypedef) 
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
## GetPackageVersionHistoryResponseTypeDef

```python
# GetPackageVersionHistoryResponseTypeDef definition

class GetPackageVersionHistoryResponseTypeDef(TypedDict):
    PackageID: str,
    PackageVersionHistoryList: List[PackageVersionHistoryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PackageVersionHistoryTypeDef](./type_defs.md#packageversionhistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InboundCrossClusterSearchConnectionTypeDef

```python
# InboundCrossClusterSearchConnectionTypeDef definition

class InboundCrossClusterSearchConnectionTypeDef(TypedDict):
    SourceDomainInfo: NotRequired[DomainInformationTypeDef],  # (1)
    DestinationDomainInfo: NotRequired[DomainInformationTypeDef],  # (1)
    CrossClusterSearchConnectionId: NotRequired[str],
    ConnectionStatus: NotRequired[InboundCrossClusterSearchConnectionStatusTypeDef],  # (3)
```

1. See [:material-code-braces: DomainInformationTypeDef](./type_defs.md#domaininformationtypedef) 
2. See [:material-code-braces: DomainInformationTypeDef](./type_defs.md#domaininformationtypedef) 
3. See [:material-code-braces: InboundCrossClusterSearchConnectionStatusTypeDef](./type_defs.md#inboundcrossclustersearchconnectionstatustypedef) 
## InstanceLimitsTypeDef

```python
# InstanceLimitsTypeDef definition

class InstanceLimitsTypeDef(TypedDict):
    InstanceCountLimits: NotRequired[InstanceCountLimitsTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceCountLimitsTypeDef](./type_defs.md#instancecountlimitstypedef) 
## ReservedElasticsearchInstanceOfferingTypeDef

```python
# ReservedElasticsearchInstanceOfferingTypeDef definition

class ReservedElasticsearchInstanceOfferingTypeDef(TypedDict):
    ReservedElasticsearchInstanceOfferingId: NotRequired[str],
    ElasticsearchInstanceType: NotRequired[ESPartitionInstanceTypeType],  # (1)
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    UsagePrice: NotRequired[float],
    CurrencyCode: NotRequired[str],
    PaymentOption: NotRequired[ReservedElasticsearchInstancePaymentOptionType],  # (2)
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (3)
```

1. See [:material-code-brackets: ESPartitionInstanceTypeType](./literals.md#espartitioninstancetypetype) 
2. See [:material-code-brackets: ReservedElasticsearchInstancePaymentOptionType](./literals.md#reservedelasticsearchinstancepaymentoptiontype) 
3. See [:material-code-braces: RecurringChargeTypeDef](./type_defs.md#recurringchargetypedef) 
## ReservedElasticsearchInstanceTypeDef

```python
# ReservedElasticsearchInstanceTypeDef definition

class ReservedElasticsearchInstanceTypeDef(TypedDict):
    ReservationName: NotRequired[str],
    ReservedElasticsearchInstanceId: NotRequired[str],
    ReservedElasticsearchInstanceOfferingId: NotRequired[str],
    ElasticsearchInstanceType: NotRequired[ESPartitionInstanceTypeType],  # (1)
    StartTime: NotRequired[datetime],
    Duration: NotRequired[int],
    FixedPrice: NotRequired[float],
    UsagePrice: NotRequired[float],
    CurrencyCode: NotRequired[str],
    ElasticsearchInstanceCount: NotRequired[int],
    State: NotRequired[str],
    PaymentOption: NotRequired[ReservedElasticsearchInstancePaymentOptionType],  # (2)
    RecurringCharges: NotRequired[List[RecurringChargeTypeDef]],  # (3)
```

1. See [:material-code-brackets: ESPartitionInstanceTypeType](./literals.md#espartitioninstancetypetype) 
2. See [:material-code-brackets: ReservedElasticsearchInstancePaymentOptionType](./literals.md#reservedelasticsearchinstancepaymentoptiontype) 
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
## AutoTuneTypeDef

```python
# AutoTuneTypeDef definition

class AutoTuneTypeDef(TypedDict):
    AutoTuneType: NotRequired[AutoTuneTypeType],  # (1)
    AutoTuneDetails: NotRequired[AutoTuneDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: AutoTuneTypeType](./literals.md#autotunetypetype) 
2. See [:material-code-braces: AutoTuneDetailsTypeDef](./type_defs.md#autotunedetailstypedef) 
## AutoTuneOptionsExtraOutputTypeDef

```python
# AutoTuneOptionsExtraOutputTypeDef definition

class AutoTuneOptionsExtraOutputTypeDef(TypedDict):
    DesiredState: NotRequired[AutoTuneDesiredStateType],  # (1)
    RollbackOnDisable: NotRequired[RollbackOnDisableType],  # (2)
    MaintenanceSchedules: NotRequired[List[AutoTuneMaintenanceScheduleOutputTypeDef]],  # (3)
```

1. See [:material-code-brackets: AutoTuneDesiredStateType](./literals.md#autotunedesiredstatetype) 
2. See [:material-code-brackets: RollbackOnDisableType](./literals.md#rollbackondisabletype) 
3. See [:material-code-braces: AutoTuneMaintenanceScheduleOutputTypeDef](./type_defs.md#autotunemaintenancescheduleoutputtypedef) 
## DescribeDomainChangeProgressResponseTypeDef

```python
# DescribeDomainChangeProgressResponseTypeDef definition

class DescribeDomainChangeProgressResponseTypeDef(TypedDict):
    ChangeProgressStatus: ChangeProgressStatusDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeProgressStatusDetailsTypeDef](./type_defs.md#changeprogressstatusdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteOutboundCrossClusterSearchConnectionResponseTypeDef

```python
# DeleteOutboundCrossClusterSearchConnectionResponseTypeDef definition

class DeleteOutboundCrossClusterSearchConnectionResponseTypeDef(TypedDict):
    CrossClusterSearchConnection: OutboundCrossClusterSearchConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutboundCrossClusterSearchConnectionTypeDef](./type_defs.md#outboundcrossclustersearchconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef

```python
# DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef definition

class DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef(TypedDict):
    CrossClusterSearchConnections: List[OutboundCrossClusterSearchConnectionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OutboundCrossClusterSearchConnectionTypeDef](./type_defs.md#outboundcrossclustersearchconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainPackageDetailsTypeDef](./type_defs.md#domainpackagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPackagesForDomainResponseTypeDef

```python
# ListPackagesForDomainResponseTypeDef definition

class ListPackagesForDomainResponseTypeDef(TypedDict):
    DomainPackageDetailsList: List[DomainPackageDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
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
## ElasticsearchClusterConfigStatusTypeDef

```python
# ElasticsearchClusterConfigStatusTypeDef definition

class ElasticsearchClusterConfigStatusTypeDef(TypedDict):
    Options: ElasticsearchClusterConfigTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: ElasticsearchClusterConfigTypeDef](./type_defs.md#elasticsearchclusterconfigtypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
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
## AcceptInboundCrossClusterSearchConnectionResponseTypeDef

```python
# AcceptInboundCrossClusterSearchConnectionResponseTypeDef definition

class AcceptInboundCrossClusterSearchConnectionResponseTypeDef(TypedDict):
    CrossClusterSearchConnection: InboundCrossClusterSearchConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InboundCrossClusterSearchConnectionTypeDef](./type_defs.md#inboundcrossclustersearchconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInboundCrossClusterSearchConnectionResponseTypeDef

```python
# DeleteInboundCrossClusterSearchConnectionResponseTypeDef definition

class DeleteInboundCrossClusterSearchConnectionResponseTypeDef(TypedDict):
    CrossClusterSearchConnection: InboundCrossClusterSearchConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InboundCrossClusterSearchConnectionTypeDef](./type_defs.md#inboundcrossclustersearchconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInboundCrossClusterSearchConnectionsResponseTypeDef

```python
# DescribeInboundCrossClusterSearchConnectionsResponseTypeDef definition

class DescribeInboundCrossClusterSearchConnectionsResponseTypeDef(TypedDict):
    CrossClusterSearchConnections: List[InboundCrossClusterSearchConnectionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InboundCrossClusterSearchConnectionTypeDef](./type_defs.md#inboundcrossclustersearchconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RejectInboundCrossClusterSearchConnectionResponseTypeDef

```python
# RejectInboundCrossClusterSearchConnectionResponseTypeDef definition

class RejectInboundCrossClusterSearchConnectionResponseTypeDef(TypedDict):
    CrossClusterSearchConnection: InboundCrossClusterSearchConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InboundCrossClusterSearchConnectionTypeDef](./type_defs.md#inboundcrossclustersearchconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef

```python
# DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef definition

class DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef(TypedDict):
    ReservedElasticsearchInstanceOfferings: List[ReservedElasticsearchInstanceOfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReservedElasticsearchInstanceOfferingTypeDef](./type_defs.md#reservedelasticsearchinstanceofferingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReservedElasticsearchInstancesResponseTypeDef

```python
# DescribeReservedElasticsearchInstancesResponseTypeDef definition

class DescribeReservedElasticsearchInstancesResponseTypeDef(TypedDict):
    ReservedElasticsearchInstances: List[ReservedElasticsearchInstanceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReservedElasticsearchInstanceTypeDef](./type_defs.md#reservedelasticsearchinstancetypedef) 
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UpgradeHistoryTypeDef](./type_defs.md#upgradehistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDomainAutoTunesResponseTypeDef

```python
# DescribeDomainAutoTunesResponseTypeDef definition

class DescribeDomainAutoTunesResponseTypeDef(TypedDict):
    AutoTunes: List[AutoTuneTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AutoTuneTypeDef](./type_defs.md#autotunetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoTuneOptionsStatusTypeDef

```python
# AutoTuneOptionsStatusTypeDef definition

class AutoTuneOptionsStatusTypeDef(TypedDict):
    Options: NotRequired[AutoTuneOptionsExtraOutputTypeDef],  # (1)
    Status: NotRequired[AutoTuneStatusTypeDef],  # (2)
```

1. See [:material-code-braces: AutoTuneOptionsExtraOutputTypeDef](./type_defs.md#autotuneoptionsextraoutputtypedef) 
2. See [:material-code-braces: AutoTuneStatusTypeDef](./type_defs.md#autotunestatustypedef) 
## AutoTuneOptionsInputTypeDef

```python
# AutoTuneOptionsInputTypeDef definition

class AutoTuneOptionsInputTypeDef(TypedDict):
    DesiredState: NotRequired[AutoTuneDesiredStateType],  # (1)
    MaintenanceSchedules: NotRequired[Sequence[AutoTuneMaintenanceScheduleUnionTypeDef]],  # (2)
```

1. See [:material-code-brackets: AutoTuneDesiredStateType](./literals.md#autotunedesiredstatetype) 
2. See [:material-code-braces: AutoTuneMaintenanceScheduleTypeDef](./type_defs.md#autotunemaintenancescheduletypedef) [:material-code-braces: AutoTuneMaintenanceScheduleOutputTypeDef](./type_defs.md#autotunemaintenancescheduleoutputtypedef) 
## AutoTuneOptionsTypeDef

```python
# AutoTuneOptionsTypeDef definition

class AutoTuneOptionsTypeDef(TypedDict):
    DesiredState: NotRequired[AutoTuneDesiredStateType],  # (1)
    RollbackOnDisable: NotRequired[RollbackOnDisableType],  # (2)
    MaintenanceSchedules: NotRequired[Sequence[AutoTuneMaintenanceScheduleUnionTypeDef]],  # (3)
```

1. See [:material-code-brackets: AutoTuneDesiredStateType](./literals.md#autotunedesiredstatetype) 
2. See [:material-code-brackets: RollbackOnDisableType](./literals.md#rollbackondisabletype) 
3. See [:material-code-braces: AutoTuneMaintenanceScheduleTypeDef](./type_defs.md#autotunemaintenancescheduletypedef) [:material-code-braces: AutoTuneMaintenanceScheduleOutputTypeDef](./type_defs.md#autotunemaintenancescheduleoutputtypedef) 
## AdvancedSecurityOptionsStatusTypeDef

```python
# AdvancedSecurityOptionsStatusTypeDef definition

class AdvancedSecurityOptionsStatusTypeDef(TypedDict):
    Options: AdvancedSecurityOptionsTypeDef,  # (1)
    Status: OptionStatusTypeDef,  # (2)
```

1. See [:material-code-braces: AdvancedSecurityOptionsTypeDef](./type_defs.md#advancedsecurityoptionstypedef) 
2. See [:material-code-braces: OptionStatusTypeDef](./type_defs.md#optionstatustypedef) 
## ElasticsearchDomainStatusTypeDef

```python
# ElasticsearchDomainStatusTypeDef definition

class ElasticsearchDomainStatusTypeDef(TypedDict):
    DomainId: str,
    DomainName: str,
    ARN: str,
    ElasticsearchClusterConfig: ElasticsearchClusterConfigTypeDef,  # (1)
    Created: NotRequired[bool],
    Deleted: NotRequired[bool],
    Endpoint: NotRequired[str],
    Endpoints: NotRequired[Dict[str, str]],
    Processing: NotRequired[bool],
    UpgradeProcessing: NotRequired[bool],
    ElasticsearchVersion: NotRequired[str],
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
    DomainProcessingStatus: NotRequired[DomainProcessingStatusTypeType],  # (14)
    ModifyingProperties: NotRequired[List[ModifyingPropertiesTypeDef]],  # (15)
```

1. See [:material-code-braces: ElasticsearchClusterConfigTypeDef](./type_defs.md#elasticsearchclusterconfigtypedef) 
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
14. See [:material-code-brackets: DomainProcessingStatusTypeType](./literals.md#domainprocessingstatustypetype) 
15. See [:material-code-braces: ModifyingPropertiesTypeDef](./type_defs.md#modifyingpropertiestypedef) 
## DescribeElasticsearchInstanceTypeLimitsResponseTypeDef

```python
# DescribeElasticsearchInstanceTypeLimitsResponseTypeDef definition

class DescribeElasticsearchInstanceTypeLimitsResponseTypeDef(TypedDict):
    LimitsByRole: Dict[str, LimitsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LimitsTypeDef](./type_defs.md#limitstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateElasticsearchDomainRequestRequestTypeDef

```python
# CreateElasticsearchDomainRequestRequestTypeDef definition

class CreateElasticsearchDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ElasticsearchVersion: NotRequired[str],
    ElasticsearchClusterConfig: NotRequired[ElasticsearchClusterConfigTypeDef],  # (1)
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
    AutoTuneOptions: NotRequired[AutoTuneOptionsInputTypeDef],  # (11)
    TagList: NotRequired[Sequence[TagTypeDef]],  # (12)
```

1. See [:material-code-braces: ElasticsearchClusterConfigTypeDef](./type_defs.md#elasticsearchclusterconfigtypedef) 
2. See [:material-code-braces: EBSOptionsTypeDef](./type_defs.md#ebsoptionstypedef) 
3. See [:material-code-braces: SnapshotOptionsTypeDef](./type_defs.md#snapshotoptionstypedef) 
4. See [:material-code-braces: VPCOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
5. See [:material-code-braces: CognitoOptionsTypeDef](./type_defs.md#cognitooptionstypedef) 
6. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef) 
7. See [:material-code-braces: NodeToNodeEncryptionOptionsTypeDef](./type_defs.md#nodetonodeencryptionoptionstypedef) 
8. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) [:material-code-braces: LogPublishingOptionTypeDef](./type_defs.md#logpublishingoptiontypedef) 
9. See [:material-code-braces: DomainEndpointOptionsTypeDef](./type_defs.md#domainendpointoptionstypedef) 
10. See [:material-code-braces: AdvancedSecurityOptionsInputTypeDef](./type_defs.md#advancedsecurityoptionsinputtypedef) 
11. See [:material-code-braces: AutoTuneOptionsInputTypeDef](./type_defs.md#autotuneoptionsinputtypedef) 
12. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateElasticsearchDomainConfigRequestRequestTypeDef

```python
# UpdateElasticsearchDomainConfigRequestRequestTypeDef definition

class UpdateElasticsearchDomainConfigRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ElasticsearchClusterConfig: NotRequired[ElasticsearchClusterConfigTypeDef],  # (1)
    EBSOptions: NotRequired[EBSOptionsTypeDef],  # (2)
    SnapshotOptions: NotRequired[SnapshotOptionsTypeDef],  # (3)
    VPCOptions: NotRequired[VPCOptionsTypeDef],  # (4)
    CognitoOptions: NotRequired[CognitoOptionsTypeDef],  # (5)
    AdvancedOptions: NotRequired[Mapping[str, str]],
    AccessPolicies: NotRequired[str],
    LogPublishingOptions: NotRequired[Mapping[LogTypeType, LogPublishingOptionTypeDef]],  # (6)
    DomainEndpointOptions: NotRequired[DomainEndpointOptionsTypeDef],  # (7)
    AdvancedSecurityOptions: NotRequired[AdvancedSecurityOptionsInputTypeDef],  # (8)
    NodeToNodeEncryptionOptions: NotRequired[NodeToNodeEncryptionOptionsTypeDef],  # (9)
    EncryptionAtRestOptions: NotRequired[EncryptionAtRestOptionsTypeDef],  # (10)
    AutoTuneOptions: NotRequired[AutoTuneOptionsTypeDef],  # (11)
    DryRun: NotRequired[bool],
```

1. See [:material-code-braces: ElasticsearchClusterConfigTypeDef](./type_defs.md#elasticsearchclusterconfigtypedef) 
2. See [:material-code-braces: EBSOptionsTypeDef](./type_defs.md#ebsoptionstypedef) 
3. See [:material-code-braces: SnapshotOptionsTypeDef](./type_defs.md#snapshotoptionstypedef) 
4. See [:material-code-braces: VPCOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
5. See [:material-code-braces: CognitoOptionsTypeDef](./type_defs.md#cognitooptionstypedef) 
6. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) [:material-code-braces: LogPublishingOptionTypeDef](./type_defs.md#logpublishingoptiontypedef) 
7. See [:material-code-braces: DomainEndpointOptionsTypeDef](./type_defs.md#domainendpointoptionstypedef) 
8. See [:material-code-braces: AdvancedSecurityOptionsInputTypeDef](./type_defs.md#advancedsecurityoptionsinputtypedef) 
9. See [:material-code-braces: NodeToNodeEncryptionOptionsTypeDef](./type_defs.md#nodetonodeencryptionoptionstypedef) 
10. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef) 
11. See [:material-code-braces: AutoTuneOptionsTypeDef](./type_defs.md#autotuneoptionstypedef) 
## ElasticsearchDomainConfigTypeDef

```python
# ElasticsearchDomainConfigTypeDef definition

class ElasticsearchDomainConfigTypeDef(TypedDict):
    ElasticsearchVersion: NotRequired[ElasticsearchVersionStatusTypeDef],  # (1)
    ElasticsearchClusterConfig: NotRequired[ElasticsearchClusterConfigStatusTypeDef],  # (2)
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
    ModifyingProperties: NotRequired[List[ModifyingPropertiesTypeDef]],  # (16)
```

1. See [:material-code-braces: ElasticsearchVersionStatusTypeDef](./type_defs.md#elasticsearchversionstatustypedef) 
2. See [:material-code-braces: ElasticsearchClusterConfigStatusTypeDef](./type_defs.md#elasticsearchclusterconfigstatustypedef) 
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
16. See [:material-code-braces: ModifyingPropertiesTypeDef](./type_defs.md#modifyingpropertiestypedef) 
## CreateElasticsearchDomainResponseTypeDef

```python
# CreateElasticsearchDomainResponseTypeDef definition

class CreateElasticsearchDomainResponseTypeDef(TypedDict):
    DomainStatus: ElasticsearchDomainStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ElasticsearchDomainStatusTypeDef](./type_defs.md#elasticsearchdomainstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteElasticsearchDomainResponseTypeDef

```python
# DeleteElasticsearchDomainResponseTypeDef definition

class DeleteElasticsearchDomainResponseTypeDef(TypedDict):
    DomainStatus: ElasticsearchDomainStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ElasticsearchDomainStatusTypeDef](./type_defs.md#elasticsearchdomainstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeElasticsearchDomainResponseTypeDef

```python
# DescribeElasticsearchDomainResponseTypeDef definition

class DescribeElasticsearchDomainResponseTypeDef(TypedDict):
    DomainStatus: ElasticsearchDomainStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ElasticsearchDomainStatusTypeDef](./type_defs.md#elasticsearchdomainstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeElasticsearchDomainsResponseTypeDef

```python
# DescribeElasticsearchDomainsResponseTypeDef definition

class DescribeElasticsearchDomainsResponseTypeDef(TypedDict):
    DomainStatusList: List[ElasticsearchDomainStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ElasticsearchDomainStatusTypeDef](./type_defs.md#elasticsearchdomainstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeElasticsearchDomainConfigResponseTypeDef

```python
# DescribeElasticsearchDomainConfigResponseTypeDef definition

class DescribeElasticsearchDomainConfigResponseTypeDef(TypedDict):
    DomainConfig: ElasticsearchDomainConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ElasticsearchDomainConfigTypeDef](./type_defs.md#elasticsearchdomainconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateElasticsearchDomainConfigResponseTypeDef

```python
# UpdateElasticsearchDomainConfigResponseTypeDef definition

class UpdateElasticsearchDomainConfigResponseTypeDef(TypedDict):
    DomainConfig: ElasticsearchDomainConfigTypeDef,  # (1)
    DryRunResults: DryRunResultsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ElasticsearchDomainConfigTypeDef](./type_defs.md#elasticsearchdomainconfigtypedef) 
2. See [:material-code-braces: DryRunResultsTypeDef](./type_defs.md#dryrunresultstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
