# Type definitions

> [Index](../README.md) > [Keyspaces](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Keyspaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#keyspaces)
    type annotations stubs module [types-aiobotocore-keyspaces](https://pypi.org/project/types-aiobotocore-keyspaces/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_keyspaces.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## SchemaDefinitionUnionTypeDef

```python
# SchemaDefinitionUnionTypeDef Union usage example

from types_aiobotocore_keyspaces.type_defs import SchemaDefinitionUnionTypeDef


def get_value() -> SchemaDefinitionUnionTypeDef:
    return ...


# SchemaDefinitionUnionTypeDef definition

SchemaDefinitionUnionTypeDef = Union[
    SchemaDefinitionTypeDef,  # (1)
    SchemaDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) 
2. See [:material-code-braces: SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef) 



## TargetTrackingScalingPolicyConfigurationTypeDef

```python
# TargetTrackingScalingPolicyConfigurationTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import TargetTrackingScalingPolicyConfigurationTypeDef


def get_value() -> TargetTrackingScalingPolicyConfigurationTypeDef:
    return {
        "disableScaleIn": ...,
    }


# TargetTrackingScalingPolicyConfigurationTypeDef definition

class TargetTrackingScalingPolicyConfigurationTypeDef(TypedDict):
    targetValue: float,
    disableScaleIn: NotRequired[bool],
    scaleInCooldown: NotRequired[int],
    scaleOutCooldown: NotRequired[int],
```

## CapacitySpecificationSummaryTypeDef

```python
# CapacitySpecificationSummaryTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import CapacitySpecificationSummaryTypeDef


def get_value() -> CapacitySpecificationSummaryTypeDef:
    return {
        "throughputMode": ...,
    }


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
# CapacitySpecificationTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import CapacitySpecificationTypeDef


def get_value() -> CapacitySpecificationTypeDef:
    return {
        "throughputMode": ...,
    }


# CapacitySpecificationTypeDef definition

class CapacitySpecificationTypeDef(TypedDict):
    throughputMode: ThroughputModeType,  # (1)
    readCapacityUnits: NotRequired[int],
    writeCapacityUnits: NotRequired[int],
```

1. See [:material-code-brackets: ThroughputModeType](./literals.md#throughputmodetype) 
## ClientSideTimestampsTypeDef

```python
# ClientSideTimestampsTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ClientSideTimestampsTypeDef


def get_value() -> ClientSideTimestampsTypeDef:
    return {
        "status": ...,
    }


# ClientSideTimestampsTypeDef definition

class ClientSideTimestampsTypeDef(TypedDict):
    status: ClientSideTimestampsStatusType,  # (1)
```

1. See [:material-code-brackets: ClientSideTimestampsStatusType](./literals.md#clientsidetimestampsstatustype) 
## ClusteringKeyTypeDef

```python
# ClusteringKeyTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ClusteringKeyTypeDef


def get_value() -> ClusteringKeyTypeDef:
    return {
        "name": ...,
    }


# ClusteringKeyTypeDef definition

class ClusteringKeyTypeDef(TypedDict):
    name: str,
    orderBy: SortOrderType,  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ColumnDefinitionTypeDef

```python
# ColumnDefinitionTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ColumnDefinitionTypeDef


def get_value() -> ColumnDefinitionTypeDef:
    return {
        "name": ...,
    }


# ColumnDefinitionTypeDef definition

class ColumnDefinitionTypeDef(TypedDict):
    name: str,
    type: str,
```

## CommentTypeDef

```python
# CommentTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import CommentTypeDef


def get_value() -> CommentTypeDef:
    return {
        "message": ...,
    }


# CommentTypeDef definition

class CommentTypeDef(TypedDict):
    message: str,
```

## ReplicationSpecificationTypeDef

```python
# ReplicationSpecificationTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ReplicationSpecificationTypeDef


def get_value() -> ReplicationSpecificationTypeDef:
    return {
        "replicationStrategy": ...,
    }


# ReplicationSpecificationTypeDef definition

class ReplicationSpecificationTypeDef(TypedDict):
    replicationStrategy: RsType,  # (1)
    regionList: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: RsType](./literals.md#rstype) 
## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


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
# EncryptionSpecificationTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import EncryptionSpecificationTypeDef


def get_value() -> EncryptionSpecificationTypeDef:
    return {
        "type": ...,
    }


# EncryptionSpecificationTypeDef definition

class EncryptionSpecificationTypeDef(TypedDict):
    type: EncryptionTypeType,  # (1)
    kmsKeyIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## PointInTimeRecoveryTypeDef

```python
# PointInTimeRecoveryTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import PointInTimeRecoveryTypeDef


def get_value() -> PointInTimeRecoveryTypeDef:
    return {
        "status": ...,
    }


# PointInTimeRecoveryTypeDef definition

class PointInTimeRecoveryTypeDef(TypedDict):
    status: PointInTimeRecoveryStatusType,  # (1)
```

1. See [:material-code-brackets: PointInTimeRecoveryStatusType](./literals.md#pointintimerecoverystatustype) 
## TimeToLiveTypeDef

```python
# TimeToLiveTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import TimeToLiveTypeDef


def get_value() -> TimeToLiveTypeDef:
    return {
        "status": ...,
    }


# TimeToLiveTypeDef definition

class TimeToLiveTypeDef(TypedDict):
    status: TimeToLiveStatusType,  # (1)
```

1. See [:material-code-brackets: TimeToLiveStatusType](./literals.md#timetolivestatustype) 
## FieldDefinitionTypeDef

```python
# FieldDefinitionTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import FieldDefinitionTypeDef


def get_value() -> FieldDefinitionTypeDef:
    return {
        "name": ...,
    }


# FieldDefinitionTypeDef definition

class FieldDefinitionTypeDef(TypedDict):
    name: str,
    type: str,
```

## DeleteKeyspaceRequestTypeDef

```python
# DeleteKeyspaceRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import DeleteKeyspaceRequestTypeDef


def get_value() -> DeleteKeyspaceRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# DeleteKeyspaceRequestTypeDef definition

class DeleteKeyspaceRequestTypeDef(TypedDict):
    keyspaceName: str,
```

## DeleteTableRequestTypeDef

```python
# DeleteTableRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import DeleteTableRequestTypeDef


def get_value() -> DeleteTableRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# DeleteTableRequestTypeDef definition

class DeleteTableRequestTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
```

## DeleteTypeRequestTypeDef

```python
# DeleteTypeRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import DeleteTypeRequestTypeDef


def get_value() -> DeleteTypeRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# DeleteTypeRequestTypeDef definition

class DeleteTypeRequestTypeDef(TypedDict):
    keyspaceName: str,
    typeName: str,
```

## GetKeyspaceRequestTypeDef

```python
# GetKeyspaceRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import GetKeyspaceRequestTypeDef


def get_value() -> GetKeyspaceRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# GetKeyspaceRequestTypeDef definition

class GetKeyspaceRequestTypeDef(TypedDict):
    keyspaceName: str,
```

## ReplicationGroupStatusTypeDef

```python
# ReplicationGroupStatusTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ReplicationGroupStatusTypeDef


def get_value() -> ReplicationGroupStatusTypeDef:
    return {
        "region": ...,
    }


# ReplicationGroupStatusTypeDef definition

class ReplicationGroupStatusTypeDef(TypedDict):
    region: str,
    keyspaceStatus: KeyspaceStatusType,  # (1)
    tablesReplicationProgress: NotRequired[str],
```

1. See [:material-code-brackets: KeyspaceStatusType](./literals.md#keyspacestatustype) 
## GetTableAutoScalingSettingsRequestTypeDef

```python
# GetTableAutoScalingSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import GetTableAutoScalingSettingsRequestTypeDef


def get_value() -> GetTableAutoScalingSettingsRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# GetTableAutoScalingSettingsRequestTypeDef definition

class GetTableAutoScalingSettingsRequestTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
```

## GetTableRequestTypeDef

```python
# GetTableRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import GetTableRequestTypeDef


def get_value() -> GetTableRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# GetTableRequestTypeDef definition

class GetTableRequestTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
```

## PointInTimeRecoverySummaryTypeDef

```python
# PointInTimeRecoverySummaryTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import PointInTimeRecoverySummaryTypeDef


def get_value() -> PointInTimeRecoverySummaryTypeDef:
    return {
        "status": ...,
    }


# PointInTimeRecoverySummaryTypeDef definition

class PointInTimeRecoverySummaryTypeDef(TypedDict):
    status: PointInTimeRecoveryStatusType,  # (1)
    earliestRestorableTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: PointInTimeRecoveryStatusType](./literals.md#pointintimerecoverystatustype) 
## GetTypeRequestTypeDef

```python
# GetTypeRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import GetTypeRequestTypeDef


def get_value() -> GetTypeRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# GetTypeRequestTypeDef definition

class GetTypeRequestTypeDef(TypedDict):
    keyspaceName: str,
    typeName: str,
```

## KeyspaceSummaryTypeDef

```python
# KeyspaceSummaryTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import KeyspaceSummaryTypeDef


def get_value() -> KeyspaceSummaryTypeDef:
    return {
        "keyspaceName": ...,
    }


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
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListKeyspacesRequestTypeDef

```python
# ListKeyspacesRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListKeyspacesRequestTypeDef


def get_value() -> ListKeyspacesRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListKeyspacesRequestTypeDef definition

class ListKeyspacesRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTablesRequestTypeDef

```python
# ListTablesRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListTablesRequestTypeDef


def get_value() -> ListTablesRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# ListTablesRequestTypeDef definition

class ListTablesRequestTypeDef(TypedDict):
    keyspaceName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TableSummaryTypeDef

```python
# TableSummaryTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import TableSummaryTypeDef


def get_value() -> TableSummaryTypeDef:
    return {
        "keyspaceName": ...,
    }


# TableSummaryTypeDef definition

class TableSummaryTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
    resourceArn: str,
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTypesRequestTypeDef

```python
# ListTypesRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListTypesRequestTypeDef


def get_value() -> ListTypesRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# ListTypesRequestTypeDef definition

class ListTypesRequestTypeDef(TypedDict):
    keyspaceName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PartitionKeyTypeDef

```python
# PartitionKeyTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import PartitionKeyTypeDef


def get_value() -> PartitionKeyTypeDef:
    return {
        "name": ...,
    }


# PartitionKeyTypeDef definition

class PartitionKeyTypeDef(TypedDict):
    name: str,
```

## StaticColumnTypeDef

```python
# StaticColumnTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import StaticColumnTypeDef


def get_value() -> StaticColumnTypeDef:
    return {
        "name": ...,
    }


# StaticColumnTypeDef definition

class StaticColumnTypeDef(TypedDict):
    name: str,
```

## AutoScalingPolicyTypeDef

```python
# AutoScalingPolicyTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import AutoScalingPolicyTypeDef


def get_value() -> AutoScalingPolicyTypeDef:
    return {
        "targetTrackingScalingPolicyConfiguration": ...,
    }


# AutoScalingPolicyTypeDef definition

class AutoScalingPolicyTypeDef(TypedDict):
    targetTrackingScalingPolicyConfiguration: NotRequired[TargetTrackingScalingPolicyConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: TargetTrackingScalingPolicyConfigurationTypeDef](./type_defs.md#targettrackingscalingpolicyconfigurationtypedef) 
## ReplicaSpecificationSummaryTypeDef

```python
# ReplicaSpecificationSummaryTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ReplicaSpecificationSummaryTypeDef


def get_value() -> ReplicaSpecificationSummaryTypeDef:
    return {
        "region": ...,
    }


# ReplicaSpecificationSummaryTypeDef definition

class ReplicaSpecificationSummaryTypeDef(TypedDict):
    region: NotRequired[str],
    status: NotRequired[TableStatusType],  # (1)
    capacitySpecification: NotRequired[CapacitySpecificationSummaryTypeDef],  # (2)
```

1. See [:material-code-brackets: TableStatusType](./literals.md#tablestatustype) 
2. See [:material-code-braces: CapacitySpecificationSummaryTypeDef](./type_defs.md#capacityspecificationsummarytypedef) 
## UpdateKeyspaceRequestTypeDef

```python
# UpdateKeyspaceRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import UpdateKeyspaceRequestTypeDef


def get_value() -> UpdateKeyspaceRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# UpdateKeyspaceRequestTypeDef definition

class UpdateKeyspaceRequestTypeDef(TypedDict):
    keyspaceName: str,
    replicationSpecification: ReplicationSpecificationTypeDef,  # (1)
    clientSideTimestamps: NotRequired[ClientSideTimestampsTypeDef],  # (2)
```

1. See [:material-code-braces: ReplicationSpecificationTypeDef](./type_defs.md#replicationspecificationtypedef) 
2. See [:material-code-braces: ClientSideTimestampsTypeDef](./type_defs.md#clientsidetimestampstypedef) 
## CreateKeyspaceRequestTypeDef

```python
# CreateKeyspaceRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import CreateKeyspaceRequestTypeDef


def get_value() -> CreateKeyspaceRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# CreateKeyspaceRequestTypeDef definition

class CreateKeyspaceRequestTypeDef(TypedDict):
    keyspaceName: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    replicationSpecification: NotRequired[ReplicationSpecificationTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ReplicationSpecificationTypeDef](./type_defs.md#replicationspecificationtypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateKeyspaceResponseTypeDef

```python
# CreateKeyspaceResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import CreateKeyspaceResponseTypeDef


def get_value() -> CreateKeyspaceResponseTypeDef:
    return {
        "resourceArn": ...,
    }


# CreateKeyspaceResponseTypeDef definition

class CreateKeyspaceResponseTypeDef(TypedDict):
    resourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTableResponseTypeDef

```python
# CreateTableResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import CreateTableResponseTypeDef


def get_value() -> CreateTableResponseTypeDef:
    return {
        "resourceArn": ...,
    }


# CreateTableResponseTypeDef definition

class CreateTableResponseTypeDef(TypedDict):
    resourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTypeResponseTypeDef

```python
# CreateTypeResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import CreateTypeResponseTypeDef


def get_value() -> CreateTypeResponseTypeDef:
    return {
        "keyspaceArn": ...,
    }


# CreateTypeResponseTypeDef definition

class CreateTypeResponseTypeDef(TypedDict):
    keyspaceArn: str,
    typeName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTypeResponseTypeDef

```python
# DeleteTypeResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import DeleteTypeResponseTypeDef


def get_value() -> DeleteTypeResponseTypeDef:
    return {
        "keyspaceArn": ...,
    }


# DeleteTypeResponseTypeDef definition

class DeleteTypeResponseTypeDef(TypedDict):
    keyspaceArn: str,
    typeName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTypesResponseTypeDef

```python
# ListTypesResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListTypesResponseTypeDef


def get_value() -> ListTypesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListTypesResponseTypeDef definition

class ListTypesResponseTypeDef(TypedDict):
    types: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreTableResponseTypeDef

```python
# RestoreTableResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import RestoreTableResponseTypeDef


def get_value() -> RestoreTableResponseTypeDef:
    return {
        "restoredTableARN": ...,
    }


# RestoreTableResponseTypeDef definition

class RestoreTableResponseTypeDef(TypedDict):
    restoredTableARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKeyspaceResponseTypeDef

```python
# UpdateKeyspaceResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import UpdateKeyspaceResponseTypeDef


def get_value() -> UpdateKeyspaceResponseTypeDef:
    return {
        "resourceArn": ...,
    }


# UpdateKeyspaceResponseTypeDef definition

class UpdateKeyspaceResponseTypeDef(TypedDict):
    resourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableResponseTypeDef

```python
# UpdateTableResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import UpdateTableResponseTypeDef


def get_value() -> UpdateTableResponseTypeDef:
    return {
        "resourceArn": ...,
    }


# UpdateTableResponseTypeDef definition

class UpdateTableResponseTypeDef(TypedDict):
    resourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTypeRequestTypeDef

```python
# CreateTypeRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import CreateTypeRequestTypeDef


def get_value() -> CreateTypeRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# CreateTypeRequestTypeDef definition

class CreateTypeRequestTypeDef(TypedDict):
    keyspaceName: str,
    typeName: str,
    fieldDefinitions: Sequence[FieldDefinitionTypeDef],  # (1)
```

1. See [:material-code-braces: FieldDefinitionTypeDef](./type_defs.md#fielddefinitiontypedef) 
## GetTypeResponseTypeDef

```python
# GetTypeResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import GetTypeResponseTypeDef


def get_value() -> GetTypeResponseTypeDef:
    return {
        "keyspaceName": ...,
    }


# GetTypeResponseTypeDef definition

class GetTypeResponseTypeDef(TypedDict):
    keyspaceName: str,
    typeName: str,
    fieldDefinitions: List[FieldDefinitionTypeDef],  # (1)
    lastModifiedTimestamp: datetime,
    status: TypeStatusType,  # (2)
    directReferringTables: List[str],
    directParentTypes: List[str],
    maxNestingDepth: int,
    keyspaceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FieldDefinitionTypeDef](./type_defs.md#fielddefinitiontypedef) 
2. See [:material-code-brackets: TypeStatusType](./literals.md#typestatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKeyspaceResponseTypeDef

```python
# GetKeyspaceResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import GetKeyspaceResponseTypeDef


def get_value() -> GetKeyspaceResponseTypeDef:
    return {
        "keyspaceName": ...,
    }


# GetKeyspaceResponseTypeDef definition

class GetKeyspaceResponseTypeDef(TypedDict):
    keyspaceName: str,
    resourceArn: str,
    replicationStrategy: RsType,  # (1)
    replicationRegions: List[str],
    replicationGroupStatuses: List[ReplicationGroupStatusTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: RsType](./literals.md#rstype) 
2. See [:material-code-braces: ReplicationGroupStatusTypeDef](./type_defs.md#replicationgroupstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKeyspacesResponseTypeDef

```python
# ListKeyspacesResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListKeyspacesResponseTypeDef


def get_value() -> ListKeyspacesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListKeyspacesResponseTypeDef definition

class ListKeyspacesResponseTypeDef(TypedDict):
    keyspaces: List[KeyspaceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KeyspaceSummaryTypeDef](./type_defs.md#keyspacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKeyspacesRequestPaginateTypeDef

```python
# ListKeyspacesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListKeyspacesRequestPaginateTypeDef


def get_value() -> ListKeyspacesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListKeyspacesRequestPaginateTypeDef definition

class ListKeyspacesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesRequestPaginateTypeDef

```python
# ListTablesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListTablesRequestPaginateTypeDef


def get_value() -> ListTablesRequestPaginateTypeDef:
    return {
        "keyspaceName": ...,
    }


# ListTablesRequestPaginateTypeDef definition

class ListTablesRequestPaginateTypeDef(TypedDict):
    keyspaceName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestPaginateTypeDef

```python
# ListTagsForResourceRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListTagsForResourceRequestPaginateTypeDef


def get_value() -> ListTagsForResourceRequestPaginateTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestPaginateTypeDef definition

class ListTagsForResourceRequestPaginateTypeDef(TypedDict):
    resourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTypesRequestPaginateTypeDef

```python
# ListTypesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListTypesRequestPaginateTypeDef


def get_value() -> ListTypesRequestPaginateTypeDef:
    return {
        "keyspaceName": ...,
    }


# ListTypesRequestPaginateTypeDef definition

class ListTypesRequestPaginateTypeDef(TypedDict):
    keyspaceName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesResponseTypeDef

```python
# ListTablesResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ListTablesResponseTypeDef


def get_value() -> ListTablesResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# SchemaDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import SchemaDefinitionOutputTypeDef


def get_value() -> SchemaDefinitionOutputTypeDef:
    return {
        "allColumns": ...,
    }


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
# SchemaDefinitionTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import SchemaDefinitionTypeDef


def get_value() -> SchemaDefinitionTypeDef:
    return {
        "allColumns": ...,
    }


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
# AutoScalingSettingsTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import AutoScalingSettingsTypeDef


def get_value() -> AutoScalingSettingsTypeDef:
    return {
        "autoScalingDisabled": ...,
    }


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
# GetTableResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import GetTableResponseTypeDef


def get_value() -> GetTableResponseTypeDef:
    return {
        "keyspaceName": ...,
    }


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
# AutoScalingSpecificationTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import AutoScalingSpecificationTypeDef


def get_value() -> AutoScalingSpecificationTypeDef:
    return {
        "writeCapacityAutoScaling": ...,
    }


# AutoScalingSpecificationTypeDef definition

class AutoScalingSpecificationTypeDef(TypedDict):
    writeCapacityAutoScaling: NotRequired[AutoScalingSettingsTypeDef],  # (1)
    readCapacityAutoScaling: NotRequired[AutoScalingSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsTypeDef](./type_defs.md#autoscalingsettingstypedef) 
2. See [:material-code-braces: AutoScalingSettingsTypeDef](./type_defs.md#autoscalingsettingstypedef) 
## ReplicaSpecificationTypeDef

```python
# ReplicaSpecificationTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ReplicaSpecificationTypeDef


def get_value() -> ReplicaSpecificationTypeDef:
    return {
        "region": ...,
    }


# ReplicaSpecificationTypeDef definition

class ReplicaSpecificationTypeDef(TypedDict):
    region: str,
    readCapacityUnits: NotRequired[int],
    readCapacityAutoScaling: NotRequired[AutoScalingSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsTypeDef](./type_defs.md#autoscalingsettingstypedef) 
## ReplicaAutoScalingSpecificationTypeDef

```python
# ReplicaAutoScalingSpecificationTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import ReplicaAutoScalingSpecificationTypeDef


def get_value() -> ReplicaAutoScalingSpecificationTypeDef:
    return {
        "region": ...,
    }


# ReplicaAutoScalingSpecificationTypeDef definition

class ReplicaAutoScalingSpecificationTypeDef(TypedDict):
    region: NotRequired[str],
    autoScalingSpecification: NotRequired[AutoScalingSpecificationTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSpecificationTypeDef](./type_defs.md#autoscalingspecificationtypedef) 
## CreateTableRequestTypeDef

```python
# CreateTableRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import CreateTableRequestTypeDef


def get_value() -> CreateTableRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# CreateTableRequestTypeDef definition

class CreateTableRequestTypeDef(TypedDict):
    keyspaceName: str,
    tableName: str,
    schemaDefinition: SchemaDefinitionUnionTypeDef,  # (1)
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

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) [:material-code-braces: SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef) 
2. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
3. See [:material-code-braces: CapacitySpecificationTypeDef](./type_defs.md#capacityspecificationtypedef) 
4. See [:material-code-braces: EncryptionSpecificationTypeDef](./type_defs.md#encryptionspecificationtypedef) 
5. See [:material-code-braces: PointInTimeRecoveryTypeDef](./type_defs.md#pointintimerecoverytypedef) 
6. See [:material-code-braces: TimeToLiveTypeDef](./type_defs.md#timetolivetypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: ClientSideTimestampsTypeDef](./type_defs.md#clientsidetimestampstypedef) 
9. See [:material-code-braces: AutoScalingSpecificationTypeDef](./type_defs.md#autoscalingspecificationtypedef) 
10. See [:material-code-braces: ReplicaSpecificationTypeDef](./type_defs.md#replicaspecificationtypedef) 
## RestoreTableRequestTypeDef

```python
# RestoreTableRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import RestoreTableRequestTypeDef


def get_value() -> RestoreTableRequestTypeDef:
    return {
        "sourceKeyspaceName": ...,
    }


# RestoreTableRequestTypeDef definition

class RestoreTableRequestTypeDef(TypedDict):
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
## UpdateTableRequestTypeDef

```python
# UpdateTableRequestTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import UpdateTableRequestTypeDef


def get_value() -> UpdateTableRequestTypeDef:
    return {
        "keyspaceName": ...,
    }


# UpdateTableRequestTypeDef definition

class UpdateTableRequestTypeDef(TypedDict):
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
# GetTableAutoScalingSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_keyspaces.type_defs import GetTableAutoScalingSettingsResponseTypeDef


def get_value() -> GetTableAutoScalingSettingsResponseTypeDef:
    return {
        "keyspaceName": ...,
    }


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
