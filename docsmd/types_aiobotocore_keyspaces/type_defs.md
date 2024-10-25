# Type definitions

> [Index](../README.md) > [Keyspaces](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Keyspaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
    type annotations stubs module [types-aiobotocore-keyspaces](https://pypi.org/project/types-aiobotocore-keyspaces/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## TargetTrackingScalingPolicyConfigurationTypeDef

```python
# TargetTrackingScalingPolicyConfigurationTypeDef definition

class TargetTrackingScalingPolicyConfigurationTypeDef(TypedDict):
    targetValue: float,
    disableScaleIn: NotRequired[bool],
    scaleInCooldown: NotRequired[int],
    scaleOutCooldown: NotRequired[int],
```

## CapacitySpecificationSummaryTypeDef

```python
# CapacitySpecificationSummaryTypeDef definition

class CapacitySpecificationSummaryTypeDef(TypedDict):
    throughputMode: ThroughputModeType,  # (1)
    readCapacityUnits: NotRequired[int],
    writeCapacityUnits: NotRequired[int],
    lastUpdateToPayPerRequestTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ThroughputModeType](./literals.md#throughputmodetype) 
## CapacitySpecificationTypeDef

```python
# CapacitySpecificationTypeDef definition

class CapacitySpecificationTypeDef(TypedDict):
    throughputMode: ThroughputModeType,  # (1)
    readCapacityUnits: NotRequired[int],
    writeCapacityUnits: NotRequired[int],
```

1. See [:material-code-brackets: ThroughputModeType](./literals.md#throughputmodetype) 
## ClientSideTimestampsTypeDef

```python
# ClientSideTimestampsTypeDef definition

class ClientSideTimestampsTypeDef(TypedDict):
    status: ClientSideTimestampsStatusType,  # (1)
```

1. See [:material-code-brackets: ClientSideTimestampsStatusType](./literals.md#clientsidetimestampsstatustype) 
## ClusteringKeyTypeDef

```python
# ClusteringKeyTypeDef definition

class ClusteringKeyTypeDef(TypedDict):
    name: str,
    orderBy: SortOrderType,  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ColumnDefinitionTypeDef

```python
# ColumnDefinitionTypeDef definition

class ColumnDefinitionTypeDef(TypedDict):
    name: str,
    type: str,
```

## CommentTypeDef

```python
# CommentTypeDef definition

class CommentTypeDef(TypedDict):
    message: str,
```

## ReplicationSpecificationTypeDef

```python
# ReplicationSpecificationTypeDef definition

class ReplicationSpecificationTypeDef(TypedDict):
    replicationStrategy: RsType,  # (1)
    regionList: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: RsType](./literals.md#rstype) 
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

## EncryptionSpecificationTypeDef

```python
# EncryptionSpecificationTypeDef definition

class EncryptionSpecificationTypeDef(TypedDict):
    type: EncryptionTypeType,  # (1)
    kmsKeyIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## PointInTimeRecoveryTypeDef

```python
# PointInTimeRecoveryTypeDef definition

class PointInTimeRecoveryTypeDef(TypedDict):
    status: PointInTimeRecoveryStatusType,  # (1)
```

1. See [:material-code-brackets: PointInTimeRecoveryStatusType](./literals.md#pointintimerecoverystatustype) 
## TimeToLiveTypeDef

```python
# TimeToLiveTypeDef definition

class TimeToLiveTypeDef(TypedDict):
    status: TimeToLiveStatusType,  # (1)
```

1. See [:material-code-brackets: TimeToLiveStatusType](./literals.md#timetolivestatustype) 
## DeleteKeyspaceRequestRequestTypeDef

```python
# DeleteKeyspaceRequestRequestTypeDef definition

class DeleteKeyspaceRequestRequestTypeDef(TypedDict):
    keyspaceName: str,
```

## DeleteTableRequestRequestTypeDef

```python
# DeleteTableRequestRequestTypeDef definition

class DeleteTableRequestRequestTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
```

## GetKeyspaceRequestRequestTypeDef

```python
# GetKeyspaceRequestRequestTypeDef definition

class GetKeyspaceRequestRequestTypeDef(TypedDict):
    keyspaceName: str,
```

## GetTableAutoScalingSettingsRequestRequestTypeDef

```python
# GetTableAutoScalingSettingsRequestRequestTypeDef definition

class GetTableAutoScalingSettingsRequestRequestTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
```

## GetTableRequestRequestTypeDef

```python
# GetTableRequestRequestTypeDef definition

class GetTableRequestRequestTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
```

## PointInTimeRecoverySummaryTypeDef

```python
# PointInTimeRecoverySummaryTypeDef definition

class PointInTimeRecoverySummaryTypeDef(TypedDict):
    status: PointInTimeRecoveryStatusType,  # (1)
    earliestRestorableTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: PointInTimeRecoveryStatusType](./literals.md#pointintimerecoverystatustype) 
## KeyspaceSummaryTypeDef

```python
# KeyspaceSummaryTypeDef definition

class KeyspaceSummaryTypeDef(TypedDict):
    keyspaceName: str,
    resourceArn: str,
    replicationStrategy: RsType,  # (1)
    replicationRegions: NotRequired[List[str]],
```

1. See [:material-code-brackets: RsType](./literals.md#rstype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListKeyspacesRequestRequestTypeDef

```python
# ListKeyspacesRequestRequestTypeDef definition

class ListKeyspacesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTablesRequestRequestTypeDef

```python
# ListTablesRequestRequestTypeDef definition

class ListTablesRequestRequestTypeDef(TypedDict):
    keyspaceName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TableSummaryTypeDef

```python
# TableSummaryTypeDef definition

class TableSummaryTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
    resourceArn: str,
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PartitionKeyTypeDef

```python
# PartitionKeyTypeDef definition

class PartitionKeyTypeDef(TypedDict):
    name: str,
```

## StaticColumnTypeDef

```python
# StaticColumnTypeDef definition

class StaticColumnTypeDef(TypedDict):
    name: str,
```

## AutoScalingPolicyTypeDef

```python
# AutoScalingPolicyTypeDef definition

class AutoScalingPolicyTypeDef(TypedDict):
    targetTrackingScalingPolicyConfiguration: NotRequired[TargetTrackingScalingPolicyConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: TargetTrackingScalingPolicyConfigurationTypeDef](./type_defs.md#targettrackingscalingpolicyconfigurationtypedef) 
## ReplicaSpecificationSummaryTypeDef

```python
# ReplicaSpecificationSummaryTypeDef definition

class ReplicaSpecificationSummaryTypeDef(TypedDict):
    region: NotRequired[str],
    status: NotRequired[TableStatusType],  # (1)
    capacitySpecification: NotRequired[CapacitySpecificationSummaryTypeDef],  # (2)
```

1. See [:material-code-brackets: TableStatusType](./literals.md#tablestatustype) 
2. See [:material-code-braces: CapacitySpecificationSummaryTypeDef](./type_defs.md#capacityspecificationsummarytypedef) 
## CreateKeyspaceRequestRequestTypeDef

```python
# CreateKeyspaceRequestRequestTypeDef definition

class CreateKeyspaceRequestRequestTypeDef(TypedDict):
    keyspaceName: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    replicationSpecification: NotRequired[ReplicationSpecificationTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ReplicationSpecificationTypeDef](./type_defs.md#replicationspecificationtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateKeyspaceResponseTypeDef

```python
# CreateKeyspaceResponseTypeDef definition

class CreateKeyspaceResponseTypeDef(TypedDict):
    resourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTableResponseTypeDef

```python
# CreateTableResponseTypeDef definition

class CreateTableResponseTypeDef(TypedDict):
    resourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKeyspaceResponseTypeDef

```python
# GetKeyspaceResponseTypeDef definition

class GetKeyspaceResponseTypeDef(TypedDict):
    keyspaceName: str,
    resourceArn: str,
    replicationStrategy: RsType,  # (1)
    replicationRegions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RsType](./literals.md#rstype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreTableResponseTypeDef

```python
# RestoreTableResponseTypeDef definition

class RestoreTableResponseTypeDef(TypedDict):
    restoredTableARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableResponseTypeDef

```python
# UpdateTableResponseTypeDef definition

class UpdateTableResponseTypeDef(TypedDict):
    resourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKeyspacesResponseTypeDef

```python
# ListKeyspacesResponseTypeDef definition

class ListKeyspacesResponseTypeDef(TypedDict):
    keyspaces: List[KeyspaceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KeyspaceSummaryTypeDef](./type_defs.md#keyspacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKeyspacesRequestListKeyspacesPaginateTypeDef

```python
# ListKeyspacesRequestListKeyspacesPaginateTypeDef definition

class ListKeyspacesRequestListKeyspacesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesRequestListTablesPaginateTypeDef

```python
# ListTablesRequestListTablesPaginateTypeDef definition

class ListTablesRequestListTablesPaginateTypeDef(TypedDict):
    keyspaceName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestListTagsForResourcePaginateTypeDef

```python
# ListTagsForResourceRequestListTagsForResourcePaginateTypeDef definition

class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(TypedDict):
    resourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesResponseTypeDef

```python
# ListTablesResponseTypeDef definition

class ListTablesResponseTypeDef(TypedDict):
    tables: List[TableSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TableSummaryTypeDef](./type_defs.md#tablesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SchemaDefinitionOutputTypeDef

```python
# SchemaDefinitionOutputTypeDef definition

class SchemaDefinitionOutputTypeDef(TypedDict):
    allColumns: List[ColumnDefinitionTypeDef],  # (1)
    partitionKeys: List[PartitionKeyTypeDef],  # (2)
    clusteringKeys: NotRequired[List[ClusteringKeyTypeDef]],  # (3)
    staticColumns: NotRequired[List[StaticColumnTypeDef]],  # (4)
```

1. See [:material-code-braces: ColumnDefinitionTypeDef](./type_defs.md#columndefinitiontypedef) 
2. See [:material-code-braces: PartitionKeyTypeDef](./type_defs.md#partitionkeytypedef) 
3. See [:material-code-braces: ClusteringKeyTypeDef](./type_defs.md#clusteringkeytypedef) 
4. See [:material-code-braces: StaticColumnTypeDef](./type_defs.md#staticcolumntypedef) 
## SchemaDefinitionTypeDef

```python
# SchemaDefinitionTypeDef definition

class SchemaDefinitionTypeDef(TypedDict):
    allColumns: Sequence[ColumnDefinitionTypeDef],  # (1)
    partitionKeys: Sequence[PartitionKeyTypeDef],  # (2)
    clusteringKeys: NotRequired[Sequence[ClusteringKeyTypeDef]],  # (3)
    staticColumns: NotRequired[Sequence[StaticColumnTypeDef]],  # (4)
```

1. See [:material-code-braces: ColumnDefinitionTypeDef](./type_defs.md#columndefinitiontypedef) 
2. See [:material-code-braces: PartitionKeyTypeDef](./type_defs.md#partitionkeytypedef) 
3. See [:material-code-braces: ClusteringKeyTypeDef](./type_defs.md#clusteringkeytypedef) 
4. See [:material-code-braces: StaticColumnTypeDef](./type_defs.md#staticcolumntypedef) 
## AutoScalingSettingsTypeDef

```python
# AutoScalingSettingsTypeDef definition

class AutoScalingSettingsTypeDef(TypedDict):
    autoScalingDisabled: NotRequired[bool],
    minimumUnits: NotRequired[int],
    maximumUnits: NotRequired[int],
    scalingPolicy: NotRequired[AutoScalingPolicyTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingPolicyTypeDef](./type_defs.md#autoscalingpolicytypedef) 
## GetTableResponseTypeDef

```python
# GetTableResponseTypeDef definition

class GetTableResponseTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
    resourceArn: str,
    creationTimestamp: datetime,
    status: TableStatusType,  # (1)
    schemaDefinition: SchemaDefinitionOutputTypeDef,  # (2)
    capacitySpecification: CapacitySpecificationSummaryTypeDef,  # (3)
    encryptionSpecification: EncryptionSpecificationTypeDef,  # (4)
    pointInTimeRecovery: PointInTimeRecoverySummaryTypeDef,  # (5)
    ttl: TimeToLiveTypeDef,  # (6)
    defaultTimeToLive: int,
    comment: CommentTypeDef,  # (7)
    clientSideTimestamps: ClientSideTimestampsTypeDef,  # (8)
    replicaSpecifications: List[ReplicaSpecificationSummaryTypeDef],  # (9)
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-brackets: TableStatusType](./literals.md#tablestatustype) 
2. See [:material-code-braces: SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef) 
3. See [:material-code-braces: CapacitySpecificationSummaryTypeDef](./type_defs.md#capacityspecificationsummarytypedef) 
4. See [:material-code-braces: EncryptionSpecificationTypeDef](./type_defs.md#encryptionspecificationtypedef) 
5. See [:material-code-braces: PointInTimeRecoverySummaryTypeDef](./type_defs.md#pointintimerecoverysummarytypedef) 
6. See [:material-code-braces: TimeToLiveTypeDef](./type_defs.md#timetolivetypedef) 
7. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
8. See [:material-code-braces: ClientSideTimestampsTypeDef](./type_defs.md#clientsidetimestampstypedef) 
9. See [:material-code-braces: ReplicaSpecificationSummaryTypeDef](./type_defs.md#replicaspecificationsummarytypedef) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoScalingSpecificationTypeDef

```python
# AutoScalingSpecificationTypeDef definition

class AutoScalingSpecificationTypeDef(TypedDict):
    writeCapacityAutoScaling: NotRequired[AutoScalingSettingsTypeDef],  # (1)
    readCapacityAutoScaling: NotRequired[AutoScalingSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsTypeDef](./type_defs.md#autoscalingsettingstypedef) 
2. See [:material-code-braces: AutoScalingSettingsTypeDef](./type_defs.md#autoscalingsettingstypedef) 
## ReplicaSpecificationTypeDef

```python
# ReplicaSpecificationTypeDef definition

class ReplicaSpecificationTypeDef(TypedDict):
    region: str,
    readCapacityUnits: NotRequired[int],
    readCapacityAutoScaling: NotRequired[AutoScalingSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsTypeDef](./type_defs.md#autoscalingsettingstypedef) 
## ReplicaAutoScalingSpecificationTypeDef

```python
# ReplicaAutoScalingSpecificationTypeDef definition

class ReplicaAutoScalingSpecificationTypeDef(TypedDict):
    region: NotRequired[str],
    autoScalingSpecification: NotRequired[AutoScalingSpecificationTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSpecificationTypeDef](./type_defs.md#autoscalingspecificationtypedef) 
## CreateTableRequestRequestTypeDef

```python
# CreateTableRequestRequestTypeDef definition

class CreateTableRequestRequestTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
    schemaDefinition: SchemaDefinitionTypeDef,  # (1)
    comment: NotRequired[CommentTypeDef],  # (2)
    capacitySpecification: NotRequired[CapacitySpecificationTypeDef],  # (3)
    encryptionSpecification: NotRequired[EncryptionSpecificationTypeDef],  # (4)
    pointInTimeRecovery: NotRequired[PointInTimeRecoveryTypeDef],  # (5)
    ttl: NotRequired[TimeToLiveTypeDef],  # (6)
    defaultTimeToLive: NotRequired[int],
    tags: NotRequired[Sequence[TagTypeDef]],  # (7)
    clientSideTimestamps: NotRequired[ClientSideTimestampsTypeDef],  # (8)
    autoScalingSpecification: NotRequired[AutoScalingSpecificationTypeDef],  # (9)
    replicaSpecifications: NotRequired[Sequence[ReplicaSpecificationTypeDef]],  # (10)
```

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) 
2. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
3. See [:material-code-braces: CapacitySpecificationTypeDef](./type_defs.md#capacityspecificationtypedef) 
4. See [:material-code-braces: EncryptionSpecificationTypeDef](./type_defs.md#encryptionspecificationtypedef) 
5. See [:material-code-braces: PointInTimeRecoveryTypeDef](./type_defs.md#pointintimerecoverytypedef) 
6. See [:material-code-braces: TimeToLiveTypeDef](./type_defs.md#timetolivetypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: ClientSideTimestampsTypeDef](./type_defs.md#clientsidetimestampstypedef) 
9. See [:material-code-braces: AutoScalingSpecificationTypeDef](./type_defs.md#autoscalingspecificationtypedef) 
10. See [:material-code-braces: ReplicaSpecificationTypeDef](./type_defs.md#replicaspecificationtypedef) 
## RestoreTableRequestRequestTypeDef

```python
# RestoreTableRequestRequestTypeDef definition

class RestoreTableRequestRequestTypeDef(TypedDict):
    sourceKeyspaceName: str,
    sourceTableName: str,
    targetKeyspaceName: str,
    targetTableName: str,
    restoreTimestamp: NotRequired[TimestampTypeDef],
    capacitySpecificationOverride: NotRequired[CapacitySpecificationTypeDef],  # (1)
    encryptionSpecificationOverride: NotRequired[EncryptionSpecificationTypeDef],  # (2)
    pointInTimeRecoveryOverride: NotRequired[PointInTimeRecoveryTypeDef],  # (3)
    tagsOverride: NotRequired[Sequence[TagTypeDef]],  # (4)
    autoScalingSpecification: NotRequired[AutoScalingSpecificationTypeDef],  # (5)
    replicaSpecifications: NotRequired[Sequence[ReplicaSpecificationTypeDef]],  # (6)
```

1. See [:material-code-braces: CapacitySpecificationTypeDef](./type_defs.md#capacityspecificationtypedef) 
2. See [:material-code-braces: EncryptionSpecificationTypeDef](./type_defs.md#encryptionspecificationtypedef) 
3. See [:material-code-braces: PointInTimeRecoveryTypeDef](./type_defs.md#pointintimerecoverytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: AutoScalingSpecificationTypeDef](./type_defs.md#autoscalingspecificationtypedef) 
6. See [:material-code-braces: ReplicaSpecificationTypeDef](./type_defs.md#replicaspecificationtypedef) 
## UpdateTableRequestRequestTypeDef

```python
# UpdateTableRequestRequestTypeDef definition

class UpdateTableRequestRequestTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
    addColumns: NotRequired[Sequence[ColumnDefinitionTypeDef]],  # (1)
    capacitySpecification: NotRequired[CapacitySpecificationTypeDef],  # (2)
    encryptionSpecification: NotRequired[EncryptionSpecificationTypeDef],  # (3)
    pointInTimeRecovery: NotRequired[PointInTimeRecoveryTypeDef],  # (4)
    ttl: NotRequired[TimeToLiveTypeDef],  # (5)
    defaultTimeToLive: NotRequired[int],
    clientSideTimestamps: NotRequired[ClientSideTimestampsTypeDef],  # (6)
    autoScalingSpecification: NotRequired[AutoScalingSpecificationTypeDef],  # (7)
    replicaSpecifications: NotRequired[Sequence[ReplicaSpecificationTypeDef]],  # (8)
```

1. See [:material-code-braces: ColumnDefinitionTypeDef](./type_defs.md#columndefinitiontypedef) 
2. See [:material-code-braces: CapacitySpecificationTypeDef](./type_defs.md#capacityspecificationtypedef) 
3. See [:material-code-braces: EncryptionSpecificationTypeDef](./type_defs.md#encryptionspecificationtypedef) 
4. See [:material-code-braces: PointInTimeRecoveryTypeDef](./type_defs.md#pointintimerecoverytypedef) 
5. See [:material-code-braces: TimeToLiveTypeDef](./type_defs.md#timetolivetypedef) 
6. See [:material-code-braces: ClientSideTimestampsTypeDef](./type_defs.md#clientsidetimestampstypedef) 
7. See [:material-code-braces: AutoScalingSpecificationTypeDef](./type_defs.md#autoscalingspecificationtypedef) 
8. See [:material-code-braces: ReplicaSpecificationTypeDef](./type_defs.md#replicaspecificationtypedef) 
## GetTableAutoScalingSettingsResponseTypeDef

```python
# GetTableAutoScalingSettingsResponseTypeDef definition

class GetTableAutoScalingSettingsResponseTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
    resourceArn: str,
    autoScalingSpecification: AutoScalingSpecificationTypeDef,  # (1)
    replicaSpecifications: List[ReplicaAutoScalingSpecificationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AutoScalingSpecificationTypeDef](./type_defs.md#autoscalingspecificationtypedef) 
2. See [:material-code-braces: ReplicaAutoScalingSpecificationTypeDef](./type_defs.md#replicaautoscalingspecificationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
