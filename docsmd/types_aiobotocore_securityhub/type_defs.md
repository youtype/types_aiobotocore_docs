# Type definitions

> [Index](../README.md) > [SecurityHub](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SecurityHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
    type annotations stubs module [types-aiobotocore-securityhub](https://pypi.org/project/types-aiobotocore-securityhub/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AcceptAdministratorInvitationRequestRequestTypeDef

```python
# AcceptAdministratorInvitationRequestRequestTypeDef definition

class AcceptAdministratorInvitationRequestRequestTypeDef(TypedDict):
    AdministratorId: str,
    InvitationId: str,
```

## AcceptInvitationRequestRequestTypeDef

```python
# AcceptInvitationRequestRequestTypeDef definition

class AcceptInvitationRequestRequestTypeDef(TypedDict):
    MasterId: str,
    InvitationId: str,
```

## AccountDetailsTypeDef

```python
# AccountDetailsTypeDef definition

class AccountDetailsTypeDef(TypedDict):
    AccountId: str,
    Email: NotRequired[str],
```

## ActionLocalIpDetailsTypeDef

```python
# ActionLocalIpDetailsTypeDef definition

class ActionLocalIpDetailsTypeDef(TypedDict):
    IpAddressV4: NotRequired[str],
```

## ActionLocalPortDetailsTypeDef

```python
# ActionLocalPortDetailsTypeDef definition

class ActionLocalPortDetailsTypeDef(TypedDict):
    Port: NotRequired[int],
    PortName: NotRequired[str],
```

## CityTypeDef

```python
# CityTypeDef definition

class CityTypeDef(TypedDict):
    CityName: NotRequired[str],
```

## CountryTypeDef

```python
# CountryTypeDef definition

class CountryTypeDef(TypedDict):
    CountryCode: NotRequired[str],
    CountryName: NotRequired[str],
```

## GeoLocationTypeDef

```python
# GeoLocationTypeDef definition

class GeoLocationTypeDef(TypedDict):
    Lon: NotRequired[float],
    Lat: NotRequired[float],
```

## IpOrganizationDetailsTypeDef

```python
# IpOrganizationDetailsTypeDef definition

class IpOrganizationDetailsTypeDef(TypedDict):
    Asn: NotRequired[int],
    AsnOrg: NotRequired[str],
    Isp: NotRequired[str],
    Org: NotRequired[str],
```

## ActionRemotePortDetailsTypeDef

```python
# ActionRemotePortDetailsTypeDef definition

class ActionRemotePortDetailsTypeDef(TypedDict):
    Port: NotRequired[int],
    PortName: NotRequired[str],
```

## ActionTargetTypeDef

```python
# ActionTargetTypeDef definition

class ActionTargetTypeDef(TypedDict):
    ActionTargetArn: str,
    Name: str,
    Description: str,
```

## DnsRequestActionTypeDef

```python
# DnsRequestActionTypeDef definition

class DnsRequestActionTypeDef(TypedDict):
    Domain: NotRequired[str],
    Protocol: NotRequired[str],
    Blocked: NotRequired[bool],
```

## AdjustmentTypeDef

```python
# AdjustmentTypeDef definition

class AdjustmentTypeDef(TypedDict):
    Metric: NotRequired[str],
    Reason: NotRequired[str],
```

## AdminAccountTypeDef

```python
# AdminAccountTypeDef definition

class AdminAccountTypeDef(TypedDict):
    AccountId: NotRequired[str],
    Status: NotRequired[AdminStatusType],  # (1)
```

1. See [:material-code-brackets: AdminStatusType](./literals.md#adminstatustype) 
## AssociatedStandardTypeDef

```python
# AssociatedStandardTypeDef definition

class AssociatedStandardTypeDef(TypedDict):
    StandardsId: NotRequired[str],
```

## AssociationStateDetailsTypeDef

```python
# AssociationStateDetailsTypeDef definition

class AssociationStateDetailsTypeDef(TypedDict):
    State: NotRequired[str],
    StatusMessage: NotRequired[str],
```

## NoteUpdateTypeDef

```python
# NoteUpdateTypeDef definition

class NoteUpdateTypeDef(TypedDict):
    Text: str,
    UpdatedBy: str,
```

## RelatedFindingTypeDef

```python
# RelatedFindingTypeDef definition

class RelatedFindingTypeDef(TypedDict):
    ProductArn: str,
    Id: str,
```

## SeverityUpdateTypeDef

```python
# SeverityUpdateTypeDef definition

class SeverityUpdateTypeDef(TypedDict):
    Normalized: NotRequired[int],
    Product: NotRequired[float],
    Label: NotRequired[SeverityLabelType],  # (1)
```

1. See [:material-code-brackets: SeverityLabelType](./literals.md#severitylabeltype) 
## WorkflowUpdateTypeDef

```python
# WorkflowUpdateTypeDef definition

class WorkflowUpdateTypeDef(TypedDict):
    Status: NotRequired[WorkflowStatusType],  # (1)
```

1. See [:material-code-brackets: WorkflowStatusType](./literals.md#workflowstatustype) 
## MapFilterTypeDef

```python
# MapFilterTypeDef definition

class MapFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    Comparison: NotRequired[MapFilterComparisonType],  # (1)
```

1. See [:material-code-brackets: MapFilterComparisonType](./literals.md#mapfiltercomparisontype) 
## NumberFilterTypeDef

```python
# NumberFilterTypeDef definition

class NumberFilterTypeDef(TypedDict):
    Gte: NotRequired[float],
    Lte: NotRequired[float],
    Eq: NotRequired[float],
```

## StringFilterTypeDef

```python
# StringFilterTypeDef definition

class StringFilterTypeDef(TypedDict):
    Value: NotRequired[str],
    Comparison: NotRequired[StringFilterComparisonType],  # (1)
```

1. See [:material-code-brackets: StringFilterComparisonType](./literals.md#stringfiltercomparisontype) 
## AutomationRulesMetadataTypeDef

```python
# AutomationRulesMetadataTypeDef definition

class AutomationRulesMetadataTypeDef(TypedDict):
    RuleArn: NotRequired[str],
    RuleStatus: NotRequired[RuleStatusType],  # (1)
    RuleOrder: NotRequired[int],
    RuleName: NotRequired[str],
    Description: NotRequired[str],
    IsTerminal: NotRequired[bool],
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
    CreatedBy: NotRequired[str],
```

1. See [:material-code-brackets: RuleStatusType](./literals.md#rulestatustype) 
## AvailabilityZoneTypeDef

```python
# AvailabilityZoneTypeDef definition

class AvailabilityZoneTypeDef(TypedDict):
    ZoneName: NotRequired[str],
    SubnetId: NotRequired[str],
```

## AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef

```python
# AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef definition

class AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef(TypedDict):
    KmsKeyId: NotRequired[str],
    UseAwsOwnedKey: NotRequired[bool],
```

## AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef

```python
# AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef definition

class AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef(TypedDict):
    Hosts: NotRequired[Sequence[str]],
    RoleBase: NotRequired[str],
    RoleName: NotRequired[str],
    RoleSearchMatching: NotRequired[str],
    RoleSearchSubtree: NotRequired[bool],
    ServiceAccountUsername: NotRequired[str],
    UserBase: NotRequired[str],
    UserRoleName: NotRequired[str],
    UserSearchMatching: NotRequired[str],
    UserSearchSubtree: NotRequired[bool],
```

## AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef

```python
# AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef definition

class AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef(TypedDict):
    DayOfWeek: NotRequired[str],
    TimeOfDay: NotRequired[str],
    TimeZone: NotRequired[str],
```

## AwsAmazonMqBrokerUsersDetailsTypeDef

```python
# AwsAmazonMqBrokerUsersDetailsTypeDef definition

class AwsAmazonMqBrokerUsersDetailsTypeDef(TypedDict):
    PendingChange: NotRequired[str],
    Username: NotRequired[str],
```

## AwsAmazonMqBrokerLogsPendingDetailsTypeDef

```python
# AwsAmazonMqBrokerLogsPendingDetailsTypeDef definition

class AwsAmazonMqBrokerLogsPendingDetailsTypeDef(TypedDict):
    Audit: NotRequired[bool],
    General: NotRequired[bool],
```

## AwsApiCallActionDomainDetailsTypeDef

```python
# AwsApiCallActionDomainDetailsTypeDef definition

class AwsApiCallActionDomainDetailsTypeDef(TypedDict):
    Domain: NotRequired[str],
```

## AwsApiGatewayAccessLogSettingsTypeDef

```python
# AwsApiGatewayAccessLogSettingsTypeDef definition

class AwsApiGatewayAccessLogSettingsTypeDef(TypedDict):
    Format: NotRequired[str],
    DestinationArn: NotRequired[str],
```

## AwsApiGatewayCanarySettingsTypeDef

```python
# AwsApiGatewayCanarySettingsTypeDef definition

class AwsApiGatewayCanarySettingsTypeDef(TypedDict):
    PercentTraffic: NotRequired[float],
    DeploymentId: NotRequired[str],
    StageVariableOverrides: NotRequired[Mapping[str, str]],
    UseStageCache: NotRequired[bool],
```

## AwsApiGatewayEndpointConfigurationTypeDef

```python
# AwsApiGatewayEndpointConfigurationTypeDef definition

class AwsApiGatewayEndpointConfigurationTypeDef(TypedDict):
    Types: NotRequired[Sequence[str]],
```

## AwsApiGatewayMethodSettingsTypeDef

```python
# AwsApiGatewayMethodSettingsTypeDef definition

class AwsApiGatewayMethodSettingsTypeDef(TypedDict):
    MetricsEnabled: NotRequired[bool],
    LoggingLevel: NotRequired[str],
    DataTraceEnabled: NotRequired[bool],
    ThrottlingBurstLimit: NotRequired[int],
    ThrottlingRateLimit: NotRequired[float],
    CachingEnabled: NotRequired[bool],
    CacheTtlInSeconds: NotRequired[int],
    CacheDataEncrypted: NotRequired[bool],
    RequireAuthorizationForCacheControl: NotRequired[bool],
    UnauthorizedCacheControlHeaderStrategy: NotRequired[str],
    HttpMethod: NotRequired[str],
    ResourcePath: NotRequired[str],
```

## AwsCorsConfigurationTypeDef

```python
# AwsCorsConfigurationTypeDef definition

class AwsCorsConfigurationTypeDef(TypedDict):
    AllowOrigins: NotRequired[Sequence[str]],
    AllowCredentials: NotRequired[bool],
    ExposeHeaders: NotRequired[Sequence[str]],
    MaxAge: NotRequired[int],
    AllowMethods: NotRequired[Sequence[str]],
    AllowHeaders: NotRequired[Sequence[str]],
```

## AwsApiGatewayV2RouteSettingsTypeDef

```python
# AwsApiGatewayV2RouteSettingsTypeDef definition

class AwsApiGatewayV2RouteSettingsTypeDef(TypedDict):
    DetailedMetricsEnabled: NotRequired[bool],
    LoggingLevel: NotRequired[str],
    DataTraceEnabled: NotRequired[bool],
    ThrottlingBurstLimit: NotRequired[int],
    ThrottlingRateLimit: NotRequired[float],
```

## AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef

```python
# AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef definition

class AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef(TypedDict):
    AuthorizerResultTtlInSeconds: NotRequired[int],
    AuthorizerUri: NotRequired[str],
    IdentityValidationExpression: NotRequired[str],
```

## AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef

```python
# AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef definition

class AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef(TypedDict):
    AuthTtL: NotRequired[int],
    ClientId: NotRequired[str],
    IatTtL: NotRequired[int],
    Issuer: NotRequired[str],
```

## AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef

```python
# AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef definition

class AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef(TypedDict):
    AppIdClientRegex: NotRequired[str],
    AwsRegion: NotRequired[str],
    DefaultAction: NotRequired[str],
    UserPoolId: NotRequired[str],
```

## AwsAppSyncGraphQlApiLogConfigDetailsTypeDef

```python
# AwsAppSyncGraphQlApiLogConfigDetailsTypeDef definition

class AwsAppSyncGraphQlApiLogConfigDetailsTypeDef(TypedDict):
    CloudWatchLogsRoleArn: NotRequired[str],
    ExcludeVerboseContent: NotRequired[bool],
    FieldLogLevel: NotRequired[str],
```

## AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef

```python
# AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef definition

class AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef(TypedDict):
    EncryptionOption: NotRequired[str],
    KmsKey: NotRequired[str],
```

## AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef

```python
# AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef definition

class AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef(TypedDict):
    Value: NotRequired[str],
```

## AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef

```python
# AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef definition

class AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef(TypedDict):
    LaunchTemplateId: NotRequired[str],
    LaunchTemplateName: NotRequired[str],
    Version: NotRequired[str],
```

## AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef

```python
# AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef definition

class AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef(TypedDict):
    OnDemandAllocationStrategy: NotRequired[str],
    OnDemandBaseCapacity: NotRequired[int],
    OnDemandPercentageAboveBaseCapacity: NotRequired[int],
    SpotAllocationStrategy: NotRequired[str],
    SpotInstancePools: NotRequired[int],
    SpotMaxPrice: NotRequired[str],
```

## AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef

```python
# AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef definition

class AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef(TypedDict):
    LaunchTemplateId: NotRequired[str],
    LaunchTemplateName: NotRequired[str],
    Version: NotRequired[str],
```

## AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef

```python
# AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef definition

class AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef(TypedDict):
    InstanceType: NotRequired[str],
    WeightedCapacity: NotRequired[str],
```

## AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef

```python
# AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef definition

class AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef(TypedDict):
    DeleteOnTermination: NotRequired[bool],
    Encrypted: NotRequired[bool],
    Iops: NotRequired[int],
    SnapshotId: NotRequired[str],
    VolumeSize: NotRequired[int],
    VolumeType: NotRequired[str],
```

## AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef

```python
# AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef definition

class AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef

```python
# AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef definition

class AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef(TypedDict):
    HttpEndpoint: NotRequired[str],
    HttpPutResponseHopLimit: NotRequired[int],
    HttpTokens: NotRequired[str],
```

## AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef

```python
# AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef definition

class AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef(TypedDict):
    BackupOptions: NotRequired[Mapping[str, str]],
    ResourceType: NotRequired[str],
```

## AwsBackupBackupPlanLifecycleDetailsTypeDef

```python
# AwsBackupBackupPlanLifecycleDetailsTypeDef definition

class AwsBackupBackupPlanLifecycleDetailsTypeDef(TypedDict):
    DeleteAfterDays: NotRequired[int],
    MoveToColdStorageAfterDays: NotRequired[int],
```

## AwsBackupBackupVaultNotificationsDetailsTypeDef

```python
# AwsBackupBackupVaultNotificationsDetailsTypeDef definition

class AwsBackupBackupVaultNotificationsDetailsTypeDef(TypedDict):
    BackupVaultEvents: NotRequired[Sequence[str]],
    SnsTopicArn: NotRequired[str],
```

## AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef

```python
# AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef definition

class AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef(TypedDict):
    DeleteAt: NotRequired[str],
    MoveToColdStorageAt: NotRequired[str],
```

## AwsBackupRecoveryPointCreatedByDetailsTypeDef

```python
# AwsBackupRecoveryPointCreatedByDetailsTypeDef definition

class AwsBackupRecoveryPointCreatedByDetailsTypeDef(TypedDict):
    BackupPlanArn: NotRequired[str],
    BackupPlanId: NotRequired[str],
    BackupPlanVersion: NotRequired[str],
    BackupRuleId: NotRequired[str],
```

## AwsBackupRecoveryPointLifecycleDetailsTypeDef

```python
# AwsBackupRecoveryPointLifecycleDetailsTypeDef definition

class AwsBackupRecoveryPointLifecycleDetailsTypeDef(TypedDict):
    DeleteAfterDays: NotRequired[int],
    MoveToColdStorageAfterDays: NotRequired[int],
```

## AwsCertificateManagerCertificateExtendedKeyUsageTypeDef

```python
# AwsCertificateManagerCertificateExtendedKeyUsageTypeDef definition

class AwsCertificateManagerCertificateExtendedKeyUsageTypeDef(TypedDict):
    Name: NotRequired[str],
    OId: NotRequired[str],
```

## AwsCertificateManagerCertificateKeyUsageTypeDef

```python
# AwsCertificateManagerCertificateKeyUsageTypeDef definition

class AwsCertificateManagerCertificateKeyUsageTypeDef(TypedDict):
    Name: NotRequired[str],
```

## AwsCertificateManagerCertificateOptionsTypeDef

```python
# AwsCertificateManagerCertificateOptionsTypeDef definition

class AwsCertificateManagerCertificateOptionsTypeDef(TypedDict):
    CertificateTransparencyLoggingPreference: NotRequired[str],
```

## AwsCertificateManagerCertificateResourceRecordTypeDef

```python
# AwsCertificateManagerCertificateResourceRecordTypeDef definition

class AwsCertificateManagerCertificateResourceRecordTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[str],
    Value: NotRequired[str],
```

## AwsCloudFormationStackDriftInformationDetailsTypeDef

```python
# AwsCloudFormationStackDriftInformationDetailsTypeDef definition

class AwsCloudFormationStackDriftInformationDetailsTypeDef(TypedDict):
    StackDriftStatus: NotRequired[str],
```

## AwsCloudFormationStackOutputsDetailsTypeDef

```python
# AwsCloudFormationStackOutputsDetailsTypeDef definition

class AwsCloudFormationStackOutputsDetailsTypeDef(TypedDict):
    Description: NotRequired[str],
    OutputKey: NotRequired[str],
    OutputValue: NotRequired[str],
```

## AwsCloudFrontDistributionCacheBehaviorTypeDef

```python
# AwsCloudFrontDistributionCacheBehaviorTypeDef definition

class AwsCloudFrontDistributionCacheBehaviorTypeDef(TypedDict):
    ViewerProtocolPolicy: NotRequired[str],
```

## AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef

```python
# AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef definition

class AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef(TypedDict):
    ViewerProtocolPolicy: NotRequired[str],
```

## AwsCloudFrontDistributionLoggingTypeDef

```python
# AwsCloudFrontDistributionLoggingTypeDef definition

class AwsCloudFrontDistributionLoggingTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Enabled: NotRequired[bool],
    IncludeCookies: NotRequired[bool],
    Prefix: NotRequired[str],
```

## AwsCloudFrontDistributionViewerCertificateTypeDef

```python
# AwsCloudFrontDistributionViewerCertificateTypeDef definition

class AwsCloudFrontDistributionViewerCertificateTypeDef(TypedDict):
    AcmCertificateArn: NotRequired[str],
    Certificate: NotRequired[str],
    CertificateSource: NotRequired[str],
    CloudFrontDefaultCertificate: NotRequired[bool],
    IamCertificateId: NotRequired[str],
    MinimumProtocolVersion: NotRequired[str],
    SslSupportMethod: NotRequired[str],
```

## AwsCloudFrontDistributionOriginSslProtocolsTypeDef

```python
# AwsCloudFrontDistributionOriginSslProtocolsTypeDef definition

class AwsCloudFrontDistributionOriginSslProtocolsTypeDef(TypedDict):
    Items: NotRequired[Sequence[str]],
    Quantity: NotRequired[int],
```

## AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef

```python
# AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef definition

class AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef(TypedDict):
    Items: NotRequired[Sequence[int]],
    Quantity: NotRequired[int],
```

## AwsCloudFrontDistributionOriginS3OriginConfigTypeDef

```python
# AwsCloudFrontDistributionOriginS3OriginConfigTypeDef definition

class AwsCloudFrontDistributionOriginS3OriginConfigTypeDef(TypedDict):
    OriginAccessIdentity: NotRequired[str],
```

## AwsCloudTrailTrailDetailsTypeDef

```python
# AwsCloudTrailTrailDetailsTypeDef definition

class AwsCloudTrailTrailDetailsTypeDef(TypedDict):
    CloudWatchLogsLogGroupArn: NotRequired[str],
    CloudWatchLogsRoleArn: NotRequired[str],
    HasCustomEventSelectors: NotRequired[bool],
    HomeRegion: NotRequired[str],
    IncludeGlobalServiceEvents: NotRequired[bool],
    IsMultiRegionTrail: NotRequired[bool],
    IsOrganizationTrail: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    LogFileValidationEnabled: NotRequired[bool],
    Name: NotRequired[str],
    S3BucketName: NotRequired[str],
    S3KeyPrefix: NotRequired[str],
    SnsTopicArn: NotRequired[str],
    SnsTopicName: NotRequired[str],
    TrailArn: NotRequired[str],
```

## AwsCloudWatchAlarmDimensionsDetailsTypeDef

```python
# AwsCloudWatchAlarmDimensionsDetailsTypeDef definition

class AwsCloudWatchAlarmDimensionsDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## AwsCodeBuildProjectArtifactsDetailsTypeDef

```python
# AwsCodeBuildProjectArtifactsDetailsTypeDef definition

class AwsCodeBuildProjectArtifactsDetailsTypeDef(TypedDict):
    ArtifactIdentifier: NotRequired[str],
    EncryptionDisabled: NotRequired[bool],
    Location: NotRequired[str],
    Name: NotRequired[str],
    NamespaceType: NotRequired[str],
    OverrideArtifactName: NotRequired[bool],
    Packaging: NotRequired[str],
    Path: NotRequired[str],
    Type: NotRequired[str],
```

## AwsCodeBuildProjectSourceTypeDef

```python
# AwsCodeBuildProjectSourceTypeDef definition

class AwsCodeBuildProjectSourceTypeDef(TypedDict):
    Type: NotRequired[str],
    Location: NotRequired[str],
    GitCloneDepth: NotRequired[int],
    InsecureSsl: NotRequired[bool],
```

## AwsCodeBuildProjectVpcConfigTypeDef

```python
# AwsCodeBuildProjectVpcConfigTypeDef definition

class AwsCodeBuildProjectVpcConfigTypeDef(TypedDict):
    VpcId: NotRequired[str],
    Subnets: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
```

## AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef

```python
# AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef definition

class AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[str],
    Value: NotRequired[str],
```

## AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef

```python
# AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef definition

class AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef(TypedDict):
    Credential: NotRequired[str],
    CredentialProvider: NotRequired[str],
```

## AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef

```python
# AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef definition

class AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef(TypedDict):
    GroupName: NotRequired[str],
    Status: NotRequired[str],
    StreamName: NotRequired[str],
```

## AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef

```python
# AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef definition

class AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef(TypedDict):
    EncryptionDisabled: NotRequired[bool],
    Location: NotRequired[str],
    Status: NotRequired[str],
```

## AwsDynamoDbTableAttributeDefinitionTypeDef

```python
# AwsDynamoDbTableAttributeDefinitionTypeDef definition

class AwsDynamoDbTableAttributeDefinitionTypeDef(TypedDict):
    AttributeName: NotRequired[str],
    AttributeType: NotRequired[str],
```

## AwsDynamoDbTableBillingModeSummaryTypeDef

```python
# AwsDynamoDbTableBillingModeSummaryTypeDef definition

class AwsDynamoDbTableBillingModeSummaryTypeDef(TypedDict):
    BillingMode: NotRequired[str],
    LastUpdateToPayPerRequestDateTime: NotRequired[str],
```

## AwsDynamoDbTableKeySchemaTypeDef

```python
# AwsDynamoDbTableKeySchemaTypeDef definition

class AwsDynamoDbTableKeySchemaTypeDef(TypedDict):
    AttributeName: NotRequired[str],
    KeyType: NotRequired[str],
```

## AwsDynamoDbTableProvisionedThroughputTypeDef

```python
# AwsDynamoDbTableProvisionedThroughputTypeDef definition

class AwsDynamoDbTableProvisionedThroughputTypeDef(TypedDict):
    LastDecreaseDateTime: NotRequired[str],
    LastIncreaseDateTime: NotRequired[str],
    NumberOfDecreasesToday: NotRequired[int],
    ReadCapacityUnits: NotRequired[int],
    WriteCapacityUnits: NotRequired[int],
```

## AwsDynamoDbTableRestoreSummaryTypeDef

```python
# AwsDynamoDbTableRestoreSummaryTypeDef definition

class AwsDynamoDbTableRestoreSummaryTypeDef(TypedDict):
    SourceBackupArn: NotRequired[str],
    SourceTableArn: NotRequired[str],
    RestoreDateTime: NotRequired[str],
    RestoreInProgress: NotRequired[bool],
```

## AwsDynamoDbTableSseDescriptionTypeDef

```python
# AwsDynamoDbTableSseDescriptionTypeDef definition

class AwsDynamoDbTableSseDescriptionTypeDef(TypedDict):
    InaccessibleEncryptionDateTime: NotRequired[str],
    Status: NotRequired[str],
    SseType: NotRequired[str],
    KmsMasterKeyArn: NotRequired[str],
```

## AwsDynamoDbTableStreamSpecificationTypeDef

```python
# AwsDynamoDbTableStreamSpecificationTypeDef definition

class AwsDynamoDbTableStreamSpecificationTypeDef(TypedDict):
    StreamEnabled: NotRequired[bool],
    StreamViewType: NotRequired[str],
```

## AwsDynamoDbTableProjectionTypeDef

```python
# AwsDynamoDbTableProjectionTypeDef definition

class AwsDynamoDbTableProjectionTypeDef(TypedDict):
    NonKeyAttributes: NotRequired[Sequence[str]],
    ProjectionType: NotRequired[str],
```

## AwsDynamoDbTableProvisionedThroughputOverrideTypeDef

```python
# AwsDynamoDbTableProvisionedThroughputOverrideTypeDef definition

class AwsDynamoDbTableProvisionedThroughputOverrideTypeDef(TypedDict):
    ReadCapacityUnits: NotRequired[int],
```

## AwsEc2EipDetailsTypeDef

```python
# AwsEc2EipDetailsTypeDef definition

class AwsEc2EipDetailsTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    PublicIp: NotRequired[str],
    AllocationId: NotRequired[str],
    AssociationId: NotRequired[str],
    Domain: NotRequired[str],
    PublicIpv4Pool: NotRequired[str],
    NetworkBorderGroup: NotRequired[str],
    NetworkInterfaceId: NotRequired[str],
    NetworkInterfaceOwnerId: NotRequired[str],
    PrivateIpAddress: NotRequired[str],
```

## AwsEc2InstanceMetadataOptionsTypeDef

```python
# AwsEc2InstanceMetadataOptionsTypeDef definition

class AwsEc2InstanceMetadataOptionsTypeDef(TypedDict):
    HttpEndpoint: NotRequired[str],
    HttpProtocolIpv6: NotRequired[str],
    HttpPutResponseHopLimit: NotRequired[int],
    HttpTokens: NotRequired[str],
    InstanceMetadataTags: NotRequired[str],
```

## AwsEc2InstanceMonitoringDetailsTypeDef

```python
# AwsEc2InstanceMonitoringDetailsTypeDef definition

class AwsEc2InstanceMonitoringDetailsTypeDef(TypedDict):
    State: NotRequired[str],
```

## AwsEc2InstanceNetworkInterfacesDetailsTypeDef

```python
# AwsEc2InstanceNetworkInterfacesDetailsTypeDef definition

class AwsEc2InstanceNetworkInterfacesDetailsTypeDef(TypedDict):
    NetworkInterfaceId: NotRequired[str],
```

## AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef definition

class AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef(TypedDict):
    DeleteOnTermination: NotRequired[bool],
    Encrypted: NotRequired[bool],
    Iops: NotRequired[int],
    KmsKeyId: NotRequired[str],
    SnapshotId: NotRequired[str],
    Throughput: NotRequired[int],
    VolumeSize: NotRequired[int],
    VolumeType: NotRequired[str],
```

## AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef definition

class AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef(TypedDict):
    CapacityReservationId: NotRequired[str],
    CapacityReservationResourceGroupArn: NotRequired[str],
```

## AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef definition

class AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef(TypedDict):
    CoreCount: NotRequired[int],
    ThreadsPerCore: NotRequired[int],
```

## AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef definition

class AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef(TypedDict):
    CpuCredits: NotRequired[str],
```

## AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef definition

class AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef(TypedDict):
    Type: NotRequired[str],
```

## AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef definition

class AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef(TypedDict):
    Count: NotRequired[int],
    Type: NotRequired[str],
```

## AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef definition

class AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef definition

class AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef(TypedDict):
    Configured: NotRequired[bool],
```

## AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef definition

class AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef definition

class AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef(TypedDict):
    LicenseConfigurationArn: NotRequired[str],
```

## AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef definition

class AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef(TypedDict):
    AutoRecovery: NotRequired[str],
```

## AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef definition

class AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef(TypedDict):
    HttpEndpoint: NotRequired[str],
    HttpProtocolIpv6: NotRequired[str],
    HttpTokens: NotRequired[str],
    HttpPutResponseHopLimit: NotRequired[int],
    InstanceMetadataTags: NotRequired[str],
```

## AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef definition

class AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## AwsEc2LaunchTemplateDataPlacementDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataPlacementDetailsTypeDef definition

class AwsEc2LaunchTemplateDataPlacementDetailsTypeDef(TypedDict):
    Affinity: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    GroupName: NotRequired[str],
    HostId: NotRequired[str],
    HostResourceGroupArn: NotRequired[str],
    PartitionNumber: NotRequired[int],
    SpreadDomain: NotRequired[str],
    Tenancy: NotRequired[str],
```

## AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef definition

class AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef(TypedDict):
    EnableResourceNameDnsAAAARecord: NotRequired[bool],
    EnableResourceNameDnsARecord: NotRequired[bool],
    HostnameType: NotRequired[str],
```

## AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef definition

class AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef(TypedDict):
    BlockDurationMinutes: NotRequired[int],
    InstanceInterruptionBehavior: NotRequired[str],
    MaxPrice: NotRequired[str],
    SpotInstanceType: NotRequired[str],
    ValidUntil: NotRequired[str],
```

## AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef definition

class AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef(TypedDict):
    Max: NotRequired[int],
    Min: NotRequired[int],
```

## AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef definition

class AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef(TypedDict):
    Max: NotRequired[int],
    Min: NotRequired[int],
```

## AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef definition

class AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef(TypedDict):
    Max: NotRequired[int],
    Min: NotRequired[int],
```

## AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef definition

class AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef(TypedDict):
    Max: NotRequired[float],
    Min: NotRequired[float],
```

## AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef definition

class AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef(TypedDict):
    Max: NotRequired[int],
    Min: NotRequired[int],
```

## AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef definition

class AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef(TypedDict):
    Max: NotRequired[int],
    Min: NotRequired[int],
```

## AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef definition

class AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef(TypedDict):
    Max: NotRequired[float],
    Min: NotRequired[float],
```

## AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef definition

class AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef(TypedDict):
    Max: NotRequired[int],
    Min: NotRequired[int],
```

## AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef definition

class AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef(TypedDict):
    Ipv4Prefix: NotRequired[str],
```

## AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef definition

class AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef(TypedDict):
    Ipv6Address: NotRequired[str],
```

## AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef definition

class AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef(TypedDict):
    Ipv6Prefix: NotRequired[str],
```

## AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef definition

class AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef(TypedDict):
    Primary: NotRequired[bool],
    PrivateIpAddress: NotRequired[str],
```

## AwsEc2NetworkAclAssociationTypeDef

```python
# AwsEc2NetworkAclAssociationTypeDef definition

class AwsEc2NetworkAclAssociationTypeDef(TypedDict):
    NetworkAclAssociationId: NotRequired[str],
    NetworkAclId: NotRequired[str],
    SubnetId: NotRequired[str],
```

## IcmpTypeCodeTypeDef

```python
# IcmpTypeCodeTypeDef definition

class IcmpTypeCodeTypeDef(TypedDict):
    Code: NotRequired[int],
    Type: NotRequired[int],
```

## PortRangeFromToTypeDef

```python
# PortRangeFromToTypeDef definition

class PortRangeFromToTypeDef(TypedDict):
    From: NotRequired[int],
    To: NotRequired[int],
```

## AwsEc2NetworkInterfaceAttachmentTypeDef

```python
# AwsEc2NetworkInterfaceAttachmentTypeDef definition

class AwsEc2NetworkInterfaceAttachmentTypeDef(TypedDict):
    AttachTime: NotRequired[str],
    AttachmentId: NotRequired[str],
    DeleteOnTermination: NotRequired[bool],
    DeviceIndex: NotRequired[int],
    InstanceId: NotRequired[str],
    InstanceOwnerId: NotRequired[str],
    Status: NotRequired[str],
```

## AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef

```python
# AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef definition

class AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef(TypedDict):
    IpV6Address: NotRequired[str],
```

## AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef

```python
# AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef definition

class AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef(TypedDict):
    PrivateIpAddress: NotRequired[str],
    PrivateDnsName: NotRequired[str],
```

## AwsEc2NetworkInterfaceSecurityGroupTypeDef

```python
# AwsEc2NetworkInterfaceSecurityGroupTypeDef definition

class AwsEc2NetworkInterfaceSecurityGroupTypeDef(TypedDict):
    GroupName: NotRequired[str],
    GroupId: NotRequired[str],
```

## PropagatingVgwSetDetailsTypeDef

```python
# PropagatingVgwSetDetailsTypeDef definition

class PropagatingVgwSetDetailsTypeDef(TypedDict):
    GatewayId: NotRequired[str],
```

## RouteSetDetailsTypeDef

```python
# RouteSetDetailsTypeDef definition

class RouteSetDetailsTypeDef(TypedDict):
    CarrierGatewayId: NotRequired[str],
    CoreNetworkArn: NotRequired[str],
    DestinationCidrBlock: NotRequired[str],
    DestinationIpv6CidrBlock: NotRequired[str],
    DestinationPrefixListId: NotRequired[str],
    EgressOnlyInternetGatewayId: NotRequired[str],
    GatewayId: NotRequired[str],
    InstanceId: NotRequired[str],
    InstanceOwnerId: NotRequired[str],
    LocalGatewayId: NotRequired[str],
    NatGatewayId: NotRequired[str],
    NetworkInterfaceId: NotRequired[str],
    Origin: NotRequired[str],
    State: NotRequired[str],
    TransitGatewayId: NotRequired[str],
    VpcPeeringConnectionId: NotRequired[str],
```

## AwsEc2SecurityGroupIpRangeTypeDef

```python
# AwsEc2SecurityGroupIpRangeTypeDef definition

class AwsEc2SecurityGroupIpRangeTypeDef(TypedDict):
    CidrIp: NotRequired[str],
```

## AwsEc2SecurityGroupIpv6RangeTypeDef

```python
# AwsEc2SecurityGroupIpv6RangeTypeDef definition

class AwsEc2SecurityGroupIpv6RangeTypeDef(TypedDict):
    CidrIpv6: NotRequired[str],
```

## AwsEc2SecurityGroupPrefixListIdTypeDef

```python
# AwsEc2SecurityGroupPrefixListIdTypeDef definition

class AwsEc2SecurityGroupPrefixListIdTypeDef(TypedDict):
    PrefixListId: NotRequired[str],
```

## AwsEc2SecurityGroupUserIdGroupPairTypeDef

```python
# AwsEc2SecurityGroupUserIdGroupPairTypeDef definition

class AwsEc2SecurityGroupUserIdGroupPairTypeDef(TypedDict):
    GroupId: NotRequired[str],
    GroupName: NotRequired[str],
    PeeringStatus: NotRequired[str],
    UserId: NotRequired[str],
    VpcId: NotRequired[str],
    VpcPeeringConnectionId: NotRequired[str],
```

## Ipv6CidrBlockAssociationTypeDef

```python
# Ipv6CidrBlockAssociationTypeDef definition

class Ipv6CidrBlockAssociationTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    Ipv6CidrBlock: NotRequired[str],
    CidrBlockState: NotRequired[str],
```

## AwsEc2TransitGatewayDetailsTypeDef

```python
# AwsEc2TransitGatewayDetailsTypeDef definition

class AwsEc2TransitGatewayDetailsTypeDef(TypedDict):
    Id: NotRequired[str],
    Description: NotRequired[str],
    DefaultRouteTablePropagation: NotRequired[str],
    AutoAcceptSharedAttachments: NotRequired[str],
    DefaultRouteTableAssociation: NotRequired[str],
    TransitGatewayCidrBlocks: NotRequired[Sequence[str]],
    AssociationDefaultRouteTableId: NotRequired[str],
    PropagationDefaultRouteTableId: NotRequired[str],
    VpnEcmpSupport: NotRequired[str],
    DnsSupport: NotRequired[str],
    MulticastSupport: NotRequired[str],
    AmazonSideAsn: NotRequired[int],
```

## AwsEc2VolumeAttachmentTypeDef

```python
# AwsEc2VolumeAttachmentTypeDef definition

class AwsEc2VolumeAttachmentTypeDef(TypedDict):
    AttachTime: NotRequired[str],
    DeleteOnTermination: NotRequired[bool],
    InstanceId: NotRequired[str],
    Status: NotRequired[str],
```

## CidrBlockAssociationTypeDef

```python
# CidrBlockAssociationTypeDef definition

class CidrBlockAssociationTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    CidrBlock: NotRequired[str],
    CidrBlockState: NotRequired[str],
```

## AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef

```python
# AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef definition

class AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef(TypedDict):
    ServiceType: NotRequired[str],
```

## AwsEc2VpcPeeringConnectionStatusDetailsTypeDef

```python
# AwsEc2VpcPeeringConnectionStatusDetailsTypeDef definition

class AwsEc2VpcPeeringConnectionStatusDetailsTypeDef(TypedDict):
    Code: NotRequired[str],
    Message: NotRequired[str],
```

## VpcInfoCidrBlockSetDetailsTypeDef

```python
# VpcInfoCidrBlockSetDetailsTypeDef definition

class VpcInfoCidrBlockSetDetailsTypeDef(TypedDict):
    CidrBlock: NotRequired[str],
```

## VpcInfoIpv6CidrBlockSetDetailsTypeDef

```python
# VpcInfoIpv6CidrBlockSetDetailsTypeDef definition

class VpcInfoIpv6CidrBlockSetDetailsTypeDef(TypedDict):
    Ipv6CidrBlock: NotRequired[str],
```

## VpcInfoPeeringOptionsDetailsTypeDef

```python
# VpcInfoPeeringOptionsDetailsTypeDef definition

class VpcInfoPeeringOptionsDetailsTypeDef(TypedDict):
    AllowDnsResolutionFromRemoteVpc: NotRequired[bool],
    AllowEgressFromLocalClassicLinkToRemoteVpc: NotRequired[bool],
    AllowEgressFromLocalVpcToRemoteClassicLink: NotRequired[bool],
```

## AwsEc2VpnConnectionRoutesDetailsTypeDef

```python
# AwsEc2VpnConnectionRoutesDetailsTypeDef definition

class AwsEc2VpnConnectionRoutesDetailsTypeDef(TypedDict):
    DestinationCidrBlock: NotRequired[str],
    State: NotRequired[str],
```

## AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef

```python
# AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef definition

class AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef(TypedDict):
    AcceptedRouteCount: NotRequired[int],
    CertificateArn: NotRequired[str],
    LastStatusChange: NotRequired[str],
    OutsideIpAddress: NotRequired[str],
    Status: NotRequired[str],
    StatusMessage: NotRequired[str],
```

## AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef

```python
# AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef definition

class AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef(TypedDict):
    DpdTimeoutSeconds: NotRequired[int],
    IkeVersions: NotRequired[Sequence[str]],
    OutsideIpAddress: NotRequired[str],
    Phase1DhGroupNumbers: NotRequired[Sequence[int]],
    Phase1EncryptionAlgorithms: NotRequired[Sequence[str]],
    Phase1IntegrityAlgorithms: NotRequired[Sequence[str]],
    Phase1LifetimeSeconds: NotRequired[int],
    Phase2DhGroupNumbers: NotRequired[Sequence[int]],
    Phase2EncryptionAlgorithms: NotRequired[Sequence[str]],
    Phase2IntegrityAlgorithms: NotRequired[Sequence[str]],
    Phase2LifetimeSeconds: NotRequired[int],
    PreSharedKey: NotRequired[str],
    RekeyFuzzPercentage: NotRequired[int],
    RekeyMarginTimeSeconds: NotRequired[int],
    ReplayWindowSize: NotRequired[int],
    TunnelInsideCidr: NotRequired[str],
```

## AwsEcrContainerImageDetailsTypeDef

```python
# AwsEcrContainerImageDetailsTypeDef definition

class AwsEcrContainerImageDetailsTypeDef(TypedDict):
    RegistryId: NotRequired[str],
    RepositoryName: NotRequired[str],
    Architecture: NotRequired[str],
    ImageDigest: NotRequired[str],
    ImageTags: NotRequired[Sequence[str]],
    ImagePublishedAt: NotRequired[str],
```

## AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef

```python
# AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef definition

class AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef(TypedDict):
    ScanOnPush: NotRequired[bool],
```

## AwsEcrRepositoryLifecyclePolicyDetailsTypeDef

```python
# AwsEcrRepositoryLifecyclePolicyDetailsTypeDef definition

class AwsEcrRepositoryLifecyclePolicyDetailsTypeDef(TypedDict):
    LifecyclePolicyText: NotRequired[str],
    RegistryId: NotRequired[str],
```

## AwsEcsClusterClusterSettingsDetailsTypeDef

```python
# AwsEcsClusterClusterSettingsDetailsTypeDef definition

class AwsEcsClusterClusterSettingsDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef

```python
# AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef definition

class AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef(TypedDict):
    CloudWatchEncryptionEnabled: NotRequired[bool],
    CloudWatchLogGroupName: NotRequired[str],
    S3BucketName: NotRequired[str],
    S3EncryptionEnabled: NotRequired[bool],
    S3KeyPrefix: NotRequired[str],
```

## AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef

```python
# AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef definition

class AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef(TypedDict):
    Base: NotRequired[int],
    CapacityProvider: NotRequired[str],
    Weight: NotRequired[int],
```

## AwsMountPointTypeDef

```python
# AwsMountPointTypeDef definition

class AwsMountPointTypeDef(TypedDict):
    SourceVolume: NotRequired[str],
    ContainerPath: NotRequired[str],
```

## AwsEcsServiceCapacityProviderStrategyDetailsTypeDef

```python
# AwsEcsServiceCapacityProviderStrategyDetailsTypeDef definition

class AwsEcsServiceCapacityProviderStrategyDetailsTypeDef(TypedDict):
    Base: NotRequired[int],
    CapacityProvider: NotRequired[str],
    Weight: NotRequired[int],
```

## AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef

```python
# AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef definition

class AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef(TypedDict):
    Enable: NotRequired[bool],
    Rollback: NotRequired[bool],
```

## AwsEcsServiceDeploymentControllerDetailsTypeDef

```python
# AwsEcsServiceDeploymentControllerDetailsTypeDef definition

class AwsEcsServiceDeploymentControllerDetailsTypeDef(TypedDict):
    Type: NotRequired[str],
```

## AwsEcsServiceLoadBalancersDetailsTypeDef

```python
# AwsEcsServiceLoadBalancersDetailsTypeDef definition

class AwsEcsServiceLoadBalancersDetailsTypeDef(TypedDict):
    ContainerName: NotRequired[str],
    ContainerPort: NotRequired[int],
    LoadBalancerName: NotRequired[str],
    TargetGroupArn: NotRequired[str],
```

## AwsEcsServicePlacementConstraintsDetailsTypeDef

```python
# AwsEcsServicePlacementConstraintsDetailsTypeDef definition

class AwsEcsServicePlacementConstraintsDetailsTypeDef(TypedDict):
    Expression: NotRequired[str],
    Type: NotRequired[str],
```

## AwsEcsServicePlacementStrategiesDetailsTypeDef

```python
# AwsEcsServicePlacementStrategiesDetailsTypeDef definition

class AwsEcsServicePlacementStrategiesDetailsTypeDef(TypedDict):
    Field: NotRequired[str],
    Type: NotRequired[str],
```

## AwsEcsServiceServiceRegistriesDetailsTypeDef

```python
# AwsEcsServiceServiceRegistriesDetailsTypeDef definition

class AwsEcsServiceServiceRegistriesDetailsTypeDef(TypedDict):
    ContainerName: NotRequired[str],
    ContainerPort: NotRequired[int],
    Port: NotRequired[int],
    RegistryArn: NotRequired[str],
```

## AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef

```python
# AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef definition

class AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef(TypedDict):
    AssignPublicIp: NotRequired[str],
    SecurityGroups: NotRequired[Sequence[str]],
    Subnets: NotRequired[Sequence[str]],
```

## AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef(TypedDict):
    Condition: NotRequired[str],
    ContainerName: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef(TypedDict):
    Type: NotRequired[str],
    Value: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef(TypedDict):
    Hostname: NotRequired[str],
    IpAddress: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef(TypedDict):
    Options: NotRequired[Mapping[str, str]],
    Type: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef(TypedDict):
    Command: NotRequired[Sequence[str]],
    Interval: NotRequired[int],
    Retries: NotRequired[int],
    StartPeriod: NotRequired[int],
    Timeout: NotRequired[int],
```

## AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef(TypedDict):
    ContainerPath: NotRequired[str],
    ReadOnly: NotRequired[bool],
    SourceVolume: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef(TypedDict):
    ContainerPort: NotRequired[int],
    HostPort: NotRequired[int],
    Protocol: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef(TypedDict):
    CredentialsParameter: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef(TypedDict):
    Type: NotRequired[str],
    Value: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    ValueFrom: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef(TypedDict):
    Namespace: NotRequired[str],
    Value: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef(TypedDict):
    HardLimit: NotRequired[int],
    Name: NotRequired[str],
    SoftLimit: NotRequired[int],
```

## AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef(TypedDict):
    ReadOnly: NotRequired[bool],
    SourceContainer: NotRequired[str],
```

## AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef(TypedDict):
    Add: NotRequired[Sequence[str]],
    Drop: NotRequired[Sequence[str]],
```

## AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef(TypedDict):
    ContainerPath: NotRequired[str],
    HostPath: NotRequired[str],
    Permissions: NotRequired[Sequence[str]],
```

## AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef(TypedDict):
    ContainerPath: NotRequired[str],
    MountOptions: NotRequired[Sequence[str]],
    Size: NotRequired[int],
```

## AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    ValueFrom: NotRequired[str],
```

## AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef

```python
# AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef definition

class AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef(TypedDict):
    DeviceName: NotRequired[str],
    DeviceType: NotRequired[str],
```

## AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef

```python
# AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef definition

class AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef(TypedDict):
    Expression: NotRequired[str],
    Type: NotRequired[str],
```

## AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef

```python
# AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef definition

class AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef

```python
# AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef definition

class AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef(TypedDict):
    Autoprovision: NotRequired[bool],
    Driver: NotRequired[str],
    DriverOpts: NotRequired[Mapping[str, str]],
    Labels: NotRequired[Mapping[str, str]],
    Scope: NotRequired[str],
```

## AwsEcsTaskDefinitionVolumesHostDetailsTypeDef

```python
# AwsEcsTaskDefinitionVolumesHostDetailsTypeDef definition

class AwsEcsTaskDefinitionVolumesHostDetailsTypeDef(TypedDict):
    SourcePath: NotRequired[str],
```

## AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef

```python
# AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef definition

class AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef(TypedDict):
    AccessPointId: NotRequired[str],
    Iam: NotRequired[str],
```

## AwsEcsTaskVolumeHostDetailsTypeDef

```python
# AwsEcsTaskVolumeHostDetailsTypeDef definition

class AwsEcsTaskVolumeHostDetailsTypeDef(TypedDict):
    SourcePath: NotRequired[str],
```

## AwsEfsAccessPointPosixUserDetailsTypeDef

```python
# AwsEfsAccessPointPosixUserDetailsTypeDef definition

class AwsEfsAccessPointPosixUserDetailsTypeDef(TypedDict):
    Gid: NotRequired[str],
    SecondaryGids: NotRequired[Sequence[str]],
    Uid: NotRequired[str],
```

## AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef

```python
# AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef definition

class AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef(TypedDict):
    OwnerGid: NotRequired[str],
    OwnerUid: NotRequired[str],
    Permissions: NotRequired[str],
```

## AwsEksClusterResourcesVpcConfigDetailsTypeDef

```python
# AwsEksClusterResourcesVpcConfigDetailsTypeDef definition

class AwsEksClusterResourcesVpcConfigDetailsTypeDef(TypedDict):
    SecurityGroupIds: NotRequired[Sequence[str]],
    SubnetIds: NotRequired[Sequence[str]],
    EndpointPublicAccess: NotRequired[bool],
```

## AwsEksClusterLoggingClusterLoggingDetailsTypeDef

```python
# AwsEksClusterLoggingClusterLoggingDetailsTypeDef definition

class AwsEksClusterLoggingClusterLoggingDetailsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    Types: NotRequired[Sequence[str]],
```

## AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef

```python
# AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef definition

class AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef(TypedDict):
    EnvironmentName: NotRequired[str],
    LinkName: NotRequired[str],
```

## AwsElasticBeanstalkEnvironmentOptionSettingTypeDef

```python
# AwsElasticBeanstalkEnvironmentOptionSettingTypeDef definition

class AwsElasticBeanstalkEnvironmentOptionSettingTypeDef(TypedDict):
    Namespace: NotRequired[str],
    OptionName: NotRequired[str],
    ResourceName: NotRequired[str],
    Value: NotRequired[str],
```

## AwsElasticBeanstalkEnvironmentTierTypeDef

```python
# AwsElasticBeanstalkEnvironmentTierTypeDef definition

class AwsElasticBeanstalkEnvironmentTierTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[str],
    Version: NotRequired[str],
```

## AwsElasticsearchDomainDomainEndpointOptionsTypeDef

```python
# AwsElasticsearchDomainDomainEndpointOptionsTypeDef definition

class AwsElasticsearchDomainDomainEndpointOptionsTypeDef(TypedDict):
    EnforceHTTPS: NotRequired[bool],
    TLSSecurityPolicy: NotRequired[str],
```

## AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef

```python
# AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef definition

class AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    KmsKeyId: NotRequired[str],
```

## AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef

```python
# AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef definition

class AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## AwsElasticsearchDomainServiceSoftwareOptionsTypeDef

```python
# AwsElasticsearchDomainServiceSoftwareOptionsTypeDef definition

class AwsElasticsearchDomainServiceSoftwareOptionsTypeDef(TypedDict):
    AutomatedUpdateDate: NotRequired[str],
    Cancellable: NotRequired[bool],
    CurrentVersion: NotRequired[str],
    Description: NotRequired[str],
    NewVersion: NotRequired[str],
    UpdateAvailable: NotRequired[bool],
    UpdateStatus: NotRequired[str],
```

## AwsElasticsearchDomainVPCOptionsTypeDef

```python
# AwsElasticsearchDomainVPCOptionsTypeDef definition

class AwsElasticsearchDomainVPCOptionsTypeDef(TypedDict):
    AvailabilityZones: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
    SubnetIds: NotRequired[Sequence[str]],
    VPCId: NotRequired[str],
```

## AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef

```python
# AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef definition

class AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef(TypedDict):
    AvailabilityZoneCount: NotRequired[int],
```

## AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef

```python
# AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef definition

class AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef(TypedDict):
    CloudWatchLogsLogGroupArn: NotRequired[str],
    Enabled: NotRequired[bool],
```

## AwsElbAppCookieStickinessPolicyTypeDef

```python
# AwsElbAppCookieStickinessPolicyTypeDef definition

class AwsElbAppCookieStickinessPolicyTypeDef(TypedDict):
    CookieName: NotRequired[str],
    PolicyName: NotRequired[str],
```

## AwsElbLbCookieStickinessPolicyTypeDef

```python
# AwsElbLbCookieStickinessPolicyTypeDef definition

class AwsElbLbCookieStickinessPolicyTypeDef(TypedDict):
    CookieExpirationPeriod: NotRequired[int],
    PolicyName: NotRequired[str],
```

## AwsElbLoadBalancerAccessLogTypeDef

```python
# AwsElbLoadBalancerAccessLogTypeDef definition

class AwsElbLoadBalancerAccessLogTypeDef(TypedDict):
    EmitInterval: NotRequired[int],
    Enabled: NotRequired[bool],
    S3BucketName: NotRequired[str],
    S3BucketPrefix: NotRequired[str],
```

## AwsElbLoadBalancerAdditionalAttributeTypeDef

```python
# AwsElbLoadBalancerAdditionalAttributeTypeDef definition

class AwsElbLoadBalancerAdditionalAttributeTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## AwsElbLoadBalancerConnectionDrainingTypeDef

```python
# AwsElbLoadBalancerConnectionDrainingTypeDef definition

class AwsElbLoadBalancerConnectionDrainingTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    Timeout: NotRequired[int],
```

## AwsElbLoadBalancerConnectionSettingsTypeDef

```python
# AwsElbLoadBalancerConnectionSettingsTypeDef definition

class AwsElbLoadBalancerConnectionSettingsTypeDef(TypedDict):
    IdleTimeout: NotRequired[int],
```

## AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef

```python
# AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef definition

class AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## AwsElbLoadBalancerBackendServerDescriptionTypeDef

```python
# AwsElbLoadBalancerBackendServerDescriptionTypeDef definition

class AwsElbLoadBalancerBackendServerDescriptionTypeDef(TypedDict):
    InstancePort: NotRequired[int],
    PolicyNames: NotRequired[Sequence[str]],
```

## AwsElbLoadBalancerHealthCheckTypeDef

```python
# AwsElbLoadBalancerHealthCheckTypeDef definition

class AwsElbLoadBalancerHealthCheckTypeDef(TypedDict):
    HealthyThreshold: NotRequired[int],
    Interval: NotRequired[int],
    Target: NotRequired[str],
    Timeout: NotRequired[int],
    UnhealthyThreshold: NotRequired[int],
```

## AwsElbLoadBalancerInstanceTypeDef

```python
# AwsElbLoadBalancerInstanceTypeDef definition

class AwsElbLoadBalancerInstanceTypeDef(TypedDict):
    InstanceId: NotRequired[str],
```

## AwsElbLoadBalancerSourceSecurityGroupTypeDef

```python
# AwsElbLoadBalancerSourceSecurityGroupTypeDef definition

class AwsElbLoadBalancerSourceSecurityGroupTypeDef(TypedDict):
    GroupName: NotRequired[str],
    OwnerAlias: NotRequired[str],
```

## AwsElbLoadBalancerListenerTypeDef

```python
# AwsElbLoadBalancerListenerTypeDef definition

class AwsElbLoadBalancerListenerTypeDef(TypedDict):
    InstancePort: NotRequired[int],
    InstanceProtocol: NotRequired[str],
    LoadBalancerPort: NotRequired[int],
    Protocol: NotRequired[str],
    SslCertificateId: NotRequired[str],
```

## AwsElbv2LoadBalancerAttributeTypeDef

```python
# AwsElbv2LoadBalancerAttributeTypeDef definition

class AwsElbv2LoadBalancerAttributeTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## LoadBalancerStateTypeDef

```python
# LoadBalancerStateTypeDef definition

class LoadBalancerStateTypeDef(TypedDict):
    Code: NotRequired[str],
    Reason: NotRequired[str],
```

## AwsEventSchemasRegistryDetailsTypeDef

```python
# AwsEventSchemasRegistryDetailsTypeDef definition

class AwsEventSchemasRegistryDetailsTypeDef(TypedDict):
    Description: NotRequired[str],
    RegistryArn: NotRequired[str],
    RegistryName: NotRequired[str],
```

## AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef

```python
# AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef definition

class AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef(TypedDict):
    Status: NotRequired[str],
```

## AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef

```python
# AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef definition

class AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef(TypedDict):
    Status: NotRequired[str],
```

## AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef

```python
# AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef definition

class AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef(TypedDict):
    Status: NotRequired[str],
```

## AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef

```python
# AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef definition

class AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef(TypedDict):
    Status: NotRequired[str],
```

## AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef

```python
# AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef definition

class AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef(TypedDict):
    Status: NotRequired[str],
```

## AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef

```python
# AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef definition

class AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef(TypedDict):
    Reason: NotRequired[str],
    Status: NotRequired[str],
```

## AwsGuardDutyDetectorFeaturesDetailsTypeDef

```python
# AwsGuardDutyDetectorFeaturesDetailsTypeDef definition

class AwsGuardDutyDetectorFeaturesDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[str],
```

## AwsIamAccessKeySessionContextAttributesTypeDef

```python
# AwsIamAccessKeySessionContextAttributesTypeDef definition

class AwsIamAccessKeySessionContextAttributesTypeDef(TypedDict):
    MfaAuthenticated: NotRequired[bool],
    CreationDate: NotRequired[str],
```

## AwsIamAccessKeySessionContextSessionIssuerTypeDef

```python
# AwsIamAccessKeySessionContextSessionIssuerTypeDef definition

class AwsIamAccessKeySessionContextSessionIssuerTypeDef(TypedDict):
    Type: NotRequired[str],
    PrincipalId: NotRequired[str],
    Arn: NotRequired[str],
    AccountId: NotRequired[str],
    UserName: NotRequired[str],
```

## AwsIamAttachedManagedPolicyTypeDef

```python
# AwsIamAttachedManagedPolicyTypeDef definition

class AwsIamAttachedManagedPolicyTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    PolicyArn: NotRequired[str],
```

## AwsIamGroupPolicyTypeDef

```python
# AwsIamGroupPolicyTypeDef definition

class AwsIamGroupPolicyTypeDef(TypedDict):
    PolicyName: NotRequired[str],
```

## AwsIamInstanceProfileRoleTypeDef

```python
# AwsIamInstanceProfileRoleTypeDef definition

class AwsIamInstanceProfileRoleTypeDef(TypedDict):
    Arn: NotRequired[str],
    AssumeRolePolicyDocument: NotRequired[str],
    CreateDate: NotRequired[str],
    Path: NotRequired[str],
    RoleId: NotRequired[str],
    RoleName: NotRequired[str],
```

## AwsIamPermissionsBoundaryTypeDef

```python
# AwsIamPermissionsBoundaryTypeDef definition

class AwsIamPermissionsBoundaryTypeDef(TypedDict):
    PermissionsBoundaryArn: NotRequired[str],
    PermissionsBoundaryType: NotRequired[str],
```

## AwsIamPolicyVersionTypeDef

```python
# AwsIamPolicyVersionTypeDef definition

class AwsIamPolicyVersionTypeDef(TypedDict):
    VersionId: NotRequired[str],
    IsDefaultVersion: NotRequired[bool],
    CreateDate: NotRequired[str],
```

## AwsIamRolePolicyTypeDef

```python
# AwsIamRolePolicyTypeDef definition

class AwsIamRolePolicyTypeDef(TypedDict):
    PolicyName: NotRequired[str],
```

## AwsIamUserPolicyTypeDef

```python
# AwsIamUserPolicyTypeDef definition

class AwsIamUserPolicyTypeDef(TypedDict):
    PolicyName: NotRequired[str],
```

## AwsKinesisStreamStreamEncryptionDetailsTypeDef

```python
# AwsKinesisStreamStreamEncryptionDetailsTypeDef definition

class AwsKinesisStreamStreamEncryptionDetailsTypeDef(TypedDict):
    EncryptionType: NotRequired[str],
    KeyId: NotRequired[str],
```

## AwsKmsKeyDetailsTypeDef

```python
# AwsKmsKeyDetailsTypeDef definition

class AwsKmsKeyDetailsTypeDef(TypedDict):
    AWSAccountId: NotRequired[str],
    CreationDate: NotRequired[float],
    KeyId: NotRequired[str],
    KeyManager: NotRequired[str],
    KeyState: NotRequired[str],
    Origin: NotRequired[str],
    Description: NotRequired[str],
    KeyRotationStatus: NotRequired[bool],
```

## AwsLambdaFunctionCodeTypeDef

```python
# AwsLambdaFunctionCodeTypeDef definition

class AwsLambdaFunctionCodeTypeDef(TypedDict):
    S3Bucket: NotRequired[str],
    S3Key: NotRequired[str],
    S3ObjectVersion: NotRequired[str],
    ZipFile: NotRequired[str],
```

## AwsLambdaFunctionDeadLetterConfigTypeDef

```python
# AwsLambdaFunctionDeadLetterConfigTypeDef definition

class AwsLambdaFunctionDeadLetterConfigTypeDef(TypedDict):
    TargetArn: NotRequired[str],
```

## AwsLambdaFunctionLayerTypeDef

```python
# AwsLambdaFunctionLayerTypeDef definition

class AwsLambdaFunctionLayerTypeDef(TypedDict):
    Arn: NotRequired[str],
    CodeSize: NotRequired[int],
```

## AwsLambdaFunctionTracingConfigTypeDef

```python
# AwsLambdaFunctionTracingConfigTypeDef definition

class AwsLambdaFunctionTracingConfigTypeDef(TypedDict):
    Mode: NotRequired[str],
```

## AwsLambdaFunctionVpcConfigTypeDef

```python
# AwsLambdaFunctionVpcConfigTypeDef definition

class AwsLambdaFunctionVpcConfigTypeDef(TypedDict):
    SecurityGroupIds: NotRequired[Sequence[str]],
    SubnetIds: NotRequired[Sequence[str]],
    VpcId: NotRequired[str],
```

## AwsLambdaFunctionEnvironmentErrorTypeDef

```python
# AwsLambdaFunctionEnvironmentErrorTypeDef definition

class AwsLambdaFunctionEnvironmentErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## AwsLambdaLayerVersionDetailsTypeDef

```python
# AwsLambdaLayerVersionDetailsTypeDef definition

class AwsLambdaLayerVersionDetailsTypeDef(TypedDict):
    Version: NotRequired[int],
    CompatibleRuntimes: NotRequired[Sequence[str]],
    CreatedDate: NotRequired[str],
```

## AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef

```python
# AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef definition

class AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef(TypedDict):
    SubnetId: NotRequired[str],
```

## AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef

```python
# AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef definition

class AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef(TypedDict):
    MasterUserArn: NotRequired[str],
    MasterUserName: NotRequired[str],
    MasterUserPassword: NotRequired[str],
```

## AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef

```python
# AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef definition

class AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef(TypedDict):
    AvailabilityZoneCount: NotRequired[int],
```

## AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef

```python
# AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef definition

class AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef(TypedDict):
    CustomEndpointCertificateArn: NotRequired[str],
    CustomEndpointEnabled: NotRequired[bool],
    EnforceHTTPS: NotRequired[bool],
    CustomEndpoint: NotRequired[str],
    TLSSecurityPolicy: NotRequired[str],
```

## AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef

```python
# AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef definition

class AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    KmsKeyId: NotRequired[str],
```

## AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef

```python
# AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef definition

class AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef

```python
# AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef definition

class AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef(TypedDict):
    AutomatedUpdateDate: NotRequired[str],
    Cancellable: NotRequired[bool],
    CurrentVersion: NotRequired[str],
    Description: NotRequired[str],
    NewVersion: NotRequired[str],
    UpdateAvailable: NotRequired[bool],
    UpdateStatus: NotRequired[str],
    OptionalDeployment: NotRequired[bool],
```

## AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef

```python
# AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef definition

class AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef(TypedDict):
    SecurityGroupIds: NotRequired[Sequence[str]],
    SubnetIds: NotRequired[Sequence[str]],
```

## AwsOpenSearchServiceDomainLogPublishingOptionTypeDef

```python
# AwsOpenSearchServiceDomainLogPublishingOptionTypeDef definition

class AwsOpenSearchServiceDomainLogPublishingOptionTypeDef(TypedDict):
    CloudWatchLogsLogGroupArn: NotRequired[str],
    Enabled: NotRequired[bool],
```

## AwsRdsDbClusterAssociatedRoleTypeDef

```python
# AwsRdsDbClusterAssociatedRoleTypeDef definition

class AwsRdsDbClusterAssociatedRoleTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    Status: NotRequired[str],
```

## AwsRdsDbClusterMemberTypeDef

```python
# AwsRdsDbClusterMemberTypeDef definition

class AwsRdsDbClusterMemberTypeDef(TypedDict):
    IsClusterWriter: NotRequired[bool],
    PromotionTier: NotRequired[int],
    DbInstanceIdentifier: NotRequired[str],
    DbClusterParameterGroupStatus: NotRequired[str],
```

## AwsRdsDbClusterOptionGroupMembershipTypeDef

```python
# AwsRdsDbClusterOptionGroupMembershipTypeDef definition

class AwsRdsDbClusterOptionGroupMembershipTypeDef(TypedDict):
    DbClusterOptionGroupName: NotRequired[str],
    Status: NotRequired[str],
```

## AwsRdsDbDomainMembershipTypeDef

```python
# AwsRdsDbDomainMembershipTypeDef definition

class AwsRdsDbDomainMembershipTypeDef(TypedDict):
    Domain: NotRequired[str],
    Status: NotRequired[str],
    Fqdn: NotRequired[str],
    IamRoleName: NotRequired[str],
```

## AwsRdsDbInstanceVpcSecurityGroupTypeDef

```python
# AwsRdsDbInstanceVpcSecurityGroupTypeDef definition

class AwsRdsDbInstanceVpcSecurityGroupTypeDef(TypedDict):
    VpcSecurityGroupId: NotRequired[str],
    Status: NotRequired[str],
```

## AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef

```python
# AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef definition

class AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef(TypedDict):
    AttributeName: NotRequired[str],
    AttributeValues: NotRequired[Sequence[str]],
```

## AwsRdsDbInstanceAssociatedRoleTypeDef

```python
# AwsRdsDbInstanceAssociatedRoleTypeDef definition

class AwsRdsDbInstanceAssociatedRoleTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    FeatureName: NotRequired[str],
    Status: NotRequired[str],
```

## AwsRdsDbInstanceEndpointTypeDef

```python
# AwsRdsDbInstanceEndpointTypeDef definition

class AwsRdsDbInstanceEndpointTypeDef(TypedDict):
    Address: NotRequired[str],
    Port: NotRequired[int],
    HostedZoneId: NotRequired[str],
```

## AwsRdsDbOptionGroupMembershipTypeDef

```python
# AwsRdsDbOptionGroupMembershipTypeDef definition

class AwsRdsDbOptionGroupMembershipTypeDef(TypedDict):
    OptionGroupName: NotRequired[str],
    Status: NotRequired[str],
```

## AwsRdsDbParameterGroupTypeDef

```python
# AwsRdsDbParameterGroupTypeDef definition

class AwsRdsDbParameterGroupTypeDef(TypedDict):
    DbParameterGroupName: NotRequired[str],
    ParameterApplyStatus: NotRequired[str],
```

## AwsRdsDbProcessorFeatureTypeDef

```python
# AwsRdsDbProcessorFeatureTypeDef definition

class AwsRdsDbProcessorFeatureTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## AwsRdsDbStatusInfoTypeDef

```python
# AwsRdsDbStatusInfoTypeDef definition

class AwsRdsDbStatusInfoTypeDef(TypedDict):
    StatusType: NotRequired[str],
    Normal: NotRequired[bool],
    Status: NotRequired[str],
    Message: NotRequired[str],
```

## AwsRdsPendingCloudWatchLogsExportsTypeDef

```python
# AwsRdsPendingCloudWatchLogsExportsTypeDef definition

class AwsRdsPendingCloudWatchLogsExportsTypeDef(TypedDict):
    LogTypesToEnable: NotRequired[Sequence[str]],
    LogTypesToDisable: NotRequired[Sequence[str]],
```

## AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef

```python
# AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef definition

class AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef(TypedDict):
    Ec2SecurityGroupId: NotRequired[str],
    Ec2SecurityGroupName: NotRequired[str],
    Ec2SecurityGroupOwnerId: NotRequired[str],
    Status: NotRequired[str],
```

## AwsRdsDbSecurityGroupIpRangeTypeDef

```python
# AwsRdsDbSecurityGroupIpRangeTypeDef definition

class AwsRdsDbSecurityGroupIpRangeTypeDef(TypedDict):
    CidrIp: NotRequired[str],
    Status: NotRequired[str],
```

## AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef

```python
# AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef definition

class AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef(TypedDict):
    Name: NotRequired[str],
```

## AwsRdsEventSubscriptionDetailsTypeDef

```python
# AwsRdsEventSubscriptionDetailsTypeDef definition

class AwsRdsEventSubscriptionDetailsTypeDef(TypedDict):
    CustSubscriptionId: NotRequired[str],
    CustomerAwsId: NotRequired[str],
    Enabled: NotRequired[bool],
    EventCategoriesList: NotRequired[Sequence[str]],
    EventSubscriptionArn: NotRequired[str],
    SnsTopicArn: NotRequired[str],
    SourceIdsList: NotRequired[Sequence[str]],
    SourceType: NotRequired[str],
    Status: NotRequired[str],
    SubscriptionCreationTime: NotRequired[str],
```

## AwsRedshiftClusterClusterNodeTypeDef

```python
# AwsRedshiftClusterClusterNodeTypeDef definition

class AwsRedshiftClusterClusterNodeTypeDef(TypedDict):
    NodeRole: NotRequired[str],
    PrivateIpAddress: NotRequired[str],
    PublicIpAddress: NotRequired[str],
```

## AwsRedshiftClusterClusterParameterStatusTypeDef

```python
# AwsRedshiftClusterClusterParameterStatusTypeDef definition

class AwsRedshiftClusterClusterParameterStatusTypeDef(TypedDict):
    ParameterName: NotRequired[str],
    ParameterApplyStatus: NotRequired[str],
    ParameterApplyErrorDescription: NotRequired[str],
```

## AwsRedshiftClusterClusterSecurityGroupTypeDef

```python
# AwsRedshiftClusterClusterSecurityGroupTypeDef definition

class AwsRedshiftClusterClusterSecurityGroupTypeDef(TypedDict):
    ClusterSecurityGroupName: NotRequired[str],
    Status: NotRequired[str],
```

## AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef

```python
# AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef definition

class AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef(TypedDict):
    DestinationRegion: NotRequired[str],
    ManualSnapshotRetentionPeriod: NotRequired[int],
    RetentionPeriod: NotRequired[int],
    SnapshotCopyGrantName: NotRequired[str],
```

## AwsRedshiftClusterDeferredMaintenanceWindowTypeDef

```python
# AwsRedshiftClusterDeferredMaintenanceWindowTypeDef definition

class AwsRedshiftClusterDeferredMaintenanceWindowTypeDef(TypedDict):
    DeferMaintenanceEndTime: NotRequired[str],
    DeferMaintenanceIdentifier: NotRequired[str],
    DeferMaintenanceStartTime: NotRequired[str],
```

## AwsRedshiftClusterElasticIpStatusTypeDef

```python
# AwsRedshiftClusterElasticIpStatusTypeDef definition

class AwsRedshiftClusterElasticIpStatusTypeDef(TypedDict):
    ElasticIp: NotRequired[str],
    Status: NotRequired[str],
```

## AwsRedshiftClusterEndpointTypeDef

```python
# AwsRedshiftClusterEndpointTypeDef definition

class AwsRedshiftClusterEndpointTypeDef(TypedDict):
    Address: NotRequired[str],
    Port: NotRequired[int],
```

## AwsRedshiftClusterHsmStatusTypeDef

```python
# AwsRedshiftClusterHsmStatusTypeDef definition

class AwsRedshiftClusterHsmStatusTypeDef(TypedDict):
    HsmClientCertificateIdentifier: NotRequired[str],
    HsmConfigurationIdentifier: NotRequired[str],
    Status: NotRequired[str],
```

## AwsRedshiftClusterIamRoleTypeDef

```python
# AwsRedshiftClusterIamRoleTypeDef definition

class AwsRedshiftClusterIamRoleTypeDef(TypedDict):
    ApplyStatus: NotRequired[str],
    IamRoleArn: NotRequired[str],
```

## AwsRedshiftClusterLoggingStatusTypeDef

```python
# AwsRedshiftClusterLoggingStatusTypeDef definition

class AwsRedshiftClusterLoggingStatusTypeDef(TypedDict):
    BucketName: NotRequired[str],
    LastFailureMessage: NotRequired[str],
    LastFailureTime: NotRequired[str],
    LastSuccessfulDeliveryTime: NotRequired[str],
    LoggingEnabled: NotRequired[bool],
    S3KeyPrefix: NotRequired[str],
```

## AwsRedshiftClusterPendingModifiedValuesTypeDef

```python
# AwsRedshiftClusterPendingModifiedValuesTypeDef definition

class AwsRedshiftClusterPendingModifiedValuesTypeDef(TypedDict):
    AutomatedSnapshotRetentionPeriod: NotRequired[int],
    ClusterIdentifier: NotRequired[str],
    ClusterType: NotRequired[str],
    ClusterVersion: NotRequired[str],
    EncryptionType: NotRequired[str],
    EnhancedVpcRouting: NotRequired[bool],
    MaintenanceTrackName: NotRequired[str],
    MasterUserPassword: NotRequired[str],
    NodeType: NotRequired[str],
    NumberOfNodes: NotRequired[int],
    PubliclyAccessible: NotRequired[bool],
```

## AwsRedshiftClusterResizeInfoTypeDef

```python
# AwsRedshiftClusterResizeInfoTypeDef definition

class AwsRedshiftClusterResizeInfoTypeDef(TypedDict):
    AllowCancelResize: NotRequired[bool],
    ResizeType: NotRequired[str],
```

## AwsRedshiftClusterRestoreStatusTypeDef

```python
# AwsRedshiftClusterRestoreStatusTypeDef definition

class AwsRedshiftClusterRestoreStatusTypeDef(TypedDict):
    CurrentRestoreRateInMegaBytesPerSecond: NotRequired[float],
    ElapsedTimeInSeconds: NotRequired[int],
    EstimatedTimeToCompletionInSeconds: NotRequired[int],
    ProgressInMegaBytes: NotRequired[int],
    SnapshotSizeInMegaBytes: NotRequired[int],
    Status: NotRequired[str],
```

## AwsRedshiftClusterVpcSecurityGroupTypeDef

```python
# AwsRedshiftClusterVpcSecurityGroupTypeDef definition

class AwsRedshiftClusterVpcSecurityGroupTypeDef(TypedDict):
    Status: NotRequired[str],
    VpcSecurityGroupId: NotRequired[str],
```

## AwsS3AccountPublicAccessBlockDetailsTypeDef

```python
# AwsS3AccountPublicAccessBlockDetailsTypeDef definition

class AwsS3AccountPublicAccessBlockDetailsTypeDef(TypedDict):
    BlockPublicAcls: NotRequired[bool],
    BlockPublicPolicy: NotRequired[bool],
    IgnorePublicAcls: NotRequired[bool],
    RestrictPublicBuckets: NotRequired[bool],
```

## AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef

```python
# AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef definition

class AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef(TypedDict):
    DaysAfterInitiation: NotRequired[int],
```

## AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef

```python
# AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef definition

class AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef(TypedDict):
    Days: NotRequired[int],
    StorageClass: NotRequired[str],
```

## AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef

```python
# AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef definition

class AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef(TypedDict):
    Date: NotRequired[str],
    Days: NotRequired[int],
    StorageClass: NotRequired[str],
```

## AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef

```python
# AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef definition

class AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef

```python
# AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef definition

class AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## AwsS3BucketBucketVersioningConfigurationTypeDef

```python
# AwsS3BucketBucketVersioningConfigurationTypeDef definition

class AwsS3BucketBucketVersioningConfigurationTypeDef(TypedDict):
    IsMfaDeleteEnabled: NotRequired[bool],
    Status: NotRequired[str],
```

## AwsS3BucketLoggingConfigurationTypeDef

```python
# AwsS3BucketLoggingConfigurationTypeDef definition

class AwsS3BucketLoggingConfigurationTypeDef(TypedDict):
    DestinationBucketName: NotRequired[str],
    LogFilePrefix: NotRequired[str],
```

## AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef

```python
# AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef definition

class AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef(TypedDict):
    Name: NotRequired[AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType],  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType](./literals.md#awss3bucketnotificationconfigurations3keyfilterrulenametype) 
## AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef

```python
# AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef definition

class AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef(TypedDict):
    Days: NotRequired[int],
    Mode: NotRequired[str],
    Years: NotRequired[int],
```

## AwsS3BucketServerSideEncryptionByDefaultTypeDef

```python
# AwsS3BucketServerSideEncryptionByDefaultTypeDef definition

class AwsS3BucketServerSideEncryptionByDefaultTypeDef(TypedDict):
    SSEAlgorithm: NotRequired[str],
    KMSMasterKeyID: NotRequired[str],
```

## AwsS3BucketWebsiteConfigurationRedirectToTypeDef

```python
# AwsS3BucketWebsiteConfigurationRedirectToTypeDef definition

class AwsS3BucketWebsiteConfigurationRedirectToTypeDef(TypedDict):
    Hostname: NotRequired[str],
    Protocol: NotRequired[str],
```

## AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef

```python
# AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef definition

class AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef(TypedDict):
    HttpErrorCodeReturnedEquals: NotRequired[str],
    KeyPrefixEquals: NotRequired[str],
```

## AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef

```python
# AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef definition

class AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef(TypedDict):
    Hostname: NotRequired[str],
    HttpRedirectCode: NotRequired[str],
    Protocol: NotRequired[str],
    ReplaceKeyPrefixWith: NotRequired[str],
    ReplaceKeyWith: NotRequired[str],
```

## AwsS3ObjectDetailsTypeDef

```python
# AwsS3ObjectDetailsTypeDef definition

class AwsS3ObjectDetailsTypeDef(TypedDict):
    LastModified: NotRequired[str],
    ETag: NotRequired[str],
    VersionId: NotRequired[str],
    ContentType: NotRequired[str],
    ServerSideEncryption: NotRequired[str],
    SSEKMSKeyId: NotRequired[str],
```

## AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef

```python
# AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef definition

class AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef(TypedDict):
    MinimumInstanceMetadataServiceVersion: NotRequired[str],
```

## AwsSecretsManagerSecretRotationRulesTypeDef

```python
# AwsSecretsManagerSecretRotationRulesTypeDef definition

class AwsSecretsManagerSecretRotationRulesTypeDef(TypedDict):
    AutomaticallyAfterDays: NotRequired[int],
```

## BooleanFilterTypeDef

```python
# BooleanFilterTypeDef definition

class BooleanFilterTypeDef(TypedDict):
    Value: NotRequired[bool],
```

## IpFilterTypeDef

```python
# IpFilterTypeDef definition

class IpFilterTypeDef(TypedDict):
    Cidr: NotRequired[str],
```

## KeywordFilterTypeDef

```python
# KeywordFilterTypeDef definition

class KeywordFilterTypeDef(TypedDict):
    Value: NotRequired[str],
```

## AwsSecurityFindingIdentifierTypeDef

```python
# AwsSecurityFindingIdentifierTypeDef definition

class AwsSecurityFindingIdentifierTypeDef(TypedDict):
    Id: str,
    ProductArn: str,
```

## MalwareTypeDef

```python
# MalwareTypeDef definition

class MalwareTypeDef(TypedDict):
    Name: str,
    Type: NotRequired[MalwareTypeType],  # (1)
    Path: NotRequired[str],
    State: NotRequired[MalwareStateType],  # (2)
```

1. See [:material-code-brackets: MalwareTypeType](./literals.md#malwaretypetype) 
2. See [:material-code-brackets: MalwareStateType](./literals.md#malwarestatetype) 
## NoteTypeDef

```python
# NoteTypeDef definition

class NoteTypeDef(TypedDict):
    Text: str,
    UpdatedBy: str,
    UpdatedAt: str,
```

## PatchSummaryTypeDef

```python
# PatchSummaryTypeDef definition

class PatchSummaryTypeDef(TypedDict):
    Id: str,
    InstalledCount: NotRequired[int],
    MissingCount: NotRequired[int],
    FailedCount: NotRequired[int],
    InstalledOtherCount: NotRequired[int],
    InstalledRejectedCount: NotRequired[int],
    InstalledPendingReboot: NotRequired[int],
    OperationStartTime: NotRequired[str],
    OperationEndTime: NotRequired[str],
    RebootOption: NotRequired[str],
    Operation: NotRequired[str],
```

## ProcessDetailsTypeDef

```python
# ProcessDetailsTypeDef definition

class ProcessDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Path: NotRequired[str],
    Pid: NotRequired[int],
    ParentPid: NotRequired[int],
    LaunchedAt: NotRequired[str],
    TerminatedAt: NotRequired[str],
```

## SeverityTypeDef

```python
# SeverityTypeDef definition

class SeverityTypeDef(TypedDict):
    Product: NotRequired[float],
    Label: NotRequired[SeverityLabelType],  # (1)
    Normalized: NotRequired[int],
    Original: NotRequired[str],
```

1. See [:material-code-brackets: SeverityLabelType](./literals.md#severitylabeltype) 
## ThreatIntelIndicatorTypeDef

```python
# ThreatIntelIndicatorTypeDef definition

class ThreatIntelIndicatorTypeDef(TypedDict):
    Type: NotRequired[ThreatIntelIndicatorTypeType],  # (1)
    Value: NotRequired[str],
    Category: NotRequired[ThreatIntelIndicatorCategoryType],  # (2)
    LastObservedAt: NotRequired[str],
    Source: NotRequired[str],
    SourceUrl: NotRequired[str],
```

1. See [:material-code-brackets: ThreatIntelIndicatorTypeType](./literals.md#threatintelindicatortypetype) 
2. See [:material-code-brackets: ThreatIntelIndicatorCategoryType](./literals.md#threatintelindicatorcategorytype) 
## WorkflowTypeDef

```python
# WorkflowTypeDef definition

class WorkflowTypeDef(TypedDict):
    Status: NotRequired[WorkflowStatusType],  # (1)
```

1. See [:material-code-brackets: WorkflowStatusType](./literals.md#workflowstatustype) 
## AwsSnsTopicSubscriptionTypeDef

```python
# AwsSnsTopicSubscriptionTypeDef definition

class AwsSnsTopicSubscriptionTypeDef(TypedDict):
    Endpoint: NotRequired[str],
    Protocol: NotRequired[str],
```

## AwsSqsQueueDetailsTypeDef

```python
# AwsSqsQueueDetailsTypeDef definition

class AwsSqsQueueDetailsTypeDef(TypedDict):
    KmsDataKeyReusePeriodSeconds: NotRequired[int],
    KmsMasterKeyId: NotRequired[str],
    QueueName: NotRequired[str],
    DeadLetterTargetArn: NotRequired[str],
```

## AwsSsmComplianceSummaryTypeDef

```python
# AwsSsmComplianceSummaryTypeDef definition

class AwsSsmComplianceSummaryTypeDef(TypedDict):
    Status: NotRequired[str],
    CompliantCriticalCount: NotRequired[int],
    CompliantHighCount: NotRequired[int],
    CompliantMediumCount: NotRequired[int],
    ExecutionType: NotRequired[str],
    NonCompliantCriticalCount: NotRequired[int],
    CompliantInformationalCount: NotRequired[int],
    NonCompliantInformationalCount: NotRequired[int],
    CompliantUnspecifiedCount: NotRequired[int],
    NonCompliantLowCount: NotRequired[int],
    NonCompliantHighCount: NotRequired[int],
    CompliantLowCount: NotRequired[int],
    ComplianceType: NotRequired[str],
    PatchBaselineId: NotRequired[str],
    OverallSeverity: NotRequired[str],
    NonCompliantMediumCount: NotRequired[int],
    NonCompliantUnspecifiedCount: NotRequired[int],
    PatchGroup: NotRequired[str],
```

## AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef

```python
# AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef definition

class AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef

```python
# AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef definition

class AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef(TypedDict):
    LogGroupArn: NotRequired[str],
```

## AwsWafRateBasedRuleMatchPredicateTypeDef

```python
# AwsWafRateBasedRuleMatchPredicateTypeDef definition

class AwsWafRateBasedRuleMatchPredicateTypeDef(TypedDict):
    DataId: NotRequired[str],
    Negated: NotRequired[bool],
    Type: NotRequired[str],
```

## AwsWafRegionalRateBasedRuleMatchPredicateTypeDef

```python
# AwsWafRegionalRateBasedRuleMatchPredicateTypeDef definition

class AwsWafRegionalRateBasedRuleMatchPredicateTypeDef(TypedDict):
    DataId: NotRequired[str],
    Negated: NotRequired[bool],
    Type: NotRequired[str],
```

## AwsWafRegionalRulePredicateListDetailsTypeDef

```python
# AwsWafRegionalRulePredicateListDetailsTypeDef definition

class AwsWafRegionalRulePredicateListDetailsTypeDef(TypedDict):
    DataId: NotRequired[str],
    Negated: NotRequired[bool],
    Type: NotRequired[str],
```

## AwsWafRegionalRuleGroupRulesActionDetailsTypeDef

```python
# AwsWafRegionalRuleGroupRulesActionDetailsTypeDef definition

class AwsWafRegionalRuleGroupRulesActionDetailsTypeDef(TypedDict):
    Type: NotRequired[str],
```

## AwsWafRegionalWebAclRulesListActionDetailsTypeDef

```python
# AwsWafRegionalWebAclRulesListActionDetailsTypeDef definition

class AwsWafRegionalWebAclRulesListActionDetailsTypeDef(TypedDict):
    Type: NotRequired[str],
```

## AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef

```python
# AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef definition

class AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef(TypedDict):
    Type: NotRequired[str],
```

## AwsWafRulePredicateListDetailsTypeDef

```python
# AwsWafRulePredicateListDetailsTypeDef definition

class AwsWafRulePredicateListDetailsTypeDef(TypedDict):
    DataId: NotRequired[str],
    Negated: NotRequired[bool],
    Type: NotRequired[str],
```

## AwsWafRuleGroupRulesActionDetailsTypeDef

```python
# AwsWafRuleGroupRulesActionDetailsTypeDef definition

class AwsWafRuleGroupRulesActionDetailsTypeDef(TypedDict):
    Type: NotRequired[str],
```

## WafActionTypeDef

```python
# WafActionTypeDef definition

class WafActionTypeDef(TypedDict):
    Type: NotRequired[str],
```

## WafExcludedRuleTypeDef

```python
# WafExcludedRuleTypeDef definition

class WafExcludedRuleTypeDef(TypedDict):
    RuleId: NotRequired[str],
```

## WafOverrideActionTypeDef

```python
# WafOverrideActionTypeDef definition

class WafOverrideActionTypeDef(TypedDict):
    Type: NotRequired[str],
```

## AwsWafv2CustomHttpHeaderTypeDef

```python
# AwsWafv2CustomHttpHeaderTypeDef definition

class AwsWafv2CustomHttpHeaderTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## AwsWafv2VisibilityConfigDetailsTypeDef

```python
# AwsWafv2VisibilityConfigDetailsTypeDef definition

class AwsWafv2VisibilityConfigDetailsTypeDef(TypedDict):
    CloudWatchMetricsEnabled: NotRequired[bool],
    MetricName: NotRequired[str],
    SampledRequestsEnabled: NotRequired[bool],
```

## AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef

```python
# AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef definition

class AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef(TypedDict):
    ImmunityTime: NotRequired[int],
```

## AwsXrayEncryptionConfigDetailsTypeDef

```python
# AwsXrayEncryptionConfigDetailsTypeDef definition

class AwsXrayEncryptionConfigDetailsTypeDef(TypedDict):
    KeyId: NotRequired[str],
    Status: NotRequired[str],
    Type: NotRequired[str],
```

## BatchDeleteAutomationRulesRequestRequestTypeDef

```python
# BatchDeleteAutomationRulesRequestRequestTypeDef definition

class BatchDeleteAutomationRulesRequestRequestTypeDef(TypedDict):
    AutomationRulesArns: Sequence[str],
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

## UnprocessedAutomationRuleTypeDef

```python
# UnprocessedAutomationRuleTypeDef definition

class UnprocessedAutomationRuleTypeDef(TypedDict):
    RuleArn: NotRequired[str],
    ErrorCode: NotRequired[int],
    ErrorMessage: NotRequired[str],
```

## BatchDisableStandardsRequestRequestTypeDef

```python
# BatchDisableStandardsRequestRequestTypeDef definition

class BatchDisableStandardsRequestRequestTypeDef(TypedDict):
    StandardsSubscriptionArns: Sequence[str],
```

## StandardsSubscriptionRequestTypeDef

```python
# StandardsSubscriptionRequestTypeDef definition

class StandardsSubscriptionRequestTypeDef(TypedDict):
    StandardsArn: str,
    StandardsInput: NotRequired[Mapping[str, str]],
```

## BatchGetAutomationRulesRequestRequestTypeDef

```python
# BatchGetAutomationRulesRequestRequestTypeDef definition

class BatchGetAutomationRulesRequestRequestTypeDef(TypedDict):
    AutomationRulesArns: Sequence[str],
```

## BatchGetSecurityControlsRequestRequestTypeDef

```python
# BatchGetSecurityControlsRequestRequestTypeDef definition

class BatchGetSecurityControlsRequestRequestTypeDef(TypedDict):
    SecurityControlIds: Sequence[str],
```

## SecurityControlTypeDef

```python
# SecurityControlTypeDef definition

class SecurityControlTypeDef(TypedDict):
    SecurityControlId: str,
    SecurityControlArn: str,
    Title: str,
    Description: str,
    RemediationUrl: str,
    SeverityRating: SeverityRatingType,  # (1)
    SecurityControlStatus: ControlStatusType,  # (2)
```

1. See [:material-code-brackets: SeverityRatingType](./literals.md#severityratingtype) 
2. See [:material-code-brackets: ControlStatusType](./literals.md#controlstatustype) 
## UnprocessedSecurityControlTypeDef

```python
# UnprocessedSecurityControlTypeDef definition

class UnprocessedSecurityControlTypeDef(TypedDict):
    SecurityControlId: str,
    ErrorCode: UnprocessedErrorCodeType,  # (1)
    ErrorReason: NotRequired[str],
```

1. See [:material-code-brackets: UnprocessedErrorCodeType](./literals.md#unprocessederrorcodetype) 
## StandardsControlAssociationIdTypeDef

```python
# StandardsControlAssociationIdTypeDef definition

class StandardsControlAssociationIdTypeDef(TypedDict):
    SecurityControlId: str,
    StandardsArn: str,
```

## StandardsControlAssociationDetailTypeDef

```python
# StandardsControlAssociationDetailTypeDef definition

class StandardsControlAssociationDetailTypeDef(TypedDict):
    StandardsArn: str,
    SecurityControlId: str,
    SecurityControlArn: str,
    AssociationStatus: AssociationStatusType,  # (1)
    RelatedRequirements: NotRequired[List[str]],
    UpdatedAt: NotRequired[datetime],
    UpdatedReason: NotRequired[str],
    StandardsControlTitle: NotRequired[str],
    StandardsControlDescription: NotRequired[str],
    StandardsControlArns: NotRequired[List[str]],
```

1. See [:material-code-brackets: AssociationStatusType](./literals.md#associationstatustype) 
## ImportFindingsErrorTypeDef

```python
# ImportFindingsErrorTypeDef definition

class ImportFindingsErrorTypeDef(TypedDict):
    Id: str,
    ErrorCode: str,
    ErrorMessage: str,
```

## StandardsControlAssociationUpdateTypeDef

```python
# StandardsControlAssociationUpdateTypeDef definition

class StandardsControlAssociationUpdateTypeDef(TypedDict):
    StandardsArn: str,
    SecurityControlId: str,
    AssociationStatus: AssociationStatusType,  # (1)
    UpdatedReason: NotRequired[str],
```

1. See [:material-code-brackets: AssociationStatusType](./literals.md#associationstatustype) 
## CellTypeDef

```python
# CellTypeDef definition

class CellTypeDef(TypedDict):
    Column: NotRequired[int],
    Row: NotRequired[int],
    ColumnName: NotRequired[str],
    CellReference: NotRequired[str],
```

## ClassificationStatusTypeDef

```python
# ClassificationStatusTypeDef definition

class ClassificationStatusTypeDef(TypedDict):
    Code: NotRequired[str],
    Reason: NotRequired[str],
```

## StatusReasonTypeDef

```python
# StatusReasonTypeDef definition

class StatusReasonTypeDef(TypedDict):
    ReasonCode: str,
    Description: NotRequired[str],
```

## VolumeMountTypeDef

```python
# VolumeMountTypeDef definition

class VolumeMountTypeDef(TypedDict):
    Name: NotRequired[str],
    MountPath: NotRequired[str],
```

## CreateActionTargetRequestRequestTypeDef

```python
# CreateActionTargetRequestRequestTypeDef definition

class CreateActionTargetRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: str,
    Id: str,
```

## CreateFindingAggregatorRequestRequestTypeDef

```python
# CreateFindingAggregatorRequestRequestTypeDef definition

class CreateFindingAggregatorRequestRequestTypeDef(TypedDict):
    RegionLinkingMode: str,
    Regions: NotRequired[Sequence[str]],
```

## ResultTypeDef

```python
# ResultTypeDef definition

class ResultTypeDef(TypedDict):
    AccountId: NotRequired[str],
    ProcessingResult: NotRequired[str],
```

## DateRangeTypeDef

```python
# DateRangeTypeDef definition

class DateRangeTypeDef(TypedDict):
    Value: NotRequired[int],
    Unit: NotRequired[DateRangeUnitType],  # (1)
```

1. See [:material-code-brackets: DateRangeUnitType](./literals.md#daterangeunittype) 
## DeclineInvitationsRequestRequestTypeDef

```python
# DeclineInvitationsRequestRequestTypeDef definition

class DeclineInvitationsRequestRequestTypeDef(TypedDict):
    AccountIds: Sequence[str],
```

## DeleteActionTargetRequestRequestTypeDef

```python
# DeleteActionTargetRequestRequestTypeDef definition

class DeleteActionTargetRequestRequestTypeDef(TypedDict):
    ActionTargetArn: str,
```

## DeleteFindingAggregatorRequestRequestTypeDef

```python
# DeleteFindingAggregatorRequestRequestTypeDef definition

class DeleteFindingAggregatorRequestRequestTypeDef(TypedDict):
    FindingAggregatorArn: str,
```

## DeleteInsightRequestRequestTypeDef

```python
# DeleteInsightRequestRequestTypeDef definition

class DeleteInsightRequestRequestTypeDef(TypedDict):
    InsightArn: str,
```

## DeleteInvitationsRequestRequestTypeDef

```python
# DeleteInvitationsRequestRequestTypeDef definition

class DeleteInvitationsRequestRequestTypeDef(TypedDict):
    AccountIds: Sequence[str],
```

## DeleteMembersRequestRequestTypeDef

```python
# DeleteMembersRequestRequestTypeDef definition

class DeleteMembersRequestRequestTypeDef(TypedDict):
    AccountIds: Sequence[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeActionTargetsRequestRequestTypeDef

```python
# DescribeActionTargetsRequestRequestTypeDef definition

class DescribeActionTargetsRequestRequestTypeDef(TypedDict):
    ActionTargetArns: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeHubRequestRequestTypeDef

```python
# DescribeHubRequestRequestTypeDef definition

class DescribeHubRequestRequestTypeDef(TypedDict):
    HubArn: NotRequired[str],
```

## DescribeProductsRequestRequestTypeDef

```python
# DescribeProductsRequestRequestTypeDef definition

class DescribeProductsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ProductArn: NotRequired[str],
```

## ProductTypeDef

```python
# ProductTypeDef definition

class ProductTypeDef(TypedDict):
    ProductArn: str,
    ProductName: NotRequired[str],
    CompanyName: NotRequired[str],
    Description: NotRequired[str],
    Categories: NotRequired[List[str]],
    IntegrationTypes: NotRequired[List[IntegrationTypeType]],  # (1)
    MarketplaceUrl: NotRequired[str],
    ActivationUrl: NotRequired[str],
    ProductSubscriptionResourcePolicy: NotRequired[str],
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
## DescribeStandardsControlsRequestRequestTypeDef

```python
# DescribeStandardsControlsRequestRequestTypeDef definition

class DescribeStandardsControlsRequestRequestTypeDef(TypedDict):
    StandardsSubscriptionArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## StandardsControlTypeDef

```python
# StandardsControlTypeDef definition

class StandardsControlTypeDef(TypedDict):
    StandardsControlArn: NotRequired[str],
    ControlStatus: NotRequired[ControlStatusType],  # (1)
    DisabledReason: NotRequired[str],
    ControlStatusUpdatedAt: NotRequired[datetime],
    ControlId: NotRequired[str],
    Title: NotRequired[str],
    Description: NotRequired[str],
    RemediationUrl: NotRequired[str],
    SeverityRating: NotRequired[SeverityRatingType],  # (2)
    RelatedRequirements: NotRequired[List[str]],
```

1. See [:material-code-brackets: ControlStatusType](./literals.md#controlstatustype) 
2. See [:material-code-brackets: SeverityRatingType](./literals.md#severityratingtype) 
## DescribeStandardsRequestRequestTypeDef

```python
# DescribeStandardsRequestRequestTypeDef definition

class DescribeStandardsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DisableImportFindingsForProductRequestRequestTypeDef

```python
# DisableImportFindingsForProductRequestRequestTypeDef definition

class DisableImportFindingsForProductRequestRequestTypeDef(TypedDict):
    ProductSubscriptionArn: str,
```

## DisableOrganizationAdminAccountRequestRequestTypeDef

```python
# DisableOrganizationAdminAccountRequestRequestTypeDef definition

class DisableOrganizationAdminAccountRequestRequestTypeDef(TypedDict):
    AdminAccountId: str,
```

## DisassociateMembersRequestRequestTypeDef

```python
# DisassociateMembersRequestRequestTypeDef definition

class DisassociateMembersRequestRequestTypeDef(TypedDict):
    AccountIds: Sequence[str],
```

## EnableImportFindingsForProductRequestRequestTypeDef

```python
# EnableImportFindingsForProductRequestRequestTypeDef definition

class EnableImportFindingsForProductRequestRequestTypeDef(TypedDict):
    ProductArn: str,
```

## EnableOrganizationAdminAccountRequestRequestTypeDef

```python
# EnableOrganizationAdminAccountRequestRequestTypeDef definition

class EnableOrganizationAdminAccountRequestRequestTypeDef(TypedDict):
    AdminAccountId: str,
```

## EnableSecurityHubRequestRequestTypeDef

```python
# EnableSecurityHubRequestRequestTypeDef definition

class EnableSecurityHubRequestRequestTypeDef(TypedDict):
    Tags: NotRequired[Mapping[str, str]],
    EnableDefaultStandards: NotRequired[bool],
    ControlFindingGenerator: NotRequired[ControlFindingGeneratorType],  # (1)
```

1. See [:material-code-brackets: ControlFindingGeneratorType](./literals.md#controlfindinggeneratortype) 
## FilePathsTypeDef

```python
# FilePathsTypeDef definition

class FilePathsTypeDef(TypedDict):
    FilePath: NotRequired[str],
    FileName: NotRequired[str],
    ResourceId: NotRequired[str],
    Hash: NotRequired[str],
```

## FindingAggregatorTypeDef

```python
# FindingAggregatorTypeDef definition

class FindingAggregatorTypeDef(TypedDict):
    FindingAggregatorArn: NotRequired[str],
```

## FindingHistoryUpdateSourceTypeDef

```python
# FindingHistoryUpdateSourceTypeDef definition

class FindingHistoryUpdateSourceTypeDef(TypedDict):
    Type: NotRequired[FindingHistoryUpdateSourceTypeType],  # (1)
    Identity: NotRequired[str],
```

1. See [:material-code-brackets: FindingHistoryUpdateSourceTypeType](./literals.md#findinghistoryupdatesourcetypetype) 
## FindingHistoryUpdateTypeDef

```python
# FindingHistoryUpdateTypeDef definition

class FindingHistoryUpdateTypeDef(TypedDict):
    UpdatedField: NotRequired[str],
    OldValue: NotRequired[str],
    NewValue: NotRequired[str],
```

## FindingProviderSeverityTypeDef

```python
# FindingProviderSeverityTypeDef definition

class FindingProviderSeverityTypeDef(TypedDict):
    Label: NotRequired[SeverityLabelType],  # (1)
    Original: NotRequired[str],
```

1. See [:material-code-brackets: SeverityLabelType](./literals.md#severitylabeltype) 
## FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef

```python
# FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef definition

class FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
```

## FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef

```python
# FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef definition

class FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef(TypedDict):
    Priority: NotRequired[int],
    ResourceArn: NotRequired[str],
```

## InvitationTypeDef

```python
# InvitationTypeDef definition

class InvitationTypeDef(TypedDict):
    AccountId: NotRequired[str],
    InvitationId: NotRequired[str],
    InvitedAt: NotRequired[datetime],
    MemberStatus: NotRequired[str],
```

## GetEnabledStandardsRequestRequestTypeDef

```python
# GetEnabledStandardsRequestRequestTypeDef definition

class GetEnabledStandardsRequestRequestTypeDef(TypedDict):
    StandardsSubscriptionArns: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetFindingAggregatorRequestRequestTypeDef

```python
# GetFindingAggregatorRequestRequestTypeDef definition

class GetFindingAggregatorRequestRequestTypeDef(TypedDict):
    FindingAggregatorArn: str,
```

## SortCriterionTypeDef

```python
# SortCriterionTypeDef definition

class SortCriterionTypeDef(TypedDict):
    Field: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## GetInsightResultsRequestRequestTypeDef

```python
# GetInsightResultsRequestRequestTypeDef definition

class GetInsightResultsRequestRequestTypeDef(TypedDict):
    InsightArn: str,
```

## GetInsightsRequestRequestTypeDef

```python
# GetInsightsRequestRequestTypeDef definition

class GetInsightsRequestRequestTypeDef(TypedDict):
    InsightArns: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetMembersRequestRequestTypeDef

```python
# GetMembersRequestRequestTypeDef definition

class GetMembersRequestRequestTypeDef(TypedDict):
    AccountIds: Sequence[str],
```

## MemberTypeDef

```python
# MemberTypeDef definition

class MemberTypeDef(TypedDict):
    AccountId: NotRequired[str],
    Email: NotRequired[str],
    MasterId: NotRequired[str],
    AdministratorId: NotRequired[str],
    MemberStatus: NotRequired[str],
    InvitedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
```

## InsightResultValueTypeDef

```python
# InsightResultValueTypeDef definition

class InsightResultValueTypeDef(TypedDict):
    GroupByAttributeValue: str,
    Count: int,
```

## InviteMembersRequestRequestTypeDef

```python
# InviteMembersRequestRequestTypeDef definition

class InviteMembersRequestRequestTypeDef(TypedDict):
    AccountIds: Sequence[str],
```

## ListAutomationRulesRequestRequestTypeDef

```python
# ListAutomationRulesRequestRequestTypeDef definition

class ListAutomationRulesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListEnabledProductsForImportRequestRequestTypeDef

```python
# ListEnabledProductsForImportRequestRequestTypeDef definition

class ListEnabledProductsForImportRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListFindingAggregatorsRequestRequestTypeDef

```python
# ListFindingAggregatorsRequestRequestTypeDef definition

class ListFindingAggregatorsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListInvitationsRequestRequestTypeDef

```python
# ListInvitationsRequestRequestTypeDef definition

class ListInvitationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListMembersRequestRequestTypeDef

```python
# ListMembersRequestRequestTypeDef definition

class ListMembersRequestRequestTypeDef(TypedDict):
    OnlyAssociated: NotRequired[bool],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListOrganizationAdminAccountsRequestRequestTypeDef

```python
# ListOrganizationAdminAccountsRequestRequestTypeDef definition

class ListOrganizationAdminAccountsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListSecurityControlDefinitionsRequestRequestTypeDef

```python
# ListSecurityControlDefinitionsRequestRequestTypeDef definition

class ListSecurityControlDefinitionsRequestRequestTypeDef(TypedDict):
    StandardsArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SecurityControlDefinitionTypeDef

```python
# SecurityControlDefinitionTypeDef definition

class SecurityControlDefinitionTypeDef(TypedDict):
    SecurityControlId: str,
    Title: str,
    Description: str,
    RemediationUrl: str,
    SeverityRating: SeverityRatingType,  # (1)
    CurrentRegionAvailability: RegionAvailabilityStatusType,  # (2)
```

1. See [:material-code-brackets: SeverityRatingType](./literals.md#severityratingtype) 
2. See [:material-code-brackets: RegionAvailabilityStatusType](./literals.md#regionavailabilitystatustype) 
## ListStandardsControlAssociationsRequestRequestTypeDef

```python
# ListStandardsControlAssociationsRequestRequestTypeDef definition

class ListStandardsControlAssociationsRequestRequestTypeDef(TypedDict):
    SecurityControlId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## StandardsControlAssociationSummaryTypeDef

```python
# StandardsControlAssociationSummaryTypeDef definition

class StandardsControlAssociationSummaryTypeDef(TypedDict):
    StandardsArn: str,
    SecurityControlId: str,
    SecurityControlArn: str,
    AssociationStatus: AssociationStatusType,  # (1)
    RelatedRequirements: NotRequired[List[str]],
    UpdatedAt: NotRequired[datetime],
    UpdatedReason: NotRequired[str],
    StandardsControlTitle: NotRequired[str],
    StandardsControlDescription: NotRequired[str],
```

1. See [:material-code-brackets: AssociationStatusType](./literals.md#associationstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PortRangeTypeDef

```python
# PortRangeTypeDef definition

class PortRangeTypeDef(TypedDict):
    Begin: NotRequired[int],
    End: NotRequired[int],
```

## RangeTypeDef

```python
# RangeTypeDef definition

class RangeTypeDef(TypedDict):
    Start: NotRequired[int],
    End: NotRequired[int],
    StartColumn: NotRequired[int],
```

## RecordTypeDef

```python
# RecordTypeDef definition

class RecordTypeDef(TypedDict):
    JsonPath: NotRequired[str],
    RecordIndex: NotRequired[int],
```

## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    Text: NotRequired[str],
    Url: NotRequired[str],
```

## RuleGroupSourceListDetailsTypeDef

```python
# RuleGroupSourceListDetailsTypeDef definition

class RuleGroupSourceListDetailsTypeDef(TypedDict):
    GeneratedRulesType: NotRequired[str],
    TargetTypes: NotRequired[Sequence[str]],
    Targets: NotRequired[Sequence[str]],
```

## RuleGroupSourceStatefulRulesHeaderDetailsTypeDef

```python
# RuleGroupSourceStatefulRulesHeaderDetailsTypeDef definition

class RuleGroupSourceStatefulRulesHeaderDetailsTypeDef(TypedDict):
    Destination: NotRequired[str],
    DestinationPort: NotRequired[str],
    Direction: NotRequired[str],
    Protocol: NotRequired[str],
    Source: NotRequired[str],
    SourcePort: NotRequired[str],
```

## RuleGroupSourceStatefulRulesOptionsDetailsTypeDef

```python
# RuleGroupSourceStatefulRulesOptionsDetailsTypeDef definition

class RuleGroupSourceStatefulRulesOptionsDetailsTypeDef(TypedDict):
    Keyword: NotRequired[str],
    Settings: NotRequired[Sequence[str]],
```

## RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef

```python
# RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef definition

class RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef(TypedDict):
    FromPort: NotRequired[int],
    ToPort: NotRequired[int],
```

## RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef

```python
# RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef definition

class RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef(TypedDict):
    AddressDefinition: NotRequired[str],
```

## RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef

```python
# RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef definition

class RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef(TypedDict):
    FromPort: NotRequired[int],
    ToPort: NotRequired[int],
```

## RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef

```python
# RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef definition

class RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef(TypedDict):
    AddressDefinition: NotRequired[str],
```

## RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef

```python
# RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef definition

class RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef(TypedDict):
    Flags: NotRequired[Sequence[str]],
    Masks: NotRequired[Sequence[str]],
```

## RuleGroupVariablesIpSetsDetailsTypeDef

```python
# RuleGroupVariablesIpSetsDetailsTypeDef definition

class RuleGroupVariablesIpSetsDetailsTypeDef(TypedDict):
    Definition: NotRequired[Sequence[str]],
```

## RuleGroupVariablesPortSetsDetailsTypeDef

```python
# RuleGroupVariablesPortSetsDetailsTypeDef definition

class RuleGroupVariablesPortSetsDetailsTypeDef(TypedDict):
    Definition: NotRequired[Sequence[str]],
```

## SoftwarePackageTypeDef

```python
# SoftwarePackageTypeDef definition

class SoftwarePackageTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
    Epoch: NotRequired[str],
    Release: NotRequired[str],
    Architecture: NotRequired[str],
    PackageManager: NotRequired[str],
    FilePath: NotRequired[str],
    FixedInVersion: NotRequired[str],
    Remediation: NotRequired[str],
    SourceLayerHash: NotRequired[str],
    SourceLayerArn: NotRequired[str],
```

## StandardsManagedByTypeDef

```python
# StandardsManagedByTypeDef definition

class StandardsManagedByTypeDef(TypedDict):
    Company: NotRequired[str],
    Product: NotRequired[str],
```

## StandardsStatusReasonTypeDef

```python
# StandardsStatusReasonTypeDef definition

class StandardsStatusReasonTypeDef(TypedDict):
    StatusReasonCode: StatusReasonCodeType,  # (1)
```

1. See [:material-code-brackets: StatusReasonCodeType](./literals.md#statusreasoncodetype) 
## StatelessCustomPublishMetricActionDimensionTypeDef

```python
# StatelessCustomPublishMetricActionDimensionTypeDef definition

class StatelessCustomPublishMetricActionDimensionTypeDef(TypedDict):
    Value: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateActionTargetRequestRequestTypeDef

```python
# UpdateActionTargetRequestRequestTypeDef definition

class UpdateActionTargetRequestRequestTypeDef(TypedDict):
    ActionTargetArn: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateFindingAggregatorRequestRequestTypeDef

```python
# UpdateFindingAggregatorRequestRequestTypeDef definition

class UpdateFindingAggregatorRequestRequestTypeDef(TypedDict):
    FindingAggregatorArn: str,
    RegionLinkingMode: str,
    Regions: NotRequired[Sequence[str]],
```

## UpdateOrganizationConfigurationRequestRequestTypeDef

```python
# UpdateOrganizationConfigurationRequestRequestTypeDef definition

class UpdateOrganizationConfigurationRequestRequestTypeDef(TypedDict):
    AutoEnable: bool,
    AutoEnableStandards: NotRequired[AutoEnableStandardsType],  # (1)
```

1. See [:material-code-brackets: AutoEnableStandardsType](./literals.md#autoenablestandardstype) 
## UpdateSecurityHubConfigurationRequestRequestTypeDef

```python
# UpdateSecurityHubConfigurationRequestRequestTypeDef definition

class UpdateSecurityHubConfigurationRequestRequestTypeDef(TypedDict):
    AutoEnableControls: NotRequired[bool],
    ControlFindingGenerator: NotRequired[ControlFindingGeneratorType],  # (1)
```

1. See [:material-code-brackets: ControlFindingGeneratorType](./literals.md#controlfindinggeneratortype) 
## UpdateStandardsControlRequestRequestTypeDef

```python
# UpdateStandardsControlRequestRequestTypeDef definition

class UpdateStandardsControlRequestRequestTypeDef(TypedDict):
    StandardsControlArn: str,
    ControlStatus: NotRequired[ControlStatusType],  # (1)
    DisabledReason: NotRequired[str],
```

1. See [:material-code-brackets: ControlStatusType](./literals.md#controlstatustype) 
## VulnerabilityVendorTypeDef

```python
# VulnerabilityVendorTypeDef definition

class VulnerabilityVendorTypeDef(TypedDict):
    Name: str,
    Url: NotRequired[str],
    VendorSeverity: NotRequired[str],
    VendorCreatedAt: NotRequired[str],
    VendorUpdatedAt: NotRequired[str],
```

## CreateMembersRequestRequestTypeDef

```python
# CreateMembersRequestRequestTypeDef definition

class CreateMembersRequestRequestTypeDef(TypedDict):
    AccountDetails: Sequence[AccountDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AccountDetailsTypeDef](./type_defs.md#accountdetailstypedef) 
## ActionRemoteIpDetailsTypeDef

```python
# ActionRemoteIpDetailsTypeDef definition

class ActionRemoteIpDetailsTypeDef(TypedDict):
    IpAddressV4: NotRequired[str],
    Organization: NotRequired[IpOrganizationDetailsTypeDef],  # (1)
    Country: NotRequired[CountryTypeDef],  # (2)
    City: NotRequired[CityTypeDef],  # (3)
    GeoLocation: NotRequired[GeoLocationTypeDef],  # (4)
```

1. See [:material-code-braces: IpOrganizationDetailsTypeDef](./type_defs.md#iporganizationdetailstypedef) 
2. See [:material-code-braces: CountryTypeDef](./type_defs.md#countrytypedef) 
3. See [:material-code-braces: CityTypeDef](./type_defs.md#citytypedef) 
4. See [:material-code-braces: GeoLocationTypeDef](./type_defs.md#geolocationtypedef) 
## CvssTypeDef

```python
# CvssTypeDef definition

class CvssTypeDef(TypedDict):
    Version: NotRequired[str],
    BaseScore: NotRequired[float],
    BaseVector: NotRequired[str],
    Source: NotRequired[str],
    Adjustments: NotRequired[Sequence[AdjustmentTypeDef]],  # (1)
```

1. See [:material-code-braces: AdjustmentTypeDef](./type_defs.md#adjustmenttypedef) 
## AssociationSetDetailsTypeDef

```python
# AssociationSetDetailsTypeDef definition

class AssociationSetDetailsTypeDef(TypedDict):
    AssociationState: NotRequired[AssociationStateDetailsTypeDef],  # (1)
    GatewayId: NotRequired[str],
    Main: NotRequired[bool],
    RouteTableAssociationId: NotRequired[str],
    RouteTableId: NotRequired[str],
    SubnetId: NotRequired[str],
```

1. See [:material-code-braces: AssociationStateDetailsTypeDef](./type_defs.md#associationstatedetailstypedef) 
## AutomationRulesFindingFieldsUpdateTypeDef

```python
# AutomationRulesFindingFieldsUpdateTypeDef definition

class AutomationRulesFindingFieldsUpdateTypeDef(TypedDict):
    Note: NotRequired[NoteUpdateTypeDef],  # (1)
    Severity: NotRequired[SeverityUpdateTypeDef],  # (2)
    VerificationState: NotRequired[VerificationStateType],  # (3)
    Confidence: NotRequired[int],
    Criticality: NotRequired[int],
    Types: NotRequired[List[str]],
    UserDefinedFields: NotRequired[Dict[str, str]],
    Workflow: NotRequired[WorkflowUpdateTypeDef],  # (4)
    RelatedFindings: NotRequired[List[RelatedFindingTypeDef]],  # (5)
```

1. See [:material-code-braces: NoteUpdateTypeDef](./type_defs.md#noteupdatetypedef) 
2. See [:material-code-braces: SeverityUpdateTypeDef](./type_defs.md#severityupdatetypedef) 
3. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
4. See [:material-code-braces: WorkflowUpdateTypeDef](./type_defs.md#workflowupdatetypedef) 
5. See [:material-code-braces: RelatedFindingTypeDef](./type_defs.md#relatedfindingtypedef) 
## AwsAmazonMqBrokerLogsDetailsTypeDef

```python
# AwsAmazonMqBrokerLogsDetailsTypeDef definition

class AwsAmazonMqBrokerLogsDetailsTypeDef(TypedDict):
    Audit: NotRequired[bool],
    General: NotRequired[bool],
    AuditLogGroup: NotRequired[str],
    GeneralLogGroup: NotRequired[str],
    Pending: NotRequired[AwsAmazonMqBrokerLogsPendingDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsAmazonMqBrokerLogsPendingDetailsTypeDef](./type_defs.md#awsamazonmqbrokerlogspendingdetailstypedef) 
## AwsApiGatewayRestApiDetailsTypeDef

```python
# AwsApiGatewayRestApiDetailsTypeDef definition

class AwsApiGatewayRestApiDetailsTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    CreatedDate: NotRequired[str],
    Version: NotRequired[str],
    BinaryMediaTypes: NotRequired[Sequence[str]],
    MinimumCompressionSize: NotRequired[int],
    ApiKeySource: NotRequired[str],
    EndpointConfiguration: NotRequired[AwsApiGatewayEndpointConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AwsApiGatewayEndpointConfigurationTypeDef](./type_defs.md#awsapigatewayendpointconfigurationtypedef) 
## AwsApiGatewayStageDetailsTypeDef

```python
# AwsApiGatewayStageDetailsTypeDef definition

class AwsApiGatewayStageDetailsTypeDef(TypedDict):
    DeploymentId: NotRequired[str],
    ClientCertificateId: NotRequired[str],
    StageName: NotRequired[str],
    Description: NotRequired[str],
    CacheClusterEnabled: NotRequired[bool],
    CacheClusterSize: NotRequired[str],
    CacheClusterStatus: NotRequired[str],
    MethodSettings: NotRequired[Sequence[AwsApiGatewayMethodSettingsTypeDef]],  # (1)
    Variables: NotRequired[Mapping[str, str]],
    DocumentationVersion: NotRequired[str],
    AccessLogSettings: NotRequired[AwsApiGatewayAccessLogSettingsTypeDef],  # (2)
    CanarySettings: NotRequired[AwsApiGatewayCanarySettingsTypeDef],  # (3)
    TracingEnabled: NotRequired[bool],
    CreatedDate: NotRequired[str],
    LastUpdatedDate: NotRequired[str],
    WebAclArn: NotRequired[str],
```

1. See [:material-code-braces: AwsApiGatewayMethodSettingsTypeDef](./type_defs.md#awsapigatewaymethodsettingstypedef) 
2. See [:material-code-braces: AwsApiGatewayAccessLogSettingsTypeDef](./type_defs.md#awsapigatewayaccesslogsettingstypedef) 
3. See [:material-code-braces: AwsApiGatewayCanarySettingsTypeDef](./type_defs.md#awsapigatewaycanarysettingstypedef) 
## AwsApiGatewayV2ApiDetailsTypeDef

```python
# AwsApiGatewayV2ApiDetailsTypeDef definition

class AwsApiGatewayV2ApiDetailsTypeDef(TypedDict):
    ApiEndpoint: NotRequired[str],
    ApiId: NotRequired[str],
    ApiKeySelectionExpression: NotRequired[str],
    CreatedDate: NotRequired[str],
    Description: NotRequired[str],
    Version: NotRequired[str],
    Name: NotRequired[str],
    ProtocolType: NotRequired[str],
    RouteSelectionExpression: NotRequired[str],
    CorsConfiguration: NotRequired[AwsCorsConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AwsCorsConfigurationTypeDef](./type_defs.md#awscorsconfigurationtypedef) 
## AwsApiGatewayV2StageDetailsTypeDef

```python
# AwsApiGatewayV2StageDetailsTypeDef definition

class AwsApiGatewayV2StageDetailsTypeDef(TypedDict):
    ClientCertificateId: NotRequired[str],
    CreatedDate: NotRequired[str],
    Description: NotRequired[str],
    DefaultRouteSettings: NotRequired[AwsApiGatewayV2RouteSettingsTypeDef],  # (1)
    DeploymentId: NotRequired[str],
    LastUpdatedDate: NotRequired[str],
    RouteSettings: NotRequired[AwsApiGatewayV2RouteSettingsTypeDef],  # (1)
    StageName: NotRequired[str],
    StageVariables: NotRequired[Mapping[str, str]],
    AccessLogSettings: NotRequired[AwsApiGatewayAccessLogSettingsTypeDef],  # (3)
    AutoDeploy: NotRequired[bool],
    LastDeploymentStatusMessage: NotRequired[str],
    ApiGatewayManaged: NotRequired[bool],
```

1. See [:material-code-braces: AwsApiGatewayV2RouteSettingsTypeDef](./type_defs.md#awsapigatewayv2routesettingstypedef) 
2. See [:material-code-braces: AwsApiGatewayV2RouteSettingsTypeDef](./type_defs.md#awsapigatewayv2routesettingstypedef) 
3. See [:material-code-braces: AwsApiGatewayAccessLogSettingsTypeDef](./type_defs.md#awsapigatewayaccesslogsettingstypedef) 
## AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef

```python
# AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef definition

class AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef(TypedDict):
    AuthenticationType: NotRequired[str],
    LambdaAuthorizerConfig: NotRequired[AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef],  # (1)
    OpenIdConnectConfig: NotRequired[AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef],  # (2)
    UserPoolConfig: NotRequired[AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef](./type_defs.md#awsappsyncgraphqlapilambdaauthorizerconfigdetailstypedef) 
2. See [:material-code-braces: AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef](./type_defs.md#awsappsyncgraphqlapiopenidconnectconfigdetailstypedef) 
3. See [:material-code-braces: AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef](./type_defs.md#awsappsyncgraphqlapiuserpoolconfigdetailstypedef) 
## AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef

```python
# AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef definition

class AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef(TypedDict):
    EncryptionConfiguration: NotRequired[AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef](./type_defs.md#awsathenaworkgroupconfigurationresultconfigurationencryptionconfigurationdetailstypedef) 
## AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef

```python
# AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef definition

class AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef(TypedDict):
    LaunchTemplateSpecification: NotRequired[AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef],  # (1)
    Overrides: NotRequired[Sequence[AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef]],  # (2)
```

1. See [:material-code-braces: AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef](./type_defs.md#awsautoscalingautoscalinggroupmixedinstancespolicylaunchtemplatelaunchtemplatespecificationtypedef) 
2. See [:material-code-braces: AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef](./type_defs.md#awsautoscalingautoscalinggroupmixedinstancespolicylaunchtemplateoverrideslistdetailstypedef) 
## AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef

```python
# AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef definition

class AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef(TypedDict):
    DeviceName: NotRequired[str],
    Ebs: NotRequired[AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef],  # (1)
    NoDevice: NotRequired[bool],
    VirtualName: NotRequired[str],
```

1. See [:material-code-braces: AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef](./type_defs.md#awsautoscalinglaunchconfigurationblockdevicemappingsebsdetailstypedef) 
## AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef

```python
# AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef definition

class AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef(TypedDict):
    DestinationBackupVaultArn: NotRequired[str],
    Lifecycle: NotRequired[AwsBackupBackupPlanLifecycleDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsBackupBackupPlanLifecycleDetailsTypeDef](./type_defs.md#awsbackupbackupplanlifecycledetailstypedef) 
## AwsBackupBackupVaultDetailsTypeDef

```python
# AwsBackupBackupVaultDetailsTypeDef definition

class AwsBackupBackupVaultDetailsTypeDef(TypedDict):
    BackupVaultArn: NotRequired[str],
    BackupVaultName: NotRequired[str],
    EncryptionKeyArn: NotRequired[str],
    Notifications: NotRequired[AwsBackupBackupVaultNotificationsDetailsTypeDef],  # (1)
    AccessPolicy: NotRequired[str],
```

1. See [:material-code-braces: AwsBackupBackupVaultNotificationsDetailsTypeDef](./type_defs.md#awsbackupbackupvaultnotificationsdetailstypedef) 
## AwsBackupRecoveryPointDetailsTypeDef

```python
# AwsBackupRecoveryPointDetailsTypeDef definition

class AwsBackupRecoveryPointDetailsTypeDef(TypedDict):
    BackupSizeInBytes: NotRequired[int],
    BackupVaultArn: NotRequired[str],
    BackupVaultName: NotRequired[str],
    CalculatedLifecycle: NotRequired[AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef],  # (1)
    CompletionDate: NotRequired[str],
    CreatedBy: NotRequired[AwsBackupRecoveryPointCreatedByDetailsTypeDef],  # (2)
    CreationDate: NotRequired[str],
    EncryptionKeyArn: NotRequired[str],
    IamRoleArn: NotRequired[str],
    IsEncrypted: NotRequired[bool],
    LastRestoreTime: NotRequired[str],
    Lifecycle: NotRequired[AwsBackupRecoveryPointLifecycleDetailsTypeDef],  # (3)
    RecoveryPointArn: NotRequired[str],
    ResourceArn: NotRequired[str],
    ResourceType: NotRequired[str],
    SourceBackupVaultArn: NotRequired[str],
    Status: NotRequired[str],
    StatusMessage: NotRequired[str],
    StorageClass: NotRequired[str],
```

1. See [:material-code-braces: AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef](./type_defs.md#awsbackuprecoverypointcalculatedlifecycledetailstypedef) 
2. See [:material-code-braces: AwsBackupRecoveryPointCreatedByDetailsTypeDef](./type_defs.md#awsbackuprecoverypointcreatedbydetailstypedef) 
3. See [:material-code-braces: AwsBackupRecoveryPointLifecycleDetailsTypeDef](./type_defs.md#awsbackuprecoverypointlifecycledetailstypedef) 
## AwsCertificateManagerCertificateDomainValidationOptionTypeDef

```python
# AwsCertificateManagerCertificateDomainValidationOptionTypeDef definition

class AwsCertificateManagerCertificateDomainValidationOptionTypeDef(TypedDict):
    DomainName: NotRequired[str],
    ResourceRecord: NotRequired[AwsCertificateManagerCertificateResourceRecordTypeDef],  # (1)
    ValidationDomain: NotRequired[str],
    ValidationEmails: NotRequired[Sequence[str]],
    ValidationMethod: NotRequired[str],
    ValidationStatus: NotRequired[str],
```

1. See [:material-code-braces: AwsCertificateManagerCertificateResourceRecordTypeDef](./type_defs.md#awscertificatemanagercertificateresourcerecordtypedef) 
## AwsCloudFormationStackDetailsTypeDef

```python
# AwsCloudFormationStackDetailsTypeDef definition

class AwsCloudFormationStackDetailsTypeDef(TypedDict):
    Capabilities: NotRequired[Sequence[str]],
    CreationTime: NotRequired[str],
    Description: NotRequired[str],
    DisableRollback: NotRequired[bool],
    DriftInformation: NotRequired[AwsCloudFormationStackDriftInformationDetailsTypeDef],  # (1)
    EnableTerminationProtection: NotRequired[bool],
    LastUpdatedTime: NotRequired[str],
    NotificationArns: NotRequired[Sequence[str]],
    Outputs: NotRequired[Sequence[AwsCloudFormationStackOutputsDetailsTypeDef]],  # (2)
    RoleArn: NotRequired[str],
    StackId: NotRequired[str],
    StackName: NotRequired[str],
    StackStatus: NotRequired[str],
    StackStatusReason: NotRequired[str],
    TimeoutInMinutes: NotRequired[int],
```

1. See [:material-code-braces: AwsCloudFormationStackDriftInformationDetailsTypeDef](./type_defs.md#awscloudformationstackdriftinformationdetailstypedef) 
2. See [:material-code-braces: AwsCloudFormationStackOutputsDetailsTypeDef](./type_defs.md#awscloudformationstackoutputsdetailstypedef) 
## AwsCloudFrontDistributionCacheBehaviorsTypeDef

```python
# AwsCloudFrontDistributionCacheBehaviorsTypeDef definition

class AwsCloudFrontDistributionCacheBehaviorsTypeDef(TypedDict):
    Items: NotRequired[Sequence[AwsCloudFrontDistributionCacheBehaviorTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsCloudFrontDistributionCacheBehaviorTypeDef](./type_defs.md#awscloudfrontdistributioncachebehaviortypedef) 
## AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef

```python
# AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef definition

class AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef(TypedDict):
    HttpPort: NotRequired[int],
    HttpsPort: NotRequired[int],
    OriginKeepaliveTimeout: NotRequired[int],
    OriginProtocolPolicy: NotRequired[str],
    OriginReadTimeout: NotRequired[int],
    OriginSslProtocols: NotRequired[AwsCloudFrontDistributionOriginSslProtocolsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsCloudFrontDistributionOriginSslProtocolsTypeDef](./type_defs.md#awscloudfrontdistributionoriginsslprotocolstypedef) 
## AwsCloudFrontDistributionOriginGroupFailoverTypeDef

```python
# AwsCloudFrontDistributionOriginGroupFailoverTypeDef definition

class AwsCloudFrontDistributionOriginGroupFailoverTypeDef(TypedDict):
    StatusCodes: NotRequired[AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef],  # (1)
```

1. See [:material-code-braces: AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef](./type_defs.md#awscloudfrontdistributionorigingroupfailoverstatuscodestypedef) 
## AwsCloudWatchAlarmDetailsTypeDef

```python
# AwsCloudWatchAlarmDetailsTypeDef definition

class AwsCloudWatchAlarmDetailsTypeDef(TypedDict):
    ActionsEnabled: NotRequired[bool],
    AlarmActions: NotRequired[Sequence[str]],
    AlarmArn: NotRequired[str],
    AlarmConfigurationUpdatedTimestamp: NotRequired[str],
    AlarmDescription: NotRequired[str],
    AlarmName: NotRequired[str],
    ComparisonOperator: NotRequired[str],
    DatapointsToAlarm: NotRequired[int],
    Dimensions: NotRequired[Sequence[AwsCloudWatchAlarmDimensionsDetailsTypeDef]],  # (1)
    EvaluateLowSampleCountPercentile: NotRequired[str],
    EvaluationPeriods: NotRequired[int],
    ExtendedStatistic: NotRequired[str],
    InsufficientDataActions: NotRequired[Sequence[str]],
    MetricName: NotRequired[str],
    Namespace: NotRequired[str],
    OkActions: NotRequired[Sequence[str]],
    Period: NotRequired[int],
    Statistic: NotRequired[str],
    Threshold: NotRequired[float],
    ThresholdMetricId: NotRequired[str],
    TreatMissingData: NotRequired[str],
    Unit: NotRequired[str],
```

1. See [:material-code-braces: AwsCloudWatchAlarmDimensionsDetailsTypeDef](./type_defs.md#awscloudwatchalarmdimensionsdetailstypedef) 
## AwsCodeBuildProjectEnvironmentTypeDef

```python
# AwsCodeBuildProjectEnvironmentTypeDef definition

class AwsCodeBuildProjectEnvironmentTypeDef(TypedDict):
    Certificate: NotRequired[str],
    EnvironmentVariables: NotRequired[Sequence[AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef]],  # (1)
    PrivilegedMode: NotRequired[bool],
    ImagePullCredentialsType: NotRequired[str],
    RegistryCredential: NotRequired[AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef],  # (2)
    Type: NotRequired[str],
```

1. See [:material-code-braces: AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef](./type_defs.md#awscodebuildprojectenvironmentenvironmentvariablesdetailstypedef) 
2. See [:material-code-braces: AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef](./type_defs.md#awscodebuildprojectenvironmentregistrycredentialtypedef) 
## AwsCodeBuildProjectLogsConfigDetailsTypeDef

```python
# AwsCodeBuildProjectLogsConfigDetailsTypeDef definition

class AwsCodeBuildProjectLogsConfigDetailsTypeDef(TypedDict):
    CloudWatchLogs: NotRequired[AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef],  # (1)
    S3Logs: NotRequired[AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef](./type_defs.md#awscodebuildprojectlogsconfigcloudwatchlogsdetailstypedef) 
2. See [:material-code-braces: AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef](./type_defs.md#awscodebuildprojectlogsconfigs3logsdetailstypedef) 
## AwsDynamoDbTableGlobalSecondaryIndexTypeDef

```python
# AwsDynamoDbTableGlobalSecondaryIndexTypeDef definition

class AwsDynamoDbTableGlobalSecondaryIndexTypeDef(TypedDict):
    Backfilling: NotRequired[bool],
    IndexArn: NotRequired[str],
    IndexName: NotRequired[str],
    IndexSizeBytes: NotRequired[int],
    IndexStatus: NotRequired[str],
    ItemCount: NotRequired[int],
    KeySchema: NotRequired[Sequence[AwsDynamoDbTableKeySchemaTypeDef]],  # (1)
    Projection: NotRequired[AwsDynamoDbTableProjectionTypeDef],  # (2)
    ProvisionedThroughput: NotRequired[AwsDynamoDbTableProvisionedThroughputTypeDef],  # (3)
```

1. See [:material-code-braces: AwsDynamoDbTableKeySchemaTypeDef](./type_defs.md#awsdynamodbtablekeyschematypedef) 
2. See [:material-code-braces: AwsDynamoDbTableProjectionTypeDef](./type_defs.md#awsdynamodbtableprojectiontypedef) 
3. See [:material-code-braces: AwsDynamoDbTableProvisionedThroughputTypeDef](./type_defs.md#awsdynamodbtableprovisionedthroughputtypedef) 
## AwsDynamoDbTableLocalSecondaryIndexTypeDef

```python
# AwsDynamoDbTableLocalSecondaryIndexTypeDef definition

class AwsDynamoDbTableLocalSecondaryIndexTypeDef(TypedDict):
    IndexArn: NotRequired[str],
    IndexName: NotRequired[str],
    KeySchema: NotRequired[Sequence[AwsDynamoDbTableKeySchemaTypeDef]],  # (1)
    Projection: NotRequired[AwsDynamoDbTableProjectionTypeDef],  # (2)
```

1. See [:material-code-braces: AwsDynamoDbTableKeySchemaTypeDef](./type_defs.md#awsdynamodbtablekeyschematypedef) 
2. See [:material-code-braces: AwsDynamoDbTableProjectionTypeDef](./type_defs.md#awsdynamodbtableprojectiontypedef) 
## AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef

```python
# AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef definition

class AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef(TypedDict):
    IndexName: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[AwsDynamoDbTableProvisionedThroughputOverrideTypeDef],  # (1)
```

1. See [:material-code-braces: AwsDynamoDbTableProvisionedThroughputOverrideTypeDef](./type_defs.md#awsdynamodbtableprovisionedthroughputoverridetypedef) 
## AwsEc2InstanceDetailsTypeDef

```python
# AwsEc2InstanceDetailsTypeDef definition

class AwsEc2InstanceDetailsTypeDef(TypedDict):
    Type: NotRequired[str],
    ImageId: NotRequired[str],
    IpV4Addresses: NotRequired[Sequence[str]],
    IpV6Addresses: NotRequired[Sequence[str]],
    KeyName: NotRequired[str],
    IamInstanceProfileArn: NotRequired[str],
    VpcId: NotRequired[str],
    SubnetId: NotRequired[str],
    LaunchedAt: NotRequired[str],
    NetworkInterfaces: NotRequired[Sequence[AwsEc2InstanceNetworkInterfacesDetailsTypeDef]],  # (1)
    VirtualizationType: NotRequired[str],
    MetadataOptions: NotRequired[AwsEc2InstanceMetadataOptionsTypeDef],  # (2)
    Monitoring: NotRequired[AwsEc2InstanceMonitoringDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: AwsEc2InstanceNetworkInterfacesDetailsTypeDef](./type_defs.md#awsec2instancenetworkinterfacesdetailstypedef) 
2. See [:material-code-braces: AwsEc2InstanceMetadataOptionsTypeDef](./type_defs.md#awsec2instancemetadataoptionstypedef) 
3. See [:material-code-braces: AwsEc2InstanceMonitoringDetailsTypeDef](./type_defs.md#awsec2instancemonitoringdetailstypedef) 
## AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef definition

class AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef(TypedDict):
    DeviceName: NotRequired[str],
    Ebs: NotRequired[AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef],  # (1)
    NoDevice: NotRequired[str],
    VirtualName: NotRequired[str],
```

1. See [:material-code-braces: AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatablockdevicemappingsetebsdetailstypedef) 
## AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef definition

class AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef(TypedDict):
    CapacityReservationPreference: NotRequired[str],
    CapacityReservationTarget: NotRequired[AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatacapacityreservationspecificationcapacityreservationtargetdetailstypedef) 
## AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef definition

class AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef(TypedDict):
    MarketType: NotRequired[str],
    SpotOptions: NotRequired[AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatainstancemarketoptionsspotoptionsdetailstypedef) 
## AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef definition

class AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef(TypedDict):
    AcceleratorCount: NotRequired[AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef],  # (1)
    AcceleratorManufacturers: NotRequired[Sequence[str]],
    AcceleratorNames: NotRequired[Sequence[str]],
    AcceleratorTotalMemoryMiB: NotRequired[AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef],  # (2)
    AcceleratorTypes: NotRequired[Sequence[str]],
    BareMetal: NotRequired[str],
    BaselineEbsBandwidthMbps: NotRequired[AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef],  # (3)
    BurstablePerformance: NotRequired[str],
    CpuManufacturers: NotRequired[Sequence[str]],
    ExcludedInstanceTypes: NotRequired[Sequence[str]],
    InstanceGenerations: NotRequired[Sequence[str]],
    LocalStorage: NotRequired[str],
    LocalStorageTypes: NotRequired[Sequence[str]],
    MemoryGiBPerVCpu: NotRequired[AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef],  # (4)
    MemoryMiB: NotRequired[AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef],  # (5)
    NetworkInterfaceCount: NotRequired[AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef],  # (6)
    OnDemandMaxPricePercentageOverLowestPrice: NotRequired[int],
    RequireHibernateSupport: NotRequired[bool],
    SpotMaxPricePercentageOverLowestPrice: NotRequired[int],
    TotalLocalStorageGB: NotRequired[AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef],  # (7)
    VCpuCount: NotRequired[AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef],  # (8)
```

1. See [:material-code-braces: AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatainstancerequirementsacceleratorcountdetailstypedef) 
2. See [:material-code-braces: AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatainstancerequirementsacceleratortotalmemorymibdetailstypedef) 
3. See [:material-code-braces: AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatainstancerequirementsbaselineebsbandwidthmbpsdetailstypedef) 
4. See [:material-code-braces: AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatainstancerequirementsmemorygibpervcpudetailstypedef) 
5. See [:material-code-braces: AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatainstancerequirementsmemorymibdetailstypedef) 
6. See [:material-code-braces: AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatainstancerequirementsnetworkinterfacecountdetailstypedef) 
7. See [:material-code-braces: AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatainstancerequirementstotallocalstoragegbdetailstypedef) 
8. See [:material-code-braces: AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatainstancerequirementsvcpucountdetailstypedef) 
## AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef definition

class AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef(TypedDict):
    AssociateCarrierIpAddress: NotRequired[bool],
    AssociatePublicIpAddress: NotRequired[bool],
    DeleteOnTermination: NotRequired[bool],
    Description: NotRequired[str],
    DeviceIndex: NotRequired[int],
    Groups: NotRequired[Sequence[str]],
    InterfaceType: NotRequired[str],
    Ipv4PrefixCount: NotRequired[int],
    Ipv4Prefixes: NotRequired[Sequence[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef]],  # (1)
    Ipv6AddressCount: NotRequired[int],
    Ipv6Addresses: NotRequired[Sequence[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef]],  # (2)
    Ipv6PrefixCount: NotRequired[int],
    Ipv6Prefixes: NotRequired[Sequence[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef]],  # (3)
    NetworkCardIndex: NotRequired[int],
    NetworkInterfaceId: NotRequired[str],
    PrivateIpAddress: NotRequired[str],
    PrivateIpAddresses: NotRequired[Sequence[AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef]],  # (4)
    SecondaryPrivateIpAddressCount: NotRequired[int],
    SubnetId: NotRequired[str],
```

1. See [:material-code-braces: AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatanetworkinterfacesetipv4prefixesdetailstypedef) 
2. See [:material-code-braces: AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatanetworkinterfacesetipv6addressesdetailstypedef) 
3. See [:material-code-braces: AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatanetworkinterfacesetipv6prefixesdetailstypedef) 
4. See [:material-code-braces: AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatanetworkinterfacesetprivateipaddressesdetailstypedef) 
## AwsEc2NetworkAclEntryTypeDef

```python
# AwsEc2NetworkAclEntryTypeDef definition

class AwsEc2NetworkAclEntryTypeDef(TypedDict):
    CidrBlock: NotRequired[str],
    Egress: NotRequired[bool],
    IcmpTypeCode: NotRequired[IcmpTypeCodeTypeDef],  # (1)
    Ipv6CidrBlock: NotRequired[str],
    PortRange: NotRequired[PortRangeFromToTypeDef],  # (2)
    Protocol: NotRequired[str],
    RuleAction: NotRequired[str],
    RuleNumber: NotRequired[int],
```

1. See [:material-code-braces: IcmpTypeCodeTypeDef](./type_defs.md#icmptypecodetypedef) 
2. See [:material-code-braces: PortRangeFromToTypeDef](./type_defs.md#portrangefromtotypedef) 
## AwsEc2NetworkInterfaceDetailsTypeDef

```python
# AwsEc2NetworkInterfaceDetailsTypeDef definition

class AwsEc2NetworkInterfaceDetailsTypeDef(TypedDict):
    Attachment: NotRequired[AwsEc2NetworkInterfaceAttachmentTypeDef],  # (1)
    NetworkInterfaceId: NotRequired[str],
    SecurityGroups: NotRequired[Sequence[AwsEc2NetworkInterfaceSecurityGroupTypeDef]],  # (2)
    SourceDestCheck: NotRequired[bool],
    IpV6Addresses: NotRequired[Sequence[AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef]],  # (3)
    PrivateIpAddresses: NotRequired[Sequence[AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef]],  # (4)
    PublicDnsName: NotRequired[str],
    PublicIp: NotRequired[str],
```

1. See [:material-code-braces: AwsEc2NetworkInterfaceAttachmentTypeDef](./type_defs.md#awsec2networkinterfaceattachmenttypedef) 
2. See [:material-code-braces: AwsEc2NetworkInterfaceSecurityGroupTypeDef](./type_defs.md#awsec2networkinterfacesecuritygrouptypedef) 
3. See [:material-code-braces: AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef](./type_defs.md#awsec2networkinterfaceipv6addressdetailtypedef) 
4. See [:material-code-braces: AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef](./type_defs.md#awsec2networkinterfaceprivateipaddressdetailtypedef) 
## AwsEc2SecurityGroupIpPermissionTypeDef

```python
# AwsEc2SecurityGroupIpPermissionTypeDef definition

class AwsEc2SecurityGroupIpPermissionTypeDef(TypedDict):
    IpProtocol: NotRequired[str],
    FromPort: NotRequired[int],
    ToPort: NotRequired[int],
    UserIdGroupPairs: NotRequired[Sequence[AwsEc2SecurityGroupUserIdGroupPairTypeDef]],  # (1)
    IpRanges: NotRequired[Sequence[AwsEc2SecurityGroupIpRangeTypeDef]],  # (2)
    Ipv6Ranges: NotRequired[Sequence[AwsEc2SecurityGroupIpv6RangeTypeDef]],  # (3)
    PrefixListIds: NotRequired[Sequence[AwsEc2SecurityGroupPrefixListIdTypeDef]],  # (4)
```

1. See [:material-code-braces: AwsEc2SecurityGroupUserIdGroupPairTypeDef](./type_defs.md#awsec2securitygroupuseridgrouppairtypedef) 
2. See [:material-code-braces: AwsEc2SecurityGroupIpRangeTypeDef](./type_defs.md#awsec2securitygroupiprangetypedef) 
3. See [:material-code-braces: AwsEc2SecurityGroupIpv6RangeTypeDef](./type_defs.md#awsec2securitygroupipv6rangetypedef) 
4. See [:material-code-braces: AwsEc2SecurityGroupPrefixListIdTypeDef](./type_defs.md#awsec2securitygroupprefixlistidtypedef) 
## AwsEc2SubnetDetailsTypeDef

```python
# AwsEc2SubnetDetailsTypeDef definition

class AwsEc2SubnetDetailsTypeDef(TypedDict):
    AssignIpv6AddressOnCreation: NotRequired[bool],
    AvailabilityZone: NotRequired[str],
    AvailabilityZoneId: NotRequired[str],
    AvailableIpAddressCount: NotRequired[int],
    CidrBlock: NotRequired[str],
    DefaultForAz: NotRequired[bool],
    MapPublicIpOnLaunch: NotRequired[bool],
    OwnerId: NotRequired[str],
    State: NotRequired[str],
    SubnetArn: NotRequired[str],
    SubnetId: NotRequired[str],
    VpcId: NotRequired[str],
    Ipv6CidrBlockAssociationSet: NotRequired[Sequence[Ipv6CidrBlockAssociationTypeDef]],  # (1)
```

1. See [:material-code-braces: Ipv6CidrBlockAssociationTypeDef](./type_defs.md#ipv6cidrblockassociationtypedef) 
## AwsEc2VolumeDetailsTypeDef

```python
# AwsEc2VolumeDetailsTypeDef definition

class AwsEc2VolumeDetailsTypeDef(TypedDict):
    CreateTime: NotRequired[str],
    DeviceName: NotRequired[str],
    Encrypted: NotRequired[bool],
    Size: NotRequired[int],
    SnapshotId: NotRequired[str],
    Status: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Attachments: NotRequired[Sequence[AwsEc2VolumeAttachmentTypeDef]],  # (1)
    VolumeId: NotRequired[str],
    VolumeType: NotRequired[str],
    VolumeScanStatus: NotRequired[str],
```

1. See [:material-code-braces: AwsEc2VolumeAttachmentTypeDef](./type_defs.md#awsec2volumeattachmenttypedef) 
## AwsEc2VpcDetailsTypeDef

```python
# AwsEc2VpcDetailsTypeDef definition

class AwsEc2VpcDetailsTypeDef(TypedDict):
    CidrBlockAssociationSet: NotRequired[Sequence[CidrBlockAssociationTypeDef]],  # (1)
    Ipv6CidrBlockAssociationSet: NotRequired[Sequence[Ipv6CidrBlockAssociationTypeDef]],  # (2)
    DhcpOptionsId: NotRequired[str],
    State: NotRequired[str],
```

1. See [:material-code-braces: CidrBlockAssociationTypeDef](./type_defs.md#cidrblockassociationtypedef) 
2. See [:material-code-braces: Ipv6CidrBlockAssociationTypeDef](./type_defs.md#ipv6cidrblockassociationtypedef) 
## AwsEc2VpcEndpointServiceDetailsTypeDef

```python
# AwsEc2VpcEndpointServiceDetailsTypeDef definition

class AwsEc2VpcEndpointServiceDetailsTypeDef(TypedDict):
    AcceptanceRequired: NotRequired[bool],
    AvailabilityZones: NotRequired[Sequence[str]],
    BaseEndpointDnsNames: NotRequired[Sequence[str]],
    ManagesVpcEndpoints: NotRequired[bool],
    GatewayLoadBalancerArns: NotRequired[Sequence[str]],
    NetworkLoadBalancerArns: NotRequired[Sequence[str]],
    PrivateDnsName: NotRequired[str],
    ServiceId: NotRequired[str],
    ServiceName: NotRequired[str],
    ServiceState: NotRequired[str],
    ServiceType: NotRequired[Sequence[AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef](./type_defs.md#awsec2vpcendpointserviceservicetypedetailstypedef) 
## AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef

```python
# AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef definition

class AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef(TypedDict):
    CidrBlock: NotRequired[str],
    CidrBlockSet: NotRequired[Sequence[VpcInfoCidrBlockSetDetailsTypeDef]],  # (1)
    Ipv6CidrBlockSet: NotRequired[Sequence[VpcInfoIpv6CidrBlockSetDetailsTypeDef]],  # (2)
    OwnerId: NotRequired[str],
    PeeringOptions: NotRequired[VpcInfoPeeringOptionsDetailsTypeDef],  # (3)
    Region: NotRequired[str],
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: VpcInfoCidrBlockSetDetailsTypeDef](./type_defs.md#vpcinfocidrblocksetdetailstypedef) 
2. See [:material-code-braces: VpcInfoIpv6CidrBlockSetDetailsTypeDef](./type_defs.md#vpcinfoipv6cidrblocksetdetailstypedef) 
3. See [:material-code-braces: VpcInfoPeeringOptionsDetailsTypeDef](./type_defs.md#vpcinfopeeringoptionsdetailstypedef) 
## AwsEc2VpnConnectionOptionsDetailsTypeDef

```python
# AwsEc2VpnConnectionOptionsDetailsTypeDef definition

class AwsEc2VpnConnectionOptionsDetailsTypeDef(TypedDict):
    StaticRoutesOnly: NotRequired[bool],
    TunnelOptions: NotRequired[Sequence[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef](./type_defs.md#awsec2vpnconnectionoptionstunneloptionsdetailstypedef) 
## AwsEcrRepositoryDetailsTypeDef

```python
# AwsEcrRepositoryDetailsTypeDef definition

class AwsEcrRepositoryDetailsTypeDef(TypedDict):
    Arn: NotRequired[str],
    ImageScanningConfiguration: NotRequired[AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef],  # (1)
    ImageTagMutability: NotRequired[str],
    LifecyclePolicy: NotRequired[AwsEcrRepositoryLifecyclePolicyDetailsTypeDef],  # (2)
    RepositoryName: NotRequired[str],
    RepositoryPolicyText: NotRequired[str],
```

1. See [:material-code-braces: AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef](./type_defs.md#awsecrrepositoryimagescanningconfigurationdetailstypedef) 
2. See [:material-code-braces: AwsEcrRepositoryLifecyclePolicyDetailsTypeDef](./type_defs.md#awsecrrepositorylifecyclepolicydetailstypedef) 
## AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef

```python
# AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef definition

class AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef(TypedDict):
    KmsKeyId: NotRequired[str],
    LogConfiguration: NotRequired[AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef],  # (1)
    Logging: NotRequired[str],
```

1. See [:material-code-braces: AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef](./type_defs.md#awsecsclusterconfigurationexecutecommandconfigurationlogconfigurationdetailstypedef) 
## AwsEcsContainerDetailsTypeDef

```python
# AwsEcsContainerDetailsTypeDef definition

class AwsEcsContainerDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Image: NotRequired[str],
    MountPoints: NotRequired[Sequence[AwsMountPointTypeDef]],  # (1)
    Privileged: NotRequired[bool],
```

1. See [:material-code-braces: AwsMountPointTypeDef](./type_defs.md#awsmountpointtypedef) 
## AwsEcsServiceDeploymentConfigurationDetailsTypeDef

```python
# AwsEcsServiceDeploymentConfigurationDetailsTypeDef definition

class AwsEcsServiceDeploymentConfigurationDetailsTypeDef(TypedDict):
    DeploymentCircuitBreaker: NotRequired[AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef],  # (1)
    MaximumPercent: NotRequired[int],
    MinimumHealthyPercent: NotRequired[int],
```

1. See [:material-code-braces: AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef](./type_defs.md#awsecsservicedeploymentconfigurationdeploymentcircuitbreakerdetailstypedef) 
## AwsEcsServiceNetworkConfigurationDetailsTypeDef

```python
# AwsEcsServiceNetworkConfigurationDetailsTypeDef definition

class AwsEcsServiceNetworkConfigurationDetailsTypeDef(TypedDict):
    AwsVpcConfiguration: NotRequired[AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef](./type_defs.md#awsecsservicenetworkconfigurationawsvpcconfigurationdetailstypedef) 
## AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef(TypedDict):
    Capabilities: NotRequired[AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef],  # (1)
    Devices: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef]],  # (2)
    InitProcessEnabled: NotRequired[bool],
    MaxSwap: NotRequired[int],
    SharedMemorySize: NotRequired[int],
    Swappiness: NotRequired[int],
    Tmpfs: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef]],  # (3)
```

1. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionslinuxparameterscapabilitiesdetailstypedef) 
2. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionslinuxparametersdevicesdetailstypedef) 
3. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionslinuxparameterstmpfsdetailstypedef) 
## AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef(TypedDict):
    LogDriver: NotRequired[str],
    Options: NotRequired[Mapping[str, str]],
    SecretOptions: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionslogconfigurationsecretoptionsdetailstypedef) 
## AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef

```python
# AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef definition

class AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef(TypedDict):
    ContainerName: NotRequired[str],
    ProxyConfigurationProperties: NotRequired[Sequence[AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef]],  # (1)
    Type: NotRequired[str],
```

1. See [:material-code-braces: AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef](./type_defs.md#awsecstaskdefinitionproxyconfigurationproxyconfigurationpropertiesdetailstypedef) 
## AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef

```python
# AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef definition

class AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef(TypedDict):
    AuthorizationConfig: NotRequired[AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef],  # (1)
    FilesystemId: NotRequired[str],
    RootDirectory: NotRequired[str],
    TransitEncryption: NotRequired[str],
    TransitEncryptionPort: NotRequired[int],
```

1. See [:material-code-braces: AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef](./type_defs.md#awsecstaskdefinitionvolumesefsvolumeconfigurationauthorizationconfigdetailstypedef) 
## AwsEcsTaskVolumeDetailsTypeDef

```python
# AwsEcsTaskVolumeDetailsTypeDef definition

class AwsEcsTaskVolumeDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Host: NotRequired[AwsEcsTaskVolumeHostDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsEcsTaskVolumeHostDetailsTypeDef](./type_defs.md#awsecstaskvolumehostdetailstypedef) 
## AwsEfsAccessPointRootDirectoryDetailsTypeDef

```python
# AwsEfsAccessPointRootDirectoryDetailsTypeDef definition

class AwsEfsAccessPointRootDirectoryDetailsTypeDef(TypedDict):
    CreationInfo: NotRequired[AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef],  # (1)
    Path: NotRequired[str],
```

1. See [:material-code-braces: AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef](./type_defs.md#awsefsaccesspointrootdirectorycreationinfodetailstypedef) 
## AwsEksClusterLoggingDetailsTypeDef

```python
# AwsEksClusterLoggingDetailsTypeDef definition

class AwsEksClusterLoggingDetailsTypeDef(TypedDict):
    ClusterLogging: NotRequired[Sequence[AwsEksClusterLoggingClusterLoggingDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsEksClusterLoggingClusterLoggingDetailsTypeDef](./type_defs.md#awseksclusterloggingclusterloggingdetailstypedef) 
## AwsElasticBeanstalkEnvironmentDetailsTypeDef

```python
# AwsElasticBeanstalkEnvironmentDetailsTypeDef definition

class AwsElasticBeanstalkEnvironmentDetailsTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    Cname: NotRequired[str],
    DateCreated: NotRequired[str],
    DateUpdated: NotRequired[str],
    Description: NotRequired[str],
    EndpointUrl: NotRequired[str],
    EnvironmentArn: NotRequired[str],
    EnvironmentId: NotRequired[str],
    EnvironmentLinks: NotRequired[Sequence[AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef]],  # (1)
    EnvironmentName: NotRequired[str],
    OptionSettings: NotRequired[Sequence[AwsElasticBeanstalkEnvironmentOptionSettingTypeDef]],  # (2)
    PlatformArn: NotRequired[str],
    SolutionStackName: NotRequired[str],
    Status: NotRequired[str],
    Tier: NotRequired[AwsElasticBeanstalkEnvironmentTierTypeDef],  # (3)
    VersionLabel: NotRequired[str],
```

1. See [:material-code-braces: AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef](./type_defs.md#awselasticbeanstalkenvironmentenvironmentlinktypedef) 
2. See [:material-code-braces: AwsElasticBeanstalkEnvironmentOptionSettingTypeDef](./type_defs.md#awselasticbeanstalkenvironmentoptionsettingtypedef) 
3. See [:material-code-braces: AwsElasticBeanstalkEnvironmentTierTypeDef](./type_defs.md#awselasticbeanstalkenvironmenttiertypedef) 
## AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef

```python
# AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef definition

class AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef(TypedDict):
    DedicatedMasterCount: NotRequired[int],
    DedicatedMasterEnabled: NotRequired[bool],
    DedicatedMasterType: NotRequired[str],
    InstanceCount: NotRequired[int],
    InstanceType: NotRequired[str],
    ZoneAwarenessConfig: NotRequired[AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef],  # (1)
    ZoneAwarenessEnabled: NotRequired[bool],
```

1. See [:material-code-braces: AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef](./type_defs.md#awselasticsearchdomainelasticsearchclusterconfigzoneawarenessconfigdetailstypedef) 
## AwsElasticsearchDomainLogPublishingOptionsTypeDef

```python
# AwsElasticsearchDomainLogPublishingOptionsTypeDef definition

class AwsElasticsearchDomainLogPublishingOptionsTypeDef(TypedDict):
    IndexSlowLogs: NotRequired[AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef],  # (1)
    SearchSlowLogs: NotRequired[AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef],  # (1)
    AuditLogs: NotRequired[AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef],  # (1)
```

1. See [:material-code-braces: AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef](./type_defs.md#awselasticsearchdomainlogpublishingoptionslogconfigtypedef) 
2. See [:material-code-braces: AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef](./type_defs.md#awselasticsearchdomainlogpublishingoptionslogconfigtypedef) 
3. See [:material-code-braces: AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef](./type_defs.md#awselasticsearchdomainlogpublishingoptionslogconfigtypedef) 
## AwsElbLoadBalancerPoliciesTypeDef

```python
# AwsElbLoadBalancerPoliciesTypeDef definition

class AwsElbLoadBalancerPoliciesTypeDef(TypedDict):
    AppCookieStickinessPolicies: NotRequired[Sequence[AwsElbAppCookieStickinessPolicyTypeDef]],  # (1)
    LbCookieStickinessPolicies: NotRequired[Sequence[AwsElbLbCookieStickinessPolicyTypeDef]],  # (2)
    OtherPolicies: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: AwsElbAppCookieStickinessPolicyTypeDef](./type_defs.md#awselbappcookiestickinesspolicytypedef) 
2. See [:material-code-braces: AwsElbLbCookieStickinessPolicyTypeDef](./type_defs.md#awselblbcookiestickinesspolicytypedef) 
## AwsElbLoadBalancerAttributesTypeDef

```python
# AwsElbLoadBalancerAttributesTypeDef definition

class AwsElbLoadBalancerAttributesTypeDef(TypedDict):
    AccessLog: NotRequired[AwsElbLoadBalancerAccessLogTypeDef],  # (1)
    ConnectionDraining: NotRequired[AwsElbLoadBalancerConnectionDrainingTypeDef],  # (2)
    ConnectionSettings: NotRequired[AwsElbLoadBalancerConnectionSettingsTypeDef],  # (3)
    CrossZoneLoadBalancing: NotRequired[AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef],  # (4)
    AdditionalAttributes: NotRequired[Sequence[AwsElbLoadBalancerAdditionalAttributeTypeDef]],  # (5)
```

1. See [:material-code-braces: AwsElbLoadBalancerAccessLogTypeDef](./type_defs.md#awselbloadbalanceraccesslogtypedef) 
2. See [:material-code-braces: AwsElbLoadBalancerConnectionDrainingTypeDef](./type_defs.md#awselbloadbalancerconnectiondrainingtypedef) 
3. See [:material-code-braces: AwsElbLoadBalancerConnectionSettingsTypeDef](./type_defs.md#awselbloadbalancerconnectionsettingstypedef) 
4. See [:material-code-braces: AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef](./type_defs.md#awselbloadbalancercrosszoneloadbalancingtypedef) 
5. See [:material-code-braces: AwsElbLoadBalancerAdditionalAttributeTypeDef](./type_defs.md#awselbloadbalanceradditionalattributetypedef) 
## AwsElbLoadBalancerListenerDescriptionTypeDef

```python
# AwsElbLoadBalancerListenerDescriptionTypeDef definition

class AwsElbLoadBalancerListenerDescriptionTypeDef(TypedDict):
    Listener: NotRequired[AwsElbLoadBalancerListenerTypeDef],  # (1)
    PolicyNames: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: AwsElbLoadBalancerListenerTypeDef](./type_defs.md#awselbloadbalancerlistenertypedef) 
## AwsElbv2LoadBalancerDetailsTypeDef

```python
# AwsElbv2LoadBalancerDetailsTypeDef definition

class AwsElbv2LoadBalancerDetailsTypeDef(TypedDict):
    AvailabilityZones: NotRequired[Sequence[AvailabilityZoneTypeDef]],  # (1)
    CanonicalHostedZoneId: NotRequired[str],
    CreatedTime: NotRequired[str],
    DNSName: NotRequired[str],
    IpAddressType: NotRequired[str],
    Scheme: NotRequired[str],
    SecurityGroups: NotRequired[Sequence[str]],
    State: NotRequired[LoadBalancerStateTypeDef],  # (2)
    Type: NotRequired[str],
    VpcId: NotRequired[str],
    LoadBalancerAttributes: NotRequired[Sequence[AwsElbv2LoadBalancerAttributeTypeDef]],  # (3)
```

1. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
2. See [:material-code-braces: LoadBalancerStateTypeDef](./type_defs.md#loadbalancerstatetypedef) 
3. See [:material-code-braces: AwsElbv2LoadBalancerAttributeTypeDef](./type_defs.md#awselbv2loadbalancerattributetypedef) 
## AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef

```python
# AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef definition

class AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef(TypedDict):
    AuditLogs: NotRequired[AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef](./type_defs.md#awsguarddutydetectordatasourceskubernetesauditlogsdetailstypedef) 
## AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef

```python
# AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef definition

class AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef(TypedDict):
    EbsVolumes: NotRequired[AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef](./type_defs.md#awsguarddutydetectordatasourcesmalwareprotectionscanec2instancewithfindingsebsvolumesdetailstypedef) 
## AwsIamAccessKeySessionContextTypeDef

```python
# AwsIamAccessKeySessionContextTypeDef definition

class AwsIamAccessKeySessionContextTypeDef(TypedDict):
    Attributes: NotRequired[AwsIamAccessKeySessionContextAttributesTypeDef],  # (1)
    SessionIssuer: NotRequired[AwsIamAccessKeySessionContextSessionIssuerTypeDef],  # (2)
```

1. See [:material-code-braces: AwsIamAccessKeySessionContextAttributesTypeDef](./type_defs.md#awsiamaccesskeysessioncontextattributestypedef) 
2. See [:material-code-braces: AwsIamAccessKeySessionContextSessionIssuerTypeDef](./type_defs.md#awsiamaccesskeysessioncontextsessionissuertypedef) 
## AwsIamGroupDetailsTypeDef

```python
# AwsIamGroupDetailsTypeDef definition

class AwsIamGroupDetailsTypeDef(TypedDict):
    AttachedManagedPolicies: NotRequired[Sequence[AwsIamAttachedManagedPolicyTypeDef]],  # (1)
    CreateDate: NotRequired[str],
    GroupId: NotRequired[str],
    GroupName: NotRequired[str],
    GroupPolicyList: NotRequired[Sequence[AwsIamGroupPolicyTypeDef]],  # (2)
    Path: NotRequired[str],
```

1. See [:material-code-braces: AwsIamAttachedManagedPolicyTypeDef](./type_defs.md#awsiamattachedmanagedpolicytypedef) 
2. See [:material-code-braces: AwsIamGroupPolicyTypeDef](./type_defs.md#awsiamgrouppolicytypedef) 
## AwsIamInstanceProfileTypeDef

```python
# AwsIamInstanceProfileTypeDef definition

class AwsIamInstanceProfileTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreateDate: NotRequired[str],
    InstanceProfileId: NotRequired[str],
    InstanceProfileName: NotRequired[str],
    Path: NotRequired[str],
    Roles: NotRequired[Sequence[AwsIamInstanceProfileRoleTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsIamInstanceProfileRoleTypeDef](./type_defs.md#awsiaminstanceprofileroletypedef) 
## AwsIamPolicyDetailsTypeDef

```python
# AwsIamPolicyDetailsTypeDef definition

class AwsIamPolicyDetailsTypeDef(TypedDict):
    AttachmentCount: NotRequired[int],
    CreateDate: NotRequired[str],
    DefaultVersionId: NotRequired[str],
    Description: NotRequired[str],
    IsAttachable: NotRequired[bool],
    Path: NotRequired[str],
    PermissionsBoundaryUsageCount: NotRequired[int],
    PolicyId: NotRequired[str],
    PolicyName: NotRequired[str],
    PolicyVersionList: NotRequired[Sequence[AwsIamPolicyVersionTypeDef]],  # (1)
    UpdateDate: NotRequired[str],
```

1. See [:material-code-braces: AwsIamPolicyVersionTypeDef](./type_defs.md#awsiampolicyversiontypedef) 
## AwsIamUserDetailsTypeDef

```python
# AwsIamUserDetailsTypeDef definition

class AwsIamUserDetailsTypeDef(TypedDict):
    AttachedManagedPolicies: NotRequired[Sequence[AwsIamAttachedManagedPolicyTypeDef]],  # (1)
    CreateDate: NotRequired[str],
    GroupList: NotRequired[Sequence[str]],
    Path: NotRequired[str],
    PermissionsBoundary: NotRequired[AwsIamPermissionsBoundaryTypeDef],  # (2)
    UserId: NotRequired[str],
    UserName: NotRequired[str],
    UserPolicyList: NotRequired[Sequence[AwsIamUserPolicyTypeDef]],  # (3)
```

1. See [:material-code-braces: AwsIamAttachedManagedPolicyTypeDef](./type_defs.md#awsiamattachedmanagedpolicytypedef) 
2. See [:material-code-braces: AwsIamPermissionsBoundaryTypeDef](./type_defs.md#awsiampermissionsboundarytypedef) 
3. See [:material-code-braces: AwsIamUserPolicyTypeDef](./type_defs.md#awsiamuserpolicytypedef) 
## AwsKinesisStreamDetailsTypeDef

```python
# AwsKinesisStreamDetailsTypeDef definition

class AwsKinesisStreamDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    StreamEncryption: NotRequired[AwsKinesisStreamStreamEncryptionDetailsTypeDef],  # (1)
    ShardCount: NotRequired[int],
    RetentionPeriodHours: NotRequired[int],
```

1. See [:material-code-braces: AwsKinesisStreamStreamEncryptionDetailsTypeDef](./type_defs.md#awskinesisstreamstreamencryptiondetailstypedef) 
## AwsLambdaFunctionEnvironmentTypeDef

```python
# AwsLambdaFunctionEnvironmentTypeDef definition

class AwsLambdaFunctionEnvironmentTypeDef(TypedDict):
    Variables: NotRequired[Mapping[str, str]],
    Error: NotRequired[AwsLambdaFunctionEnvironmentErrorTypeDef],  # (1)
```

1. See [:material-code-braces: AwsLambdaFunctionEnvironmentErrorTypeDef](./type_defs.md#awslambdafunctionenvironmenterrortypedef) 
## AwsNetworkFirewallFirewallDetailsTypeDef

```python
# AwsNetworkFirewallFirewallDetailsTypeDef definition

class AwsNetworkFirewallFirewallDetailsTypeDef(TypedDict):
    DeleteProtection: NotRequired[bool],
    Description: NotRequired[str],
    FirewallArn: NotRequired[str],
    FirewallId: NotRequired[str],
    FirewallName: NotRequired[str],
    FirewallPolicyArn: NotRequired[str],
    FirewallPolicyChangeProtection: NotRequired[bool],
    SubnetChangeProtection: NotRequired[bool],
    SubnetMappings: NotRequired[Sequence[AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef]],  # (1)
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef](./type_defs.md#awsnetworkfirewallfirewallsubnetmappingsdetailstypedef) 
## AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef

```python
# AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef definition

class AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    InternalUserDatabaseEnabled: NotRequired[bool],
    MasterUserOptions: NotRequired[AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef](./type_defs.md#awsopensearchservicedomainmasteruseroptionsdetailstypedef) 
## AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef

```python
# AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef definition

class AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef(TypedDict):
    InstanceCount: NotRequired[int],
    WarmEnabled: NotRequired[bool],
    WarmCount: NotRequired[int],
    DedicatedMasterEnabled: NotRequired[bool],
    ZoneAwarenessConfig: NotRequired[AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef],  # (1)
    DedicatedMasterCount: NotRequired[int],
    InstanceType: NotRequired[str],
    WarmType: NotRequired[str],
    ZoneAwarenessEnabled: NotRequired[bool],
    DedicatedMasterType: NotRequired[str],
```

1. See [:material-code-braces: AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef](./type_defs.md#awsopensearchservicedomainclusterconfigzoneawarenessconfigdetailstypedef) 
## AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef

```python
# AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef definition

class AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef(TypedDict):
    IndexSlowLogs: NotRequired[AwsOpenSearchServiceDomainLogPublishingOptionTypeDef],  # (1)
    SearchSlowLogs: NotRequired[AwsOpenSearchServiceDomainLogPublishingOptionTypeDef],  # (1)
    AuditLogs: NotRequired[AwsOpenSearchServiceDomainLogPublishingOptionTypeDef],  # (1)
```

1. See [:material-code-braces: AwsOpenSearchServiceDomainLogPublishingOptionTypeDef](./type_defs.md#awsopensearchservicedomainlogpublishingoptiontypedef) 
2. See [:material-code-braces: AwsOpenSearchServiceDomainLogPublishingOptionTypeDef](./type_defs.md#awsopensearchservicedomainlogpublishingoptiontypedef) 
3. See [:material-code-braces: AwsOpenSearchServiceDomainLogPublishingOptionTypeDef](./type_defs.md#awsopensearchservicedomainlogpublishingoptiontypedef) 
## AwsRdsDbClusterDetailsTypeDef

```python
# AwsRdsDbClusterDetailsTypeDef definition

class AwsRdsDbClusterDetailsTypeDef(TypedDict):
    AllocatedStorage: NotRequired[int],
    AvailabilityZones: NotRequired[Sequence[str]],
    BackupRetentionPeriod: NotRequired[int],
    DatabaseName: NotRequired[str],
    Status: NotRequired[str],
    Endpoint: NotRequired[str],
    ReaderEndpoint: NotRequired[str],
    CustomEndpoints: NotRequired[Sequence[str]],
    MultiAz: NotRequired[bool],
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    Port: NotRequired[int],
    MasterUsername: NotRequired[str],
    PreferredBackupWindow: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    ReadReplicaIdentifiers: NotRequired[Sequence[str]],
    VpcSecurityGroups: NotRequired[Sequence[AwsRdsDbInstanceVpcSecurityGroupTypeDef]],  # (1)
    HostedZoneId: NotRequired[str],
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    DbClusterResourceId: NotRequired[str],
    AssociatedRoles: NotRequired[Sequence[AwsRdsDbClusterAssociatedRoleTypeDef]],  # (2)
    ClusterCreateTime: NotRequired[str],
    EnabledCloudWatchLogsExports: NotRequired[Sequence[str]],
    EngineMode: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    HttpEndpointEnabled: NotRequired[bool],
    ActivityStreamStatus: NotRequired[str],
    CopyTagsToSnapshot: NotRequired[bool],
    CrossAccountClone: NotRequired[bool],
    DomainMemberships: NotRequired[Sequence[AwsRdsDbDomainMembershipTypeDef]],  # (3)
    DbClusterParameterGroup: NotRequired[str],
    DbSubnetGroup: NotRequired[str],
    DbClusterOptionGroupMemberships: NotRequired[Sequence[AwsRdsDbClusterOptionGroupMembershipTypeDef]],  # (4)
    DbClusterIdentifier: NotRequired[str],
    DbClusterMembers: NotRequired[Sequence[AwsRdsDbClusterMemberTypeDef]],  # (5)
    IamDatabaseAuthenticationEnabled: NotRequired[bool],
```

1. See [:material-code-braces: AwsRdsDbInstanceVpcSecurityGroupTypeDef](./type_defs.md#awsrdsdbinstancevpcsecuritygrouptypedef) 
2. See [:material-code-braces: AwsRdsDbClusterAssociatedRoleTypeDef](./type_defs.md#awsrdsdbclusterassociatedroletypedef) 
3. See [:material-code-braces: AwsRdsDbDomainMembershipTypeDef](./type_defs.md#awsrdsdbdomainmembershiptypedef) 
4. See [:material-code-braces: AwsRdsDbClusterOptionGroupMembershipTypeDef](./type_defs.md#awsrdsdbclusteroptiongroupmembershiptypedef) 
5. See [:material-code-braces: AwsRdsDbClusterMemberTypeDef](./type_defs.md#awsrdsdbclustermembertypedef) 
## AwsRdsDbClusterSnapshotDetailsTypeDef

```python
# AwsRdsDbClusterSnapshotDetailsTypeDef definition

class AwsRdsDbClusterSnapshotDetailsTypeDef(TypedDict):
    AvailabilityZones: NotRequired[Sequence[str]],
    SnapshotCreateTime: NotRequired[str],
    Engine: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    Status: NotRequired[str],
    Port: NotRequired[int],
    VpcId: NotRequired[str],
    ClusterCreateTime: NotRequired[str],
    MasterUsername: NotRequired[str],
    EngineVersion: NotRequired[str],
    LicenseModel: NotRequired[str],
    SnapshotType: NotRequired[str],
    PercentProgress: NotRequired[int],
    StorageEncrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    DbClusterIdentifier: NotRequired[str],
    DbClusterSnapshotIdentifier: NotRequired[str],
    IamDatabaseAuthenticationEnabled: NotRequired[bool],
    DbClusterSnapshotAttributes: NotRequired[Sequence[AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef](./type_defs.md#awsrdsdbclustersnapshotdbclustersnapshotattributetypedef) 
## AwsRdsDbSnapshotDetailsTypeDef

```python
# AwsRdsDbSnapshotDetailsTypeDef definition

class AwsRdsDbSnapshotDetailsTypeDef(TypedDict):
    DbSnapshotIdentifier: NotRequired[str],
    DbInstanceIdentifier: NotRequired[str],
    SnapshotCreateTime: NotRequired[str],
    Engine: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    Status: NotRequired[str],
    Port: NotRequired[int],
    AvailabilityZone: NotRequired[str],
    VpcId: NotRequired[str],
    InstanceCreateTime: NotRequired[str],
    MasterUsername: NotRequired[str],
    EngineVersion: NotRequired[str],
    LicenseModel: NotRequired[str],
    SnapshotType: NotRequired[str],
    Iops: NotRequired[int],
    OptionGroupName: NotRequired[str],
    PercentProgress: NotRequired[int],
    SourceRegion: NotRequired[str],
    SourceDbSnapshotIdentifier: NotRequired[str],
    StorageType: NotRequired[str],
    TdeCredentialArn: NotRequired[str],
    Encrypted: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    Timezone: NotRequired[str],
    IamDatabaseAuthenticationEnabled: NotRequired[bool],
    ProcessorFeatures: NotRequired[Sequence[AwsRdsDbProcessorFeatureTypeDef]],  # (1)
    DbiResourceId: NotRequired[str],
```

1. See [:material-code-braces: AwsRdsDbProcessorFeatureTypeDef](./type_defs.md#awsrdsdbprocessorfeaturetypedef) 
## AwsRdsDbPendingModifiedValuesTypeDef

```python
# AwsRdsDbPendingModifiedValuesTypeDef definition

class AwsRdsDbPendingModifiedValuesTypeDef(TypedDict):
    DbInstanceClass: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    MasterUserPassword: NotRequired[str],
    Port: NotRequired[int],
    BackupRetentionPeriod: NotRequired[int],
    MultiAZ: NotRequired[bool],
    EngineVersion: NotRequired[str],
    LicenseModel: NotRequired[str],
    Iops: NotRequired[int],
    DbInstanceIdentifier: NotRequired[str],
    StorageType: NotRequired[str],
    CaCertificateIdentifier: NotRequired[str],
    DbSubnetGroupName: NotRequired[str],
    PendingCloudWatchLogsExports: NotRequired[AwsRdsPendingCloudWatchLogsExportsTypeDef],  # (1)
    ProcessorFeatures: NotRequired[Sequence[AwsRdsDbProcessorFeatureTypeDef]],  # (2)
```

1. See [:material-code-braces: AwsRdsPendingCloudWatchLogsExportsTypeDef](./type_defs.md#awsrdspendingcloudwatchlogsexportstypedef) 
2. See [:material-code-braces: AwsRdsDbProcessorFeatureTypeDef](./type_defs.md#awsrdsdbprocessorfeaturetypedef) 
## AwsRdsDbSecurityGroupDetailsTypeDef

```python
# AwsRdsDbSecurityGroupDetailsTypeDef definition

class AwsRdsDbSecurityGroupDetailsTypeDef(TypedDict):
    DbSecurityGroupArn: NotRequired[str],
    DbSecurityGroupDescription: NotRequired[str],
    DbSecurityGroupName: NotRequired[str],
    Ec2SecurityGroups: NotRequired[Sequence[AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef]],  # (1)
    IpRanges: NotRequired[Sequence[AwsRdsDbSecurityGroupIpRangeTypeDef]],  # (2)
    OwnerId: NotRequired[str],
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef](./type_defs.md#awsrdsdbsecuritygroupec2securitygrouptypedef) 
2. See [:material-code-braces: AwsRdsDbSecurityGroupIpRangeTypeDef](./type_defs.md#awsrdsdbsecuritygroupiprangetypedef) 
## AwsRdsDbSubnetGroupSubnetTypeDef

```python
# AwsRdsDbSubnetGroupSubnetTypeDef definition

class AwsRdsDbSubnetGroupSubnetTypeDef(TypedDict):
    SubnetIdentifier: NotRequired[str],
    SubnetAvailabilityZone: NotRequired[AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef],  # (1)
    SubnetStatus: NotRequired[str],
```

1. See [:material-code-braces: AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef](./type_defs.md#awsrdsdbsubnetgroupsubnetavailabilityzonetypedef) 
## AwsRedshiftClusterClusterParameterGroupTypeDef

```python
# AwsRedshiftClusterClusterParameterGroupTypeDef definition

class AwsRedshiftClusterClusterParameterGroupTypeDef(TypedDict):
    ClusterParameterStatusList: NotRequired[Sequence[AwsRedshiftClusterClusterParameterStatusTypeDef]],  # (1)
    ParameterApplyStatus: NotRequired[str],
    ParameterGroupName: NotRequired[str],
```

1. See [:material-code-braces: AwsRedshiftClusterClusterParameterStatusTypeDef](./type_defs.md#awsredshiftclusterclusterparameterstatustypedef) 
## AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef

```python
# AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef definition

class AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Tag: NotRequired[AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef],  # (1)
    Type: NotRequired[str],
```

1. See [:material-code-braces: AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef](./type_defs.md#awss3bucketbucketlifecycleconfigurationrulesfilterpredicateoperandstagdetailstypedef) 
## AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef

```python
# AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef definition

class AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef(TypedDict):
    FilterRules: NotRequired[Sequence[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef](./type_defs.md#awss3bucketnotificationconfigurations3keyfilterruletypedef) 
## AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef

```python
# AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef definition

class AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef(TypedDict):
    DefaultRetention: NotRequired[AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef](./type_defs.md#awss3bucketobjectlockconfigurationruledefaultretentiondetailstypedef) 
## AwsS3BucketServerSideEncryptionRuleTypeDef

```python
# AwsS3BucketServerSideEncryptionRuleTypeDef definition

class AwsS3BucketServerSideEncryptionRuleTypeDef(TypedDict):
    ApplyServerSideEncryptionByDefault: NotRequired[AwsS3BucketServerSideEncryptionByDefaultTypeDef],  # (1)
```

1. See [:material-code-braces: AwsS3BucketServerSideEncryptionByDefaultTypeDef](./type_defs.md#awss3bucketserversideencryptionbydefaulttypedef) 
## AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef

```python
# AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef definition

class AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef(TypedDict):
    Condition: NotRequired[AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef],  # (1)
    Redirect: NotRequired[AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef],  # (2)
```

1. See [:material-code-braces: AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef](./type_defs.md#awss3bucketwebsiteconfigurationroutingruleconditiontypedef) 
2. See [:material-code-braces: AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef](./type_defs.md#awss3bucketwebsiteconfigurationroutingruleredirecttypedef) 
## AwsSageMakerNotebookInstanceDetailsTypeDef

```python
# AwsSageMakerNotebookInstanceDetailsTypeDef definition

class AwsSageMakerNotebookInstanceDetailsTypeDef(TypedDict):
    AcceleratorTypes: NotRequired[Sequence[str]],
    AdditionalCodeRepositories: NotRequired[Sequence[str]],
    DefaultCodeRepository: NotRequired[str],
    DirectInternetAccess: NotRequired[str],
    FailureReason: NotRequired[str],
    InstanceMetadataServiceConfiguration: NotRequired[AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef],  # (1)
    InstanceType: NotRequired[str],
    KmsKeyId: NotRequired[str],
    NetworkInterfaceId: NotRequired[str],
    NotebookInstanceArn: NotRequired[str],
    NotebookInstanceLifecycleConfigName: NotRequired[str],
    NotebookInstanceName: NotRequired[str],
    NotebookInstanceStatus: NotRequired[str],
    PlatformIdentifier: NotRequired[str],
    RoleArn: NotRequired[str],
    RootAccess: NotRequired[str],
    SecurityGroups: NotRequired[Sequence[str]],
    SubnetId: NotRequired[str],
    Url: NotRequired[str],
    VolumeSizeInGB: NotRequired[int],
```

1. See [:material-code-braces: AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef](./type_defs.md#awssagemakernotebookinstancemetadataserviceconfigurationdetailstypedef) 
## AwsSecretsManagerSecretDetailsTypeDef

```python
# AwsSecretsManagerSecretDetailsTypeDef definition

class AwsSecretsManagerSecretDetailsTypeDef(TypedDict):
    RotationRules: NotRequired[AwsSecretsManagerSecretRotationRulesTypeDef],  # (1)
    RotationOccurredWithinFrequency: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    RotationEnabled: NotRequired[bool],
    RotationLambdaArn: NotRequired[str],
    Deleted: NotRequired[bool],
    Name: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-braces: AwsSecretsManagerSecretRotationRulesTypeDef](./type_defs.md#awssecretsmanagersecretrotationrulestypedef) 
## BatchUpdateFindingsRequestRequestTypeDef

```python
# BatchUpdateFindingsRequestRequestTypeDef definition

class BatchUpdateFindingsRequestRequestTypeDef(TypedDict):
    FindingIdentifiers: Sequence[AwsSecurityFindingIdentifierTypeDef],  # (1)
    Note: NotRequired[NoteUpdateTypeDef],  # (2)
    Severity: NotRequired[SeverityUpdateTypeDef],  # (3)
    VerificationState: NotRequired[VerificationStateType],  # (4)
    Confidence: NotRequired[int],
    Criticality: NotRequired[int],
    Types: NotRequired[Sequence[str]],
    UserDefinedFields: NotRequired[Mapping[str, str]],
    Workflow: NotRequired[WorkflowUpdateTypeDef],  # (5)
    RelatedFindings: NotRequired[Sequence[RelatedFindingTypeDef]],  # (6)
```

1. See [:material-code-braces: AwsSecurityFindingIdentifierTypeDef](./type_defs.md#awssecurityfindingidentifiertypedef) 
2. See [:material-code-braces: NoteUpdateTypeDef](./type_defs.md#noteupdatetypedef) 
3. See [:material-code-braces: SeverityUpdateTypeDef](./type_defs.md#severityupdatetypedef) 
4. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
5. See [:material-code-braces: WorkflowUpdateTypeDef](./type_defs.md#workflowupdatetypedef) 
6. See [:material-code-braces: RelatedFindingTypeDef](./type_defs.md#relatedfindingtypedef) 
## BatchUpdateFindingsUnprocessedFindingTypeDef

```python
# BatchUpdateFindingsUnprocessedFindingTypeDef definition

class BatchUpdateFindingsUnprocessedFindingTypeDef(TypedDict):
    FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,  # (1)
    ErrorCode: str,
    ErrorMessage: str,
```

1. See [:material-code-braces: AwsSecurityFindingIdentifierTypeDef](./type_defs.md#awssecurityfindingidentifiertypedef) 
## AwsSnsTopicDetailsTypeDef

```python
# AwsSnsTopicDetailsTypeDef definition

class AwsSnsTopicDetailsTypeDef(TypedDict):
    KmsMasterKeyId: NotRequired[str],
    Subscription: NotRequired[Sequence[AwsSnsTopicSubscriptionTypeDef]],  # (1)
    TopicName: NotRequired[str],
    Owner: NotRequired[str],
    SqsSuccessFeedbackRoleArn: NotRequired[str],
    SqsFailureFeedbackRoleArn: NotRequired[str],
    ApplicationSuccessFeedbackRoleArn: NotRequired[str],
    FirehoseSuccessFeedbackRoleArn: NotRequired[str],
    FirehoseFailureFeedbackRoleArn: NotRequired[str],
    HttpSuccessFeedbackRoleArn: NotRequired[str],
    HttpFailureFeedbackRoleArn: NotRequired[str],
```

1. See [:material-code-braces: AwsSnsTopicSubscriptionTypeDef](./type_defs.md#awssnstopicsubscriptiontypedef) 
## AwsSsmPatchTypeDef

```python
# AwsSsmPatchTypeDef definition

class AwsSsmPatchTypeDef(TypedDict):
    ComplianceSummary: NotRequired[AwsSsmComplianceSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: AwsSsmComplianceSummaryTypeDef](./type_defs.md#awsssmcompliancesummarytypedef) 
## AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef

```python
# AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef definition

class AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef(TypedDict):
    CloudWatchLogsLogGroup: NotRequired[AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef](./type_defs.md#awsstepfunctionstatemachineloggingconfigurationdestinationscloudwatchlogsloggroupdetailstypedef) 
## AwsWafRateBasedRuleDetailsTypeDef

```python
# AwsWafRateBasedRuleDetailsTypeDef definition

class AwsWafRateBasedRuleDetailsTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Name: NotRequired[str],
    RateKey: NotRequired[str],
    RateLimit: NotRequired[int],
    RuleId: NotRequired[str],
    MatchPredicates: NotRequired[Sequence[AwsWafRateBasedRuleMatchPredicateTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsWafRateBasedRuleMatchPredicateTypeDef](./type_defs.md#awswafratebasedrulematchpredicatetypedef) 
## AwsWafRegionalRateBasedRuleDetailsTypeDef

```python
# AwsWafRegionalRateBasedRuleDetailsTypeDef definition

class AwsWafRegionalRateBasedRuleDetailsTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Name: NotRequired[str],
    RateKey: NotRequired[str],
    RateLimit: NotRequired[int],
    RuleId: NotRequired[str],
    MatchPredicates: NotRequired[Sequence[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsWafRegionalRateBasedRuleMatchPredicateTypeDef](./type_defs.md#awswafregionalratebasedrulematchpredicatetypedef) 
## AwsWafRegionalRuleDetailsTypeDef

```python
# AwsWafRegionalRuleDetailsTypeDef definition

class AwsWafRegionalRuleDetailsTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Name: NotRequired[str],
    PredicateList: NotRequired[Sequence[AwsWafRegionalRulePredicateListDetailsTypeDef]],  # (1)
    RuleId: NotRequired[str],
```

1. See [:material-code-braces: AwsWafRegionalRulePredicateListDetailsTypeDef](./type_defs.md#awswafregionalrulepredicatelistdetailstypedef) 
## AwsWafRegionalRuleGroupRulesDetailsTypeDef

```python
# AwsWafRegionalRuleGroupRulesDetailsTypeDef definition

class AwsWafRegionalRuleGroupRulesDetailsTypeDef(TypedDict):
    Action: NotRequired[AwsWafRegionalRuleGroupRulesActionDetailsTypeDef],  # (1)
    Priority: NotRequired[int],
    RuleId: NotRequired[str],
    Type: NotRequired[str],
```

1. See [:material-code-braces: AwsWafRegionalRuleGroupRulesActionDetailsTypeDef](./type_defs.md#awswafregionalrulegrouprulesactiondetailstypedef) 
## AwsWafRegionalWebAclRulesListDetailsTypeDef

```python
# AwsWafRegionalWebAclRulesListDetailsTypeDef definition

class AwsWafRegionalWebAclRulesListDetailsTypeDef(TypedDict):
    Action: NotRequired[AwsWafRegionalWebAclRulesListActionDetailsTypeDef],  # (1)
    OverrideAction: NotRequired[AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef],  # (2)
    Priority: NotRequired[int],
    RuleId: NotRequired[str],
    Type: NotRequired[str],
```

1. See [:material-code-braces: AwsWafRegionalWebAclRulesListActionDetailsTypeDef](./type_defs.md#awswafregionalwebaclruleslistactiondetailstypedef) 
2. See [:material-code-braces: AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef](./type_defs.md#awswafregionalwebaclruleslistoverrideactiondetailstypedef) 
## AwsWafRuleDetailsTypeDef

```python
# AwsWafRuleDetailsTypeDef definition

class AwsWafRuleDetailsTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Name: NotRequired[str],
    PredicateList: NotRequired[Sequence[AwsWafRulePredicateListDetailsTypeDef]],  # (1)
    RuleId: NotRequired[str],
```

1. See [:material-code-braces: AwsWafRulePredicateListDetailsTypeDef](./type_defs.md#awswafrulepredicatelistdetailstypedef) 
## AwsWafRuleGroupRulesDetailsTypeDef

```python
# AwsWafRuleGroupRulesDetailsTypeDef definition

class AwsWafRuleGroupRulesDetailsTypeDef(TypedDict):
    Action: NotRequired[AwsWafRuleGroupRulesActionDetailsTypeDef],  # (1)
    Priority: NotRequired[int],
    RuleId: NotRequired[str],
    Type: NotRequired[str],
```

1. See [:material-code-braces: AwsWafRuleGroupRulesActionDetailsTypeDef](./type_defs.md#awswafrulegrouprulesactiondetailstypedef) 
## AwsWafWebAclRuleTypeDef

```python
# AwsWafWebAclRuleTypeDef definition

class AwsWafWebAclRuleTypeDef(TypedDict):
    Action: NotRequired[WafActionTypeDef],  # (1)
    ExcludedRules: NotRequired[Sequence[WafExcludedRuleTypeDef]],  # (2)
    OverrideAction: NotRequired[WafOverrideActionTypeDef],  # (3)
    Priority: NotRequired[int],
    RuleId: NotRequired[str],
    Type: NotRequired[str],
```

1. See [:material-code-braces: WafActionTypeDef](./type_defs.md#wafactiontypedef) 
2. See [:material-code-braces: WafExcludedRuleTypeDef](./type_defs.md#wafexcludedruletypedef) 
3. See [:material-code-braces: WafOverrideActionTypeDef](./type_defs.md#wafoverrideactiontypedef) 
## AwsWafv2CustomRequestHandlingDetailsTypeDef

```python
# AwsWafv2CustomRequestHandlingDetailsTypeDef definition

class AwsWafv2CustomRequestHandlingDetailsTypeDef(TypedDict):
    InsertHeaders: NotRequired[Sequence[AwsWafv2CustomHttpHeaderTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsWafv2CustomHttpHeaderTypeDef](./type_defs.md#awswafv2customhttpheadertypedef) 
## AwsWafv2CustomResponseDetailsTypeDef

```python
# AwsWafv2CustomResponseDetailsTypeDef definition

class AwsWafv2CustomResponseDetailsTypeDef(TypedDict):
    CustomResponseBodyKey: NotRequired[str],
    ResponseCode: NotRequired[int],
    ResponseHeaders: NotRequired[Sequence[AwsWafv2CustomHttpHeaderTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsWafv2CustomHttpHeaderTypeDef](./type_defs.md#awswafv2customhttpheadertypedef) 
## AwsWafv2WebAclCaptchaConfigDetailsTypeDef

```python
# AwsWafv2WebAclCaptchaConfigDetailsTypeDef definition

class AwsWafv2WebAclCaptchaConfigDetailsTypeDef(TypedDict):
    ImmunityTimeProperty: NotRequired[AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef](./type_defs.md#awswafv2webaclcaptchaconfigimmunitytimepropertydetailstypedef) 
## CreateActionTargetResponseTypeDef

```python
# CreateActionTargetResponseTypeDef definition

class CreateActionTargetResponseTypeDef(TypedDict):
    ActionTargetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAutomationRuleResponseTypeDef

```python
# CreateAutomationRuleResponseTypeDef definition

class CreateAutomationRuleResponseTypeDef(TypedDict):
    RuleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFindingAggregatorResponseTypeDef

```python
# CreateFindingAggregatorResponseTypeDef definition

class CreateFindingAggregatorResponseTypeDef(TypedDict):
    FindingAggregatorArn: str,
    FindingAggregationRegion: str,
    RegionLinkingMode: str,
    Regions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInsightResponseTypeDef

```python
# CreateInsightResponseTypeDef definition

class CreateInsightResponseTypeDef(TypedDict):
    InsightArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteActionTargetResponseTypeDef

```python
# DeleteActionTargetResponseTypeDef definition

class DeleteActionTargetResponseTypeDef(TypedDict):
    ActionTargetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInsightResponseTypeDef

```python
# DeleteInsightResponseTypeDef definition

class DeleteInsightResponseTypeDef(TypedDict):
    InsightArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeActionTargetsResponseTypeDef

```python
# DescribeActionTargetsResponseTypeDef definition

class DescribeActionTargetsResponseTypeDef(TypedDict):
    ActionTargets: List[ActionTargetTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeHubResponseTypeDef

```python
# DescribeHubResponseTypeDef definition

class DescribeHubResponseTypeDef(TypedDict):
    HubArn: str,
    SubscribedAt: str,
    AutoEnableControls: bool,
    ControlFindingGenerator: ControlFindingGeneratorType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ControlFindingGeneratorType](./literals.md#controlfindinggeneratortype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationConfigurationResponseTypeDef

```python
# DescribeOrganizationConfigurationResponseTypeDef definition

class DescribeOrganizationConfigurationResponseTypeDef(TypedDict):
    AutoEnable: bool,
    MemberAccountLimitReached: bool,
    AutoEnableStandards: AutoEnableStandardsType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AutoEnableStandardsType](./literals.md#autoenablestandardstype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableImportFindingsForProductResponseTypeDef

```python
# EnableImportFindingsForProductResponseTypeDef definition

class EnableImportFindingsForProductResponseTypeDef(TypedDict):
    ProductSubscriptionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFindingAggregatorResponseTypeDef

```python
# GetFindingAggregatorResponseTypeDef definition

class GetFindingAggregatorResponseTypeDef(TypedDict):
    FindingAggregatorArn: str,
    FindingAggregationRegion: str,
    RegionLinkingMode: str,
    Regions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInvitationsCountResponseTypeDef

```python
# GetInvitationsCountResponseTypeDef definition

class GetInvitationsCountResponseTypeDef(TypedDict):
    InvitationsCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAutomationRulesResponseTypeDef

```python
# ListAutomationRulesResponseTypeDef definition

class ListAutomationRulesResponseTypeDef(TypedDict):
    AutomationRulesMetadata: List[AutomationRulesMetadataTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutomationRulesMetadataTypeDef](./type_defs.md#automationrulesmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnabledProductsForImportResponseTypeDef

```python
# ListEnabledProductsForImportResponseTypeDef definition

class ListEnabledProductsForImportResponseTypeDef(TypedDict):
    ProductSubscriptions: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOrganizationAdminAccountsResponseTypeDef

```python
# ListOrganizationAdminAccountsResponseTypeDef definition

class ListOrganizationAdminAccountsResponseTypeDef(TypedDict):
    AdminAccounts: List[AdminAccountTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
## UpdateFindingAggregatorResponseTypeDef

```python
# UpdateFindingAggregatorResponseTypeDef definition

class UpdateFindingAggregatorResponseTypeDef(TypedDict):
    FindingAggregatorArn: str,
    FindingAggregationRegion: str,
    RegionLinkingMode: str,
    Regions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteAutomationRulesResponseTypeDef

```python
# BatchDeleteAutomationRulesResponseTypeDef definition

class BatchDeleteAutomationRulesResponseTypeDef(TypedDict):
    ProcessedAutomationRules: List[str],
    UnprocessedAutomationRules: List[UnprocessedAutomationRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAutomationRuleTypeDef](./type_defs.md#unprocessedautomationruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateAutomationRulesResponseTypeDef

```python
# BatchUpdateAutomationRulesResponseTypeDef definition

class BatchUpdateAutomationRulesResponseTypeDef(TypedDict):
    ProcessedAutomationRules: List[str],
    UnprocessedAutomationRules: List[UnprocessedAutomationRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedAutomationRuleTypeDef](./type_defs.md#unprocessedautomationruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchEnableStandardsRequestRequestTypeDef

```python
# BatchEnableStandardsRequestRequestTypeDef definition

class BatchEnableStandardsRequestRequestTypeDef(TypedDict):
    StandardsSubscriptionRequests: Sequence[StandardsSubscriptionRequestTypeDef],  # (1)
```

1. See [:material-code-braces: StandardsSubscriptionRequestTypeDef](./type_defs.md#standardssubscriptionrequesttypedef) 
## BatchGetSecurityControlsResponseTypeDef

```python
# BatchGetSecurityControlsResponseTypeDef definition

class BatchGetSecurityControlsResponseTypeDef(TypedDict):
    SecurityControls: List[SecurityControlTypeDef],  # (1)
    UnprocessedIds: List[UnprocessedSecurityControlTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SecurityControlTypeDef](./type_defs.md#securitycontroltypedef) 
2. See [:material-code-braces: UnprocessedSecurityControlTypeDef](./type_defs.md#unprocessedsecuritycontroltypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetStandardsControlAssociationsRequestRequestTypeDef

```python
# BatchGetStandardsControlAssociationsRequestRequestTypeDef definition

class BatchGetStandardsControlAssociationsRequestRequestTypeDef(TypedDict):
    StandardsControlAssociationIds: Sequence[StandardsControlAssociationIdTypeDef],  # (1)
```

1. See [:material-code-braces: StandardsControlAssociationIdTypeDef](./type_defs.md#standardscontrolassociationidtypedef) 
## UnprocessedStandardsControlAssociationTypeDef

```python
# UnprocessedStandardsControlAssociationTypeDef definition

class UnprocessedStandardsControlAssociationTypeDef(TypedDict):
    StandardsControlAssociationId: StandardsControlAssociationIdTypeDef,  # (1)
    ErrorCode: UnprocessedErrorCodeType,  # (2)
    ErrorReason: NotRequired[str],
```

1. See [:material-code-braces: StandardsControlAssociationIdTypeDef](./type_defs.md#standardscontrolassociationidtypedef) 
2. See [:material-code-brackets: UnprocessedErrorCodeType](./literals.md#unprocessederrorcodetype) 
## BatchImportFindingsResponseTypeDef

```python
# BatchImportFindingsResponseTypeDef definition

class BatchImportFindingsResponseTypeDef(TypedDict):
    FailedCount: int,
    SuccessCount: int,
    FailedFindings: List[ImportFindingsErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportFindingsErrorTypeDef](./type_defs.md#importfindingserrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateStandardsControlAssociationsRequestRequestTypeDef

```python
# BatchUpdateStandardsControlAssociationsRequestRequestTypeDef definition

class BatchUpdateStandardsControlAssociationsRequestRequestTypeDef(TypedDict):
    StandardsControlAssociationUpdates: Sequence[StandardsControlAssociationUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: StandardsControlAssociationUpdateTypeDef](./type_defs.md#standardscontrolassociationupdatetypedef) 
## UnprocessedStandardsControlAssociationUpdateTypeDef

```python
# UnprocessedStandardsControlAssociationUpdateTypeDef definition

class UnprocessedStandardsControlAssociationUpdateTypeDef(TypedDict):
    StandardsControlAssociationUpdate: StandardsControlAssociationUpdateTypeDef,  # (1)
    ErrorCode: UnprocessedErrorCodeType,  # (2)
    ErrorReason: NotRequired[str],
```

1. See [:material-code-braces: StandardsControlAssociationUpdateTypeDef](./type_defs.md#standardscontrolassociationupdatetypedef) 
2. See [:material-code-brackets: UnprocessedErrorCodeType](./literals.md#unprocessederrorcodetype) 
## ComplianceTypeDef

```python
# ComplianceTypeDef definition

class ComplianceTypeDef(TypedDict):
    Status: NotRequired[ComplianceStatusType],  # (1)
    RelatedRequirements: NotRequired[Sequence[str]],
    StatusReasons: NotRequired[Sequence[StatusReasonTypeDef]],  # (2)
    SecurityControlId: NotRequired[str],
    AssociatedStandards: NotRequired[Sequence[AssociatedStandardTypeDef]],  # (3)
```

1. See [:material-code-brackets: ComplianceStatusType](./literals.md#compliancestatustype) 
2. See [:material-code-braces: StatusReasonTypeDef](./type_defs.md#statusreasontypedef) 
3. See [:material-code-braces: AssociatedStandardTypeDef](./type_defs.md#associatedstandardtypedef) 
## ContainerDetailsTypeDef

```python
# ContainerDetailsTypeDef definition

class ContainerDetailsTypeDef(TypedDict):
    ContainerRuntime: NotRequired[str],
    Name: NotRequired[str],
    ImageId: NotRequired[str],
    ImageName: NotRequired[str],
    LaunchedAt: NotRequired[str],
    VolumeMounts: NotRequired[Sequence[VolumeMountTypeDef]],  # (1)
    Privileged: NotRequired[bool],
```

1. See [:material-code-braces: VolumeMountTypeDef](./type_defs.md#volumemounttypedef) 
## CreateMembersResponseTypeDef

```python
# CreateMembersResponseTypeDef definition

class CreateMembersResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[ResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResultTypeDef](./type_defs.md#resulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeclineInvitationsResponseTypeDef

```python
# DeclineInvitationsResponseTypeDef definition

class DeclineInvitationsResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[ResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResultTypeDef](./type_defs.md#resulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInvitationsResponseTypeDef

```python
# DeleteInvitationsResponseTypeDef definition

class DeleteInvitationsResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[ResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResultTypeDef](./type_defs.md#resulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMembersResponseTypeDef

```python
# DeleteMembersResponseTypeDef definition

class DeleteMembersResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[ResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResultTypeDef](./type_defs.md#resulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InviteMembersResponseTypeDef

```python
# InviteMembersResponseTypeDef definition

class InviteMembersResponseTypeDef(TypedDict):
    UnprocessedAccounts: List[ResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResultTypeDef](./type_defs.md#resulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DateFilterTypeDef

```python
# DateFilterTypeDef definition

class DateFilterTypeDef(TypedDict):
    Start: NotRequired[str],
    End: NotRequired[str],
    DateRange: NotRequired[DateRangeTypeDef],  # (1)
```

1. See [:material-code-braces: DateRangeTypeDef](./type_defs.md#daterangetypedef) 
## DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef

```python
# DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef definition

class DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef(TypedDict):
    ActionTargetArns: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeProductsRequestDescribeProductsPaginateTypeDef

```python
# DescribeProductsRequestDescribeProductsPaginateTypeDef definition

class DescribeProductsRequestDescribeProductsPaginateTypeDef(TypedDict):
    ProductArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef

```python
# DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef definition

class DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef(TypedDict):
    StandardsSubscriptionArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeStandardsRequestDescribeStandardsPaginateTypeDef

```python
# DescribeStandardsRequestDescribeStandardsPaginateTypeDef definition

class DescribeStandardsRequestDescribeStandardsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef

```python
# GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef definition

class GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef(TypedDict):
    StandardsSubscriptionArns: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetInsightsRequestGetInsightsPaginateTypeDef

```python
# GetInsightsRequestGetInsightsPaginateTypeDef definition

class GetInsightsRequestGetInsightsPaginateTypeDef(TypedDict):
    InsightArns: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef

```python
# ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef definition

class ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef

```python
# ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef definition

class ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInvitationsRequestListInvitationsPaginateTypeDef

```python
# ListInvitationsRequestListInvitationsPaginateTypeDef definition

class ListInvitationsRequestListInvitationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembersRequestListMembersPaginateTypeDef

```python
# ListMembersRequestListMembersPaginateTypeDef definition

class ListMembersRequestListMembersPaginateTypeDef(TypedDict):
    OnlyAssociated: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef

```python
# ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef definition

class ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef

```python
# ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef definition

class ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef(TypedDict):
    StandardsArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef

```python
# ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef definition

class ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef(TypedDict):
    SecurityControlId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeProductsResponseTypeDef

```python
# DescribeProductsResponseTypeDef definition

class DescribeProductsResponseTypeDef(TypedDict):
    Products: List[ProductTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProductTypeDef](./type_defs.md#producttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStandardsControlsResponseTypeDef

```python
# DescribeStandardsControlsResponseTypeDef definition

class DescribeStandardsControlsResponseTypeDef(TypedDict):
    Controls: List[StandardsControlTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StandardsControlTypeDef](./type_defs.md#standardscontroltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ThreatTypeDef

```python
# ThreatTypeDef definition

class ThreatTypeDef(TypedDict):
    Name: NotRequired[str],
    Severity: NotRequired[str],
    ItemCount: NotRequired[int],
    FilePaths: NotRequired[Sequence[FilePathsTypeDef]],  # (1)
```

1. See [:material-code-braces: FilePathsTypeDef](./type_defs.md#filepathstypedef) 
## ListFindingAggregatorsResponseTypeDef

```python
# ListFindingAggregatorsResponseTypeDef definition

class ListFindingAggregatorsResponseTypeDef(TypedDict):
    FindingAggregators: List[FindingAggregatorTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FindingAggregatorTypeDef](./type_defs.md#findingaggregatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FindingHistoryRecordTypeDef

```python
# FindingHistoryRecordTypeDef definition

class FindingHistoryRecordTypeDef(TypedDict):
    FindingIdentifier: NotRequired[AwsSecurityFindingIdentifierTypeDef],  # (1)
    UpdateTime: NotRequired[datetime],
    FindingCreated: NotRequired[bool],
    UpdateSource: NotRequired[FindingHistoryUpdateSourceTypeDef],  # (2)
    Updates: NotRequired[List[FindingHistoryUpdateTypeDef]],  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AwsSecurityFindingIdentifierTypeDef](./type_defs.md#awssecurityfindingidentifiertypedef) 
2. See [:material-code-braces: FindingHistoryUpdateSourceTypeDef](./type_defs.md#findinghistoryupdatesourcetypedef) 
3. See [:material-code-braces: FindingHistoryUpdateTypeDef](./type_defs.md#findinghistoryupdatetypedef) 
## FindingProviderFieldsTypeDef

```python
# FindingProviderFieldsTypeDef definition

class FindingProviderFieldsTypeDef(TypedDict):
    Confidence: NotRequired[int],
    Criticality: NotRequired[int],
    RelatedFindings: NotRequired[Sequence[RelatedFindingTypeDef]],  # (1)
    Severity: NotRequired[FindingProviderSeverityTypeDef],  # (2)
    Types: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: RelatedFindingTypeDef](./type_defs.md#relatedfindingtypedef) 
2. See [:material-code-braces: FindingProviderSeverityTypeDef](./type_defs.md#findingproviderseveritytypedef) 
## GetAdministratorAccountResponseTypeDef

```python
# GetAdministratorAccountResponseTypeDef definition

class GetAdministratorAccountResponseTypeDef(TypedDict):
    Administrator: InvitationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InvitationTypeDef](./type_defs.md#invitationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMasterAccountResponseTypeDef

```python
# GetMasterAccountResponseTypeDef definition

class GetMasterAccountResponseTypeDef(TypedDict):
    Master: InvitationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InvitationTypeDef](./type_defs.md#invitationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInvitationsResponseTypeDef

```python
# ListInvitationsResponseTypeDef definition

class ListInvitationsResponseTypeDef(TypedDict):
    Invitations: List[InvitationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InvitationTypeDef](./type_defs.md#invitationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef

```python
# GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef definition

class GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef(TypedDict):
    FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,  # (1)
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AwsSecurityFindingIdentifierTypeDef](./type_defs.md#awssecurityfindingidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetFindingHistoryRequestRequestTypeDef

```python
# GetFindingHistoryRequestRequestTypeDef definition

class GetFindingHistoryRequestRequestTypeDef(TypedDict):
    FindingIdentifier: AwsSecurityFindingIdentifierTypeDef,  # (1)
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: AwsSecurityFindingIdentifierTypeDef](./type_defs.md#awssecurityfindingidentifiertypedef) 
## GetMembersResponseTypeDef

```python
# GetMembersResponseTypeDef definition

class GetMembersResponseTypeDef(TypedDict):
    Members: List[MemberTypeDef],  # (1)
    UnprocessedAccounts: List[ResultTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
2. See [:material-code-braces: ResultTypeDef](./type_defs.md#resulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMembersResponseTypeDef

```python
# ListMembersResponseTypeDef definition

class ListMembersResponseTypeDef(TypedDict):
    Members: List[MemberTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InsightResultsTypeDef

```python
# InsightResultsTypeDef definition

class InsightResultsTypeDef(TypedDict):
    InsightArn: str,
    GroupByAttribute: str,
    ResultValues: List[InsightResultValueTypeDef],  # (1)
```

1. See [:material-code-braces: InsightResultValueTypeDef](./type_defs.md#insightresultvaluetypedef) 
## ListSecurityControlDefinitionsResponseTypeDef

```python
# ListSecurityControlDefinitionsResponseTypeDef definition

class ListSecurityControlDefinitionsResponseTypeDef(TypedDict):
    SecurityControlDefinitions: List[SecurityControlDefinitionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityControlDefinitionTypeDef](./type_defs.md#securitycontroldefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStandardsControlAssociationsResponseTypeDef

```python
# ListStandardsControlAssociationsResponseTypeDef definition

class ListStandardsControlAssociationsResponseTypeDef(TypedDict):
    StandardsControlAssociationSummaries: List[StandardsControlAssociationSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StandardsControlAssociationSummaryTypeDef](./type_defs.md#standardscontrolassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkPathComponentDetailsTypeDef

```python
# NetworkPathComponentDetailsTypeDef definition

class NetworkPathComponentDetailsTypeDef(TypedDict):
    Address: NotRequired[Sequence[str]],
    PortRanges: NotRequired[Sequence[PortRangeTypeDef]],  # (1)
```

1. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
## NetworkTypeDef

```python
# NetworkTypeDef definition

class NetworkTypeDef(TypedDict):
    Direction: NotRequired[NetworkDirectionType],  # (1)
    Protocol: NotRequired[str],
    OpenPortRange: NotRequired[PortRangeTypeDef],  # (2)
    SourceIpV4: NotRequired[str],
    SourceIpV6: NotRequired[str],
    SourcePort: NotRequired[int],
    SourceDomain: NotRequired[str],
    SourceMac: NotRequired[str],
    DestinationIpV4: NotRequired[str],
    DestinationIpV6: NotRequired[str],
    DestinationPort: NotRequired[int],
    DestinationDomain: NotRequired[str],
```

1. See [:material-code-brackets: NetworkDirectionType](./literals.md#networkdirectiontype) 
2. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
## PageTypeDef

```python
# PageTypeDef definition

class PageTypeDef(TypedDict):
    PageNumber: NotRequired[int],
    LineRange: NotRequired[RangeTypeDef],  # (1)
    OffsetRange: NotRequired[RangeTypeDef],  # (1)
```

1. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
2. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
## RemediationTypeDef

```python
# RemediationTypeDef definition

class RemediationTypeDef(TypedDict):
    Recommendation: NotRequired[RecommendationTypeDef],  # (1)
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
## RuleGroupSourceStatefulRulesDetailsTypeDef

```python
# RuleGroupSourceStatefulRulesDetailsTypeDef definition

class RuleGroupSourceStatefulRulesDetailsTypeDef(TypedDict):
    Action: NotRequired[str],
    Header: NotRequired[RuleGroupSourceStatefulRulesHeaderDetailsTypeDef],  # (1)
    RuleOptions: NotRequired[Sequence[RuleGroupSourceStatefulRulesOptionsDetailsTypeDef]],  # (2)
```

1. See [:material-code-braces: RuleGroupSourceStatefulRulesHeaderDetailsTypeDef](./type_defs.md#rulegroupsourcestatefulrulesheaderdetailstypedef) 
2. See [:material-code-braces: RuleGroupSourceStatefulRulesOptionsDetailsTypeDef](./type_defs.md#rulegroupsourcestatefulrulesoptionsdetailstypedef) 
## RuleGroupSourceStatelessRuleMatchAttributesTypeDef

```python
# RuleGroupSourceStatelessRuleMatchAttributesTypeDef definition

class RuleGroupSourceStatelessRuleMatchAttributesTypeDef(TypedDict):
    DestinationPorts: NotRequired[Sequence[RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef]],  # (1)
    Destinations: NotRequired[Sequence[RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef]],  # (2)
    Protocols: NotRequired[Sequence[int]],
    SourcePorts: NotRequired[Sequence[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef]],  # (3)
    Sources: NotRequired[Sequence[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef]],  # (4)
    TcpFlags: NotRequired[Sequence[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef]],  # (5)
```

1. See [:material-code-braces: RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef](./type_defs.md#rulegroupsourcestatelessrulematchattributesdestinationportstypedef) 
2. See [:material-code-braces: RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef](./type_defs.md#rulegroupsourcestatelessrulematchattributesdestinationstypedef) 
3. See [:material-code-braces: RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef](./type_defs.md#rulegroupsourcestatelessrulematchattributessourceportstypedef) 
4. See [:material-code-braces: RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef](./type_defs.md#rulegroupsourcestatelessrulematchattributessourcestypedef) 
5. See [:material-code-braces: RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef](./type_defs.md#rulegroupsourcestatelessrulematchattributestcpflagstypedef) 
## RuleGroupVariablesTypeDef

```python
# RuleGroupVariablesTypeDef definition

class RuleGroupVariablesTypeDef(TypedDict):
    IpSets: NotRequired[RuleGroupVariablesIpSetsDetailsTypeDef],  # (1)
    PortSets: NotRequired[RuleGroupVariablesPortSetsDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: RuleGroupVariablesIpSetsDetailsTypeDef](./type_defs.md#rulegroupvariablesipsetsdetailstypedef) 
2. See [:material-code-braces: RuleGroupVariablesPortSetsDetailsTypeDef](./type_defs.md#rulegroupvariablesportsetsdetailstypedef) 
## StandardTypeDef

```python
# StandardTypeDef definition

class StandardTypeDef(TypedDict):
    StandardsArn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    EnabledByDefault: NotRequired[bool],
    StandardsManagedBy: NotRequired[StandardsManagedByTypeDef],  # (1)
```

1. See [:material-code-braces: StandardsManagedByTypeDef](./type_defs.md#standardsmanagedbytypedef) 
## StandardsSubscriptionTypeDef

```python
# StandardsSubscriptionTypeDef definition

class StandardsSubscriptionTypeDef(TypedDict):
    StandardsSubscriptionArn: str,
    StandardsArn: str,
    StandardsInput: Dict[str, str],
    StandardsStatus: StandardsStatusType,  # (1)
    StandardsStatusReason: NotRequired[StandardsStatusReasonTypeDef],  # (2)
```

1. See [:material-code-brackets: StandardsStatusType](./literals.md#standardsstatustype) 
2. See [:material-code-braces: StandardsStatusReasonTypeDef](./type_defs.md#standardsstatusreasontypedef) 
## StatelessCustomPublishMetricActionTypeDef

```python
# StatelessCustomPublishMetricActionTypeDef definition

class StatelessCustomPublishMetricActionTypeDef(TypedDict):
    Dimensions: NotRequired[Sequence[StatelessCustomPublishMetricActionDimensionTypeDef]],  # (1)
```

1. See [:material-code-braces: StatelessCustomPublishMetricActionDimensionTypeDef](./type_defs.md#statelesscustompublishmetricactiondimensiontypedef) 
## AwsApiCallActionTypeDef

```python
# AwsApiCallActionTypeDef definition

class AwsApiCallActionTypeDef(TypedDict):
    Api: NotRequired[str],
    ServiceName: NotRequired[str],
    CallerType: NotRequired[str],
    RemoteIpDetails: NotRequired[ActionRemoteIpDetailsTypeDef],  # (1)
    DomainDetails: NotRequired[AwsApiCallActionDomainDetailsTypeDef],  # (2)
    AffectedResources: NotRequired[Mapping[str, str]],
    FirstSeen: NotRequired[str],
    LastSeen: NotRequired[str],
```

1. See [:material-code-braces: ActionRemoteIpDetailsTypeDef](./type_defs.md#actionremoteipdetailstypedef) 
2. See [:material-code-braces: AwsApiCallActionDomainDetailsTypeDef](./type_defs.md#awsapicallactiondomaindetailstypedef) 
## NetworkConnectionActionTypeDef

```python
# NetworkConnectionActionTypeDef definition

class NetworkConnectionActionTypeDef(TypedDict):
    ConnectionDirection: NotRequired[str],
    RemoteIpDetails: NotRequired[ActionRemoteIpDetailsTypeDef],  # (1)
    RemotePortDetails: NotRequired[ActionRemotePortDetailsTypeDef],  # (2)
    LocalPortDetails: NotRequired[ActionLocalPortDetailsTypeDef],  # (3)
    Protocol: NotRequired[str],
    Blocked: NotRequired[bool],
```

1. See [:material-code-braces: ActionRemoteIpDetailsTypeDef](./type_defs.md#actionremoteipdetailstypedef) 
2. See [:material-code-braces: ActionRemotePortDetailsTypeDef](./type_defs.md#actionremoteportdetailstypedef) 
3. See [:material-code-braces: ActionLocalPortDetailsTypeDef](./type_defs.md#actionlocalportdetailstypedef) 
## PortProbeDetailTypeDef

```python
# PortProbeDetailTypeDef definition

class PortProbeDetailTypeDef(TypedDict):
    LocalPortDetails: NotRequired[ActionLocalPortDetailsTypeDef],  # (1)
    LocalIpDetails: NotRequired[ActionLocalIpDetailsTypeDef],  # (2)
    RemoteIpDetails: NotRequired[ActionRemoteIpDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: ActionLocalPortDetailsTypeDef](./type_defs.md#actionlocalportdetailstypedef) 
2. See [:material-code-braces: ActionLocalIpDetailsTypeDef](./type_defs.md#actionlocalipdetailstypedef) 
3. See [:material-code-braces: ActionRemoteIpDetailsTypeDef](./type_defs.md#actionremoteipdetailstypedef) 
## VulnerabilityTypeDef

```python
# VulnerabilityTypeDef definition

class VulnerabilityTypeDef(TypedDict):
    Id: str,
    VulnerablePackages: NotRequired[Sequence[SoftwarePackageTypeDef]],  # (1)
    Cvss: NotRequired[Sequence[CvssTypeDef]],  # (2)
    RelatedVulnerabilities: NotRequired[Sequence[str]],
    Vendor: NotRequired[VulnerabilityVendorTypeDef],  # (3)
    ReferenceUrls: NotRequired[Sequence[str]],
    FixAvailable: NotRequired[VulnerabilityFixAvailableType],  # (4)
```

1. See [:material-code-braces: SoftwarePackageTypeDef](./type_defs.md#softwarepackagetypedef) 
2. See [:material-code-braces: CvssTypeDef](./type_defs.md#cvsstypedef) 
3. See [:material-code-braces: VulnerabilityVendorTypeDef](./type_defs.md#vulnerabilityvendortypedef) 
4. See [:material-code-brackets: VulnerabilityFixAvailableType](./literals.md#vulnerabilityfixavailabletype) 
## AwsEc2RouteTableDetailsTypeDef

```python
# AwsEc2RouteTableDetailsTypeDef definition

class AwsEc2RouteTableDetailsTypeDef(TypedDict):
    AssociationSet: NotRequired[Sequence[AssociationSetDetailsTypeDef]],  # (1)
    OwnerId: NotRequired[str],
    PropagatingVgwSet: NotRequired[Sequence[PropagatingVgwSetDetailsTypeDef]],  # (2)
    RouteTableId: NotRequired[str],
    RouteSet: NotRequired[Sequence[RouteSetDetailsTypeDef]],  # (3)
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: AssociationSetDetailsTypeDef](./type_defs.md#associationsetdetailstypedef) 
2. See [:material-code-braces: PropagatingVgwSetDetailsTypeDef](./type_defs.md#propagatingvgwsetdetailstypedef) 
3. See [:material-code-braces: RouteSetDetailsTypeDef](./type_defs.md#routesetdetailstypedef) 
## AutomationRulesActionTypeDef

```python
# AutomationRulesActionTypeDef definition

class AutomationRulesActionTypeDef(TypedDict):
    Type: NotRequired[AutomationRulesActionTypeType],  # (1)
    FindingFieldsUpdate: NotRequired[AutomationRulesFindingFieldsUpdateTypeDef],  # (2)
```

1. See [:material-code-brackets: AutomationRulesActionTypeType](./literals.md#automationrulesactiontypetype) 
2. See [:material-code-braces: AutomationRulesFindingFieldsUpdateTypeDef](./type_defs.md#automationrulesfindingfieldsupdatetypedef) 
## AwsAmazonMqBrokerDetailsTypeDef

```python
# AwsAmazonMqBrokerDetailsTypeDef definition

class AwsAmazonMqBrokerDetailsTypeDef(TypedDict):
    AuthenticationStrategy: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    BrokerArn: NotRequired[str],
    BrokerName: NotRequired[str],
    DeploymentMode: NotRequired[str],
    EncryptionOptions: NotRequired[AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef],  # (1)
    EngineType: NotRequired[str],
    EngineVersion: NotRequired[str],
    HostInstanceType: NotRequired[str],
    BrokerId: NotRequired[str],
    LdapServerMetadata: NotRequired[AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef],  # (2)
    Logs: NotRequired[AwsAmazonMqBrokerLogsDetailsTypeDef],  # (3)
    MaintenanceWindowStartTime: NotRequired[AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef],  # (4)
    PubliclyAccessible: NotRequired[bool],
    SecurityGroups: NotRequired[Sequence[str]],
    StorageType: NotRequired[str],
    SubnetIds: NotRequired[Sequence[str]],
    Users: NotRequired[Sequence[AwsAmazonMqBrokerUsersDetailsTypeDef]],  # (5)
```

1. See [:material-code-braces: AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef](./type_defs.md#awsamazonmqbrokerencryptionoptionsdetailstypedef) 
2. See [:material-code-braces: AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef](./type_defs.md#awsamazonmqbrokerldapservermetadatadetailstypedef) 
3. See [:material-code-braces: AwsAmazonMqBrokerLogsDetailsTypeDef](./type_defs.md#awsamazonmqbrokerlogsdetailstypedef) 
4. See [:material-code-braces: AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef](./type_defs.md#awsamazonmqbrokermaintenancewindowstarttimedetailstypedef) 
5. See [:material-code-braces: AwsAmazonMqBrokerUsersDetailsTypeDef](./type_defs.md#awsamazonmqbrokerusersdetailstypedef) 
## AwsAppSyncGraphQlApiDetailsTypeDef

```python
# AwsAppSyncGraphQlApiDetailsTypeDef definition

class AwsAppSyncGraphQlApiDetailsTypeDef(TypedDict):
    ApiId: NotRequired[str],
    Id: NotRequired[str],
    OpenIdConnectConfig: NotRequired[AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef],  # (1)
    Name: NotRequired[str],
    LambdaAuthorizerConfig: NotRequired[AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef],  # (2)
    XrayEnabled: NotRequired[bool],
    Arn: NotRequired[str],
    UserPoolConfig: NotRequired[AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef],  # (3)
    AuthenticationType: NotRequired[str],
    LogConfig: NotRequired[AwsAppSyncGraphQlApiLogConfigDetailsTypeDef],  # (4)
    AdditionalAuthenticationProviders: NotRequired[Sequence[AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef]],  # (5)
    WafWebAclArn: NotRequired[str],
```

1. See [:material-code-braces: AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef](./type_defs.md#awsappsyncgraphqlapiopenidconnectconfigdetailstypedef) 
2. See [:material-code-braces: AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef](./type_defs.md#awsappsyncgraphqlapilambdaauthorizerconfigdetailstypedef) 
3. See [:material-code-braces: AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef](./type_defs.md#awsappsyncgraphqlapiuserpoolconfigdetailstypedef) 
4. See [:material-code-braces: AwsAppSyncGraphQlApiLogConfigDetailsTypeDef](./type_defs.md#awsappsyncgraphqlapilogconfigdetailstypedef) 
5. See [:material-code-braces: AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef](./type_defs.md#awsappsyncgraphqlapiadditionalauthenticationprovidersdetailstypedef) 
## AwsAthenaWorkGroupConfigurationDetailsTypeDef

```python
# AwsAthenaWorkGroupConfigurationDetailsTypeDef definition

class AwsAthenaWorkGroupConfigurationDetailsTypeDef(TypedDict):
    ResultConfiguration: NotRequired[AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef](./type_defs.md#awsathenaworkgroupconfigurationresultconfigurationdetailstypedef) 
## AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef

```python
# AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef definition

class AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef(TypedDict):
    InstancesDistribution: NotRequired[AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef],  # (1)
    LaunchTemplate: NotRequired[AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef](./type_defs.md#awsautoscalingautoscalinggroupmixedinstancespolicyinstancesdistributiondetailstypedef) 
2. See [:material-code-braces: AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef](./type_defs.md#awsautoscalingautoscalinggroupmixedinstancespolicylaunchtemplatedetailstypedef) 
## AwsAutoScalingLaunchConfigurationDetailsTypeDef

```python
# AwsAutoScalingLaunchConfigurationDetailsTypeDef definition

class AwsAutoScalingLaunchConfigurationDetailsTypeDef(TypedDict):
    AssociatePublicIpAddress: NotRequired[bool],
    BlockDeviceMappings: NotRequired[Sequence[AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef]],  # (1)
    ClassicLinkVpcId: NotRequired[str],
    ClassicLinkVpcSecurityGroups: NotRequired[Sequence[str]],
    CreatedTime: NotRequired[str],
    EbsOptimized: NotRequired[bool],
    IamInstanceProfile: NotRequired[str],
    ImageId: NotRequired[str],
    InstanceMonitoring: NotRequired[AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef],  # (2)
    InstanceType: NotRequired[str],
    KernelId: NotRequired[str],
    KeyName: NotRequired[str],
    LaunchConfigurationName: NotRequired[str],
    PlacementTenancy: NotRequired[str],
    RamdiskId: NotRequired[str],
    SecurityGroups: NotRequired[Sequence[str]],
    SpotPrice: NotRequired[str],
    UserData: NotRequired[str],
    MetadataOptions: NotRequired[AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef](./type_defs.md#awsautoscalinglaunchconfigurationblockdevicemappingsdetailstypedef) 
2. See [:material-code-braces: AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef](./type_defs.md#awsautoscalinglaunchconfigurationinstancemonitoringdetailstypedef) 
3. See [:material-code-braces: AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef](./type_defs.md#awsautoscalinglaunchconfigurationmetadataoptionstypedef) 
## AwsBackupBackupPlanRuleDetailsTypeDef

```python
# AwsBackupBackupPlanRuleDetailsTypeDef definition

class AwsBackupBackupPlanRuleDetailsTypeDef(TypedDict):
    TargetBackupVault: NotRequired[str],
    StartWindowMinutes: NotRequired[int],
    ScheduleExpression: NotRequired[str],
    RuleName: NotRequired[str],
    RuleId: NotRequired[str],
    EnableContinuousBackup: NotRequired[bool],
    CompletionWindowMinutes: NotRequired[int],
    CopyActions: NotRequired[Sequence[AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef]],  # (1)
    Lifecycle: NotRequired[AwsBackupBackupPlanLifecycleDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef](./type_defs.md#awsbackupbackupplanrulecopyactionsdetailstypedef) 
2. See [:material-code-braces: AwsBackupBackupPlanLifecycleDetailsTypeDef](./type_defs.md#awsbackupbackupplanlifecycledetailstypedef) 
## AwsCertificateManagerCertificateRenewalSummaryTypeDef

```python
# AwsCertificateManagerCertificateRenewalSummaryTypeDef definition

class AwsCertificateManagerCertificateRenewalSummaryTypeDef(TypedDict):
    DomainValidationOptions: NotRequired[Sequence[AwsCertificateManagerCertificateDomainValidationOptionTypeDef]],  # (1)
    RenewalStatus: NotRequired[str],
    RenewalStatusReason: NotRequired[str],
    UpdatedAt: NotRequired[str],
```

1. See [:material-code-braces: AwsCertificateManagerCertificateDomainValidationOptionTypeDef](./type_defs.md#awscertificatemanagercertificatedomainvalidationoptiontypedef) 
## AwsCloudFrontDistributionOriginItemTypeDef

```python
# AwsCloudFrontDistributionOriginItemTypeDef definition

class AwsCloudFrontDistributionOriginItemTypeDef(TypedDict):
    DomainName: NotRequired[str],
    Id: NotRequired[str],
    OriginPath: NotRequired[str],
    S3OriginConfig: NotRequired[AwsCloudFrontDistributionOriginS3OriginConfigTypeDef],  # (1)
    CustomOriginConfig: NotRequired[AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AwsCloudFrontDistributionOriginS3OriginConfigTypeDef](./type_defs.md#awscloudfrontdistributionorigins3originconfigtypedef) 
2. See [:material-code-braces: AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef](./type_defs.md#awscloudfrontdistributionorigincustomoriginconfigtypedef) 
## AwsCloudFrontDistributionOriginGroupTypeDef

```python
# AwsCloudFrontDistributionOriginGroupTypeDef definition

class AwsCloudFrontDistributionOriginGroupTypeDef(TypedDict):
    FailoverCriteria: NotRequired[AwsCloudFrontDistributionOriginGroupFailoverTypeDef],  # (1)
```

1. See [:material-code-braces: AwsCloudFrontDistributionOriginGroupFailoverTypeDef](./type_defs.md#awscloudfrontdistributionorigingroupfailovertypedef) 
## AwsCodeBuildProjectDetailsTypeDef

```python
# AwsCodeBuildProjectDetailsTypeDef definition

class AwsCodeBuildProjectDetailsTypeDef(TypedDict):
    EncryptionKey: NotRequired[str],
    Artifacts: NotRequired[Sequence[AwsCodeBuildProjectArtifactsDetailsTypeDef]],  # (1)
    Environment: NotRequired[AwsCodeBuildProjectEnvironmentTypeDef],  # (2)
    Name: NotRequired[str],
    Source: NotRequired[AwsCodeBuildProjectSourceTypeDef],  # (3)
    ServiceRole: NotRequired[str],
    LogsConfig: NotRequired[AwsCodeBuildProjectLogsConfigDetailsTypeDef],  # (4)
    VpcConfig: NotRequired[AwsCodeBuildProjectVpcConfigTypeDef],  # (5)
    SecondaryArtifacts: NotRequired[Sequence[AwsCodeBuildProjectArtifactsDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsCodeBuildProjectArtifactsDetailsTypeDef](./type_defs.md#awscodebuildprojectartifactsdetailstypedef) 
2. See [:material-code-braces: AwsCodeBuildProjectEnvironmentTypeDef](./type_defs.md#awscodebuildprojectenvironmenttypedef) 
3. See [:material-code-braces: AwsCodeBuildProjectSourceTypeDef](./type_defs.md#awscodebuildprojectsourcetypedef) 
4. See [:material-code-braces: AwsCodeBuildProjectLogsConfigDetailsTypeDef](./type_defs.md#awscodebuildprojectlogsconfigdetailstypedef) 
5. See [:material-code-braces: AwsCodeBuildProjectVpcConfigTypeDef](./type_defs.md#awscodebuildprojectvpcconfigtypedef) 
6. See [:material-code-braces: AwsCodeBuildProjectArtifactsDetailsTypeDef](./type_defs.md#awscodebuildprojectartifactsdetailstypedef) 
## AwsDynamoDbTableReplicaTypeDef

```python
# AwsDynamoDbTableReplicaTypeDef definition

class AwsDynamoDbTableReplicaTypeDef(TypedDict):
    GlobalSecondaryIndexes: NotRequired[Sequence[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef]],  # (1)
    KmsMasterKeyId: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[AwsDynamoDbTableProvisionedThroughputOverrideTypeDef],  # (2)
    RegionName: NotRequired[str],
    ReplicaStatus: NotRequired[str],
    ReplicaStatusDescription: NotRequired[str],
```

1. See [:material-code-braces: AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef](./type_defs.md#awsdynamodbtablereplicaglobalsecondaryindextypedef) 
2. See [:material-code-braces: AwsDynamoDbTableProvisionedThroughputOverrideTypeDef](./type_defs.md#awsdynamodbtableprovisionedthroughputoverridetypedef) 
## AwsEc2LaunchTemplateDataDetailsTypeDef

```python
# AwsEc2LaunchTemplateDataDetailsTypeDef definition

class AwsEc2LaunchTemplateDataDetailsTypeDef(TypedDict):
    BlockDeviceMappingSet: NotRequired[Sequence[AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef]],  # (1)
    CapacityReservationSpecification: NotRequired[AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef],  # (2)
    CpuOptions: NotRequired[AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef],  # (3)
    CreditSpecification: NotRequired[AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef],  # (4)
    DisableApiStop: NotRequired[bool],
    DisableApiTermination: NotRequired[bool],
    EbsOptimized: NotRequired[bool],
    ElasticGpuSpecificationSet: NotRequired[Sequence[AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef]],  # (5)
    ElasticInferenceAcceleratorSet: NotRequired[Sequence[AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef]],  # (6)
    EnclaveOptions: NotRequired[AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef],  # (7)
    HibernationOptions: NotRequired[AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef],  # (8)
    IamInstanceProfile: NotRequired[AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef],  # (9)
    ImageId: NotRequired[str],
    InstanceInitiatedShutdownBehavior: NotRequired[str],
    InstanceMarketOptions: NotRequired[AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef],  # (10)
    InstanceRequirements: NotRequired[AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef],  # (11)
    InstanceType: NotRequired[str],
    KernelId: NotRequired[str],
    KeyName: NotRequired[str],
    LicenseSet: NotRequired[Sequence[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef]],  # (12)
    MaintenanceOptions: NotRequired[AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef],  # (13)
    MetadataOptions: NotRequired[AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef],  # (14)
    Monitoring: NotRequired[AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef],  # (15)
    NetworkInterfaceSet: NotRequired[Sequence[AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef]],  # (16)
    Placement: NotRequired[AwsEc2LaunchTemplateDataPlacementDetailsTypeDef],  # (17)
    PrivateDnsNameOptions: NotRequired[AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef],  # (18)
    RamDiskId: NotRequired[str],
    SecurityGroupIdSet: NotRequired[Sequence[str]],
    SecurityGroupSet: NotRequired[Sequence[str]],
    UserData: NotRequired[str],
```

1. See [:material-code-braces: AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatablockdevicemappingsetdetailstypedef) 
2. See [:material-code-braces: AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatacapacityreservationspecificationdetailstypedef) 
3. See [:material-code-braces: AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatacpuoptionsdetailstypedef) 
4. See [:material-code-braces: AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatacreditspecificationdetailstypedef) 
5. See [:material-code-braces: AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef](./type_defs.md#awsec2launchtemplatedataelasticgpuspecificationsetdetailstypedef) 
6. See [:material-code-braces: AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef](./type_defs.md#awsec2launchtemplatedataelasticinferenceacceleratorsetdetailstypedef) 
7. See [:material-code-braces: AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef](./type_defs.md#awsec2launchtemplatedataenclaveoptionsdetailstypedef) 
8. See [:material-code-braces: AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatahibernationoptionsdetailstypedef) 
9. See [:material-code-braces: AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef](./type_defs.md#awsec2launchtemplatedataiaminstanceprofiledetailstypedef) 
10. See [:material-code-braces: AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatainstancemarketoptionsdetailstypedef) 
11. See [:material-code-braces: AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatainstancerequirementsdetailstypedef) 
12. See [:material-code-braces: AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatalicensesetdetailstypedef) 
13. See [:material-code-braces: AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatamaintenanceoptionsdetailstypedef) 
14. See [:material-code-braces: AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatametadataoptionsdetailstypedef) 
15. See [:material-code-braces: AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatamonitoringdetailstypedef) 
16. See [:material-code-braces: AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatanetworkinterfacesetdetailstypedef) 
17. See [:material-code-braces: AwsEc2LaunchTemplateDataPlacementDetailsTypeDef](./type_defs.md#awsec2launchtemplatedataplacementdetailstypedef) 
18. See [:material-code-braces: AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef](./type_defs.md#awsec2launchtemplatedataprivatednsnameoptionsdetailstypedef) 
## AwsEc2NetworkAclDetailsTypeDef

```python
# AwsEc2NetworkAclDetailsTypeDef definition

class AwsEc2NetworkAclDetailsTypeDef(TypedDict):
    IsDefault: NotRequired[bool],
    NetworkAclId: NotRequired[str],
    OwnerId: NotRequired[str],
    VpcId: NotRequired[str],
    Associations: NotRequired[Sequence[AwsEc2NetworkAclAssociationTypeDef]],  # (1)
    Entries: NotRequired[Sequence[AwsEc2NetworkAclEntryTypeDef]],  # (2)
```

1. See [:material-code-braces: AwsEc2NetworkAclAssociationTypeDef](./type_defs.md#awsec2networkaclassociationtypedef) 
2. See [:material-code-braces: AwsEc2NetworkAclEntryTypeDef](./type_defs.md#awsec2networkaclentrytypedef) 
## AwsEc2SecurityGroupDetailsTypeDef

```python
# AwsEc2SecurityGroupDetailsTypeDef definition

class AwsEc2SecurityGroupDetailsTypeDef(TypedDict):
    GroupName: NotRequired[str],
    GroupId: NotRequired[str],
    OwnerId: NotRequired[str],
    VpcId: NotRequired[str],
    IpPermissions: NotRequired[Sequence[AwsEc2SecurityGroupIpPermissionTypeDef]],  # (1)
    IpPermissionsEgress: NotRequired[Sequence[AwsEc2SecurityGroupIpPermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsEc2SecurityGroupIpPermissionTypeDef](./type_defs.md#awsec2securitygroupippermissiontypedef) 
2. See [:material-code-braces: AwsEc2SecurityGroupIpPermissionTypeDef](./type_defs.md#awsec2securitygroupippermissiontypedef) 
## AwsEc2VpcPeeringConnectionDetailsTypeDef

```python
# AwsEc2VpcPeeringConnectionDetailsTypeDef definition

class AwsEc2VpcPeeringConnectionDetailsTypeDef(TypedDict):
    AccepterVpcInfo: NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef],  # (1)
    ExpirationTime: NotRequired[str],
    RequesterVpcInfo: NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef],  # (1)
    Status: NotRequired[AwsEc2VpcPeeringConnectionStatusDetailsTypeDef],  # (3)
    VpcPeeringConnectionId: NotRequired[str],
```

1. See [:material-code-braces: AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef](./type_defs.md#awsec2vpcpeeringconnectionvpcinfodetailstypedef) 
2. See [:material-code-braces: AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef](./type_defs.md#awsec2vpcpeeringconnectionvpcinfodetailstypedef) 
3. See [:material-code-braces: AwsEc2VpcPeeringConnectionStatusDetailsTypeDef](./type_defs.md#awsec2vpcpeeringconnectionstatusdetailstypedef) 
## AwsEc2VpnConnectionDetailsTypeDef

```python
# AwsEc2VpnConnectionDetailsTypeDef definition

class AwsEc2VpnConnectionDetailsTypeDef(TypedDict):
    VpnConnectionId: NotRequired[str],
    State: NotRequired[str],
    CustomerGatewayId: NotRequired[str],
    CustomerGatewayConfiguration: NotRequired[str],
    Type: NotRequired[str],
    VpnGatewayId: NotRequired[str],
    Category: NotRequired[str],
    VgwTelemetry: NotRequired[Sequence[AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef]],  # (1)
    Options: NotRequired[AwsEc2VpnConnectionOptionsDetailsTypeDef],  # (2)
    Routes: NotRequired[Sequence[AwsEc2VpnConnectionRoutesDetailsTypeDef]],  # (3)
    TransitGatewayId: NotRequired[str],
```

1. See [:material-code-braces: AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef](./type_defs.md#awsec2vpnconnectionvgwtelemetrydetailstypedef) 
2. See [:material-code-braces: AwsEc2VpnConnectionOptionsDetailsTypeDef](./type_defs.md#awsec2vpnconnectionoptionsdetailstypedef) 
3. See [:material-code-braces: AwsEc2VpnConnectionRoutesDetailsTypeDef](./type_defs.md#awsec2vpnconnectionroutesdetailstypedef) 
## AwsEcsClusterConfigurationDetailsTypeDef

```python
# AwsEcsClusterConfigurationDetailsTypeDef definition

class AwsEcsClusterConfigurationDetailsTypeDef(TypedDict):
    ExecuteCommandConfiguration: NotRequired[AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef](./type_defs.md#awsecsclusterconfigurationexecutecommandconfigurationdetailstypedef) 
## AwsEcsServiceDetailsTypeDef

```python
# AwsEcsServiceDetailsTypeDef definition

class AwsEcsServiceDetailsTypeDef(TypedDict):
    CapacityProviderStrategy: NotRequired[Sequence[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef]],  # (1)
    Cluster: NotRequired[str],
    DeploymentConfiguration: NotRequired[AwsEcsServiceDeploymentConfigurationDetailsTypeDef],  # (2)
    DeploymentController: NotRequired[AwsEcsServiceDeploymentControllerDetailsTypeDef],  # (3)
    DesiredCount: NotRequired[int],
    EnableEcsManagedTags: NotRequired[bool],
    EnableExecuteCommand: NotRequired[bool],
    HealthCheckGracePeriodSeconds: NotRequired[int],
    LaunchType: NotRequired[str],
    LoadBalancers: NotRequired[Sequence[AwsEcsServiceLoadBalancersDetailsTypeDef]],  # (4)
    Name: NotRequired[str],
    NetworkConfiguration: NotRequired[AwsEcsServiceNetworkConfigurationDetailsTypeDef],  # (5)
    PlacementConstraints: NotRequired[Sequence[AwsEcsServicePlacementConstraintsDetailsTypeDef]],  # (6)
    PlacementStrategies: NotRequired[Sequence[AwsEcsServicePlacementStrategiesDetailsTypeDef]],  # (7)
    PlatformVersion: NotRequired[str],
    PropagateTags: NotRequired[str],
    Role: NotRequired[str],
    SchedulingStrategy: NotRequired[str],
    ServiceArn: NotRequired[str],
    ServiceName: NotRequired[str],
    ServiceRegistries: NotRequired[Sequence[AwsEcsServiceServiceRegistriesDetailsTypeDef]],  # (8)
    TaskDefinition: NotRequired[str],
```

1. See [:material-code-braces: AwsEcsServiceCapacityProviderStrategyDetailsTypeDef](./type_defs.md#awsecsservicecapacityproviderstrategydetailstypedef) 
2. See [:material-code-braces: AwsEcsServiceDeploymentConfigurationDetailsTypeDef](./type_defs.md#awsecsservicedeploymentconfigurationdetailstypedef) 
3. See [:material-code-braces: AwsEcsServiceDeploymentControllerDetailsTypeDef](./type_defs.md#awsecsservicedeploymentcontrollerdetailstypedef) 
4. See [:material-code-braces: AwsEcsServiceLoadBalancersDetailsTypeDef](./type_defs.md#awsecsserviceloadbalancersdetailstypedef) 
5. See [:material-code-braces: AwsEcsServiceNetworkConfigurationDetailsTypeDef](./type_defs.md#awsecsservicenetworkconfigurationdetailstypedef) 
6. See [:material-code-braces: AwsEcsServicePlacementConstraintsDetailsTypeDef](./type_defs.md#awsecsserviceplacementconstraintsdetailstypedef) 
7. See [:material-code-braces: AwsEcsServicePlacementStrategiesDetailsTypeDef](./type_defs.md#awsecsserviceplacementstrategiesdetailstypedef) 
8. See [:material-code-braces: AwsEcsServiceServiceRegistriesDetailsTypeDef](./type_defs.md#awsecsserviceserviceregistriesdetailstypedef) 
## AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef

```python
# AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef definition

class AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef(TypedDict):
    Command: NotRequired[Sequence[str]],
    Cpu: NotRequired[int],
    DependsOn: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef]],  # (1)
    DisableNetworking: NotRequired[bool],
    DnsSearchDomains: NotRequired[Sequence[str]],
    DnsServers: NotRequired[Sequence[str]],
    DockerLabels: NotRequired[Mapping[str, str]],
    DockerSecurityOptions: NotRequired[Sequence[str]],
    EntryPoint: NotRequired[Sequence[str]],
    Environment: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef]],  # (2)
    EnvironmentFiles: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef]],  # (3)
    Essential: NotRequired[bool],
    ExtraHosts: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef]],  # (4)
    FirelensConfiguration: NotRequired[AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef],  # (5)
    HealthCheck: NotRequired[AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef],  # (6)
    Hostname: NotRequired[str],
    Image: NotRequired[str],
    Interactive: NotRequired[bool],
    Links: NotRequired[Sequence[str]],
    LinuxParameters: NotRequired[AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef],  # (7)
    LogConfiguration: NotRequired[AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef],  # (8)
    Memory: NotRequired[int],
    MemoryReservation: NotRequired[int],
    MountPoints: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef]],  # (9)
    Name: NotRequired[str],
    PortMappings: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef]],  # (10)
    Privileged: NotRequired[bool],
    PseudoTerminal: NotRequired[bool],
    ReadonlyRootFilesystem: NotRequired[bool],
    RepositoryCredentials: NotRequired[AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef],  # (11)
    ResourceRequirements: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef]],  # (12)
    Secrets: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef]],  # (13)
    StartTimeout: NotRequired[int],
    StopTimeout: NotRequired[int],
    SystemControls: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef]],  # (14)
    Ulimits: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef]],  # (15)
    User: NotRequired[str],
    VolumesFrom: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef]],  # (16)
    WorkingDirectory: NotRequired[str],
```

1. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsdependsondetailstypedef) 
2. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsenvironmentdetailstypedef) 
3. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsenvironmentfilesdetailstypedef) 
4. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsextrahostsdetailstypedef) 
5. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsfirelensconfigurationdetailstypedef) 
6. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionshealthcheckdetailstypedef) 
7. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionslinuxparametersdetailstypedef) 
8. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionslogconfigurationdetailstypedef) 
9. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsmountpointsdetailstypedef) 
10. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsportmappingsdetailstypedef) 
11. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsrepositorycredentialsdetailstypedef) 
12. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsresourcerequirementsdetailstypedef) 
13. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionssecretsdetailstypedef) 
14. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionssystemcontrolsdetailstypedef) 
15. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsulimitsdetailstypedef) 
16. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsvolumesfromdetailstypedef) 
## AwsEcsTaskDefinitionVolumesDetailsTypeDef

```python
# AwsEcsTaskDefinitionVolumesDetailsTypeDef definition

class AwsEcsTaskDefinitionVolumesDetailsTypeDef(TypedDict):
    DockerVolumeConfiguration: NotRequired[AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef],  # (1)
    EfsVolumeConfiguration: NotRequired[AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef],  # (2)
    Host: NotRequired[AwsEcsTaskDefinitionVolumesHostDetailsTypeDef],  # (3)
    Name: NotRequired[str],
```

1. See [:material-code-braces: AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef](./type_defs.md#awsecstaskdefinitionvolumesdockervolumeconfigurationdetailstypedef) 
2. See [:material-code-braces: AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef](./type_defs.md#awsecstaskdefinitionvolumesefsvolumeconfigurationdetailstypedef) 
3. See [:material-code-braces: AwsEcsTaskDefinitionVolumesHostDetailsTypeDef](./type_defs.md#awsecstaskdefinitionvolumeshostdetailstypedef) 
## AwsEcsTaskDetailsTypeDef

```python
# AwsEcsTaskDetailsTypeDef definition

class AwsEcsTaskDetailsTypeDef(TypedDict):
    ClusterArn: NotRequired[str],
    TaskDefinitionArn: NotRequired[str],
    Version: NotRequired[str],
    CreatedAt: NotRequired[str],
    StartedAt: NotRequired[str],
    StartedBy: NotRequired[str],
    Group: NotRequired[str],
    Volumes: NotRequired[Sequence[AwsEcsTaskVolumeDetailsTypeDef]],  # (1)
    Containers: NotRequired[Sequence[AwsEcsContainerDetailsTypeDef]],  # (2)
```

1. See [:material-code-braces: AwsEcsTaskVolumeDetailsTypeDef](./type_defs.md#awsecstaskvolumedetailstypedef) 
2. See [:material-code-braces: AwsEcsContainerDetailsTypeDef](./type_defs.md#awsecscontainerdetailstypedef) 
## AwsEfsAccessPointDetailsTypeDef

```python
# AwsEfsAccessPointDetailsTypeDef definition

class AwsEfsAccessPointDetailsTypeDef(TypedDict):
    AccessPointId: NotRequired[str],
    Arn: NotRequired[str],
    ClientToken: NotRequired[str],
    FileSystemId: NotRequired[str],
    PosixUser: NotRequired[AwsEfsAccessPointPosixUserDetailsTypeDef],  # (1)
    RootDirectory: NotRequired[AwsEfsAccessPointRootDirectoryDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: AwsEfsAccessPointPosixUserDetailsTypeDef](./type_defs.md#awsefsaccesspointposixuserdetailstypedef) 
2. See [:material-code-braces: AwsEfsAccessPointRootDirectoryDetailsTypeDef](./type_defs.md#awsefsaccesspointrootdirectorydetailstypedef) 
## AwsEksClusterDetailsTypeDef

```python
# AwsEksClusterDetailsTypeDef definition

class AwsEksClusterDetailsTypeDef(TypedDict):
    Arn: NotRequired[str],
    CertificateAuthorityData: NotRequired[str],
    ClusterStatus: NotRequired[str],
    Endpoint: NotRequired[str],
    Name: NotRequired[str],
    ResourcesVpcConfig: NotRequired[AwsEksClusterResourcesVpcConfigDetailsTypeDef],  # (1)
    RoleArn: NotRequired[str],
    Version: NotRequired[str],
    Logging: NotRequired[AwsEksClusterLoggingDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: AwsEksClusterResourcesVpcConfigDetailsTypeDef](./type_defs.md#awseksclusterresourcesvpcconfigdetailstypedef) 
2. See [:material-code-braces: AwsEksClusterLoggingDetailsTypeDef](./type_defs.md#awseksclusterloggingdetailstypedef) 
## AwsElasticsearchDomainDetailsTypeDef

```python
# AwsElasticsearchDomainDetailsTypeDef definition

class AwsElasticsearchDomainDetailsTypeDef(TypedDict):
    AccessPolicies: NotRequired[str],
    DomainEndpointOptions: NotRequired[AwsElasticsearchDomainDomainEndpointOptionsTypeDef],  # (1)
    DomainId: NotRequired[str],
    DomainName: NotRequired[str],
    Endpoint: NotRequired[str],
    Endpoints: NotRequired[Mapping[str, str]],
    ElasticsearchVersion: NotRequired[str],
    ElasticsearchClusterConfig: NotRequired[AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef],  # (2)
    EncryptionAtRestOptions: NotRequired[AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef],  # (3)
    LogPublishingOptions: NotRequired[AwsElasticsearchDomainLogPublishingOptionsTypeDef],  # (4)
    NodeToNodeEncryptionOptions: NotRequired[AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef],  # (5)
    ServiceSoftwareOptions: NotRequired[AwsElasticsearchDomainServiceSoftwareOptionsTypeDef],  # (6)
    VPCOptions: NotRequired[AwsElasticsearchDomainVPCOptionsTypeDef],  # (7)
```

1. See [:material-code-braces: AwsElasticsearchDomainDomainEndpointOptionsTypeDef](./type_defs.md#awselasticsearchdomaindomainendpointoptionstypedef) 
2. See [:material-code-braces: AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef](./type_defs.md#awselasticsearchdomainelasticsearchclusterconfigdetailstypedef) 
3. See [:material-code-braces: AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef](./type_defs.md#awselasticsearchdomainencryptionatrestoptionstypedef) 
4. See [:material-code-braces: AwsElasticsearchDomainLogPublishingOptionsTypeDef](./type_defs.md#awselasticsearchdomainlogpublishingoptionstypedef) 
5. See [:material-code-braces: AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef](./type_defs.md#awselasticsearchdomainnodetonodeencryptionoptionstypedef) 
6. See [:material-code-braces: AwsElasticsearchDomainServiceSoftwareOptionsTypeDef](./type_defs.md#awselasticsearchdomainservicesoftwareoptionstypedef) 
7. See [:material-code-braces: AwsElasticsearchDomainVPCOptionsTypeDef](./type_defs.md#awselasticsearchdomainvpcoptionstypedef) 
## AwsElbLoadBalancerDetailsTypeDef

```python
# AwsElbLoadBalancerDetailsTypeDef definition

class AwsElbLoadBalancerDetailsTypeDef(TypedDict):
    AvailabilityZones: NotRequired[Sequence[str]],
    BackendServerDescriptions: NotRequired[Sequence[AwsElbLoadBalancerBackendServerDescriptionTypeDef]],  # (1)
    CanonicalHostedZoneName: NotRequired[str],
    CanonicalHostedZoneNameID: NotRequired[str],
    CreatedTime: NotRequired[str],
    DnsName: NotRequired[str],
    HealthCheck: NotRequired[AwsElbLoadBalancerHealthCheckTypeDef],  # (2)
    Instances: NotRequired[Sequence[AwsElbLoadBalancerInstanceTypeDef]],  # (3)
    ListenerDescriptions: NotRequired[Sequence[AwsElbLoadBalancerListenerDescriptionTypeDef]],  # (4)
    LoadBalancerAttributes: NotRequired[AwsElbLoadBalancerAttributesTypeDef],  # (5)
    LoadBalancerName: NotRequired[str],
    Policies: NotRequired[AwsElbLoadBalancerPoliciesTypeDef],  # (6)
    Scheme: NotRequired[str],
    SecurityGroups: NotRequired[Sequence[str]],
    SourceSecurityGroup: NotRequired[AwsElbLoadBalancerSourceSecurityGroupTypeDef],  # (7)
    Subnets: NotRequired[Sequence[str]],
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: AwsElbLoadBalancerBackendServerDescriptionTypeDef](./type_defs.md#awselbloadbalancerbackendserverdescriptiontypedef) 
2. See [:material-code-braces: AwsElbLoadBalancerHealthCheckTypeDef](./type_defs.md#awselbloadbalancerhealthchecktypedef) 
3. See [:material-code-braces: AwsElbLoadBalancerInstanceTypeDef](./type_defs.md#awselbloadbalancerinstancetypedef) 
4. See [:material-code-braces: AwsElbLoadBalancerListenerDescriptionTypeDef](./type_defs.md#awselbloadbalancerlistenerdescriptiontypedef) 
5. See [:material-code-braces: AwsElbLoadBalancerAttributesTypeDef](./type_defs.md#awselbloadbalancerattributestypedef) 
6. See [:material-code-braces: AwsElbLoadBalancerPoliciesTypeDef](./type_defs.md#awselbloadbalancerpoliciestypedef) 
7. See [:material-code-braces: AwsElbLoadBalancerSourceSecurityGroupTypeDef](./type_defs.md#awselbloadbalancersourcesecuritygrouptypedef) 
## AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef

```python
# AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef definition

class AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef(TypedDict):
    ScanEc2InstanceWithFindings: NotRequired[AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef],  # (1)
    ServiceRole: NotRequired[str],
```

1. See [:material-code-braces: AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef](./type_defs.md#awsguarddutydetectordatasourcesmalwareprotectionscanec2instancewithfindingsdetailstypedef) 
## AwsIamAccessKeyDetailsTypeDef

```python
# AwsIamAccessKeyDetailsTypeDef definition

class AwsIamAccessKeyDetailsTypeDef(TypedDict):
    UserName: NotRequired[str],
    Status: NotRequired[AwsIamAccessKeyStatusType],  # (1)
    CreatedAt: NotRequired[str],
    PrincipalId: NotRequired[str],
    PrincipalType: NotRequired[str],
    PrincipalName: NotRequired[str],
    AccountId: NotRequired[str],
    AccessKeyId: NotRequired[str],
    SessionContext: NotRequired[AwsIamAccessKeySessionContextTypeDef],  # (2)
```

1. See [:material-code-brackets: AwsIamAccessKeyStatusType](./literals.md#awsiamaccesskeystatustype) 
2. See [:material-code-braces: AwsIamAccessKeySessionContextTypeDef](./type_defs.md#awsiamaccesskeysessioncontexttypedef) 
## AwsIamRoleDetailsTypeDef

```python
# AwsIamRoleDetailsTypeDef definition

class AwsIamRoleDetailsTypeDef(TypedDict):
    AssumeRolePolicyDocument: NotRequired[str],
    AttachedManagedPolicies: NotRequired[Sequence[AwsIamAttachedManagedPolicyTypeDef]],  # (1)
    CreateDate: NotRequired[str],
    InstanceProfileList: NotRequired[Sequence[AwsIamInstanceProfileTypeDef]],  # (2)
    PermissionsBoundary: NotRequired[AwsIamPermissionsBoundaryTypeDef],  # (3)
    RoleId: NotRequired[str],
    RoleName: NotRequired[str],
    RolePolicyList: NotRequired[Sequence[AwsIamRolePolicyTypeDef]],  # (4)
    MaxSessionDuration: NotRequired[int],
    Path: NotRequired[str],
```

1. See [:material-code-braces: AwsIamAttachedManagedPolicyTypeDef](./type_defs.md#awsiamattachedmanagedpolicytypedef) 
2. See [:material-code-braces: AwsIamInstanceProfileTypeDef](./type_defs.md#awsiaminstanceprofiletypedef) 
3. See [:material-code-braces: AwsIamPermissionsBoundaryTypeDef](./type_defs.md#awsiampermissionsboundarytypedef) 
4. See [:material-code-braces: AwsIamRolePolicyTypeDef](./type_defs.md#awsiamrolepolicytypedef) 
## AwsLambdaFunctionDetailsTypeDef

```python
# AwsLambdaFunctionDetailsTypeDef definition

class AwsLambdaFunctionDetailsTypeDef(TypedDict):
    Code: NotRequired[AwsLambdaFunctionCodeTypeDef],  # (1)
    CodeSha256: NotRequired[str],
    DeadLetterConfig: NotRequired[AwsLambdaFunctionDeadLetterConfigTypeDef],  # (2)
    Environment: NotRequired[AwsLambdaFunctionEnvironmentTypeDef],  # (3)
    FunctionName: NotRequired[str],
    Handler: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    LastModified: NotRequired[str],
    Layers: NotRequired[Sequence[AwsLambdaFunctionLayerTypeDef]],  # (4)
    MasterArn: NotRequired[str],
    MemorySize: NotRequired[int],
    RevisionId: NotRequired[str],
    Role: NotRequired[str],
    Runtime: NotRequired[str],
    Timeout: NotRequired[int],
    TracingConfig: NotRequired[AwsLambdaFunctionTracingConfigTypeDef],  # (5)
    VpcConfig: NotRequired[AwsLambdaFunctionVpcConfigTypeDef],  # (6)
    Version: NotRequired[str],
    Architectures: NotRequired[Sequence[str]],
    PackageType: NotRequired[str],
```

1. See [:material-code-braces: AwsLambdaFunctionCodeTypeDef](./type_defs.md#awslambdafunctioncodetypedef) 
2. See [:material-code-braces: AwsLambdaFunctionDeadLetterConfigTypeDef](./type_defs.md#awslambdafunctiondeadletterconfigtypedef) 
3. See [:material-code-braces: AwsLambdaFunctionEnvironmentTypeDef](./type_defs.md#awslambdafunctionenvironmenttypedef) 
4. See [:material-code-braces: AwsLambdaFunctionLayerTypeDef](./type_defs.md#awslambdafunctionlayertypedef) 
5. See [:material-code-braces: AwsLambdaFunctionTracingConfigTypeDef](./type_defs.md#awslambdafunctiontracingconfigtypedef) 
6. See [:material-code-braces: AwsLambdaFunctionVpcConfigTypeDef](./type_defs.md#awslambdafunctionvpcconfigtypedef) 
## AwsOpenSearchServiceDomainDetailsTypeDef

```python
# AwsOpenSearchServiceDomainDetailsTypeDef definition

class AwsOpenSearchServiceDomainDetailsTypeDef(TypedDict):
    Arn: NotRequired[str],
    AccessPolicies: NotRequired[str],
    DomainName: NotRequired[str],
    Id: NotRequired[str],
    DomainEndpoint: NotRequired[str],
    EngineVersion: NotRequired[str],
    EncryptionAtRestOptions: NotRequired[AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef],  # (1)
    NodeToNodeEncryptionOptions: NotRequired[AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef],  # (2)
    ServiceSoftwareOptions: NotRequired[AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef],  # (3)
    ClusterConfig: NotRequired[AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef],  # (4)
    DomainEndpointOptions: NotRequired[AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef],  # (5)
    VpcOptions: NotRequired[AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef],  # (6)
    LogPublishingOptions: NotRequired[AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef],  # (7)
    DomainEndpoints: NotRequired[Mapping[str, str]],
    AdvancedSecurityOptions: NotRequired[AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef],  # (8)
```

1. See [:material-code-braces: AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef](./type_defs.md#awsopensearchservicedomainencryptionatrestoptionsdetailstypedef) 
2. See [:material-code-braces: AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef](./type_defs.md#awsopensearchservicedomainnodetonodeencryptionoptionsdetailstypedef) 
3. See [:material-code-braces: AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef](./type_defs.md#awsopensearchservicedomainservicesoftwareoptionsdetailstypedef) 
4. See [:material-code-braces: AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef](./type_defs.md#awsopensearchservicedomainclusterconfigdetailstypedef) 
5. See [:material-code-braces: AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef](./type_defs.md#awsopensearchservicedomaindomainendpointoptionsdetailstypedef) 
6. See [:material-code-braces: AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef](./type_defs.md#awsopensearchservicedomainvpcoptionsdetailstypedef) 
7. See [:material-code-braces: AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef](./type_defs.md#awsopensearchservicedomainlogpublishingoptionsdetailstypedef) 
8. See [:material-code-braces: AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef](./type_defs.md#awsopensearchservicedomainadvancedsecurityoptionsdetailstypedef) 
## AwsRdsDbSubnetGroupTypeDef

```python
# AwsRdsDbSubnetGroupTypeDef definition

class AwsRdsDbSubnetGroupTypeDef(TypedDict):
    DbSubnetGroupName: NotRequired[str],
    DbSubnetGroupDescription: NotRequired[str],
    VpcId: NotRequired[str],
    SubnetGroupStatus: NotRequired[str],
    Subnets: NotRequired[Sequence[AwsRdsDbSubnetGroupSubnetTypeDef]],  # (1)
    DbSubnetGroupArn: NotRequired[str],
```

1. See [:material-code-braces: AwsRdsDbSubnetGroupSubnetTypeDef](./type_defs.md#awsrdsdbsubnetgroupsubnettypedef) 
## AwsRedshiftClusterDetailsTypeDef

```python
# AwsRedshiftClusterDetailsTypeDef definition

class AwsRedshiftClusterDetailsTypeDef(TypedDict):
    AllowVersionUpgrade: NotRequired[bool],
    AutomatedSnapshotRetentionPeriod: NotRequired[int],
    AvailabilityZone: NotRequired[str],
    ClusterAvailabilityStatus: NotRequired[str],
    ClusterCreateTime: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
    ClusterNodes: NotRequired[Sequence[AwsRedshiftClusterClusterNodeTypeDef]],  # (1)
    ClusterParameterGroups: NotRequired[Sequence[AwsRedshiftClusterClusterParameterGroupTypeDef]],  # (2)
    ClusterPublicKey: NotRequired[str],
    ClusterRevisionNumber: NotRequired[str],
    ClusterSecurityGroups: NotRequired[Sequence[AwsRedshiftClusterClusterSecurityGroupTypeDef]],  # (3)
    ClusterSnapshotCopyStatus: NotRequired[AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef],  # (4)
    ClusterStatus: NotRequired[str],
    ClusterSubnetGroupName: NotRequired[str],
    ClusterVersion: NotRequired[str],
    DBName: NotRequired[str],
    DeferredMaintenanceWindows: NotRequired[Sequence[AwsRedshiftClusterDeferredMaintenanceWindowTypeDef]],  # (5)
    ElasticIpStatus: NotRequired[AwsRedshiftClusterElasticIpStatusTypeDef],  # (6)
    ElasticResizeNumberOfNodeOptions: NotRequired[str],
    Encrypted: NotRequired[bool],
    Endpoint: NotRequired[AwsRedshiftClusterEndpointTypeDef],  # (7)
    EnhancedVpcRouting: NotRequired[bool],
    ExpectedNextSnapshotScheduleTime: NotRequired[str],
    ExpectedNextSnapshotScheduleTimeStatus: NotRequired[str],
    HsmStatus: NotRequired[AwsRedshiftClusterHsmStatusTypeDef],  # (8)
    IamRoles: NotRequired[Sequence[AwsRedshiftClusterIamRoleTypeDef]],  # (9)
    KmsKeyId: NotRequired[str],
    MaintenanceTrackName: NotRequired[str],
    ManualSnapshotRetentionPeriod: NotRequired[int],
    MasterUsername: NotRequired[str],
    NextMaintenanceWindowStartTime: NotRequired[str],
    NodeType: NotRequired[str],
    NumberOfNodes: NotRequired[int],
    PendingActions: NotRequired[Sequence[str]],
    PendingModifiedValues: NotRequired[AwsRedshiftClusterPendingModifiedValuesTypeDef],  # (10)
    PreferredMaintenanceWindow: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    ResizeInfo: NotRequired[AwsRedshiftClusterResizeInfoTypeDef],  # (11)
    RestoreStatus: NotRequired[AwsRedshiftClusterRestoreStatusTypeDef],  # (12)
    SnapshotScheduleIdentifier: NotRequired[str],
    SnapshotScheduleState: NotRequired[str],
    VpcId: NotRequired[str],
    VpcSecurityGroups: NotRequired[Sequence[AwsRedshiftClusterVpcSecurityGroupTypeDef]],  # (13)
    LoggingStatus: NotRequired[AwsRedshiftClusterLoggingStatusTypeDef],  # (14)
```

1. See [:material-code-braces: AwsRedshiftClusterClusterNodeTypeDef](./type_defs.md#awsredshiftclusterclusternodetypedef) 
2. See [:material-code-braces: AwsRedshiftClusterClusterParameterGroupTypeDef](./type_defs.md#awsredshiftclusterclusterparametergrouptypedef) 
3. See [:material-code-braces: AwsRedshiftClusterClusterSecurityGroupTypeDef](./type_defs.md#awsredshiftclusterclustersecuritygrouptypedef) 
4. See [:material-code-braces: AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef](./type_defs.md#awsredshiftclusterclustersnapshotcopystatustypedef) 
5. See [:material-code-braces: AwsRedshiftClusterDeferredMaintenanceWindowTypeDef](./type_defs.md#awsredshiftclusterdeferredmaintenancewindowtypedef) 
6. See [:material-code-braces: AwsRedshiftClusterElasticIpStatusTypeDef](./type_defs.md#awsredshiftclusterelasticipstatustypedef) 
7. See [:material-code-braces: AwsRedshiftClusterEndpointTypeDef](./type_defs.md#awsredshiftclusterendpointtypedef) 
8. See [:material-code-braces: AwsRedshiftClusterHsmStatusTypeDef](./type_defs.md#awsredshiftclusterhsmstatustypedef) 
9. See [:material-code-braces: AwsRedshiftClusterIamRoleTypeDef](./type_defs.md#awsredshiftclusteriamroletypedef) 
10. See [:material-code-braces: AwsRedshiftClusterPendingModifiedValuesTypeDef](./type_defs.md#awsredshiftclusterpendingmodifiedvaluestypedef) 
11. See [:material-code-braces: AwsRedshiftClusterResizeInfoTypeDef](./type_defs.md#awsredshiftclusterresizeinfotypedef) 
12. See [:material-code-braces: AwsRedshiftClusterRestoreStatusTypeDef](./type_defs.md#awsredshiftclusterrestorestatustypedef) 
13. See [:material-code-braces: AwsRedshiftClusterVpcSecurityGroupTypeDef](./type_defs.md#awsredshiftclustervpcsecuritygrouptypedef) 
14. See [:material-code-braces: AwsRedshiftClusterLoggingStatusTypeDef](./type_defs.md#awsredshiftclusterloggingstatustypedef) 
## AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef

```python
# AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef definition

class AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef(TypedDict):
    Operands: NotRequired[Sequence[AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef]],  # (1)
    Prefix: NotRequired[str],
    Tag: NotRequired[AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef],  # (2)
    Type: NotRequired[str],
```

1. See [:material-code-braces: AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef](./type_defs.md#awss3bucketbucketlifecycleconfigurationrulesfilterpredicateoperandsdetailstypedef) 
2. See [:material-code-braces: AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef](./type_defs.md#awss3bucketbucketlifecycleconfigurationrulesfilterpredicatetagdetailstypedef) 
## AwsS3BucketNotificationConfigurationFilterTypeDef

```python
# AwsS3BucketNotificationConfigurationFilterTypeDef definition

class AwsS3BucketNotificationConfigurationFilterTypeDef(TypedDict):
    S3KeyFilter: NotRequired[AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef],  # (1)
```

1. See [:material-code-braces: AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef](./type_defs.md#awss3bucketnotificationconfigurations3keyfiltertypedef) 
## AwsS3BucketObjectLockConfigurationTypeDef

```python
# AwsS3BucketObjectLockConfigurationTypeDef definition

class AwsS3BucketObjectLockConfigurationTypeDef(TypedDict):
    ObjectLockEnabled: NotRequired[str],
    Rule: NotRequired[AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef](./type_defs.md#awss3bucketobjectlockconfigurationruledetailstypedef) 
## AwsS3BucketServerSideEncryptionConfigurationTypeDef

```python
# AwsS3BucketServerSideEncryptionConfigurationTypeDef definition

class AwsS3BucketServerSideEncryptionConfigurationTypeDef(TypedDict):
    Rules: NotRequired[Sequence[AwsS3BucketServerSideEncryptionRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsS3BucketServerSideEncryptionRuleTypeDef](./type_defs.md#awss3bucketserversideencryptionruletypedef) 
## AwsS3BucketWebsiteConfigurationTypeDef

```python
# AwsS3BucketWebsiteConfigurationTypeDef definition

class AwsS3BucketWebsiteConfigurationTypeDef(TypedDict):
    ErrorDocument: NotRequired[str],
    IndexDocumentSuffix: NotRequired[str],
    RedirectAllRequestsTo: NotRequired[AwsS3BucketWebsiteConfigurationRedirectToTypeDef],  # (1)
    RoutingRules: NotRequired[Sequence[AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef]],  # (2)
```

1. See [:material-code-braces: AwsS3BucketWebsiteConfigurationRedirectToTypeDef](./type_defs.md#awss3bucketwebsiteconfigurationredirecttotypedef) 
2. See [:material-code-braces: AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef](./type_defs.md#awss3bucketwebsiteconfigurationroutingruletypedef) 
## BatchUpdateFindingsResponseTypeDef

```python
# BatchUpdateFindingsResponseTypeDef definition

class BatchUpdateFindingsResponseTypeDef(TypedDict):
    ProcessedFindings: List[AwsSecurityFindingIdentifierTypeDef],  # (1)
    UnprocessedFindings: List[BatchUpdateFindingsUnprocessedFindingTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AwsSecurityFindingIdentifierTypeDef](./type_defs.md#awssecurityfindingidentifiertypedef) 
2. See [:material-code-braces: BatchUpdateFindingsUnprocessedFindingTypeDef](./type_defs.md#batchupdatefindingsunprocessedfindingtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AwsSsmPatchComplianceDetailsTypeDef

```python
# AwsSsmPatchComplianceDetailsTypeDef definition

class AwsSsmPatchComplianceDetailsTypeDef(TypedDict):
    Patch: NotRequired[AwsSsmPatchTypeDef],  # (1)
```

1. See [:material-code-braces: AwsSsmPatchTypeDef](./type_defs.md#awsssmpatchtypedef) 
## AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef

```python
# AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef definition

class AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef(TypedDict):
    Destinations: NotRequired[Sequence[AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef]],  # (1)
    IncludeExecutionData: NotRequired[bool],
    Level: NotRequired[str],
```

1. See [:material-code-braces: AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef](./type_defs.md#awsstepfunctionstatemachineloggingconfigurationdestinationsdetailstypedef) 
## AwsWafRegionalRuleGroupDetailsTypeDef

```python
# AwsWafRegionalRuleGroupDetailsTypeDef definition

class AwsWafRegionalRuleGroupDetailsTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Name: NotRequired[str],
    RuleGroupId: NotRequired[str],
    Rules: NotRequired[Sequence[AwsWafRegionalRuleGroupRulesDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsWafRegionalRuleGroupRulesDetailsTypeDef](./type_defs.md#awswafregionalrulegrouprulesdetailstypedef) 
## AwsWafRegionalWebAclDetailsTypeDef

```python
# AwsWafRegionalWebAclDetailsTypeDef definition

class AwsWafRegionalWebAclDetailsTypeDef(TypedDict):
    DefaultAction: NotRequired[str],
    MetricName: NotRequired[str],
    Name: NotRequired[str],
    RulesList: NotRequired[Sequence[AwsWafRegionalWebAclRulesListDetailsTypeDef]],  # (1)
    WebAclId: NotRequired[str],
```

1. See [:material-code-braces: AwsWafRegionalWebAclRulesListDetailsTypeDef](./type_defs.md#awswafregionalwebaclruleslistdetailstypedef) 
## AwsWafRuleGroupDetailsTypeDef

```python
# AwsWafRuleGroupDetailsTypeDef definition

class AwsWafRuleGroupDetailsTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Name: NotRequired[str],
    RuleGroupId: NotRequired[str],
    Rules: NotRequired[Sequence[AwsWafRuleGroupRulesDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsWafRuleGroupRulesDetailsTypeDef](./type_defs.md#awswafrulegrouprulesdetailstypedef) 
## AwsWafWebAclDetailsTypeDef

```python
# AwsWafWebAclDetailsTypeDef definition

class AwsWafWebAclDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    DefaultAction: NotRequired[str],
    Rules: NotRequired[Sequence[AwsWafWebAclRuleTypeDef]],  # (1)
    WebAclId: NotRequired[str],
```

1. See [:material-code-braces: AwsWafWebAclRuleTypeDef](./type_defs.md#awswafwebaclruletypedef) 
## AwsWafv2ActionAllowDetailsTypeDef

```python
# AwsWafv2ActionAllowDetailsTypeDef definition

class AwsWafv2ActionAllowDetailsTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[AwsWafv2CustomRequestHandlingDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsWafv2CustomRequestHandlingDetailsTypeDef](./type_defs.md#awswafv2customrequesthandlingdetailstypedef) 
## AwsWafv2RulesActionCaptchaDetailsTypeDef

```python
# AwsWafv2RulesActionCaptchaDetailsTypeDef definition

class AwsWafv2RulesActionCaptchaDetailsTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[AwsWafv2CustomRequestHandlingDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsWafv2CustomRequestHandlingDetailsTypeDef](./type_defs.md#awswafv2customrequesthandlingdetailstypedef) 
## AwsWafv2RulesActionCountDetailsTypeDef

```python
# AwsWafv2RulesActionCountDetailsTypeDef definition

class AwsWafv2RulesActionCountDetailsTypeDef(TypedDict):
    CustomRequestHandling: NotRequired[AwsWafv2CustomRequestHandlingDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsWafv2CustomRequestHandlingDetailsTypeDef](./type_defs.md#awswafv2customrequesthandlingdetailstypedef) 
## AwsWafv2ActionBlockDetailsTypeDef

```python
# AwsWafv2ActionBlockDetailsTypeDef definition

class AwsWafv2ActionBlockDetailsTypeDef(TypedDict):
    CustomResponse: NotRequired[AwsWafv2CustomResponseDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsWafv2CustomResponseDetailsTypeDef](./type_defs.md#awswafv2customresponsedetailstypedef) 
## BatchGetStandardsControlAssociationsResponseTypeDef

```python
# BatchGetStandardsControlAssociationsResponseTypeDef definition

class BatchGetStandardsControlAssociationsResponseTypeDef(TypedDict):
    StandardsControlAssociationDetails: List[StandardsControlAssociationDetailTypeDef],  # (1)
    UnprocessedAssociations: List[UnprocessedStandardsControlAssociationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: StandardsControlAssociationDetailTypeDef](./type_defs.md#standardscontrolassociationdetailtypedef) 
2. See [:material-code-braces: UnprocessedStandardsControlAssociationTypeDef](./type_defs.md#unprocessedstandardscontrolassociationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateStandardsControlAssociationsResponseTypeDef

```python
# BatchUpdateStandardsControlAssociationsResponseTypeDef definition

class BatchUpdateStandardsControlAssociationsResponseTypeDef(TypedDict):
    UnprocessedAssociationUpdates: List[UnprocessedStandardsControlAssociationUpdateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedStandardsControlAssociationUpdateTypeDef](./type_defs.md#unprocessedstandardscontrolassociationupdatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutomationRulesFindingFiltersTypeDef

```python
# AutomationRulesFindingFiltersTypeDef definition

class AutomationRulesFindingFiltersTypeDef(TypedDict):
    ProductArn: NotRequired[List[StringFilterTypeDef]],  # (1)
    AwsAccountId: NotRequired[List[StringFilterTypeDef]],  # (1)
    Id: NotRequired[List[StringFilterTypeDef]],  # (1)
    GeneratorId: NotRequired[List[StringFilterTypeDef]],  # (1)
    Type: NotRequired[List[StringFilterTypeDef]],  # (1)
    FirstObservedAt: NotRequired[List[DateFilterTypeDef]],  # (6)
    LastObservedAt: NotRequired[List[DateFilterTypeDef]],  # (6)
    CreatedAt: NotRequired[List[DateFilterTypeDef]],  # (6)
    UpdatedAt: NotRequired[List[DateFilterTypeDef]],  # (6)
    Confidence: NotRequired[List[NumberFilterTypeDef]],  # (10)
    Criticality: NotRequired[List[NumberFilterTypeDef]],  # (10)
    Title: NotRequired[List[StringFilterTypeDef]],  # (1)
    Description: NotRequired[List[StringFilterTypeDef]],  # (1)
    SourceUrl: NotRequired[List[StringFilterTypeDef]],  # (1)
    ProductName: NotRequired[List[StringFilterTypeDef]],  # (1)
    CompanyName: NotRequired[List[StringFilterTypeDef]],  # (1)
    SeverityLabel: NotRequired[List[StringFilterTypeDef]],  # (1)
    ResourceType: NotRequired[List[StringFilterTypeDef]],  # (1)
    ResourceId: NotRequired[List[StringFilterTypeDef]],  # (1)
    ResourcePartition: NotRequired[List[StringFilterTypeDef]],  # (1)
    ResourceRegion: NotRequired[List[StringFilterTypeDef]],  # (1)
    ResourceTags: NotRequired[List[MapFilterTypeDef]],  # (22)
    ResourceDetailsOther: NotRequired[List[MapFilterTypeDef]],  # (22)
    ComplianceStatus: NotRequired[List[StringFilterTypeDef]],  # (1)
    ComplianceSecurityControlId: NotRequired[List[StringFilterTypeDef]],  # (1)
    ComplianceAssociatedStandardsId: NotRequired[List[StringFilterTypeDef]],  # (1)
    VerificationState: NotRequired[List[StringFilterTypeDef]],  # (1)
    WorkflowStatus: NotRequired[List[StringFilterTypeDef]],  # (1)
    RecordState: NotRequired[List[StringFilterTypeDef]],  # (1)
    RelatedFindingsProductArn: NotRequired[List[StringFilterTypeDef]],  # (1)
    RelatedFindingsId: NotRequired[List[StringFilterTypeDef]],  # (1)
    NoteText: NotRequired[List[StringFilterTypeDef]],  # (1)
    NoteUpdatedAt: NotRequired[List[DateFilterTypeDef]],  # (6)
    NoteUpdatedBy: NotRequired[List[StringFilterTypeDef]],  # (1)
    UserDefinedFields: NotRequired[List[MapFilterTypeDef]],  # (22)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
6. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
7. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
8. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
9. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
10. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
11. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
12. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
13. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
14. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
15. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
16. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
17. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
18. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
19. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
20. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
21. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
22. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
23. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
24. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
25. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
26. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
27. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
28. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
29. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
30. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
31. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
32. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
33. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
34. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
35. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
## AwsSecurityFindingFiltersTypeDef

```python
# AwsSecurityFindingFiltersTypeDef definition

class AwsSecurityFindingFiltersTypeDef(TypedDict):
    ProductArn: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    AwsAccountId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    Id: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    GeneratorId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    Region: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    Type: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    FirstObservedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (7)
    LastObservedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (7)
    CreatedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (7)
    UpdatedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (7)
    SeverityProduct: NotRequired[Sequence[NumberFilterTypeDef]],  # (11)
    SeverityNormalized: NotRequired[Sequence[NumberFilterTypeDef]],  # (11)
    SeverityLabel: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    Confidence: NotRequired[Sequence[NumberFilterTypeDef]],  # (11)
    Criticality: NotRequired[Sequence[NumberFilterTypeDef]],  # (11)
    Title: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    Description: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    RecommendationText: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    SourceUrl: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ProductFields: NotRequired[Sequence[MapFilterTypeDef]],  # (20)
    ProductName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    CompanyName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    UserDefinedFields: NotRequired[Sequence[MapFilterTypeDef]],  # (20)
    MalwareName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    MalwareType: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    MalwarePath: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    MalwareState: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    NetworkDirection: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    NetworkProtocol: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    NetworkSourceIpV4: NotRequired[Sequence[IpFilterTypeDef]],  # (30)
    NetworkSourceIpV6: NotRequired[Sequence[IpFilterTypeDef]],  # (30)
    NetworkSourcePort: NotRequired[Sequence[NumberFilterTypeDef]],  # (11)
    NetworkSourceDomain: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    NetworkSourceMac: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    NetworkDestinationIpV4: NotRequired[Sequence[IpFilterTypeDef]],  # (30)
    NetworkDestinationIpV6: NotRequired[Sequence[IpFilterTypeDef]],  # (30)
    NetworkDestinationPort: NotRequired[Sequence[NumberFilterTypeDef]],  # (11)
    NetworkDestinationDomain: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ProcessName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ProcessPath: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ProcessPid: NotRequired[Sequence[NumberFilterTypeDef]],  # (11)
    ProcessParentPid: NotRequired[Sequence[NumberFilterTypeDef]],  # (11)
    ProcessLaunchedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (7)
    ProcessTerminatedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (7)
    ThreatIntelIndicatorType: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ThreatIntelIndicatorValue: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ThreatIntelIndicatorCategory: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ThreatIntelIndicatorLastObservedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (7)
    ThreatIntelIndicatorSource: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ThreatIntelIndicatorSourceUrl: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceType: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourcePartition: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceRegion: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceTags: NotRequired[Sequence[MapFilterTypeDef]],  # (20)
    ResourceAwsEc2InstanceType: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceAwsEc2InstanceImageId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceAwsEc2InstanceIpV4Addresses: NotRequired[Sequence[IpFilterTypeDef]],  # (30)
    ResourceAwsEc2InstanceIpV6Addresses: NotRequired[Sequence[IpFilterTypeDef]],  # (30)
    ResourceAwsEc2InstanceKeyName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceAwsEc2InstanceIamInstanceProfileArn: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceAwsEc2InstanceVpcId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceAwsEc2InstanceSubnetId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceAwsEc2InstanceLaunchedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (7)
    ResourceAwsS3BucketOwnerId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceAwsS3BucketOwnerName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceAwsIamAccessKeyUserName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceAwsIamAccessKeyPrincipalName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceAwsIamAccessKeyStatus: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceAwsIamAccessKeyCreatedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (7)
    ResourceAwsIamUserUserName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceContainerName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceContainerImageId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceContainerImageName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ResourceContainerLaunchedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (7)
    ResourceDetailsOther: NotRequired[Sequence[MapFilterTypeDef]],  # (20)
    ComplianceStatus: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    VerificationState: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    WorkflowState: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    WorkflowStatus: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    RecordState: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    RelatedFindingsProductArn: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    RelatedFindingsId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    NoteText: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    NoteUpdatedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (7)
    NoteUpdatedBy: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    Keyword: NotRequired[Sequence[KeywordFilterTypeDef]],  # (87)
    FindingProviderFieldsConfidence: NotRequired[Sequence[NumberFilterTypeDef]],  # (11)
    FindingProviderFieldsCriticality: NotRequired[Sequence[NumberFilterTypeDef]],  # (11)
    FindingProviderFieldsRelatedFindingsId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    FindingProviderFieldsRelatedFindingsProductArn: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    FindingProviderFieldsSeverityLabel: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    FindingProviderFieldsSeverityOriginal: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    FindingProviderFieldsTypes: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    Sample: NotRequired[Sequence[BooleanFilterTypeDef]],  # (95)
    ComplianceSecurityControlId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ComplianceAssociatedStandardsId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
6. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
7. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
8. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
9. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
10. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
11. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
12. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
13. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
14. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
15. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
16. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
17. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
18. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
19. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
20. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
21. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
22. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
23. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
24. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
25. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
26. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
27. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
28. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
29. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
30. See [:material-code-braces: IpFilterTypeDef](./type_defs.md#ipfiltertypedef) 
31. See [:material-code-braces: IpFilterTypeDef](./type_defs.md#ipfiltertypedef) 
32. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
33. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
34. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
35. See [:material-code-braces: IpFilterTypeDef](./type_defs.md#ipfiltertypedef) 
36. See [:material-code-braces: IpFilterTypeDef](./type_defs.md#ipfiltertypedef) 
37. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
38. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
39. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
40. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
41. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
42. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
43. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
44. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
45. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
46. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
47. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
48. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
49. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
50. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
51. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
52. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
53. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
54. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
55. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
56. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
57. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
58. See [:material-code-braces: IpFilterTypeDef](./type_defs.md#ipfiltertypedef) 
59. See [:material-code-braces: IpFilterTypeDef](./type_defs.md#ipfiltertypedef) 
60. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
61. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
62. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
63. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
64. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
65. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
66. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
67. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
68. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
69. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
70. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
71. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
72. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
73. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
74. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
75. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
76. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
77. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
78. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
79. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
80. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
81. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
82. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
83. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
84. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
85. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
86. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
87. See [:material-code-braces: KeywordFilterTypeDef](./type_defs.md#keywordfiltertypedef) 
88. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
89. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
90. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
91. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
92. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
93. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
94. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
95. See [:material-code-braces: BooleanFilterTypeDef](./type_defs.md#booleanfiltertypedef) 
96. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
97. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
## GetFindingHistoryResponseTypeDef

```python
# GetFindingHistoryResponseTypeDef definition

class GetFindingHistoryResponseTypeDef(TypedDict):
    Records: List[FindingHistoryRecordTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FindingHistoryRecordTypeDef](./type_defs.md#findinghistoryrecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInsightResultsResponseTypeDef

```python
# GetInsightResultsResponseTypeDef definition

class GetInsightResultsResponseTypeDef(TypedDict):
    InsightResults: InsightResultsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InsightResultsTypeDef](./type_defs.md#insightresultstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkHeaderTypeDef

```python
# NetworkHeaderTypeDef definition

class NetworkHeaderTypeDef(TypedDict):
    Protocol: NotRequired[str],
    Destination: NotRequired[NetworkPathComponentDetailsTypeDef],  # (1)
    Source: NotRequired[NetworkPathComponentDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: NetworkPathComponentDetailsTypeDef](./type_defs.md#networkpathcomponentdetailstypedef) 
2. See [:material-code-braces: NetworkPathComponentDetailsTypeDef](./type_defs.md#networkpathcomponentdetailstypedef) 
## OccurrencesTypeDef

```python
# OccurrencesTypeDef definition

class OccurrencesTypeDef(TypedDict):
    LineRanges: NotRequired[Sequence[RangeTypeDef]],  # (1)
    OffsetRanges: NotRequired[Sequence[RangeTypeDef]],  # (1)
    Pages: NotRequired[Sequence[PageTypeDef]],  # (3)
    Records: NotRequired[Sequence[RecordTypeDef]],  # (4)
    Cells: NotRequired[Sequence[CellTypeDef]],  # (5)
```

1. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
2. See [:material-code-braces: RangeTypeDef](./type_defs.md#rangetypedef) 
3. See [:material-code-braces: PageTypeDef](./type_defs.md#pagetypedef) 
4. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
5. See [:material-code-braces: CellTypeDef](./type_defs.md#celltypedef) 
## RuleGroupSourceStatelessRuleDefinitionTypeDef

```python
# RuleGroupSourceStatelessRuleDefinitionTypeDef definition

class RuleGroupSourceStatelessRuleDefinitionTypeDef(TypedDict):
    Actions: NotRequired[Sequence[str]],
    MatchAttributes: NotRequired[RuleGroupSourceStatelessRuleMatchAttributesTypeDef],  # (1)
```

1. See [:material-code-braces: RuleGroupSourceStatelessRuleMatchAttributesTypeDef](./type_defs.md#rulegroupsourcestatelessrulematchattributestypedef) 
## DescribeStandardsResponseTypeDef

```python
# DescribeStandardsResponseTypeDef definition

class DescribeStandardsResponseTypeDef(TypedDict):
    Standards: List[StandardTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StandardTypeDef](./type_defs.md#standardtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisableStandardsResponseTypeDef

```python
# BatchDisableStandardsResponseTypeDef definition

class BatchDisableStandardsResponseTypeDef(TypedDict):
    StandardsSubscriptions: List[StandardsSubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StandardsSubscriptionTypeDef](./type_defs.md#standardssubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchEnableStandardsResponseTypeDef

```python
# BatchEnableStandardsResponseTypeDef definition

class BatchEnableStandardsResponseTypeDef(TypedDict):
    StandardsSubscriptions: List[StandardsSubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StandardsSubscriptionTypeDef](./type_defs.md#standardssubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnabledStandardsResponseTypeDef

```python
# GetEnabledStandardsResponseTypeDef definition

class GetEnabledStandardsResponseTypeDef(TypedDict):
    StandardsSubscriptions: List[StandardsSubscriptionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StandardsSubscriptionTypeDef](./type_defs.md#standardssubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StatelessCustomActionDefinitionTypeDef

```python
# StatelessCustomActionDefinitionTypeDef definition

class StatelessCustomActionDefinitionTypeDef(TypedDict):
    PublishMetricAction: NotRequired[StatelessCustomPublishMetricActionTypeDef],  # (1)
```

1. See [:material-code-braces: StatelessCustomPublishMetricActionTypeDef](./type_defs.md#statelesscustompublishmetricactiontypedef) 
## PortProbeActionTypeDef

```python
# PortProbeActionTypeDef definition

class PortProbeActionTypeDef(TypedDict):
    PortProbeDetails: NotRequired[Sequence[PortProbeDetailTypeDef]],  # (1)
    Blocked: NotRequired[bool],
```

1. See [:material-code-braces: PortProbeDetailTypeDef](./type_defs.md#portprobedetailtypedef) 
## AwsAthenaWorkGroupDetailsTypeDef

```python
# AwsAthenaWorkGroupDetailsTypeDef definition

class AwsAthenaWorkGroupDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    State: NotRequired[str],
    Configuration: NotRequired[AwsAthenaWorkGroupConfigurationDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsAthenaWorkGroupConfigurationDetailsTypeDef](./type_defs.md#awsathenaworkgroupconfigurationdetailstypedef) 
## AwsAutoScalingAutoScalingGroupDetailsTypeDef

```python
# AwsAutoScalingAutoScalingGroupDetailsTypeDef definition

class AwsAutoScalingAutoScalingGroupDetailsTypeDef(TypedDict):
    LaunchConfigurationName: NotRequired[str],
    LoadBalancerNames: NotRequired[Sequence[str]],
    HealthCheckType: NotRequired[str],
    HealthCheckGracePeriod: NotRequired[int],
    CreatedTime: NotRequired[str],
    MixedInstancesPolicy: NotRequired[AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef],  # (1)
    AvailabilityZones: NotRequired[Sequence[AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef]],  # (2)
    LaunchTemplate: NotRequired[AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef],  # (3)
    CapacityRebalance: NotRequired[bool],
```

1. See [:material-code-braces: AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef](./type_defs.md#awsautoscalingautoscalinggroupmixedinstancespolicydetailstypedef) 
2. See [:material-code-braces: AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef](./type_defs.md#awsautoscalingautoscalinggroupavailabilityzoneslistdetailstypedef) 
3. See [:material-code-braces: AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef](./type_defs.md#awsautoscalingautoscalinggrouplaunchtemplatelaunchtemplatespecificationtypedef) 
## AwsBackupBackupPlanBackupPlanDetailsTypeDef

```python
# AwsBackupBackupPlanBackupPlanDetailsTypeDef definition

class AwsBackupBackupPlanBackupPlanDetailsTypeDef(TypedDict):
    BackupPlanName: NotRequired[str],
    AdvancedBackupSettings: NotRequired[Sequence[AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef]],  # (1)
    BackupPlanRule: NotRequired[Sequence[AwsBackupBackupPlanRuleDetailsTypeDef]],  # (2)
```

1. See [:material-code-braces: AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef](./type_defs.md#awsbackupbackupplanadvancedbackupsettingsdetailstypedef) 
2. See [:material-code-braces: AwsBackupBackupPlanRuleDetailsTypeDef](./type_defs.md#awsbackupbackupplanruledetailstypedef) 
## AwsCertificateManagerCertificateDetailsTypeDef

```python
# AwsCertificateManagerCertificateDetailsTypeDef definition

class AwsCertificateManagerCertificateDetailsTypeDef(TypedDict):
    CertificateAuthorityArn: NotRequired[str],
    CreatedAt: NotRequired[str],
    DomainName: NotRequired[str],
    DomainValidationOptions: NotRequired[Sequence[AwsCertificateManagerCertificateDomainValidationOptionTypeDef]],  # (1)
    ExtendedKeyUsages: NotRequired[Sequence[AwsCertificateManagerCertificateExtendedKeyUsageTypeDef]],  # (2)
    FailureReason: NotRequired[str],
    ImportedAt: NotRequired[str],
    InUseBy: NotRequired[Sequence[str]],
    IssuedAt: NotRequired[str],
    Issuer: NotRequired[str],
    KeyAlgorithm: NotRequired[str],
    KeyUsages: NotRequired[Sequence[AwsCertificateManagerCertificateKeyUsageTypeDef]],  # (3)
    NotAfter: NotRequired[str],
    NotBefore: NotRequired[str],
    Options: NotRequired[AwsCertificateManagerCertificateOptionsTypeDef],  # (4)
    RenewalEligibility: NotRequired[str],
    RenewalSummary: NotRequired[AwsCertificateManagerCertificateRenewalSummaryTypeDef],  # (5)
    Serial: NotRequired[str],
    SignatureAlgorithm: NotRequired[str],
    Status: NotRequired[str],
    Subject: NotRequired[str],
    SubjectAlternativeNames: NotRequired[Sequence[str]],
    Type: NotRequired[str],
```

1. See [:material-code-braces: AwsCertificateManagerCertificateDomainValidationOptionTypeDef](./type_defs.md#awscertificatemanagercertificatedomainvalidationoptiontypedef) 
2. See [:material-code-braces: AwsCertificateManagerCertificateExtendedKeyUsageTypeDef](./type_defs.md#awscertificatemanagercertificateextendedkeyusagetypedef) 
3. See [:material-code-braces: AwsCertificateManagerCertificateKeyUsageTypeDef](./type_defs.md#awscertificatemanagercertificatekeyusagetypedef) 
4. See [:material-code-braces: AwsCertificateManagerCertificateOptionsTypeDef](./type_defs.md#awscertificatemanagercertificateoptionstypedef) 
5. See [:material-code-braces: AwsCertificateManagerCertificateRenewalSummaryTypeDef](./type_defs.md#awscertificatemanagercertificaterenewalsummarytypedef) 
## AwsCloudFrontDistributionOriginsTypeDef

```python
# AwsCloudFrontDistributionOriginsTypeDef definition

class AwsCloudFrontDistributionOriginsTypeDef(TypedDict):
    Items: NotRequired[Sequence[AwsCloudFrontDistributionOriginItemTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsCloudFrontDistributionOriginItemTypeDef](./type_defs.md#awscloudfrontdistributionoriginitemtypedef) 
## AwsCloudFrontDistributionOriginGroupsTypeDef

```python
# AwsCloudFrontDistributionOriginGroupsTypeDef definition

class AwsCloudFrontDistributionOriginGroupsTypeDef(TypedDict):
    Items: NotRequired[Sequence[AwsCloudFrontDistributionOriginGroupTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsCloudFrontDistributionOriginGroupTypeDef](./type_defs.md#awscloudfrontdistributionorigingrouptypedef) 
## AwsDynamoDbTableDetailsTypeDef

```python
# AwsDynamoDbTableDetailsTypeDef definition

class AwsDynamoDbTableDetailsTypeDef(TypedDict):
    AttributeDefinitions: NotRequired[Sequence[AwsDynamoDbTableAttributeDefinitionTypeDef]],  # (1)
    BillingModeSummary: NotRequired[AwsDynamoDbTableBillingModeSummaryTypeDef],  # (2)
    CreationDateTime: NotRequired[str],
    GlobalSecondaryIndexes: NotRequired[Sequence[AwsDynamoDbTableGlobalSecondaryIndexTypeDef]],  # (3)
    GlobalTableVersion: NotRequired[str],
    ItemCount: NotRequired[int],
    KeySchema: NotRequired[Sequence[AwsDynamoDbTableKeySchemaTypeDef]],  # (4)
    LatestStreamArn: NotRequired[str],
    LatestStreamLabel: NotRequired[str],
    LocalSecondaryIndexes: NotRequired[Sequence[AwsDynamoDbTableLocalSecondaryIndexTypeDef]],  # (5)
    ProvisionedThroughput: NotRequired[AwsDynamoDbTableProvisionedThroughputTypeDef],  # (6)
    Replicas: NotRequired[Sequence[AwsDynamoDbTableReplicaTypeDef]],  # (7)
    RestoreSummary: NotRequired[AwsDynamoDbTableRestoreSummaryTypeDef],  # (8)
    SseDescription: NotRequired[AwsDynamoDbTableSseDescriptionTypeDef],  # (9)
    StreamSpecification: NotRequired[AwsDynamoDbTableStreamSpecificationTypeDef],  # (10)
    TableId: NotRequired[str],
    TableName: NotRequired[str],
    TableSizeBytes: NotRequired[int],
    TableStatus: NotRequired[str],
```

1. See [:material-code-braces: AwsDynamoDbTableAttributeDefinitionTypeDef](./type_defs.md#awsdynamodbtableattributedefinitiontypedef) 
2. See [:material-code-braces: AwsDynamoDbTableBillingModeSummaryTypeDef](./type_defs.md#awsdynamodbtablebillingmodesummarytypedef) 
3. See [:material-code-braces: AwsDynamoDbTableGlobalSecondaryIndexTypeDef](./type_defs.md#awsdynamodbtableglobalsecondaryindextypedef) 
4. See [:material-code-braces: AwsDynamoDbTableKeySchemaTypeDef](./type_defs.md#awsdynamodbtablekeyschematypedef) 
5. See [:material-code-braces: AwsDynamoDbTableLocalSecondaryIndexTypeDef](./type_defs.md#awsdynamodbtablelocalsecondaryindextypedef) 
6. See [:material-code-braces: AwsDynamoDbTableProvisionedThroughputTypeDef](./type_defs.md#awsdynamodbtableprovisionedthroughputtypedef) 
7. See [:material-code-braces: AwsDynamoDbTableReplicaTypeDef](./type_defs.md#awsdynamodbtablereplicatypedef) 
8. See [:material-code-braces: AwsDynamoDbTableRestoreSummaryTypeDef](./type_defs.md#awsdynamodbtablerestoresummarytypedef) 
9. See [:material-code-braces: AwsDynamoDbTableSseDescriptionTypeDef](./type_defs.md#awsdynamodbtablessedescriptiontypedef) 
10. See [:material-code-braces: AwsDynamoDbTableStreamSpecificationTypeDef](./type_defs.md#awsdynamodbtablestreamspecificationtypedef) 
## AwsEc2LaunchTemplateDetailsTypeDef

```python
# AwsEc2LaunchTemplateDetailsTypeDef definition

class AwsEc2LaunchTemplateDetailsTypeDef(TypedDict):
    LaunchTemplateName: NotRequired[str],
    Id: NotRequired[str],
    LaunchTemplateData: NotRequired[AwsEc2LaunchTemplateDataDetailsTypeDef],  # (1)
    DefaultVersionNumber: NotRequired[int],
    LatestVersionNumber: NotRequired[int],
```

1. See [:material-code-braces: AwsEc2LaunchTemplateDataDetailsTypeDef](./type_defs.md#awsec2launchtemplatedatadetailstypedef) 
## AwsEcsClusterDetailsTypeDef

```python
# AwsEcsClusterDetailsTypeDef definition

class AwsEcsClusterDetailsTypeDef(TypedDict):
    ClusterArn: NotRequired[str],
    ActiveServicesCount: NotRequired[int],
    CapacityProviders: NotRequired[Sequence[str]],
    ClusterSettings: NotRequired[Sequence[AwsEcsClusterClusterSettingsDetailsTypeDef]],  # (1)
    Configuration: NotRequired[AwsEcsClusterConfigurationDetailsTypeDef],  # (2)
    DefaultCapacityProviderStrategy: NotRequired[Sequence[AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef]],  # (3)
    ClusterName: NotRequired[str],
    RegisteredContainerInstancesCount: NotRequired[int],
    RunningTasksCount: NotRequired[int],
    Status: NotRequired[str],
```

1. See [:material-code-braces: AwsEcsClusterClusterSettingsDetailsTypeDef](./type_defs.md#awsecsclusterclustersettingsdetailstypedef) 
2. See [:material-code-braces: AwsEcsClusterConfigurationDetailsTypeDef](./type_defs.md#awsecsclusterconfigurationdetailstypedef) 
3. See [:material-code-braces: AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef](./type_defs.md#awsecsclusterdefaultcapacityproviderstrategydetailstypedef) 
## AwsEcsTaskDefinitionDetailsTypeDef

```python
# AwsEcsTaskDefinitionDetailsTypeDef definition

class AwsEcsTaskDefinitionDetailsTypeDef(TypedDict):
    ContainerDefinitions: NotRequired[Sequence[AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef]],  # (1)
    Cpu: NotRequired[str],
    ExecutionRoleArn: NotRequired[str],
    Family: NotRequired[str],
    InferenceAccelerators: NotRequired[Sequence[AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef]],  # (2)
    IpcMode: NotRequired[str],
    Memory: NotRequired[str],
    NetworkMode: NotRequired[str],
    PidMode: NotRequired[str],
    PlacementConstraints: NotRequired[Sequence[AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef]],  # (3)
    ProxyConfiguration: NotRequired[AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef],  # (4)
    RequiresCompatibilities: NotRequired[Sequence[str]],
    TaskRoleArn: NotRequired[str],
    Volumes: NotRequired[Sequence[AwsEcsTaskDefinitionVolumesDetailsTypeDef]],  # (5)
```

1. See [:material-code-braces: AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioncontainerdefinitionsdetailstypedef) 
2. See [:material-code-braces: AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef](./type_defs.md#awsecstaskdefinitioninferenceacceleratorsdetailstypedef) 
3. See [:material-code-braces: AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef](./type_defs.md#awsecstaskdefinitionplacementconstraintsdetailstypedef) 
4. See [:material-code-braces: AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef](./type_defs.md#awsecstaskdefinitionproxyconfigurationdetailstypedef) 
5. See [:material-code-braces: AwsEcsTaskDefinitionVolumesDetailsTypeDef](./type_defs.md#awsecstaskdefinitionvolumesdetailstypedef) 
## AwsGuardDutyDetectorDataSourcesDetailsTypeDef

```python
# AwsGuardDutyDetectorDataSourcesDetailsTypeDef definition

class AwsGuardDutyDetectorDataSourcesDetailsTypeDef(TypedDict):
    CloudTrail: NotRequired[AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef],  # (1)
    DnsLogs: NotRequired[AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef],  # (2)
    FlowLogs: NotRequired[AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef],  # (3)
    Kubernetes: NotRequired[AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef],  # (4)
    MalwareProtection: NotRequired[AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef],  # (5)
    S3Logs: NotRequired[AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef],  # (6)
```

1. See [:material-code-braces: AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef](./type_defs.md#awsguarddutydetectordatasourcescloudtraildetailstypedef) 
2. See [:material-code-braces: AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef](./type_defs.md#awsguarddutydetectordatasourcesdnslogsdetailstypedef) 
3. See [:material-code-braces: AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef](./type_defs.md#awsguarddutydetectordatasourcesflowlogsdetailstypedef) 
4. See [:material-code-braces: AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef](./type_defs.md#awsguarddutydetectordatasourceskubernetesdetailstypedef) 
5. See [:material-code-braces: AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef](./type_defs.md#awsguarddutydetectordatasourcesmalwareprotectiondetailstypedef) 
6. See [:material-code-braces: AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef](./type_defs.md#awsguarddutydetectordatasourcess3logsdetailstypedef) 
## AwsRdsDbInstanceDetailsTypeDef

```python
# AwsRdsDbInstanceDetailsTypeDef definition

class AwsRdsDbInstanceDetailsTypeDef(TypedDict):
    AssociatedRoles: NotRequired[Sequence[AwsRdsDbInstanceAssociatedRoleTypeDef]],  # (1)
    CACertificateIdentifier: NotRequired[str],
    DBClusterIdentifier: NotRequired[str],
    DBInstanceIdentifier: NotRequired[str],
    DBInstanceClass: NotRequired[str],
    DbInstancePort: NotRequired[int],
    DbiResourceId: NotRequired[str],
    DBName: NotRequired[str],
    DeletionProtection: NotRequired[bool],
    Endpoint: NotRequired[AwsRdsDbInstanceEndpointTypeDef],  # (2)
    Engine: NotRequired[str],
    EngineVersion: NotRequired[str],
    IAMDatabaseAuthenticationEnabled: NotRequired[bool],
    InstanceCreateTime: NotRequired[str],
    KmsKeyId: NotRequired[str],
    PubliclyAccessible: NotRequired[bool],
    StorageEncrypted: NotRequired[bool],
    TdeCredentialArn: NotRequired[str],
    VpcSecurityGroups: NotRequired[Sequence[AwsRdsDbInstanceVpcSecurityGroupTypeDef]],  # (3)
    MultiAz: NotRequired[bool],
    EnhancedMonitoringResourceArn: NotRequired[str],
    DbInstanceStatus: NotRequired[str],
    MasterUsername: NotRequired[str],
    AllocatedStorage: NotRequired[int],
    PreferredBackupWindow: NotRequired[str],
    BackupRetentionPeriod: NotRequired[int],
    DbSecurityGroups: NotRequired[Sequence[str]],
    DbParameterGroups: NotRequired[Sequence[AwsRdsDbParameterGroupTypeDef]],  # (4)
    AvailabilityZone: NotRequired[str],
    DbSubnetGroup: NotRequired[AwsRdsDbSubnetGroupTypeDef],  # (5)
    PreferredMaintenanceWindow: NotRequired[str],
    PendingModifiedValues: NotRequired[AwsRdsDbPendingModifiedValuesTypeDef],  # (6)
    LatestRestorableTime: NotRequired[str],
    AutoMinorVersionUpgrade: NotRequired[bool],
    ReadReplicaSourceDBInstanceIdentifier: NotRequired[str],
    ReadReplicaDBInstanceIdentifiers: NotRequired[Sequence[str]],
    ReadReplicaDBClusterIdentifiers: NotRequired[Sequence[str]],
    LicenseModel: NotRequired[str],
    Iops: NotRequired[int],
    OptionGroupMemberships: NotRequired[Sequence[AwsRdsDbOptionGroupMembershipTypeDef]],  # (7)
    CharacterSetName: NotRequired[str],
    SecondaryAvailabilityZone: NotRequired[str],
    StatusInfos: NotRequired[Sequence[AwsRdsDbStatusInfoTypeDef]],  # (8)
    StorageType: NotRequired[str],
    DomainMemberships: NotRequired[Sequence[AwsRdsDbDomainMembershipTypeDef]],  # (9)
    CopyTagsToSnapshot: NotRequired[bool],
    MonitoringInterval: NotRequired[int],
    MonitoringRoleArn: NotRequired[str],
    PromotionTier: NotRequired[int],
    Timezone: NotRequired[str],
    PerformanceInsightsEnabled: NotRequired[bool],
    PerformanceInsightsKmsKeyId: NotRequired[str],
    PerformanceInsightsRetentionPeriod: NotRequired[int],
    EnabledCloudWatchLogsExports: NotRequired[Sequence[str]],
    ProcessorFeatures: NotRequired[Sequence[AwsRdsDbProcessorFeatureTypeDef]],  # (10)
    ListenerEndpoint: NotRequired[AwsRdsDbInstanceEndpointTypeDef],  # (2)
    MaxAllocatedStorage: NotRequired[int],
```

1. See [:material-code-braces: AwsRdsDbInstanceAssociatedRoleTypeDef](./type_defs.md#awsrdsdbinstanceassociatedroletypedef) 
2. See [:material-code-braces: AwsRdsDbInstanceEndpointTypeDef](./type_defs.md#awsrdsdbinstanceendpointtypedef) 
3. See [:material-code-braces: AwsRdsDbInstanceVpcSecurityGroupTypeDef](./type_defs.md#awsrdsdbinstancevpcsecuritygrouptypedef) 
4. See [:material-code-braces: AwsRdsDbParameterGroupTypeDef](./type_defs.md#awsrdsdbparametergrouptypedef) 
5. See [:material-code-braces: AwsRdsDbSubnetGroupTypeDef](./type_defs.md#awsrdsdbsubnetgrouptypedef) 
6. See [:material-code-braces: AwsRdsDbPendingModifiedValuesTypeDef](./type_defs.md#awsrdsdbpendingmodifiedvaluestypedef) 
7. See [:material-code-braces: AwsRdsDbOptionGroupMembershipTypeDef](./type_defs.md#awsrdsdboptiongroupmembershiptypedef) 
8. See [:material-code-braces: AwsRdsDbStatusInfoTypeDef](./type_defs.md#awsrdsdbstatusinfotypedef) 
9. See [:material-code-braces: AwsRdsDbDomainMembershipTypeDef](./type_defs.md#awsrdsdbdomainmembershiptypedef) 
10. See [:material-code-braces: AwsRdsDbProcessorFeatureTypeDef](./type_defs.md#awsrdsdbprocessorfeaturetypedef) 
11. See [:material-code-braces: AwsRdsDbInstanceEndpointTypeDef](./type_defs.md#awsrdsdbinstanceendpointtypedef) 
## AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef

```python
# AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef definition

class AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef(TypedDict):
    Predicate: NotRequired[AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef](./type_defs.md#awss3bucketbucketlifecycleconfigurationrulesfilterpredicatedetailstypedef) 
## AwsS3BucketNotificationConfigurationDetailTypeDef

```python
# AwsS3BucketNotificationConfigurationDetailTypeDef definition

class AwsS3BucketNotificationConfigurationDetailTypeDef(TypedDict):
    Events: NotRequired[Sequence[str]],
    Filter: NotRequired[AwsS3BucketNotificationConfigurationFilterTypeDef],  # (1)
    Destination: NotRequired[str],
    Type: NotRequired[str],
```

1. See [:material-code-braces: AwsS3BucketNotificationConfigurationFilterTypeDef](./type_defs.md#awss3bucketnotificationconfigurationfiltertypedef) 
## AwsStepFunctionStateMachineDetailsTypeDef

```python
# AwsStepFunctionStateMachineDetailsTypeDef definition

class AwsStepFunctionStateMachineDetailsTypeDef(TypedDict):
    Label: NotRequired[str],
    LoggingConfiguration: NotRequired[AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef],  # (1)
    Name: NotRequired[str],
    RoleArn: NotRequired[str],
    StateMachineArn: NotRequired[str],
    Status: NotRequired[str],
    TracingConfiguration: NotRequired[AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef],  # (2)
    Type: NotRequired[str],
```

1. See [:material-code-braces: AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef](./type_defs.md#awsstepfunctionstatemachineloggingconfigurationdetailstypedef) 
2. See [:material-code-braces: AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef](./type_defs.md#awsstepfunctionstatemachinetracingconfigurationdetailstypedef) 
## AwsWafv2RulesActionDetailsTypeDef

```python
# AwsWafv2RulesActionDetailsTypeDef definition

class AwsWafv2RulesActionDetailsTypeDef(TypedDict):
    Allow: NotRequired[AwsWafv2ActionAllowDetailsTypeDef],  # (1)
    Block: NotRequired[AwsWafv2ActionBlockDetailsTypeDef],  # (2)
    Captcha: NotRequired[AwsWafv2RulesActionCaptchaDetailsTypeDef],  # (3)
    Count: NotRequired[AwsWafv2RulesActionCountDetailsTypeDef],  # (4)
```

1. See [:material-code-braces: AwsWafv2ActionAllowDetailsTypeDef](./type_defs.md#awswafv2actionallowdetailstypedef) 
2. See [:material-code-braces: AwsWafv2ActionBlockDetailsTypeDef](./type_defs.md#awswafv2actionblockdetailstypedef) 
3. See [:material-code-braces: AwsWafv2RulesActionCaptchaDetailsTypeDef](./type_defs.md#awswafv2rulesactioncaptchadetailstypedef) 
4. See [:material-code-braces: AwsWafv2RulesActionCountDetailsTypeDef](./type_defs.md#awswafv2rulesactioncountdetailstypedef) 
## AwsWafv2WebAclActionDetailsTypeDef

```python
# AwsWafv2WebAclActionDetailsTypeDef definition

class AwsWafv2WebAclActionDetailsTypeDef(TypedDict):
    Allow: NotRequired[AwsWafv2ActionAllowDetailsTypeDef],  # (1)
    Block: NotRequired[AwsWafv2ActionBlockDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: AwsWafv2ActionAllowDetailsTypeDef](./type_defs.md#awswafv2actionallowdetailstypedef) 
2. See [:material-code-braces: AwsWafv2ActionBlockDetailsTypeDef](./type_defs.md#awswafv2actionblockdetailstypedef) 
## AutomationRulesConfigTypeDef

```python
# AutomationRulesConfigTypeDef definition

class AutomationRulesConfigTypeDef(TypedDict):
    RuleArn: NotRequired[str],
    RuleStatus: NotRequired[RuleStatusType],  # (1)
    RuleOrder: NotRequired[int],
    RuleName: NotRequired[str],
    Description: NotRequired[str],
    IsTerminal: NotRequired[bool],
    Criteria: NotRequired[AutomationRulesFindingFiltersTypeDef],  # (2)
    Actions: NotRequired[List[AutomationRulesActionTypeDef]],  # (3)
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
    CreatedBy: NotRequired[str],
```

1. See [:material-code-brackets: RuleStatusType](./literals.md#rulestatustype) 
2. See [:material-code-braces: AutomationRulesFindingFiltersTypeDef](./type_defs.md#automationrulesfindingfilterstypedef) 
3. See [:material-code-braces: AutomationRulesActionTypeDef](./type_defs.md#automationrulesactiontypedef) 
## CreateAutomationRuleRequestRequestTypeDef

```python
# CreateAutomationRuleRequestRequestTypeDef definition

class CreateAutomationRuleRequestRequestTypeDef(TypedDict):
    RuleOrder: int,
    RuleName: str,
    Description: str,
    Criteria: AutomationRulesFindingFiltersTypeDef,  # (1)
    Actions: Sequence[AutomationRulesActionTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
    RuleStatus: NotRequired[RuleStatusType],  # (3)
    IsTerminal: NotRequired[bool],
```

1. See [:material-code-braces: AutomationRulesFindingFiltersTypeDef](./type_defs.md#automationrulesfindingfilterstypedef) 
2. See [:material-code-braces: AutomationRulesActionTypeDef](./type_defs.md#automationrulesactiontypedef) 
3. See [:material-code-brackets: RuleStatusType](./literals.md#rulestatustype) 
## UpdateAutomationRulesRequestItemTypeDef

```python
# UpdateAutomationRulesRequestItemTypeDef definition

class UpdateAutomationRulesRequestItemTypeDef(TypedDict):
    RuleArn: str,
    RuleStatus: NotRequired[RuleStatusType],  # (1)
    RuleOrder: NotRequired[int],
    Description: NotRequired[str],
    RuleName: NotRequired[str],
    IsTerminal: NotRequired[bool],
    Criteria: NotRequired[AutomationRulesFindingFiltersTypeDef],  # (2)
    Actions: NotRequired[Sequence[AutomationRulesActionTypeDef]],  # (3)
```

1. See [:material-code-brackets: RuleStatusType](./literals.md#rulestatustype) 
2. See [:material-code-braces: AutomationRulesFindingFiltersTypeDef](./type_defs.md#automationrulesfindingfilterstypedef) 
3. See [:material-code-braces: AutomationRulesActionTypeDef](./type_defs.md#automationrulesactiontypedef) 
## CreateInsightRequestRequestTypeDef

```python
# CreateInsightRequestRequestTypeDef definition

class CreateInsightRequestRequestTypeDef(TypedDict):
    Name: str,
    Filters: AwsSecurityFindingFiltersTypeDef,  # (1)
    GroupByAttribute: str,
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) 
## GetFindingsRequestGetFindingsPaginateTypeDef

```python
# GetFindingsRequestGetFindingsPaginateTypeDef definition

class GetFindingsRequestGetFindingsPaginateTypeDef(TypedDict):
    Filters: NotRequired[AwsSecurityFindingFiltersTypeDef],  # (1)
    SortCriteria: NotRequired[Sequence[SortCriterionTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) 
2. See [:material-code-braces: SortCriterionTypeDef](./type_defs.md#sortcriteriontypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetFindingsRequestRequestTypeDef

```python
# GetFindingsRequestRequestTypeDef definition

class GetFindingsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[AwsSecurityFindingFiltersTypeDef],  # (1)
    SortCriteria: NotRequired[Sequence[SortCriterionTypeDef]],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) 
2. See [:material-code-braces: SortCriterionTypeDef](./type_defs.md#sortcriteriontypedef) 
## InsightTypeDef

```python
# InsightTypeDef definition

class InsightTypeDef(TypedDict):
    InsightArn: str,
    Name: str,
    Filters: AwsSecurityFindingFiltersTypeDef,  # (1)
    GroupByAttribute: str,
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) 
## UpdateFindingsRequestRequestTypeDef

```python
# UpdateFindingsRequestRequestTypeDef definition

class UpdateFindingsRequestRequestTypeDef(TypedDict):
    Filters: AwsSecurityFindingFiltersTypeDef,  # (1)
    Note: NotRequired[NoteUpdateTypeDef],  # (2)
    RecordState: NotRequired[RecordStateType],  # (3)
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) 
2. See [:material-code-braces: NoteUpdateTypeDef](./type_defs.md#noteupdatetypedef) 
3. See [:material-code-brackets: RecordStateType](./literals.md#recordstatetype) 
## UpdateInsightRequestRequestTypeDef

```python
# UpdateInsightRequestRequestTypeDef definition

class UpdateInsightRequestRequestTypeDef(TypedDict):
    InsightArn: str,
    Name: NotRequired[str],
    Filters: NotRequired[AwsSecurityFindingFiltersTypeDef],  # (1)
    GroupByAttribute: NotRequired[str],
```

1. See [:material-code-braces: AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef) 
## NetworkPathComponentTypeDef

```python
# NetworkPathComponentTypeDef definition

class NetworkPathComponentTypeDef(TypedDict):
    ComponentId: NotRequired[str],
    ComponentType: NotRequired[str],
    Egress: NotRequired[NetworkHeaderTypeDef],  # (1)
    Ingress: NotRequired[NetworkHeaderTypeDef],  # (1)
```

1. See [:material-code-braces: NetworkHeaderTypeDef](./type_defs.md#networkheadertypedef) 
2. See [:material-code-braces: NetworkHeaderTypeDef](./type_defs.md#networkheadertypedef) 
## CustomDataIdentifiersDetectionsTypeDef

```python
# CustomDataIdentifiersDetectionsTypeDef definition

class CustomDataIdentifiersDetectionsTypeDef(TypedDict):
    Count: NotRequired[int],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    Occurrences: NotRequired[OccurrencesTypeDef],  # (1)
```

1. See [:material-code-braces: OccurrencesTypeDef](./type_defs.md#occurrencestypedef) 
## SensitiveDataDetectionsTypeDef

```python
# SensitiveDataDetectionsTypeDef definition

class SensitiveDataDetectionsTypeDef(TypedDict):
    Count: NotRequired[int],
    Type: NotRequired[str],
    Occurrences: NotRequired[OccurrencesTypeDef],  # (1)
```

1. See [:material-code-braces: OccurrencesTypeDef](./type_defs.md#occurrencestypedef) 
## RuleGroupSourceStatelessRulesDetailsTypeDef

```python
# RuleGroupSourceStatelessRulesDetailsTypeDef definition

class RuleGroupSourceStatelessRulesDetailsTypeDef(TypedDict):
    Priority: NotRequired[int],
    RuleDefinition: NotRequired[RuleGroupSourceStatelessRuleDefinitionTypeDef],  # (1)
```

1. See [:material-code-braces: RuleGroupSourceStatelessRuleDefinitionTypeDef](./type_defs.md#rulegroupsourcestatelessruledefinitiontypedef) 
## FirewallPolicyStatelessCustomActionsDetailsTypeDef

```python
# FirewallPolicyStatelessCustomActionsDetailsTypeDef definition

class FirewallPolicyStatelessCustomActionsDetailsTypeDef(TypedDict):
    ActionDefinition: NotRequired[StatelessCustomActionDefinitionTypeDef],  # (1)
    ActionName: NotRequired[str],
```

1. See [:material-code-braces: StatelessCustomActionDefinitionTypeDef](./type_defs.md#statelesscustomactiondefinitiontypedef) 
## RuleGroupSourceCustomActionsDetailsTypeDef

```python
# RuleGroupSourceCustomActionsDetailsTypeDef definition

class RuleGroupSourceCustomActionsDetailsTypeDef(TypedDict):
    ActionDefinition: NotRequired[StatelessCustomActionDefinitionTypeDef],  # (1)
    ActionName: NotRequired[str],
```

1. See [:material-code-braces: StatelessCustomActionDefinitionTypeDef](./type_defs.md#statelesscustomactiondefinitiontypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    ActionType: NotRequired[str],
    NetworkConnectionAction: NotRequired[NetworkConnectionActionTypeDef],  # (1)
    AwsApiCallAction: NotRequired[AwsApiCallActionTypeDef],  # (2)
    DnsRequestAction: NotRequired[DnsRequestActionTypeDef],  # (3)
    PortProbeAction: NotRequired[PortProbeActionTypeDef],  # (4)
```

1. See [:material-code-braces: NetworkConnectionActionTypeDef](./type_defs.md#networkconnectionactiontypedef) 
2. See [:material-code-braces: AwsApiCallActionTypeDef](./type_defs.md#awsapicallactiontypedef) 
3. See [:material-code-braces: DnsRequestActionTypeDef](./type_defs.md#dnsrequestactiontypedef) 
4. See [:material-code-braces: PortProbeActionTypeDef](./type_defs.md#portprobeactiontypedef) 
## AwsBackupBackupPlanDetailsTypeDef

```python
# AwsBackupBackupPlanDetailsTypeDef definition

class AwsBackupBackupPlanDetailsTypeDef(TypedDict):
    BackupPlan: NotRequired[AwsBackupBackupPlanBackupPlanDetailsTypeDef],  # (1)
    BackupPlanArn: NotRequired[str],
    BackupPlanId: NotRequired[str],
    VersionId: NotRequired[str],
```

1. See [:material-code-braces: AwsBackupBackupPlanBackupPlanDetailsTypeDef](./type_defs.md#awsbackupbackupplanbackupplandetailstypedef) 
## AwsCloudFrontDistributionDetailsTypeDef

```python
# AwsCloudFrontDistributionDetailsTypeDef definition

class AwsCloudFrontDistributionDetailsTypeDef(TypedDict):
    CacheBehaviors: NotRequired[AwsCloudFrontDistributionCacheBehaviorsTypeDef],  # (1)
    DefaultCacheBehavior: NotRequired[AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef],  # (2)
    DefaultRootObject: NotRequired[str],
    DomainName: NotRequired[str],
    ETag: NotRequired[str],
    LastModifiedTime: NotRequired[str],
    Logging: NotRequired[AwsCloudFrontDistributionLoggingTypeDef],  # (3)
    Origins: NotRequired[AwsCloudFrontDistributionOriginsTypeDef],  # (4)
    OriginGroups: NotRequired[AwsCloudFrontDistributionOriginGroupsTypeDef],  # (5)
    ViewerCertificate: NotRequired[AwsCloudFrontDistributionViewerCertificateTypeDef],  # (6)
    Status: NotRequired[str],
    WebAclId: NotRequired[str],
```

1. See [:material-code-braces: AwsCloudFrontDistributionCacheBehaviorsTypeDef](./type_defs.md#awscloudfrontdistributioncachebehaviorstypedef) 
2. See [:material-code-braces: AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef](./type_defs.md#awscloudfrontdistributiondefaultcachebehaviortypedef) 
3. See [:material-code-braces: AwsCloudFrontDistributionLoggingTypeDef](./type_defs.md#awscloudfrontdistributionloggingtypedef) 
4. See [:material-code-braces: AwsCloudFrontDistributionOriginsTypeDef](./type_defs.md#awscloudfrontdistributionoriginstypedef) 
5. See [:material-code-braces: AwsCloudFrontDistributionOriginGroupsTypeDef](./type_defs.md#awscloudfrontdistributionorigingroupstypedef) 
6. See [:material-code-braces: AwsCloudFrontDistributionViewerCertificateTypeDef](./type_defs.md#awscloudfrontdistributionviewercertificatetypedef) 
## AwsGuardDutyDetectorDetailsTypeDef

```python
# AwsGuardDutyDetectorDetailsTypeDef definition

class AwsGuardDutyDetectorDetailsTypeDef(TypedDict):
    DataSources: NotRequired[AwsGuardDutyDetectorDataSourcesDetailsTypeDef],  # (1)
    Features: NotRequired[Sequence[AwsGuardDutyDetectorFeaturesDetailsTypeDef]],  # (2)
    FindingPublishingFrequency: NotRequired[str],
    ServiceRole: NotRequired[str],
    Status: NotRequired[str],
```

1. See [:material-code-braces: AwsGuardDutyDetectorDataSourcesDetailsTypeDef](./type_defs.md#awsguarddutydetectordatasourcesdetailstypedef) 
2. See [:material-code-braces: AwsGuardDutyDetectorFeaturesDetailsTypeDef](./type_defs.md#awsguarddutydetectorfeaturesdetailstypedef) 
## AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef

```python
# AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef definition

class AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef(TypedDict):
    AbortIncompleteMultipartUpload: NotRequired[AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef],  # (1)
    ExpirationDate: NotRequired[str],
    ExpirationInDays: NotRequired[int],
    ExpiredObjectDeleteMarker: NotRequired[bool],
    Filter: NotRequired[AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef],  # (2)
    ID: NotRequired[str],
    NoncurrentVersionExpirationInDays: NotRequired[int],
    NoncurrentVersionTransitions: NotRequired[Sequence[AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef]],  # (3)
    Prefix: NotRequired[str],
    Status: NotRequired[str],
    Transitions: NotRequired[Sequence[AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef]],  # (4)
```

1. See [:material-code-braces: AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef](./type_defs.md#awss3bucketbucketlifecycleconfigurationrulesabortincompletemultipartuploaddetailstypedef) 
2. See [:material-code-braces: AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef](./type_defs.md#awss3bucketbucketlifecycleconfigurationrulesfilterdetailstypedef) 
3. See [:material-code-braces: AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef](./type_defs.md#awss3bucketbucketlifecycleconfigurationrulesnoncurrentversiontransitionsdetailstypedef) 
4. See [:material-code-braces: AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef](./type_defs.md#awss3bucketbucketlifecycleconfigurationrulestransitionsdetailstypedef) 
## AwsS3BucketNotificationConfigurationTypeDef

```python
# AwsS3BucketNotificationConfigurationTypeDef definition

class AwsS3BucketNotificationConfigurationTypeDef(TypedDict):
    Configurations: NotRequired[Sequence[AwsS3BucketNotificationConfigurationDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsS3BucketNotificationConfigurationDetailTypeDef](./type_defs.md#awss3bucketnotificationconfigurationdetailtypedef) 
## AwsWafv2RulesDetailsTypeDef

```python
# AwsWafv2RulesDetailsTypeDef definition

class AwsWafv2RulesDetailsTypeDef(TypedDict):
    Action: NotRequired[AwsWafv2RulesActionDetailsTypeDef],  # (1)
    Name: NotRequired[str],
    OverrideAction: NotRequired[str],
    Priority: NotRequired[int],
    VisibilityConfig: NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: AwsWafv2RulesActionDetailsTypeDef](./type_defs.md#awswafv2rulesactiondetailstypedef) 
2. See [:material-code-braces: AwsWafv2VisibilityConfigDetailsTypeDef](./type_defs.md#awswafv2visibilityconfigdetailstypedef) 
## BatchGetAutomationRulesResponseTypeDef

```python
# BatchGetAutomationRulesResponseTypeDef definition

class BatchGetAutomationRulesResponseTypeDef(TypedDict):
    Rules: List[AutomationRulesConfigTypeDef],  # (1)
    UnprocessedAutomationRules: List[UnprocessedAutomationRuleTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AutomationRulesConfigTypeDef](./type_defs.md#automationrulesconfigtypedef) 
2. See [:material-code-braces: UnprocessedAutomationRuleTypeDef](./type_defs.md#unprocessedautomationruletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateAutomationRulesRequestRequestTypeDef

```python
# BatchUpdateAutomationRulesRequestRequestTypeDef definition

class BatchUpdateAutomationRulesRequestRequestTypeDef(TypedDict):
    UpdateAutomationRulesRequestItems: Sequence[UpdateAutomationRulesRequestItemTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateAutomationRulesRequestItemTypeDef](./type_defs.md#updateautomationrulesrequestitemtypedef) 
## GetInsightsResponseTypeDef

```python
# GetInsightsResponseTypeDef definition

class GetInsightsResponseTypeDef(TypedDict):
    Insights: List[InsightTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InsightTypeDef](./type_defs.md#insighttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomDataIdentifiersResultTypeDef

```python
# CustomDataIdentifiersResultTypeDef definition

class CustomDataIdentifiersResultTypeDef(TypedDict):
    Detections: NotRequired[Sequence[CustomDataIdentifiersDetectionsTypeDef]],  # (1)
    TotalCount: NotRequired[int],
```

1. See [:material-code-braces: CustomDataIdentifiersDetectionsTypeDef](./type_defs.md#customdataidentifiersdetectionstypedef) 
## SensitiveDataResultTypeDef

```python
# SensitiveDataResultTypeDef definition

class SensitiveDataResultTypeDef(TypedDict):
    Category: NotRequired[str],
    Detections: NotRequired[Sequence[SensitiveDataDetectionsTypeDef]],  # (1)
    TotalCount: NotRequired[int],
```

1. See [:material-code-braces: SensitiveDataDetectionsTypeDef](./type_defs.md#sensitivedatadetectionstypedef) 
## FirewallPolicyDetailsTypeDef

```python
# FirewallPolicyDetailsTypeDef definition

class FirewallPolicyDetailsTypeDef(TypedDict):
    StatefulRuleGroupReferences: NotRequired[Sequence[FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef]],  # (1)
    StatelessCustomActions: NotRequired[Sequence[FirewallPolicyStatelessCustomActionsDetailsTypeDef]],  # (2)
    StatelessDefaultActions: NotRequired[Sequence[str]],
    StatelessFragmentDefaultActions: NotRequired[Sequence[str]],
    StatelessRuleGroupReferences: NotRequired[Sequence[FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef]],  # (3)
```

1. See [:material-code-braces: FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef](./type_defs.md#firewallpolicystatefulrulegroupreferencesdetailstypedef) 
2. See [:material-code-braces: FirewallPolicyStatelessCustomActionsDetailsTypeDef](./type_defs.md#firewallpolicystatelesscustomactionsdetailstypedef) 
3. See [:material-code-braces: FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef](./type_defs.md#firewallpolicystatelessrulegroupreferencesdetailstypedef) 
## RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef

```python
# RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef definition

class RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef(TypedDict):
    CustomActions: NotRequired[Sequence[RuleGroupSourceCustomActionsDetailsTypeDef]],  # (1)
    StatelessRules: NotRequired[Sequence[RuleGroupSourceStatelessRulesDetailsTypeDef]],  # (2)
```

1. See [:material-code-braces: RuleGroupSourceCustomActionsDetailsTypeDef](./type_defs.md#rulegroupsourcecustomactionsdetailstypedef) 
2. See [:material-code-braces: RuleGroupSourceStatelessRulesDetailsTypeDef](./type_defs.md#rulegroupsourcestatelessrulesdetailstypedef) 
## AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef

```python
# AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef definition

class AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef(TypedDict):
    Rules: NotRequired[Sequence[AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef](./type_defs.md#awss3bucketbucketlifecycleconfigurationrulesdetailstypedef) 
## AwsWafv2RuleGroupDetailsTypeDef

```python
# AwsWafv2RuleGroupDetailsTypeDef definition

class AwsWafv2RuleGroupDetailsTypeDef(TypedDict):
    Capacity: NotRequired[int],
    Description: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    Arn: NotRequired[str],
    Rules: NotRequired[Sequence[AwsWafv2RulesDetailsTypeDef]],  # (1)
    Scope: NotRequired[str],
    VisibilityConfig: NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: AwsWafv2RulesDetailsTypeDef](./type_defs.md#awswafv2rulesdetailstypedef) 
2. See [:material-code-braces: AwsWafv2VisibilityConfigDetailsTypeDef](./type_defs.md#awswafv2visibilityconfigdetailstypedef) 
## AwsWafv2WebAclDetailsTypeDef

```python
# AwsWafv2WebAclDetailsTypeDef definition

class AwsWafv2WebAclDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    ManagedbyFirewallManager: NotRequired[bool],
    Id: NotRequired[str],
    Capacity: NotRequired[int],
    CaptchaConfig: NotRequired[AwsWafv2WebAclCaptchaConfigDetailsTypeDef],  # (1)
    DefaultAction: NotRequired[AwsWafv2WebAclActionDetailsTypeDef],  # (2)
    Description: NotRequired[str],
    Rules: NotRequired[Sequence[AwsWafv2RulesDetailsTypeDef]],  # (3)
    VisibilityConfig: NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],  # (4)
```

1. See [:material-code-braces: AwsWafv2WebAclCaptchaConfigDetailsTypeDef](./type_defs.md#awswafv2webaclcaptchaconfigdetailstypedef) 
2. See [:material-code-braces: AwsWafv2WebAclActionDetailsTypeDef](./type_defs.md#awswafv2webaclactiondetailstypedef) 
3. See [:material-code-braces: AwsWafv2RulesDetailsTypeDef](./type_defs.md#awswafv2rulesdetailstypedef) 
4. See [:material-code-braces: AwsWafv2VisibilityConfigDetailsTypeDef](./type_defs.md#awswafv2visibilityconfigdetailstypedef) 
## ClassificationResultTypeDef

```python
# ClassificationResultTypeDef definition

class ClassificationResultTypeDef(TypedDict):
    MimeType: NotRequired[str],
    SizeClassified: NotRequired[int],
    AdditionalOccurrences: NotRequired[bool],
    Status: NotRequired[ClassificationStatusTypeDef],  # (1)
    SensitiveData: NotRequired[Sequence[SensitiveDataResultTypeDef]],  # (2)
    CustomDataIdentifiers: NotRequired[CustomDataIdentifiersResultTypeDef],  # (3)
```

1. See [:material-code-braces: ClassificationStatusTypeDef](./type_defs.md#classificationstatustypedef) 
2. See [:material-code-braces: SensitiveDataResultTypeDef](./type_defs.md#sensitivedataresulttypedef) 
3. See [:material-code-braces: CustomDataIdentifiersResultTypeDef](./type_defs.md#customdataidentifiersresulttypedef) 
## AwsNetworkFirewallFirewallPolicyDetailsTypeDef

```python
# AwsNetworkFirewallFirewallPolicyDetailsTypeDef definition

class AwsNetworkFirewallFirewallPolicyDetailsTypeDef(TypedDict):
    FirewallPolicy: NotRequired[FirewallPolicyDetailsTypeDef],  # (1)
    FirewallPolicyArn: NotRequired[str],
    FirewallPolicyId: NotRequired[str],
    FirewallPolicyName: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-braces: FirewallPolicyDetailsTypeDef](./type_defs.md#firewallpolicydetailstypedef) 
## RuleGroupSourceTypeDef

```python
# RuleGroupSourceTypeDef definition

class RuleGroupSourceTypeDef(TypedDict):
    RulesSourceList: NotRequired[RuleGroupSourceListDetailsTypeDef],  # (1)
    RulesString: NotRequired[str],
    StatefulRules: NotRequired[Sequence[RuleGroupSourceStatefulRulesDetailsTypeDef]],  # (2)
    StatelessRulesAndCustomActions: NotRequired[RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: RuleGroupSourceListDetailsTypeDef](./type_defs.md#rulegroupsourcelistdetailstypedef) 
2. See [:material-code-braces: RuleGroupSourceStatefulRulesDetailsTypeDef](./type_defs.md#rulegroupsourcestatefulrulesdetailstypedef) 
3. See [:material-code-braces: RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef](./type_defs.md#rulegroupsourcestatelessrulesandcustomactionsdetailstypedef) 
## AwsS3BucketDetailsTypeDef

```python
# AwsS3BucketDetailsTypeDef definition

class AwsS3BucketDetailsTypeDef(TypedDict):
    OwnerId: NotRequired[str],
    OwnerName: NotRequired[str],
    OwnerAccountId: NotRequired[str],
    CreatedAt: NotRequired[str],
    ServerSideEncryptionConfiguration: NotRequired[AwsS3BucketServerSideEncryptionConfigurationTypeDef],  # (1)
    BucketLifecycleConfiguration: NotRequired[AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef],  # (2)
    PublicAccessBlockConfiguration: NotRequired[AwsS3AccountPublicAccessBlockDetailsTypeDef],  # (3)
    AccessControlList: NotRequired[str],
    BucketLoggingConfiguration: NotRequired[AwsS3BucketLoggingConfigurationTypeDef],  # (4)
    BucketWebsiteConfiguration: NotRequired[AwsS3BucketWebsiteConfigurationTypeDef],  # (5)
    BucketNotificationConfiguration: NotRequired[AwsS3BucketNotificationConfigurationTypeDef],  # (6)
    BucketVersioningConfiguration: NotRequired[AwsS3BucketBucketVersioningConfigurationTypeDef],  # (7)
    ObjectLockConfiguration: NotRequired[AwsS3BucketObjectLockConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: AwsS3BucketServerSideEncryptionConfigurationTypeDef](./type_defs.md#awss3bucketserversideencryptionconfigurationtypedef) 
2. See [:material-code-braces: AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef](./type_defs.md#awss3bucketbucketlifecycleconfigurationdetailstypedef) 
3. See [:material-code-braces: AwsS3AccountPublicAccessBlockDetailsTypeDef](./type_defs.md#awss3accountpublicaccessblockdetailstypedef) 
4. See [:material-code-braces: AwsS3BucketLoggingConfigurationTypeDef](./type_defs.md#awss3bucketloggingconfigurationtypedef) 
5. See [:material-code-braces: AwsS3BucketWebsiteConfigurationTypeDef](./type_defs.md#awss3bucketwebsiteconfigurationtypedef) 
6. See [:material-code-braces: AwsS3BucketNotificationConfigurationTypeDef](./type_defs.md#awss3bucketnotificationconfigurationtypedef) 
7. See [:material-code-braces: AwsS3BucketBucketVersioningConfigurationTypeDef](./type_defs.md#awss3bucketbucketversioningconfigurationtypedef) 
8. See [:material-code-braces: AwsS3BucketObjectLockConfigurationTypeDef](./type_defs.md#awss3bucketobjectlockconfigurationtypedef) 
## DataClassificationDetailsTypeDef

```python
# DataClassificationDetailsTypeDef definition

class DataClassificationDetailsTypeDef(TypedDict):
    DetailedResultsLocation: NotRequired[str],
    Result: NotRequired[ClassificationResultTypeDef],  # (1)
```

1. See [:material-code-braces: ClassificationResultTypeDef](./type_defs.md#classificationresulttypedef) 
## RuleGroupDetailsTypeDef

```python
# RuleGroupDetailsTypeDef definition

class RuleGroupDetailsTypeDef(TypedDict):
    RuleVariables: NotRequired[RuleGroupVariablesTypeDef],  # (1)
    RulesSource: NotRequired[RuleGroupSourceTypeDef],  # (2)
```

1. See [:material-code-braces: RuleGroupVariablesTypeDef](./type_defs.md#rulegroupvariablestypedef) 
2. See [:material-code-braces: RuleGroupSourceTypeDef](./type_defs.md#rulegroupsourcetypedef) 
## AwsNetworkFirewallRuleGroupDetailsTypeDef

```python
# AwsNetworkFirewallRuleGroupDetailsTypeDef definition

class AwsNetworkFirewallRuleGroupDetailsTypeDef(TypedDict):
    Capacity: NotRequired[int],
    Description: NotRequired[str],
    RuleGroup: NotRequired[RuleGroupDetailsTypeDef],  # (1)
    RuleGroupArn: NotRequired[str],
    RuleGroupId: NotRequired[str],
    RuleGroupName: NotRequired[str],
    Type: NotRequired[str],
```

1. See [:material-code-braces: RuleGroupDetailsTypeDef](./type_defs.md#rulegroupdetailstypedef) 
## ResourceDetailsTypeDef

```python
# ResourceDetailsTypeDef definition

class ResourceDetailsTypeDef(TypedDict):
    AwsAutoScalingAutoScalingGroup: NotRequired[AwsAutoScalingAutoScalingGroupDetailsTypeDef],  # (1)
    AwsCodeBuildProject: NotRequired[AwsCodeBuildProjectDetailsTypeDef],  # (2)
    AwsCloudFrontDistribution: NotRequired[AwsCloudFrontDistributionDetailsTypeDef],  # (3)
    AwsEc2Instance: NotRequired[AwsEc2InstanceDetailsTypeDef],  # (4)
    AwsEc2NetworkInterface: NotRequired[AwsEc2NetworkInterfaceDetailsTypeDef],  # (5)
    AwsEc2SecurityGroup: NotRequired[AwsEc2SecurityGroupDetailsTypeDef],  # (6)
    AwsEc2Volume: NotRequired[AwsEc2VolumeDetailsTypeDef],  # (7)
    AwsEc2Vpc: NotRequired[AwsEc2VpcDetailsTypeDef],  # (8)
    AwsEc2Eip: NotRequired[AwsEc2EipDetailsTypeDef],  # (9)
    AwsEc2Subnet: NotRequired[AwsEc2SubnetDetailsTypeDef],  # (10)
    AwsEc2NetworkAcl: NotRequired[AwsEc2NetworkAclDetailsTypeDef],  # (11)
    AwsElbv2LoadBalancer: NotRequired[AwsElbv2LoadBalancerDetailsTypeDef],  # (12)
    AwsElasticBeanstalkEnvironment: NotRequired[AwsElasticBeanstalkEnvironmentDetailsTypeDef],  # (13)
    AwsElasticsearchDomain: NotRequired[AwsElasticsearchDomainDetailsTypeDef],  # (14)
    AwsS3Bucket: NotRequired[AwsS3BucketDetailsTypeDef],  # (15)
    AwsS3AccountPublicAccessBlock: NotRequired[AwsS3AccountPublicAccessBlockDetailsTypeDef],  # (16)
    AwsS3Object: NotRequired[AwsS3ObjectDetailsTypeDef],  # (17)
    AwsSecretsManagerSecret: NotRequired[AwsSecretsManagerSecretDetailsTypeDef],  # (18)
    AwsIamAccessKey: NotRequired[AwsIamAccessKeyDetailsTypeDef],  # (19)
    AwsIamUser: NotRequired[AwsIamUserDetailsTypeDef],  # (20)
    AwsIamPolicy: NotRequired[AwsIamPolicyDetailsTypeDef],  # (21)
    AwsApiGatewayV2Stage: NotRequired[AwsApiGatewayV2StageDetailsTypeDef],  # (22)
    AwsApiGatewayV2Api: NotRequired[AwsApiGatewayV2ApiDetailsTypeDef],  # (23)
    AwsDynamoDbTable: NotRequired[AwsDynamoDbTableDetailsTypeDef],  # (24)
    AwsApiGatewayStage: NotRequired[AwsApiGatewayStageDetailsTypeDef],  # (25)
    AwsApiGatewayRestApi: NotRequired[AwsApiGatewayRestApiDetailsTypeDef],  # (26)
    AwsCloudTrailTrail: NotRequired[AwsCloudTrailTrailDetailsTypeDef],  # (27)
    AwsSsmPatchCompliance: NotRequired[AwsSsmPatchComplianceDetailsTypeDef],  # (28)
    AwsCertificateManagerCertificate: NotRequired[AwsCertificateManagerCertificateDetailsTypeDef],  # (29)
    AwsRedshiftCluster: NotRequired[AwsRedshiftClusterDetailsTypeDef],  # (30)
    AwsElbLoadBalancer: NotRequired[AwsElbLoadBalancerDetailsTypeDef],  # (31)
    AwsIamGroup: NotRequired[AwsIamGroupDetailsTypeDef],  # (32)
    AwsIamRole: NotRequired[AwsIamRoleDetailsTypeDef],  # (33)
    AwsKmsKey: NotRequired[AwsKmsKeyDetailsTypeDef],  # (34)
    AwsLambdaFunction: NotRequired[AwsLambdaFunctionDetailsTypeDef],  # (35)
    AwsLambdaLayerVersion: NotRequired[AwsLambdaLayerVersionDetailsTypeDef],  # (36)
    AwsRdsDbInstance: NotRequired[AwsRdsDbInstanceDetailsTypeDef],  # (37)
    AwsSnsTopic: NotRequired[AwsSnsTopicDetailsTypeDef],  # (38)
    AwsSqsQueue: NotRequired[AwsSqsQueueDetailsTypeDef],  # (39)
    AwsWafWebAcl: NotRequired[AwsWafWebAclDetailsTypeDef],  # (40)
    AwsRdsDbSnapshot: NotRequired[AwsRdsDbSnapshotDetailsTypeDef],  # (41)
    AwsRdsDbClusterSnapshot: NotRequired[AwsRdsDbClusterSnapshotDetailsTypeDef],  # (42)
    AwsRdsDbCluster: NotRequired[AwsRdsDbClusterDetailsTypeDef],  # (43)
    AwsEcsCluster: NotRequired[AwsEcsClusterDetailsTypeDef],  # (44)
    AwsEcsContainer: NotRequired[AwsEcsContainerDetailsTypeDef],  # (45)
    AwsEcsTaskDefinition: NotRequired[AwsEcsTaskDefinitionDetailsTypeDef],  # (46)
    Container: NotRequired[ContainerDetailsTypeDef],  # (47)
    Other: NotRequired[Mapping[str, str]],
    AwsRdsEventSubscription: NotRequired[AwsRdsEventSubscriptionDetailsTypeDef],  # (48)
    AwsEcsService: NotRequired[AwsEcsServiceDetailsTypeDef],  # (49)
    AwsAutoScalingLaunchConfiguration: NotRequired[AwsAutoScalingLaunchConfigurationDetailsTypeDef],  # (50)
    AwsEc2VpnConnection: NotRequired[AwsEc2VpnConnectionDetailsTypeDef],  # (51)
    AwsEcrContainerImage: NotRequired[AwsEcrContainerImageDetailsTypeDef],  # (52)
    AwsOpenSearchServiceDomain: NotRequired[AwsOpenSearchServiceDomainDetailsTypeDef],  # (53)
    AwsEc2VpcEndpointService: NotRequired[AwsEc2VpcEndpointServiceDetailsTypeDef],  # (54)
    AwsXrayEncryptionConfig: NotRequired[AwsXrayEncryptionConfigDetailsTypeDef],  # (55)
    AwsWafRateBasedRule: NotRequired[AwsWafRateBasedRuleDetailsTypeDef],  # (56)
    AwsWafRegionalRateBasedRule: NotRequired[AwsWafRegionalRateBasedRuleDetailsTypeDef],  # (57)
    AwsEcrRepository: NotRequired[AwsEcrRepositoryDetailsTypeDef],  # (58)
    AwsEksCluster: NotRequired[AwsEksClusterDetailsTypeDef],  # (59)
    AwsNetworkFirewallFirewallPolicy: NotRequired[AwsNetworkFirewallFirewallPolicyDetailsTypeDef],  # (60)
    AwsNetworkFirewallFirewall: NotRequired[AwsNetworkFirewallFirewallDetailsTypeDef],  # (61)
    AwsNetworkFirewallRuleGroup: NotRequired[AwsNetworkFirewallRuleGroupDetailsTypeDef],  # (62)
    AwsRdsDbSecurityGroup: NotRequired[AwsRdsDbSecurityGroupDetailsTypeDef],  # (63)
    AwsKinesisStream: NotRequired[AwsKinesisStreamDetailsTypeDef],  # (64)
    AwsEc2TransitGateway: NotRequired[AwsEc2TransitGatewayDetailsTypeDef],  # (65)
    AwsEfsAccessPoint: NotRequired[AwsEfsAccessPointDetailsTypeDef],  # (66)
    AwsCloudFormationStack: NotRequired[AwsCloudFormationStackDetailsTypeDef],  # (67)
    AwsCloudWatchAlarm: NotRequired[AwsCloudWatchAlarmDetailsTypeDef],  # (68)
    AwsEc2VpcPeeringConnection: NotRequired[AwsEc2VpcPeeringConnectionDetailsTypeDef],  # (69)
    AwsWafRegionalRuleGroup: NotRequired[AwsWafRegionalRuleGroupDetailsTypeDef],  # (70)
    AwsWafRegionalRule: NotRequired[AwsWafRegionalRuleDetailsTypeDef],  # (71)
    AwsWafRegionalWebAcl: NotRequired[AwsWafRegionalWebAclDetailsTypeDef],  # (72)
    AwsWafRule: NotRequired[AwsWafRuleDetailsTypeDef],  # (73)
    AwsWafRuleGroup: NotRequired[AwsWafRuleGroupDetailsTypeDef],  # (74)
    AwsEcsTask: NotRequired[AwsEcsTaskDetailsTypeDef],  # (75)
    AwsBackupBackupVault: NotRequired[AwsBackupBackupVaultDetailsTypeDef],  # (76)
    AwsBackupBackupPlan: NotRequired[AwsBackupBackupPlanDetailsTypeDef],  # (77)
    AwsBackupRecoveryPoint: NotRequired[AwsBackupRecoveryPointDetailsTypeDef],  # (78)
    AwsEc2LaunchTemplate: NotRequired[AwsEc2LaunchTemplateDetailsTypeDef],  # (79)
    AwsSageMakerNotebookInstance: NotRequired[AwsSageMakerNotebookInstanceDetailsTypeDef],  # (80)
    AwsWafv2WebAcl: NotRequired[AwsWafv2WebAclDetailsTypeDef],  # (81)
    AwsWafv2RuleGroup: NotRequired[AwsWafv2RuleGroupDetailsTypeDef],  # (82)
    AwsEc2RouteTable: NotRequired[AwsEc2RouteTableDetailsTypeDef],  # (83)
    AwsAmazonMqBroker: NotRequired[AwsAmazonMqBrokerDetailsTypeDef],  # (84)
    AwsAppSyncGraphQlApi: NotRequired[AwsAppSyncGraphQlApiDetailsTypeDef],  # (85)
    AwsEventSchemasRegistry: NotRequired[AwsEventSchemasRegistryDetailsTypeDef],  # (86)
    AwsGuardDutyDetector: NotRequired[AwsGuardDutyDetectorDetailsTypeDef],  # (87)
    AwsStepFunctionStateMachine: NotRequired[AwsStepFunctionStateMachineDetailsTypeDef],  # (88)
    AwsAthenaWorkGroup: NotRequired[AwsAthenaWorkGroupDetailsTypeDef],  # (89)
```

1. See [:material-code-braces: AwsAutoScalingAutoScalingGroupDetailsTypeDef](./type_defs.md#awsautoscalingautoscalinggroupdetailstypedef) 
2. See [:material-code-braces: AwsCodeBuildProjectDetailsTypeDef](./type_defs.md#awscodebuildprojectdetailstypedef) 
3. See [:material-code-braces: AwsCloudFrontDistributionDetailsTypeDef](./type_defs.md#awscloudfrontdistributiondetailstypedef) 
4. See [:material-code-braces: AwsEc2InstanceDetailsTypeDef](./type_defs.md#awsec2instancedetailstypedef) 
5. See [:material-code-braces: AwsEc2NetworkInterfaceDetailsTypeDef](./type_defs.md#awsec2networkinterfacedetailstypedef) 
6. See [:material-code-braces: AwsEc2SecurityGroupDetailsTypeDef](./type_defs.md#awsec2securitygroupdetailstypedef) 
7. See [:material-code-braces: AwsEc2VolumeDetailsTypeDef](./type_defs.md#awsec2volumedetailstypedef) 
8. See [:material-code-braces: AwsEc2VpcDetailsTypeDef](./type_defs.md#awsec2vpcdetailstypedef) 
9. See [:material-code-braces: AwsEc2EipDetailsTypeDef](./type_defs.md#awsec2eipdetailstypedef) 
10. See [:material-code-braces: AwsEc2SubnetDetailsTypeDef](./type_defs.md#awsec2subnetdetailstypedef) 
11. See [:material-code-braces: AwsEc2NetworkAclDetailsTypeDef](./type_defs.md#awsec2networkacldetailstypedef) 
12. See [:material-code-braces: AwsElbv2LoadBalancerDetailsTypeDef](./type_defs.md#awselbv2loadbalancerdetailstypedef) 
13. See [:material-code-braces: AwsElasticBeanstalkEnvironmentDetailsTypeDef](./type_defs.md#awselasticbeanstalkenvironmentdetailstypedef) 
14. See [:material-code-braces: AwsElasticsearchDomainDetailsTypeDef](./type_defs.md#awselasticsearchdomaindetailstypedef) 
15. See [:material-code-braces: AwsS3BucketDetailsTypeDef](./type_defs.md#awss3bucketdetailstypedef) 
16. See [:material-code-braces: AwsS3AccountPublicAccessBlockDetailsTypeDef](./type_defs.md#awss3accountpublicaccessblockdetailstypedef) 
17. See [:material-code-braces: AwsS3ObjectDetailsTypeDef](./type_defs.md#awss3objectdetailstypedef) 
18. See [:material-code-braces: AwsSecretsManagerSecretDetailsTypeDef](./type_defs.md#awssecretsmanagersecretdetailstypedef) 
19. See [:material-code-braces: AwsIamAccessKeyDetailsTypeDef](./type_defs.md#awsiamaccesskeydetailstypedef) 
20. See [:material-code-braces: AwsIamUserDetailsTypeDef](./type_defs.md#awsiamuserdetailstypedef) 
21. See [:material-code-braces: AwsIamPolicyDetailsTypeDef](./type_defs.md#awsiampolicydetailstypedef) 
22. See [:material-code-braces: AwsApiGatewayV2StageDetailsTypeDef](./type_defs.md#awsapigatewayv2stagedetailstypedef) 
23. See [:material-code-braces: AwsApiGatewayV2ApiDetailsTypeDef](./type_defs.md#awsapigatewayv2apidetailstypedef) 
24. See [:material-code-braces: AwsDynamoDbTableDetailsTypeDef](./type_defs.md#awsdynamodbtabledetailstypedef) 
25. See [:material-code-braces: AwsApiGatewayStageDetailsTypeDef](./type_defs.md#awsapigatewaystagedetailstypedef) 
26. See [:material-code-braces: AwsApiGatewayRestApiDetailsTypeDef](./type_defs.md#awsapigatewayrestapidetailstypedef) 
27. See [:material-code-braces: AwsCloudTrailTrailDetailsTypeDef](./type_defs.md#awscloudtrailtraildetailstypedef) 
28. See [:material-code-braces: AwsSsmPatchComplianceDetailsTypeDef](./type_defs.md#awsssmpatchcompliancedetailstypedef) 
29. See [:material-code-braces: AwsCertificateManagerCertificateDetailsTypeDef](./type_defs.md#awscertificatemanagercertificatedetailstypedef) 
30. See [:material-code-braces: AwsRedshiftClusterDetailsTypeDef](./type_defs.md#awsredshiftclusterdetailstypedef) 
31. See [:material-code-braces: AwsElbLoadBalancerDetailsTypeDef](./type_defs.md#awselbloadbalancerdetailstypedef) 
32. See [:material-code-braces: AwsIamGroupDetailsTypeDef](./type_defs.md#awsiamgroupdetailstypedef) 
33. See [:material-code-braces: AwsIamRoleDetailsTypeDef](./type_defs.md#awsiamroledetailstypedef) 
34. See [:material-code-braces: AwsKmsKeyDetailsTypeDef](./type_defs.md#awskmskeydetailstypedef) 
35. See [:material-code-braces: AwsLambdaFunctionDetailsTypeDef](./type_defs.md#awslambdafunctiondetailstypedef) 
36. See [:material-code-braces: AwsLambdaLayerVersionDetailsTypeDef](./type_defs.md#awslambdalayerversiondetailstypedef) 
37. See [:material-code-braces: AwsRdsDbInstanceDetailsTypeDef](./type_defs.md#awsrdsdbinstancedetailstypedef) 
38. See [:material-code-braces: AwsSnsTopicDetailsTypeDef](./type_defs.md#awssnstopicdetailstypedef) 
39. See [:material-code-braces: AwsSqsQueueDetailsTypeDef](./type_defs.md#awssqsqueuedetailstypedef) 
40. See [:material-code-braces: AwsWafWebAclDetailsTypeDef](./type_defs.md#awswafwebacldetailstypedef) 
41. See [:material-code-braces: AwsRdsDbSnapshotDetailsTypeDef](./type_defs.md#awsrdsdbsnapshotdetailstypedef) 
42. See [:material-code-braces: AwsRdsDbClusterSnapshotDetailsTypeDef](./type_defs.md#awsrdsdbclustersnapshotdetailstypedef) 
43. See [:material-code-braces: AwsRdsDbClusterDetailsTypeDef](./type_defs.md#awsrdsdbclusterdetailstypedef) 
44. See [:material-code-braces: AwsEcsClusterDetailsTypeDef](./type_defs.md#awsecsclusterdetailstypedef) 
45. See [:material-code-braces: AwsEcsContainerDetailsTypeDef](./type_defs.md#awsecscontainerdetailstypedef) 
46. See [:material-code-braces: AwsEcsTaskDefinitionDetailsTypeDef](./type_defs.md#awsecstaskdefinitiondetailstypedef) 
47. See [:material-code-braces: ContainerDetailsTypeDef](./type_defs.md#containerdetailstypedef) 
48. See [:material-code-braces: AwsRdsEventSubscriptionDetailsTypeDef](./type_defs.md#awsrdseventsubscriptiondetailstypedef) 
49. See [:material-code-braces: AwsEcsServiceDetailsTypeDef](./type_defs.md#awsecsservicedetailstypedef) 
50. See [:material-code-braces: AwsAutoScalingLaunchConfigurationDetailsTypeDef](./type_defs.md#awsautoscalinglaunchconfigurationdetailstypedef) 
51. See [:material-code-braces: AwsEc2VpnConnectionDetailsTypeDef](./type_defs.md#awsec2vpnconnectiondetailstypedef) 
52. See [:material-code-braces: AwsEcrContainerImageDetailsTypeDef](./type_defs.md#awsecrcontainerimagedetailstypedef) 
53. See [:material-code-braces: AwsOpenSearchServiceDomainDetailsTypeDef](./type_defs.md#awsopensearchservicedomaindetailstypedef) 
54. See [:material-code-braces: AwsEc2VpcEndpointServiceDetailsTypeDef](./type_defs.md#awsec2vpcendpointservicedetailstypedef) 
55. See [:material-code-braces: AwsXrayEncryptionConfigDetailsTypeDef](./type_defs.md#awsxrayencryptionconfigdetailstypedef) 
56. See [:material-code-braces: AwsWafRateBasedRuleDetailsTypeDef](./type_defs.md#awswafratebasedruledetailstypedef) 
57. See [:material-code-braces: AwsWafRegionalRateBasedRuleDetailsTypeDef](./type_defs.md#awswafregionalratebasedruledetailstypedef) 
58. See [:material-code-braces: AwsEcrRepositoryDetailsTypeDef](./type_defs.md#awsecrrepositorydetailstypedef) 
59. See [:material-code-braces: AwsEksClusterDetailsTypeDef](./type_defs.md#awseksclusterdetailstypedef) 
60. See [:material-code-braces: AwsNetworkFirewallFirewallPolicyDetailsTypeDef](./type_defs.md#awsnetworkfirewallfirewallpolicydetailstypedef) 
61. See [:material-code-braces: AwsNetworkFirewallFirewallDetailsTypeDef](./type_defs.md#awsnetworkfirewallfirewalldetailstypedef) 
62. See [:material-code-braces: AwsNetworkFirewallRuleGroupDetailsTypeDef](./type_defs.md#awsnetworkfirewallrulegroupdetailstypedef) 
63. See [:material-code-braces: AwsRdsDbSecurityGroupDetailsTypeDef](./type_defs.md#awsrdsdbsecuritygroupdetailstypedef) 
64. See [:material-code-braces: AwsKinesisStreamDetailsTypeDef](./type_defs.md#awskinesisstreamdetailstypedef) 
65. See [:material-code-braces: AwsEc2TransitGatewayDetailsTypeDef](./type_defs.md#awsec2transitgatewaydetailstypedef) 
66. See [:material-code-braces: AwsEfsAccessPointDetailsTypeDef](./type_defs.md#awsefsaccesspointdetailstypedef) 
67. See [:material-code-braces: AwsCloudFormationStackDetailsTypeDef](./type_defs.md#awscloudformationstackdetailstypedef) 
68. See [:material-code-braces: AwsCloudWatchAlarmDetailsTypeDef](./type_defs.md#awscloudwatchalarmdetailstypedef) 
69. See [:material-code-braces: AwsEc2VpcPeeringConnectionDetailsTypeDef](./type_defs.md#awsec2vpcpeeringconnectiondetailstypedef) 
70. See [:material-code-braces: AwsWafRegionalRuleGroupDetailsTypeDef](./type_defs.md#awswafregionalrulegroupdetailstypedef) 
71. See [:material-code-braces: AwsWafRegionalRuleDetailsTypeDef](./type_defs.md#awswafregionalruledetailstypedef) 
72. See [:material-code-braces: AwsWafRegionalWebAclDetailsTypeDef](./type_defs.md#awswafregionalwebacldetailstypedef) 
73. See [:material-code-braces: AwsWafRuleDetailsTypeDef](./type_defs.md#awswafruledetailstypedef) 
74. See [:material-code-braces: AwsWafRuleGroupDetailsTypeDef](./type_defs.md#awswafrulegroupdetailstypedef) 
75. See [:material-code-braces: AwsEcsTaskDetailsTypeDef](./type_defs.md#awsecstaskdetailstypedef) 
76. See [:material-code-braces: AwsBackupBackupVaultDetailsTypeDef](./type_defs.md#awsbackupbackupvaultdetailstypedef) 
77. See [:material-code-braces: AwsBackupBackupPlanDetailsTypeDef](./type_defs.md#awsbackupbackupplandetailstypedef) 
78. See [:material-code-braces: AwsBackupRecoveryPointDetailsTypeDef](./type_defs.md#awsbackuprecoverypointdetailstypedef) 
79. See [:material-code-braces: AwsEc2LaunchTemplateDetailsTypeDef](./type_defs.md#awsec2launchtemplatedetailstypedef) 
80. See [:material-code-braces: AwsSageMakerNotebookInstanceDetailsTypeDef](./type_defs.md#awssagemakernotebookinstancedetailstypedef) 
81. See [:material-code-braces: AwsWafv2WebAclDetailsTypeDef](./type_defs.md#awswafv2webacldetailstypedef) 
82. See [:material-code-braces: AwsWafv2RuleGroupDetailsTypeDef](./type_defs.md#awswafv2rulegroupdetailstypedef) 
83. See [:material-code-braces: AwsEc2RouteTableDetailsTypeDef](./type_defs.md#awsec2routetabledetailstypedef) 
84. See [:material-code-braces: AwsAmazonMqBrokerDetailsTypeDef](./type_defs.md#awsamazonmqbrokerdetailstypedef) 
85. See [:material-code-braces: AwsAppSyncGraphQlApiDetailsTypeDef](./type_defs.md#awsappsyncgraphqlapidetailstypedef) 
86. See [:material-code-braces: AwsEventSchemasRegistryDetailsTypeDef](./type_defs.md#awseventschemasregistrydetailstypedef) 
87. See [:material-code-braces: AwsGuardDutyDetectorDetailsTypeDef](./type_defs.md#awsguarddutydetectordetailstypedef) 
88. See [:material-code-braces: AwsStepFunctionStateMachineDetailsTypeDef](./type_defs.md#awsstepfunctionstatemachinedetailstypedef) 
89. See [:material-code-braces: AwsAthenaWorkGroupDetailsTypeDef](./type_defs.md#awsathenaworkgroupdetailstypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    Type: str,
    Id: str,
    Partition: NotRequired[PartitionType],  # (1)
    Region: NotRequired[str],
    ResourceRole: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    DataClassification: NotRequired[DataClassificationDetailsTypeDef],  # (2)
    Details: NotRequired[ResourceDetailsTypeDef],  # (3)
```

1. See [:material-code-brackets: PartitionType](./literals.md#partitiontype) 
2. See [:material-code-braces: DataClassificationDetailsTypeDef](./type_defs.md#dataclassificationdetailstypedef) 
3. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
## AwsSecurityFindingTypeDef

```python
# AwsSecurityFindingTypeDef definition

class AwsSecurityFindingTypeDef(TypedDict):
    SchemaVersion: str,
    Id: str,
    ProductArn: str,
    GeneratorId: str,
    AwsAccountId: str,
    CreatedAt: str,
    UpdatedAt: str,
    Title: str,
    Description: str,
    Resources: Sequence[ResourceTypeDef],  # (9)
    ProductName: NotRequired[str],
    CompanyName: NotRequired[str],
    Region: NotRequired[str],
    Types: NotRequired[Sequence[str]],
    FirstObservedAt: NotRequired[str],
    LastObservedAt: NotRequired[str],
    Severity: NotRequired[SeverityTypeDef],  # (1)
    Confidence: NotRequired[int],
    Criticality: NotRequired[int],
    Remediation: NotRequired[RemediationTypeDef],  # (2)
    SourceUrl: NotRequired[str],
    ProductFields: NotRequired[Mapping[str, str]],
    UserDefinedFields: NotRequired[Mapping[str, str]],
    Malware: NotRequired[Sequence[MalwareTypeDef]],  # (3)
    Network: NotRequired[NetworkTypeDef],  # (4)
    NetworkPath: NotRequired[Sequence[NetworkPathComponentTypeDef]],  # (5)
    Process: NotRequired[ProcessDetailsTypeDef],  # (6)
    Threats: NotRequired[Sequence[ThreatTypeDef]],  # (7)
    ThreatIntelIndicators: NotRequired[Sequence[ThreatIntelIndicatorTypeDef]],  # (8)
    Compliance: NotRequired[ComplianceTypeDef],  # (10)
    VerificationState: NotRequired[VerificationStateType],  # (11)
    WorkflowState: NotRequired[WorkflowStateType],  # (12)
    Workflow: NotRequired[WorkflowTypeDef],  # (13)
    RecordState: NotRequired[RecordStateType],  # (14)
    RelatedFindings: NotRequired[Sequence[RelatedFindingTypeDef]],  # (15)
    Note: NotRequired[NoteTypeDef],  # (16)
    Vulnerabilities: NotRequired[Sequence[VulnerabilityTypeDef]],  # (17)
    PatchSummary: NotRequired[PatchSummaryTypeDef],  # (18)
    Action: NotRequired[ActionTypeDef],  # (19)
    FindingProviderFields: NotRequired[FindingProviderFieldsTypeDef],  # (20)
    Sample: NotRequired[bool],
```

1. See [:material-code-braces: SeverityTypeDef](./type_defs.md#severitytypedef) 
2. See [:material-code-braces: RemediationTypeDef](./type_defs.md#remediationtypedef) 
3. See [:material-code-braces: MalwareTypeDef](./type_defs.md#malwaretypedef) 
4. See [:material-code-braces: NetworkTypeDef](./type_defs.md#networktypedef) 
5. See [:material-code-braces: NetworkPathComponentTypeDef](./type_defs.md#networkpathcomponenttypedef) 
6. See [:material-code-braces: ProcessDetailsTypeDef](./type_defs.md#processdetailstypedef) 
7. See [:material-code-braces: ThreatTypeDef](./type_defs.md#threattypedef) 
8. See [:material-code-braces: ThreatIntelIndicatorTypeDef](./type_defs.md#threatintelindicatortypedef) 
9. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
10. See [:material-code-braces: ComplianceTypeDef](./type_defs.md#compliancetypedef) 
11. See [:material-code-brackets: VerificationStateType](./literals.md#verificationstatetype) 
12. See [:material-code-brackets: WorkflowStateType](./literals.md#workflowstatetype) 
13. See [:material-code-braces: WorkflowTypeDef](./type_defs.md#workflowtypedef) 
14. See [:material-code-brackets: RecordStateType](./literals.md#recordstatetype) 
15. See [:material-code-braces: RelatedFindingTypeDef](./type_defs.md#relatedfindingtypedef) 
16. See [:material-code-braces: NoteTypeDef](./type_defs.md#notetypedef) 
17. See [:material-code-braces: VulnerabilityTypeDef](./type_defs.md#vulnerabilitytypedef) 
18. See [:material-code-braces: PatchSummaryTypeDef](./type_defs.md#patchsummarytypedef) 
19. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
20. See [:material-code-braces: FindingProviderFieldsTypeDef](./type_defs.md#findingproviderfieldstypedef) 
## BatchImportFindingsRequestRequestTypeDef

```python
# BatchImportFindingsRequestRequestTypeDef definition

class BatchImportFindingsRequestRequestTypeDef(TypedDict):
    Findings: Sequence[AwsSecurityFindingTypeDef],  # (1)
```

1. See [:material-code-braces: AwsSecurityFindingTypeDef](./type_defs.md#awssecurityfindingtypedef) 
## GetFindingsResponseTypeDef

```python
# GetFindingsResponseTypeDef definition

class GetFindingsResponseTypeDef(TypedDict):
    Findings: List[AwsSecurityFindingTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AwsSecurityFindingTypeDef](./type_defs.md#awssecurityfindingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
