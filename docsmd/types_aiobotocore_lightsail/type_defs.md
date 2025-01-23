# Type definitions

> [Index](../README.md) > [Lightsail](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Lightsail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#lightsail)
    type annotations stubs module [types-aiobotocore-lightsail](https://pypi.org/project/types-aiobotocore-lightsail/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ContainerUnionTypeDef

```python
# ContainerUnionTypeDef definition

ContainerUnionTypeDef = Union[
    ContainerTypeDef,  # (1)
    ContainerOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) 
2. See [:material-code-braces: ContainerOutputTypeDef](./type_defs.md#containeroutputtypedef) 

## CookieObjectUnionTypeDef

```python
# CookieObjectUnionTypeDef definition

CookieObjectUnionTypeDef = Union[
    CookieObjectTypeDef,  # (1)
    CookieObjectOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CookieObjectTypeDef](./type_defs.md#cookieobjecttypedef) 
2. See [:material-code-braces: CookieObjectOutputTypeDef](./type_defs.md#cookieobjectoutputtypedef) 

## HeaderObjectUnionTypeDef

```python
# HeaderObjectUnionTypeDef definition

HeaderObjectUnionTypeDef = Union[
    HeaderObjectTypeDef,  # (1)
    HeaderObjectOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HeaderObjectTypeDef](./type_defs.md#headerobjecttypedef) 
2. See [:material-code-braces: HeaderObjectOutputTypeDef](./type_defs.md#headerobjectoutputtypedef) 

## QueryStringObjectUnionTypeDef

```python
# QueryStringObjectUnionTypeDef definition

QueryStringObjectUnionTypeDef = Union[
    QueryStringObjectTypeDef,  # (1)
    QueryStringObjectOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: QueryStringObjectTypeDef](./type_defs.md#querystringobjecttypedef) 
2. See [:material-code-braces: QueryStringObjectOutputTypeDef](./type_defs.md#querystringobjectoutputtypedef) 



## AccessKeyLastUsedTypeDef

```python
# AccessKeyLastUsedTypeDef definition

class AccessKeyLastUsedTypeDef(TypedDict):
    lastUsedDate: NotRequired[datetime],
    region: NotRequired[str],
    serviceName: NotRequired[str],
```

## AccessRulesTypeDef

```python
# AccessRulesTypeDef definition

class AccessRulesTypeDef(TypedDict):
    getObject: NotRequired[AccessTypeType],  # (1)
    allowPublicOverrides: NotRequired[bool],
```

1. See [:material-code-brackets: AccessTypeType](./literals.md#accesstypetype) 
## AccountLevelBpaSyncTypeDef

```python
# AccountLevelBpaSyncTypeDef definition

class AccountLevelBpaSyncTypeDef(TypedDict):
    status: NotRequired[AccountLevelBpaSyncStatusType],  # (1)
    lastSyncedAt: NotRequired[datetime],
    message: NotRequired[BPAStatusMessageType],  # (2)
    bpaImpactsLightsail: NotRequired[bool],
```

1. See [:material-code-brackets: AccountLevelBpaSyncStatusType](./literals.md#accountlevelbpasyncstatustype) 
2. See [:material-code-brackets: BPAStatusMessageType](./literals.md#bpastatusmessagetype) 
## AutoSnapshotAddOnRequestTypeDef

```python
# AutoSnapshotAddOnRequestTypeDef definition

class AutoSnapshotAddOnRequestTypeDef(TypedDict):
    snapshotTimeOfDay: NotRequired[str],
```

## StopInstanceOnIdleRequestTypeDef

```python
# StopInstanceOnIdleRequestTypeDef definition

class StopInstanceOnIdleRequestTypeDef(TypedDict):
    threshold: NotRequired[str],
    duration: NotRequired[str],
```

## AddOnTypeDef

```python
# AddOnTypeDef definition

class AddOnTypeDef(TypedDict):
    name: NotRequired[str],
    status: NotRequired[str],
    snapshotTimeOfDay: NotRequired[str],
    nextSnapshotTimeOfDay: NotRequired[str],
    threshold: NotRequired[str],
    duration: NotRequired[str],
```

## MonitoredResourceInfoTypeDef

```python
# MonitoredResourceInfoTypeDef definition

class MonitoredResourceInfoTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ResourceLocationTypeDef

```python
# ResourceLocationTypeDef definition

class ResourceLocationTypeDef(TypedDict):
    availabilityZone: NotRequired[str],
    regionName: NotRequired[RegionNameType],  # (1)
```

1. See [:material-code-brackets: RegionNameType](./literals.md#regionnametype) 
## AllocateStaticIpRequestRequestTypeDef

```python
# AllocateStaticIpRequestRequestTypeDef definition

class AllocateStaticIpRequestRequestTypeDef(TypedDict):
    staticIpName: str,
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

## AttachCertificateToDistributionRequestRequestTypeDef

```python
# AttachCertificateToDistributionRequestRequestTypeDef definition

class AttachCertificateToDistributionRequestRequestTypeDef(TypedDict):
    distributionName: str,
    certificateName: str,
```

## AttachDiskRequestRequestTypeDef

```python
# AttachDiskRequestRequestTypeDef definition

class AttachDiskRequestRequestTypeDef(TypedDict):
    diskName: str,
    instanceName: str,
    diskPath: str,
    autoMounting: NotRequired[bool],
```

## AttachInstancesToLoadBalancerRequestRequestTypeDef

```python
# AttachInstancesToLoadBalancerRequestRequestTypeDef definition

class AttachInstancesToLoadBalancerRequestRequestTypeDef(TypedDict):
    loadBalancerName: str,
    instanceNames: Sequence[str],
```

## AttachLoadBalancerTlsCertificateRequestRequestTypeDef

```python
# AttachLoadBalancerTlsCertificateRequestRequestTypeDef definition

class AttachLoadBalancerTlsCertificateRequestRequestTypeDef(TypedDict):
    loadBalancerName: str,
    certificateName: str,
```

## AttachStaticIpRequestRequestTypeDef

```python
# AttachStaticIpRequestRequestTypeDef definition

class AttachStaticIpRequestRequestTypeDef(TypedDict):
    staticIpName: str,
    instanceName: str,
```

## AttachedDiskTypeDef

```python
# AttachedDiskTypeDef definition

class AttachedDiskTypeDef(TypedDict):
    path: NotRequired[str],
    sizeInGb: NotRequired[int],
```

## AvailabilityZoneTypeDef

```python
# AvailabilityZoneTypeDef definition

class AvailabilityZoneTypeDef(TypedDict):
    zoneName: NotRequired[str],
    state: NotRequired[str],
```

## BlueprintTypeDef

```python
# BlueprintTypeDef definition

class BlueprintTypeDef(TypedDict):
    blueprintId: NotRequired[str],
    name: NotRequired[str],
    group: NotRequired[str],
    type: NotRequired[BlueprintTypeType],  # (1)
    description: NotRequired[str],
    isActive: NotRequired[bool],
    minPower: NotRequired[int],
    version: NotRequired[str],
    versionCode: NotRequired[str],
    productUrl: NotRequired[str],
    licenseUrl: NotRequired[str],
    platform: NotRequired[InstancePlatformType],  # (2)
    appCategory: NotRequired[AppCategoryType],  # (3)
```

1. See [:material-code-brackets: BlueprintTypeType](./literals.md#blueprinttypetype) 
2. See [:material-code-brackets: InstancePlatformType](./literals.md#instanceplatformtype) 
3. See [:material-code-brackets: AppCategoryType](./literals.md#appcategorytype) 
## BucketAccessLogConfigTypeDef

```python
# BucketAccessLogConfigTypeDef definition

class BucketAccessLogConfigTypeDef(TypedDict):
    enabled: bool,
    destination: NotRequired[str],
    prefix: NotRequired[str],
```

## BucketBundleTypeDef

```python
# BucketBundleTypeDef definition

class BucketBundleTypeDef(TypedDict):
    bundleId: NotRequired[str],
    name: NotRequired[str],
    price: NotRequired[float],
    storagePerMonthInGb: NotRequired[int],
    transferPerMonthInGb: NotRequired[int],
    isActive: NotRequired[bool],
```

## BucketStateTypeDef

```python
# BucketStateTypeDef definition

class BucketStateTypeDef(TypedDict):
    code: NotRequired[str],
    message: NotRequired[str],
```

## ResourceReceivingAccessTypeDef

```python
# ResourceReceivingAccessTypeDef definition

class ResourceReceivingAccessTypeDef(TypedDict):
    name: NotRequired[str],
    resourceType: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## BundleTypeDef

```python
# BundleTypeDef definition

class BundleTypeDef(TypedDict):
    price: NotRequired[float],
    cpuCount: NotRequired[int],
    diskSizeInGb: NotRequired[int],
    bundleId: NotRequired[str],
    instanceType: NotRequired[str],
    isActive: NotRequired[bool],
    name: NotRequired[str],
    power: NotRequired[int],
    ramSizeInGb: NotRequired[float],
    transferPerMonthInGb: NotRequired[int],
    supportedPlatforms: NotRequired[List[InstancePlatformType]],  # (1)
    supportedAppCategories: NotRequired[List[AppCategoryType]],  # (2)
    publicIpv4AddressCount: NotRequired[int],
```

1. See [:material-code-brackets: InstancePlatformType](./literals.md#instanceplatformtype) 
2. See [:material-code-brackets: AppCategoryType](./literals.md#appcategorytype) 
## CacheBehaviorPerPathTypeDef

```python
# CacheBehaviorPerPathTypeDef definition

class CacheBehaviorPerPathTypeDef(TypedDict):
    path: NotRequired[str],
    behavior: NotRequired[BehaviorEnumType],  # (1)
```

1. See [:material-code-brackets: BehaviorEnumType](./literals.md#behaviorenumtype) 
## CacheBehaviorTypeDef

```python
# CacheBehaviorTypeDef definition

class CacheBehaviorTypeDef(TypedDict):
    behavior: NotRequired[BehaviorEnumType],  # (1)
```

1. See [:material-code-brackets: BehaviorEnumType](./literals.md#behaviorenumtype) 
## CookieObjectOutputTypeDef

```python
# CookieObjectOutputTypeDef definition

class CookieObjectOutputTypeDef(TypedDict):
    option: NotRequired[ForwardValuesType],  # (1)
    cookiesAllowList: NotRequired[List[str]],
```

1. See [:material-code-brackets: ForwardValuesType](./literals.md#forwardvaluestype) 
## HeaderObjectOutputTypeDef

```python
# HeaderObjectOutputTypeDef definition

class HeaderObjectOutputTypeDef(TypedDict):
    option: NotRequired[ForwardValuesType],  # (1)
    headersAllowList: NotRequired[List[HeaderEnumType]],  # (2)
```

1. See [:material-code-brackets: ForwardValuesType](./literals.md#forwardvaluestype) 
2. See [:material-code-brackets: HeaderEnumType](./literals.md#headerenumtype) 
## QueryStringObjectOutputTypeDef

```python
# QueryStringObjectOutputTypeDef definition

class QueryStringObjectOutputTypeDef(TypedDict):
    option: NotRequired[bool],
    queryStringsAllowList: NotRequired[List[str]],
```

## PortInfoTypeDef

```python
# PortInfoTypeDef definition

class PortInfoTypeDef(TypedDict):
    fromPort: NotRequired[int],
    toPort: NotRequired[int],
    protocol: NotRequired[NetworkProtocolType],  # (1)
    cidrs: NotRequired[Sequence[str]],
    ipv6Cidrs: NotRequired[Sequence[str]],
    cidrListAliases: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: NetworkProtocolType](./literals.md#networkprotocoltype) 
## CloudFormationStackRecordSourceInfoTypeDef

```python
# CloudFormationStackRecordSourceInfoTypeDef definition

class CloudFormationStackRecordSourceInfoTypeDef(TypedDict):
    resourceType: NotRequired[CloudFormationStackRecordSourceTypeType],  # (1)
    name: NotRequired[str],
    arn: NotRequired[str],
```

1. See [:material-code-brackets: CloudFormationStackRecordSourceTypeType](./literals.md#cloudformationstackrecordsourcetypetype) 
## DestinationInfoTypeDef

```python
# DestinationInfoTypeDef definition

class DestinationInfoTypeDef(TypedDict):
    id: NotRequired[str],
    service: NotRequired[str],
```

## ContainerImageTypeDef

```python
# ContainerImageTypeDef definition

class ContainerImageTypeDef(TypedDict):
    image: NotRequired[str],
    digest: NotRequired[str],
    createdAt: NotRequired[datetime],
```

## ContainerOutputTypeDef

```python
# ContainerOutputTypeDef definition

class ContainerOutputTypeDef(TypedDict):
    image: NotRequired[str],
    command: NotRequired[List[str]],
    environment: NotRequired[Dict[str, str]],
    ports: NotRequired[Dict[str, ContainerServiceProtocolType]],  # (1)
```

1. See [:material-code-brackets: ContainerServiceProtocolType](./literals.md#containerserviceprotocoltype) 
## ContainerServiceECRImagePullerRoleRequestTypeDef

```python
# ContainerServiceECRImagePullerRoleRequestTypeDef definition

class ContainerServiceECRImagePullerRoleRequestTypeDef(TypedDict):
    isActive: NotRequired[bool],
```

## ContainerServiceECRImagePullerRoleTypeDef

```python
# ContainerServiceECRImagePullerRoleTypeDef definition

class ContainerServiceECRImagePullerRoleTypeDef(TypedDict):
    isActive: NotRequired[bool],
    principalArn: NotRequired[str],
```

## ContainerServiceHealthCheckConfigTypeDef

```python
# ContainerServiceHealthCheckConfigTypeDef definition

class ContainerServiceHealthCheckConfigTypeDef(TypedDict):
    healthyThreshold: NotRequired[int],
    unhealthyThreshold: NotRequired[int],
    timeoutSeconds: NotRequired[int],
    intervalSeconds: NotRequired[int],
    path: NotRequired[str],
    successCodes: NotRequired[str],
```

## ContainerServiceLogEventTypeDef

```python
# ContainerServiceLogEventTypeDef definition

class ContainerServiceLogEventTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    message: NotRequired[str],
```

## ContainerServicePowerTypeDef

```python
# ContainerServicePowerTypeDef definition

class ContainerServicePowerTypeDef(TypedDict):
    powerId: NotRequired[str],
    price: NotRequired[float],
    cpuCount: NotRequired[float],
    ramSizeInGb: NotRequired[float],
    name: NotRequired[str],
    isActive: NotRequired[bool],
```

## ContainerServiceRegistryLoginTypeDef

```python
# ContainerServiceRegistryLoginTypeDef definition

class ContainerServiceRegistryLoginTypeDef(TypedDict):
    username: NotRequired[str],
    password: NotRequired[str],
    expiresAt: NotRequired[datetime],
    registry: NotRequired[str],
```

## ContainerServiceStateDetailTypeDef

```python
# ContainerServiceStateDetailTypeDef definition

class ContainerServiceStateDetailTypeDef(TypedDict):
    code: NotRequired[ContainerServiceStateDetailCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: ContainerServiceStateDetailCodeType](./literals.md#containerservicestatedetailcodetype) 
## ContainerTypeDef

```python
# ContainerTypeDef definition

class ContainerTypeDef(TypedDict):
    image: NotRequired[str],
    command: NotRequired[Sequence[str]],
    environment: NotRequired[Mapping[str, str]],
    ports: NotRequired[Mapping[str, ContainerServiceProtocolType]],  # (1)
```

1. See [:material-code-brackets: ContainerServiceProtocolType](./literals.md#containerserviceprotocoltype) 
## CookieObjectTypeDef

```python
# CookieObjectTypeDef definition

class CookieObjectTypeDef(TypedDict):
    option: NotRequired[ForwardValuesType],  # (1)
    cookiesAllowList: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ForwardValuesType](./literals.md#forwardvaluestype) 
## CopySnapshotRequestRequestTypeDef

```python
# CopySnapshotRequestRequestTypeDef definition

class CopySnapshotRequestRequestTypeDef(TypedDict):
    targetSnapshotName: str,
    sourceRegion: RegionNameType,  # (1)
    sourceSnapshotName: NotRequired[str],
    sourceResourceName: NotRequired[str],
    restoreDate: NotRequired[str],
    useLatestRestorableAutoSnapshot: NotRequired[bool],
```

1. See [:material-code-brackets: RegionNameType](./literals.md#regionnametype) 
## CreateBucketAccessKeyRequestRequestTypeDef

```python
# CreateBucketAccessKeyRequestRequestTypeDef definition

class CreateBucketAccessKeyRequestRequestTypeDef(TypedDict):
    bucketName: str,
```

## InstanceEntryTypeDef

```python
# InstanceEntryTypeDef definition

class InstanceEntryTypeDef(TypedDict):
    sourceName: str,
    instanceType: str,
    portInfoSource: PortInfoSourceTypeType,  # (1)
    availabilityZone: str,
    userData: NotRequired[str],
```

1. See [:material-code-brackets: PortInfoSourceTypeType](./literals.md#portinfosourcetypetype) 
## CreateContactMethodRequestRequestTypeDef

```python
# CreateContactMethodRequestRequestTypeDef definition

class CreateContactMethodRequestRequestTypeDef(TypedDict):
    protocol: ContactProtocolType,  # (1)
    contactEndpoint: str,
```

1. See [:material-code-brackets: ContactProtocolType](./literals.md#contactprotocoltype) 
## InputOriginTypeDef

```python
# InputOriginTypeDef definition

class InputOriginTypeDef(TypedDict):
    name: NotRequired[str],
    regionName: NotRequired[RegionNameType],  # (1)
    protocolPolicy: NotRequired[OriginProtocolPolicyEnumType],  # (2)
    responseTimeout: NotRequired[int],
```

1. See [:material-code-brackets: RegionNameType](./literals.md#regionnametype) 
2. See [:material-code-brackets: OriginProtocolPolicyEnumType](./literals.md#originprotocolpolicyenumtype) 
## DomainEntryTypeDef

```python
# DomainEntryTypeDef definition

class DomainEntryTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    target: NotRequired[str],
    isAlias: NotRequired[bool],
    type: NotRequired[str],
    options: NotRequired[Mapping[str, str]],
```

## CreateGUISessionAccessDetailsRequestRequestTypeDef

```python
# CreateGUISessionAccessDetailsRequestRequestTypeDef definition

class CreateGUISessionAccessDetailsRequestRequestTypeDef(TypedDict):
    resourceName: str,
```

## SessionTypeDef

```python
# SessionTypeDef definition

class SessionTypeDef(TypedDict):
    name: NotRequired[str],
    url: NotRequired[str],
    isPrimary: NotRequired[bool],
```

## DiskMapTypeDef

```python
# DiskMapTypeDef definition

class DiskMapTypeDef(TypedDict):
    originalDiskPath: NotRequired[str],
    newDiskName: NotRequired[str],
```

## DeleteAlarmRequestRequestTypeDef

```python
# DeleteAlarmRequestRequestTypeDef definition

class DeleteAlarmRequestRequestTypeDef(TypedDict):
    alarmName: str,
```

## DeleteAutoSnapshotRequestRequestTypeDef

```python
# DeleteAutoSnapshotRequestRequestTypeDef definition

class DeleteAutoSnapshotRequestRequestTypeDef(TypedDict):
    resourceName: str,
    date: str,
```

## DeleteBucketAccessKeyRequestRequestTypeDef

```python
# DeleteBucketAccessKeyRequestRequestTypeDef definition

class DeleteBucketAccessKeyRequestRequestTypeDef(TypedDict):
    bucketName: str,
    accessKeyId: str,
```

## DeleteBucketRequestRequestTypeDef

```python
# DeleteBucketRequestRequestTypeDef definition

class DeleteBucketRequestRequestTypeDef(TypedDict):
    bucketName: str,
    forceDelete: NotRequired[bool],
```

## DeleteCertificateRequestRequestTypeDef

```python
# DeleteCertificateRequestRequestTypeDef definition

class DeleteCertificateRequestRequestTypeDef(TypedDict):
    certificateName: str,
```

## DeleteContactMethodRequestRequestTypeDef

```python
# DeleteContactMethodRequestRequestTypeDef definition

class DeleteContactMethodRequestRequestTypeDef(TypedDict):
    protocol: ContactProtocolType,  # (1)
```

1. See [:material-code-brackets: ContactProtocolType](./literals.md#contactprotocoltype) 
## DeleteContainerImageRequestRequestTypeDef

```python
# DeleteContainerImageRequestRequestTypeDef definition

class DeleteContainerImageRequestRequestTypeDef(TypedDict):
    serviceName: str,
    image: str,
```

## DeleteContainerServiceRequestRequestTypeDef

```python
# DeleteContainerServiceRequestRequestTypeDef definition

class DeleteContainerServiceRequestRequestTypeDef(TypedDict):
    serviceName: str,
```

## DeleteDiskRequestRequestTypeDef

```python
# DeleteDiskRequestRequestTypeDef definition

class DeleteDiskRequestRequestTypeDef(TypedDict):
    diskName: str,
    forceDeleteAddOns: NotRequired[bool],
```

## DeleteDiskSnapshotRequestRequestTypeDef

```python
# DeleteDiskSnapshotRequestRequestTypeDef definition

class DeleteDiskSnapshotRequestRequestTypeDef(TypedDict):
    diskSnapshotName: str,
```

## DeleteDistributionRequestRequestTypeDef

```python
# DeleteDistributionRequestRequestTypeDef definition

class DeleteDistributionRequestRequestTypeDef(TypedDict):
    distributionName: NotRequired[str],
```

## DeleteDomainRequestRequestTypeDef

```python
# DeleteDomainRequestRequestTypeDef definition

class DeleteDomainRequestRequestTypeDef(TypedDict):
    domainName: str,
```

## DeleteInstanceRequestRequestTypeDef

```python
# DeleteInstanceRequestRequestTypeDef definition

class DeleteInstanceRequestRequestTypeDef(TypedDict):
    instanceName: str,
    forceDeleteAddOns: NotRequired[bool],
```

## DeleteInstanceSnapshotRequestRequestTypeDef

```python
# DeleteInstanceSnapshotRequestRequestTypeDef definition

class DeleteInstanceSnapshotRequestRequestTypeDef(TypedDict):
    instanceSnapshotName: str,
```

## DeleteKeyPairRequestRequestTypeDef

```python
# DeleteKeyPairRequestRequestTypeDef definition

class DeleteKeyPairRequestRequestTypeDef(TypedDict):
    keyPairName: str,
    expectedFingerprint: NotRequired[str],
```

## DeleteKnownHostKeysRequestRequestTypeDef

```python
# DeleteKnownHostKeysRequestRequestTypeDef definition

class DeleteKnownHostKeysRequestRequestTypeDef(TypedDict):
    instanceName: str,
```

## DeleteLoadBalancerRequestRequestTypeDef

```python
# DeleteLoadBalancerRequestRequestTypeDef definition

class DeleteLoadBalancerRequestRequestTypeDef(TypedDict):
    loadBalancerName: str,
```

## DeleteLoadBalancerTlsCertificateRequestRequestTypeDef

```python
# DeleteLoadBalancerTlsCertificateRequestRequestTypeDef definition

class DeleteLoadBalancerTlsCertificateRequestRequestTypeDef(TypedDict):
    loadBalancerName: str,
    certificateName: str,
    force: NotRequired[bool],
```

## DeleteRelationalDatabaseRequestRequestTypeDef

```python
# DeleteRelationalDatabaseRequestRequestTypeDef definition

class DeleteRelationalDatabaseRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    skipFinalSnapshot: NotRequired[bool],
    finalRelationalDatabaseSnapshotName: NotRequired[str],
```

## DeleteRelationalDatabaseSnapshotRequestRequestTypeDef

```python
# DeleteRelationalDatabaseSnapshotRequestRequestTypeDef definition

class DeleteRelationalDatabaseSnapshotRequestRequestTypeDef(TypedDict):
    relationalDatabaseSnapshotName: str,
```

## DetachCertificateFromDistributionRequestRequestTypeDef

```python
# DetachCertificateFromDistributionRequestRequestTypeDef definition

class DetachCertificateFromDistributionRequestRequestTypeDef(TypedDict):
    distributionName: str,
```

## DetachDiskRequestRequestTypeDef

```python
# DetachDiskRequestRequestTypeDef definition

class DetachDiskRequestRequestTypeDef(TypedDict):
    diskName: str,
```

## DetachInstancesFromLoadBalancerRequestRequestTypeDef

```python
# DetachInstancesFromLoadBalancerRequestRequestTypeDef definition

class DetachInstancesFromLoadBalancerRequestRequestTypeDef(TypedDict):
    loadBalancerName: str,
    instanceNames: Sequence[str],
```

## DetachStaticIpRequestRequestTypeDef

```python
# DetachStaticIpRequestRequestTypeDef definition

class DetachStaticIpRequestRequestTypeDef(TypedDict):
    staticIpName: str,
```

## DisableAddOnRequestRequestTypeDef

```python
# DisableAddOnRequestRequestTypeDef definition

class DisableAddOnRequestRequestTypeDef(TypedDict):
    addOnType: AddOnTypeType,  # (1)
    resourceName: str,
```

1. See [:material-code-brackets: AddOnTypeType](./literals.md#addontypetype) 
## DiskInfoTypeDef

```python
# DiskInfoTypeDef definition

class DiskInfoTypeDef(TypedDict):
    name: NotRequired[str],
    path: NotRequired[str],
    sizeInGb: NotRequired[int],
    isSystemDisk: NotRequired[bool],
```

## DiskSnapshotInfoTypeDef

```python
# DiskSnapshotInfoTypeDef definition

class DiskSnapshotInfoTypeDef(TypedDict):
    sizeInGb: NotRequired[int],
```

## DistributionBundleTypeDef

```python
# DistributionBundleTypeDef definition

class DistributionBundleTypeDef(TypedDict):
    bundleId: NotRequired[str],
    name: NotRequired[str],
    price: NotRequired[float],
    transferPerMonthInGb: NotRequired[int],
    isActive: NotRequired[bool],
```

## DnsRecordCreationStateTypeDef

```python
# DnsRecordCreationStateTypeDef definition

class DnsRecordCreationStateTypeDef(TypedDict):
    code: NotRequired[DnsRecordCreationStateCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: DnsRecordCreationStateCodeType](./literals.md#dnsrecordcreationstatecodetype) 
## DomainEntryOutputTypeDef

```python
# DomainEntryOutputTypeDef definition

class DomainEntryOutputTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    target: NotRequired[str],
    isAlias: NotRequired[bool],
    type: NotRequired[str],
    options: NotRequired[Dict[str, str]],
```

## ResourceRecordTypeDef

```python
# ResourceRecordTypeDef definition

class ResourceRecordTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    value: NotRequired[str],
```

## TimePeriodTypeDef

```python
# TimePeriodTypeDef definition

class TimePeriodTypeDef(TypedDict):
    start: NotRequired[datetime],
    end: NotRequired[datetime],
```

## ExportSnapshotRequestRequestTypeDef

```python
# ExportSnapshotRequestRequestTypeDef definition

class ExportSnapshotRequestRequestTypeDef(TypedDict):
    sourceSnapshotName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetActiveNamesRequestRequestTypeDef

```python
# GetActiveNamesRequestRequestTypeDef definition

class GetActiveNamesRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetAlarmsRequestRequestTypeDef

```python
# GetAlarmsRequestRequestTypeDef definition

class GetAlarmsRequestRequestTypeDef(TypedDict):
    alarmName: NotRequired[str],
    pageToken: NotRequired[str],
    monitoredResourceName: NotRequired[str],
```

## GetAutoSnapshotsRequestRequestTypeDef

```python
# GetAutoSnapshotsRequestRequestTypeDef definition

class GetAutoSnapshotsRequestRequestTypeDef(TypedDict):
    resourceName: str,
```

## GetBlueprintsRequestRequestTypeDef

```python
# GetBlueprintsRequestRequestTypeDef definition

class GetBlueprintsRequestRequestTypeDef(TypedDict):
    includeInactive: NotRequired[bool],
    pageToken: NotRequired[str],
    appCategory: NotRequired[AppCategoryType],  # (1)
```

1. See [:material-code-brackets: AppCategoryType](./literals.md#appcategorytype) 
## GetBucketAccessKeysRequestRequestTypeDef

```python
# GetBucketAccessKeysRequestRequestTypeDef definition

class GetBucketAccessKeysRequestRequestTypeDef(TypedDict):
    bucketName: str,
```

## GetBucketBundlesRequestRequestTypeDef

```python
# GetBucketBundlesRequestRequestTypeDef definition

class GetBucketBundlesRequestRequestTypeDef(TypedDict):
    includeInactive: NotRequired[bool],
```

## MetricDatapointTypeDef

```python
# MetricDatapointTypeDef definition

class MetricDatapointTypeDef(TypedDict):
    average: NotRequired[float],
    maximum: NotRequired[float],
    minimum: NotRequired[float],
    sampleCount: NotRequired[float],
    sum: NotRequired[float],
    timestamp: NotRequired[datetime],
    unit: NotRequired[MetricUnitType],  # (1)
```

1. See [:material-code-brackets: MetricUnitType](./literals.md#metricunittype) 
## GetBucketsRequestRequestTypeDef

```python
# GetBucketsRequestRequestTypeDef definition

class GetBucketsRequestRequestTypeDef(TypedDict):
    bucketName: NotRequired[str],
    pageToken: NotRequired[str],
    includeConnectedResources: NotRequired[bool],
```

## GetBundlesRequestRequestTypeDef

```python
# GetBundlesRequestRequestTypeDef definition

class GetBundlesRequestRequestTypeDef(TypedDict):
    includeInactive: NotRequired[bool],
    pageToken: NotRequired[str],
    appCategory: NotRequired[AppCategoryType],  # (1)
```

1. See [:material-code-brackets: AppCategoryType](./literals.md#appcategorytype) 
## GetCertificatesRequestRequestTypeDef

```python
# GetCertificatesRequestRequestTypeDef definition

class GetCertificatesRequestRequestTypeDef(TypedDict):
    certificateStatuses: NotRequired[Sequence[CertificateStatusType]],  # (1)
    includeCertificateDetails: NotRequired[bool],
    certificateName: NotRequired[str],
    pageToken: NotRequired[str],
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
## GetCloudFormationStackRecordsRequestRequestTypeDef

```python
# GetCloudFormationStackRecordsRequestRequestTypeDef definition

class GetCloudFormationStackRecordsRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetContactMethodsRequestRequestTypeDef

```python
# GetContactMethodsRequestRequestTypeDef definition

class GetContactMethodsRequestRequestTypeDef(TypedDict):
    protocols: NotRequired[Sequence[ContactProtocolType]],  # (1)
```

1. See [:material-code-brackets: ContactProtocolType](./literals.md#contactprotocoltype) 
## GetContainerImagesRequestRequestTypeDef

```python
# GetContainerImagesRequestRequestTypeDef definition

class GetContainerImagesRequestRequestTypeDef(TypedDict):
    serviceName: str,
```

## GetContainerServiceDeploymentsRequestRequestTypeDef

```python
# GetContainerServiceDeploymentsRequestRequestTypeDef definition

class GetContainerServiceDeploymentsRequestRequestTypeDef(TypedDict):
    serviceName: str,
```

## GetContainerServicesRequestRequestTypeDef

```python
# GetContainerServicesRequestRequestTypeDef definition

class GetContainerServicesRequestRequestTypeDef(TypedDict):
    serviceName: NotRequired[str],
```

## GetDiskRequestRequestTypeDef

```python
# GetDiskRequestRequestTypeDef definition

class GetDiskRequestRequestTypeDef(TypedDict):
    diskName: str,
```

## GetDiskSnapshotRequestRequestTypeDef

```python
# GetDiskSnapshotRequestRequestTypeDef definition

class GetDiskSnapshotRequestRequestTypeDef(TypedDict):
    diskSnapshotName: str,
```

## GetDiskSnapshotsRequestRequestTypeDef

```python
# GetDiskSnapshotsRequestRequestTypeDef definition

class GetDiskSnapshotsRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetDisksRequestRequestTypeDef

```python
# GetDisksRequestRequestTypeDef definition

class GetDisksRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetDistributionLatestCacheResetRequestRequestTypeDef

```python
# GetDistributionLatestCacheResetRequestRequestTypeDef definition

class GetDistributionLatestCacheResetRequestRequestTypeDef(TypedDict):
    distributionName: NotRequired[str],
```

## GetDistributionsRequestRequestTypeDef

```python
# GetDistributionsRequestRequestTypeDef definition

class GetDistributionsRequestRequestTypeDef(TypedDict):
    distributionName: NotRequired[str],
    pageToken: NotRequired[str],
```

## GetDomainRequestRequestTypeDef

```python
# GetDomainRequestRequestTypeDef definition

class GetDomainRequestRequestTypeDef(TypedDict):
    domainName: str,
```

## GetDomainsRequestRequestTypeDef

```python
# GetDomainsRequestRequestTypeDef definition

class GetDomainsRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetExportSnapshotRecordsRequestRequestTypeDef

```python
# GetExportSnapshotRecordsRequestRequestTypeDef definition

class GetExportSnapshotRecordsRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetInstanceAccessDetailsRequestRequestTypeDef

```python
# GetInstanceAccessDetailsRequestRequestTypeDef definition

class GetInstanceAccessDetailsRequestRequestTypeDef(TypedDict):
    instanceName: str,
    protocol: NotRequired[InstanceAccessProtocolType],  # (1)
```

1. See [:material-code-brackets: InstanceAccessProtocolType](./literals.md#instanceaccessprotocoltype) 
## GetInstancePortStatesRequestRequestTypeDef

```python
# GetInstancePortStatesRequestRequestTypeDef definition

class GetInstancePortStatesRequestRequestTypeDef(TypedDict):
    instanceName: str,
```

## InstancePortStateTypeDef

```python
# InstancePortStateTypeDef definition

class InstancePortStateTypeDef(TypedDict):
    fromPort: NotRequired[int],
    toPort: NotRequired[int],
    protocol: NotRequired[NetworkProtocolType],  # (1)
    state: NotRequired[PortStateType],  # (2)
    cidrs: NotRequired[List[str]],
    ipv6Cidrs: NotRequired[List[str]],
    cidrListAliases: NotRequired[List[str]],
```

1. See [:material-code-brackets: NetworkProtocolType](./literals.md#networkprotocoltype) 
2. See [:material-code-brackets: PortStateType](./literals.md#portstatetype) 
## GetInstanceRequestRequestTypeDef

```python
# GetInstanceRequestRequestTypeDef definition

class GetInstanceRequestRequestTypeDef(TypedDict):
    instanceName: str,
```

## GetInstanceSnapshotRequestRequestTypeDef

```python
# GetInstanceSnapshotRequestRequestTypeDef definition

class GetInstanceSnapshotRequestRequestTypeDef(TypedDict):
    instanceSnapshotName: str,
```

## GetInstanceSnapshotsRequestRequestTypeDef

```python
# GetInstanceSnapshotsRequestRequestTypeDef definition

class GetInstanceSnapshotsRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetInstanceStateRequestRequestTypeDef

```python
# GetInstanceStateRequestRequestTypeDef definition

class GetInstanceStateRequestRequestTypeDef(TypedDict):
    instanceName: str,
```

## InstanceStateTypeDef

```python
# InstanceStateTypeDef definition

class InstanceStateTypeDef(TypedDict):
    code: NotRequired[int],
    name: NotRequired[str],
```

## GetInstancesRequestRequestTypeDef

```python
# GetInstancesRequestRequestTypeDef definition

class GetInstancesRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetKeyPairRequestRequestTypeDef

```python
# GetKeyPairRequestRequestTypeDef definition

class GetKeyPairRequestRequestTypeDef(TypedDict):
    keyPairName: str,
```

## GetKeyPairsRequestRequestTypeDef

```python
# GetKeyPairsRequestRequestTypeDef definition

class GetKeyPairsRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
    includeDefaultKeyPair: NotRequired[bool],
```

## GetLoadBalancerRequestRequestTypeDef

```python
# GetLoadBalancerRequestRequestTypeDef definition

class GetLoadBalancerRequestRequestTypeDef(TypedDict):
    loadBalancerName: str,
```

## GetLoadBalancerTlsCertificatesRequestRequestTypeDef

```python
# GetLoadBalancerTlsCertificatesRequestRequestTypeDef definition

class GetLoadBalancerTlsCertificatesRequestRequestTypeDef(TypedDict):
    loadBalancerName: str,
```

## GetLoadBalancerTlsPoliciesRequestRequestTypeDef

```python
# GetLoadBalancerTlsPoliciesRequestRequestTypeDef definition

class GetLoadBalancerTlsPoliciesRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## LoadBalancerTlsPolicyTypeDef

```python
# LoadBalancerTlsPolicyTypeDef definition

class LoadBalancerTlsPolicyTypeDef(TypedDict):
    name: NotRequired[str],
    isDefault: NotRequired[bool],
    description: NotRequired[str],
    protocols: NotRequired[List[str]],
    ciphers: NotRequired[List[str]],
```

## GetLoadBalancersRequestRequestTypeDef

```python
# GetLoadBalancersRequestRequestTypeDef definition

class GetLoadBalancersRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetOperationRequestRequestTypeDef

```python
# GetOperationRequestRequestTypeDef definition

class GetOperationRequestRequestTypeDef(TypedDict):
    operationId: str,
```

## GetOperationsForResourceRequestRequestTypeDef

```python
# GetOperationsForResourceRequestRequestTypeDef definition

class GetOperationsForResourceRequestRequestTypeDef(TypedDict):
    resourceName: str,
    pageToken: NotRequired[str],
```

## GetOperationsRequestRequestTypeDef

```python
# GetOperationsRequestRequestTypeDef definition

class GetOperationsRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetRegionsRequestRequestTypeDef

```python
# GetRegionsRequestRequestTypeDef definition

class GetRegionsRequestRequestTypeDef(TypedDict):
    includeAvailabilityZones: NotRequired[bool],
    includeRelationalDatabaseAvailabilityZones: NotRequired[bool],
```

## GetRelationalDatabaseBlueprintsRequestRequestTypeDef

```python
# GetRelationalDatabaseBlueprintsRequestRequestTypeDef definition

class GetRelationalDatabaseBlueprintsRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## RelationalDatabaseBlueprintTypeDef

```python
# RelationalDatabaseBlueprintTypeDef definition

class RelationalDatabaseBlueprintTypeDef(TypedDict):
    blueprintId: NotRequired[str],
    engine: NotRequired[RelationalDatabaseEngineType],  # (1)
    engineVersion: NotRequired[str],
    engineDescription: NotRequired[str],
    engineVersionDescription: NotRequired[str],
    isEngineDefault: NotRequired[bool],
```

1. See [:material-code-brackets: RelationalDatabaseEngineType](./literals.md#relationaldatabaseenginetype) 
## GetRelationalDatabaseBundlesRequestRequestTypeDef

```python
# GetRelationalDatabaseBundlesRequestRequestTypeDef definition

class GetRelationalDatabaseBundlesRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
    includeInactive: NotRequired[bool],
```

## RelationalDatabaseBundleTypeDef

```python
# RelationalDatabaseBundleTypeDef definition

class RelationalDatabaseBundleTypeDef(TypedDict):
    bundleId: NotRequired[str],
    name: NotRequired[str],
    price: NotRequired[float],
    ramSizeInGb: NotRequired[float],
    diskSizeInGb: NotRequired[int],
    transferPerMonthInGb: NotRequired[int],
    cpuCount: NotRequired[int],
    isEncrypted: NotRequired[bool],
    isActive: NotRequired[bool],
```

## GetRelationalDatabaseEventsRequestRequestTypeDef

```python
# GetRelationalDatabaseEventsRequestRequestTypeDef definition

class GetRelationalDatabaseEventsRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    durationInMinutes: NotRequired[int],
    pageToken: NotRequired[str],
```

## RelationalDatabaseEventTypeDef

```python
# RelationalDatabaseEventTypeDef definition

class RelationalDatabaseEventTypeDef(TypedDict):
    resource: NotRequired[str],
    createdAt: NotRequired[datetime],
    message: NotRequired[str],
    eventCategories: NotRequired[List[str]],
```

## LogEventTypeDef

```python
# LogEventTypeDef definition

class LogEventTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    message: NotRequired[str],
```

## GetRelationalDatabaseLogStreamsRequestRequestTypeDef

```python
# GetRelationalDatabaseLogStreamsRequestRequestTypeDef definition

class GetRelationalDatabaseLogStreamsRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
```

## GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef

```python
# GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef definition

class GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    passwordVersion: NotRequired[RelationalDatabasePasswordVersionType],  # (1)
```

1. See [:material-code-brackets: RelationalDatabasePasswordVersionType](./literals.md#relationaldatabasepasswordversiontype) 
## GetRelationalDatabaseParametersRequestRequestTypeDef

```python
# GetRelationalDatabaseParametersRequestRequestTypeDef definition

class GetRelationalDatabaseParametersRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    pageToken: NotRequired[str],
```

## RelationalDatabaseParameterTypeDef

```python
# RelationalDatabaseParameterTypeDef definition

class RelationalDatabaseParameterTypeDef(TypedDict):
    allowedValues: NotRequired[str],
    applyMethod: NotRequired[str],
    applyType: NotRequired[str],
    dataType: NotRequired[str],
    description: NotRequired[str],
    isModifiable: NotRequired[bool],
    parameterName: NotRequired[str],
    parameterValue: NotRequired[str],
```

## GetRelationalDatabaseRequestRequestTypeDef

```python
# GetRelationalDatabaseRequestRequestTypeDef definition

class GetRelationalDatabaseRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
```

## GetRelationalDatabaseSnapshotRequestRequestTypeDef

```python
# GetRelationalDatabaseSnapshotRequestRequestTypeDef definition

class GetRelationalDatabaseSnapshotRequestRequestTypeDef(TypedDict):
    relationalDatabaseSnapshotName: str,
```

## GetRelationalDatabaseSnapshotsRequestRequestTypeDef

```python
# GetRelationalDatabaseSnapshotsRequestRequestTypeDef definition

class GetRelationalDatabaseSnapshotsRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetRelationalDatabasesRequestRequestTypeDef

```python
# GetRelationalDatabasesRequestRequestTypeDef definition

class GetRelationalDatabasesRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## GetSetupHistoryRequestRequestTypeDef

```python
# GetSetupHistoryRequestRequestTypeDef definition

class GetSetupHistoryRequestRequestTypeDef(TypedDict):
    resourceName: str,
    pageToken: NotRequired[str],
```

## GetStaticIpRequestRequestTypeDef

```python
# GetStaticIpRequestRequestTypeDef definition

class GetStaticIpRequestRequestTypeDef(TypedDict):
    staticIpName: str,
```

## GetStaticIpsRequestRequestTypeDef

```python
# GetStaticIpsRequestRequestTypeDef definition

class GetStaticIpsRequestRequestTypeDef(TypedDict):
    pageToken: NotRequired[str],
```

## HeaderObjectTypeDef

```python
# HeaderObjectTypeDef definition

class HeaderObjectTypeDef(TypedDict):
    option: NotRequired[ForwardValuesType],  # (1)
    headersAllowList: NotRequired[Sequence[HeaderEnumType]],  # (2)
```

1. See [:material-code-brackets: ForwardValuesType](./literals.md#forwardvaluestype) 
2. See [:material-code-brackets: HeaderEnumType](./literals.md#headerenumtype) 
## HostKeyAttributesTypeDef

```python
# HostKeyAttributesTypeDef definition

class HostKeyAttributesTypeDef(TypedDict):
    algorithm: NotRequired[str],
    publicKey: NotRequired[str],
    witnessedAt: NotRequired[datetime],
    fingerprintSHA1: NotRequired[str],
    fingerprintSHA256: NotRequired[str],
    notValidBefore: NotRequired[datetime],
    notValidAfter: NotRequired[datetime],
```

## ImportKeyPairRequestRequestTypeDef

```python
# ImportKeyPairRequestRequestTypeDef definition

class ImportKeyPairRequestRequestTypeDef(TypedDict):
    keyPairName: str,
    publicKeyBase64: str,
```

## PasswordDataTypeDef

```python
# PasswordDataTypeDef definition

class PasswordDataTypeDef(TypedDict):
    ciphertext: NotRequired[str],
    keyPairName: NotRequired[str],
```

## InstanceHealthSummaryTypeDef

```python
# InstanceHealthSummaryTypeDef definition

class InstanceHealthSummaryTypeDef(TypedDict):
    instanceName: NotRequired[str],
    instanceHealth: NotRequired[InstanceHealthStateType],  # (1)
    instanceHealthReason: NotRequired[InstanceHealthReasonType],  # (2)
```

1. See [:material-code-brackets: InstanceHealthStateType](./literals.md#instancehealthstatetype) 
2. See [:material-code-brackets: InstanceHealthReasonType](./literals.md#instancehealthreasontype) 
## InstanceMetadataOptionsTypeDef

```python
# InstanceMetadataOptionsTypeDef definition

class InstanceMetadataOptionsTypeDef(TypedDict):
    state: NotRequired[InstanceMetadataStateType],  # (1)
    httpTokens: NotRequired[HttpTokensType],  # (2)
    httpEndpoint: NotRequired[HttpEndpointType],  # (3)
    httpPutResponseHopLimit: NotRequired[int],
    httpProtocolIpv6: NotRequired[HttpProtocolIpv6Type],  # (4)
```

1. See [:material-code-brackets: InstanceMetadataStateType](./literals.md#instancemetadatastatetype) 
2. See [:material-code-brackets: HttpTokensType](./literals.md#httptokenstype) 
3. See [:material-code-brackets: HttpEndpointType](./literals.md#httpendpointtype) 
4. See [:material-code-brackets: HttpProtocolIpv6Type](./literals.md#httpprotocolipv6type) 
## InstancePortInfoTypeDef

```python
# InstancePortInfoTypeDef definition

class InstancePortInfoTypeDef(TypedDict):
    fromPort: NotRequired[int],
    toPort: NotRequired[int],
    protocol: NotRequired[NetworkProtocolType],  # (1)
    accessFrom: NotRequired[str],
    accessType: NotRequired[PortAccessTypeType],  # (2)
    commonName: NotRequired[str],
    accessDirection: NotRequired[AccessDirectionType],  # (3)
    cidrs: NotRequired[List[str]],
    ipv6Cidrs: NotRequired[List[str]],
    cidrListAliases: NotRequired[List[str]],
```

1. See [:material-code-brackets: NetworkProtocolType](./literals.md#networkprotocoltype) 
2. See [:material-code-brackets: PortAccessTypeType](./literals.md#portaccesstypetype) 
3. See [:material-code-brackets: AccessDirectionType](./literals.md#accessdirectiontype) 
## MonthlyTransferTypeDef

```python
# MonthlyTransferTypeDef definition

class MonthlyTransferTypeDef(TypedDict):
    gbPerMonthAllocated: NotRequired[int],
```

## OriginTypeDef

```python
# OriginTypeDef definition

class OriginTypeDef(TypedDict):
    name: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (1)
    regionName: NotRequired[RegionNameType],  # (2)
    protocolPolicy: NotRequired[OriginProtocolPolicyEnumType],  # (3)
    responseTimeout: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: RegionNameType](./literals.md#regionnametype) 
3. See [:material-code-brackets: OriginProtocolPolicyEnumType](./literals.md#originprotocolpolicyenumtype) 
## LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef

```python
# LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef definition

class LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef(TypedDict):
    code: NotRequired[LoadBalancerTlsCertificateDnsRecordCreationStateCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: LoadBalancerTlsCertificateDnsRecordCreationStateCodeType](./literals.md#loadbalancertlscertificatednsrecordcreationstatecodetype) 
## LoadBalancerTlsCertificateDomainValidationOptionTypeDef

```python
# LoadBalancerTlsCertificateDomainValidationOptionTypeDef definition

class LoadBalancerTlsCertificateDomainValidationOptionTypeDef(TypedDict):
    domainName: NotRequired[str],
    validationStatus: NotRequired[LoadBalancerTlsCertificateDomainStatusType],  # (1)
```

1. See [:material-code-brackets: LoadBalancerTlsCertificateDomainStatusType](./literals.md#loadbalancertlscertificatedomainstatustype) 
## LoadBalancerTlsCertificateSummaryTypeDef

```python
# LoadBalancerTlsCertificateSummaryTypeDef definition

class LoadBalancerTlsCertificateSummaryTypeDef(TypedDict):
    name: NotRequired[str],
    isAttached: NotRequired[bool],
```

## NameServersUpdateStateTypeDef

```python
# NameServersUpdateStateTypeDef definition

class NameServersUpdateStateTypeDef(TypedDict):
    code: NotRequired[NameServersUpdateStateCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: NameServersUpdateStateCodeType](./literals.md#nameserversupdatestatecodetype) 
## PendingMaintenanceActionTypeDef

```python
# PendingMaintenanceActionTypeDef definition

class PendingMaintenanceActionTypeDef(TypedDict):
    action: NotRequired[str],
    description: NotRequired[str],
    currentApplyDate: NotRequired[datetime],
```

## PendingModifiedRelationalDatabaseValuesTypeDef

```python
# PendingModifiedRelationalDatabaseValuesTypeDef definition

class PendingModifiedRelationalDatabaseValuesTypeDef(TypedDict):
    masterUserPassword: NotRequired[str],
    engineVersion: NotRequired[str],
    backupRetentionEnabled: NotRequired[bool],
```

## PutAlarmRequestRequestTypeDef

```python
# PutAlarmRequestRequestTypeDef definition

class PutAlarmRequestRequestTypeDef(TypedDict):
    alarmName: str,
    metricName: MetricNameType,  # (1)
    monitoredResourceName: str,
    comparisonOperator: ComparisonOperatorType,  # (2)
    threshold: float,
    evaluationPeriods: int,
    datapointsToAlarm: NotRequired[int],
    treatMissingData: NotRequired[TreatMissingDataType],  # (3)
    contactProtocols: NotRequired[Sequence[ContactProtocolType]],  # (4)
    notificationTriggers: NotRequired[Sequence[AlarmStateType]],  # (5)
    notificationEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: MetricNameType](./literals.md#metricnametype) 
2. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
3. See [:material-code-brackets: TreatMissingDataType](./literals.md#treatmissingdatatype) 
4. See [:material-code-brackets: ContactProtocolType](./literals.md#contactprotocoltype) 
5. See [:material-code-brackets: AlarmStateType](./literals.md#alarmstatetype) 
## QueryStringObjectTypeDef

```python
# QueryStringObjectTypeDef definition

class QueryStringObjectTypeDef(TypedDict):
    option: NotRequired[bool],
    queryStringsAllowList: NotRequired[Sequence[str]],
```

## R53HostedZoneDeletionStateTypeDef

```python
# R53HostedZoneDeletionStateTypeDef definition

class R53HostedZoneDeletionStateTypeDef(TypedDict):
    code: NotRequired[R53HostedZoneDeletionStateCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: R53HostedZoneDeletionStateCodeType](./literals.md#r53hostedzonedeletionstatecodetype) 
## RebootInstanceRequestRequestTypeDef

```python
# RebootInstanceRequestRequestTypeDef definition

class RebootInstanceRequestRequestTypeDef(TypedDict):
    instanceName: str,
```

## RebootRelationalDatabaseRequestRequestTypeDef

```python
# RebootRelationalDatabaseRequestRequestTypeDef definition

class RebootRelationalDatabaseRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
```

## RegisterContainerImageRequestRequestTypeDef

```python
# RegisterContainerImageRequestRequestTypeDef definition

class RegisterContainerImageRequestRequestTypeDef(TypedDict):
    serviceName: str,
    label: str,
    digest: str,
```

## RelationalDatabaseEndpointTypeDef

```python
# RelationalDatabaseEndpointTypeDef definition

class RelationalDatabaseEndpointTypeDef(TypedDict):
    port: NotRequired[int],
    address: NotRequired[str],
```

## RelationalDatabaseHardwareTypeDef

```python
# RelationalDatabaseHardwareTypeDef definition

class RelationalDatabaseHardwareTypeDef(TypedDict):
    cpuCount: NotRequired[int],
    diskSizeInGb: NotRequired[int],
    ramSizeInGb: NotRequired[float],
```

## ReleaseStaticIpRequestRequestTypeDef

```python
# ReleaseStaticIpRequestRequestTypeDef definition

class ReleaseStaticIpRequestRequestTypeDef(TypedDict):
    staticIpName: str,
```

## ResetDistributionCacheRequestRequestTypeDef

```python
# ResetDistributionCacheRequestRequestTypeDef definition

class ResetDistributionCacheRequestRequestTypeDef(TypedDict):
    distributionName: NotRequired[str],
```

## SendContactMethodVerificationRequestRequestTypeDef

```python
# SendContactMethodVerificationRequestRequestTypeDef definition

class SendContactMethodVerificationRequestRequestTypeDef(TypedDict):
    protocol: ContactMethodVerificationProtocolType,  # (1)
```

1. See [:material-code-brackets: ContactMethodVerificationProtocolType](./literals.md#contactmethodverificationprotocoltype) 
## SetIpAddressTypeRequestRequestTypeDef

```python
# SetIpAddressTypeRequestRequestTypeDef definition

class SetIpAddressTypeRequestRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    resourceName: str,
    ipAddressType: IpAddressTypeType,  # (2)
    acceptBundleUpdate: NotRequired[bool],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
## SetResourceAccessForBucketRequestRequestTypeDef

```python
# SetResourceAccessForBucketRequestRequestTypeDef definition

class SetResourceAccessForBucketRequestRequestTypeDef(TypedDict):
    resourceName: str,
    bucketName: str,
    access: ResourceBucketAccessType,  # (1)
```

1. See [:material-code-brackets: ResourceBucketAccessType](./literals.md#resourcebucketaccesstype) 
## SetupExecutionDetailsTypeDef

```python
# SetupExecutionDetailsTypeDef definition

class SetupExecutionDetailsTypeDef(TypedDict):
    command: NotRequired[str],
    dateTime: NotRequired[datetime],
    name: NotRequired[str],
    status: NotRequired[SetupStatusType],  # (1)
    standardError: NotRequired[str],
    standardOutput: NotRequired[str],
    version: NotRequired[str],
```

1. See [:material-code-brackets: SetupStatusType](./literals.md#setupstatustype) 
## SetupRequestTypeDef

```python
# SetupRequestTypeDef definition

class SetupRequestTypeDef(TypedDict):
    instanceName: NotRequired[str],
    domainNames: NotRequired[List[str]],
    certificateProvider: NotRequired[CertificateProviderType],  # (1)
```

1. See [:material-code-brackets: CertificateProviderType](./literals.md#certificateprovidertype) 
## SetupInstanceHttpsRequestRequestTypeDef

```python
# SetupInstanceHttpsRequestRequestTypeDef definition

class SetupInstanceHttpsRequestRequestTypeDef(TypedDict):
    instanceName: str,
    emailAddress: str,
    domainNames: Sequence[str],
    certificateProvider: CertificateProviderType,  # (1)
```

1. See [:material-code-brackets: CertificateProviderType](./literals.md#certificateprovidertype) 
## StartGUISessionRequestRequestTypeDef

```python
# StartGUISessionRequestRequestTypeDef definition

class StartGUISessionRequestRequestTypeDef(TypedDict):
    resourceName: str,
```

## StartInstanceRequestRequestTypeDef

```python
# StartInstanceRequestRequestTypeDef definition

class StartInstanceRequestRequestTypeDef(TypedDict):
    instanceName: str,
```

## StartRelationalDatabaseRequestRequestTypeDef

```python
# StartRelationalDatabaseRequestRequestTypeDef definition

class StartRelationalDatabaseRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
```

## StopGUISessionRequestRequestTypeDef

```python
# StopGUISessionRequestRequestTypeDef definition

class StopGUISessionRequestRequestTypeDef(TypedDict):
    resourceName: str,
```

## StopInstanceRequestRequestTypeDef

```python
# StopInstanceRequestRequestTypeDef definition

class StopInstanceRequestRequestTypeDef(TypedDict):
    instanceName: str,
    force: NotRequired[bool],
```

## StopRelationalDatabaseRequestRequestTypeDef

```python
# StopRelationalDatabaseRequestRequestTypeDef definition

class StopRelationalDatabaseRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    relationalDatabaseSnapshotName: NotRequired[str],
```

## TestAlarmRequestRequestTypeDef

```python
# TestAlarmRequestRequestTypeDef definition

class TestAlarmRequestRequestTypeDef(TypedDict):
    alarmName: str,
    state: AlarmStateType,  # (1)
```

1. See [:material-code-brackets: AlarmStateType](./literals.md#alarmstatetype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceName: str,
    tagKeys: Sequence[str],
    resourceArn: NotRequired[str],
```

## UpdateBucketBundleRequestRequestTypeDef

```python
# UpdateBucketBundleRequestRequestTypeDef definition

class UpdateBucketBundleRequestRequestTypeDef(TypedDict):
    bucketName: str,
    bundleId: str,
```

## UpdateDistributionBundleRequestRequestTypeDef

```python
# UpdateDistributionBundleRequestRequestTypeDef definition

class UpdateDistributionBundleRequestRequestTypeDef(TypedDict):
    distributionName: NotRequired[str],
    bundleId: NotRequired[str],
```

## UpdateInstanceMetadataOptionsRequestRequestTypeDef

```python
# UpdateInstanceMetadataOptionsRequestRequestTypeDef definition

class UpdateInstanceMetadataOptionsRequestRequestTypeDef(TypedDict):
    instanceName: str,
    httpTokens: NotRequired[HttpTokensType],  # (1)
    httpEndpoint: NotRequired[HttpEndpointType],  # (2)
    httpPutResponseHopLimit: NotRequired[int],
    httpProtocolIpv6: NotRequired[HttpProtocolIpv6Type],  # (3)
```

1. See [:material-code-brackets: HttpTokensType](./literals.md#httptokenstype) 
2. See [:material-code-brackets: HttpEndpointType](./literals.md#httpendpointtype) 
3. See [:material-code-brackets: HttpProtocolIpv6Type](./literals.md#httpprotocolipv6type) 
## UpdateLoadBalancerAttributeRequestRequestTypeDef

```python
# UpdateLoadBalancerAttributeRequestRequestTypeDef definition

class UpdateLoadBalancerAttributeRequestRequestTypeDef(TypedDict):
    loadBalancerName: str,
    attributeName: LoadBalancerAttributeNameType,  # (1)
    attributeValue: str,
```

1. See [:material-code-brackets: LoadBalancerAttributeNameType](./literals.md#loadbalancerattributenametype) 
## UpdateRelationalDatabaseRequestRequestTypeDef

```python
# UpdateRelationalDatabaseRequestRequestTypeDef definition

class UpdateRelationalDatabaseRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    masterUserPassword: NotRequired[str],
    rotateMasterUserPassword: NotRequired[bool],
    preferredBackupWindow: NotRequired[str],
    preferredMaintenanceWindow: NotRequired[str],
    enableBackupRetention: NotRequired[bool],
    disableBackupRetention: NotRequired[bool],
    publiclyAccessible: NotRequired[bool],
    applyImmediately: NotRequired[bool],
    caCertificateIdentifier: NotRequired[str],
    relationalDatabaseBlueprintId: NotRequired[str],
```

## AccessKeyTypeDef

```python
# AccessKeyTypeDef definition

class AccessKeyTypeDef(TypedDict):
    accessKeyId: NotRequired[str],
    secretAccessKey: NotRequired[str],
    status: NotRequired[StatusTypeType],  # (1)
    createdAt: NotRequired[datetime],
    lastUsed: NotRequired[AccessKeyLastUsedTypeDef],  # (2)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
2. See [:material-code-braces: AccessKeyLastUsedTypeDef](./type_defs.md#accesskeylastusedtypedef) 
## AddOnRequestTypeDef

```python
# AddOnRequestTypeDef definition

class AddOnRequestTypeDef(TypedDict):
    addOnType: AddOnTypeType,  # (1)
    autoSnapshotAddOnRequest: NotRequired[AutoSnapshotAddOnRequestTypeDef],  # (2)
    stopInstanceOnIdleRequest: NotRequired[StopInstanceOnIdleRequestTypeDef],  # (3)
```

1. See [:material-code-brackets: AddOnTypeType](./literals.md#addontypetype) 
2. See [:material-code-braces: AutoSnapshotAddOnRequestTypeDef](./type_defs.md#autosnapshotaddonrequesttypedef) 
3. See [:material-code-braces: StopInstanceOnIdleRequestTypeDef](./type_defs.md#stopinstanceonidlerequesttypedef) 
## AlarmTypeDef

```python
# AlarmTypeDef definition

class AlarmTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    supportCode: NotRequired[str],
    monitoredResourceInfo: NotRequired[MonitoredResourceInfoTypeDef],  # (3)
    comparisonOperator: NotRequired[ComparisonOperatorType],  # (4)
    evaluationPeriods: NotRequired[int],
    period: NotRequired[int],
    threshold: NotRequired[float],
    datapointsToAlarm: NotRequired[int],
    treatMissingData: NotRequired[TreatMissingDataType],  # (5)
    statistic: NotRequired[MetricStatisticType],  # (6)
    metricName: NotRequired[MetricNameType],  # (7)
    state: NotRequired[AlarmStateType],  # (8)
    unit: NotRequired[MetricUnitType],  # (9)
    contactProtocols: NotRequired[List[ContactProtocolType]],  # (10)
    notificationTriggers: NotRequired[List[AlarmStateType]],  # (11)
    notificationEnabled: NotRequired[bool],
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: MonitoredResourceInfoTypeDef](./type_defs.md#monitoredresourceinfotypedef) 
4. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
5. See [:material-code-brackets: TreatMissingDataType](./literals.md#treatmissingdatatype) 
6. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
7. See [:material-code-brackets: MetricNameType](./literals.md#metricnametype) 
8. See [:material-code-brackets: AlarmStateType](./literals.md#alarmstatetype) 
9. See [:material-code-brackets: MetricUnitType](./literals.md#metricunittype) 
10. See [:material-code-brackets: ContactProtocolType](./literals.md#contactprotocoltype) 
11. See [:material-code-brackets: AlarmStateType](./literals.md#alarmstatetype) 
## ContactMethodTypeDef

```python
# ContactMethodTypeDef definition

class ContactMethodTypeDef(TypedDict):
    contactEndpoint: NotRequired[str],
    status: NotRequired[ContactMethodStatusType],  # (1)
    protocol: NotRequired[ContactProtocolType],  # (2)
    name: NotRequired[str],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (3)
    resourceType: NotRequired[ResourceTypeType],  # (4)
    supportCode: NotRequired[str],
```

1. See [:material-code-brackets: ContactMethodStatusType](./literals.md#contactmethodstatustype) 
2. See [:material-code-brackets: ContactProtocolType](./literals.md#contactprotocoltype) 
3. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
4. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## OperationTypeDef

```python
# OperationTypeDef definition

class OperationTypeDef(TypedDict):
    id: NotRequired[str],
    resourceName: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (1)
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (2)
    isTerminal: NotRequired[bool],
    operationDetails: NotRequired[str],
    operationType: NotRequired[OperationTypeType],  # (3)
    status: NotRequired[OperationStatusType],  # (4)
    statusChangedAt: NotRequired[datetime],
    errorCode: NotRequired[str],
    errorDetails: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
3. See [:material-code-brackets: OperationTypeType](./literals.md#operationtypetype) 
4. See [:material-code-brackets: OperationStatusType](./literals.md#operationstatustype) 
## SetupHistoryResourceTypeDef

```python
# SetupHistoryResourceTypeDef definition

class SetupHistoryResourceTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## StaticIpTypeDef

```python
# StaticIpTypeDef definition

class StaticIpTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    ipAddress: NotRequired[str],
    attachedTo: NotRequired[str],
    isAttached: NotRequired[bool],
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## DownloadDefaultKeyPairResultTypeDef

```python
# DownloadDefaultKeyPairResultTypeDef definition

class DownloadDefaultKeyPairResultTypeDef(TypedDict):
    publicKeyBase64: str,
    privateKeyBase64: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetActiveNamesResultTypeDef

```python
# GetActiveNamesResultTypeDef definition

class GetActiveNamesResultTypeDef(TypedDict):
    activeNames: List[str],
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContainerAPIMetadataResultTypeDef

```python
# GetContainerAPIMetadataResultTypeDef definition

class GetContainerAPIMetadataResultTypeDef(TypedDict):
    metadata: List[Dict[str, str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDistributionLatestCacheResetResultTypeDef

```python
# GetDistributionLatestCacheResetResultTypeDef definition

class GetDistributionLatestCacheResetResultTypeDef(TypedDict):
    status: str,
    createTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRelationalDatabaseLogStreamsResultTypeDef

```python
# GetRelationalDatabaseLogStreamsResultTypeDef definition

class GetRelationalDatabaseLogStreamsResultTypeDef(TypedDict):
    logStreams: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRelationalDatabaseMasterUserPasswordResultTypeDef

```python
# GetRelationalDatabaseMasterUserPasswordResultTypeDef definition

class GetRelationalDatabaseMasterUserPasswordResultTypeDef(TypedDict):
    masterUserPassword: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IsVpcPeeredResultTypeDef

```python
# IsVpcPeeredResultTypeDef definition

class IsVpcPeeredResultTypeDef(TypedDict):
    isPeered: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoSnapshotDetailsTypeDef

```python
# AutoSnapshotDetailsTypeDef definition

class AutoSnapshotDetailsTypeDef(TypedDict):
    date: NotRequired[str],
    createdAt: NotRequired[datetime],
    status: NotRequired[AutoSnapshotStatusType],  # (1)
    fromAttachedDisks: NotRequired[List[AttachedDiskTypeDef]],  # (2)
```

1. See [:material-code-brackets: AutoSnapshotStatusType](./literals.md#autosnapshotstatustype) 
2. See [:material-code-braces: AttachedDiskTypeDef](./type_defs.md#attacheddisktypedef) 
## RegionTypeDef

```python
# RegionTypeDef definition

class RegionTypeDef(TypedDict):
    continentCode: NotRequired[str],
    description: NotRequired[str],
    displayName: NotRequired[str],
    name: NotRequired[RegionNameType],  # (1)
    availabilityZones: NotRequired[List[AvailabilityZoneTypeDef]],  # (2)
    relationalDatabaseAvailabilityZones: NotRequired[List[AvailabilityZoneTypeDef]],  # (2)
```

1. See [:material-code-brackets: RegionNameType](./literals.md#regionnametype) 
2. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
3. See [:material-code-braces: AvailabilityZoneTypeDef](./type_defs.md#availabilityzonetypedef) 
## GetBlueprintsResultTypeDef

```python
# GetBlueprintsResultTypeDef definition

class GetBlueprintsResultTypeDef(TypedDict):
    blueprints: List[BlueprintTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueprintTypeDef](./type_defs.md#blueprinttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBucketRequestRequestTypeDef

```python
# UpdateBucketRequestRequestTypeDef definition

class UpdateBucketRequestRequestTypeDef(TypedDict):
    bucketName: str,
    accessRules: NotRequired[AccessRulesTypeDef],  # (1)
    versioning: NotRequired[str],
    readonlyAccessAccounts: NotRequired[Sequence[str]],
    accessLogConfig: NotRequired[BucketAccessLogConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AccessRulesTypeDef](./type_defs.md#accessrulestypedef) 
2. See [:material-code-braces: BucketAccessLogConfigTypeDef](./type_defs.md#bucketaccesslogconfigtypedef) 
## GetBucketBundlesResultTypeDef

```python
# GetBucketBundlesResultTypeDef definition

class GetBucketBundlesResultTypeDef(TypedDict):
    bundles: List[BucketBundleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BucketBundleTypeDef](./type_defs.md#bucketbundletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BucketTypeDef

```python
# BucketTypeDef definition

class BucketTypeDef(TypedDict):
    resourceType: NotRequired[str],
    accessRules: NotRequired[AccessRulesTypeDef],  # (1)
    arn: NotRequired[str],
    bundleId: NotRequired[str],
    createdAt: NotRequired[datetime],
    url: NotRequired[str],
    location: NotRequired[ResourceLocationTypeDef],  # (2)
    name: NotRequired[str],
    supportCode: NotRequired[str],
    tags: NotRequired[List[TagTypeDef]],  # (3)
    objectVersioning: NotRequired[str],
    ableToUpdateBundle: NotRequired[bool],
    readonlyAccessAccounts: NotRequired[List[str]],
    resourcesReceivingAccess: NotRequired[List[ResourceReceivingAccessTypeDef]],  # (4)
    state: NotRequired[BucketStateTypeDef],  # (5)
    accessLogConfig: NotRequired[BucketAccessLogConfigTypeDef],  # (6)
```

1. See [:material-code-braces: AccessRulesTypeDef](./type_defs.md#accessrulestypedef) 
2. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ResourceReceivingAccessTypeDef](./type_defs.md#resourcereceivingaccesstypedef) 
5. See [:material-code-braces: BucketStateTypeDef](./type_defs.md#bucketstatetypedef) 
6. See [:material-code-braces: BucketAccessLogConfigTypeDef](./type_defs.md#bucketaccesslogconfigtypedef) 
## CreateBucketRequestRequestTypeDef

```python
# CreateBucketRequestRequestTypeDef definition

class CreateBucketRequestRequestTypeDef(TypedDict):
    bucketName: str,
    bundleId: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    enableObjectVersioning: NotRequired[bool],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCertificateRequestRequestTypeDef

```python
# CreateCertificateRequestRequestTypeDef definition

class CreateCertificateRequestRequestTypeDef(TypedDict):
    certificateName: str,
    domainName: str,
    subjectAlternativeNames: NotRequired[Sequence[str]],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDiskSnapshotRequestRequestTypeDef

```python
# CreateDiskSnapshotRequestRequestTypeDef definition

class CreateDiskSnapshotRequestRequestTypeDef(TypedDict):
    diskSnapshotName: str,
    diskName: NotRequired[str],
    instanceName: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDomainRequestRequestTypeDef

```python
# CreateDomainRequestRequestTypeDef definition

class CreateDomainRequestRequestTypeDef(TypedDict):
    domainName: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateInstanceSnapshotRequestRequestTypeDef

```python
# CreateInstanceSnapshotRequestRequestTypeDef definition

class CreateInstanceSnapshotRequestRequestTypeDef(TypedDict):
    instanceSnapshotName: str,
    instanceName: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateKeyPairRequestRequestTypeDef

```python
# CreateKeyPairRequestRequestTypeDef definition

class CreateKeyPairRequestRequestTypeDef(TypedDict):
    keyPairName: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateLoadBalancerRequestRequestTypeDef

```python
# CreateLoadBalancerRequestRequestTypeDef definition

class CreateLoadBalancerRequestRequestTypeDef(TypedDict):
    loadBalancerName: str,
    instancePort: int,
    healthCheckPath: NotRequired[str],
    certificateName: NotRequired[str],
    certificateDomainName: NotRequired[str],
    certificateAlternativeNames: NotRequired[Sequence[str]],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    ipAddressType: NotRequired[IpAddressTypeType],  # (2)
    tlsPolicyName: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
## CreateLoadBalancerTlsCertificateRequestRequestTypeDef

```python
# CreateLoadBalancerTlsCertificateRequestRequestTypeDef definition

class CreateLoadBalancerTlsCertificateRequestRequestTypeDef(TypedDict):
    loadBalancerName: str,
    certificateName: str,
    certificateDomainName: str,
    certificateAlternativeNames: NotRequired[Sequence[str]],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRelationalDatabaseRequestRequestTypeDef

```python
# CreateRelationalDatabaseRequestRequestTypeDef definition

class CreateRelationalDatabaseRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    relationalDatabaseBlueprintId: str,
    relationalDatabaseBundleId: str,
    masterDatabaseName: str,
    masterUsername: str,
    availabilityZone: NotRequired[str],
    masterUserPassword: NotRequired[str],
    preferredBackupWindow: NotRequired[str],
    preferredMaintenanceWindow: NotRequired[str],
    publiclyAccessible: NotRequired[bool],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRelationalDatabaseSnapshotRequestRequestTypeDef

```python
# CreateRelationalDatabaseSnapshotRequestRequestTypeDef definition

class CreateRelationalDatabaseSnapshotRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    relationalDatabaseSnapshotName: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DiskSnapshotTypeDef

```python
# DiskSnapshotTypeDef definition

class DiskSnapshotTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    sizeInGb: NotRequired[int],
    state: NotRequired[DiskSnapshotStateType],  # (4)
    progress: NotRequired[str],
    fromDiskName: NotRequired[str],
    fromDiskArn: NotRequired[str],
    fromInstanceName: NotRequired[str],
    fromInstanceArn: NotRequired[str],
    isFromAutoSnapshot: NotRequired[bool],
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: DiskSnapshotStateType](./literals.md#disksnapshotstatetype) 
## DiskTypeDef

```python
# DiskTypeDef definition

class DiskTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    addOns: NotRequired[List[AddOnTypeDef]],  # (4)
    sizeInGb: NotRequired[int],
    isSystemDisk: NotRequired[bool],
    iops: NotRequired[int],
    path: NotRequired[str],
    state: NotRequired[DiskStateType],  # (5)
    attachedTo: NotRequired[str],
    isAttached: NotRequired[bool],
    attachmentState: NotRequired[str],
    gbInUse: NotRequired[int],
    autoMountStatus: NotRequired[AutoMountStatusType],  # (6)
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: AddOnTypeDef](./type_defs.md#addontypedef) 
5. See [:material-code-brackets: DiskStateType](./literals.md#diskstatetype) 
6. See [:material-code-brackets: AutoMountStatusType](./literals.md#automountstatustype) 
## KeyPairTypeDef

```python
# KeyPairTypeDef definition

class KeyPairTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    fingerprint: NotRequired[str],
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RelationalDatabaseSnapshotTypeDef

```python
# RelationalDatabaseSnapshotTypeDef definition

class RelationalDatabaseSnapshotTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    engine: NotRequired[str],
    engineVersion: NotRequired[str],
    sizeInGb: NotRequired[int],
    state: NotRequired[str],
    fromRelationalDatabaseName: NotRequired[str],
    fromRelationalDatabaseArn: NotRequired[str],
    fromRelationalDatabaseBundleId: NotRequired[str],
    fromRelationalDatabaseBlueprintId: NotRequired[str],
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceName: str,
    tags: Sequence[TagTypeDef],  # (1)
    resourceArn: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetBundlesResultTypeDef

```python
# GetBundlesResultTypeDef definition

class GetBundlesResultTypeDef(TypedDict):
    bundles: List[BundleTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BundleTypeDef](./type_defs.md#bundletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CacheSettingsOutputTypeDef

```python
# CacheSettingsOutputTypeDef definition

class CacheSettingsOutputTypeDef(TypedDict):
    defaultTTL: NotRequired[int],
    minimumTTL: NotRequired[int],
    maximumTTL: NotRequired[int],
    allowedHTTPMethods: NotRequired[str],
    cachedHTTPMethods: NotRequired[str],
    forwardedCookies: NotRequired[CookieObjectOutputTypeDef],  # (1)
    forwardedHeaders: NotRequired[HeaderObjectOutputTypeDef],  # (2)
    forwardedQueryStrings: NotRequired[QueryStringObjectOutputTypeDef],  # (3)
```

1. See [:material-code-braces: CookieObjectOutputTypeDef](./type_defs.md#cookieobjectoutputtypedef) 
2. See [:material-code-braces: HeaderObjectOutputTypeDef](./type_defs.md#headerobjectoutputtypedef) 
3. See [:material-code-braces: QueryStringObjectOutputTypeDef](./type_defs.md#querystringobjectoutputtypedef) 
## CloseInstancePublicPortsRequestRequestTypeDef

```python
# CloseInstancePublicPortsRequestRequestTypeDef definition

class CloseInstancePublicPortsRequestRequestTypeDef(TypedDict):
    portInfo: PortInfoTypeDef,  # (1)
    instanceName: str,
```

1. See [:material-code-braces: PortInfoTypeDef](./type_defs.md#portinfotypedef) 
## OpenInstancePublicPortsRequestRequestTypeDef

```python
# OpenInstancePublicPortsRequestRequestTypeDef definition

class OpenInstancePublicPortsRequestRequestTypeDef(TypedDict):
    portInfo: PortInfoTypeDef,  # (1)
    instanceName: str,
```

1. See [:material-code-braces: PortInfoTypeDef](./type_defs.md#portinfotypedef) 
## PutInstancePublicPortsRequestRequestTypeDef

```python
# PutInstancePublicPortsRequestRequestTypeDef definition

class PutInstancePublicPortsRequestRequestTypeDef(TypedDict):
    portInfos: Sequence[PortInfoTypeDef],  # (1)
    instanceName: str,
```

1. See [:material-code-braces: PortInfoTypeDef](./type_defs.md#portinfotypedef) 
## CloudFormationStackRecordTypeDef

```python
# CloudFormationStackRecordTypeDef definition

class CloudFormationStackRecordTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    state: NotRequired[RecordStateType],  # (3)
    sourceInfo: NotRequired[List[CloudFormationStackRecordSourceInfoTypeDef]],  # (4)
    destinationInfo: NotRequired[DestinationInfoTypeDef],  # (5)
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-brackets: RecordStateType](./literals.md#recordstatetype) 
4. See [:material-code-braces: CloudFormationStackRecordSourceInfoTypeDef](./type_defs.md#cloudformationstackrecordsourceinfotypedef) 
5. See [:material-code-braces: DestinationInfoTypeDef](./type_defs.md#destinationinfotypedef) 
## GetContainerImagesResultTypeDef

```python
# GetContainerImagesResultTypeDef definition

class GetContainerImagesResultTypeDef(TypedDict):
    containerImages: List[ContainerImageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerImageTypeDef](./type_defs.md#containerimagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterContainerImageResultTypeDef

```python
# RegisterContainerImageResultTypeDef definition

class RegisterContainerImageResultTypeDef(TypedDict):
    containerImage: ContainerImageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerImageTypeDef](./type_defs.md#containerimagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PrivateRegistryAccessRequestTypeDef

```python
# PrivateRegistryAccessRequestTypeDef definition

class PrivateRegistryAccessRequestTypeDef(TypedDict):
    ecrImagePullerRole: NotRequired[ContainerServiceECRImagePullerRoleRequestTypeDef],  # (1)
```

1. See [:material-code-braces: ContainerServiceECRImagePullerRoleRequestTypeDef](./type_defs.md#containerserviceecrimagepullerrolerequesttypedef) 
## PrivateRegistryAccessTypeDef

```python
# PrivateRegistryAccessTypeDef definition

class PrivateRegistryAccessTypeDef(TypedDict):
    ecrImagePullerRole: NotRequired[ContainerServiceECRImagePullerRoleTypeDef],  # (1)
```

1. See [:material-code-braces: ContainerServiceECRImagePullerRoleTypeDef](./type_defs.md#containerserviceecrimagepullerroletypedef) 
## ContainerServiceEndpointTypeDef

```python
# ContainerServiceEndpointTypeDef definition

class ContainerServiceEndpointTypeDef(TypedDict):
    containerName: NotRequired[str],
    containerPort: NotRequired[int],
    healthCheck: NotRequired[ContainerServiceHealthCheckConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ContainerServiceHealthCheckConfigTypeDef](./type_defs.md#containerservicehealthcheckconfigtypedef) 
## EndpointRequestTypeDef

```python
# EndpointRequestTypeDef definition

class EndpointRequestTypeDef(TypedDict):
    containerName: str,
    containerPort: int,
    healthCheck: NotRequired[ContainerServiceHealthCheckConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ContainerServiceHealthCheckConfigTypeDef](./type_defs.md#containerservicehealthcheckconfigtypedef) 
## GetContainerLogResultTypeDef

```python
# GetContainerLogResultTypeDef definition

class GetContainerLogResultTypeDef(TypedDict):
    logEvents: List[ContainerServiceLogEventTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerServiceLogEventTypeDef](./type_defs.md#containerservicelogeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContainerServicePowersResultTypeDef

```python
# GetContainerServicePowersResultTypeDef definition

class GetContainerServicePowersResultTypeDef(TypedDict):
    powers: List[ContainerServicePowerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerServicePowerTypeDef](./type_defs.md#containerservicepowertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContainerServiceRegistryLoginResultTypeDef

```python
# CreateContainerServiceRegistryLoginResultTypeDef definition

class CreateContainerServiceRegistryLoginResultTypeDef(TypedDict):
    registryLogin: ContainerServiceRegistryLoginTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerServiceRegistryLoginTypeDef](./type_defs.md#containerserviceregistrylogintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCloudFormationStackRequestRequestTypeDef

```python
# CreateCloudFormationStackRequestRequestTypeDef definition

class CreateCloudFormationStackRequestRequestTypeDef(TypedDict):
    instances: Sequence[InstanceEntryTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceEntryTypeDef](./type_defs.md#instanceentrytypedef) 
## CreateDomainEntryRequestRequestTypeDef

```python
# CreateDomainEntryRequestRequestTypeDef definition

class CreateDomainEntryRequestRequestTypeDef(TypedDict):
    domainName: str,
    domainEntry: DomainEntryTypeDef,  # (1)
```

1. See [:material-code-braces: DomainEntryTypeDef](./type_defs.md#domainentrytypedef) 
## DeleteDomainEntryRequestRequestTypeDef

```python
# DeleteDomainEntryRequestRequestTypeDef definition

class DeleteDomainEntryRequestRequestTypeDef(TypedDict):
    domainName: str,
    domainEntry: DomainEntryTypeDef,  # (1)
```

1. See [:material-code-braces: DomainEntryTypeDef](./type_defs.md#domainentrytypedef) 
## UpdateDomainEntryRequestRequestTypeDef

```python
# UpdateDomainEntryRequestRequestTypeDef definition

class UpdateDomainEntryRequestRequestTypeDef(TypedDict):
    domainName: str,
    domainEntry: DomainEntryTypeDef,  # (1)
```

1. See [:material-code-braces: DomainEntryTypeDef](./type_defs.md#domainentrytypedef) 
## CreateGUISessionAccessDetailsResultTypeDef

```python
# CreateGUISessionAccessDetailsResultTypeDef definition

class CreateGUISessionAccessDetailsResultTypeDef(TypedDict):
    resourceName: str,
    status: StatusType,  # (1)
    percentageComplete: int,
    failureReason: str,
    sessions: List[SessionTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef

```python
# CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef definition

class CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    availabilityZone: NotRequired[str],
    publiclyAccessible: NotRequired[bool],
    relationalDatabaseSnapshotName: NotRequired[str],
    relationalDatabaseBundleId: NotRequired[str],
    sourceRelationalDatabaseName: NotRequired[str],
    restoreTime: NotRequired[TimestampTypeDef],
    useLatestRestorableTime: NotRequired[bool],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetBucketMetricDataRequestRequestTypeDef

```python
# GetBucketMetricDataRequestRequestTypeDef definition

class GetBucketMetricDataRequestRequestTypeDef(TypedDict):
    bucketName: str,
    metricName: BucketMetricNameType,  # (1)
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    period: int,
    statistics: Sequence[MetricStatisticType],  # (2)
    unit: MetricUnitType,  # (3)
```

1. See [:material-code-brackets: BucketMetricNameType](./literals.md#bucketmetricnametype) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
3. See [:material-code-brackets: MetricUnitType](./literals.md#metricunittype) 
## GetContainerLogRequestRequestTypeDef

```python
# GetContainerLogRequestRequestTypeDef definition

class GetContainerLogRequestRequestTypeDef(TypedDict):
    serviceName: str,
    containerName: str,
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    filterPattern: NotRequired[str],
    pageToken: NotRequired[str],
```

## GetContainerServiceMetricDataRequestRequestTypeDef

```python
# GetContainerServiceMetricDataRequestRequestTypeDef definition

class GetContainerServiceMetricDataRequestRequestTypeDef(TypedDict):
    serviceName: str,
    metricName: ContainerServiceMetricNameType,  # (1)
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    period: int,
    statistics: Sequence[MetricStatisticType],  # (2)
```

1. See [:material-code-brackets: ContainerServiceMetricNameType](./literals.md#containerservicemetricnametype) 
2. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## GetCostEstimateRequestRequestTypeDef

```python
# GetCostEstimateRequestRequestTypeDef definition

class GetCostEstimateRequestRequestTypeDef(TypedDict):
    resourceName: str,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
```

## GetDistributionMetricDataRequestRequestTypeDef

```python
# GetDistributionMetricDataRequestRequestTypeDef definition

class GetDistributionMetricDataRequestRequestTypeDef(TypedDict):
    distributionName: str,
    metricName: DistributionMetricNameType,  # (1)
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    period: int,
    unit: MetricUnitType,  # (2)
    statistics: Sequence[MetricStatisticType],  # (3)
```

1. See [:material-code-brackets: DistributionMetricNameType](./literals.md#distributionmetricnametype) 
2. See [:material-code-brackets: MetricUnitType](./literals.md#metricunittype) 
3. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## GetInstanceMetricDataRequestRequestTypeDef

```python
# GetInstanceMetricDataRequestRequestTypeDef definition

class GetInstanceMetricDataRequestRequestTypeDef(TypedDict):
    instanceName: str,
    metricName: InstanceMetricNameType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    unit: MetricUnitType,  # (2)
    statistics: Sequence[MetricStatisticType],  # (3)
```

1. See [:material-code-brackets: InstanceMetricNameType](./literals.md#instancemetricnametype) 
2. See [:material-code-brackets: MetricUnitType](./literals.md#metricunittype) 
3. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## GetLoadBalancerMetricDataRequestRequestTypeDef

```python
# GetLoadBalancerMetricDataRequestRequestTypeDef definition

class GetLoadBalancerMetricDataRequestRequestTypeDef(TypedDict):
    loadBalancerName: str,
    metricName: LoadBalancerMetricNameType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    unit: MetricUnitType,  # (2)
    statistics: Sequence[MetricStatisticType],  # (3)
```

1. See [:material-code-brackets: LoadBalancerMetricNameType](./literals.md#loadbalancermetricnametype) 
2. See [:material-code-brackets: MetricUnitType](./literals.md#metricunittype) 
3. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## GetRelationalDatabaseLogEventsRequestRequestTypeDef

```python
# GetRelationalDatabaseLogEventsRequestRequestTypeDef definition

class GetRelationalDatabaseLogEventsRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    logStreamName: str,
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    startFromHead: NotRequired[bool],
    pageToken: NotRequired[str],
```

## GetRelationalDatabaseMetricDataRequestRequestTypeDef

```python
# GetRelationalDatabaseMetricDataRequestRequestTypeDef definition

class GetRelationalDatabaseMetricDataRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    metricName: RelationalDatabaseMetricNameType,  # (1)
    period: int,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    unit: MetricUnitType,  # (2)
    statistics: Sequence[MetricStatisticType],  # (3)
```

1. See [:material-code-brackets: RelationalDatabaseMetricNameType](./literals.md#relationaldatabasemetricnametype) 
2. See [:material-code-brackets: MetricUnitType](./literals.md#metricunittype) 
3. See [:material-code-brackets: MetricStatisticType](./literals.md#metricstatistictype) 
## InstanceSnapshotInfoTypeDef

```python
# InstanceSnapshotInfoTypeDef definition

class InstanceSnapshotInfoTypeDef(TypedDict):
    fromBundleId: NotRequired[str],
    fromBlueprintId: NotRequired[str],
    fromDiskInfo: NotRequired[List[DiskInfoTypeDef]],  # (1)
```

1. See [:material-code-braces: DiskInfoTypeDef](./type_defs.md#diskinfotypedef) 
## GetDistributionBundlesResultTypeDef

```python
# GetDistributionBundlesResultTypeDef definition

class GetDistributionBundlesResultTypeDef(TypedDict):
    bundles: List[DistributionBundleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionBundleTypeDef](./type_defs.md#distributionbundletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainValidationRecordTypeDef

```python
# DomainValidationRecordTypeDef definition

class DomainValidationRecordTypeDef(TypedDict):
    domainName: NotRequired[str],
    resourceRecord: NotRequired[ResourceRecordTypeDef],  # (1)
    dnsRecordCreationState: NotRequired[DnsRecordCreationStateTypeDef],  # (2)
    validationStatus: NotRequired[CertificateDomainValidationStatusType],  # (3)
```

1. See [:material-code-braces: ResourceRecordTypeDef](./type_defs.md#resourcerecordtypedef) 
2. See [:material-code-braces: DnsRecordCreationStateTypeDef](./type_defs.md#dnsrecordcreationstatetypedef) 
3. See [:material-code-brackets: CertificateDomainValidationStatusType](./literals.md#certificatedomainvalidationstatustype) 
## EstimateByTimeTypeDef

```python
# EstimateByTimeTypeDef definition

class EstimateByTimeTypeDef(TypedDict):
    usageCost: NotRequired[float],
    pricingUnit: NotRequired[PricingUnitType],  # (1)
    unit: NotRequired[float],
    currency: NotRequired[CurrencyType],  # (2)
    timePeriod: NotRequired[TimePeriodTypeDef],  # (3)
```

1. See [:material-code-brackets: PricingUnitType](./literals.md#pricingunittype) 
2. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
3. See [:material-code-braces: TimePeriodTypeDef](./type_defs.md#timeperiodtypedef) 
## GetActiveNamesRequestPaginateTypeDef

```python
# GetActiveNamesRequestPaginateTypeDef definition

class GetActiveNamesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetBlueprintsRequestPaginateTypeDef

```python
# GetBlueprintsRequestPaginateTypeDef definition

class GetBlueprintsRequestPaginateTypeDef(TypedDict):
    includeInactive: NotRequired[bool],
    appCategory: NotRequired[AppCategoryType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AppCategoryType](./literals.md#appcategorytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetBundlesRequestPaginateTypeDef

```python
# GetBundlesRequestPaginateTypeDef definition

class GetBundlesRequestPaginateTypeDef(TypedDict):
    includeInactive: NotRequired[bool],
    appCategory: NotRequired[AppCategoryType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AppCategoryType](./literals.md#appcategorytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetCloudFormationStackRecordsRequestPaginateTypeDef

```python
# GetCloudFormationStackRecordsRequestPaginateTypeDef definition

class GetCloudFormationStackRecordsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDiskSnapshotsRequestPaginateTypeDef

```python
# GetDiskSnapshotsRequestPaginateTypeDef definition

class GetDiskSnapshotsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDisksRequestPaginateTypeDef

```python
# GetDisksRequestPaginateTypeDef definition

class GetDisksRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDomainsRequestPaginateTypeDef

```python
# GetDomainsRequestPaginateTypeDef definition

class GetDomainsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetExportSnapshotRecordsRequestPaginateTypeDef

```python
# GetExportSnapshotRecordsRequestPaginateTypeDef definition

class GetExportSnapshotRecordsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetInstanceSnapshotsRequestPaginateTypeDef

```python
# GetInstanceSnapshotsRequestPaginateTypeDef definition

class GetInstanceSnapshotsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetInstancesRequestPaginateTypeDef

```python
# GetInstancesRequestPaginateTypeDef definition

class GetInstancesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetKeyPairsRequestPaginateTypeDef

```python
# GetKeyPairsRequestPaginateTypeDef definition

class GetKeyPairsRequestPaginateTypeDef(TypedDict):
    includeDefaultKeyPair: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetLoadBalancersRequestPaginateTypeDef

```python
# GetLoadBalancersRequestPaginateTypeDef definition

class GetLoadBalancersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetOperationsRequestPaginateTypeDef

```python
# GetOperationsRequestPaginateTypeDef definition

class GetOperationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRelationalDatabaseBlueprintsRequestPaginateTypeDef

```python
# GetRelationalDatabaseBlueprintsRequestPaginateTypeDef definition

class GetRelationalDatabaseBlueprintsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRelationalDatabaseBundlesRequestPaginateTypeDef

```python
# GetRelationalDatabaseBundlesRequestPaginateTypeDef definition

class GetRelationalDatabaseBundlesRequestPaginateTypeDef(TypedDict):
    includeInactive: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRelationalDatabaseEventsRequestPaginateTypeDef

```python
# GetRelationalDatabaseEventsRequestPaginateTypeDef definition

class GetRelationalDatabaseEventsRequestPaginateTypeDef(TypedDict):
    relationalDatabaseName: str,
    durationInMinutes: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRelationalDatabaseParametersRequestPaginateTypeDef

```python
# GetRelationalDatabaseParametersRequestPaginateTypeDef definition

class GetRelationalDatabaseParametersRequestPaginateTypeDef(TypedDict):
    relationalDatabaseName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRelationalDatabaseSnapshotsRequestPaginateTypeDef

```python
# GetRelationalDatabaseSnapshotsRequestPaginateTypeDef definition

class GetRelationalDatabaseSnapshotsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRelationalDatabasesRequestPaginateTypeDef

```python
# GetRelationalDatabasesRequestPaginateTypeDef definition

class GetRelationalDatabasesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetStaticIpsRequestPaginateTypeDef

```python
# GetStaticIpsRequestPaginateTypeDef definition

class GetStaticIpsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetBucketMetricDataResultTypeDef

```python
# GetBucketMetricDataResultTypeDef definition

class GetBucketMetricDataResultTypeDef(TypedDict):
    metricName: BucketMetricNameType,  # (1)
    metricData: List[MetricDatapointTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: BucketMetricNameType](./literals.md#bucketmetricnametype) 
2. See [:material-code-braces: MetricDatapointTypeDef](./type_defs.md#metricdatapointtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContainerServiceMetricDataResultTypeDef

```python
# GetContainerServiceMetricDataResultTypeDef definition

class GetContainerServiceMetricDataResultTypeDef(TypedDict):
    metricName: ContainerServiceMetricNameType,  # (1)
    metricData: List[MetricDatapointTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ContainerServiceMetricNameType](./literals.md#containerservicemetricnametype) 
2. See [:material-code-braces: MetricDatapointTypeDef](./type_defs.md#metricdatapointtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDistributionMetricDataResultTypeDef

```python
# GetDistributionMetricDataResultTypeDef definition

class GetDistributionMetricDataResultTypeDef(TypedDict):
    metricName: DistributionMetricNameType,  # (1)
    metricData: List[MetricDatapointTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DistributionMetricNameType](./literals.md#distributionmetricnametype) 
2. See [:material-code-braces: MetricDatapointTypeDef](./type_defs.md#metricdatapointtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstanceMetricDataResultTypeDef

```python
# GetInstanceMetricDataResultTypeDef definition

class GetInstanceMetricDataResultTypeDef(TypedDict):
    metricName: InstanceMetricNameType,  # (1)
    metricData: List[MetricDatapointTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: InstanceMetricNameType](./literals.md#instancemetricnametype) 
2. See [:material-code-braces: MetricDatapointTypeDef](./type_defs.md#metricdatapointtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLoadBalancerMetricDataResultTypeDef

```python
# GetLoadBalancerMetricDataResultTypeDef definition

class GetLoadBalancerMetricDataResultTypeDef(TypedDict):
    metricName: LoadBalancerMetricNameType,  # (1)
    metricData: List[MetricDatapointTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: LoadBalancerMetricNameType](./literals.md#loadbalancermetricnametype) 
2. See [:material-code-braces: MetricDatapointTypeDef](./type_defs.md#metricdatapointtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRelationalDatabaseMetricDataResultTypeDef

```python
# GetRelationalDatabaseMetricDataResultTypeDef definition

class GetRelationalDatabaseMetricDataResultTypeDef(TypedDict):
    metricName: RelationalDatabaseMetricNameType,  # (1)
    metricData: List[MetricDatapointTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: RelationalDatabaseMetricNameType](./literals.md#relationaldatabasemetricnametype) 
2. See [:material-code-braces: MetricDatapointTypeDef](./type_defs.md#metricdatapointtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstancePortStatesResultTypeDef

```python
# GetInstancePortStatesResultTypeDef definition

class GetInstancePortStatesResultTypeDef(TypedDict):
    portStates: List[InstancePortStateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstancePortStateTypeDef](./type_defs.md#instanceportstatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstanceStateResultTypeDef

```python
# GetInstanceStateResultTypeDef definition

class GetInstanceStateResultTypeDef(TypedDict):
    state: InstanceStateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceStateTypeDef](./type_defs.md#instancestatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLoadBalancerTlsPoliciesResultTypeDef

```python
# GetLoadBalancerTlsPoliciesResultTypeDef definition

class GetLoadBalancerTlsPoliciesResultTypeDef(TypedDict):
    tlsPolicies: List[LoadBalancerTlsPolicyTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerTlsPolicyTypeDef](./type_defs.md#loadbalancertlspolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRelationalDatabaseBlueprintsResultTypeDef

```python
# GetRelationalDatabaseBlueprintsResultTypeDef definition

class GetRelationalDatabaseBlueprintsResultTypeDef(TypedDict):
    blueprints: List[RelationalDatabaseBlueprintTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RelationalDatabaseBlueprintTypeDef](./type_defs.md#relationaldatabaseblueprinttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRelationalDatabaseBundlesResultTypeDef

```python
# GetRelationalDatabaseBundlesResultTypeDef definition

class GetRelationalDatabaseBundlesResultTypeDef(TypedDict):
    bundles: List[RelationalDatabaseBundleTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RelationalDatabaseBundleTypeDef](./type_defs.md#relationaldatabasebundletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRelationalDatabaseEventsResultTypeDef

```python
# GetRelationalDatabaseEventsResultTypeDef definition

class GetRelationalDatabaseEventsResultTypeDef(TypedDict):
    relationalDatabaseEvents: List[RelationalDatabaseEventTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RelationalDatabaseEventTypeDef](./type_defs.md#relationaldatabaseeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRelationalDatabaseLogEventsResultTypeDef

```python
# GetRelationalDatabaseLogEventsResultTypeDef definition

class GetRelationalDatabaseLogEventsResultTypeDef(TypedDict):
    resourceLogEvents: List[LogEventTypeDef],  # (1)
    nextBackwardToken: str,
    nextForwardToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LogEventTypeDef](./type_defs.md#logeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRelationalDatabaseParametersResultTypeDef

```python
# GetRelationalDatabaseParametersResultTypeDef definition

class GetRelationalDatabaseParametersResultTypeDef(TypedDict):
    parameters: List[RelationalDatabaseParameterTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RelationalDatabaseParameterTypeDef](./type_defs.md#relationaldatabaseparametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRelationalDatabaseParametersRequestRequestTypeDef

```python
# UpdateRelationalDatabaseParametersRequestRequestTypeDef definition

class UpdateRelationalDatabaseParametersRequestRequestTypeDef(TypedDict):
    relationalDatabaseName: str,
    parameters: Sequence[RelationalDatabaseParameterTypeDef],  # (1)
```

1. See [:material-code-braces: RelationalDatabaseParameterTypeDef](./type_defs.md#relationaldatabaseparametertypedef) 
## InstanceAccessDetailsTypeDef

```python
# InstanceAccessDetailsTypeDef definition

class InstanceAccessDetailsTypeDef(TypedDict):
    certKey: NotRequired[str],
    expiresAt: NotRequired[datetime],
    ipAddress: NotRequired[str],
    ipv6Addresses: NotRequired[List[str]],
    password: NotRequired[str],
    passwordData: NotRequired[PasswordDataTypeDef],  # (1)
    privateKey: NotRequired[str],
    protocol: NotRequired[InstanceAccessProtocolType],  # (2)
    instanceName: NotRequired[str],
    username: NotRequired[str],
    hostKeys: NotRequired[List[HostKeyAttributesTypeDef]],  # (3)
```

1. See [:material-code-braces: PasswordDataTypeDef](./type_defs.md#passworddatatypedef) 
2. See [:material-code-brackets: InstanceAccessProtocolType](./literals.md#instanceaccessprotocoltype) 
3. See [:material-code-braces: HostKeyAttributesTypeDef](./type_defs.md#hostkeyattributestypedef) 
## InstanceNetworkingTypeDef

```python
# InstanceNetworkingTypeDef definition

class InstanceNetworkingTypeDef(TypedDict):
    monthlyTransfer: NotRequired[MonthlyTransferTypeDef],  # (1)
    ports: NotRequired[List[InstancePortInfoTypeDef]],  # (2)
```

1. See [:material-code-braces: MonthlyTransferTypeDef](./type_defs.md#monthlytransfertypedef) 
2. See [:material-code-braces: InstancePortInfoTypeDef](./type_defs.md#instanceportinfotypedef) 
## LoadBalancerTlsCertificateDomainValidationRecordTypeDef

```python
# LoadBalancerTlsCertificateDomainValidationRecordTypeDef definition

class LoadBalancerTlsCertificateDomainValidationRecordTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[str],
    value: NotRequired[str],
    validationStatus: NotRequired[LoadBalancerTlsCertificateDomainStatusType],  # (1)
    domainName: NotRequired[str],
    dnsRecordCreationState: NotRequired[LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef],  # (2)
```

1. See [:material-code-brackets: LoadBalancerTlsCertificateDomainStatusType](./literals.md#loadbalancertlscertificatedomainstatustype) 
2. See [:material-code-braces: LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef](./type_defs.md#loadbalancertlscertificatednsrecordcreationstatetypedef) 
## LoadBalancerTlsCertificateRenewalSummaryTypeDef

```python
# LoadBalancerTlsCertificateRenewalSummaryTypeDef definition

class LoadBalancerTlsCertificateRenewalSummaryTypeDef(TypedDict):
    renewalStatus: NotRequired[LoadBalancerTlsCertificateRenewalStatusType],  # (1)
    domainValidationOptions: NotRequired[List[LoadBalancerTlsCertificateDomainValidationOptionTypeDef]],  # (2)
```

1. See [:material-code-brackets: LoadBalancerTlsCertificateRenewalStatusType](./literals.md#loadbalancertlscertificaterenewalstatustype) 
2. See [:material-code-braces: LoadBalancerTlsCertificateDomainValidationOptionTypeDef](./type_defs.md#loadbalancertlscertificatedomainvalidationoptiontypedef) 
## LoadBalancerTypeDef

```python
# LoadBalancerTypeDef definition

class LoadBalancerTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    dnsName: NotRequired[str],
    state: NotRequired[LoadBalancerStateType],  # (4)
    protocol: NotRequired[LoadBalancerProtocolType],  # (5)
    publicPorts: NotRequired[List[int]],
    healthCheckPath: NotRequired[str],
    instancePort: NotRequired[int],
    instanceHealthSummary: NotRequired[List[InstanceHealthSummaryTypeDef]],  # (6)
    tlsCertificateSummaries: NotRequired[List[LoadBalancerTlsCertificateSummaryTypeDef]],  # (7)
    configurationOptions: NotRequired[Dict[LoadBalancerAttributeNameType, str]],  # (8)
    ipAddressType: NotRequired[IpAddressTypeType],  # (9)
    httpsRedirectionEnabled: NotRequired[bool],
    tlsPolicyName: NotRequired[str],
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: LoadBalancerStateType](./literals.md#loadbalancerstatetype) 
5. See [:material-code-brackets: LoadBalancerProtocolType](./literals.md#loadbalancerprotocoltype) 
6. See [:material-code-braces: InstanceHealthSummaryTypeDef](./type_defs.md#instancehealthsummarytypedef) 
7. See [:material-code-braces: LoadBalancerTlsCertificateSummaryTypeDef](./type_defs.md#loadbalancertlscertificatesummarytypedef) 
8. See [:material-code-brackets: LoadBalancerAttributeNameType](./literals.md#loadbalancerattributenametype) 
9. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
## RegisteredDomainDelegationInfoTypeDef

```python
# RegisteredDomainDelegationInfoTypeDef definition

class RegisteredDomainDelegationInfoTypeDef(TypedDict):
    nameServersUpdateState: NotRequired[NameServersUpdateStateTypeDef],  # (1)
    r53HostedZoneDeletionState: NotRequired[R53HostedZoneDeletionStateTypeDef],  # (2)
```

1. See [:material-code-braces: NameServersUpdateStateTypeDef](./type_defs.md#nameserversupdatestatetypedef) 
2. See [:material-code-braces: R53HostedZoneDeletionStateTypeDef](./type_defs.md#r53hostedzonedeletionstatetypedef) 
## RelationalDatabaseTypeDef

```python
# RelationalDatabaseTypeDef definition

class RelationalDatabaseTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    relationalDatabaseBlueprintId: NotRequired[str],
    relationalDatabaseBundleId: NotRequired[str],
    masterDatabaseName: NotRequired[str],
    hardware: NotRequired[RelationalDatabaseHardwareTypeDef],  # (4)
    state: NotRequired[str],
    secondaryAvailabilityZone: NotRequired[str],
    backupRetentionEnabled: NotRequired[bool],
    pendingModifiedValues: NotRequired[PendingModifiedRelationalDatabaseValuesTypeDef],  # (5)
    engine: NotRequired[str],
    engineVersion: NotRequired[str],
    latestRestorableTime: NotRequired[datetime],
    masterUsername: NotRequired[str],
    parameterApplyStatus: NotRequired[str],
    preferredBackupWindow: NotRequired[str],
    preferredMaintenanceWindow: NotRequired[str],
    publiclyAccessible: NotRequired[bool],
    masterEndpoint: NotRequired[RelationalDatabaseEndpointTypeDef],  # (6)
    pendingMaintenanceActions: NotRequired[List[PendingMaintenanceActionTypeDef]],  # (7)
    caCertificateIdentifier: NotRequired[str],
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: RelationalDatabaseHardwareTypeDef](./type_defs.md#relationaldatabasehardwaretypedef) 
5. See [:material-code-braces: PendingModifiedRelationalDatabaseValuesTypeDef](./type_defs.md#pendingmodifiedrelationaldatabasevaluestypedef) 
6. See [:material-code-braces: RelationalDatabaseEndpointTypeDef](./type_defs.md#relationaldatabaseendpointtypedef) 
7. See [:material-code-braces: PendingMaintenanceActionTypeDef](./type_defs.md#pendingmaintenanceactiontypedef) 
## GetBucketAccessKeysResultTypeDef

```python
# GetBucketAccessKeysResultTypeDef definition

class GetBucketAccessKeysResultTypeDef(TypedDict):
    accessKeys: List[AccessKeyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessKeyTypeDef](./type_defs.md#accesskeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDiskFromSnapshotRequestRequestTypeDef

```python
# CreateDiskFromSnapshotRequestRequestTypeDef definition

class CreateDiskFromSnapshotRequestRequestTypeDef(TypedDict):
    diskName: str,
    availabilityZone: str,
    sizeInGb: int,
    diskSnapshotName: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    addOns: NotRequired[Sequence[AddOnRequestTypeDef]],  # (2)
    sourceDiskName: NotRequired[str],
    restoreDate: NotRequired[str],
    useLatestRestorableAutoSnapshot: NotRequired[bool],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: AddOnRequestTypeDef](./type_defs.md#addonrequesttypedef) 
## CreateDiskRequestRequestTypeDef

```python
# CreateDiskRequestRequestTypeDef definition

class CreateDiskRequestRequestTypeDef(TypedDict):
    diskName: str,
    availabilityZone: str,
    sizeInGb: int,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    addOns: NotRequired[Sequence[AddOnRequestTypeDef]],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: AddOnRequestTypeDef](./type_defs.md#addonrequesttypedef) 
## CreateInstancesFromSnapshotRequestRequestTypeDef

```python
# CreateInstancesFromSnapshotRequestRequestTypeDef definition

class CreateInstancesFromSnapshotRequestRequestTypeDef(TypedDict):
    instanceNames: Sequence[str],
    availabilityZone: str,
    bundleId: str,
    attachedDiskMapping: NotRequired[Mapping[str, Sequence[DiskMapTypeDef]]],  # (1)
    instanceSnapshotName: NotRequired[str],
    userData: NotRequired[str],
    keyPairName: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    addOns: NotRequired[Sequence[AddOnRequestTypeDef]],  # (3)
    ipAddressType: NotRequired[IpAddressTypeType],  # (4)
    sourceInstanceName: NotRequired[str],
    restoreDate: NotRequired[str],
    useLatestRestorableAutoSnapshot: NotRequired[bool],
```

1. See [:material-code-braces: DiskMapTypeDef](./type_defs.md#diskmaptypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: AddOnRequestTypeDef](./type_defs.md#addonrequesttypedef) 
4. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
## CreateInstancesRequestRequestTypeDef

```python
# CreateInstancesRequestRequestTypeDef definition

class CreateInstancesRequestRequestTypeDef(TypedDict):
    instanceNames: Sequence[str],
    availabilityZone: str,
    blueprintId: str,
    bundleId: str,
    customImageName: NotRequired[str],
    userData: NotRequired[str],
    keyPairName: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    addOns: NotRequired[Sequence[AddOnRequestTypeDef]],  # (2)
    ipAddressType: NotRequired[IpAddressTypeType],  # (3)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: AddOnRequestTypeDef](./type_defs.md#addonrequesttypedef) 
3. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
## EnableAddOnRequestRequestTypeDef

```python
# EnableAddOnRequestRequestTypeDef definition

class EnableAddOnRequestRequestTypeDef(TypedDict):
    resourceName: str,
    addOnRequest: AddOnRequestTypeDef,  # (1)
```

1. See [:material-code-braces: AddOnRequestTypeDef](./type_defs.md#addonrequesttypedef) 
## GetAlarmsResultTypeDef

```python
# GetAlarmsResultTypeDef definition

class GetAlarmsResultTypeDef(TypedDict):
    alarms: List[AlarmTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContactMethodsResultTypeDef

```python
# GetContactMethodsResultTypeDef definition

class GetContactMethodsResultTypeDef(TypedDict):
    contactMethods: List[ContactMethodTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContactMethodTypeDef](./type_defs.md#contactmethodtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AllocateStaticIpResultTypeDef

```python
# AllocateStaticIpResultTypeDef definition

class AllocateStaticIpResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachCertificateToDistributionResultTypeDef

```python
# AttachCertificateToDistributionResultTypeDef definition

class AttachCertificateToDistributionResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachDiskResultTypeDef

```python
# AttachDiskResultTypeDef definition

class AttachDiskResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachInstancesToLoadBalancerResultTypeDef

```python
# AttachInstancesToLoadBalancerResultTypeDef definition

class AttachInstancesToLoadBalancerResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachLoadBalancerTlsCertificateResultTypeDef

```python
# AttachLoadBalancerTlsCertificateResultTypeDef definition

class AttachLoadBalancerTlsCertificateResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachStaticIpResultTypeDef

```python
# AttachStaticIpResultTypeDef definition

class AttachStaticIpResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CloseInstancePublicPortsResultTypeDef

```python
# CloseInstancePublicPortsResultTypeDef definition

class CloseInstancePublicPortsResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopySnapshotResultTypeDef

```python
# CopySnapshotResultTypeDef definition

class CopySnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBucketAccessKeyResultTypeDef

```python
# CreateBucketAccessKeyResultTypeDef definition

class CreateBucketAccessKeyResultTypeDef(TypedDict):
    accessKey: AccessKeyTypeDef,  # (1)
    operations: List[OperationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AccessKeyTypeDef](./type_defs.md#accesskeytypedef) 
2. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCloudFormationStackResultTypeDef

```python
# CreateCloudFormationStackResultTypeDef definition

class CreateCloudFormationStackResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContactMethodResultTypeDef

```python
# CreateContactMethodResultTypeDef definition

class CreateContactMethodResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDiskFromSnapshotResultTypeDef

```python
# CreateDiskFromSnapshotResultTypeDef definition

class CreateDiskFromSnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDiskResultTypeDef

```python
# CreateDiskResultTypeDef definition

class CreateDiskResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDiskSnapshotResultTypeDef

```python
# CreateDiskSnapshotResultTypeDef definition

class CreateDiskSnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDomainEntryResultTypeDef

```python
# CreateDomainEntryResultTypeDef definition

class CreateDomainEntryResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDomainResultTypeDef

```python
# CreateDomainResultTypeDef definition

class CreateDomainResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstanceSnapshotResultTypeDef

```python
# CreateInstanceSnapshotResultTypeDef definition

class CreateInstanceSnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstancesFromSnapshotResultTypeDef

```python
# CreateInstancesFromSnapshotResultTypeDef definition

class CreateInstancesFromSnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInstancesResultTypeDef

```python
# CreateInstancesResultTypeDef definition

class CreateInstancesResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLoadBalancerResultTypeDef

```python
# CreateLoadBalancerResultTypeDef definition

class CreateLoadBalancerResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLoadBalancerTlsCertificateResultTypeDef

```python
# CreateLoadBalancerTlsCertificateResultTypeDef definition

class CreateLoadBalancerTlsCertificateResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRelationalDatabaseFromSnapshotResultTypeDef

```python
# CreateRelationalDatabaseFromSnapshotResultTypeDef definition

class CreateRelationalDatabaseFromSnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRelationalDatabaseResultTypeDef

```python
# CreateRelationalDatabaseResultTypeDef definition

class CreateRelationalDatabaseResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRelationalDatabaseSnapshotResultTypeDef

```python
# CreateRelationalDatabaseSnapshotResultTypeDef definition

class CreateRelationalDatabaseSnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAlarmResultTypeDef

```python
# DeleteAlarmResultTypeDef definition

class DeleteAlarmResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAutoSnapshotResultTypeDef

```python
# DeleteAutoSnapshotResultTypeDef definition

class DeleteAutoSnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBucketAccessKeyResultTypeDef

```python
# DeleteBucketAccessKeyResultTypeDef definition

class DeleteBucketAccessKeyResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBucketResultTypeDef

```python
# DeleteBucketResultTypeDef definition

class DeleteBucketResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCertificateResultTypeDef

```python
# DeleteCertificateResultTypeDef definition

class DeleteCertificateResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteContactMethodResultTypeDef

```python
# DeleteContactMethodResultTypeDef definition

class DeleteContactMethodResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDiskResultTypeDef

```python
# DeleteDiskResultTypeDef definition

class DeleteDiskResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDiskSnapshotResultTypeDef

```python
# DeleteDiskSnapshotResultTypeDef definition

class DeleteDiskSnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDistributionResultTypeDef

```python
# DeleteDistributionResultTypeDef definition

class DeleteDistributionResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDomainEntryResultTypeDef

```python
# DeleteDomainEntryResultTypeDef definition

class DeleteDomainEntryResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDomainResultTypeDef

```python
# DeleteDomainResultTypeDef definition

class DeleteDomainResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInstanceResultTypeDef

```python
# DeleteInstanceResultTypeDef definition

class DeleteInstanceResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInstanceSnapshotResultTypeDef

```python
# DeleteInstanceSnapshotResultTypeDef definition

class DeleteInstanceSnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteKeyPairResultTypeDef

```python
# DeleteKeyPairResultTypeDef definition

class DeleteKeyPairResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteKnownHostKeysResultTypeDef

```python
# DeleteKnownHostKeysResultTypeDef definition

class DeleteKnownHostKeysResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteLoadBalancerResultTypeDef

```python
# DeleteLoadBalancerResultTypeDef definition

class DeleteLoadBalancerResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteLoadBalancerTlsCertificateResultTypeDef

```python
# DeleteLoadBalancerTlsCertificateResultTypeDef definition

class DeleteLoadBalancerTlsCertificateResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRelationalDatabaseResultTypeDef

```python
# DeleteRelationalDatabaseResultTypeDef definition

class DeleteRelationalDatabaseResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRelationalDatabaseSnapshotResultTypeDef

```python
# DeleteRelationalDatabaseSnapshotResultTypeDef definition

class DeleteRelationalDatabaseSnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetachCertificateFromDistributionResultTypeDef

```python
# DetachCertificateFromDistributionResultTypeDef definition

class DetachCertificateFromDistributionResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetachDiskResultTypeDef

```python
# DetachDiskResultTypeDef definition

class DetachDiskResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetachInstancesFromLoadBalancerResultTypeDef

```python
# DetachInstancesFromLoadBalancerResultTypeDef definition

class DetachInstancesFromLoadBalancerResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetachStaticIpResultTypeDef

```python
# DetachStaticIpResultTypeDef definition

class DetachStaticIpResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableAddOnResultTypeDef

```python
# DisableAddOnResultTypeDef definition

class DisableAddOnResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableAddOnResultTypeDef

```python
# EnableAddOnResultTypeDef definition

class EnableAddOnResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportSnapshotResultTypeDef

```python
# ExportSnapshotResultTypeDef definition

class ExportSnapshotResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOperationResultTypeDef

```python
# GetOperationResultTypeDef definition

class GetOperationResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOperationsForResourceResultTypeDef

```python
# GetOperationsForResourceResultTypeDef definition

class GetOperationsForResourceResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    nextPageCount: str,
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOperationsResultTypeDef

```python
# GetOperationsResultTypeDef definition

class GetOperationsResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportKeyPairResultTypeDef

```python
# ImportKeyPairResultTypeDef definition

class ImportKeyPairResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OpenInstancePublicPortsResultTypeDef

```python
# OpenInstancePublicPortsResultTypeDef definition

class OpenInstancePublicPortsResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PeerVpcResultTypeDef

```python
# PeerVpcResultTypeDef definition

class PeerVpcResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAlarmResultTypeDef

```python
# PutAlarmResultTypeDef definition

class PutAlarmResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutInstancePublicPortsResultTypeDef

```python
# PutInstancePublicPortsResultTypeDef definition

class PutInstancePublicPortsResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RebootInstanceResultTypeDef

```python
# RebootInstanceResultTypeDef definition

class RebootInstanceResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RebootRelationalDatabaseResultTypeDef

```python
# RebootRelationalDatabaseResultTypeDef definition

class RebootRelationalDatabaseResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReleaseStaticIpResultTypeDef

```python
# ReleaseStaticIpResultTypeDef definition

class ReleaseStaticIpResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetDistributionCacheResultTypeDef

```python
# ResetDistributionCacheResultTypeDef definition

class ResetDistributionCacheResultTypeDef(TypedDict):
    status: str,
    createTime: datetime,
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendContactMethodVerificationResultTypeDef

```python
# SendContactMethodVerificationResultTypeDef definition

class SendContactMethodVerificationResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetIpAddressTypeResultTypeDef

```python
# SetIpAddressTypeResultTypeDef definition

class SetIpAddressTypeResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetResourceAccessForBucketResultTypeDef

```python
# SetResourceAccessForBucketResultTypeDef definition

class SetResourceAccessForBucketResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetupInstanceHttpsResultTypeDef

```python
# SetupInstanceHttpsResultTypeDef definition

class SetupInstanceHttpsResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartGUISessionResultTypeDef

```python
# StartGUISessionResultTypeDef definition

class StartGUISessionResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartInstanceResultTypeDef

```python
# StartInstanceResultTypeDef definition

class StartInstanceResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartRelationalDatabaseResultTypeDef

```python
# StartRelationalDatabaseResultTypeDef definition

class StartRelationalDatabaseResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopGUISessionResultTypeDef

```python
# StopGUISessionResultTypeDef definition

class StopGUISessionResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopInstanceResultTypeDef

```python
# StopInstanceResultTypeDef definition

class StopInstanceResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopRelationalDatabaseResultTypeDef

```python
# StopRelationalDatabaseResultTypeDef definition

class StopRelationalDatabaseResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceResultTypeDef

```python
# TagResourceResultTypeDef definition

class TagResourceResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestAlarmResultTypeDef

```python
# TestAlarmResultTypeDef definition

class TestAlarmResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UnpeerVpcResultTypeDef

```python
# UnpeerVpcResultTypeDef definition

class UnpeerVpcResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UntagResourceResultTypeDef

```python
# UntagResourceResultTypeDef definition

class UntagResourceResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBucketBundleResultTypeDef

```python
# UpdateBucketBundleResultTypeDef definition

class UpdateBucketBundleResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDistributionBundleResultTypeDef

```python
# UpdateDistributionBundleResultTypeDef definition

class UpdateDistributionBundleResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDistributionResultTypeDef

```python
# UpdateDistributionResultTypeDef definition

class UpdateDistributionResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainEntryResultTypeDef

```python
# UpdateDomainEntryResultTypeDef definition

class UpdateDomainEntryResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInstanceMetadataOptionsResultTypeDef

```python
# UpdateInstanceMetadataOptionsResultTypeDef definition

class UpdateInstanceMetadataOptionsResultTypeDef(TypedDict):
    operation: OperationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLoadBalancerAttributeResultTypeDef

```python
# UpdateLoadBalancerAttributeResultTypeDef definition

class UpdateLoadBalancerAttributeResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRelationalDatabaseParametersResultTypeDef

```python
# UpdateRelationalDatabaseParametersResultTypeDef definition

class UpdateRelationalDatabaseParametersResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRelationalDatabaseResultTypeDef

```python
# UpdateRelationalDatabaseResultTypeDef definition

class UpdateRelationalDatabaseResultTypeDef(TypedDict):
    operations: List[OperationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetupHistoryTypeDef

```python
# SetupHistoryTypeDef definition

class SetupHistoryTypeDef(TypedDict):
    operationId: NotRequired[str],
    request: NotRequired[SetupRequestTypeDef],  # (1)
    resource: NotRequired[SetupHistoryResourceTypeDef],  # (2)
    executionDetails: NotRequired[List[SetupExecutionDetailsTypeDef]],  # (3)
    status: NotRequired[SetupStatusType],  # (4)
```

1. See [:material-code-braces: SetupRequestTypeDef](./type_defs.md#setuprequesttypedef) 
2. See [:material-code-braces: SetupHistoryResourceTypeDef](./type_defs.md#setuphistoryresourcetypedef) 
3. See [:material-code-braces: SetupExecutionDetailsTypeDef](./type_defs.md#setupexecutiondetailstypedef) 
4. See [:material-code-brackets: SetupStatusType](./literals.md#setupstatustype) 
## GetStaticIpResultTypeDef

```python
# GetStaticIpResultTypeDef definition

class GetStaticIpResultTypeDef(TypedDict):
    staticIp: StaticIpTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StaticIpTypeDef](./type_defs.md#staticiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStaticIpsResultTypeDef

```python
# GetStaticIpsResultTypeDef definition

class GetStaticIpsResultTypeDef(TypedDict):
    staticIps: List[StaticIpTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StaticIpTypeDef](./type_defs.md#staticiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAutoSnapshotsResultTypeDef

```python
# GetAutoSnapshotsResultTypeDef definition

class GetAutoSnapshotsResultTypeDef(TypedDict):
    resourceName: str,
    resourceType: ResourceTypeType,  # (1)
    autoSnapshots: List[AutoSnapshotDetailsTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: AutoSnapshotDetailsTypeDef](./type_defs.md#autosnapshotdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRegionsResultTypeDef

```python
# GetRegionsResultTypeDef definition

class GetRegionsResultTypeDef(TypedDict):
    regions: List[RegionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegionTypeDef](./type_defs.md#regiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBucketResultTypeDef

```python
# CreateBucketResultTypeDef definition

class CreateBucketResultTypeDef(TypedDict):
    bucket: BucketTypeDef,  # (1)
    operations: List[OperationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BucketTypeDef](./type_defs.md#buckettypedef) 
2. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBucketsResultTypeDef

```python
# GetBucketsResultTypeDef definition

class GetBucketsResultTypeDef(TypedDict):
    buckets: List[BucketTypeDef],  # (1)
    nextPageToken: str,
    accountLevelBpaSync: AccountLevelBpaSyncTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BucketTypeDef](./type_defs.md#buckettypedef) 
2. See [:material-code-braces: AccountLevelBpaSyncTypeDef](./type_defs.md#accountlevelbpasynctypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBucketResultTypeDef

```python
# UpdateBucketResultTypeDef definition

class UpdateBucketResultTypeDef(TypedDict):
    bucket: BucketTypeDef,  # (1)
    operations: List[OperationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BucketTypeDef](./type_defs.md#buckettypedef) 
2. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDiskSnapshotResultTypeDef

```python
# GetDiskSnapshotResultTypeDef definition

class GetDiskSnapshotResultTypeDef(TypedDict):
    diskSnapshot: DiskSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DiskSnapshotTypeDef](./type_defs.md#disksnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDiskSnapshotsResultTypeDef

```python
# GetDiskSnapshotsResultTypeDef definition

class GetDiskSnapshotsResultTypeDef(TypedDict):
    diskSnapshots: List[DiskSnapshotTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DiskSnapshotTypeDef](./type_defs.md#disksnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDiskResultTypeDef

```python
# GetDiskResultTypeDef definition

class GetDiskResultTypeDef(TypedDict):
    disk: DiskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DiskTypeDef](./type_defs.md#disktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDisksResultTypeDef

```python
# GetDisksResultTypeDef definition

class GetDisksResultTypeDef(TypedDict):
    disks: List[DiskTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DiskTypeDef](./type_defs.md#disktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceHardwareTypeDef

```python
# InstanceHardwareTypeDef definition

class InstanceHardwareTypeDef(TypedDict):
    cpuCount: NotRequired[int],
    disks: NotRequired[List[DiskTypeDef]],  # (1)
    ramSizeInGb: NotRequired[float],
```

1. See [:material-code-braces: DiskTypeDef](./type_defs.md#disktypedef) 
## InstanceSnapshotTypeDef

```python
# InstanceSnapshotTypeDef definition

class InstanceSnapshotTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    state: NotRequired[InstanceSnapshotStateType],  # (4)
    progress: NotRequired[str],
    fromAttachedDisks: NotRequired[List[DiskTypeDef]],  # (5)
    fromInstanceName: NotRequired[str],
    fromInstanceArn: NotRequired[str],
    fromBlueprintId: NotRequired[str],
    fromBundleId: NotRequired[str],
    isFromAutoSnapshot: NotRequired[bool],
    sizeInGb: NotRequired[int],
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: InstanceSnapshotStateType](./literals.md#instancesnapshotstatetype) 
5. See [:material-code-braces: DiskTypeDef](./type_defs.md#disktypedef) 
## CreateKeyPairResultTypeDef

```python
# CreateKeyPairResultTypeDef definition

class CreateKeyPairResultTypeDef(TypedDict):
    keyPair: KeyPairTypeDef,  # (1)
    publicKeyBase64: str,
    privateKeyBase64: str,
    operation: OperationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: KeyPairTypeDef](./type_defs.md#keypairtypedef) 
2. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKeyPairResultTypeDef

```python
# GetKeyPairResultTypeDef definition

class GetKeyPairResultTypeDef(TypedDict):
    keyPair: KeyPairTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyPairTypeDef](./type_defs.md#keypairtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKeyPairsResultTypeDef

```python
# GetKeyPairsResultTypeDef definition

class GetKeyPairsResultTypeDef(TypedDict):
    keyPairs: List[KeyPairTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KeyPairTypeDef](./type_defs.md#keypairtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRelationalDatabaseSnapshotResultTypeDef

```python
# GetRelationalDatabaseSnapshotResultTypeDef definition

class GetRelationalDatabaseSnapshotResultTypeDef(TypedDict):
    relationalDatabaseSnapshot: RelationalDatabaseSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RelationalDatabaseSnapshotTypeDef](./type_defs.md#relationaldatabasesnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRelationalDatabaseSnapshotsResultTypeDef

```python
# GetRelationalDatabaseSnapshotsResultTypeDef definition

class GetRelationalDatabaseSnapshotsResultTypeDef(TypedDict):
    relationalDatabaseSnapshots: List[RelationalDatabaseSnapshotTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RelationalDatabaseSnapshotTypeDef](./type_defs.md#relationaldatabasesnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LightsailDistributionTypeDef

```python
# LightsailDistributionTypeDef definition

class LightsailDistributionTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    alternativeDomainNames: NotRequired[List[str]],
    status: NotRequired[str],
    isEnabled: NotRequired[bool],
    domainName: NotRequired[str],
    bundleId: NotRequired[str],
    certificateName: NotRequired[str],
    origin: NotRequired[OriginTypeDef],  # (3)
    originPublicDNS: NotRequired[str],
    defaultCacheBehavior: NotRequired[CacheBehaviorTypeDef],  # (4)
    cacheBehaviorSettings: NotRequired[CacheSettingsOutputTypeDef],  # (5)
    cacheBehaviors: NotRequired[List[CacheBehaviorPerPathTypeDef]],  # (6)
    ableToUpdateBundle: NotRequired[bool],
    ipAddressType: NotRequired[IpAddressTypeType],  # (7)
    tags: NotRequired[List[TagTypeDef]],  # (8)
    viewerMinimumTlsProtocolVersion: NotRequired[str],
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: OriginTypeDef](./type_defs.md#origintypedef) 
4. See [:material-code-braces: CacheBehaviorTypeDef](./type_defs.md#cachebehaviortypedef) 
5. See [:material-code-braces: CacheSettingsOutputTypeDef](./type_defs.md#cachesettingsoutputtypedef) 
6. See [:material-code-braces: CacheBehaviorPerPathTypeDef](./type_defs.md#cachebehaviorperpathtypedef) 
7. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetCloudFormationStackRecordsResultTypeDef

```python
# GetCloudFormationStackRecordsResultTypeDef definition

class GetCloudFormationStackRecordsResultTypeDef(TypedDict):
    cloudFormationStackRecords: List[CloudFormationStackRecordTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudFormationStackRecordTypeDef](./type_defs.md#cloudformationstackrecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContainerServiceRequestRequestTypeDef

```python
# UpdateContainerServiceRequestRequestTypeDef definition

class UpdateContainerServiceRequestRequestTypeDef(TypedDict):
    serviceName: str,
    power: NotRequired[ContainerServicePowerNameType],  # (1)
    scale: NotRequired[int],
    isDisabled: NotRequired[bool],
    publicDomainNames: NotRequired[Mapping[str, Sequence[str]]],
    privateRegistryAccess: NotRequired[PrivateRegistryAccessRequestTypeDef],  # (2)
```

1. See [:material-code-brackets: ContainerServicePowerNameType](./literals.md#containerservicepowernametype) 
2. See [:material-code-braces: PrivateRegistryAccessRequestTypeDef](./type_defs.md#privateregistryaccessrequesttypedef) 
## ContainerServiceDeploymentTypeDef

```python
# ContainerServiceDeploymentTypeDef definition

class ContainerServiceDeploymentTypeDef(TypedDict):
    version: NotRequired[int],
    state: NotRequired[ContainerServiceDeploymentStateType],  # (1)
    containers: NotRequired[Dict[str, ContainerOutputTypeDef]],  # (2)
    publicEndpoint: NotRequired[ContainerServiceEndpointTypeDef],  # (3)
    createdAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ContainerServiceDeploymentStateType](./literals.md#containerservicedeploymentstatetype) 
2. See [:material-code-braces: ContainerOutputTypeDef](./type_defs.md#containeroutputtypedef) 
3. See [:material-code-braces: ContainerServiceEndpointTypeDef](./type_defs.md#containerserviceendpointtypedef) 
## ContainerServiceDeploymentRequestTypeDef

```python
# ContainerServiceDeploymentRequestTypeDef definition

class ContainerServiceDeploymentRequestTypeDef(TypedDict):
    containers: NotRequired[Mapping[str, ContainerUnionTypeDef]],  # (1)
    publicEndpoint: NotRequired[EndpointRequestTypeDef],  # (2)
```

1. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) [:material-code-braces: ContainerOutputTypeDef](./type_defs.md#containeroutputtypedef) 
2. See [:material-code-braces: EndpointRequestTypeDef](./type_defs.md#endpointrequesttypedef) 
## CreateContainerServiceDeploymentRequestRequestTypeDef

```python
# CreateContainerServiceDeploymentRequestRequestTypeDef definition

class CreateContainerServiceDeploymentRequestRequestTypeDef(TypedDict):
    serviceName: str,
    containers: NotRequired[Mapping[str, ContainerUnionTypeDef]],  # (1)
    publicEndpoint: NotRequired[EndpointRequestTypeDef],  # (2)
```

1. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) [:material-code-braces: ContainerOutputTypeDef](./type_defs.md#containeroutputtypedef) 
2. See [:material-code-braces: EndpointRequestTypeDef](./type_defs.md#endpointrequesttypedef) 
## ExportSnapshotRecordSourceInfoTypeDef

```python
# ExportSnapshotRecordSourceInfoTypeDef definition

class ExportSnapshotRecordSourceInfoTypeDef(TypedDict):
    resourceType: NotRequired[ExportSnapshotRecordSourceTypeType],  # (1)
    createdAt: NotRequired[datetime],
    name: NotRequired[str],
    arn: NotRequired[str],
    fromResourceName: NotRequired[str],
    fromResourceArn: NotRequired[str],
    instanceSnapshotInfo: NotRequired[InstanceSnapshotInfoTypeDef],  # (2)
    diskSnapshotInfo: NotRequired[DiskSnapshotInfoTypeDef],  # (3)
```

1. See [:material-code-brackets: ExportSnapshotRecordSourceTypeType](./literals.md#exportsnapshotrecordsourcetypetype) 
2. See [:material-code-braces: InstanceSnapshotInfoTypeDef](./type_defs.md#instancesnapshotinfotypedef) 
3. See [:material-code-braces: DiskSnapshotInfoTypeDef](./type_defs.md#disksnapshotinfotypedef) 
## RenewalSummaryTypeDef

```python
# RenewalSummaryTypeDef definition

class RenewalSummaryTypeDef(TypedDict):
    domainValidationRecords: NotRequired[List[DomainValidationRecordTypeDef]],  # (1)
    renewalStatus: NotRequired[RenewalStatusType],  # (2)
    renewalStatusReason: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: DomainValidationRecordTypeDef](./type_defs.md#domainvalidationrecordtypedef) 
2. See [:material-code-brackets: RenewalStatusType](./literals.md#renewalstatustype) 
## CostEstimateTypeDef

```python
# CostEstimateTypeDef definition

class CostEstimateTypeDef(TypedDict):
    usageType: NotRequired[str],
    resultsByTime: NotRequired[List[EstimateByTimeTypeDef]],  # (1)
```

1. See [:material-code-braces: EstimateByTimeTypeDef](./type_defs.md#estimatebytimetypedef) 
## GetInstanceAccessDetailsResultTypeDef

```python
# GetInstanceAccessDetailsResultTypeDef definition

class GetInstanceAccessDetailsResultTypeDef(TypedDict):
    accessDetails: InstanceAccessDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceAccessDetailsTypeDef](./type_defs.md#instanceaccessdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoadBalancerTlsCertificateTypeDef

```python
# LoadBalancerTlsCertificateTypeDef definition

class LoadBalancerTlsCertificateTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    loadBalancerName: NotRequired[str],
    isAttached: NotRequired[bool],
    status: NotRequired[LoadBalancerTlsCertificateStatusType],  # (4)
    domainName: NotRequired[str],
    domainValidationRecords: NotRequired[List[LoadBalancerTlsCertificateDomainValidationRecordTypeDef]],  # (5)
    failureReason: NotRequired[LoadBalancerTlsCertificateFailureReasonType],  # (6)
    issuedAt: NotRequired[datetime],
    issuer: NotRequired[str],
    keyAlgorithm: NotRequired[str],
    notAfter: NotRequired[datetime],
    notBefore: NotRequired[datetime],
    renewalSummary: NotRequired[LoadBalancerTlsCertificateRenewalSummaryTypeDef],  # (7)
    revocationReason: NotRequired[LoadBalancerTlsCertificateRevocationReasonType],  # (8)
    revokedAt: NotRequired[datetime],
    serial: NotRequired[str],
    signatureAlgorithm: NotRequired[str],
    subject: NotRequired[str],
    subjectAlternativeNames: NotRequired[List[str]],
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: LoadBalancerTlsCertificateStatusType](./literals.md#loadbalancertlscertificatestatustype) 
5. See [:material-code-braces: LoadBalancerTlsCertificateDomainValidationRecordTypeDef](./type_defs.md#loadbalancertlscertificatedomainvalidationrecordtypedef) 
6. See [:material-code-brackets: LoadBalancerTlsCertificateFailureReasonType](./literals.md#loadbalancertlscertificatefailurereasontype) 
7. See [:material-code-braces: LoadBalancerTlsCertificateRenewalSummaryTypeDef](./type_defs.md#loadbalancertlscertificaterenewalsummarytypedef) 
8. See [:material-code-brackets: LoadBalancerTlsCertificateRevocationReasonType](./literals.md#loadbalancertlscertificaterevocationreasontype) 
## GetLoadBalancerResultTypeDef

```python
# GetLoadBalancerResultTypeDef definition

class GetLoadBalancerResultTypeDef(TypedDict):
    loadBalancer: LoadBalancerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLoadBalancersResultTypeDef

```python
# GetLoadBalancersResultTypeDef definition

class GetLoadBalancersResultTypeDef(TypedDict):
    loadBalancers: List[LoadBalancerTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CacheSettingsTypeDef

```python
# CacheSettingsTypeDef definition

class CacheSettingsTypeDef(TypedDict):
    defaultTTL: NotRequired[int],
    minimumTTL: NotRequired[int],
    maximumTTL: NotRequired[int],
    allowedHTTPMethods: NotRequired[str],
    cachedHTTPMethods: NotRequired[str],
    forwardedCookies: NotRequired[CookieObjectUnionTypeDef],  # (1)
    forwardedHeaders: NotRequired[HeaderObjectUnionTypeDef],  # (2)
    forwardedQueryStrings: NotRequired[QueryStringObjectUnionTypeDef],  # (3)
```

1. See [:material-code-braces: CookieObjectTypeDef](./type_defs.md#cookieobjecttypedef) [:material-code-braces: CookieObjectOutputTypeDef](./type_defs.md#cookieobjectoutputtypedef) 
2. See [:material-code-braces: HeaderObjectTypeDef](./type_defs.md#headerobjecttypedef) [:material-code-braces: HeaderObjectOutputTypeDef](./type_defs.md#headerobjectoutputtypedef) 
3. See [:material-code-braces: QueryStringObjectTypeDef](./type_defs.md#querystringobjecttypedef) [:material-code-braces: QueryStringObjectOutputTypeDef](./type_defs.md#querystringobjectoutputtypedef) 
## DomainTypeDef

```python
# DomainTypeDef definition

class DomainTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    domainEntries: NotRequired[List[DomainEntryOutputTypeDef]],  # (4)
    registeredDomainDelegationInfo: NotRequired[RegisteredDomainDelegationInfoTypeDef],  # (5)
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: DomainEntryOutputTypeDef](./type_defs.md#domainentryoutputtypedef) 
5. See [:material-code-braces: RegisteredDomainDelegationInfoTypeDef](./type_defs.md#registereddomaindelegationinfotypedef) 
## GetRelationalDatabaseResultTypeDef

```python
# GetRelationalDatabaseResultTypeDef definition

class GetRelationalDatabaseResultTypeDef(TypedDict):
    relationalDatabase: RelationalDatabaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RelationalDatabaseTypeDef](./type_defs.md#relationaldatabasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRelationalDatabasesResultTypeDef

```python
# GetRelationalDatabasesResultTypeDef definition

class GetRelationalDatabasesResultTypeDef(TypedDict):
    relationalDatabases: List[RelationalDatabaseTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RelationalDatabaseTypeDef](./type_defs.md#relationaldatabasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSetupHistoryResultTypeDef

```python
# GetSetupHistoryResultTypeDef definition

class GetSetupHistoryResultTypeDef(TypedDict):
    setupHistory: List[SetupHistoryTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SetupHistoryTypeDef](./type_defs.md#setuphistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    supportCode: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    blueprintId: NotRequired[str],
    blueprintName: NotRequired[str],
    bundleId: NotRequired[str],
    addOns: NotRequired[List[AddOnTypeDef]],  # (4)
    isStaticIp: NotRequired[bool],
    privateIpAddress: NotRequired[str],
    publicIpAddress: NotRequired[str],
    ipv6Addresses: NotRequired[List[str]],
    ipAddressType: NotRequired[IpAddressTypeType],  # (5)
    hardware: NotRequired[InstanceHardwareTypeDef],  # (6)
    networking: NotRequired[InstanceNetworkingTypeDef],  # (7)
    state: NotRequired[InstanceStateTypeDef],  # (8)
    username: NotRequired[str],
    sshKeyName: NotRequired[str],
    metadataOptions: NotRequired[InstanceMetadataOptionsTypeDef],  # (9)
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: AddOnTypeDef](./type_defs.md#addontypedef) 
5. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
6. See [:material-code-braces: InstanceHardwareTypeDef](./type_defs.md#instancehardwaretypedef) 
7. See [:material-code-braces: InstanceNetworkingTypeDef](./type_defs.md#instancenetworkingtypedef) 
8. See [:material-code-braces: InstanceStateTypeDef](./type_defs.md#instancestatetypedef) 
9. See [:material-code-braces: InstanceMetadataOptionsTypeDef](./type_defs.md#instancemetadataoptionstypedef) 
## GetInstanceSnapshotResultTypeDef

```python
# GetInstanceSnapshotResultTypeDef definition

class GetInstanceSnapshotResultTypeDef(TypedDict):
    instanceSnapshot: InstanceSnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceSnapshotTypeDef](./type_defs.md#instancesnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstanceSnapshotsResultTypeDef

```python
# GetInstanceSnapshotsResultTypeDef definition

class GetInstanceSnapshotsResultTypeDef(TypedDict):
    instanceSnapshots: List[InstanceSnapshotTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceSnapshotTypeDef](./type_defs.md#instancesnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDistributionResultTypeDef

```python
# CreateDistributionResultTypeDef definition

class CreateDistributionResultTypeDef(TypedDict):
    distribution: LightsailDistributionTypeDef,  # (1)
    operation: OperationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: LightsailDistributionTypeDef](./type_defs.md#lightsaildistributiontypedef) 
2. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDistributionsResultTypeDef

```python
# GetDistributionsResultTypeDef definition

class GetDistributionsResultTypeDef(TypedDict):
    distributions: List[LightsailDistributionTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LightsailDistributionTypeDef](./type_defs.md#lightsaildistributiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContainerServiceTypeDef

```python
# ContainerServiceTypeDef definition

class ContainerServiceTypeDef(TypedDict):
    containerServiceName: NotRequired[str],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
    power: NotRequired[ContainerServicePowerNameType],  # (4)
    powerId: NotRequired[str],
    state: NotRequired[ContainerServiceStateType],  # (5)
    stateDetail: NotRequired[ContainerServiceStateDetailTypeDef],  # (6)
    scale: NotRequired[int],
    currentDeployment: NotRequired[ContainerServiceDeploymentTypeDef],  # (7)
    nextDeployment: NotRequired[ContainerServiceDeploymentTypeDef],  # (7)
    isDisabled: NotRequired[bool],
    principalArn: NotRequired[str],
    privateDomainName: NotRequired[str],
    publicDomainNames: NotRequired[Dict[str, List[str]]],
    url: NotRequired[str],
    privateRegistryAccess: NotRequired[PrivateRegistryAccessTypeDef],  # (9)
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: ContainerServicePowerNameType](./literals.md#containerservicepowernametype) 
5. See [:material-code-brackets: ContainerServiceStateType](./literals.md#containerservicestatetype) 
6. See [:material-code-braces: ContainerServiceStateDetailTypeDef](./type_defs.md#containerservicestatedetailtypedef) 
7. See [:material-code-braces: ContainerServiceDeploymentTypeDef](./type_defs.md#containerservicedeploymenttypedef) 
8. See [:material-code-braces: ContainerServiceDeploymentTypeDef](./type_defs.md#containerservicedeploymenttypedef) 
9. See [:material-code-braces: PrivateRegistryAccessTypeDef](./type_defs.md#privateregistryaccesstypedef) 
## GetContainerServiceDeploymentsResultTypeDef

```python
# GetContainerServiceDeploymentsResultTypeDef definition

class GetContainerServiceDeploymentsResultTypeDef(TypedDict):
    deployments: List[ContainerServiceDeploymentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerServiceDeploymentTypeDef](./type_defs.md#containerservicedeploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContainerServiceRequestRequestTypeDef

```python
# CreateContainerServiceRequestRequestTypeDef definition

class CreateContainerServiceRequestRequestTypeDef(TypedDict):
    serviceName: str,
    power: ContainerServicePowerNameType,  # (1)
    scale: int,
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    publicDomainNames: NotRequired[Mapping[str, Sequence[str]]],
    deployment: NotRequired[ContainerServiceDeploymentRequestTypeDef],  # (3)
    privateRegistryAccess: NotRequired[PrivateRegistryAccessRequestTypeDef],  # (4)
```

1. See [:material-code-brackets: ContainerServicePowerNameType](./literals.md#containerservicepowernametype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ContainerServiceDeploymentRequestTypeDef](./type_defs.md#containerservicedeploymentrequesttypedef) 
4. See [:material-code-braces: PrivateRegistryAccessRequestTypeDef](./type_defs.md#privateregistryaccessrequesttypedef) 
## ExportSnapshotRecordTypeDef

```python
# ExportSnapshotRecordTypeDef definition

class ExportSnapshotRecordTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    location: NotRequired[ResourceLocationTypeDef],  # (1)
    resourceType: NotRequired[ResourceTypeType],  # (2)
    state: NotRequired[RecordStateType],  # (3)
    sourceInfo: NotRequired[ExportSnapshotRecordSourceInfoTypeDef],  # (4)
    destinationInfo: NotRequired[DestinationInfoTypeDef],  # (5)
```

1. See [:material-code-braces: ResourceLocationTypeDef](./type_defs.md#resourcelocationtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-brackets: RecordStateType](./literals.md#recordstatetype) 
4. See [:material-code-braces: ExportSnapshotRecordSourceInfoTypeDef](./type_defs.md#exportsnapshotrecordsourceinfotypedef) 
5. See [:material-code-braces: DestinationInfoTypeDef](./type_defs.md#destinationinfotypedef) 
## CertificateTypeDef

```python
# CertificateTypeDef definition

class CertificateTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    domainName: NotRequired[str],
    status: NotRequired[CertificateStatusType],  # (1)
    serialNumber: NotRequired[str],
    subjectAlternativeNames: NotRequired[List[str]],
    domainValidationRecords: NotRequired[List[DomainValidationRecordTypeDef]],  # (2)
    requestFailureReason: NotRequired[str],
    inUseResourceCount: NotRequired[int],
    keyAlgorithm: NotRequired[str],
    createdAt: NotRequired[datetime],
    issuedAt: NotRequired[datetime],
    issuerCA: NotRequired[str],
    notBefore: NotRequired[datetime],
    notAfter: NotRequired[datetime],
    eligibleToRenew: NotRequired[str],
    renewalSummary: NotRequired[RenewalSummaryTypeDef],  # (3)
    revokedAt: NotRequired[datetime],
    revocationReason: NotRequired[str],
    tags: NotRequired[List[TagTypeDef]],  # (4)
    supportCode: NotRequired[str],
```

1. See [:material-code-brackets: CertificateStatusType](./literals.md#certificatestatustype) 
2. See [:material-code-braces: DomainValidationRecordTypeDef](./type_defs.md#domainvalidationrecordtypedef) 
3. See [:material-code-braces: RenewalSummaryTypeDef](./type_defs.md#renewalsummarytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ResourceBudgetEstimateTypeDef

```python
# ResourceBudgetEstimateTypeDef definition

class ResourceBudgetEstimateTypeDef(TypedDict):
    resourceName: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (1)
    costEstimates: NotRequired[List[CostEstimateTypeDef]],  # (2)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: CostEstimateTypeDef](./type_defs.md#costestimatetypedef) 
## GetLoadBalancerTlsCertificatesResultTypeDef

```python
# GetLoadBalancerTlsCertificatesResultTypeDef definition

class GetLoadBalancerTlsCertificatesResultTypeDef(TypedDict):
    tlsCertificates: List[LoadBalancerTlsCertificateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoadBalancerTlsCertificateTypeDef](./type_defs.md#loadbalancertlscertificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDistributionRequestRequestTypeDef

```python
# CreateDistributionRequestRequestTypeDef definition

class CreateDistributionRequestRequestTypeDef(TypedDict):
    distributionName: str,
    origin: InputOriginTypeDef,  # (1)
    defaultCacheBehavior: CacheBehaviorTypeDef,  # (2)
    bundleId: str,
    cacheBehaviorSettings: NotRequired[CacheSettingsTypeDef],  # (3)
    cacheBehaviors: NotRequired[Sequence[CacheBehaviorPerPathTypeDef]],  # (4)
    ipAddressType: NotRequired[IpAddressTypeType],  # (5)
    tags: NotRequired[Sequence[TagTypeDef]],  # (6)
    certificateName: NotRequired[str],
    viewerMinimumTlsProtocolVersion: NotRequired[ViewerMinimumTlsProtocolVersionEnumType],  # (7)
```

1. See [:material-code-braces: InputOriginTypeDef](./type_defs.md#inputorigintypedef) 
2. See [:material-code-braces: CacheBehaviorTypeDef](./type_defs.md#cachebehaviortypedef) 
3. See [:material-code-braces: CacheSettingsTypeDef](./type_defs.md#cachesettingstypedef) 
4. See [:material-code-braces: CacheBehaviorPerPathTypeDef](./type_defs.md#cachebehaviorperpathtypedef) 
5. See [:material-code-brackets: IpAddressTypeType](./literals.md#ipaddresstypetype) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-brackets: ViewerMinimumTlsProtocolVersionEnumType](./literals.md#viewerminimumtlsprotocolversionenumtype) 
## UpdateDistributionRequestRequestTypeDef

```python
# UpdateDistributionRequestRequestTypeDef definition

class UpdateDistributionRequestRequestTypeDef(TypedDict):
    distributionName: str,
    origin: NotRequired[InputOriginTypeDef],  # (1)
    defaultCacheBehavior: NotRequired[CacheBehaviorTypeDef],  # (2)
    cacheBehaviorSettings: NotRequired[CacheSettingsTypeDef],  # (3)
    cacheBehaviors: NotRequired[Sequence[CacheBehaviorPerPathTypeDef]],  # (4)
    isEnabled: NotRequired[bool],
    viewerMinimumTlsProtocolVersion: NotRequired[ViewerMinimumTlsProtocolVersionEnumType],  # (5)
    certificateName: NotRequired[str],
    useDefaultCertificate: NotRequired[bool],
```

1. See [:material-code-braces: InputOriginTypeDef](./type_defs.md#inputorigintypedef) 
2. See [:material-code-braces: CacheBehaviorTypeDef](./type_defs.md#cachebehaviortypedef) 
3. See [:material-code-braces: CacheSettingsTypeDef](./type_defs.md#cachesettingstypedef) 
4. See [:material-code-braces: CacheBehaviorPerPathTypeDef](./type_defs.md#cachebehaviorperpathtypedef) 
5. See [:material-code-brackets: ViewerMinimumTlsProtocolVersionEnumType](./literals.md#viewerminimumtlsprotocolversionenumtype) 
## GetDomainResultTypeDef

```python
# GetDomainResultTypeDef definition

class GetDomainResultTypeDef(TypedDict):
    domain: DomainTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainTypeDef](./type_defs.md#domaintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDomainsResultTypeDef

```python
# GetDomainsResultTypeDef definition

class GetDomainsResultTypeDef(TypedDict):
    domains: List[DomainTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainTypeDef](./type_defs.md#domaintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstanceResultTypeDef

```python
# GetInstanceResultTypeDef definition

class GetInstanceResultTypeDef(TypedDict):
    instance: InstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstancesResultTypeDef

```python
# GetInstancesResultTypeDef definition

class GetInstancesResultTypeDef(TypedDict):
    instances: List[InstanceTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContainerServicesListResultTypeDef

```python
# ContainerServicesListResultTypeDef definition

class ContainerServicesListResultTypeDef(TypedDict):
    containerServices: List[ContainerServiceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerServiceTypeDef](./type_defs.md#containerservicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContainerServiceDeploymentResultTypeDef

```python
# CreateContainerServiceDeploymentResultTypeDef definition

class CreateContainerServiceDeploymentResultTypeDef(TypedDict):
    containerService: ContainerServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerServiceTypeDef](./type_defs.md#containerservicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContainerServiceResultTypeDef

```python
# CreateContainerServiceResultTypeDef definition

class CreateContainerServiceResultTypeDef(TypedDict):
    containerService: ContainerServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerServiceTypeDef](./type_defs.md#containerservicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContainerServiceResultTypeDef

```python
# UpdateContainerServiceResultTypeDef definition

class UpdateContainerServiceResultTypeDef(TypedDict):
    containerService: ContainerServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerServiceTypeDef](./type_defs.md#containerservicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExportSnapshotRecordsResultTypeDef

```python
# GetExportSnapshotRecordsResultTypeDef definition

class GetExportSnapshotRecordsResultTypeDef(TypedDict):
    exportSnapshotRecords: List[ExportSnapshotRecordTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportSnapshotRecordTypeDef](./type_defs.md#exportsnapshotrecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CertificateSummaryTypeDef

```python
# CertificateSummaryTypeDef definition

class CertificateSummaryTypeDef(TypedDict):
    certificateArn: NotRequired[str],
    certificateName: NotRequired[str],
    domainName: NotRequired[str],
    certificateDetail: NotRequired[CertificateTypeDef],  # (1)
    tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetCostEstimateResultTypeDef

```python
# GetCostEstimateResultTypeDef definition

class GetCostEstimateResultTypeDef(TypedDict):
    resourcesBudgetEstimate: List[ResourceBudgetEstimateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceBudgetEstimateTypeDef](./type_defs.md#resourcebudgetestimatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCertificateResultTypeDef

```python
# CreateCertificateResultTypeDef definition

class CreateCertificateResultTypeDef(TypedDict):
    certificate: CertificateSummaryTypeDef,  # (1)
    operations: List[OperationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CertificateSummaryTypeDef](./type_defs.md#certificatesummarytypedef) 
2. See [:material-code-braces: OperationTypeDef](./type_defs.md#operationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCertificatesResultTypeDef

```python
# GetCertificatesResultTypeDef definition

class GetCertificatesResultTypeDef(TypedDict):
    certificates: List[CertificateSummaryTypeDef],  # (1)
    nextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CertificateSummaryTypeDef](./type_defs.md#certificatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
