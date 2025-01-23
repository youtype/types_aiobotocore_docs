# Type definitions

> [Index](../README.md) > [GuardDuty](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [GuardDuty](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#guardduty)
    type annotations stubs module [types-aiobotocore-guardduty](https://pypi.org/project/types-aiobotocore-guardduty/).

## ConditionUnionTypeDef

```python
# ConditionUnionTypeDef definition

ConditionUnionTypeDef = Union[
    ConditionTypeDef,  # (1)
    ConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
2. See [:material-code-braces: ConditionOutputTypeDef](./type_defs.md#conditionoutputtypedef) 

## CreateS3BucketResourceUnionTypeDef

```python
# CreateS3BucketResourceUnionTypeDef definition

CreateS3BucketResourceUnionTypeDef = Union[
    CreateS3BucketResourceTypeDef,  # (1)
    CreateS3BucketResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CreateS3BucketResourceTypeDef](./type_defs.md#creates3bucketresourcetypedef) 
2. See [:material-code-braces: CreateS3BucketResourceOutputTypeDef](./type_defs.md#creates3bucketresourceoutputtypedef) 

## ScanConditionUnionTypeDef

```python
# ScanConditionUnionTypeDef definition

ScanConditionUnionTypeDef = Union[
    ScanConditionTypeDef,  # (1)
    ScanConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScanConditionTypeDef](./type_defs.md#scanconditiontypedef) 
2. See [:material-code-braces: ScanConditionOutputTypeDef](./type_defs.md#scanconditionoutputtypedef) 



## AcceptAdministratorInvitationRequestRequestTypeDef

```python
# AcceptAdministratorInvitationRequestRequestTypeDef definition

class AcceptAdministratorInvitationRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AdministratorId: str,
    InvitationId: str,
```

## AcceptInvitationRequestRequestTypeDef

```python
# AcceptInvitationRequestRequestTypeDef definition

class AcceptInvitationRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    MasterId: str,
    InvitationId: str,
```

## AccessControlListTypeDef

```python
# AccessControlListTypeDef definition

class AccessControlListTypeDef(TypedDict):
    AllowsPublicReadAccess: NotRequired[bool],
    AllowsPublicWriteAccess: NotRequired[bool],
```

## AccessKeyDetailsTypeDef

```python
# AccessKeyDetailsTypeDef definition

class AccessKeyDetailsTypeDef(TypedDict):
    AccessKeyId: NotRequired[str],
    PrincipalId: NotRequired[str],
    UserName: NotRequired[str],
    UserType: NotRequired[str],
```

## AccessKeyTypeDef

```python
# AccessKeyTypeDef definition

class AccessKeyTypeDef(TypedDict):
    PrincipalId: NotRequired[str],
    UserName: NotRequired[str],
    UserType: NotRequired[str],
```

## AccountDetailTypeDef

```python
# AccountDetailTypeDef definition

class AccountDetailTypeDef(TypedDict):
    AccountId: str,
    Email: str,
```

## FreeTrialFeatureConfigurationResultTypeDef

```python
# FreeTrialFeatureConfigurationResultTypeDef definition

class FreeTrialFeatureConfigurationResultTypeDef(TypedDict):
    Name: NotRequired[FreeTrialFeatureResultType],  # (1)
    FreeTrialDaysRemaining: NotRequired[int],
```

1. See [:material-code-brackets: FreeTrialFeatureResultType](./literals.md#freetrialfeatureresulttype) 
## BlockPublicAccessTypeDef

```python
# BlockPublicAccessTypeDef definition

class BlockPublicAccessTypeDef(TypedDict):
    IgnorePublicAcls: NotRequired[bool],
    RestrictPublicBuckets: NotRequired[bool],
    BlockPublicAcls: NotRequired[bool],
    BlockPublicPolicy: NotRequired[bool],
```

## AccountStatisticsTypeDef

```python
# AccountStatisticsTypeDef definition

class AccountStatisticsTypeDef(TypedDict):
    AccountId: NotRequired[str],
    LastGeneratedAt: NotRequired[datetime],
    TotalFindings: NotRequired[int],
```

## AccountTypeDef

```python
# AccountTypeDef definition

class AccountTypeDef(TypedDict):
    Uid: str,
    Name: NotRequired[str],
```

## DnsRequestActionTypeDef

```python
# DnsRequestActionTypeDef definition

class DnsRequestActionTypeDef(TypedDict):
    Domain: NotRequired[str],
    Protocol: NotRequired[str],
    Blocked: NotRequired[bool],
    DomainWithSuffix: NotRequired[str],
```

## KubernetesPermissionCheckedDetailsTypeDef

```python
# KubernetesPermissionCheckedDetailsTypeDef definition

class KubernetesPermissionCheckedDetailsTypeDef(TypedDict):
    Verb: NotRequired[str],
    Resource: NotRequired[str],
    Namespace: NotRequired[str],
    Allowed: NotRequired[bool],
```

## KubernetesRoleBindingDetailsTypeDef

```python
# KubernetesRoleBindingDetailsTypeDef definition

class KubernetesRoleBindingDetailsTypeDef(TypedDict):
    Kind: NotRequired[str],
    Name: NotRequired[str],
    Uid: NotRequired[str],
    RoleRefName: NotRequired[str],
    RoleRefKind: NotRequired[str],
```

## KubernetesRoleDetailsTypeDef

```python
# KubernetesRoleDetailsTypeDef definition

class KubernetesRoleDetailsTypeDef(TypedDict):
    Kind: NotRequired[str],
    Name: NotRequired[str],
    Uid: NotRequired[str],
```

## SessionTypeDef

```python
# SessionTypeDef definition

class SessionTypeDef(TypedDict):
    Uid: NotRequired[str],
    MfaStatus: NotRequired[MfaStatusType],  # (1)
    CreatedTime: NotRequired[datetime],
    Issuer: NotRequired[str],
```

1. See [:material-code-brackets: MfaStatusType](./literals.md#mfastatustype) 
## AddonDetailsTypeDef

```python
# AddonDetailsTypeDef definition

class AddonDetailsTypeDef(TypedDict):
    AddonVersion: NotRequired[str],
    AddonStatus: NotRequired[str],
```

## AdminAccountTypeDef

```python
# AdminAccountTypeDef definition

class AdminAccountTypeDef(TypedDict):
    AdminAccountId: NotRequired[str],
    AdminStatus: NotRequired[AdminStatusType],  # (1)
```

1. See [:material-code-brackets: AdminStatusType](./literals.md#adminstatustype) 
## AdministratorTypeDef

```python
# AdministratorTypeDef definition

class AdministratorTypeDef(TypedDict):
    AccountId: NotRequired[str],
    InvitationId: NotRequired[str],
    RelationshipStatus: NotRequired[str],
    InvitedAt: NotRequired[str],
```

## AgentDetailsTypeDef

```python
# AgentDetailsTypeDef definition

class AgentDetailsTypeDef(TypedDict):
    Version: NotRequired[str],
```

## ObservationsTypeDef

```python
# ObservationsTypeDef definition

class ObservationsTypeDef(TypedDict):
    Text: NotRequired[List[str]],
```

## ArchiveFindingsRequestRequestTypeDef

```python
# ArchiveFindingsRequestRequestTypeDef definition

class ArchiveFindingsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    FindingIds: Sequence[str],
```

## AutonomousSystemTypeDef

```python
# AutonomousSystemTypeDef definition

class AutonomousSystemTypeDef(TypedDict):
    Name: str,
    Number: int,
```

## DomainDetailsTypeDef

```python
# DomainDetailsTypeDef definition

class DomainDetailsTypeDef(TypedDict):
    Domain: NotRequired[str],
```

## RemoteAccountDetailsTypeDef

```python
# RemoteAccountDetailsTypeDef definition

class RemoteAccountDetailsTypeDef(TypedDict):
    AccountId: NotRequired[str],
    Affiliated: NotRequired[bool],
```

## BucketPolicyTypeDef

```python
# BucketPolicyTypeDef definition

class BucketPolicyTypeDef(TypedDict):
    AllowsPublicReadAccess: NotRequired[bool],
    AllowsPublicWriteAccess: NotRequired[bool],
```

## CityTypeDef

```python
# CityTypeDef definition

class CityTypeDef(TypedDict):
    CityName: NotRequired[str],
```

## CloudTrailConfigurationResultTypeDef

```python
# CloudTrailConfigurationResultTypeDef definition

class CloudTrailConfigurationResultTypeDef(TypedDict):
    Status: DataSourceStatusType,  # (1)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## ConditionOutputTypeDef

```python
# ConditionOutputTypeDef definition

class ConditionOutputTypeDef(TypedDict):
    Eq: NotRequired[List[str]],
    Neq: NotRequired[List[str]],
    Gt: NotRequired[int],
    Gte: NotRequired[int],
    Lt: NotRequired[int],
    Lte: NotRequired[int],
    Equals: NotRequired[List[str]],
    NotEquals: NotRequired[List[str]],
    GreaterThan: NotRequired[int],
    GreaterThanOrEqual: NotRequired[int],
    LessThan: NotRequired[int],
    LessThanOrEqual: NotRequired[int],
```

## ConditionTypeDef

```python
# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    Eq: NotRequired[Sequence[str]],
    Neq: NotRequired[Sequence[str]],
    Gt: NotRequired[int],
    Gte: NotRequired[int],
    Lt: NotRequired[int],
    Lte: NotRequired[int],
    Equals: NotRequired[Sequence[str]],
    NotEquals: NotRequired[Sequence[str]],
    GreaterThan: NotRequired[int],
    GreaterThanOrEqual: NotRequired[int],
    LessThan: NotRequired[int],
    LessThanOrEqual: NotRequired[int],
```

## ContainerInstanceDetailsTypeDef

```python
# ContainerInstanceDetailsTypeDef definition

class ContainerInstanceDetailsTypeDef(TypedDict):
    CoveredContainerInstances: NotRequired[int],
    CompatibleContainerInstances: NotRequired[int],
```

## SecurityContextTypeDef

```python
# SecurityContextTypeDef definition

class SecurityContextTypeDef(TypedDict):
    Privileged: NotRequired[bool],
    AllowPrivilegeEscalation: NotRequired[bool],
```

## VolumeMountTypeDef

```python
# VolumeMountTypeDef definition

class VolumeMountTypeDef(TypedDict):
    Name: NotRequired[str],
    MountPath: NotRequired[str],
```

## CountryTypeDef

```python
# CountryTypeDef definition

class CountryTypeDef(TypedDict):
    CountryCode: NotRequired[str],
    CountryName: NotRequired[str],
```

## FargateDetailsTypeDef

```python
# FargateDetailsTypeDef definition

class FargateDetailsTypeDef(TypedDict):
    Issues: NotRequired[List[str]],
    ManagementType: NotRequired[ManagementTypeType],  # (1)
```

1. See [:material-code-brackets: ManagementTypeType](./literals.md#managementtypetype) 
## CoverageFilterConditionTypeDef

```python
# CoverageFilterConditionTypeDef definition

class CoverageFilterConditionTypeDef(TypedDict):
    Equals: NotRequired[Sequence[str]],
    NotEquals: NotRequired[Sequence[str]],
```

## CoverageSortCriteriaTypeDef

```python
# CoverageSortCriteriaTypeDef definition

class CoverageSortCriteriaTypeDef(TypedDict):
    AttributeName: NotRequired[CoverageSortKeyType],  # (1)
    OrderBy: NotRequired[OrderByType],  # (2)
```

1. See [:material-code-brackets: CoverageSortKeyType](./literals.md#coveragesortkeytype) 
2. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
## CoverageStatisticsTypeDef

```python
# CoverageStatisticsTypeDef definition

class CoverageStatisticsTypeDef(TypedDict):
    CountByResourceType: NotRequired[Dict[ResourceTypeType, int]],  # (1)
    CountByCoverageStatus: NotRequired[Dict[CoverageStatusType, int]],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: CoverageStatusType](./literals.md#coveragestatustype) 
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

## CreateIPSetRequestRequestTypeDef

```python
# CreateIPSetRequestRequestTypeDef definition

class CreateIPSetRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    Name: str,
    Format: IpSetFormatType,  # (1)
    Location: str,
    Activate: bool,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: IpSetFormatType](./literals.md#ipsetformattype) 
## UnprocessedAccountTypeDef

```python
# UnprocessedAccountTypeDef definition

class UnprocessedAccountTypeDef(TypedDict):
    AccountId: str,
    Result: str,
```

## CreateS3BucketResourceOutputTypeDef

```python
# CreateS3BucketResourceOutputTypeDef definition

class CreateS3BucketResourceOutputTypeDef(TypedDict):
    BucketName: NotRequired[str],
    ObjectPrefixes: NotRequired[List[str]],
```

## DestinationPropertiesTypeDef

```python
# DestinationPropertiesTypeDef definition

class DestinationPropertiesTypeDef(TypedDict):
    DestinationArn: NotRequired[str],
    KmsKeyArn: NotRequired[str],
```

## CreateS3BucketResourceTypeDef

```python
# CreateS3BucketResourceTypeDef definition

class CreateS3BucketResourceTypeDef(TypedDict):
    BucketName: NotRequired[str],
    ObjectPrefixes: NotRequired[Sequence[str]],
```

## CreateSampleFindingsRequestRequestTypeDef

```python
# CreateSampleFindingsRequestRequestTypeDef definition

class CreateSampleFindingsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    FindingTypes: NotRequired[Sequence[str]],
```

## CreateThreatIntelSetRequestRequestTypeDef

```python
# CreateThreatIntelSetRequestRequestTypeDef definition

class CreateThreatIntelSetRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    Name: str,
    Format: ThreatIntelSetFormatType,  # (1)
    Location: str,
    Activate: bool,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ThreatIntelSetFormatType](./literals.md#threatintelsetformattype) 
## DNSLogsConfigurationResultTypeDef

```python
# DNSLogsConfigurationResultTypeDef definition

class DNSLogsConfigurationResultTypeDef(TypedDict):
    Status: DataSourceStatusType,  # (1)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## FlowLogsConfigurationResultTypeDef

```python
# FlowLogsConfigurationResultTypeDef definition

class FlowLogsConfigurationResultTypeDef(TypedDict):
    Status: DataSourceStatusType,  # (1)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## S3LogsConfigurationResultTypeDef

```python
# S3LogsConfigurationResultTypeDef definition

class S3LogsConfigurationResultTypeDef(TypedDict):
    Status: DataSourceStatusType,  # (1)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## S3LogsConfigurationTypeDef

```python
# S3LogsConfigurationTypeDef definition

class S3LogsConfigurationTypeDef(TypedDict):
    Enable: bool,
```

## DataSourceFreeTrialTypeDef

```python
# DataSourceFreeTrialTypeDef definition

class DataSourceFreeTrialTypeDef(TypedDict):
    FreeTrialDaysRemaining: NotRequired[int],
```

## DateStatisticsTypeDef

```python
# DateStatisticsTypeDef definition

class DateStatisticsTypeDef(TypedDict):
    Date: NotRequired[datetime],
    LastGeneratedAt: NotRequired[datetime],
    Severity: NotRequired[float],
    TotalFindings: NotRequired[int],
```

## DeclineInvitationsRequestRequestTypeDef

```python
# DeclineInvitationsRequestRequestTypeDef definition

class DeclineInvitationsRequestRequestTypeDef(TypedDict):
    AccountIds: Sequence[str],
```

## DefaultServerSideEncryptionTypeDef

```python
# DefaultServerSideEncryptionTypeDef definition

class DefaultServerSideEncryptionTypeDef(TypedDict):
    EncryptionType: NotRequired[str],
    KmsMasterKeyArn: NotRequired[str],
```

## DeleteDetectorRequestRequestTypeDef

```python
# DeleteDetectorRequestRequestTypeDef definition

class DeleteDetectorRequestRequestTypeDef(TypedDict):
    DetectorId: str,
```

## DeleteFilterRequestRequestTypeDef

```python
# DeleteFilterRequestRequestTypeDef definition

class DeleteFilterRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    FilterName: str,
```

## DeleteIPSetRequestRequestTypeDef

```python
# DeleteIPSetRequestRequestTypeDef definition

class DeleteIPSetRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    IpSetId: str,
```

## DeleteInvitationsRequestRequestTypeDef

```python
# DeleteInvitationsRequestRequestTypeDef definition

class DeleteInvitationsRequestRequestTypeDef(TypedDict):
    AccountIds: Sequence[str],
```

## DeleteMalwareProtectionPlanRequestRequestTypeDef

```python
# DeleteMalwareProtectionPlanRequestRequestTypeDef definition

class DeleteMalwareProtectionPlanRequestRequestTypeDef(TypedDict):
    MalwareProtectionPlanId: str,
```

## DeleteMembersRequestRequestTypeDef

```python
# DeleteMembersRequestRequestTypeDef definition

class DeleteMembersRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AccountIds: Sequence[str],
```

## DeletePublishingDestinationRequestRequestTypeDef

```python
# DeletePublishingDestinationRequestRequestTypeDef definition

class DeletePublishingDestinationRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    DestinationId: str,
```

## DeleteThreatIntelSetRequestRequestTypeDef

```python
# DeleteThreatIntelSetRequestRequestTypeDef definition

class DeleteThreatIntelSetRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    ThreatIntelSetId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## SortCriteriaTypeDef

```python
# SortCriteriaTypeDef definition

class SortCriteriaTypeDef(TypedDict):
    AttributeName: NotRequired[str],
    OrderBy: NotRequired[OrderByType],  # (1)
```

1. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
## DescribeOrganizationConfigurationRequestRequestTypeDef

```python
# DescribeOrganizationConfigurationRequestRequestTypeDef definition

class DescribeOrganizationConfigurationRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribePublishingDestinationRequestRequestTypeDef

```python
# DescribePublishingDestinationRequestRequestTypeDef definition

class DescribePublishingDestinationRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    DestinationId: str,
```

## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    DestinationId: str,
    DestinationType: DestinationTypeType,  # (1)
    Status: PublishingStatusType,  # (2)
```

1. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype) 
2. See [:material-code-brackets: PublishingStatusType](./literals.md#publishingstatustype) 
## DetectorAdditionalConfigurationResultTypeDef

```python
# DetectorAdditionalConfigurationResultTypeDef definition

class DetectorAdditionalConfigurationResultTypeDef(TypedDict):
    Name: NotRequired[FeatureAdditionalConfigurationType],  # (1)
    Status: NotRequired[FeatureStatusType],  # (2)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: FeatureAdditionalConfigurationType](./literals.md#featureadditionalconfigurationtype) 
2. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## DetectorAdditionalConfigurationTypeDef

```python
# DetectorAdditionalConfigurationTypeDef definition

class DetectorAdditionalConfigurationTypeDef(TypedDict):
    Name: NotRequired[FeatureAdditionalConfigurationType],  # (1)
    Status: NotRequired[FeatureStatusType],  # (2)
```

1. See [:material-code-brackets: FeatureAdditionalConfigurationType](./literals.md#featureadditionalconfigurationtype) 
2. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## DisableOrganizationAdminAccountRequestRequestTypeDef

```python
# DisableOrganizationAdminAccountRequestRequestTypeDef definition

class DisableOrganizationAdminAccountRequestRequestTypeDef(TypedDict):
    AdminAccountId: str,
```

## DisassociateFromAdministratorAccountRequestRequestTypeDef

```python
# DisassociateFromAdministratorAccountRequestRequestTypeDef definition

class DisassociateFromAdministratorAccountRequestRequestTypeDef(TypedDict):
    DetectorId: str,
```

## DisassociateFromMasterAccountRequestRequestTypeDef

```python
# DisassociateFromMasterAccountRequestRequestTypeDef definition

class DisassociateFromMasterAccountRequestRequestTypeDef(TypedDict):
    DetectorId: str,
```

## DisassociateMembersRequestRequestTypeDef

```python
# DisassociateMembersRequestRequestTypeDef definition

class DisassociateMembersRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AccountIds: Sequence[str],
```

## VolumeDetailTypeDef

```python
# VolumeDetailTypeDef definition

class VolumeDetailTypeDef(TypedDict):
    VolumeArn: NotRequired[str],
    VolumeType: NotRequired[str],
    DeviceName: NotRequired[str],
    VolumeSizeInGB: NotRequired[int],
    EncryptionType: NotRequired[str],
    SnapshotArn: NotRequired[str],
    KmsKeyArn: NotRequired[str],
```

## EbsVolumesResultTypeDef

```python
# EbsVolumesResultTypeDef definition

class EbsVolumesResultTypeDef(TypedDict):
    Status: NotRequired[DataSourceStatusType],  # (1)
    Reason: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## IamInstanceProfileTypeDef

```python
# IamInstanceProfileTypeDef definition

class IamInstanceProfileTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
```

## ProductCodeTypeDef

```python
# ProductCodeTypeDef definition

class ProductCodeTypeDef(TypedDict):
    Code: NotRequired[str],
    ProductType: NotRequired[str],
```

## PrivateIpAddressDetailsTypeDef

```python
# PrivateIpAddressDetailsTypeDef definition

class PrivateIpAddressDetailsTypeDef(TypedDict):
    PrivateDnsName: NotRequired[str],
    PrivateIpAddress: NotRequired[str],
```

## SecurityGroupTypeDef

```python
# SecurityGroupTypeDef definition

class SecurityGroupTypeDef(TypedDict):
    GroupId: NotRequired[str],
    GroupName: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## EnableOrganizationAdminAccountRequestRequestTypeDef

```python
# EnableOrganizationAdminAccountRequestRequestTypeDef definition

class EnableOrganizationAdminAccountRequestRequestTypeDef(TypedDict):
    AdminAccountId: str,
```

## ThreatIntelligenceDetailTypeDef

```python
# ThreatIntelligenceDetailTypeDef definition

class ThreatIntelligenceDetailTypeDef(TypedDict):
    ThreatListName: NotRequired[str],
    ThreatNames: NotRequired[List[str]],
    ThreatFileSha256: NotRequired[str],
```

## FilterConditionTypeDef

```python
# FilterConditionTypeDef definition

class FilterConditionTypeDef(TypedDict):
    EqualsValue: NotRequired[str],
    GreaterThan: NotRequired[int],
    LessThan: NotRequired[int],
```

## FindingTypeStatisticsTypeDef

```python
# FindingTypeStatisticsTypeDef definition

class FindingTypeStatisticsTypeDef(TypedDict):
    FindingType: NotRequired[str],
    LastGeneratedAt: NotRequired[datetime],
    TotalFindings: NotRequired[int],
```

## ResourceStatisticsTypeDef

```python
# ResourceStatisticsTypeDef definition

class ResourceStatisticsTypeDef(TypedDict):
    AccountId: NotRequired[str],
    LastGeneratedAt: NotRequired[datetime],
    ResourceId: NotRequired[str],
    ResourceType: NotRequired[str],
    TotalFindings: NotRequired[int],
```

## SeverityStatisticsTypeDef

```python
# SeverityStatisticsTypeDef definition

class SeverityStatisticsTypeDef(TypedDict):
    LastGeneratedAt: NotRequired[datetime],
    Severity: NotRequired[float],
    TotalFindings: NotRequired[int],
```

## GeoLocationTypeDef

```python
# GeoLocationTypeDef definition

class GeoLocationTypeDef(TypedDict):
    Lat: NotRequired[float],
    Lon: NotRequired[float],
```

## GetAdministratorAccountRequestRequestTypeDef

```python
# GetAdministratorAccountRequestRequestTypeDef definition

class GetAdministratorAccountRequestRequestTypeDef(TypedDict):
    DetectorId: str,
```

## GetDetectorRequestRequestTypeDef

```python
# GetDetectorRequestRequestTypeDef definition

class GetDetectorRequestRequestTypeDef(TypedDict):
    DetectorId: str,
```

## GetFilterRequestRequestTypeDef

```python
# GetFilterRequestRequestTypeDef definition

class GetFilterRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    FilterName: str,
```

## GetIPSetRequestRequestTypeDef

```python
# GetIPSetRequestRequestTypeDef definition

class GetIPSetRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    IpSetId: str,
```

## GetMalwareProtectionPlanRequestRequestTypeDef

```python
# GetMalwareProtectionPlanRequestRequestTypeDef definition

class GetMalwareProtectionPlanRequestRequestTypeDef(TypedDict):
    MalwareProtectionPlanId: str,
```

## MalwareProtectionPlanStatusReasonTypeDef

```python
# MalwareProtectionPlanStatusReasonTypeDef definition

class MalwareProtectionPlanStatusReasonTypeDef(TypedDict):
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## GetMalwareScanSettingsRequestRequestTypeDef

```python
# GetMalwareScanSettingsRequestRequestTypeDef definition

class GetMalwareScanSettingsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
```

## GetMasterAccountRequestRequestTypeDef

```python
# GetMasterAccountRequestRequestTypeDef definition

class GetMasterAccountRequestRequestTypeDef(TypedDict):
    DetectorId: str,
```

## MasterTypeDef

```python
# MasterTypeDef definition

class MasterTypeDef(TypedDict):
    AccountId: NotRequired[str],
    InvitationId: NotRequired[str],
    RelationshipStatus: NotRequired[str],
    InvitedAt: NotRequired[str],
```

## GetMemberDetectorsRequestRequestTypeDef

```python
# GetMemberDetectorsRequestRequestTypeDef definition

class GetMemberDetectorsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AccountIds: Sequence[str],
```

## GetMembersRequestRequestTypeDef

```python
# GetMembersRequestRequestTypeDef definition

class GetMembersRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AccountIds: Sequence[str],
```

## MemberTypeDef

```python
# MemberTypeDef definition

class MemberTypeDef(TypedDict):
    AccountId: str,
    MasterId: str,
    Email: str,
    RelationshipStatus: str,
    UpdatedAt: str,
    DetectorId: NotRequired[str],
    InvitedAt: NotRequired[str],
    AdministratorId: NotRequired[str],
```

## GetRemainingFreeTrialDaysRequestRequestTypeDef

```python
# GetRemainingFreeTrialDaysRequestRequestTypeDef definition

class GetRemainingFreeTrialDaysRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AccountIds: NotRequired[Sequence[str]],
```

## GetThreatIntelSetRequestRequestTypeDef

```python
# GetThreatIntelSetRequestRequestTypeDef definition

class GetThreatIntelSetRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    ThreatIntelSetId: str,
```

## UsageCriteriaTypeDef

```python
# UsageCriteriaTypeDef definition

class UsageCriteriaTypeDef(TypedDict):
    AccountIds: NotRequired[Sequence[str]],
    DataSources: NotRequired[Sequence[DataSourceType]],  # (1)
    Resources: NotRequired[Sequence[str]],
    Features: NotRequired[Sequence[UsageFeatureType]],  # (2)
```

1. See [:material-code-brackets: DataSourceType](./literals.md#datasourcetype) 
2. See [:material-code-brackets: UsageFeatureType](./literals.md#usagefeaturetype) 
## HighestSeverityThreatDetailsTypeDef

```python
# HighestSeverityThreatDetailsTypeDef definition

class HighestSeverityThreatDetailsTypeDef(TypedDict):
    Severity: NotRequired[str],
    ThreatName: NotRequired[str],
    Count: NotRequired[int],
```

## HostPathTypeDef

```python
# HostPathTypeDef definition

class HostPathTypeDef(TypedDict):
    Path: NotRequired[str],
```

## ImpersonatedUserTypeDef

```python
# ImpersonatedUserTypeDef definition

class ImpersonatedUserTypeDef(TypedDict):
    Username: NotRequired[str],
    Groups: NotRequired[List[str]],
```

## IndicatorTypeDef

```python
# IndicatorTypeDef definition

class IndicatorTypeDef(TypedDict):
    Key: IndicatorTypeType,  # (1)
    Values: NotRequired[List[str]],
    Title: NotRequired[str],
```

1. See [:material-code-brackets: IndicatorTypeType](./literals.md#indicatortypetype) 
## InvitationTypeDef

```python
# InvitationTypeDef definition

class InvitationTypeDef(TypedDict):
    AccountId: NotRequired[str],
    InvitationId: NotRequired[str],
    RelationshipStatus: NotRequired[str],
    InvitedAt: NotRequired[str],
```

## InviteMembersRequestRequestTypeDef

```python
# InviteMembersRequestRequestTypeDef definition

class InviteMembersRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AccountIds: Sequence[str],
    DisableEmailNotification: NotRequired[bool],
    Message: NotRequired[str],
```

## ItemPathTypeDef

```python
# ItemPathTypeDef definition

class ItemPathTypeDef(TypedDict):
    NestedItemPath: NotRequired[str],
    Hash: NotRequired[str],
```

## KubernetesAuditLogsConfigurationResultTypeDef

```python
# KubernetesAuditLogsConfigurationResultTypeDef definition

class KubernetesAuditLogsConfigurationResultTypeDef(TypedDict):
    Status: DataSourceStatusType,  # (1)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## KubernetesAuditLogsConfigurationTypeDef

```python
# KubernetesAuditLogsConfigurationTypeDef definition

class KubernetesAuditLogsConfigurationTypeDef(TypedDict):
    Enable: bool,
```

## LineageObjectTypeDef

```python
# LineageObjectTypeDef definition

class LineageObjectTypeDef(TypedDict):
    StartTime: NotRequired[datetime],
    NamespacePid: NotRequired[int],
    UserId: NotRequired[int],
    Name: NotRequired[str],
    Pid: NotRequired[int],
    Uuid: NotRequired[str],
    ExecutablePath: NotRequired[str],
    Euid: NotRequired[int],
    ParentUuid: NotRequired[str],
```

## ListDetectorsRequestRequestTypeDef

```python
# ListDetectorsRequestRequestTypeDef definition

class ListDetectorsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListFiltersRequestRequestTypeDef

```python
# ListFiltersRequestRequestTypeDef definition

class ListFiltersRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListIPSetsRequestRequestTypeDef

```python
# ListIPSetsRequestRequestTypeDef definition

class ListIPSetsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListInvitationsRequestRequestTypeDef

```python
# ListInvitationsRequestRequestTypeDef definition

class ListInvitationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListMalwareProtectionPlansRequestRequestTypeDef

```python
# ListMalwareProtectionPlansRequestRequestTypeDef definition

class ListMalwareProtectionPlansRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## MalwareProtectionPlanSummaryTypeDef

```python
# MalwareProtectionPlanSummaryTypeDef definition

class MalwareProtectionPlanSummaryTypeDef(TypedDict):
    MalwareProtectionPlanId: NotRequired[str],
```

## ListMembersRequestRequestTypeDef

```python
# ListMembersRequestRequestTypeDef definition

class ListMembersRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    OnlyAssociated: NotRequired[str],
```

## ListOrganizationAdminAccountsRequestRequestTypeDef

```python
# ListOrganizationAdminAccountsRequestRequestTypeDef definition

class ListOrganizationAdminAccountsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListPublishingDestinationsRequestRequestTypeDef

```python
# ListPublishingDestinationsRequestRequestTypeDef definition

class ListPublishingDestinationsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListThreatIntelSetsRequestRequestTypeDef

```python
# ListThreatIntelSetsRequestRequestTypeDef definition

class ListThreatIntelSetsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## LocalIpDetailsTypeDef

```python
# LocalIpDetailsTypeDef definition

class LocalIpDetailsTypeDef(TypedDict):
    IpAddressV4: NotRequired[str],
    IpAddressV6: NotRequired[str],
```

## LocalPortDetailsTypeDef

```python
# LocalPortDetailsTypeDef definition

class LocalPortDetailsTypeDef(TypedDict):
    Port: NotRequired[int],
    PortName: NotRequired[str],
```

## LoginAttributeTypeDef

```python
# LoginAttributeTypeDef definition

class LoginAttributeTypeDef(TypedDict):
    User: NotRequired[str],
    Application: NotRequired[str],
    FailedLoginAttempts: NotRequired[int],
    SuccessfulLoginAttempts: NotRequired[int],
```

## ScanEc2InstanceWithFindingsTypeDef

```python
# ScanEc2InstanceWithFindingsTypeDef definition

class ScanEc2InstanceWithFindingsTypeDef(TypedDict):
    EbsVolumes: NotRequired[bool],
```

## MalwareProtectionPlanTaggingActionTypeDef

```python
# MalwareProtectionPlanTaggingActionTypeDef definition

class MalwareProtectionPlanTaggingActionTypeDef(TypedDict):
    Status: NotRequired[MalwareProtectionPlanTaggingActionStatusType],  # (1)
```

1. See [:material-code-brackets: MalwareProtectionPlanTaggingActionStatusType](./literals.md#malwareprotectionplantaggingactionstatustype) 
## MemberAdditionalConfigurationResultTypeDef

```python
# MemberAdditionalConfigurationResultTypeDef definition

class MemberAdditionalConfigurationResultTypeDef(TypedDict):
    Name: NotRequired[OrgFeatureAdditionalConfigurationType],  # (1)
    Status: NotRequired[FeatureStatusType],  # (2)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: OrgFeatureAdditionalConfigurationType](./literals.md#orgfeatureadditionalconfigurationtype) 
2. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## MemberAdditionalConfigurationTypeDef

```python
# MemberAdditionalConfigurationTypeDef definition

class MemberAdditionalConfigurationTypeDef(TypedDict):
    Name: NotRequired[OrgFeatureAdditionalConfigurationType],  # (1)
    Status: NotRequired[FeatureStatusType],  # (2)
```

1. See [:material-code-brackets: OrgFeatureAdditionalConfigurationType](./literals.md#orgfeatureadditionalconfigurationtype) 
2. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## RemotePortDetailsTypeDef

```python
# RemotePortDetailsTypeDef definition

class RemotePortDetailsTypeDef(TypedDict):
    Port: NotRequired[int],
    PortName: NotRequired[str],
```

## NetworkConnectionTypeDef

```python
# NetworkConnectionTypeDef definition

class NetworkConnectionTypeDef(TypedDict):
    Direction: NetworkDirectionType,  # (1)
```

1. See [:material-code-brackets: NetworkDirectionType](./literals.md#networkdirectiontype) 
## NetworkGeoLocationTypeDef

```python
# NetworkGeoLocationTypeDef definition

class NetworkGeoLocationTypeDef(TypedDict):
    City: str,
    Country: str,
    Latitude: float,
    Longitude: float,
```

## OrganizationAdditionalConfigurationResultTypeDef

```python
# OrganizationAdditionalConfigurationResultTypeDef definition

class OrganizationAdditionalConfigurationResultTypeDef(TypedDict):
    Name: NotRequired[OrgFeatureAdditionalConfigurationType],  # (1)
    AutoEnable: NotRequired[OrgFeatureStatusType],  # (2)
```

1. See [:material-code-brackets: OrgFeatureAdditionalConfigurationType](./literals.md#orgfeatureadditionalconfigurationtype) 
2. See [:material-code-brackets: OrgFeatureStatusType](./literals.md#orgfeaturestatustype) 
## OrganizationAdditionalConfigurationTypeDef

```python
# OrganizationAdditionalConfigurationTypeDef definition

class OrganizationAdditionalConfigurationTypeDef(TypedDict):
    Name: NotRequired[OrgFeatureAdditionalConfigurationType],  # (1)
    AutoEnable: NotRequired[OrgFeatureStatusType],  # (2)
```

1. See [:material-code-brackets: OrgFeatureAdditionalConfigurationType](./literals.md#orgfeatureadditionalconfigurationtype) 
2. See [:material-code-brackets: OrgFeatureStatusType](./literals.md#orgfeaturestatustype) 
## OrganizationS3LogsConfigurationResultTypeDef

```python
# OrganizationS3LogsConfigurationResultTypeDef definition

class OrganizationS3LogsConfigurationResultTypeDef(TypedDict):
    AutoEnable: bool,
```

## OrganizationS3LogsConfigurationTypeDef

```python
# OrganizationS3LogsConfigurationTypeDef definition

class OrganizationS3LogsConfigurationTypeDef(TypedDict):
    AutoEnable: bool,
```

## OrganizationEbsVolumesResultTypeDef

```python
# OrganizationEbsVolumesResultTypeDef definition

class OrganizationEbsVolumesResultTypeDef(TypedDict):
    AutoEnable: NotRequired[bool],
```

## OrganizationEbsVolumesTypeDef

```python
# OrganizationEbsVolumesTypeDef definition

class OrganizationEbsVolumesTypeDef(TypedDict):
    AutoEnable: NotRequired[bool],
```

## OrganizationFeatureStatisticsAdditionalConfigurationTypeDef

```python
# OrganizationFeatureStatisticsAdditionalConfigurationTypeDef definition

class OrganizationFeatureStatisticsAdditionalConfigurationTypeDef(TypedDict):
    Name: NotRequired[OrgFeatureAdditionalConfigurationType],  # (1)
    EnabledAccountsCount: NotRequired[int],
```

1. See [:material-code-brackets: OrgFeatureAdditionalConfigurationType](./literals.md#orgfeatureadditionalconfigurationtype) 
## OrganizationKubernetesAuditLogsConfigurationResultTypeDef

```python
# OrganizationKubernetesAuditLogsConfigurationResultTypeDef definition

class OrganizationKubernetesAuditLogsConfigurationResultTypeDef(TypedDict):
    AutoEnable: bool,
```

## OrganizationKubernetesAuditLogsConfigurationTypeDef

```python
# OrganizationKubernetesAuditLogsConfigurationTypeDef definition

class OrganizationKubernetesAuditLogsConfigurationTypeDef(TypedDict):
    AutoEnable: bool,
```

## OrganizationTypeDef

```python
# OrganizationTypeDef definition

class OrganizationTypeDef(TypedDict):
    Asn: NotRequired[str],
    AsnOrg: NotRequired[str],
    Isp: NotRequired[str],
    Org: NotRequired[str],
```

## OwnerTypeDef

```python
# OwnerTypeDef definition

class OwnerTypeDef(TypedDict):
    Id: NotRequired[str],
```

## PublicAccessConfigurationTypeDef

```python
# PublicAccessConfigurationTypeDef definition

class PublicAccessConfigurationTypeDef(TypedDict):
    PublicAclAccess: NotRequired[PublicAccessStatusType],  # (1)
    PublicPolicyAccess: NotRequired[PublicAccessStatusType],  # (1)
    PublicAclIgnoreBehavior: NotRequired[PublicAclIgnoreBehaviorType],  # (3)
    PublicBucketRestrictBehavior: NotRequired[PublicBucketRestrictBehaviorType],  # (4)
```

1. See [:material-code-brackets: PublicAccessStatusType](./literals.md#publicaccessstatustype) 
2. See [:material-code-brackets: PublicAccessStatusType](./literals.md#publicaccessstatustype) 
3. See [:material-code-brackets: PublicAclIgnoreBehaviorType](./literals.md#publicaclignorebehaviortype) 
4. See [:material-code-brackets: PublicBucketRestrictBehaviorType](./literals.md#publicbucketrestrictbehaviortype) 
## RdsDbUserDetailsTypeDef

```python
# RdsDbUserDetailsTypeDef definition

class RdsDbUserDetailsTypeDef(TypedDict):
    User: NotRequired[str],
    Application: NotRequired[str],
    Database: NotRequired[str],
    Ssl: NotRequired[str],
    AuthMethod: NotRequired[str],
```

## S3ObjectTypeDef

```python
# S3ObjectTypeDef definition

class S3ObjectTypeDef(TypedDict):
    ETag: NotRequired[str],
    Key: NotRequired[str],
    VersionId: NotRequired[str],
```

## ResourceDetailsTypeDef

```python
# ResourceDetailsTypeDef definition

class ResourceDetailsTypeDef(TypedDict):
    InstanceArn: NotRequired[str],
```

## S3ObjectDetailTypeDef

```python
# S3ObjectDetailTypeDef definition

class S3ObjectDetailTypeDef(TypedDict):
    ObjectArn: NotRequired[str],
    Key: NotRequired[str],
    ETag: NotRequired[str],
    Hash: NotRequired[str],
    VersionId: NotRequired[str],
```

## ScanConditionPairTypeDef

```python
# ScanConditionPairTypeDef definition

class ScanConditionPairTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## ScannedItemCountTypeDef

```python
# ScannedItemCountTypeDef definition

class ScannedItemCountTypeDef(TypedDict):
    TotalGb: NotRequired[int],
    Files: NotRequired[int],
    Volumes: NotRequired[int],
```

## ThreatsDetectedItemCountTypeDef

```python
# ThreatsDetectedItemCountTypeDef definition

class ThreatsDetectedItemCountTypeDef(TypedDict):
    Files: NotRequired[int],
```

## ScanFilePathTypeDef

```python
# ScanFilePathTypeDef definition

class ScanFilePathTypeDef(TypedDict):
    FilePath: NotRequired[str],
    VolumeArn: NotRequired[str],
    Hash: NotRequired[str],
    FileName: NotRequired[str],
```

## ScanResultDetailsTypeDef

```python
# ScanResultDetailsTypeDef definition

class ScanResultDetailsTypeDef(TypedDict):
    ScanResult: NotRequired[ScanResultType],  # (1)
```

1. See [:material-code-brackets: ScanResultType](./literals.md#scanresulttype) 
## TriggerDetailsTypeDef

```python
# TriggerDetailsTypeDef definition

class TriggerDetailsTypeDef(TypedDict):
    GuardDutyFindingId: NotRequired[str],
    Description: NotRequired[str],
```

## ServiceAdditionalInfoTypeDef

```python
# ServiceAdditionalInfoTypeDef definition

class ServiceAdditionalInfoTypeDef(TypedDict):
    Value: NotRequired[str],
    Type: NotRequired[str],
```

## StartMalwareScanRequestRequestTypeDef

```python
# StartMalwareScanRequestRequestTypeDef definition

class StartMalwareScanRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## StartMonitoringMembersRequestRequestTypeDef

```python
# StartMonitoringMembersRequestRequestTypeDef definition

class StartMonitoringMembersRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AccountIds: Sequence[str],
```

## StopMonitoringMembersRequestRequestTypeDef

```python
# StopMonitoringMembersRequestRequestTypeDef definition

class StopMonitoringMembersRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AccountIds: Sequence[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## TotalTypeDef

```python
# TotalTypeDef definition

class TotalTypeDef(TypedDict):
    Amount: NotRequired[str],
    Unit: NotRequired[str],
```

## UnarchiveFindingsRequestRequestTypeDef

```python
# UnarchiveFindingsRequestRequestTypeDef definition

class UnarchiveFindingsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    FindingIds: Sequence[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateFindingsFeedbackRequestRequestTypeDef

```python
# UpdateFindingsFeedbackRequestRequestTypeDef definition

class UpdateFindingsFeedbackRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    FindingIds: Sequence[str],
    Feedback: FeedbackType,  # (1)
    Comments: NotRequired[str],
```

1. See [:material-code-brackets: FeedbackType](./literals.md#feedbacktype) 
## UpdateIPSetRequestRequestTypeDef

```python
# UpdateIPSetRequestRequestTypeDef definition

class UpdateIPSetRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    IpSetId: str,
    Name: NotRequired[str],
    Location: NotRequired[str],
    Activate: NotRequired[bool],
```

## UpdateS3BucketResourceTypeDef

```python
# UpdateS3BucketResourceTypeDef definition

class UpdateS3BucketResourceTypeDef(TypedDict):
    ObjectPrefixes: NotRequired[Sequence[str]],
```

## UpdateThreatIntelSetRequestRequestTypeDef

```python
# UpdateThreatIntelSetRequestRequestTypeDef definition

class UpdateThreatIntelSetRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    ThreatIntelSetId: str,
    Name: NotRequired[str],
    Location: NotRequired[str],
    Activate: NotRequired[bool],
```

## CreateMembersRequestRequestTypeDef

```python
# CreateMembersRequestRequestTypeDef definition

class CreateMembersRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AccountDetails: Sequence[AccountDetailTypeDef],  # (1)
```

1. See [:material-code-braces: AccountDetailTypeDef](./type_defs.md#accountdetailtypedef) 
## AccountLevelPermissionsTypeDef

```python
# AccountLevelPermissionsTypeDef definition

class AccountLevelPermissionsTypeDef(TypedDict):
    BlockPublicAccess: NotRequired[BlockPublicAccessTypeDef],  # (1)
```

1. See [:material-code-braces: BlockPublicAccessTypeDef](./type_defs.md#blockpublicaccesstypedef) 
## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    Name: str,
    Uid: str,
    Type: str,
    CredentialUid: NotRequired[str],
    Account: NotRequired[AccountTypeDef],  # (1)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
## CoverageEksClusterDetailsTypeDef

```python
# CoverageEksClusterDetailsTypeDef definition

class CoverageEksClusterDetailsTypeDef(TypedDict):
    ClusterName: NotRequired[str],
    CoveredNodes: NotRequired[int],
    CompatibleNodes: NotRequired[int],
    AddonDetails: NotRequired[AddonDetailsTypeDef],  # (1)
    ManagementType: NotRequired[ManagementTypeType],  # (2)
```

1. See [:material-code-braces: AddonDetailsTypeDef](./type_defs.md#addondetailstypedef) 
2. See [:material-code-brackets: ManagementTypeType](./literals.md#managementtypetype) 
## CoverageEc2InstanceDetailsTypeDef

```python
# CoverageEc2InstanceDetailsTypeDef definition

class CoverageEc2InstanceDetailsTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    InstanceType: NotRequired[str],
    ClusterArn: NotRequired[str],
    AgentDetails: NotRequired[AgentDetailsTypeDef],  # (1)
    ManagementType: NotRequired[ManagementTypeType],  # (2)
```

1. See [:material-code-braces: AgentDetailsTypeDef](./type_defs.md#agentdetailstypedef) 
2. See [:material-code-brackets: ManagementTypeType](./literals.md#managementtypetype) 
## AnomalyObjectTypeDef

```python
# AnomalyObjectTypeDef definition

class AnomalyObjectTypeDef(TypedDict):
    ProfileType: NotRequired[ProfileTypeType],  # (1)
    ProfileSubtype: NotRequired[ProfileSubtypeType],  # (2)
    Observations: NotRequired[ObservationsTypeDef],  # (3)
```

1. See [:material-code-brackets: ProfileTypeType](./literals.md#profiletypetype) 
2. See [:material-code-brackets: ProfileSubtypeType](./literals.md#profilesubtypetype) 
3. See [:material-code-braces: ObservationsTypeDef](./type_defs.md#observationstypedef) 
## BucketLevelPermissionsTypeDef

```python
# BucketLevelPermissionsTypeDef definition

class BucketLevelPermissionsTypeDef(TypedDict):
    AccessControlList: NotRequired[AccessControlListTypeDef],  # (1)
    BucketPolicy: NotRequired[BucketPolicyTypeDef],  # (2)
    BlockPublicAccess: NotRequired[BlockPublicAccessTypeDef],  # (3)
```

1. See [:material-code-braces: AccessControlListTypeDef](./type_defs.md#accesscontrollisttypedef) 
2. See [:material-code-braces: BucketPolicyTypeDef](./type_defs.md#bucketpolicytypedef) 
3. See [:material-code-braces: BlockPublicAccessTypeDef](./type_defs.md#blockpublicaccesstypedef) 
## FindingCriteriaOutputTypeDef

```python
# FindingCriteriaOutputTypeDef definition

class FindingCriteriaOutputTypeDef(TypedDict):
    Criterion: NotRequired[Dict[str, ConditionOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: ConditionOutputTypeDef](./type_defs.md#conditionoutputtypedef) 
## ContainerTypeDef

```python
# ContainerTypeDef definition

class ContainerTypeDef(TypedDict):
    ContainerRuntime: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    Image: NotRequired[str],
    ImagePrefix: NotRequired[str],
    VolumeMounts: NotRequired[List[VolumeMountTypeDef]],  # (1)
    SecurityContext: NotRequired[SecurityContextTypeDef],  # (2)
```

1. See [:material-code-braces: VolumeMountTypeDef](./type_defs.md#volumemounttypedef) 
2. See [:material-code-braces: SecurityContextTypeDef](./type_defs.md#securitycontexttypedef) 
## CoverageEcsClusterDetailsTypeDef

```python
# CoverageEcsClusterDetailsTypeDef definition

class CoverageEcsClusterDetailsTypeDef(TypedDict):
    ClusterName: NotRequired[str],
    FargateDetails: NotRequired[FargateDetailsTypeDef],  # (1)
    ContainerInstanceDetails: NotRequired[ContainerInstanceDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: FargateDetailsTypeDef](./type_defs.md#fargatedetailstypedef) 
2. See [:material-code-braces: ContainerInstanceDetailsTypeDef](./type_defs.md#containerinstancedetailstypedef) 
## CoverageFilterCriterionTypeDef

```python
# CoverageFilterCriterionTypeDef definition

class CoverageFilterCriterionTypeDef(TypedDict):
    CriterionKey: NotRequired[CoverageFilterCriterionKeyType],  # (1)
    FilterCondition: NotRequired[CoverageFilterConditionTypeDef],  # (2)
```

1. See [:material-code-brackets: CoverageFilterCriterionKeyType](./literals.md#coveragefiltercriterionkeytype) 
2. See [:material-code-braces: CoverageFilterConditionTypeDef](./type_defs.md#coveragefilterconditiontypedef) 
## CreateFilterResponseTypeDef

```python
# CreateFilterResponseTypeDef definition

class CreateFilterResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIPSetResponseTypeDef

```python
# CreateIPSetResponseTypeDef definition

class CreateIPSetResponseTypeDef(TypedDict):
    IpSetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMalwareProtectionPlanResponseTypeDef

```python
# CreateMalwareProtectionPlanResponseTypeDef definition

class CreateMalwareProtectionPlanResponseTypeDef(TypedDict):
    MalwareProtectionPlanId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePublishingDestinationResponseTypeDef

```python
# CreatePublishingDestinationResponseTypeDef definition

class CreatePublishingDestinationResponseTypeDef(TypedDict):
    DestinationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateThreatIntelSetResponseTypeDef

```python
# CreateThreatIntelSetResponseTypeDef definition

class CreateThreatIntelSetResponseTypeDef(TypedDict):
    ThreatIntelSetId: str,
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
## GetAdministratorAccountResponseTypeDef

```python
# GetAdministratorAccountResponseTypeDef definition

class GetAdministratorAccountResponseTypeDef(TypedDict):
    Administrator: AdministratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AdministratorTypeDef](./type_defs.md#administratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCoverageStatisticsResponseTypeDef

```python
# GetCoverageStatisticsResponseTypeDef definition

class GetCoverageStatisticsResponseTypeDef(TypedDict):
    CoverageStatistics: CoverageStatisticsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CoverageStatisticsTypeDef](./type_defs.md#coveragestatisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIPSetResponseTypeDef

```python
# GetIPSetResponseTypeDef definition

class GetIPSetResponseTypeDef(TypedDict):
    Name: str,
    Format: IpSetFormatType,  # (1)
    Location: str,
    Status: IpSetStatusType,  # (2)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: IpSetFormatType](./literals.md#ipsetformattype) 
2. See [:material-code-brackets: IpSetStatusType](./literals.md#ipsetstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInvitationsCountResponseTypeDef

```python
# GetInvitationsCountResponseTypeDef definition

class GetInvitationsCountResponseTypeDef(TypedDict):
    InvitationsCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetThreatIntelSetResponseTypeDef

```python
# GetThreatIntelSetResponseTypeDef definition

class GetThreatIntelSetResponseTypeDef(TypedDict):
    Name: str,
    Format: ThreatIntelSetFormatType,  # (1)
    Location: str,
    Status: ThreatIntelSetStatusType,  # (2)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ThreatIntelSetFormatType](./literals.md#threatintelsetformattype) 
2. See [:material-code-brackets: ThreatIntelSetStatusType](./literals.md#threatintelsetstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDetectorsResponseTypeDef

```python
# ListDetectorsResponseTypeDef definition

class ListDetectorsResponseTypeDef(TypedDict):
    DetectorIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFiltersResponseTypeDef

```python
# ListFiltersResponseTypeDef definition

class ListFiltersResponseTypeDef(TypedDict):
    FilterNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFindingsResponseTypeDef

```python
# ListFindingsResponseTypeDef definition

class ListFindingsResponseTypeDef(TypedDict):
    FindingIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIPSetsResponseTypeDef

```python
# ListIPSetsResponseTypeDef definition

class ListIPSetsResponseTypeDef(TypedDict):
    IpSetIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOrganizationAdminAccountsResponseTypeDef

```python
# ListOrganizationAdminAccountsResponseTypeDef definition

class ListOrganizationAdminAccountsResponseTypeDef(TypedDict):
    AdminAccounts: List[AdminAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AdminAccountTypeDef](./type_defs.md#adminaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThreatIntelSetsResponseTypeDef

```python
# ListThreatIntelSetsResponseTypeDef definition

class ListThreatIntelSetsResponseTypeDef(TypedDict):
    ThreatIntelSetIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMalwareScanResponseTypeDef

```python
# StartMalwareScanResponseTypeDef definition

class StartMalwareScanResponseTypeDef(TypedDict):
    ScanId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFilterResponseTypeDef

```python
# UpdateFilterResponseTypeDef definition

class UpdateFilterResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMembersResponseTypeDef

```python
# CreateMembersResponseTypeDef definition

class CreateMembersResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeclineInvitationsResponseTypeDef

```python
# DeclineInvitationsResponseTypeDef definition

class DeclineInvitationsResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInvitationsResponseTypeDef

```python
# DeleteInvitationsResponseTypeDef definition

class DeleteInvitationsResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMembersResponseTypeDef

```python
# DeleteMembersResponseTypeDef definition

class DeleteMembersResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateMembersResponseTypeDef

```python
# DisassociateMembersResponseTypeDef definition

class DisassociateMembersResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InviteMembersResponseTypeDef

```python
# InviteMembersResponseTypeDef definition

class InviteMembersResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMonitoringMembersResponseTypeDef

```python
# StartMonitoringMembersResponseTypeDef definition

class StartMonitoringMembersResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopMonitoringMembersResponseTypeDef

```python
# StopMonitoringMembersResponseTypeDef definition

class StopMonitoringMembersResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMemberDetectorsResponseTypeDef

```python
# UpdateMemberDetectorsResponseTypeDef definition

class UpdateMemberDetectorsResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProtectedResourceOutputTypeDef

```python
# CreateProtectedResourceOutputTypeDef definition

class CreateProtectedResourceOutputTypeDef(TypedDict):
    S3Bucket: NotRequired[CreateS3BucketResourceOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CreateS3BucketResourceOutputTypeDef](./type_defs.md#creates3bucketresourceoutputtypedef) 
## CreatePublishingDestinationRequestRequestTypeDef

```python
# CreatePublishingDestinationRequestRequestTypeDef definition

class CreatePublishingDestinationRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    DestinationType: DestinationTypeType,  # (1)
    DestinationProperties: DestinationPropertiesTypeDef,  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype) 
2. See [:material-code-braces: DestinationPropertiesTypeDef](./type_defs.md#destinationpropertiestypedef) 
## DescribePublishingDestinationResponseTypeDef

```python
# DescribePublishingDestinationResponseTypeDef definition

class DescribePublishingDestinationResponseTypeDef(TypedDict):
    DestinationId: str,
    DestinationType: DestinationTypeType,  # (1)
    Status: PublishingStatusType,  # (2)
    PublishingFailureStartTimestamp: int,
    DestinationProperties: DestinationPropertiesTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype) 
2. See [:material-code-brackets: PublishingStatusType](./literals.md#publishingstatustype) 
3. See [:material-code-braces: DestinationPropertiesTypeDef](./type_defs.md#destinationpropertiestypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePublishingDestinationRequestRequestTypeDef

```python
# UpdatePublishingDestinationRequestRequestTypeDef definition

class UpdatePublishingDestinationRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    DestinationId: str,
    DestinationProperties: NotRequired[DestinationPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: DestinationPropertiesTypeDef](./type_defs.md#destinationpropertiestypedef) 
## KubernetesDataSourceFreeTrialTypeDef

```python
# KubernetesDataSourceFreeTrialTypeDef definition

class KubernetesDataSourceFreeTrialTypeDef(TypedDict):
    AuditLogs: NotRequired[DataSourceFreeTrialTypeDef],  # (1)
```

1. See [:material-code-braces: DataSourceFreeTrialTypeDef](./type_defs.md#datasourcefreetrialtypedef) 
## MalwareProtectionDataSourceFreeTrialTypeDef

```python
# MalwareProtectionDataSourceFreeTrialTypeDef definition

class MalwareProtectionDataSourceFreeTrialTypeDef(TypedDict):
    ScanEc2InstanceWithFindings: NotRequired[DataSourceFreeTrialTypeDef],  # (1)
```

1. See [:material-code-braces: DataSourceFreeTrialTypeDef](./type_defs.md#datasourcefreetrialtypedef) 
## ListDetectorsRequestPaginateTypeDef

```python
# ListDetectorsRequestPaginateTypeDef definition

class ListDetectorsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFiltersRequestPaginateTypeDef

```python
# ListFiltersRequestPaginateTypeDef definition

class ListFiltersRequestPaginateTypeDef(TypedDict):
    DetectorId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIPSetsRequestPaginateTypeDef

```python
# ListIPSetsRequestPaginateTypeDef definition

class ListIPSetsRequestPaginateTypeDef(TypedDict):
    DetectorId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInvitationsRequestPaginateTypeDef

```python
# ListInvitationsRequestPaginateTypeDef definition

class ListInvitationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembersRequestPaginateTypeDef

```python
# ListMembersRequestPaginateTypeDef definition

class ListMembersRequestPaginateTypeDef(TypedDict):
    DetectorId: str,
    OnlyAssociated: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrganizationAdminAccountsRequestPaginateTypeDef

```python
# ListOrganizationAdminAccountsRequestPaginateTypeDef definition

class ListOrganizationAdminAccountsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThreatIntelSetsRequestPaginateTypeDef

```python
# ListThreatIntelSetsRequestPaginateTypeDef definition

class ListThreatIntelSetsRequestPaginateTypeDef(TypedDict):
    DetectorId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetFindingsRequestRequestTypeDef

```python
# GetFindingsRequestRequestTypeDef definition

class GetFindingsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    FindingIds: Sequence[str],
    SortCriteria: NotRequired[SortCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
## ListPublishingDestinationsResponseTypeDef

```python
# ListPublishingDestinationsResponseTypeDef definition

class ListPublishingDestinationsResponseTypeDef(TypedDict):
    Destinations: List[DestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectorFeatureConfigurationResultTypeDef

```python
# DetectorFeatureConfigurationResultTypeDef definition

class DetectorFeatureConfigurationResultTypeDef(TypedDict):
    Name: NotRequired[DetectorFeatureResultType],  # (1)
    Status: NotRequired[FeatureStatusType],  # (2)
    UpdatedAt: NotRequired[datetime],
    AdditionalConfiguration: NotRequired[List[DetectorAdditionalConfigurationResultTypeDef]],  # (3)
```

1. See [:material-code-brackets: DetectorFeatureResultType](./literals.md#detectorfeatureresulttype) 
2. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
3. See [:material-code-braces: DetectorAdditionalConfigurationResultTypeDef](./type_defs.md#detectoradditionalconfigurationresulttypedef) 
## DetectorFeatureConfigurationTypeDef

```python
# DetectorFeatureConfigurationTypeDef definition

class DetectorFeatureConfigurationTypeDef(TypedDict):
    Name: NotRequired[DetectorFeatureType],  # (1)
    Status: NotRequired[FeatureStatusType],  # (2)
    AdditionalConfiguration: NotRequired[Sequence[DetectorAdditionalConfigurationTypeDef]],  # (3)
```

1. See [:material-code-brackets: DetectorFeatureType](./literals.md#detectorfeaturetype) 
2. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
3. See [:material-code-braces: DetectorAdditionalConfigurationTypeDef](./type_defs.md#detectoradditionalconfigurationtypedef) 
## EbsVolumeDetailsTypeDef

```python
# EbsVolumeDetailsTypeDef definition

class EbsVolumeDetailsTypeDef(TypedDict):
    ScannedVolumeDetails: NotRequired[List[VolumeDetailTypeDef]],  # (1)
    SkippedVolumeDetails: NotRequired[List[VolumeDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: VolumeDetailTypeDef](./type_defs.md#volumedetailtypedef) 
2. See [:material-code-braces: VolumeDetailTypeDef](./type_defs.md#volumedetailtypedef) 
## ScanEc2InstanceWithFindingsResultTypeDef

```python
# ScanEc2InstanceWithFindingsResultTypeDef definition

class ScanEc2InstanceWithFindingsResultTypeDef(TypedDict):
    EbsVolumes: NotRequired[EbsVolumesResultTypeDef],  # (1)
```

1. See [:material-code-braces: EbsVolumesResultTypeDef](./type_defs.md#ebsvolumesresulttypedef) 
## Ec2InstanceTypeDef

```python
# Ec2InstanceTypeDef definition

class Ec2InstanceTypeDef(TypedDict):
    AvailabilityZone: NotRequired[str],
    ImageDescription: NotRequired[str],
    InstanceState: NotRequired[str],
    IamInstanceProfile: NotRequired[IamInstanceProfileTypeDef],  # (1)
    InstanceType: NotRequired[str],
    OutpostArn: NotRequired[str],
    Platform: NotRequired[str],
    ProductCodes: NotRequired[List[ProductCodeTypeDef]],  # (2)
    Ec2NetworkInterfaceUids: NotRequired[List[str]],
```

1. See [:material-code-braces: IamInstanceProfileTypeDef](./type_defs.md#iaminstanceprofiletypedef) 
2. See [:material-code-braces: ProductCodeTypeDef](./type_defs.md#productcodetypedef) 
## Ec2NetworkInterfaceTypeDef

```python
# Ec2NetworkInterfaceTypeDef definition

class Ec2NetworkInterfaceTypeDef(TypedDict):
    Ipv6Addresses: NotRequired[List[str]],
    PrivateIpAddresses: NotRequired[List[PrivateIpAddressDetailsTypeDef]],  # (1)
    PublicIp: NotRequired[str],
    SecurityGroups: NotRequired[List[SecurityGroupTypeDef]],  # (2)
    SubNetId: NotRequired[str],
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: PrivateIpAddressDetailsTypeDef](./type_defs.md#privateipaddressdetailstypedef) 
2. See [:material-code-braces: SecurityGroupTypeDef](./type_defs.md#securitygrouptypedef) 
## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    Ipv6Addresses: NotRequired[List[str]],
    NetworkInterfaceId: NotRequired[str],
    PrivateDnsName: NotRequired[str],
    PrivateIpAddress: NotRequired[str],
    PrivateIpAddresses: NotRequired[List[PrivateIpAddressDetailsTypeDef]],  # (1)
    PublicDnsName: NotRequired[str],
    PublicIp: NotRequired[str],
    SecurityGroups: NotRequired[List[SecurityGroupTypeDef]],  # (2)
    SubnetId: NotRequired[str],
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: PrivateIpAddressDetailsTypeDef](./type_defs.md#privateipaddressdetailstypedef) 
2. See [:material-code-braces: SecurityGroupTypeDef](./type_defs.md#securitygrouptypedef) 
## VpcConfigTypeDef

```python
# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    SubnetIds: NotRequired[List[str]],
    VpcId: NotRequired[str],
    SecurityGroups: NotRequired[List[SecurityGroupTypeDef]],  # (1)
```

1. See [:material-code-braces: SecurityGroupTypeDef](./type_defs.md#securitygrouptypedef) 
## EksClusterDetailsTypeDef

```python
# EksClusterDetailsTypeDef definition

class EksClusterDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    VpcId: NotRequired[str],
    Status: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    CreatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RdsDbInstanceDetailsTypeDef

```python
# RdsDbInstanceDetailsTypeDef definition

class RdsDbInstanceDetailsTypeDef(TypedDict):
    DbInstanceIdentifier: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    DbClusterIdentifier: NotRequired[str],
    DbInstanceArn: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RdsLimitlessDbDetailsTypeDef

```python
# RdsLimitlessDbDetailsTypeDef definition

class RdsLimitlessDbDetailsTypeDef(TypedDict):
    DbShardGroupIdentifier: NotRequired[str],
    DbShardGroupResourceId: NotRequired[str],
    DbShardGroupArn: NotRequired[str],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    DbClusterIdentifier: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## EvidenceTypeDef

```python
# EvidenceTypeDef definition

class EvidenceTypeDef(TypedDict):
    ThreatIntelligenceDetails: NotRequired[List[ThreatIntelligenceDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: ThreatIntelligenceDetailTypeDef](./type_defs.md#threatintelligencedetailtypedef) 
## FilterCriterionTypeDef

```python
# FilterCriterionTypeDef definition

class FilterCriterionTypeDef(TypedDict):
    CriterionKey: NotRequired[CriterionKeyType],  # (1)
    FilterCondition: NotRequired[FilterConditionTypeDef],  # (2)
```

1. See [:material-code-brackets: CriterionKeyType](./literals.md#criterionkeytype) 
2. See [:material-code-braces: FilterConditionTypeDef](./type_defs.md#filterconditiontypedef) 
## FindingStatisticsTypeDef

```python
# FindingStatisticsTypeDef definition

class FindingStatisticsTypeDef(TypedDict):
    CountBySeverity: NotRequired[Dict[str, int]],
    GroupedByAccount: NotRequired[List[AccountStatisticsTypeDef]],  # (1)
    GroupedByDate: NotRequired[List[DateStatisticsTypeDef]],  # (2)
    GroupedByFindingType: NotRequired[List[FindingTypeStatisticsTypeDef]],  # (3)
    GroupedByResource: NotRequired[List[ResourceStatisticsTypeDef]],  # (4)
    GroupedBySeverity: NotRequired[List[SeverityStatisticsTypeDef]],  # (5)
```

1. See [:material-code-braces: AccountStatisticsTypeDef](./type_defs.md#accountstatisticstypedef) 
2. See [:material-code-braces: DateStatisticsTypeDef](./type_defs.md#datestatisticstypedef) 
3. See [:material-code-braces: FindingTypeStatisticsTypeDef](./type_defs.md#findingtypestatisticstypedef) 
4. See [:material-code-braces: ResourceStatisticsTypeDef](./type_defs.md#resourcestatisticstypedef) 
5. See [:material-code-braces: SeverityStatisticsTypeDef](./type_defs.md#severitystatisticstypedef) 
## GetMasterAccountResponseTypeDef

```python
# GetMasterAccountResponseTypeDef definition

class GetMasterAccountResponseTypeDef(TypedDict):
    Master: MasterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MasterTypeDef](./type_defs.md#mastertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMembersResponseTypeDef

```python
# GetMembersResponseTypeDef definition

class GetMembersResponseTypeDef(TypedDict):
    Members: List[MemberTypeDef],  # (1)
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
2. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMembersResponseTypeDef

```python
# ListMembersResponseTypeDef definition

class ListMembersResponseTypeDef(TypedDict):
    Members: List[MemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUsageStatisticsRequestRequestTypeDef

```python
# GetUsageStatisticsRequestRequestTypeDef definition

class GetUsageStatisticsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    UsageStatisticType: UsageStatisticTypeType,  # (1)
    UsageCriteria: UsageCriteriaTypeDef,  # (2)
    Unit: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: UsageStatisticTypeType](./literals.md#usagestatistictypetype) 
2. See [:material-code-braces: UsageCriteriaTypeDef](./type_defs.md#usagecriteriatypedef) 
## VolumeTypeDef

```python
# VolumeTypeDef definition

class VolumeTypeDef(TypedDict):
    Name: NotRequired[str],
    HostPath: NotRequired[HostPathTypeDef],  # (1)
```

1. See [:material-code-braces: HostPathTypeDef](./type_defs.md#hostpathtypedef) 
## KubernetesUserDetailsTypeDef

```python
# KubernetesUserDetailsTypeDef definition

class KubernetesUserDetailsTypeDef(TypedDict):
    Username: NotRequired[str],
    Uid: NotRequired[str],
    Groups: NotRequired[List[str]],
    SessionName: NotRequired[List[str]],
    ImpersonatedUser: NotRequired[ImpersonatedUserTypeDef],  # (1)
```

1. See [:material-code-braces: ImpersonatedUserTypeDef](./type_defs.md#impersonatedusertypedef) 
## SignalTypeDef

```python
# SignalTypeDef definition

class SignalTypeDef(TypedDict):
    Uid: str,
    Type: SignalTypeType,  # (1)
    Name: str,
    CreatedAt: datetime,
    UpdatedAt: datetime,
    FirstSeenAt: datetime,
    LastSeenAt: datetime,
    Count: int,
    Description: NotRequired[str],
    Severity: NotRequired[float],
    ResourceUids: NotRequired[List[str]],
    ActorIds: NotRequired[List[str]],
    EndpointIds: NotRequired[List[str]],
    SignalIndicators: NotRequired[List[IndicatorTypeDef]],  # (2)
```

1. See [:material-code-brackets: SignalTypeType](./literals.md#signaltypetype) 
2. See [:material-code-braces: IndicatorTypeDef](./type_defs.md#indicatortypedef) 
## ListInvitationsResponseTypeDef

```python
# ListInvitationsResponseTypeDef definition

class ListInvitationsResponseTypeDef(TypedDict):
    Invitations: List[InvitationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InvitationTypeDef](./type_defs.md#invitationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ThreatTypeDef

```python
# ThreatTypeDef definition

class ThreatTypeDef(TypedDict):
    Name: NotRequired[str],
    Source: NotRequired[str],
    ItemPaths: NotRequired[List[ItemPathTypeDef]],  # (1)
```

1. See [:material-code-braces: ItemPathTypeDef](./type_defs.md#itempathtypedef) 
## KubernetesConfigurationResultTypeDef

```python
# KubernetesConfigurationResultTypeDef definition

class KubernetesConfigurationResultTypeDef(TypedDict):
    AuditLogs: KubernetesAuditLogsConfigurationResultTypeDef,  # (1)
```

1. See [:material-code-braces: KubernetesAuditLogsConfigurationResultTypeDef](./type_defs.md#kubernetesauditlogsconfigurationresulttypedef) 
## KubernetesConfigurationTypeDef

```python
# KubernetesConfigurationTypeDef definition

class KubernetesConfigurationTypeDef(TypedDict):
    AuditLogs: KubernetesAuditLogsConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: KubernetesAuditLogsConfigurationTypeDef](./type_defs.md#kubernetesauditlogsconfigurationtypedef) 
## ProcessDetailsTypeDef

```python
# ProcessDetailsTypeDef definition

class ProcessDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    ExecutablePath: NotRequired[str],
    ExecutableSha256: NotRequired[str],
    NamespacePid: NotRequired[int],
    Pwd: NotRequired[str],
    Pid: NotRequired[int],
    StartTime: NotRequired[datetime],
    Uuid: NotRequired[str],
    ParentUuid: NotRequired[str],
    User: NotRequired[str],
    UserId: NotRequired[int],
    Euid: NotRequired[int],
    Lineage: NotRequired[List[LineageObjectTypeDef]],  # (1)
```

1. See [:material-code-braces: LineageObjectTypeDef](./type_defs.md#lineageobjecttypedef) 
## ListMalwareProtectionPlansResponseTypeDef

```python
# ListMalwareProtectionPlansResponseTypeDef definition

class ListMalwareProtectionPlansResponseTypeDef(TypedDict):
    MalwareProtectionPlans: List[MalwareProtectionPlanSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MalwareProtectionPlanSummaryTypeDef](./type_defs.md#malwareprotectionplansummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MalwareProtectionConfigurationTypeDef

```python
# MalwareProtectionConfigurationTypeDef definition

class MalwareProtectionConfigurationTypeDef(TypedDict):
    ScanEc2InstanceWithFindings: NotRequired[ScanEc2InstanceWithFindingsTypeDef],  # (1)
```

1. See [:material-code-braces: ScanEc2InstanceWithFindingsTypeDef](./type_defs.md#scanec2instancewithfindingstypedef) 
## MalwareProtectionPlanActionsTypeDef

```python
# MalwareProtectionPlanActionsTypeDef definition

class MalwareProtectionPlanActionsTypeDef(TypedDict):
    Tagging: NotRequired[MalwareProtectionPlanTaggingActionTypeDef],  # (1)
```

1. See [:material-code-braces: MalwareProtectionPlanTaggingActionTypeDef](./type_defs.md#malwareprotectionplantaggingactiontypedef) 
## MemberFeaturesConfigurationResultTypeDef

```python
# MemberFeaturesConfigurationResultTypeDef definition

class MemberFeaturesConfigurationResultTypeDef(TypedDict):
    Name: NotRequired[OrgFeatureType],  # (1)
    Status: NotRequired[FeatureStatusType],  # (2)
    UpdatedAt: NotRequired[datetime],
    AdditionalConfiguration: NotRequired[List[MemberAdditionalConfigurationResultTypeDef]],  # (3)
```

1. See [:material-code-brackets: OrgFeatureType](./literals.md#orgfeaturetype) 
2. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
3. See [:material-code-braces: MemberAdditionalConfigurationResultTypeDef](./type_defs.md#memberadditionalconfigurationresulttypedef) 
## MemberFeaturesConfigurationTypeDef

```python
# MemberFeaturesConfigurationTypeDef definition

class MemberFeaturesConfigurationTypeDef(TypedDict):
    Name: NotRequired[OrgFeatureType],  # (1)
    Status: NotRequired[FeatureStatusType],  # (2)
    AdditionalConfiguration: NotRequired[Sequence[MemberAdditionalConfigurationTypeDef]],  # (3)
```

1. See [:material-code-brackets: OrgFeatureType](./literals.md#orgfeaturetype) 
2. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
3. See [:material-code-braces: MemberAdditionalConfigurationTypeDef](./type_defs.md#memberadditionalconfigurationtypedef) 
## NetworkEndpointTypeDef

```python
# NetworkEndpointTypeDef definition

class NetworkEndpointTypeDef(TypedDict):
    Id: str,
    Ip: NotRequired[str],
    Domain: NotRequired[str],
    Port: NotRequired[int],
    Location: NotRequired[NetworkGeoLocationTypeDef],  # (1)
    AutonomousSystem: NotRequired[AutonomousSystemTypeDef],  # (2)
    Connection: NotRequired[NetworkConnectionTypeDef],  # (3)
```

1. See [:material-code-braces: NetworkGeoLocationTypeDef](./type_defs.md#networkgeolocationtypedef) 
2. See [:material-code-braces: AutonomousSystemTypeDef](./type_defs.md#autonomoussystemtypedef) 
3. See [:material-code-braces: NetworkConnectionTypeDef](./type_defs.md#networkconnectiontypedef) 
## OrganizationFeatureConfigurationResultTypeDef

```python
# OrganizationFeatureConfigurationResultTypeDef definition

class OrganizationFeatureConfigurationResultTypeDef(TypedDict):
    Name: NotRequired[OrgFeatureType],  # (1)
    AutoEnable: NotRequired[OrgFeatureStatusType],  # (2)
    AdditionalConfiguration: NotRequired[List[OrganizationAdditionalConfigurationResultTypeDef]],  # (3)
```

1. See [:material-code-brackets: OrgFeatureType](./literals.md#orgfeaturetype) 
2. See [:material-code-brackets: OrgFeatureStatusType](./literals.md#orgfeaturestatustype) 
3. See [:material-code-braces: OrganizationAdditionalConfigurationResultTypeDef](./type_defs.md#organizationadditionalconfigurationresulttypedef) 
## OrganizationFeatureConfigurationTypeDef

```python
# OrganizationFeatureConfigurationTypeDef definition

class OrganizationFeatureConfigurationTypeDef(TypedDict):
    Name: NotRequired[OrgFeatureType],  # (1)
    AutoEnable: NotRequired[OrgFeatureStatusType],  # (2)
    AdditionalConfiguration: NotRequired[Sequence[OrganizationAdditionalConfigurationTypeDef]],  # (3)
```

1. See [:material-code-brackets: OrgFeatureType](./literals.md#orgfeaturetype) 
2. See [:material-code-brackets: OrgFeatureStatusType](./literals.md#orgfeaturestatustype) 
3. See [:material-code-braces: OrganizationAdditionalConfigurationTypeDef](./type_defs.md#organizationadditionalconfigurationtypedef) 
## OrganizationScanEc2InstanceWithFindingsResultTypeDef

```python
# OrganizationScanEc2InstanceWithFindingsResultTypeDef definition

class OrganizationScanEc2InstanceWithFindingsResultTypeDef(TypedDict):
    EbsVolumes: NotRequired[OrganizationEbsVolumesResultTypeDef],  # (1)
```

1. See [:material-code-braces: OrganizationEbsVolumesResultTypeDef](./type_defs.md#organizationebsvolumesresulttypedef) 
## OrganizationScanEc2InstanceWithFindingsTypeDef

```python
# OrganizationScanEc2InstanceWithFindingsTypeDef definition

class OrganizationScanEc2InstanceWithFindingsTypeDef(TypedDict):
    EbsVolumes: NotRequired[OrganizationEbsVolumesTypeDef],  # (1)
```

1. See [:material-code-braces: OrganizationEbsVolumesTypeDef](./type_defs.md#organizationebsvolumestypedef) 
## OrganizationFeatureStatisticsTypeDef

```python
# OrganizationFeatureStatisticsTypeDef definition

class OrganizationFeatureStatisticsTypeDef(TypedDict):
    Name: NotRequired[OrgFeatureType],  # (1)
    EnabledAccountsCount: NotRequired[int],
    AdditionalConfiguration: NotRequired[List[OrganizationFeatureStatisticsAdditionalConfigurationTypeDef]],  # (2)
```

1. See [:material-code-brackets: OrgFeatureType](./literals.md#orgfeaturetype) 
2. See [:material-code-braces: OrganizationFeatureStatisticsAdditionalConfigurationTypeDef](./type_defs.md#organizationfeaturestatisticsadditionalconfigurationtypedef) 
## OrganizationKubernetesConfigurationResultTypeDef

```python
# OrganizationKubernetesConfigurationResultTypeDef definition

class OrganizationKubernetesConfigurationResultTypeDef(TypedDict):
    AuditLogs: OrganizationKubernetesAuditLogsConfigurationResultTypeDef,  # (1)
```

1. See [:material-code-braces: OrganizationKubernetesAuditLogsConfigurationResultTypeDef](./type_defs.md#organizationkubernetesauditlogsconfigurationresulttypedef) 
## OrganizationKubernetesConfigurationTypeDef

```python
# OrganizationKubernetesConfigurationTypeDef definition

class OrganizationKubernetesConfigurationTypeDef(TypedDict):
    AuditLogs: OrganizationKubernetesAuditLogsConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: OrganizationKubernetesAuditLogsConfigurationTypeDef](./type_defs.md#organizationkubernetesauditlogsconfigurationtypedef) 
## RemoteIpDetailsTypeDef

```python
# RemoteIpDetailsTypeDef definition

class RemoteIpDetailsTypeDef(TypedDict):
    City: NotRequired[CityTypeDef],  # (1)
    Country: NotRequired[CountryTypeDef],  # (2)
    GeoLocation: NotRequired[GeoLocationTypeDef],  # (3)
    IpAddressV4: NotRequired[str],
    IpAddressV6: NotRequired[str],
    Organization: NotRequired[OrganizationTypeDef],  # (4)
```

1. See [:material-code-braces: CityTypeDef](./type_defs.md#citytypedef) 
2. See [:material-code-braces: CountryTypeDef](./type_defs.md#countrytypedef) 
3. See [:material-code-braces: GeoLocationTypeDef](./type_defs.md#geolocationtypedef) 
4. See [:material-code-braces: OrganizationTypeDef](./type_defs.md#organizationtypedef) 
## S3BucketTypeDef

```python
# S3BucketTypeDef definition

class S3BucketTypeDef(TypedDict):
    OwnerId: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    EncryptionType: NotRequired[str],
    EncryptionKeyArn: NotRequired[str],
    EffectivePermission: NotRequired[str],
    PublicReadAccess: NotRequired[PublicAccessStatusType],  # (1)
    PublicWriteAccess: NotRequired[PublicAccessStatusType],  # (1)
    AccountPublicAccess: NotRequired[PublicAccessConfigurationTypeDef],  # (3)
    BucketPublicAccess: NotRequired[PublicAccessConfigurationTypeDef],  # (3)
    S3ObjectUids: NotRequired[List[str]],
```

1. See [:material-code-brackets: PublicAccessStatusType](./literals.md#publicaccessstatustype) 
2. See [:material-code-brackets: PublicAccessStatusType](./literals.md#publicaccessstatustype) 
3. See [:material-code-braces: PublicAccessConfigurationTypeDef](./type_defs.md#publicaccessconfigurationtypedef) 
4. See [:material-code-braces: PublicAccessConfigurationTypeDef](./type_defs.md#publicaccessconfigurationtypedef) 
## ScanConditionOutputTypeDef

```python
# ScanConditionOutputTypeDef definition

class ScanConditionOutputTypeDef(TypedDict):
    MapEquals: List[ScanConditionPairTypeDef],  # (1)
```

1. See [:material-code-braces: ScanConditionPairTypeDef](./type_defs.md#scanconditionpairtypedef) 
## ScanConditionTypeDef

```python
# ScanConditionTypeDef definition

class ScanConditionTypeDef(TypedDict):
    MapEquals: Sequence[ScanConditionPairTypeDef],  # (1)
```

1. See [:material-code-braces: ScanConditionPairTypeDef](./type_defs.md#scanconditionpairtypedef) 
## ScanThreatNameTypeDef

```python
# ScanThreatNameTypeDef definition

class ScanThreatNameTypeDef(TypedDict):
    Name: NotRequired[str],
    Severity: NotRequired[str],
    ItemCount: NotRequired[int],
    FilePaths: NotRequired[List[ScanFilePathTypeDef]],  # (1)
```

1. See [:material-code-braces: ScanFilePathTypeDef](./type_defs.md#scanfilepathtypedef) 
## ScanTypeDef

```python
# ScanTypeDef definition

class ScanTypeDef(TypedDict):
    DetectorId: NotRequired[str],
    AdminDetectorId: NotRequired[str],
    ScanId: NotRequired[str],
    ScanStatus: NotRequired[ScanStatusType],  # (1)
    FailureReason: NotRequired[str],
    ScanStartTime: NotRequired[datetime],
    ScanEndTime: NotRequired[datetime],
    TriggerDetails: NotRequired[TriggerDetailsTypeDef],  # (2)
    ResourceDetails: NotRequired[ResourceDetailsTypeDef],  # (3)
    ScanResultDetails: NotRequired[ScanResultDetailsTypeDef],  # (4)
    AccountId: NotRequired[str],
    TotalBytes: NotRequired[int],
    FileCount: NotRequired[int],
    AttachedVolumes: NotRequired[List[VolumeDetailTypeDef]],  # (5)
    ScanType: NotRequired[ScanTypeType],  # (6)
```

1. See [:material-code-brackets: ScanStatusType](./literals.md#scanstatustype) 
2. See [:material-code-braces: TriggerDetailsTypeDef](./type_defs.md#triggerdetailstypedef) 
3. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
4. See [:material-code-braces: ScanResultDetailsTypeDef](./type_defs.md#scanresultdetailstypedef) 
5. See [:material-code-braces: VolumeDetailTypeDef](./type_defs.md#volumedetailtypedef) 
6. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
## UsageAccountResultTypeDef

```python
# UsageAccountResultTypeDef definition

class UsageAccountResultTypeDef(TypedDict):
    AccountId: NotRequired[str],
    Total: NotRequired[TotalTypeDef],  # (1)
```

1. See [:material-code-braces: TotalTypeDef](./type_defs.md#totaltypedef) 
## UsageDataSourceResultTypeDef

```python
# UsageDataSourceResultTypeDef definition

class UsageDataSourceResultTypeDef(TypedDict):
    DataSource: NotRequired[DataSourceType],  # (1)
    Total: NotRequired[TotalTypeDef],  # (2)
```

1. See [:material-code-brackets: DataSourceType](./literals.md#datasourcetype) 
2. See [:material-code-braces: TotalTypeDef](./type_defs.md#totaltypedef) 
## UsageFeatureResultTypeDef

```python
# UsageFeatureResultTypeDef definition

class UsageFeatureResultTypeDef(TypedDict):
    Feature: NotRequired[UsageFeatureType],  # (1)
    Total: NotRequired[TotalTypeDef],  # (2)
```

1. See [:material-code-brackets: UsageFeatureType](./literals.md#usagefeaturetype) 
2. See [:material-code-braces: TotalTypeDef](./type_defs.md#totaltypedef) 
## UsageResourceResultTypeDef

```python
# UsageResourceResultTypeDef definition

class UsageResourceResultTypeDef(TypedDict):
    Resource: NotRequired[str],
    Total: NotRequired[TotalTypeDef],  # (1)
```

1. See [:material-code-braces: TotalTypeDef](./type_defs.md#totaltypedef) 
## UsageTopAccountResultTypeDef

```python
# UsageTopAccountResultTypeDef definition

class UsageTopAccountResultTypeDef(TypedDict):
    AccountId: NotRequired[str],
    Total: NotRequired[TotalTypeDef],  # (1)
```

1. See [:material-code-braces: TotalTypeDef](./type_defs.md#totaltypedef) 
## UpdateProtectedResourceTypeDef

```python
# UpdateProtectedResourceTypeDef definition

class UpdateProtectedResourceTypeDef(TypedDict):
    S3Bucket: NotRequired[UpdateS3BucketResourceTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateS3BucketResourceTypeDef](./type_defs.md#updates3bucketresourcetypedef) 
## ActorTypeDef

```python
# ActorTypeDef definition

class ActorTypeDef(TypedDict):
    Id: str,
    User: NotRequired[UserTypeDef],  # (1)
    Session: NotRequired[SessionTypeDef],  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
## AnomalyUnusualTypeDef

```python
# AnomalyUnusualTypeDef definition

class AnomalyUnusualTypeDef(TypedDict):
    Behavior: NotRequired[Dict[str, Dict[str, AnomalyObjectTypeDef]]],  # (1)
```

1. See [:material-code-braces: AnomalyObjectTypeDef](./type_defs.md#anomalyobjecttypedef) 
## PermissionConfigurationTypeDef

```python
# PermissionConfigurationTypeDef definition

class PermissionConfigurationTypeDef(TypedDict):
    BucketLevelPermissions: NotRequired[BucketLevelPermissionsTypeDef],  # (1)
    AccountLevelPermissions: NotRequired[AccountLevelPermissionsTypeDef],  # (2)
```

1. See [:material-code-braces: BucketLevelPermissionsTypeDef](./type_defs.md#bucketlevelpermissionstypedef) 
2. See [:material-code-braces: AccountLevelPermissionsTypeDef](./type_defs.md#accountlevelpermissionstypedef) 
## GetFilterResponseTypeDef

```python
# GetFilterResponseTypeDef definition

class GetFilterResponseTypeDef(TypedDict):
    Name: str,
    Description: str,
    Action: FilterActionType,  # (1)
    Rank: int,
    FindingCriteria: FindingCriteriaOutputTypeDef,  # (2)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: FindingCriteriaOutputTypeDef](./type_defs.md#findingcriteriaoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FindingCriteriaTypeDef

```python
# FindingCriteriaTypeDef definition

class FindingCriteriaTypeDef(TypedDict):
    Criterion: NotRequired[Mapping[str, ConditionUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) [:material-code-braces: ConditionOutputTypeDef](./type_defs.md#conditionoutputtypedef) 
## CoverageResourceDetailsTypeDef

```python
# CoverageResourceDetailsTypeDef definition

class CoverageResourceDetailsTypeDef(TypedDict):
    EksClusterDetails: NotRequired[CoverageEksClusterDetailsTypeDef],  # (1)
    ResourceType: NotRequired[ResourceTypeType],  # (2)
    EcsClusterDetails: NotRequired[CoverageEcsClusterDetailsTypeDef],  # (3)
    Ec2InstanceDetails: NotRequired[CoverageEc2InstanceDetailsTypeDef],  # (4)
```

1. See [:material-code-braces: CoverageEksClusterDetailsTypeDef](./type_defs.md#coverageeksclusterdetailstypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: CoverageEcsClusterDetailsTypeDef](./type_defs.md#coverageecsclusterdetailstypedef) 
4. See [:material-code-braces: CoverageEc2InstanceDetailsTypeDef](./type_defs.md#coverageec2instancedetailstypedef) 
## CoverageFilterCriteriaTypeDef

```python
# CoverageFilterCriteriaTypeDef definition

class CoverageFilterCriteriaTypeDef(TypedDict):
    FilterCriterion: NotRequired[Sequence[CoverageFilterCriterionTypeDef]],  # (1)
```

1. See [:material-code-braces: CoverageFilterCriterionTypeDef](./type_defs.md#coveragefiltercriteriontypedef) 
## CreateProtectedResourceTypeDef

```python
# CreateProtectedResourceTypeDef definition

class CreateProtectedResourceTypeDef(TypedDict):
    S3Bucket: NotRequired[CreateS3BucketResourceUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CreateS3BucketResourceTypeDef](./type_defs.md#creates3bucketresourcetypedef) [:material-code-braces: CreateS3BucketResourceOutputTypeDef](./type_defs.md#creates3bucketresourceoutputtypedef) 
## DataSourcesFreeTrialTypeDef

```python
# DataSourcesFreeTrialTypeDef definition

class DataSourcesFreeTrialTypeDef(TypedDict):
    CloudTrail: NotRequired[DataSourceFreeTrialTypeDef],  # (1)
    DnsLogs: NotRequired[DataSourceFreeTrialTypeDef],  # (1)
    FlowLogs: NotRequired[DataSourceFreeTrialTypeDef],  # (1)
    S3Logs: NotRequired[DataSourceFreeTrialTypeDef],  # (1)
    Kubernetes: NotRequired[KubernetesDataSourceFreeTrialTypeDef],  # (5)
    MalwareProtection: NotRequired[MalwareProtectionDataSourceFreeTrialTypeDef],  # (6)
```

1. See [:material-code-braces: DataSourceFreeTrialTypeDef](./type_defs.md#datasourcefreetrialtypedef) 
2. See [:material-code-braces: DataSourceFreeTrialTypeDef](./type_defs.md#datasourcefreetrialtypedef) 
3. See [:material-code-braces: DataSourceFreeTrialTypeDef](./type_defs.md#datasourcefreetrialtypedef) 
4. See [:material-code-braces: DataSourceFreeTrialTypeDef](./type_defs.md#datasourcefreetrialtypedef) 
5. See [:material-code-braces: KubernetesDataSourceFreeTrialTypeDef](./type_defs.md#kubernetesdatasourcefreetrialtypedef) 
6. See [:material-code-braces: MalwareProtectionDataSourceFreeTrialTypeDef](./type_defs.md#malwareprotectiondatasourcefreetrialtypedef) 
## MalwareProtectionConfigurationResultTypeDef

```python
# MalwareProtectionConfigurationResultTypeDef definition

class MalwareProtectionConfigurationResultTypeDef(TypedDict):
    ScanEc2InstanceWithFindings: NotRequired[ScanEc2InstanceWithFindingsResultTypeDef],  # (1)
    ServiceRole: NotRequired[str],
```

1. See [:material-code-braces: ScanEc2InstanceWithFindingsResultTypeDef](./type_defs.md#scanec2instancewithfindingsresulttypedef) 
## InstanceDetailsTypeDef

```python
# InstanceDetailsTypeDef definition

class InstanceDetailsTypeDef(TypedDict):
    AvailabilityZone: NotRequired[str],
    IamInstanceProfile: NotRequired[IamInstanceProfileTypeDef],  # (1)
    ImageDescription: NotRequired[str],
    ImageId: NotRequired[str],
    InstanceId: NotRequired[str],
    InstanceState: NotRequired[str],
    InstanceType: NotRequired[str],
    OutpostArn: NotRequired[str],
    LaunchTime: NotRequired[str],
    NetworkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (2)
    Platform: NotRequired[str],
    ProductCodes: NotRequired[List[ProductCodeTypeDef]],  # (3)
    Tags: NotRequired[List[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: IamInstanceProfileTypeDef](./type_defs.md#iaminstanceprofiletypedef) 
2. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
3. See [:material-code-braces: ProductCodeTypeDef](./type_defs.md#productcodetypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## LambdaDetailsTypeDef

```python
# LambdaDetailsTypeDef definition

class LambdaDetailsTypeDef(TypedDict):
    FunctionArn: NotRequired[str],
    FunctionName: NotRequired[str],
    Description: NotRequired[str],
    LastModifiedAt: NotRequired[datetime],
    RevisionId: NotRequired[str],
    FunctionVersion: NotRequired[str],
    Role: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (1)
    Tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## FilterCriteriaTypeDef

```python
# FilterCriteriaTypeDef definition

class FilterCriteriaTypeDef(TypedDict):
    FilterCriterion: NotRequired[Sequence[FilterCriterionTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterCriterionTypeDef](./type_defs.md#filtercriteriontypedef) 
## GetFindingsStatisticsResponseTypeDef

```python
# GetFindingsStatisticsResponseTypeDef definition

class GetFindingsStatisticsResponseTypeDef(TypedDict):
    FindingStatistics: FindingStatisticsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FindingStatisticsTypeDef](./type_defs.md#findingstatisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EcsTaskDetailsTypeDef

```python
# EcsTaskDetailsTypeDef definition

class EcsTaskDetailsTypeDef(TypedDict):
    Arn: NotRequired[str],
    DefinitionArn: NotRequired[str],
    Version: NotRequired[str],
    TaskCreatedAt: NotRequired[datetime],
    StartedAt: NotRequired[datetime],
    StartedBy: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    Volumes: NotRequired[List[VolumeTypeDef]],  # (2)
    Containers: NotRequired[List[ContainerTypeDef]],  # (3)
    Group: NotRequired[str],
    LaunchType: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
3. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) 
## KubernetesWorkloadDetailsTypeDef

```python
# KubernetesWorkloadDetailsTypeDef definition

class KubernetesWorkloadDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[str],
    Uid: NotRequired[str],
    Namespace: NotRequired[str],
    HostNetwork: NotRequired[bool],
    Containers: NotRequired[List[ContainerTypeDef]],  # (1)
    Volumes: NotRequired[List[VolumeTypeDef]],  # (2)
    ServiceAccountName: NotRequired[str],
    HostIPC: NotRequired[bool],
    HostPID: NotRequired[bool],
```

1. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) 
2. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
## MalwareScanDetailsTypeDef

```python
# MalwareScanDetailsTypeDef definition

class MalwareScanDetailsTypeDef(TypedDict):
    Threats: NotRequired[List[ThreatTypeDef]],  # (1)
```

1. See [:material-code-braces: ThreatTypeDef](./type_defs.md#threattypedef) 
## RuntimeContextTypeDef

```python
# RuntimeContextTypeDef definition

class RuntimeContextTypeDef(TypedDict):
    ModifyingProcess: NotRequired[ProcessDetailsTypeDef],  # (1)
    ModifiedAt: NotRequired[datetime],
    ScriptPath: NotRequired[str],
    LibraryPath: NotRequired[str],
    LdPreloadValue: NotRequired[str],
    SocketPath: NotRequired[str],
    RuncBinaryPath: NotRequired[str],
    ReleaseAgentPath: NotRequired[str],
    MountSource: NotRequired[str],
    MountTarget: NotRequired[str],
    FileSystemType: NotRequired[str],
    Flags: NotRequired[List[str]],
    ModuleName: NotRequired[str],
    ModuleFilePath: NotRequired[str],
    ModuleSha256: NotRequired[str],
    ShellHistoryFilePath: NotRequired[str],
    TargetProcess: NotRequired[ProcessDetailsTypeDef],  # (1)
    AddressFamily: NotRequired[str],
    IanaProtocolNumber: NotRequired[int],
    MemoryRegions: NotRequired[List[str]],
    ToolName: NotRequired[str],
    ToolCategory: NotRequired[str],
    ServiceName: NotRequired[str],
    CommandLineExample: NotRequired[str],
    ThreatFilePath: NotRequired[str],
```

1. See [:material-code-braces: ProcessDetailsTypeDef](./type_defs.md#processdetailstypedef) 
2. See [:material-code-braces: ProcessDetailsTypeDef](./type_defs.md#processdetailstypedef) 
## DataSourceConfigurationsTypeDef

```python
# DataSourceConfigurationsTypeDef definition

class DataSourceConfigurationsTypeDef(TypedDict):
    S3Logs: NotRequired[S3LogsConfigurationTypeDef],  # (1)
    Kubernetes: NotRequired[KubernetesConfigurationTypeDef],  # (2)
    MalwareProtection: NotRequired[MalwareProtectionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: S3LogsConfigurationTypeDef](./type_defs.md#s3logsconfigurationtypedef) 
2. See [:material-code-braces: KubernetesConfigurationTypeDef](./type_defs.md#kubernetesconfigurationtypedef) 
3. See [:material-code-braces: MalwareProtectionConfigurationTypeDef](./type_defs.md#malwareprotectionconfigurationtypedef) 
## GetMalwareProtectionPlanResponseTypeDef

```python
# GetMalwareProtectionPlanResponseTypeDef definition

class GetMalwareProtectionPlanResponseTypeDef(TypedDict):
    Arn: str,
    Role: str,
    ProtectedResource: CreateProtectedResourceOutputTypeDef,  # (1)
    Actions: MalwareProtectionPlanActionsTypeDef,  # (2)
    CreatedAt: datetime,
    Status: MalwareProtectionPlanStatusType,  # (3)
    StatusReasons: List[MalwareProtectionPlanStatusReasonTypeDef],  # (4)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: CreateProtectedResourceOutputTypeDef](./type_defs.md#createprotectedresourceoutputtypedef) 
2. See [:material-code-braces: MalwareProtectionPlanActionsTypeDef](./type_defs.md#malwareprotectionplanactionstypedef) 
3. See [:material-code-brackets: MalwareProtectionPlanStatusType](./literals.md#malwareprotectionplanstatustype) 
4. See [:material-code-braces: MalwareProtectionPlanStatusReasonTypeDef](./type_defs.md#malwareprotectionplanstatusreasontypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OrganizationMalwareProtectionConfigurationResultTypeDef

```python
# OrganizationMalwareProtectionConfigurationResultTypeDef definition

class OrganizationMalwareProtectionConfigurationResultTypeDef(TypedDict):
    ScanEc2InstanceWithFindings: NotRequired[OrganizationScanEc2InstanceWithFindingsResultTypeDef],  # (1)
```

1. See [:material-code-braces: OrganizationScanEc2InstanceWithFindingsResultTypeDef](./type_defs.md#organizationscanec2instancewithfindingsresulttypedef) 
## OrganizationMalwareProtectionConfigurationTypeDef

```python
# OrganizationMalwareProtectionConfigurationTypeDef definition

class OrganizationMalwareProtectionConfigurationTypeDef(TypedDict):
    ScanEc2InstanceWithFindings: NotRequired[OrganizationScanEc2InstanceWithFindingsTypeDef],  # (1)
```

1. See [:material-code-braces: OrganizationScanEc2InstanceWithFindingsTypeDef](./type_defs.md#organizationscanec2instancewithfindingstypedef) 
## OrganizationStatisticsTypeDef

```python
# OrganizationStatisticsTypeDef definition

class OrganizationStatisticsTypeDef(TypedDict):
    TotalAccountsCount: NotRequired[int],
    MemberAccountsCount: NotRequired[int],
    ActiveAccountsCount: NotRequired[int],
    EnabledAccountsCount: NotRequired[int],
    CountByFeature: NotRequired[List[OrganizationFeatureStatisticsTypeDef]],  # (1)
```

1. See [:material-code-braces: OrganizationFeatureStatisticsTypeDef](./type_defs.md#organizationfeaturestatisticstypedef) 
## AwsApiCallActionTypeDef

```python
# AwsApiCallActionTypeDef definition

class AwsApiCallActionTypeDef(TypedDict):
    Api: NotRequired[str],
    CallerType: NotRequired[str],
    DomainDetails: NotRequired[DomainDetailsTypeDef],  # (1)
    ErrorCode: NotRequired[str],
    UserAgent: NotRequired[str],
    RemoteIpDetails: NotRequired[RemoteIpDetailsTypeDef],  # (2)
    ServiceName: NotRequired[str],
    RemoteAccountDetails: NotRequired[RemoteAccountDetailsTypeDef],  # (3)
    AffectedResources: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DomainDetailsTypeDef](./type_defs.md#domaindetailstypedef) 
2. See [:material-code-braces: RemoteIpDetailsTypeDef](./type_defs.md#remoteipdetailstypedef) 
3. See [:material-code-braces: RemoteAccountDetailsTypeDef](./type_defs.md#remoteaccountdetailstypedef) 
## KubernetesApiCallActionTypeDef

```python
# KubernetesApiCallActionTypeDef definition

class KubernetesApiCallActionTypeDef(TypedDict):
    RequestUri: NotRequired[str],
    Verb: NotRequired[str],
    SourceIps: NotRequired[List[str]],
    UserAgent: NotRequired[str],
    RemoteIpDetails: NotRequired[RemoteIpDetailsTypeDef],  # (1)
    StatusCode: NotRequired[int],
    Parameters: NotRequired[str],
    Resource: NotRequired[str],
    Subresource: NotRequired[str],
    Namespace: NotRequired[str],
    ResourceName: NotRequired[str],
```

1. See [:material-code-braces: RemoteIpDetailsTypeDef](./type_defs.md#remoteipdetailstypedef) 
## NetworkConnectionActionTypeDef

```python
# NetworkConnectionActionTypeDef definition

class NetworkConnectionActionTypeDef(TypedDict):
    Blocked: NotRequired[bool],
    ConnectionDirection: NotRequired[str],
    LocalPortDetails: NotRequired[LocalPortDetailsTypeDef],  # (1)
    Protocol: NotRequired[str],
    LocalIpDetails: NotRequired[LocalIpDetailsTypeDef],  # (2)
    LocalNetworkInterface: NotRequired[str],
    RemoteIpDetails: NotRequired[RemoteIpDetailsTypeDef],  # (3)
    RemotePortDetails: NotRequired[RemotePortDetailsTypeDef],  # (4)
```

1. See [:material-code-braces: LocalPortDetailsTypeDef](./type_defs.md#localportdetailstypedef) 
2. See [:material-code-braces: LocalIpDetailsTypeDef](./type_defs.md#localipdetailstypedef) 
3. See [:material-code-braces: RemoteIpDetailsTypeDef](./type_defs.md#remoteipdetailstypedef) 
4. See [:material-code-braces: RemotePortDetailsTypeDef](./type_defs.md#remoteportdetailstypedef) 
## PortProbeDetailTypeDef

```python
# PortProbeDetailTypeDef definition

class PortProbeDetailTypeDef(TypedDict):
    LocalPortDetails: NotRequired[LocalPortDetailsTypeDef],  # (1)
    LocalIpDetails: NotRequired[LocalIpDetailsTypeDef],  # (2)
    RemoteIpDetails: NotRequired[RemoteIpDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: LocalPortDetailsTypeDef](./type_defs.md#localportdetailstypedef) 
2. See [:material-code-braces: LocalIpDetailsTypeDef](./type_defs.md#localipdetailstypedef) 
3. See [:material-code-braces: RemoteIpDetailsTypeDef](./type_defs.md#remoteipdetailstypedef) 
## RdsLoginAttemptActionTypeDef

```python
# RdsLoginAttemptActionTypeDef definition

class RdsLoginAttemptActionTypeDef(TypedDict):
    RemoteIpDetails: NotRequired[RemoteIpDetailsTypeDef],  # (1)
    LoginAttributes: NotRequired[List[LoginAttributeTypeDef]],  # (2)
```

1. See [:material-code-braces: RemoteIpDetailsTypeDef](./type_defs.md#remoteipdetailstypedef) 
2. See [:material-code-braces: LoginAttributeTypeDef](./type_defs.md#loginattributetypedef) 
## ResourceDataTypeDef

```python
# ResourceDataTypeDef definition

class ResourceDataTypeDef(TypedDict):
    S3Bucket: NotRequired[S3BucketTypeDef],  # (1)
    Ec2Instance: NotRequired[Ec2InstanceTypeDef],  # (2)
    AccessKey: NotRequired[AccessKeyTypeDef],  # (3)
    Ec2NetworkInterface: NotRequired[Ec2NetworkInterfaceTypeDef],  # (4)
    S3Object: NotRequired[S3ObjectTypeDef],  # (5)
```

1. See [:material-code-braces: S3BucketTypeDef](./type_defs.md#s3buckettypedef) 
2. See [:material-code-braces: Ec2InstanceTypeDef](./type_defs.md#ec2instancetypedef) 
3. See [:material-code-braces: AccessKeyTypeDef](./type_defs.md#accesskeytypedef) 
4. See [:material-code-braces: Ec2NetworkInterfaceTypeDef](./type_defs.md#ec2networkinterfacetypedef) 
5. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## ScanResourceCriteriaOutputTypeDef

```python
# ScanResourceCriteriaOutputTypeDef definition

class ScanResourceCriteriaOutputTypeDef(TypedDict):
    Include: NotRequired[Dict[ScanCriterionKeyType, ScanConditionOutputTypeDef]],  # (1)
    Exclude: NotRequired[Dict[ScanCriterionKeyType, ScanConditionOutputTypeDef]],  # (1)
```

1. See [:material-code-brackets: ScanCriterionKeyType](./literals.md#scancriterionkeytype) [:material-code-braces: ScanConditionOutputTypeDef](./type_defs.md#scanconditionoutputtypedef) 
2. See [:material-code-brackets: ScanCriterionKeyType](./literals.md#scancriterionkeytype) [:material-code-braces: ScanConditionOutputTypeDef](./type_defs.md#scanconditionoutputtypedef) 
## ThreatDetectedByNameTypeDef

```python
# ThreatDetectedByNameTypeDef definition

class ThreatDetectedByNameTypeDef(TypedDict):
    ItemCount: NotRequired[int],
    UniqueThreatNameCount: NotRequired[int],
    Shortened: NotRequired[bool],
    ThreatNames: NotRequired[List[ScanThreatNameTypeDef]],  # (1)
```

1. See [:material-code-braces: ScanThreatNameTypeDef](./type_defs.md#scanthreatnametypedef) 
## DescribeMalwareScansResponseTypeDef

```python
# DescribeMalwareScansResponseTypeDef definition

class DescribeMalwareScansResponseTypeDef(TypedDict):
    Scans: List[ScanTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScanTypeDef](./type_defs.md#scantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UsageTopAccountsResultTypeDef

```python
# UsageTopAccountsResultTypeDef definition

class UsageTopAccountsResultTypeDef(TypedDict):
    Feature: NotRequired[UsageFeatureType],  # (1)
    Accounts: NotRequired[List[UsageTopAccountResultTypeDef]],  # (2)
```

1. See [:material-code-brackets: UsageFeatureType](./literals.md#usagefeaturetype) 
2. See [:material-code-braces: UsageTopAccountResultTypeDef](./type_defs.md#usagetopaccountresulttypedef) 
## UpdateMalwareProtectionPlanRequestRequestTypeDef

```python
# UpdateMalwareProtectionPlanRequestRequestTypeDef definition

class UpdateMalwareProtectionPlanRequestRequestTypeDef(TypedDict):
    MalwareProtectionPlanId: str,
    Role: NotRequired[str],
    Actions: NotRequired[MalwareProtectionPlanActionsTypeDef],  # (1)
    ProtectedResource: NotRequired[UpdateProtectedResourceTypeDef],  # (2)
```

1. See [:material-code-braces: MalwareProtectionPlanActionsTypeDef](./type_defs.md#malwareprotectionplanactionstypedef) 
2. See [:material-code-braces: UpdateProtectedResourceTypeDef](./type_defs.md#updateprotectedresourcetypedef) 
## AnomalyTypeDef

```python
# AnomalyTypeDef definition

class AnomalyTypeDef(TypedDict):
    Profiles: NotRequired[Dict[str, Dict[str, List[AnomalyObjectTypeDef]]]],  # (1)
    Unusual: NotRequired[AnomalyUnusualTypeDef],  # (2)
```

1. See [:material-code-braces: AnomalyObjectTypeDef](./type_defs.md#anomalyobjecttypedef) 
2. See [:material-code-braces: AnomalyUnusualTypeDef](./type_defs.md#anomalyunusualtypedef) 
## PublicAccessTypeDef

```python
# PublicAccessTypeDef definition

class PublicAccessTypeDef(TypedDict):
    PermissionConfiguration: NotRequired[PermissionConfigurationTypeDef],  # (1)
    EffectivePermission: NotRequired[str],
```

1. See [:material-code-braces: PermissionConfigurationTypeDef](./type_defs.md#permissionconfigurationtypedef) 
## CreateFilterRequestRequestTypeDef

```python
# CreateFilterRequestRequestTypeDef definition

class CreateFilterRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    Name: str,
    FindingCriteria: FindingCriteriaTypeDef,  # (1)
    Description: NotRequired[str],
    Action: NotRequired[FilterActionType],  # (2)
    Rank: NotRequired[int],
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef) 
2. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
## GetFindingsStatisticsRequestRequestTypeDef

```python
# GetFindingsStatisticsRequestRequestTypeDef definition

class GetFindingsStatisticsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    FindingStatisticTypes: NotRequired[Sequence[FindingStatisticTypeType]],  # (1)
    FindingCriteria: NotRequired[FindingCriteriaTypeDef],  # (2)
    GroupBy: NotRequired[GroupByTypeType],  # (3)
    OrderBy: NotRequired[OrderByType],  # (4)
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: FindingStatisticTypeType](./literals.md#findingstatistictypetype) 
2. See [:material-code-braces: FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef) 
3. See [:material-code-brackets: GroupByTypeType](./literals.md#groupbytypetype) 
4. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
## ListFindingsRequestPaginateTypeDef

```python
# ListFindingsRequestPaginateTypeDef definition

class ListFindingsRequestPaginateTypeDef(TypedDict):
    DetectorId: str,
    FindingCriteria: NotRequired[FindingCriteriaTypeDef],  # (1)
    SortCriteria: NotRequired[SortCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFindingsRequestRequestTypeDef

```python
# ListFindingsRequestRequestTypeDef definition

class ListFindingsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    FindingCriteria: NotRequired[FindingCriteriaTypeDef],  # (1)
    SortCriteria: NotRequired[SortCriteriaTypeDef],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
## UpdateFilterRequestRequestTypeDef

```python
# UpdateFilterRequestRequestTypeDef definition

class UpdateFilterRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    FilterName: str,
    Description: NotRequired[str],
    Action: NotRequired[FilterActionType],  # (1)
    Rank: NotRequired[int],
    FindingCriteria: NotRequired[FindingCriteriaTypeDef],  # (2)
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef) 
## CoverageResourceTypeDef

```python
# CoverageResourceTypeDef definition

class CoverageResourceTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    DetectorId: NotRequired[str],
    AccountId: NotRequired[str],
    ResourceDetails: NotRequired[CoverageResourceDetailsTypeDef],  # (1)
    CoverageStatus: NotRequired[CoverageStatusType],  # (2)
    Issue: NotRequired[str],
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: CoverageResourceDetailsTypeDef](./type_defs.md#coverageresourcedetailstypedef) 
2. See [:material-code-brackets: CoverageStatusType](./literals.md#coveragestatustype) 
## GetCoverageStatisticsRequestRequestTypeDef

```python
# GetCoverageStatisticsRequestRequestTypeDef definition

class GetCoverageStatisticsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    StatisticsType: Sequence[CoverageStatisticsTypeType],  # (1)
    FilterCriteria: NotRequired[CoverageFilterCriteriaTypeDef],  # (2)
```

1. See [:material-code-brackets: CoverageStatisticsTypeType](./literals.md#coveragestatisticstypetype) 
2. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
## ListCoverageRequestPaginateTypeDef

```python
# ListCoverageRequestPaginateTypeDef definition

class ListCoverageRequestPaginateTypeDef(TypedDict):
    DetectorId: str,
    FilterCriteria: NotRequired[CoverageFilterCriteriaTypeDef],  # (1)
    SortCriteria: NotRequired[CoverageSortCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-braces: CoverageSortCriteriaTypeDef](./type_defs.md#coveragesortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCoverageRequestRequestTypeDef

```python
# ListCoverageRequestRequestTypeDef definition

class ListCoverageRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    FilterCriteria: NotRequired[CoverageFilterCriteriaTypeDef],  # (1)
    SortCriteria: NotRequired[CoverageSortCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-braces: CoverageSortCriteriaTypeDef](./type_defs.md#coveragesortcriteriatypedef) 
## CreateMalwareProtectionPlanRequestRequestTypeDef

```python
# CreateMalwareProtectionPlanRequestRequestTypeDef definition

class CreateMalwareProtectionPlanRequestRequestTypeDef(TypedDict):
    Role: str,
    ProtectedResource: CreateProtectedResourceTypeDef,  # (1)
    ClientToken: NotRequired[str],
    Actions: NotRequired[MalwareProtectionPlanActionsTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CreateProtectedResourceTypeDef](./type_defs.md#createprotectedresourcetypedef) 
2. See [:material-code-braces: MalwareProtectionPlanActionsTypeDef](./type_defs.md#malwareprotectionplanactionstypedef) 
## AccountFreeTrialInfoTypeDef

```python
# AccountFreeTrialInfoTypeDef definition

class AccountFreeTrialInfoTypeDef(TypedDict):
    AccountId: NotRequired[str],
    DataSources: NotRequired[DataSourcesFreeTrialTypeDef],  # (1)
    Features: NotRequired[List[FreeTrialFeatureConfigurationResultTypeDef]],  # (2)
```

1. See [:material-code-braces: DataSourcesFreeTrialTypeDef](./type_defs.md#datasourcesfreetrialtypedef) 
2. See [:material-code-braces: FreeTrialFeatureConfigurationResultTypeDef](./type_defs.md#freetrialfeatureconfigurationresulttypedef) 
## DataSourceConfigurationsResultTypeDef

```python
# DataSourceConfigurationsResultTypeDef definition

class DataSourceConfigurationsResultTypeDef(TypedDict):
    CloudTrail: CloudTrailConfigurationResultTypeDef,  # (1)
    DNSLogs: DNSLogsConfigurationResultTypeDef,  # (2)
    FlowLogs: FlowLogsConfigurationResultTypeDef,  # (3)
    S3Logs: S3LogsConfigurationResultTypeDef,  # (4)
    Kubernetes: NotRequired[KubernetesConfigurationResultTypeDef],  # (5)
    MalwareProtection: NotRequired[MalwareProtectionConfigurationResultTypeDef],  # (6)
```

1. See [:material-code-braces: CloudTrailConfigurationResultTypeDef](./type_defs.md#cloudtrailconfigurationresulttypedef) 
2. See [:material-code-braces: DNSLogsConfigurationResultTypeDef](./type_defs.md#dnslogsconfigurationresulttypedef) 
3. See [:material-code-braces: FlowLogsConfigurationResultTypeDef](./type_defs.md#flowlogsconfigurationresulttypedef) 
4. See [:material-code-braces: S3LogsConfigurationResultTypeDef](./type_defs.md#s3logsconfigurationresulttypedef) 
5. See [:material-code-braces: KubernetesConfigurationResultTypeDef](./type_defs.md#kubernetesconfigurationresulttypedef) 
6. See [:material-code-braces: MalwareProtectionConfigurationResultTypeDef](./type_defs.md#malwareprotectionconfigurationresulttypedef) 
## UnprocessedDataSourcesResultTypeDef

```python
# UnprocessedDataSourcesResultTypeDef definition

class UnprocessedDataSourcesResultTypeDef(TypedDict):
    MalwareProtection: NotRequired[MalwareProtectionConfigurationResultTypeDef],  # (1)
```

1. See [:material-code-braces: MalwareProtectionConfigurationResultTypeDef](./type_defs.md#malwareprotectionconfigurationresulttypedef) 
## DescribeMalwareScansRequestPaginateTypeDef

```python
# DescribeMalwareScansRequestPaginateTypeDef definition

class DescribeMalwareScansRequestPaginateTypeDef(TypedDict):
    DetectorId: str,
    FilterCriteria: NotRequired[FilterCriteriaTypeDef],  # (1)
    SortCriteria: NotRequired[SortCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMalwareScansRequestRequestTypeDef

```python
# DescribeMalwareScansRequestRequestTypeDef definition

class DescribeMalwareScansRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    FilterCriteria: NotRequired[FilterCriteriaTypeDef],  # (1)
    SortCriteria: NotRequired[SortCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
## EcsClusterDetailsTypeDef

```python
# EcsClusterDetailsTypeDef definition

class EcsClusterDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    Status: NotRequired[str],
    ActiveServicesCount: NotRequired[int],
    RegisteredContainerInstancesCount: NotRequired[int],
    RunningTasksCount: NotRequired[int],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    TaskDetails: NotRequired[EcsTaskDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EcsTaskDetailsTypeDef](./type_defs.md#ecstaskdetailstypedef) 
## KubernetesDetailsTypeDef

```python
# KubernetesDetailsTypeDef definition

class KubernetesDetailsTypeDef(TypedDict):
    KubernetesUserDetails: NotRequired[KubernetesUserDetailsTypeDef],  # (1)
    KubernetesWorkloadDetails: NotRequired[KubernetesWorkloadDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: KubernetesUserDetailsTypeDef](./type_defs.md#kubernetesuserdetailstypedef) 
2. See [:material-code-braces: KubernetesWorkloadDetailsTypeDef](./type_defs.md#kubernetesworkloaddetailstypedef) 
## RuntimeDetailsTypeDef

```python
# RuntimeDetailsTypeDef definition

class RuntimeDetailsTypeDef(TypedDict):
    Process: NotRequired[ProcessDetailsTypeDef],  # (1)
    Context: NotRequired[RuntimeContextTypeDef],  # (2)
```

1. See [:material-code-braces: ProcessDetailsTypeDef](./type_defs.md#processdetailstypedef) 
2. See [:material-code-braces: RuntimeContextTypeDef](./type_defs.md#runtimecontexttypedef) 
## CreateDetectorRequestRequestTypeDef

```python
# CreateDetectorRequestRequestTypeDef definition

class CreateDetectorRequestRequestTypeDef(TypedDict):
    Enable: bool,
    ClientToken: NotRequired[str],
    FindingPublishingFrequency: NotRequired[FindingPublishingFrequencyType],  # (1)
    DataSources: NotRequired[DataSourceConfigurationsTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
    Features: NotRequired[Sequence[DetectorFeatureConfigurationTypeDef]],  # (3)
```

1. See [:material-code-brackets: FindingPublishingFrequencyType](./literals.md#findingpublishingfrequencytype) 
2. See [:material-code-braces: DataSourceConfigurationsTypeDef](./type_defs.md#datasourceconfigurationstypedef) 
3. See [:material-code-braces: DetectorFeatureConfigurationTypeDef](./type_defs.md#detectorfeatureconfigurationtypedef) 
## UpdateDetectorRequestRequestTypeDef

```python
# UpdateDetectorRequestRequestTypeDef definition

class UpdateDetectorRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    Enable: NotRequired[bool],
    FindingPublishingFrequency: NotRequired[FindingPublishingFrequencyType],  # (1)
    DataSources: NotRequired[DataSourceConfigurationsTypeDef],  # (2)
    Features: NotRequired[Sequence[DetectorFeatureConfigurationTypeDef]],  # (3)
```

1. See [:material-code-brackets: FindingPublishingFrequencyType](./literals.md#findingpublishingfrequencytype) 
2. See [:material-code-braces: DataSourceConfigurationsTypeDef](./type_defs.md#datasourceconfigurationstypedef) 
3. See [:material-code-braces: DetectorFeatureConfigurationTypeDef](./type_defs.md#detectorfeatureconfigurationtypedef) 
## UpdateMemberDetectorsRequestRequestTypeDef

```python
# UpdateMemberDetectorsRequestRequestTypeDef definition

class UpdateMemberDetectorsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AccountIds: Sequence[str],
    DataSources: NotRequired[DataSourceConfigurationsTypeDef],  # (1)
    Features: NotRequired[Sequence[MemberFeaturesConfigurationTypeDef]],  # (2)
```

1. See [:material-code-braces: DataSourceConfigurationsTypeDef](./type_defs.md#datasourceconfigurationstypedef) 
2. See [:material-code-braces: MemberFeaturesConfigurationTypeDef](./type_defs.md#memberfeaturesconfigurationtypedef) 
## OrganizationDataSourceConfigurationsResultTypeDef

```python
# OrganizationDataSourceConfigurationsResultTypeDef definition

class OrganizationDataSourceConfigurationsResultTypeDef(TypedDict):
    S3Logs: OrganizationS3LogsConfigurationResultTypeDef,  # (1)
    Kubernetes: NotRequired[OrganizationKubernetesConfigurationResultTypeDef],  # (2)
    MalwareProtection: NotRequired[OrganizationMalwareProtectionConfigurationResultTypeDef],  # (3)
```

1. See [:material-code-braces: OrganizationS3LogsConfigurationResultTypeDef](./type_defs.md#organizations3logsconfigurationresulttypedef) 
2. See [:material-code-braces: OrganizationKubernetesConfigurationResultTypeDef](./type_defs.md#organizationkubernetesconfigurationresulttypedef) 
3. See [:material-code-braces: OrganizationMalwareProtectionConfigurationResultTypeDef](./type_defs.md#organizationmalwareprotectionconfigurationresulttypedef) 
## OrganizationDataSourceConfigurationsTypeDef

```python
# OrganizationDataSourceConfigurationsTypeDef definition

class OrganizationDataSourceConfigurationsTypeDef(TypedDict):
    S3Logs: NotRequired[OrganizationS3LogsConfigurationTypeDef],  # (1)
    Kubernetes: NotRequired[OrganizationKubernetesConfigurationTypeDef],  # (2)
    MalwareProtection: NotRequired[OrganizationMalwareProtectionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: OrganizationS3LogsConfigurationTypeDef](./type_defs.md#organizations3logsconfigurationtypedef) 
2. See [:material-code-braces: OrganizationKubernetesConfigurationTypeDef](./type_defs.md#organizationkubernetesconfigurationtypedef) 
3. See [:material-code-braces: OrganizationMalwareProtectionConfigurationTypeDef](./type_defs.md#organizationmalwareprotectionconfigurationtypedef) 
## OrganizationDetailsTypeDef

```python
# OrganizationDetailsTypeDef definition

class OrganizationDetailsTypeDef(TypedDict):
    UpdatedAt: NotRequired[datetime],
    OrganizationStatistics: NotRequired[OrganizationStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: OrganizationStatisticsTypeDef](./type_defs.md#organizationstatisticstypedef) 
## PortProbeActionTypeDef

```python
# PortProbeActionTypeDef definition

class PortProbeActionTypeDef(TypedDict):
    Blocked: NotRequired[bool],
    PortProbeDetails: NotRequired[List[PortProbeDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: PortProbeDetailTypeDef](./type_defs.md#portprobedetailtypedef) 
## ResourceV2TypeDef

```python
# ResourceV2TypeDef definition

class ResourceV2TypeDef(TypedDict):
    Uid: str,
    ResourceType: FindingResourceTypeType,  # (1)
    Name: NotRequired[str],
    AccountId: NotRequired[str],
    Region: NotRequired[str],
    Service: NotRequired[str],
    CloudPartition: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    Data: NotRequired[ResourceDataTypeDef],  # (3)
```

1. See [:material-code-brackets: FindingResourceTypeType](./literals.md#findingresourcetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResourceDataTypeDef](./type_defs.md#resourcedatatypedef) 
## GetMalwareScanSettingsResponseTypeDef

```python
# GetMalwareScanSettingsResponseTypeDef definition

class GetMalwareScanSettingsResponseTypeDef(TypedDict):
    ScanResourceCriteria: ScanResourceCriteriaOutputTypeDef,  # (1)
    EbsSnapshotPreservation: EbsSnapshotPreservationType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ScanResourceCriteriaOutputTypeDef](./type_defs.md#scanresourcecriteriaoutputtypedef) 
2. See [:material-code-brackets: EbsSnapshotPreservationType](./literals.md#ebssnapshotpreservationtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScanResourceCriteriaTypeDef

```python
# ScanResourceCriteriaTypeDef definition

class ScanResourceCriteriaTypeDef(TypedDict):
    Include: NotRequired[Mapping[ScanCriterionKeyType, ScanConditionUnionTypeDef]],  # (1)
    Exclude: NotRequired[Mapping[ScanCriterionKeyType, ScanConditionTypeDef]],  # (2)
```

1. See [:material-code-brackets: ScanCriterionKeyType](./literals.md#scancriterionkeytype) [:material-code-braces: ScanConditionTypeDef](./type_defs.md#scanconditiontypedef) [:material-code-braces: ScanConditionOutputTypeDef](./type_defs.md#scanconditionoutputtypedef) 
2. See [:material-code-brackets: ScanCriterionKeyType](./literals.md#scancriterionkeytype) [:material-code-braces: ScanConditionTypeDef](./type_defs.md#scanconditiontypedef) 
## ScanDetectionsTypeDef

```python
# ScanDetectionsTypeDef definition

class ScanDetectionsTypeDef(TypedDict):
    ScannedItemCount: NotRequired[ScannedItemCountTypeDef],  # (1)
    ThreatsDetectedItemCount: NotRequired[ThreatsDetectedItemCountTypeDef],  # (2)
    HighestSeverityThreatDetails: NotRequired[HighestSeverityThreatDetailsTypeDef],  # (3)
    ThreatDetectedByName: NotRequired[ThreatDetectedByNameTypeDef],  # (4)
```

1. See [:material-code-braces: ScannedItemCountTypeDef](./type_defs.md#scanneditemcounttypedef) 
2. See [:material-code-braces: ThreatsDetectedItemCountTypeDef](./type_defs.md#threatsdetecteditemcounttypedef) 
3. See [:material-code-braces: HighestSeverityThreatDetailsTypeDef](./type_defs.md#highestseveritythreatdetailstypedef) 
4. See [:material-code-braces: ThreatDetectedByNameTypeDef](./type_defs.md#threatdetectedbynametypedef) 
## UsageStatisticsTypeDef

```python
# UsageStatisticsTypeDef definition

class UsageStatisticsTypeDef(TypedDict):
    SumByAccount: NotRequired[List[UsageAccountResultTypeDef]],  # (1)
    TopAccountsByFeature: NotRequired[List[UsageTopAccountsResultTypeDef]],  # (2)
    SumByDataSource: NotRequired[List[UsageDataSourceResultTypeDef]],  # (3)
    SumByResource: NotRequired[List[UsageResourceResultTypeDef]],  # (4)
    TopResources: NotRequired[List[UsageResourceResultTypeDef]],  # (4)
    SumByFeature: NotRequired[List[UsageFeatureResultTypeDef]],  # (6)
```

1. See [:material-code-braces: UsageAccountResultTypeDef](./type_defs.md#usageaccountresulttypedef) 
2. See [:material-code-braces: UsageTopAccountsResultTypeDef](./type_defs.md#usagetopaccountsresulttypedef) 
3. See [:material-code-braces: UsageDataSourceResultTypeDef](./type_defs.md#usagedatasourceresulttypedef) 
4. See [:material-code-braces: UsageResourceResultTypeDef](./type_defs.md#usageresourceresulttypedef) 
5. See [:material-code-braces: UsageResourceResultTypeDef](./type_defs.md#usageresourceresulttypedef) 
6. See [:material-code-braces: UsageFeatureResultTypeDef](./type_defs.md#usagefeatureresulttypedef) 
## S3BucketDetailTypeDef

```python
# S3BucketDetailTypeDef definition

class S3BucketDetailTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Owner: NotRequired[OwnerTypeDef],  # (1)
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    DefaultServerSideEncryption: NotRequired[DefaultServerSideEncryptionTypeDef],  # (3)
    PublicAccess: NotRequired[PublicAccessTypeDef],  # (4)
    S3ObjectDetails: NotRequired[List[S3ObjectDetailTypeDef]],  # (5)
```

1. See [:material-code-braces: OwnerTypeDef](./type_defs.md#ownertypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: DefaultServerSideEncryptionTypeDef](./type_defs.md#defaultserversideencryptiontypedef) 
4. See [:material-code-braces: PublicAccessTypeDef](./type_defs.md#publicaccesstypedef) 
5. See [:material-code-braces: S3ObjectDetailTypeDef](./type_defs.md#s3objectdetailtypedef) 
## ListCoverageResponseTypeDef

```python
# ListCoverageResponseTypeDef definition

class ListCoverageResponseTypeDef(TypedDict):
    Resources: List[CoverageResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CoverageResourceTypeDef](./type_defs.md#coverageresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRemainingFreeTrialDaysResponseTypeDef

```python
# GetRemainingFreeTrialDaysResponseTypeDef definition

class GetRemainingFreeTrialDaysResponseTypeDef(TypedDict):
    Accounts: List[AccountFreeTrialInfoTypeDef],  # (1)
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AccountFreeTrialInfoTypeDef](./type_defs.md#accountfreetrialinfotypedef) 
2. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDetectorResponseTypeDef

```python
# GetDetectorResponseTypeDef definition

class GetDetectorResponseTypeDef(TypedDict):
    CreatedAt: str,
    FindingPublishingFrequency: FindingPublishingFrequencyType,  # (1)
    ServiceRole: str,
    Status: DetectorStatusType,  # (2)
    UpdatedAt: str,
    DataSources: DataSourceConfigurationsResultTypeDef,  # (3)
    Tags: Dict[str, str],
    Features: List[DetectorFeatureConfigurationResultTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: FindingPublishingFrequencyType](./literals.md#findingpublishingfrequencytype) 
2. See [:material-code-brackets: DetectorStatusType](./literals.md#detectorstatustype) 
3. See [:material-code-braces: DataSourceConfigurationsResultTypeDef](./type_defs.md#datasourceconfigurationsresulttypedef) 
4. See [:material-code-braces: DetectorFeatureConfigurationResultTypeDef](./type_defs.md#detectorfeatureconfigurationresulttypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MemberDataSourceConfigurationTypeDef

```python
# MemberDataSourceConfigurationTypeDef definition

class MemberDataSourceConfigurationTypeDef(TypedDict):
    AccountId: str,
    DataSources: NotRequired[DataSourceConfigurationsResultTypeDef],  # (1)
    Features: NotRequired[List[MemberFeaturesConfigurationResultTypeDef]],  # (2)
```

1. See [:material-code-braces: DataSourceConfigurationsResultTypeDef](./type_defs.md#datasourceconfigurationsresulttypedef) 
2. See [:material-code-braces: MemberFeaturesConfigurationResultTypeDef](./type_defs.md#memberfeaturesconfigurationresulttypedef) 
## CreateDetectorResponseTypeDef

```python
# CreateDetectorResponseTypeDef definition

class CreateDetectorResponseTypeDef(TypedDict):
    DetectorId: str,
    UnprocessedDataSources: UnprocessedDataSourcesResultTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedDataSourcesResultTypeDef](./type_defs.md#unprocesseddatasourcesresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationConfigurationResponseTypeDef

```python
# DescribeOrganizationConfigurationResponseTypeDef definition

class DescribeOrganizationConfigurationResponseTypeDef(TypedDict):
    AutoEnable: bool,
    MemberAccountLimitReached: bool,
    DataSources: OrganizationDataSourceConfigurationsResultTypeDef,  # (1)
    Features: List[OrganizationFeatureConfigurationResultTypeDef],  # (2)
    AutoEnableOrganizationMembers: AutoEnableMembersType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OrganizationDataSourceConfigurationsResultTypeDef](./type_defs.md#organizationdatasourceconfigurationsresulttypedef) 
2. See [:material-code-braces: OrganizationFeatureConfigurationResultTypeDef](./type_defs.md#organizationfeatureconfigurationresulttypedef) 
3. See [:material-code-brackets: AutoEnableMembersType](./literals.md#autoenablememberstype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOrganizationConfigurationRequestRequestTypeDef

```python
# UpdateOrganizationConfigurationRequestRequestTypeDef definition

class UpdateOrganizationConfigurationRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    AutoEnable: NotRequired[bool],
    DataSources: NotRequired[OrganizationDataSourceConfigurationsTypeDef],  # (1)
    Features: NotRequired[Sequence[OrganizationFeatureConfigurationTypeDef]],  # (2)
    AutoEnableOrganizationMembers: NotRequired[AutoEnableMembersType],  # (3)
```

1. See [:material-code-braces: OrganizationDataSourceConfigurationsTypeDef](./type_defs.md#organizationdatasourceconfigurationstypedef) 
2. See [:material-code-braces: OrganizationFeatureConfigurationTypeDef](./type_defs.md#organizationfeatureconfigurationtypedef) 
3. See [:material-code-brackets: AutoEnableMembersType](./literals.md#autoenablememberstype) 
## GetOrganizationStatisticsResponseTypeDef

```python
# GetOrganizationStatisticsResponseTypeDef definition

class GetOrganizationStatisticsResponseTypeDef(TypedDict):
    OrganizationDetails: OrganizationDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationDetailsTypeDef](./type_defs.md#organizationdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    ActionType: NotRequired[str],
    AwsApiCallAction: NotRequired[AwsApiCallActionTypeDef],  # (1)
    DnsRequestAction: NotRequired[DnsRequestActionTypeDef],  # (2)
    NetworkConnectionAction: NotRequired[NetworkConnectionActionTypeDef],  # (3)
    PortProbeAction: NotRequired[PortProbeActionTypeDef],  # (4)
    KubernetesApiCallAction: NotRequired[KubernetesApiCallActionTypeDef],  # (5)
    RdsLoginAttemptAction: NotRequired[RdsLoginAttemptActionTypeDef],  # (6)
    KubernetesPermissionCheckedDetails: NotRequired[KubernetesPermissionCheckedDetailsTypeDef],  # (7)
    KubernetesRoleBindingDetails: NotRequired[KubernetesRoleBindingDetailsTypeDef],  # (8)
    KubernetesRoleDetails: NotRequired[KubernetesRoleDetailsTypeDef],  # (9)
```

1. See [:material-code-braces: AwsApiCallActionTypeDef](./type_defs.md#awsapicallactiontypedef) 
2. See [:material-code-braces: DnsRequestActionTypeDef](./type_defs.md#dnsrequestactiontypedef) 
3. See [:material-code-braces: NetworkConnectionActionTypeDef](./type_defs.md#networkconnectionactiontypedef) 
4. See [:material-code-braces: PortProbeActionTypeDef](./type_defs.md#portprobeactiontypedef) 
5. See [:material-code-braces: KubernetesApiCallActionTypeDef](./type_defs.md#kubernetesapicallactiontypedef) 
6. See [:material-code-braces: RdsLoginAttemptActionTypeDef](./type_defs.md#rdsloginattemptactiontypedef) 
7. See [:material-code-braces: KubernetesPermissionCheckedDetailsTypeDef](./type_defs.md#kubernetespermissioncheckeddetailstypedef) 
8. See [:material-code-braces: KubernetesRoleBindingDetailsTypeDef](./type_defs.md#kubernetesrolebindingdetailstypedef) 
9. See [:material-code-braces: KubernetesRoleDetailsTypeDef](./type_defs.md#kubernetesroledetailstypedef) 
## SequenceTypeDef

```python
# SequenceTypeDef definition

class SequenceTypeDef(TypedDict):
    Uid: str,
    Description: str,
    Signals: List[SignalTypeDef],  # (4)
    Actors: NotRequired[List[ActorTypeDef]],  # (1)
    Resources: NotRequired[List[ResourceV2TypeDef]],  # (2)
    Endpoints: NotRequired[List[NetworkEndpointTypeDef]],  # (3)
    SequenceIndicators: NotRequired[List[IndicatorTypeDef]],  # (5)
```

1. See [:material-code-braces: ActorTypeDef](./type_defs.md#actortypedef) 
2. See [:material-code-braces: ResourceV2TypeDef](./type_defs.md#resourcev2typedef) 
3. See [:material-code-braces: NetworkEndpointTypeDef](./type_defs.md#networkendpointtypedef) 
4. See [:material-code-braces: SignalTypeDef](./type_defs.md#signaltypedef) 
5. See [:material-code-braces: IndicatorTypeDef](./type_defs.md#indicatortypedef) 
## UpdateMalwareScanSettingsRequestRequestTypeDef

```python
# UpdateMalwareScanSettingsRequestRequestTypeDef definition

class UpdateMalwareScanSettingsRequestRequestTypeDef(TypedDict):
    DetectorId: str,
    ScanResourceCriteria: NotRequired[ScanResourceCriteriaTypeDef],  # (1)
    EbsSnapshotPreservation: NotRequired[EbsSnapshotPreservationType],  # (2)
```

1. See [:material-code-braces: ScanResourceCriteriaTypeDef](./type_defs.md#scanresourcecriteriatypedef) 
2. See [:material-code-brackets: EbsSnapshotPreservationType](./literals.md#ebssnapshotpreservationtype) 
## EbsVolumeScanDetailsTypeDef

```python
# EbsVolumeScanDetailsTypeDef definition

class EbsVolumeScanDetailsTypeDef(TypedDict):
    ScanId: NotRequired[str],
    ScanStartedAt: NotRequired[datetime],
    ScanCompletedAt: NotRequired[datetime],
    TriggerFindingId: NotRequired[str],
    Sources: NotRequired[List[str]],
    ScanDetections: NotRequired[ScanDetectionsTypeDef],  # (1)
    ScanType: NotRequired[ScanTypeType],  # (2)
```

1. See [:material-code-braces: ScanDetectionsTypeDef](./type_defs.md#scandetectionstypedef) 
2. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
## GetUsageStatisticsResponseTypeDef

```python
# GetUsageStatisticsResponseTypeDef definition

class GetUsageStatisticsResponseTypeDef(TypedDict):
    UsageStatistics: UsageStatisticsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UsageStatisticsTypeDef](./type_defs.md#usagestatisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    AccessKeyDetails: NotRequired[AccessKeyDetailsTypeDef],  # (1)
    S3BucketDetails: NotRequired[List[S3BucketDetailTypeDef]],  # (2)
    InstanceDetails: NotRequired[InstanceDetailsTypeDef],  # (3)
    EksClusterDetails: NotRequired[EksClusterDetailsTypeDef],  # (4)
    KubernetesDetails: NotRequired[KubernetesDetailsTypeDef],  # (5)
    ResourceType: NotRequired[str],
    EbsVolumeDetails: NotRequired[EbsVolumeDetailsTypeDef],  # (6)
    EcsClusterDetails: NotRequired[EcsClusterDetailsTypeDef],  # (7)
    ContainerDetails: NotRequired[ContainerTypeDef],  # (8)
    RdsDbInstanceDetails: NotRequired[RdsDbInstanceDetailsTypeDef],  # (9)
    RdsLimitlessDbDetails: NotRequired[RdsLimitlessDbDetailsTypeDef],  # (10)
    RdsDbUserDetails: NotRequired[RdsDbUserDetailsTypeDef],  # (11)
    LambdaDetails: NotRequired[LambdaDetailsTypeDef],  # (12)
```

1. See [:material-code-braces: AccessKeyDetailsTypeDef](./type_defs.md#accesskeydetailstypedef) 
2. See [:material-code-braces: S3BucketDetailTypeDef](./type_defs.md#s3bucketdetailtypedef) 
3. See [:material-code-braces: InstanceDetailsTypeDef](./type_defs.md#instancedetailstypedef) 
4. See [:material-code-braces: EksClusterDetailsTypeDef](./type_defs.md#eksclusterdetailstypedef) 
5. See [:material-code-braces: KubernetesDetailsTypeDef](./type_defs.md#kubernetesdetailstypedef) 
6. See [:material-code-braces: EbsVolumeDetailsTypeDef](./type_defs.md#ebsvolumedetailstypedef) 
7. See [:material-code-braces: EcsClusterDetailsTypeDef](./type_defs.md#ecsclusterdetailstypedef) 
8. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) 
9. See [:material-code-braces: RdsDbInstanceDetailsTypeDef](./type_defs.md#rdsdbinstancedetailstypedef) 
10. See [:material-code-braces: RdsLimitlessDbDetailsTypeDef](./type_defs.md#rdslimitlessdbdetailstypedef) 
11. See [:material-code-braces: RdsDbUserDetailsTypeDef](./type_defs.md#rdsdbuserdetailstypedef) 
12. See [:material-code-braces: LambdaDetailsTypeDef](./type_defs.md#lambdadetailstypedef) 
## GetMemberDetectorsResponseTypeDef

```python
# GetMemberDetectorsResponseTypeDef definition

class GetMemberDetectorsResponseTypeDef(TypedDict):
    MemberDataSourceConfigurations: List[MemberDataSourceConfigurationTypeDef],  # (1)
    UnprocessedAccounts: List[UnprocessedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MemberDataSourceConfigurationTypeDef](./type_defs.md#memberdatasourceconfigurationtypedef) 
2. See [:material-code-braces: UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectionTypeDef

```python
# DetectionTypeDef definition

class DetectionTypeDef(TypedDict):
    Anomaly: NotRequired[AnomalyTypeDef],  # (1)
    Sequence: NotRequired[SequenceTypeDef],  # (2)
```

1. See [:material-code-braces: AnomalyTypeDef](./type_defs.md#anomalytypedef) 
2. See [:material-code-braces: SequenceTypeDef](./type_defs.md#sequencetypedef) 
## ServiceTypeDef

```python
# ServiceTypeDef definition

class ServiceTypeDef(TypedDict):
    Action: NotRequired[ActionTypeDef],  # (1)
    Evidence: NotRequired[EvidenceTypeDef],  # (2)
    Archived: NotRequired[bool],
    Count: NotRequired[int],
    DetectorId: NotRequired[str],
    EventFirstSeen: NotRequired[str],
    EventLastSeen: NotRequired[str],
    ResourceRole: NotRequired[str],
    ServiceName: NotRequired[str],
    UserFeedback: NotRequired[str],
    AdditionalInfo: NotRequired[ServiceAdditionalInfoTypeDef],  # (3)
    FeatureName: NotRequired[str],
    EbsVolumeScanDetails: NotRequired[EbsVolumeScanDetailsTypeDef],  # (4)
    RuntimeDetails: NotRequired[RuntimeDetailsTypeDef],  # (5)
    Detection: NotRequired[DetectionTypeDef],  # (6)
    MalwareScanDetails: NotRequired[MalwareScanDetailsTypeDef],  # (7)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: EvidenceTypeDef](./type_defs.md#evidencetypedef) 
3. See [:material-code-braces: ServiceAdditionalInfoTypeDef](./type_defs.md#serviceadditionalinfotypedef) 
4. See [:material-code-braces: EbsVolumeScanDetailsTypeDef](./type_defs.md#ebsvolumescandetailstypedef) 
5. See [:material-code-braces: RuntimeDetailsTypeDef](./type_defs.md#runtimedetailstypedef) 
6. See [:material-code-braces: DetectionTypeDef](./type_defs.md#detectiontypedef) 
7. See [:material-code-braces: MalwareScanDetailsTypeDef](./type_defs.md#malwarescandetailstypedef) 
## FindingTypeDef

```python
# FindingTypeDef definition

class FindingTypeDef(TypedDict):
    AccountId: str,
    Arn: str,
    CreatedAt: str,
    Id: str,
    Region: str,
    Resource: ResourceTypeDef,  # (1)
    SchemaVersion: str,
    Severity: float,
    Type: str,
    UpdatedAt: str,
    Confidence: NotRequired[float],
    Description: NotRequired[str],
    Partition: NotRequired[str],
    Service: NotRequired[ServiceTypeDef],  # (2)
    Title: NotRequired[str],
    AssociatedAttackSequenceArn: NotRequired[str],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
## GetFindingsResponseTypeDef

```python
# GetFindingsResponseTypeDef definition

class GetFindingsResponseTypeDef(TypedDict):
    Findings: List[FindingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FindingTypeDef](./type_defs.md#findingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
