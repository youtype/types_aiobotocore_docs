# Type definitions

> [Index](../README.md) > [RedshiftServerless](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RedshiftServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#redshiftserverless)
    type annotations stubs module [types-aiobotocore-redshift-serverless](https://pypi.org/project/types-aiobotocore-redshift-serverless/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## CreateSnapshotScheduleActionParametersUnionTypeDef

```python
# CreateSnapshotScheduleActionParametersUnionTypeDef definition

CreateSnapshotScheduleActionParametersUnionTypeDef = Union[
    CreateSnapshotScheduleActionParametersTypeDef,  # (1)
    CreateSnapshotScheduleActionParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CreateSnapshotScheduleActionParametersTypeDef](./type_defs.md#createsnapshotscheduleactionparameterstypedef) 
2. See [:material-code-braces: CreateSnapshotScheduleActionParametersOutputTypeDef](./type_defs.md#createsnapshotscheduleactionparametersoutputtypedef) 



## AssociationTypeDef

```python
# AssociationTypeDef definition

class AssociationTypeDef(TypedDict):
    customDomainCertificateArn: NotRequired[str],
    customDomainCertificateExpiryTime: NotRequired[datetime],
    customDomainName: NotRequired[str],
    workgroupName: NotRequired[str],
```

## ConfigParameterTypeDef

```python
# ConfigParameterTypeDef definition

class ConfigParameterTypeDef(TypedDict):
    parameterKey: NotRequired[str],
    parameterValue: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
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

## SnapshotTypeDef

```python
# SnapshotTypeDef definition

class SnapshotTypeDef(TypedDict):
    accountsWithProvisionedRestoreAccess: NotRequired[List[str]],
    accountsWithRestoreAccess: NotRequired[List[str]],
    actualIncrementalBackupSizeInMegaBytes: NotRequired[float],
    adminPasswordSecretArn: NotRequired[str],
    adminPasswordSecretKmsKeyId: NotRequired[str],
    adminUsername: NotRequired[str],
    backupProgressInMegaBytes: NotRequired[float],
    currentBackupRateInMegaBytesPerSecond: NotRequired[float],
    elapsedTimeInSeconds: NotRequired[int],
    estimatedSecondsToCompletion: NotRequired[int],
    kmsKeyId: NotRequired[str],
    namespaceArn: NotRequired[str],
    namespaceName: NotRequired[str],
    ownerAccount: NotRequired[str],
    snapshotArn: NotRequired[str],
    snapshotCreateTime: NotRequired[datetime],
    snapshotName: NotRequired[str],
    snapshotRemainingDays: NotRequired[int],
    snapshotRetentionPeriod: NotRequired[int],
    snapshotRetentionStartTime: NotRequired[datetime],
    status: NotRequired[SnapshotStatusType],  # (1)
    totalBackupSizeInMegaBytes: NotRequired[float],
```

1. See [:material-code-brackets: SnapshotStatusType](./literals.md#snapshotstatustype) 
## CreateCustomDomainAssociationRequestRequestTypeDef

```python
# CreateCustomDomainAssociationRequestRequestTypeDef definition

class CreateCustomDomainAssociationRequestRequestTypeDef(TypedDict):
    customDomainCertificateArn: str,
    customDomainName: str,
    workgroupName: str,
```

## CreateEndpointAccessRequestRequestTypeDef

```python
# CreateEndpointAccessRequestRequestTypeDef definition

class CreateEndpointAccessRequestRequestTypeDef(TypedDict):
    endpointName: str,
    subnetIds: Sequence[str],
    workgroupName: str,
    ownerAccount: NotRequired[str],
    vpcSecurityGroupIds: NotRequired[Sequence[str]],
```

## NamespaceTypeDef

```python
# NamespaceTypeDef definition

class NamespaceTypeDef(TypedDict):
    adminPasswordSecretArn: NotRequired[str],
    adminPasswordSecretKmsKeyId: NotRequired[str],
    adminUsername: NotRequired[str],
    creationDate: NotRequired[datetime],
    dbName: NotRequired[str],
    defaultIamRoleArn: NotRequired[str],
    iamRoles: NotRequired[List[str]],
    kmsKeyId: NotRequired[str],
    logExports: NotRequired[List[LogExportType]],  # (1)
    namespaceArn: NotRequired[str],
    namespaceId: NotRequired[str],
    namespaceName: NotRequired[str],
    status: NotRequired[NamespaceStatusType],  # (2)
```

1. See [:material-code-brackets: LogExportType](./literals.md#logexporttype) 
2. See [:material-code-brackets: NamespaceStatusType](./literals.md#namespacestatustype) 
## CreateSnapshotCopyConfigurationRequestRequestTypeDef

```python
# CreateSnapshotCopyConfigurationRequestRequestTypeDef definition

class CreateSnapshotCopyConfigurationRequestRequestTypeDef(TypedDict):
    destinationRegion: str,
    namespaceName: str,
    destinationKmsKeyId: NotRequired[str],
    snapshotRetentionPeriod: NotRequired[int],
```

## SnapshotCopyConfigurationTypeDef

```python
# SnapshotCopyConfigurationTypeDef definition

class SnapshotCopyConfigurationTypeDef(TypedDict):
    destinationKmsKeyId: NotRequired[str],
    destinationRegion: NotRequired[str],
    namespaceName: NotRequired[str],
    snapshotCopyConfigurationArn: NotRequired[str],
    snapshotCopyConfigurationId: NotRequired[str],
    snapshotRetentionPeriod: NotRequired[int],
```

## CreateUsageLimitRequestRequestTypeDef

```python
# CreateUsageLimitRequestRequestTypeDef definition

class CreateUsageLimitRequestRequestTypeDef(TypedDict):
    amount: int,
    resourceArn: str,
    usageType: UsageLimitUsageTypeType,  # (1)
    breachAction: NotRequired[UsageLimitBreachActionType],  # (2)
    period: NotRequired[UsageLimitPeriodType],  # (3)
```

1. See [:material-code-brackets: UsageLimitUsageTypeType](./literals.md#usagelimitusagetypetype) 
2. See [:material-code-brackets: UsageLimitBreachActionType](./literals.md#usagelimitbreachactiontype) 
3. See [:material-code-brackets: UsageLimitPeriodType](./literals.md#usagelimitperiodtype) 
## UsageLimitTypeDef

```python
# UsageLimitTypeDef definition

class UsageLimitTypeDef(TypedDict):
    amount: NotRequired[int],
    breachAction: NotRequired[UsageLimitBreachActionType],  # (1)
    period: NotRequired[UsageLimitPeriodType],  # (2)
    resourceArn: NotRequired[str],
    usageLimitArn: NotRequired[str],
    usageLimitId: NotRequired[str],
    usageType: NotRequired[UsageLimitUsageTypeType],  # (3)
```

1. See [:material-code-brackets: UsageLimitBreachActionType](./literals.md#usagelimitbreachactiontype) 
2. See [:material-code-brackets: UsageLimitPeriodType](./literals.md#usagelimitperiodtype) 
3. See [:material-code-brackets: UsageLimitUsageTypeType](./literals.md#usagelimitusagetypetype) 
## PerformanceTargetTypeDef

```python
# PerformanceTargetTypeDef definition

class PerformanceTargetTypeDef(TypedDict):
    level: NotRequired[int],
    status: NotRequired[PerformanceTargetStatusType],  # (1)
```

1. See [:material-code-brackets: PerformanceTargetStatusType](./literals.md#performancetargetstatustype) 
## DeleteCustomDomainAssociationRequestRequestTypeDef

```python
# DeleteCustomDomainAssociationRequestRequestTypeDef definition

class DeleteCustomDomainAssociationRequestRequestTypeDef(TypedDict):
    customDomainName: str,
    workgroupName: str,
```

## DeleteEndpointAccessRequestRequestTypeDef

```python
# DeleteEndpointAccessRequestRequestTypeDef definition

class DeleteEndpointAccessRequestRequestTypeDef(TypedDict):
    endpointName: str,
```

## DeleteNamespaceRequestRequestTypeDef

```python
# DeleteNamespaceRequestRequestTypeDef definition

class DeleteNamespaceRequestRequestTypeDef(TypedDict):
    namespaceName: str,
    finalSnapshotName: NotRequired[str],
    finalSnapshotRetentionPeriod: NotRequired[int],
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## DeleteScheduledActionRequestRequestTypeDef

```python
# DeleteScheduledActionRequestRequestTypeDef definition

class DeleteScheduledActionRequestRequestTypeDef(TypedDict):
    scheduledActionName: str,
```

## DeleteSnapshotCopyConfigurationRequestRequestTypeDef

```python
# DeleteSnapshotCopyConfigurationRequestRequestTypeDef definition

class DeleteSnapshotCopyConfigurationRequestRequestTypeDef(TypedDict):
    snapshotCopyConfigurationId: str,
```

## DeleteSnapshotRequestRequestTypeDef

```python
# DeleteSnapshotRequestRequestTypeDef definition

class DeleteSnapshotRequestRequestTypeDef(TypedDict):
    snapshotName: str,
```

## DeleteUsageLimitRequestRequestTypeDef

```python
# DeleteUsageLimitRequestRequestTypeDef definition

class DeleteUsageLimitRequestRequestTypeDef(TypedDict):
    usageLimitId: str,
```

## DeleteWorkgroupRequestRequestTypeDef

```python
# DeleteWorkgroupRequestRequestTypeDef definition

class DeleteWorkgroupRequestRequestTypeDef(TypedDict):
    workgroupName: str,
```

## VpcSecurityGroupMembershipTypeDef

```python
# VpcSecurityGroupMembershipTypeDef definition

class VpcSecurityGroupMembershipTypeDef(TypedDict):
    status: NotRequired[str],
    vpcSecurityGroupId: NotRequired[str],
```

## GetCredentialsRequestRequestTypeDef

```python
# GetCredentialsRequestRequestTypeDef definition

class GetCredentialsRequestRequestTypeDef(TypedDict):
    customDomainName: NotRequired[str],
    dbName: NotRequired[str],
    durationSeconds: NotRequired[int],
    workgroupName: NotRequired[str],
```

## GetCustomDomainAssociationRequestRequestTypeDef

```python
# GetCustomDomainAssociationRequestRequestTypeDef definition

class GetCustomDomainAssociationRequestRequestTypeDef(TypedDict):
    customDomainName: str,
    workgroupName: str,
```

## GetEndpointAccessRequestRequestTypeDef

```python
# GetEndpointAccessRequestRequestTypeDef definition

class GetEndpointAccessRequestRequestTypeDef(TypedDict):
    endpointName: str,
```

## GetNamespaceRequestRequestTypeDef

```python
# GetNamespaceRequestRequestTypeDef definition

class GetNamespaceRequestRequestTypeDef(TypedDict):
    namespaceName: str,
```

## GetRecoveryPointRequestRequestTypeDef

```python
# GetRecoveryPointRequestRequestTypeDef definition

class GetRecoveryPointRequestRequestTypeDef(TypedDict):
    recoveryPointId: str,
```

## RecoveryPointTypeDef

```python
# RecoveryPointTypeDef definition

class RecoveryPointTypeDef(TypedDict):
    namespaceArn: NotRequired[str],
    namespaceName: NotRequired[str],
    recoveryPointCreateTime: NotRequired[datetime],
    recoveryPointId: NotRequired[str],
    totalSizeInMegaBytes: NotRequired[float],
    workgroupName: NotRequired[str],
```

## GetResourcePolicyRequestRequestTypeDef

```python
# GetResourcePolicyRequestRequestTypeDef definition

class GetResourcePolicyRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ResourcePolicyTypeDef

```python
# ResourcePolicyTypeDef definition

class ResourcePolicyTypeDef(TypedDict):
    policy: NotRequired[str],
    resourceArn: NotRequired[str],
```

## GetScheduledActionRequestRequestTypeDef

```python
# GetScheduledActionRequestRequestTypeDef definition

class GetScheduledActionRequestRequestTypeDef(TypedDict):
    scheduledActionName: str,
```

## GetSnapshotRequestRequestTypeDef

```python
# GetSnapshotRequestRequestTypeDef definition

class GetSnapshotRequestRequestTypeDef(TypedDict):
    ownerAccount: NotRequired[str],
    snapshotArn: NotRequired[str],
    snapshotName: NotRequired[str],
```

## GetTableRestoreStatusRequestRequestTypeDef

```python
# GetTableRestoreStatusRequestRequestTypeDef definition

class GetTableRestoreStatusRequestRequestTypeDef(TypedDict):
    tableRestoreRequestId: str,
```

## TableRestoreStatusTypeDef

```python
# TableRestoreStatusTypeDef definition

class TableRestoreStatusTypeDef(TypedDict):
    message: NotRequired[str],
    namespaceName: NotRequired[str],
    newTableName: NotRequired[str],
    progressInMegaBytes: NotRequired[int],
    recoveryPointId: NotRequired[str],
    requestTime: NotRequired[datetime],
    snapshotName: NotRequired[str],
    sourceDatabaseName: NotRequired[str],
    sourceSchemaName: NotRequired[str],
    sourceTableName: NotRequired[str],
    status: NotRequired[str],
    tableRestoreRequestId: NotRequired[str],
    targetDatabaseName: NotRequired[str],
    targetSchemaName: NotRequired[str],
    totalDataInMegaBytes: NotRequired[int],
    workgroupName: NotRequired[str],
```

## GetUsageLimitRequestRequestTypeDef

```python
# GetUsageLimitRequestRequestTypeDef definition

class GetUsageLimitRequestRequestTypeDef(TypedDict):
    usageLimitId: str,
```

## GetWorkgroupRequestRequestTypeDef

```python
# GetWorkgroupRequestRequestTypeDef definition

class GetWorkgroupRequestRequestTypeDef(TypedDict):
    workgroupName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListCustomDomainAssociationsRequestRequestTypeDef

```python
# ListCustomDomainAssociationsRequestRequestTypeDef definition

class ListCustomDomainAssociationsRequestRequestTypeDef(TypedDict):
    customDomainCertificateArn: NotRequired[str],
    customDomainName: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListEndpointAccessRequestRequestTypeDef

```python
# ListEndpointAccessRequestRequestTypeDef definition

class ListEndpointAccessRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    ownerAccount: NotRequired[str],
    vpcId: NotRequired[str],
    workgroupName: NotRequired[str],
```

## ListManagedWorkgroupsRequestRequestTypeDef

```python
# ListManagedWorkgroupsRequestRequestTypeDef definition

class ListManagedWorkgroupsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sourceArn: NotRequired[str],
```

## ManagedWorkgroupListItemTypeDef

```python
# ManagedWorkgroupListItemTypeDef definition

class ManagedWorkgroupListItemTypeDef(TypedDict):
    creationDate: NotRequired[datetime],
    managedWorkgroupId: NotRequired[str],
    managedWorkgroupName: NotRequired[str],
    sourceArn: NotRequired[str],
    status: NotRequired[ManagedWorkgroupStatusType],  # (1)
```

1. See [:material-code-brackets: ManagedWorkgroupStatusType](./literals.md#managedworkgroupstatustype) 
## ListNamespacesRequestRequestTypeDef

```python
# ListNamespacesRequestRequestTypeDef definition

class ListNamespacesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListScheduledActionsRequestRequestTypeDef

```python
# ListScheduledActionsRequestRequestTypeDef definition

class ListScheduledActionsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    namespaceName: NotRequired[str],
    nextToken: NotRequired[str],
```

## ScheduledActionAssociationTypeDef

```python
# ScheduledActionAssociationTypeDef definition

class ScheduledActionAssociationTypeDef(TypedDict):
    namespaceName: NotRequired[str],
    scheduledActionName: NotRequired[str],
```

## ListSnapshotCopyConfigurationsRequestRequestTypeDef

```python
# ListSnapshotCopyConfigurationsRequestRequestTypeDef definition

class ListSnapshotCopyConfigurationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    namespaceName: NotRequired[str],
    nextToken: NotRequired[str],
```

## ListTableRestoreStatusRequestRequestTypeDef

```python
# ListTableRestoreStatusRequestRequestTypeDef definition

class ListTableRestoreStatusRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    namespaceName: NotRequired[str],
    nextToken: NotRequired[str],
    workgroupName: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListUsageLimitsRequestRequestTypeDef

```python
# ListUsageLimitsRequestRequestTypeDef definition

class ListUsageLimitsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    resourceArn: NotRequired[str],
    usageType: NotRequired[UsageLimitUsageTypeType],  # (1)
```

1. See [:material-code-brackets: UsageLimitUsageTypeType](./literals.md#usagelimitusagetypetype) 
## ListWorkgroupsRequestRequestTypeDef

```python
# ListWorkgroupsRequestRequestTypeDef definition

class ListWorkgroupsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    ownerAccount: NotRequired[str],
```

## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    availabilityZone: NotRequired[str],
    ipv6Address: NotRequired[str],
    networkInterfaceId: NotRequired[str],
    privateIpAddress: NotRequired[str],
    subnetId: NotRequired[str],
```

## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    policy: str,
    resourceArn: str,
```

## RestoreFromRecoveryPointRequestRequestTypeDef

```python
# RestoreFromRecoveryPointRequestRequestTypeDef definition

class RestoreFromRecoveryPointRequestRequestTypeDef(TypedDict):
    namespaceName: str,
    recoveryPointId: str,
    workgroupName: str,
```

## RestoreFromSnapshotRequestRequestTypeDef

```python
# RestoreFromSnapshotRequestRequestTypeDef definition

class RestoreFromSnapshotRequestRequestTypeDef(TypedDict):
    namespaceName: str,
    workgroupName: str,
    adminPasswordSecretKmsKeyId: NotRequired[str],
    manageAdminPassword: NotRequired[bool],
    ownerAccount: NotRequired[str],
    snapshotArn: NotRequired[str],
    snapshotName: NotRequired[str],
```

## RestoreTableFromRecoveryPointRequestRequestTypeDef

```python
# RestoreTableFromRecoveryPointRequestRequestTypeDef definition

class RestoreTableFromRecoveryPointRequestRequestTypeDef(TypedDict):
    namespaceName: str,
    newTableName: str,
    recoveryPointId: str,
    sourceDatabaseName: str,
    sourceTableName: str,
    workgroupName: str,
    activateCaseSensitiveIdentifier: NotRequired[bool],
    sourceSchemaName: NotRequired[str],
    targetDatabaseName: NotRequired[str],
    targetSchemaName: NotRequired[str],
```

## RestoreTableFromSnapshotRequestRequestTypeDef

```python
# RestoreTableFromSnapshotRequestRequestTypeDef definition

class RestoreTableFromSnapshotRequestRequestTypeDef(TypedDict):
    namespaceName: str,
    newTableName: str,
    snapshotName: str,
    sourceDatabaseName: str,
    sourceTableName: str,
    workgroupName: str,
    activateCaseSensitiveIdentifier: NotRequired[bool],
    sourceSchemaName: NotRequired[str],
    targetDatabaseName: NotRequired[str],
    targetSchemaName: NotRequired[str],
```

## ScheduleOutputTypeDef

```python
# ScheduleOutputTypeDef definition

class ScheduleOutputTypeDef(TypedDict):
    at: NotRequired[datetime],
    cron: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateCustomDomainAssociationRequestRequestTypeDef

```python
# UpdateCustomDomainAssociationRequestRequestTypeDef definition

class UpdateCustomDomainAssociationRequestRequestTypeDef(TypedDict):
    customDomainCertificateArn: str,
    customDomainName: str,
    workgroupName: str,
```

## UpdateEndpointAccessRequestRequestTypeDef

```python
# UpdateEndpointAccessRequestRequestTypeDef definition

class UpdateEndpointAccessRequestRequestTypeDef(TypedDict):
    endpointName: str,
    vpcSecurityGroupIds: NotRequired[Sequence[str]],
```

## UpdateNamespaceRequestRequestTypeDef

```python
# UpdateNamespaceRequestRequestTypeDef definition

class UpdateNamespaceRequestRequestTypeDef(TypedDict):
    namespaceName: str,
    adminPasswordSecretKmsKeyId: NotRequired[str],
    adminUserPassword: NotRequired[str],
    adminUsername: NotRequired[str],
    defaultIamRoleArn: NotRequired[str],
    iamRoles: NotRequired[Sequence[str]],
    kmsKeyId: NotRequired[str],
    logExports: NotRequired[Sequence[LogExportType]],  # (1)
    manageAdminPassword: NotRequired[bool],
```

1. See [:material-code-brackets: LogExportType](./literals.md#logexporttype) 
## UpdateSnapshotCopyConfigurationRequestRequestTypeDef

```python
# UpdateSnapshotCopyConfigurationRequestRequestTypeDef definition

class UpdateSnapshotCopyConfigurationRequestRequestTypeDef(TypedDict):
    snapshotCopyConfigurationId: str,
    snapshotRetentionPeriod: NotRequired[int],
```

## UpdateSnapshotRequestRequestTypeDef

```python
# UpdateSnapshotRequestRequestTypeDef definition

class UpdateSnapshotRequestRequestTypeDef(TypedDict):
    snapshotName: str,
    retentionPeriod: NotRequired[int],
```

## UpdateUsageLimitRequestRequestTypeDef

```python
# UpdateUsageLimitRequestRequestTypeDef definition

class UpdateUsageLimitRequestRequestTypeDef(TypedDict):
    usageLimitId: str,
    amount: NotRequired[int],
    breachAction: NotRequired[UsageLimitBreachActionType],  # (1)
```

1. See [:material-code-brackets: UsageLimitBreachActionType](./literals.md#usagelimitbreachactiontype) 
## ConvertRecoveryPointToSnapshotRequestRequestTypeDef

```python
# ConvertRecoveryPointToSnapshotRequestRequestTypeDef definition

class ConvertRecoveryPointToSnapshotRequestRequestTypeDef(TypedDict):
    recoveryPointId: str,
    snapshotName: str,
    retentionPeriod: NotRequired[int],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateNamespaceRequestRequestTypeDef

```python
# CreateNamespaceRequestRequestTypeDef definition

class CreateNamespaceRequestRequestTypeDef(TypedDict):
    namespaceName: str,
    adminPasswordSecretKmsKeyId: NotRequired[str],
    adminUserPassword: NotRequired[str],
    adminUsername: NotRequired[str],
    dbName: NotRequired[str],
    defaultIamRoleArn: NotRequired[str],
    iamRoles: NotRequired[Sequence[str]],
    kmsKeyId: NotRequired[str],
    logExports: NotRequired[Sequence[LogExportType]],  # (1)
    manageAdminPassword: NotRequired[bool],
    redshiftIdcApplicationArn: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: LogExportType](./literals.md#logexporttype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSnapshotRequestRequestTypeDef

```python
# CreateSnapshotRequestRequestTypeDef definition

class CreateSnapshotRequestRequestTypeDef(TypedDict):
    namespaceName: str,
    snapshotName: str,
    retentionPeriod: NotRequired[int],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSnapshotScheduleActionParametersOutputTypeDef

```python
# CreateSnapshotScheduleActionParametersOutputTypeDef definition

class CreateSnapshotScheduleActionParametersOutputTypeDef(TypedDict):
    namespaceName: str,
    snapshotNamePrefix: str,
    retentionPeriod: NotRequired[int],
    tags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSnapshotScheduleActionParametersTypeDef

```python
# CreateSnapshotScheduleActionParametersTypeDef definition

class CreateSnapshotScheduleActionParametersTypeDef(TypedDict):
    namespaceName: str,
    snapshotNamePrefix: str,
    retentionPeriod: NotRequired[int],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateCustomDomainAssociationResponseTypeDef

```python
# CreateCustomDomainAssociationResponseTypeDef definition

class CreateCustomDomainAssociationResponseTypeDef(TypedDict):
    customDomainCertificateArn: str,
    customDomainCertificateExpiryTime: datetime,
    customDomainName: str,
    workgroupName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCredentialsResponseTypeDef

```python
# GetCredentialsResponseTypeDef definition

class GetCredentialsResponseTypeDef(TypedDict):
    dbPassword: str,
    dbUser: str,
    expiration: datetime,
    nextRefreshTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCustomDomainAssociationResponseTypeDef

```python
# GetCustomDomainAssociationResponseTypeDef definition

class GetCustomDomainAssociationResponseTypeDef(TypedDict):
    customDomainCertificateArn: str,
    customDomainCertificateExpiryTime: datetime,
    customDomainName: str,
    workgroupName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomDomainAssociationsResponseTypeDef

```python
# ListCustomDomainAssociationsResponseTypeDef definition

class ListCustomDomainAssociationsResponseTypeDef(TypedDict):
    associations: List[AssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociationTypeDef](./type_defs.md#associationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCustomDomainAssociationResponseTypeDef

```python
# UpdateCustomDomainAssociationResponseTypeDef definition

class UpdateCustomDomainAssociationResponseTypeDef(TypedDict):
    customDomainCertificateArn: str,
    customDomainCertificateExpiryTime: datetime,
    customDomainName: str,
    workgroupName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConvertRecoveryPointToSnapshotResponseTypeDef

```python
# ConvertRecoveryPointToSnapshotResponseTypeDef definition

class ConvertRecoveryPointToSnapshotResponseTypeDef(TypedDict):
    snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSnapshotResponseTypeDef

```python
# CreateSnapshotResponseTypeDef definition

class CreateSnapshotResponseTypeDef(TypedDict):
    snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSnapshotResponseTypeDef

```python
# DeleteSnapshotResponseTypeDef definition

class DeleteSnapshotResponseTypeDef(TypedDict):
    snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSnapshotResponseTypeDef

```python
# GetSnapshotResponseTypeDef definition

class GetSnapshotResponseTypeDef(TypedDict):
    snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSnapshotsResponseTypeDef

```python
# ListSnapshotsResponseTypeDef definition

class ListSnapshotsResponseTypeDef(TypedDict):
    snapshots: List[SnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSnapshotResponseTypeDef

```python
# UpdateSnapshotResponseTypeDef definition

class UpdateSnapshotResponseTypeDef(TypedDict):
    snapshot: SnapshotTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNamespaceResponseTypeDef

```python
# CreateNamespaceResponseTypeDef definition

class CreateNamespaceResponseTypeDef(TypedDict):
    namespace: NamespaceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamespaceTypeDef](./type_defs.md#namespacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteNamespaceResponseTypeDef

```python
# DeleteNamespaceResponseTypeDef definition

class DeleteNamespaceResponseTypeDef(TypedDict):
    namespace: NamespaceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamespaceTypeDef](./type_defs.md#namespacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNamespaceResponseTypeDef

```python
# GetNamespaceResponseTypeDef definition

class GetNamespaceResponseTypeDef(TypedDict):
    namespace: NamespaceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamespaceTypeDef](./type_defs.md#namespacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNamespacesResponseTypeDef

```python
# ListNamespacesResponseTypeDef definition

class ListNamespacesResponseTypeDef(TypedDict):
    namespaces: List[NamespaceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NamespaceTypeDef](./type_defs.md#namespacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreFromRecoveryPointResponseTypeDef

```python
# RestoreFromRecoveryPointResponseTypeDef definition

class RestoreFromRecoveryPointResponseTypeDef(TypedDict):
    namespace: NamespaceTypeDef,  # (1)
    recoveryPointId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamespaceTypeDef](./type_defs.md#namespacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreFromSnapshotResponseTypeDef

```python
# RestoreFromSnapshotResponseTypeDef definition

class RestoreFromSnapshotResponseTypeDef(TypedDict):
    namespace: NamespaceTypeDef,  # (1)
    ownerAccount: str,
    snapshotName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamespaceTypeDef](./type_defs.md#namespacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNamespaceResponseTypeDef

```python
# UpdateNamespaceResponseTypeDef definition

class UpdateNamespaceResponseTypeDef(TypedDict):
    namespace: NamespaceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamespaceTypeDef](./type_defs.md#namespacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecoveryPointsRequestRequestTypeDef

```python
# ListRecoveryPointsRequestRequestTypeDef definition

class ListRecoveryPointsRequestRequestTypeDef(TypedDict):
    endTime: NotRequired[TimestampTypeDef],
    maxResults: NotRequired[int],
    namespaceArn: NotRequired[str],
    namespaceName: NotRequired[str],
    nextToken: NotRequired[str],
    startTime: NotRequired[TimestampTypeDef],
```

## ListSnapshotsRequestRequestTypeDef

```python
# ListSnapshotsRequestRequestTypeDef definition

class ListSnapshotsRequestRequestTypeDef(TypedDict):
    endTime: NotRequired[TimestampTypeDef],
    maxResults: NotRequired[int],
    namespaceArn: NotRequired[str],
    namespaceName: NotRequired[str],
    nextToken: NotRequired[str],
    ownerAccount: NotRequired[str],
    startTime: NotRequired[TimestampTypeDef],
```

## ScheduleTypeDef

```python
# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    at: NotRequired[TimestampTypeDef],
    cron: NotRequired[str],
```

## CreateSnapshotCopyConfigurationResponseTypeDef

```python
# CreateSnapshotCopyConfigurationResponseTypeDef definition

class CreateSnapshotCopyConfigurationResponseTypeDef(TypedDict):
    snapshotCopyConfiguration: SnapshotCopyConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotCopyConfigurationTypeDef](./type_defs.md#snapshotcopyconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSnapshotCopyConfigurationResponseTypeDef

```python
# DeleteSnapshotCopyConfigurationResponseTypeDef definition

class DeleteSnapshotCopyConfigurationResponseTypeDef(TypedDict):
    snapshotCopyConfiguration: SnapshotCopyConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotCopyConfigurationTypeDef](./type_defs.md#snapshotcopyconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSnapshotCopyConfigurationsResponseTypeDef

```python
# ListSnapshotCopyConfigurationsResponseTypeDef definition

class ListSnapshotCopyConfigurationsResponseTypeDef(TypedDict):
    snapshotCopyConfigurations: List[SnapshotCopyConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SnapshotCopyConfigurationTypeDef](./type_defs.md#snapshotcopyconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSnapshotCopyConfigurationResponseTypeDef

```python
# UpdateSnapshotCopyConfigurationResponseTypeDef definition

class UpdateSnapshotCopyConfigurationResponseTypeDef(TypedDict):
    snapshotCopyConfiguration: SnapshotCopyConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotCopyConfigurationTypeDef](./type_defs.md#snapshotcopyconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUsageLimitResponseTypeDef

```python
# CreateUsageLimitResponseTypeDef definition

class CreateUsageLimitResponseTypeDef(TypedDict):
    usageLimit: UsageLimitTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UsageLimitTypeDef](./type_defs.md#usagelimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteUsageLimitResponseTypeDef

```python
# DeleteUsageLimitResponseTypeDef definition

class DeleteUsageLimitResponseTypeDef(TypedDict):
    usageLimit: UsageLimitTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UsageLimitTypeDef](./type_defs.md#usagelimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUsageLimitResponseTypeDef

```python
# GetUsageLimitResponseTypeDef definition

class GetUsageLimitResponseTypeDef(TypedDict):
    usageLimit: UsageLimitTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UsageLimitTypeDef](./type_defs.md#usagelimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsageLimitsResponseTypeDef

```python
# ListUsageLimitsResponseTypeDef definition

class ListUsageLimitsResponseTypeDef(TypedDict):
    usageLimits: List[UsageLimitTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: UsageLimitTypeDef](./type_defs.md#usagelimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUsageLimitResponseTypeDef

```python
# UpdateUsageLimitResponseTypeDef definition

class UpdateUsageLimitResponseTypeDef(TypedDict):
    usageLimit: UsageLimitTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UsageLimitTypeDef](./type_defs.md#usagelimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkgroupRequestRequestTypeDef

```python
# CreateWorkgroupRequestRequestTypeDef definition

class CreateWorkgroupRequestRequestTypeDef(TypedDict):
    namespaceName: str,
    workgroupName: str,
    baseCapacity: NotRequired[int],
    configParameters: NotRequired[Sequence[ConfigParameterTypeDef]],  # (1)
    enhancedVpcRouting: NotRequired[bool],
    ipAddressType: NotRequired[str],
    maxCapacity: NotRequired[int],
    port: NotRequired[int],
    pricePerformanceTarget: NotRequired[PerformanceTargetTypeDef],  # (2)
    publiclyAccessible: NotRequired[bool],
    securityGroupIds: NotRequired[Sequence[str]],
    subnetIds: NotRequired[Sequence[str]],
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: ConfigParameterTypeDef](./type_defs.md#configparametertypedef) 
2. See [:material-code-braces: PerformanceTargetTypeDef](./type_defs.md#performancetargettypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateWorkgroupRequestRequestTypeDef

```python
# UpdateWorkgroupRequestRequestTypeDef definition

class UpdateWorkgroupRequestRequestTypeDef(TypedDict):
    workgroupName: str,
    baseCapacity: NotRequired[int],
    configParameters: NotRequired[Sequence[ConfigParameterTypeDef]],  # (1)
    enhancedVpcRouting: NotRequired[bool],
    ipAddressType: NotRequired[str],
    maxCapacity: NotRequired[int],
    port: NotRequired[int],
    pricePerformanceTarget: NotRequired[PerformanceTargetTypeDef],  # (2)
    publiclyAccessible: NotRequired[bool],
    securityGroupIds: NotRequired[Sequence[str]],
    subnetIds: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ConfigParameterTypeDef](./type_defs.md#configparametertypedef) 
2. See [:material-code-braces: PerformanceTargetTypeDef](./type_defs.md#performancetargettypedef) 
## GetRecoveryPointResponseTypeDef

```python
# GetRecoveryPointResponseTypeDef definition

class GetRecoveryPointResponseTypeDef(TypedDict):
    recoveryPoint: RecoveryPointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecoveryPointTypeDef](./type_defs.md#recoverypointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecoveryPointsResponseTypeDef

```python
# ListRecoveryPointsResponseTypeDef definition

class ListRecoveryPointsResponseTypeDef(TypedDict):
    recoveryPoints: List[RecoveryPointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecoveryPointTypeDef](./type_defs.md#recoverypointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    resourcePolicy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResponseTypeDef

```python
# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    resourcePolicy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableRestoreStatusResponseTypeDef

```python
# GetTableRestoreStatusResponseTypeDef definition

class GetTableRestoreStatusResponseTypeDef(TypedDict):
    tableRestoreStatus: TableRestoreStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableRestoreStatusTypeDef](./type_defs.md#tablerestorestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTableRestoreStatusResponseTypeDef

```python
# ListTableRestoreStatusResponseTypeDef definition

class ListTableRestoreStatusResponseTypeDef(TypedDict):
    tableRestoreStatuses: List[TableRestoreStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TableRestoreStatusTypeDef](./type_defs.md#tablerestorestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreTableFromRecoveryPointResponseTypeDef

```python
# RestoreTableFromRecoveryPointResponseTypeDef definition

class RestoreTableFromRecoveryPointResponseTypeDef(TypedDict):
    tableRestoreStatus: TableRestoreStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableRestoreStatusTypeDef](./type_defs.md#tablerestorestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreTableFromSnapshotResponseTypeDef

```python
# RestoreTableFromSnapshotResponseTypeDef definition

class RestoreTableFromSnapshotResponseTypeDef(TypedDict):
    tableRestoreStatus: TableRestoreStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableRestoreStatusTypeDef](./type_defs.md#tablerestorestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomDomainAssociationsRequestPaginateTypeDef

```python
# ListCustomDomainAssociationsRequestPaginateTypeDef definition

class ListCustomDomainAssociationsRequestPaginateTypeDef(TypedDict):
    customDomainCertificateArn: NotRequired[str],
    customDomainName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEndpointAccessRequestPaginateTypeDef

```python
# ListEndpointAccessRequestPaginateTypeDef definition

class ListEndpointAccessRequestPaginateTypeDef(TypedDict):
    ownerAccount: NotRequired[str],
    vpcId: NotRequired[str],
    workgroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedWorkgroupsRequestPaginateTypeDef

```python
# ListManagedWorkgroupsRequestPaginateTypeDef definition

class ListManagedWorkgroupsRequestPaginateTypeDef(TypedDict):
    sourceArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNamespacesRequestPaginateTypeDef

```python
# ListNamespacesRequestPaginateTypeDef definition

class ListNamespacesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecoveryPointsRequestPaginateTypeDef

```python
# ListRecoveryPointsRequestPaginateTypeDef definition

class ListRecoveryPointsRequestPaginateTypeDef(TypedDict):
    endTime: NotRequired[TimestampTypeDef],
    namespaceArn: NotRequired[str],
    namespaceName: NotRequired[str],
    startTime: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListScheduledActionsRequestPaginateTypeDef

```python
# ListScheduledActionsRequestPaginateTypeDef definition

class ListScheduledActionsRequestPaginateTypeDef(TypedDict):
    namespaceName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSnapshotCopyConfigurationsRequestPaginateTypeDef

```python
# ListSnapshotCopyConfigurationsRequestPaginateTypeDef definition

class ListSnapshotCopyConfigurationsRequestPaginateTypeDef(TypedDict):
    namespaceName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSnapshotsRequestPaginateTypeDef

```python
# ListSnapshotsRequestPaginateTypeDef definition

class ListSnapshotsRequestPaginateTypeDef(TypedDict):
    endTime: NotRequired[TimestampTypeDef],
    namespaceArn: NotRequired[str],
    namespaceName: NotRequired[str],
    ownerAccount: NotRequired[str],
    startTime: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTableRestoreStatusRequestPaginateTypeDef

```python
# ListTableRestoreStatusRequestPaginateTypeDef definition

class ListTableRestoreStatusRequestPaginateTypeDef(TypedDict):
    namespaceName: NotRequired[str],
    workgroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsageLimitsRequestPaginateTypeDef

```python
# ListUsageLimitsRequestPaginateTypeDef definition

class ListUsageLimitsRequestPaginateTypeDef(TypedDict):
    resourceArn: NotRequired[str],
    usageType: NotRequired[UsageLimitUsageTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: UsageLimitUsageTypeType](./literals.md#usagelimitusagetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkgroupsRequestPaginateTypeDef

```python
# ListWorkgroupsRequestPaginateTypeDef definition

class ListWorkgroupsRequestPaginateTypeDef(TypedDict):
    ownerAccount: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedWorkgroupsResponseTypeDef

```python
# ListManagedWorkgroupsResponseTypeDef definition

class ListManagedWorkgroupsResponseTypeDef(TypedDict):
    managedWorkgroups: List[ManagedWorkgroupListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ManagedWorkgroupListItemTypeDef](./type_defs.md#managedworkgrouplistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListScheduledActionsResponseTypeDef

```python
# ListScheduledActionsResponseTypeDef definition

class ListScheduledActionsResponseTypeDef(TypedDict):
    scheduledActions: List[ScheduledActionAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ScheduledActionAssociationTypeDef](./type_defs.md#scheduledactionassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VpcEndpointTypeDef

```python
# VpcEndpointTypeDef definition

class VpcEndpointTypeDef(TypedDict):
    networkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (1)
    vpcEndpointId: NotRequired[str],
    vpcId: NotRequired[str],
```

1. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
## TargetActionOutputTypeDef

```python
# TargetActionOutputTypeDef definition

class TargetActionOutputTypeDef(TypedDict):
    createSnapshot: NotRequired[CreateSnapshotScheduleActionParametersOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CreateSnapshotScheduleActionParametersOutputTypeDef](./type_defs.md#createsnapshotscheduleactionparametersoutputtypedef) 
## EndpointAccessTypeDef

```python
# EndpointAccessTypeDef definition

class EndpointAccessTypeDef(TypedDict):
    address: NotRequired[str],
    endpointArn: NotRequired[str],
    endpointCreateTime: NotRequired[datetime],
    endpointName: NotRequired[str],
    endpointStatus: NotRequired[str],
    port: NotRequired[int],
    subnetIds: NotRequired[List[str]],
    vpcEndpoint: NotRequired[VpcEndpointTypeDef],  # (1)
    vpcSecurityGroups: NotRequired[List[VpcSecurityGroupMembershipTypeDef]],  # (2)
    workgroupName: NotRequired[str],
```

1. See [:material-code-braces: VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef) 
2. See [:material-code-braces: VpcSecurityGroupMembershipTypeDef](./type_defs.md#vpcsecuritygroupmembershiptypedef) 
## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    address: NotRequired[str],
    port: NotRequired[int],
    vpcEndpoints: NotRequired[List[VpcEndpointTypeDef]],  # (1)
```

1. See [:material-code-braces: VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef) 
## ScheduledActionResponseTypeDef

```python
# ScheduledActionResponseTypeDef definition

class ScheduledActionResponseTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    namespaceName: NotRequired[str],
    nextInvocations: NotRequired[List[datetime]],
    roleArn: NotRequired[str],
    schedule: NotRequired[ScheduleOutputTypeDef],  # (1)
    scheduledActionDescription: NotRequired[str],
    scheduledActionName: NotRequired[str],
    scheduledActionUuid: NotRequired[str],
    startTime: NotRequired[datetime],
    state: NotRequired[StateType],  # (2)
    targetAction: NotRequired[TargetActionOutputTypeDef],  # (3)
```

1. See [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
2. See [:material-code-brackets: StateType](./literals.md#statetype) 
3. See [:material-code-braces: TargetActionOutputTypeDef](./type_defs.md#targetactionoutputtypedef) 
## TargetActionTypeDef

```python
# TargetActionTypeDef definition

class TargetActionTypeDef(TypedDict):
    createSnapshot: NotRequired[CreateSnapshotScheduleActionParametersUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CreateSnapshotScheduleActionParametersTypeDef](./type_defs.md#createsnapshotscheduleactionparameterstypedef) [:material-code-braces: CreateSnapshotScheduleActionParametersOutputTypeDef](./type_defs.md#createsnapshotscheduleactionparametersoutputtypedef) 
## CreateEndpointAccessResponseTypeDef

```python
# CreateEndpointAccessResponseTypeDef definition

class CreateEndpointAccessResponseTypeDef(TypedDict):
    endpoint: EndpointAccessTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointAccessTypeDef](./type_defs.md#endpointaccesstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEndpointAccessResponseTypeDef

```python
# DeleteEndpointAccessResponseTypeDef definition

class DeleteEndpointAccessResponseTypeDef(TypedDict):
    endpoint: EndpointAccessTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointAccessTypeDef](./type_defs.md#endpointaccesstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEndpointAccessResponseTypeDef

```python
# GetEndpointAccessResponseTypeDef definition

class GetEndpointAccessResponseTypeDef(TypedDict):
    endpoint: EndpointAccessTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointAccessTypeDef](./type_defs.md#endpointaccesstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEndpointAccessResponseTypeDef

```python
# ListEndpointAccessResponseTypeDef definition

class ListEndpointAccessResponseTypeDef(TypedDict):
    endpoints: List[EndpointAccessTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EndpointAccessTypeDef](./type_defs.md#endpointaccesstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEndpointAccessResponseTypeDef

```python
# UpdateEndpointAccessResponseTypeDef definition

class UpdateEndpointAccessResponseTypeDef(TypedDict):
    endpoint: EndpointAccessTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointAccessTypeDef](./type_defs.md#endpointaccesstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkgroupTypeDef

```python
# WorkgroupTypeDef definition

class WorkgroupTypeDef(TypedDict):
    baseCapacity: NotRequired[int],
    configParameters: NotRequired[List[ConfigParameterTypeDef]],  # (1)
    creationDate: NotRequired[datetime],
    crossAccountVpcs: NotRequired[List[str]],
    customDomainCertificateArn: NotRequired[str],
    customDomainCertificateExpiryTime: NotRequired[datetime],
    customDomainName: NotRequired[str],
    endpoint: NotRequired[EndpointTypeDef],  # (2)
    enhancedVpcRouting: NotRequired[bool],
    ipAddressType: NotRequired[str],
    maxCapacity: NotRequired[int],
    namespaceName: NotRequired[str],
    patchVersion: NotRequired[str],
    port: NotRequired[int],
    pricePerformanceTarget: NotRequired[PerformanceTargetTypeDef],  # (3)
    publiclyAccessible: NotRequired[bool],
    securityGroupIds: NotRequired[List[str]],
    status: NotRequired[WorkgroupStatusType],  # (4)
    subnetIds: NotRequired[List[str]],
    workgroupArn: NotRequired[str],
    workgroupId: NotRequired[str],
    workgroupName: NotRequired[str],
    workgroupVersion: NotRequired[str],
```

1. See [:material-code-braces: ConfigParameterTypeDef](./type_defs.md#configparametertypedef) 
2. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
3. See [:material-code-braces: PerformanceTargetTypeDef](./type_defs.md#performancetargettypedef) 
4. See [:material-code-brackets: WorkgroupStatusType](./literals.md#workgroupstatustype) 
## CreateScheduledActionResponseTypeDef

```python
# CreateScheduledActionResponseTypeDef definition

class CreateScheduledActionResponseTypeDef(TypedDict):
    scheduledAction: ScheduledActionResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduledActionResponseTypeDef](./type_defs.md#scheduledactionresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteScheduledActionResponseTypeDef

```python
# DeleteScheduledActionResponseTypeDef definition

class DeleteScheduledActionResponseTypeDef(TypedDict):
    scheduledAction: ScheduledActionResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduledActionResponseTypeDef](./type_defs.md#scheduledactionresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetScheduledActionResponseTypeDef

```python
# GetScheduledActionResponseTypeDef definition

class GetScheduledActionResponseTypeDef(TypedDict):
    scheduledAction: ScheduledActionResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduledActionResponseTypeDef](./type_defs.md#scheduledactionresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateScheduledActionResponseTypeDef

```python
# UpdateScheduledActionResponseTypeDef definition

class UpdateScheduledActionResponseTypeDef(TypedDict):
    scheduledAction: ScheduledActionResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduledActionResponseTypeDef](./type_defs.md#scheduledactionresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScheduledActionRequestRequestTypeDef

```python
# CreateScheduledActionRequestRequestTypeDef definition

class CreateScheduledActionRequestRequestTypeDef(TypedDict):
    namespaceName: str,
    roleArn: str,
    schedule: ScheduleTypeDef,  # (1)
    scheduledActionName: str,
    targetAction: TargetActionTypeDef,  # (2)
    enabled: NotRequired[bool],
    endTime: NotRequired[TimestampTypeDef],
    scheduledActionDescription: NotRequired[str],
    startTime: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
2. See [:material-code-braces: TargetActionTypeDef](./type_defs.md#targetactiontypedef) 
## UpdateScheduledActionRequestRequestTypeDef

```python
# UpdateScheduledActionRequestRequestTypeDef definition

class UpdateScheduledActionRequestRequestTypeDef(TypedDict):
    scheduledActionName: str,
    enabled: NotRequired[bool],
    endTime: NotRequired[TimestampTypeDef],
    roleArn: NotRequired[str],
    schedule: NotRequired[ScheduleTypeDef],  # (1)
    scheduledActionDescription: NotRequired[str],
    startTime: NotRequired[TimestampTypeDef],
    targetAction: NotRequired[TargetActionTypeDef],  # (2)
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
2. See [:material-code-braces: TargetActionTypeDef](./type_defs.md#targetactiontypedef) 
## CreateWorkgroupResponseTypeDef

```python
# CreateWorkgroupResponseTypeDef definition

class CreateWorkgroupResponseTypeDef(TypedDict):
    workgroup: WorkgroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkgroupTypeDef](./type_defs.md#workgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkgroupResponseTypeDef

```python
# DeleteWorkgroupResponseTypeDef definition

class DeleteWorkgroupResponseTypeDef(TypedDict):
    workgroup: WorkgroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkgroupTypeDef](./type_defs.md#workgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkgroupResponseTypeDef

```python
# GetWorkgroupResponseTypeDef definition

class GetWorkgroupResponseTypeDef(TypedDict):
    workgroup: WorkgroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkgroupTypeDef](./type_defs.md#workgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkgroupsResponseTypeDef

```python
# ListWorkgroupsResponseTypeDef definition

class ListWorkgroupsResponseTypeDef(TypedDict):
    workgroups: List[WorkgroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkgroupTypeDef](./type_defs.md#workgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkgroupResponseTypeDef

```python
# UpdateWorkgroupResponseTypeDef definition

class UpdateWorkgroupResponseTypeDef(TypedDict):
    workgroup: WorkgroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkgroupTypeDef](./type_defs.md#workgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
