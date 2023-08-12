# Type definitions

> [Index](../README.md) > [RedshiftServerless](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RedshiftServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
    type annotations stubs module [types-aiobotocore-redshift-serverless](https://pypi.org/project/types-aiobotocore-redshift-serverless/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
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
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## SnapshotTypeDef

```python
# SnapshotTypeDef definition

class SnapshotTypeDef(TypedDict):
    accountsWithProvisionedRestoreAccess: NotRequired[List[str]],
    accountsWithRestoreAccess: NotRequired[List[str]],
    actualIncrementalBackupSizeInMegaBytes: NotRequired[float],
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
## CreateEndpointAccessRequestRequestTypeDef

```python
# CreateEndpointAccessRequestRequestTypeDef definition

class CreateEndpointAccessRequestRequestTypeDef(TypedDict):
    endpointName: str,
    subnetIds: Sequence[str],
    workgroupName: str,
    vpcSecurityGroupIds: NotRequired[Sequence[str]],
```

## NamespaceTypeDef

```python
# NamespaceTypeDef definition

class NamespaceTypeDef(TypedDict):
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
    workgroupName: str,
    dbName: NotRequired[str],
    durationSeconds: NotRequired[int],
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

## ListEndpointAccessRequestRequestTypeDef

```python
# ListEndpointAccessRequestRequestTypeDef definition

class ListEndpointAccessRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    vpcId: NotRequired[str],
    workgroupName: NotRequired[str],
```

## ListNamespacesRequestRequestTypeDef

```python
# ListNamespacesRequestRequestTypeDef definition

class ListNamespacesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
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
```

## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    availabilityZone: NotRequired[str],
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
    ownerAccount: NotRequired[str],
    snapshotArn: NotRequired[str],
    snapshotName: NotRequired[str],
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

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
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
    adminUserPassword: NotRequired[str],
    adminUsername: NotRequired[str],
    defaultIamRoleArn: NotRequired[str],
    iamRoles: NotRequired[Sequence[str]],
    kmsKeyId: NotRequired[str],
    logExports: NotRequired[Sequence[LogExportType]],  # (1)
```

1. See [:material-code-brackets: LogExportType](./literals.md#logexporttype) 
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
## UpdateWorkgroupRequestRequestTypeDef

```python
# UpdateWorkgroupRequestRequestTypeDef definition

class UpdateWorkgroupRequestRequestTypeDef(TypedDict):
    workgroupName: str,
    baseCapacity: NotRequired[int],
    configParameters: NotRequired[Sequence[ConfigParameterTypeDef]],  # (1)
    enhancedVpcRouting: NotRequired[bool],
    port: NotRequired[int],
    publiclyAccessible: NotRequired[bool],
    securityGroupIds: NotRequired[Sequence[str]],
    subnetIds: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ConfigParameterTypeDef](./type_defs.md#configparametertypedef) 
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
    adminUserPassword: NotRequired[str],
    adminUsername: NotRequired[str],
    dbName: NotRequired[str],
    defaultIamRoleArn: NotRequired[str],
    iamRoles: NotRequired[Sequence[str]],
    kmsKeyId: NotRequired[str],
    logExports: NotRequired[Sequence[LogExportType]],  # (1)
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
## CreateWorkgroupRequestRequestTypeDef

```python
# CreateWorkgroupRequestRequestTypeDef definition

class CreateWorkgroupRequestRequestTypeDef(TypedDict):
    namespaceName: str,
    workgroupName: str,
    baseCapacity: NotRequired[int],
    configParameters: NotRequired[Sequence[ConfigParameterTypeDef]],  # (1)
    enhancedVpcRouting: NotRequired[bool],
    port: NotRequired[int],
    publiclyAccessible: NotRequired[bool],
    securityGroupIds: NotRequired[Sequence[str]],
    subnetIds: NotRequired[Sequence[str]],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ConfigParameterTypeDef](./type_defs.md#configparametertypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
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
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    nextToken: str,
    snapshots: List[SnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    nextToken: str,
    usageLimits: List[UsageLimitTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    nextToken: str,
    recoveryPoints: List[RecoveryPointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    nextToken: str,
    tableRestoreStatuses: List[TableRestoreStatusTypeDef],  # (1)
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
## ListEndpointAccessRequestListEndpointAccessPaginateTypeDef

```python
# ListEndpointAccessRequestListEndpointAccessPaginateTypeDef definition

class ListEndpointAccessRequestListEndpointAccessPaginateTypeDef(TypedDict):
    vpcId: NotRequired[str],
    workgroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNamespacesRequestListNamespacesPaginateTypeDef

```python
# ListNamespacesRequestListNamespacesPaginateTypeDef definition

class ListNamespacesRequestListNamespacesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef

```python
# ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef definition

class ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef(TypedDict):
    namespaceName: NotRequired[str],
    workgroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsageLimitsRequestListUsageLimitsPaginateTypeDef

```python
# ListUsageLimitsRequestListUsageLimitsPaginateTypeDef definition

class ListUsageLimitsRequestListUsageLimitsPaginateTypeDef(TypedDict):
    resourceArn: NotRequired[str],
    usageType: NotRequired[UsageLimitUsageTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: UsageLimitUsageTypeType](./literals.md#usagelimitusagetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkgroupsRequestListWorkgroupsPaginateTypeDef

```python
# ListWorkgroupsRequestListWorkgroupsPaginateTypeDef definition

class ListWorkgroupsRequestListWorkgroupsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef

```python
# ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef definition

class ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef(TypedDict):
    endTime: NotRequired[Union[datetime, str]],
    namespaceArn: NotRequired[str],
    namespaceName: NotRequired[str],
    startTime: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecoveryPointsRequestRequestTypeDef

```python
# ListRecoveryPointsRequestRequestTypeDef definition

class ListRecoveryPointsRequestRequestTypeDef(TypedDict):
    endTime: NotRequired[Union[datetime, str]],
    maxResults: NotRequired[int],
    namespaceArn: NotRequired[str],
    namespaceName: NotRequired[str],
    nextToken: NotRequired[str],
    startTime: NotRequired[Union[datetime, str]],
```

## ListSnapshotsRequestListSnapshotsPaginateTypeDef

```python
# ListSnapshotsRequestListSnapshotsPaginateTypeDef definition

class ListSnapshotsRequestListSnapshotsPaginateTypeDef(TypedDict):
    endTime: NotRequired[Union[datetime, str]],
    namespaceArn: NotRequired[str],
    namespaceName: NotRequired[str],
    ownerAccount: NotRequired[str],
    startTime: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSnapshotsRequestRequestTypeDef

```python
# ListSnapshotsRequestRequestTypeDef definition

class ListSnapshotsRequestRequestTypeDef(TypedDict):
    endTime: NotRequired[Union[datetime, str]],
    maxResults: NotRequired[int],
    namespaceArn: NotRequired[str],
    namespaceName: NotRequired[str],
    nextToken: NotRequired[str],
    ownerAccount: NotRequired[str],
    startTime: NotRequired[Union[datetime, str]],
```

## VpcEndpointTypeDef

```python
# VpcEndpointTypeDef definition

class VpcEndpointTypeDef(TypedDict):
    networkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (1)
    vpcEndpointId: NotRequired[str],
    vpcId: NotRequired[str],
```

1. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    endpoint: NotRequired[EndpointTypeDef],  # (2)
    enhancedVpcRouting: NotRequired[bool],
    namespaceName: NotRequired[str],
    port: NotRequired[int],
    publiclyAccessible: NotRequired[bool],
    securityGroupIds: NotRequired[List[str]],
    status: NotRequired[WorkgroupStatusType],  # (3)
    subnetIds: NotRequired[List[str]],
    workgroupArn: NotRequired[str],
    workgroupId: NotRequired[str],
    workgroupName: NotRequired[str],
```

1. See [:material-code-braces: ConfigParameterTypeDef](./type_defs.md#configparametertypedef) 
2. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
3. See [:material-code-brackets: WorkgroupStatusType](./literals.md#workgroupstatustype) 
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
    nextToken: str,
    workgroups: List[WorkgroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
