# Type definitions

> [Index](../README.md) > [S3Tables](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [S3Tables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables.html#s3tables)
    type annotations stubs module [types-aiobotocore-s3tables](https://pypi.org/project/types-aiobotocore-s3tables/).



## CreateNamespaceRequestTypeDef

```python
# CreateNamespaceRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import CreateNamespaceRequestTypeDef


def get_value() -> CreateNamespaceRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# CreateNamespaceRequestTypeDef definition

class CreateNamespaceRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: Sequence[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import ResponseMetadataTypeDef


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

## CreateTableBucketRequestTypeDef

```python
# CreateTableBucketRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import CreateTableBucketRequestTypeDef


def get_value() -> CreateTableBucketRequestTypeDef:
    return {
        "name": ...,
    }


# CreateTableBucketRequestTypeDef definition

class CreateTableBucketRequestTypeDef(TypedDict):
    name: str,
```

## DeleteNamespaceRequestTypeDef

```python
# DeleteNamespaceRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import DeleteNamespaceRequestTypeDef


def get_value() -> DeleteNamespaceRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# DeleteNamespaceRequestTypeDef definition

class DeleteNamespaceRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
```

## DeleteTableBucketPolicyRequestTypeDef

```python
# DeleteTableBucketPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import DeleteTableBucketPolicyRequestTypeDef


def get_value() -> DeleteTableBucketPolicyRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# DeleteTableBucketPolicyRequestTypeDef definition

class DeleteTableBucketPolicyRequestTypeDef(TypedDict):
    tableBucketARN: str,
```

## DeleteTableBucketRequestTypeDef

```python
# DeleteTableBucketRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import DeleteTableBucketRequestTypeDef


def get_value() -> DeleteTableBucketRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# DeleteTableBucketRequestTypeDef definition

class DeleteTableBucketRequestTypeDef(TypedDict):
    tableBucketARN: str,
```

## DeleteTablePolicyRequestTypeDef

```python
# DeleteTablePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import DeleteTablePolicyRequestTypeDef


def get_value() -> DeleteTablePolicyRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# DeleteTablePolicyRequestTypeDef definition

class DeleteTablePolicyRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## DeleteTableRequestTypeDef

```python
# DeleteTableRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import DeleteTableRequestTypeDef


def get_value() -> DeleteTableRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# DeleteTableRequestTypeDef definition

class DeleteTableRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
    versionToken: NotRequired[str],
```

## GetNamespaceRequestTypeDef

```python
# GetNamespaceRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetNamespaceRequestTypeDef


def get_value() -> GetNamespaceRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# GetNamespaceRequestTypeDef definition

class GetNamespaceRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
```

## GetTableBucketMaintenanceConfigurationRequestTypeDef

```python
# GetTableBucketMaintenanceConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableBucketMaintenanceConfigurationRequestTypeDef


def get_value() -> GetTableBucketMaintenanceConfigurationRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# GetTableBucketMaintenanceConfigurationRequestTypeDef definition

class GetTableBucketMaintenanceConfigurationRequestTypeDef(TypedDict):
    tableBucketARN: str,
```

## GetTableBucketPolicyRequestTypeDef

```python
# GetTableBucketPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableBucketPolicyRequestTypeDef


def get_value() -> GetTableBucketPolicyRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# GetTableBucketPolicyRequestTypeDef definition

class GetTableBucketPolicyRequestTypeDef(TypedDict):
    tableBucketARN: str,
```

## GetTableBucketRequestTypeDef

```python
# GetTableBucketRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableBucketRequestTypeDef


def get_value() -> GetTableBucketRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# GetTableBucketRequestTypeDef definition

class GetTableBucketRequestTypeDef(TypedDict):
    tableBucketARN: str,
```

## GetTableMaintenanceConfigurationRequestTypeDef

```python
# GetTableMaintenanceConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableMaintenanceConfigurationRequestTypeDef


def get_value() -> GetTableMaintenanceConfigurationRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# GetTableMaintenanceConfigurationRequestTypeDef definition

class GetTableMaintenanceConfigurationRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## GetTableMaintenanceJobStatusRequestTypeDef

```python
# GetTableMaintenanceJobStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableMaintenanceJobStatusRequestTypeDef


def get_value() -> GetTableMaintenanceJobStatusRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# GetTableMaintenanceJobStatusRequestTypeDef definition

class GetTableMaintenanceJobStatusRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## TableMaintenanceJobStatusValueTypeDef

```python
# TableMaintenanceJobStatusValueTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import TableMaintenanceJobStatusValueTypeDef


def get_value() -> TableMaintenanceJobStatusValueTypeDef:
    return {
        "status": ...,
    }


# TableMaintenanceJobStatusValueTypeDef definition

class TableMaintenanceJobStatusValueTypeDef(TypedDict):
    status: JobStatusType,  # (1)
    lastRunTimestamp: NotRequired[datetime],
    failureMessage: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## GetTableMetadataLocationRequestTypeDef

```python
# GetTableMetadataLocationRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableMetadataLocationRequestTypeDef


def get_value() -> GetTableMetadataLocationRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# GetTableMetadataLocationRequestTypeDef definition

class GetTableMetadataLocationRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## GetTablePolicyRequestTypeDef

```python
# GetTablePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTablePolicyRequestTypeDef


def get_value() -> GetTablePolicyRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# GetTablePolicyRequestTypeDef definition

class GetTablePolicyRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## GetTableRequestTypeDef

```python
# GetTableRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableRequestTypeDef


def get_value() -> GetTableRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# GetTableRequestTypeDef definition

class GetTableRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## IcebergCompactionSettingsTypeDef

```python
# IcebergCompactionSettingsTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import IcebergCompactionSettingsTypeDef


def get_value() -> IcebergCompactionSettingsTypeDef:
    return {
        "targetFileSizeMB": ...,
    }


# IcebergCompactionSettingsTypeDef definition

class IcebergCompactionSettingsTypeDef(TypedDict):
    targetFileSizeMB: NotRequired[int],
```

## SchemaFieldTypeDef

```python
# SchemaFieldTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import SchemaFieldTypeDef


def get_value() -> SchemaFieldTypeDef:
    return {
        "name": ...,
    }


# SchemaFieldTypeDef definition

class SchemaFieldTypeDef(TypedDict):
    name: str,
    type: str,
    required: NotRequired[bool],
```

## IcebergSnapshotManagementSettingsTypeDef

```python
# IcebergSnapshotManagementSettingsTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import IcebergSnapshotManagementSettingsTypeDef


def get_value() -> IcebergSnapshotManagementSettingsTypeDef:
    return {
        "minSnapshotsToKeep": ...,
    }


# IcebergSnapshotManagementSettingsTypeDef definition

class IcebergSnapshotManagementSettingsTypeDef(TypedDict):
    minSnapshotsToKeep: NotRequired[int],
    maxSnapshotAgeHours: NotRequired[int],
```

## IcebergUnreferencedFileRemovalSettingsTypeDef

```python
# IcebergUnreferencedFileRemovalSettingsTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import IcebergUnreferencedFileRemovalSettingsTypeDef


def get_value() -> IcebergUnreferencedFileRemovalSettingsTypeDef:
    return {
        "unreferencedDays": ...,
    }


# IcebergUnreferencedFileRemovalSettingsTypeDef definition

class IcebergUnreferencedFileRemovalSettingsTypeDef(TypedDict):
    unreferencedDays: NotRequired[int],
    nonCurrentDays: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import PaginatorConfigTypeDef


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

## ListNamespacesRequestTypeDef

```python
# ListNamespacesRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import ListNamespacesRequestTypeDef


def get_value() -> ListNamespacesRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# ListNamespacesRequestTypeDef definition

class ListNamespacesRequestTypeDef(TypedDict):
    tableBucketARN: str,
    prefix: NotRequired[str],
    continuationToken: NotRequired[str],
    maxNamespaces: NotRequired[int],
```

## NamespaceSummaryTypeDef

```python
# NamespaceSummaryTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import NamespaceSummaryTypeDef


def get_value() -> NamespaceSummaryTypeDef:
    return {
        "namespace": ...,
    }


# NamespaceSummaryTypeDef definition

class NamespaceSummaryTypeDef(TypedDict):
    namespace: List[str],
    createdAt: datetime,
    createdBy: str,
    ownerAccountId: str,
```

## ListTableBucketsRequestTypeDef

```python
# ListTableBucketsRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import ListTableBucketsRequestTypeDef


def get_value() -> ListTableBucketsRequestTypeDef:
    return {
        "prefix": ...,
    }


# ListTableBucketsRequestTypeDef definition

class ListTableBucketsRequestTypeDef(TypedDict):
    prefix: NotRequired[str],
    continuationToken: NotRequired[str],
    maxBuckets: NotRequired[int],
```

## TableBucketSummaryTypeDef

```python
# TableBucketSummaryTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import TableBucketSummaryTypeDef


def get_value() -> TableBucketSummaryTypeDef:
    return {
        "arn": ...,
    }


# TableBucketSummaryTypeDef definition

class TableBucketSummaryTypeDef(TypedDict):
    arn: str,
    name: str,
    ownerAccountId: str,
    createdAt: datetime,
```

## ListTablesRequestTypeDef

```python
# ListTablesRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import ListTablesRequestTypeDef


def get_value() -> ListTablesRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# ListTablesRequestTypeDef definition

class ListTablesRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: NotRequired[str],
    prefix: NotRequired[str],
    continuationToken: NotRequired[str],
    maxTables: NotRequired[int],
```

## TableSummaryTypeDef

```python
# TableSummaryTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import TableSummaryTypeDef


def get_value() -> TableSummaryTypeDef:
    return {
        "namespace": ...,
    }


# TableSummaryTypeDef definition

class TableSummaryTypeDef(TypedDict):
    namespace: List[str],
    name: str,
    type: TableTypeType,  # (1)
    tableARN: str,
    createdAt: datetime,
    modifiedAt: datetime,
```

1. See [:material-code-brackets: TableTypeType](./literals.md#tabletypetype) 
## PutTableBucketPolicyRequestTypeDef

```python
# PutTableBucketPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import PutTableBucketPolicyRequestTypeDef


def get_value() -> PutTableBucketPolicyRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# PutTableBucketPolicyRequestTypeDef definition

class PutTableBucketPolicyRequestTypeDef(TypedDict):
    tableBucketARN: str,
    resourcePolicy: str,
```

## PutTablePolicyRequestTypeDef

```python
# PutTablePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import PutTablePolicyRequestTypeDef


def get_value() -> PutTablePolicyRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# PutTablePolicyRequestTypeDef definition

class PutTablePolicyRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
    resourcePolicy: str,
```

## RenameTableRequestTypeDef

```python
# RenameTableRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import RenameTableRequestTypeDef


def get_value() -> RenameTableRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# RenameTableRequestTypeDef definition

class RenameTableRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
    newNamespaceName: NotRequired[str],
    newName: NotRequired[str],
    versionToken: NotRequired[str],
```

## UpdateTableMetadataLocationRequestTypeDef

```python
# UpdateTableMetadataLocationRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import UpdateTableMetadataLocationRequestTypeDef


def get_value() -> UpdateTableMetadataLocationRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# UpdateTableMetadataLocationRequestTypeDef definition

class UpdateTableMetadataLocationRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
    versionToken: str,
    metadataLocation: str,
```

## CreateNamespaceResponseTypeDef

```python
# CreateNamespaceResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import CreateNamespaceResponseTypeDef


def get_value() -> CreateNamespaceResponseTypeDef:
    return {
        "tableBucketARN": ...,
    }


# CreateNamespaceResponseTypeDef definition

class CreateNamespaceResponseTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTableBucketResponseTypeDef

```python
# CreateTableBucketResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import CreateTableBucketResponseTypeDef


def get_value() -> CreateTableBucketResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateTableBucketResponseTypeDef definition

class CreateTableBucketResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTableResponseTypeDef

```python
# CreateTableResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import CreateTableResponseTypeDef


def get_value() -> CreateTableResponseTypeDef:
    return {
        "tableARN": ...,
    }


# CreateTableResponseTypeDef definition

class CreateTableResponseTypeDef(TypedDict):
    tableARN: str,
    versionToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNamespaceResponseTypeDef

```python
# GetNamespaceResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetNamespaceResponseTypeDef


def get_value() -> GetNamespaceResponseTypeDef:
    return {
        "namespace": ...,
    }


# GetNamespaceResponseTypeDef definition

class GetNamespaceResponseTypeDef(TypedDict):
    namespace: List[str],
    createdAt: datetime,
    createdBy: str,
    ownerAccountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableBucketPolicyResponseTypeDef

```python
# GetTableBucketPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableBucketPolicyResponseTypeDef


def get_value() -> GetTableBucketPolicyResponseTypeDef:
    return {
        "resourcePolicy": ...,
    }


# GetTableBucketPolicyResponseTypeDef definition

class GetTableBucketPolicyResponseTypeDef(TypedDict):
    resourcePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableBucketResponseTypeDef

```python
# GetTableBucketResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableBucketResponseTypeDef


def get_value() -> GetTableBucketResponseTypeDef:
    return {
        "arn": ...,
    }


# GetTableBucketResponseTypeDef definition

class GetTableBucketResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    ownerAccountId: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableMetadataLocationResponseTypeDef

```python
# GetTableMetadataLocationResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableMetadataLocationResponseTypeDef


def get_value() -> GetTableMetadataLocationResponseTypeDef:
    return {
        "versionToken": ...,
    }


# GetTableMetadataLocationResponseTypeDef definition

class GetTableMetadataLocationResponseTypeDef(TypedDict):
    versionToken: str,
    metadataLocation: str,
    warehouseLocation: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTablePolicyResponseTypeDef

```python
# GetTablePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTablePolicyResponseTypeDef


def get_value() -> GetTablePolicyResponseTypeDef:
    return {
        "resourcePolicy": ...,
    }


# GetTablePolicyResponseTypeDef definition

class GetTablePolicyResponseTypeDef(TypedDict):
    resourcePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableResponseTypeDef

```python
# GetTableResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableResponseTypeDef


def get_value() -> GetTableResponseTypeDef:
    return {
        "name": ...,
    }


# GetTableResponseTypeDef definition

class GetTableResponseTypeDef(TypedDict):
    name: str,
    type: TableTypeType,  # (1)
    tableARN: str,
    namespace: List[str],
    versionToken: str,
    metadataLocation: str,
    warehouseLocation: str,
    createdAt: datetime,
    createdBy: str,
    managedByService: str,
    modifiedAt: datetime,
    modifiedBy: str,
    ownerAccountId: str,
    format: OpenTableFormatType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TableTypeType](./literals.md#tabletypetype) 
2. See [:material-code-brackets: OpenTableFormatType](./literals.md#opentableformattype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableMetadataLocationResponseTypeDef

```python
# UpdateTableMetadataLocationResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import UpdateTableMetadataLocationResponseTypeDef


def get_value() -> UpdateTableMetadataLocationResponseTypeDef:
    return {
        "name": ...,
    }


# UpdateTableMetadataLocationResponseTypeDef definition

class UpdateTableMetadataLocationResponseTypeDef(TypedDict):
    name: str,
    tableARN: str,
    namespace: List[str],
    versionToken: str,
    metadataLocation: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableMaintenanceJobStatusResponseTypeDef

```python
# GetTableMaintenanceJobStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableMaintenanceJobStatusResponseTypeDef


def get_value() -> GetTableMaintenanceJobStatusResponseTypeDef:
    return {
        "tableARN": ...,
    }


# GetTableMaintenanceJobStatusResponseTypeDef definition

class GetTableMaintenanceJobStatusResponseTypeDef(TypedDict):
    tableARN: str,
    status: Dict[TableMaintenanceJobTypeType, TableMaintenanceJobStatusValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TableMaintenanceJobTypeType](./literals.md#tablemaintenancejobtypetype) [:material-code-braces: TableMaintenanceJobStatusValueTypeDef](./type_defs.md#tablemaintenancejobstatusvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IcebergSchemaTypeDef

```python
# IcebergSchemaTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import IcebergSchemaTypeDef


def get_value() -> IcebergSchemaTypeDef:
    return {
        "fields": ...,
    }


# IcebergSchemaTypeDef definition

class IcebergSchemaTypeDef(TypedDict):
    fields: Sequence[SchemaFieldTypeDef],  # (1)
```

1. See [:material-code-braces: SchemaFieldTypeDef](./type_defs.md#schemafieldtypedef) 
## TableMaintenanceSettingsTypeDef

```python
# TableMaintenanceSettingsTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import TableMaintenanceSettingsTypeDef


def get_value() -> TableMaintenanceSettingsTypeDef:
    return {
        "icebergCompaction": ...,
    }


# TableMaintenanceSettingsTypeDef definition

class TableMaintenanceSettingsTypeDef(TypedDict):
    icebergCompaction: NotRequired[IcebergCompactionSettingsTypeDef],  # (1)
    icebergSnapshotManagement: NotRequired[IcebergSnapshotManagementSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: IcebergCompactionSettingsTypeDef](./type_defs.md#icebergcompactionsettingstypedef) 
2. See [:material-code-braces: IcebergSnapshotManagementSettingsTypeDef](./type_defs.md#icebergsnapshotmanagementsettingstypedef) 
## TableBucketMaintenanceSettingsTypeDef

```python
# TableBucketMaintenanceSettingsTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import TableBucketMaintenanceSettingsTypeDef


def get_value() -> TableBucketMaintenanceSettingsTypeDef:
    return {
        "icebergUnreferencedFileRemoval": ...,
    }


# TableBucketMaintenanceSettingsTypeDef definition

class TableBucketMaintenanceSettingsTypeDef(TypedDict):
    icebergUnreferencedFileRemoval: NotRequired[IcebergUnreferencedFileRemovalSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: IcebergUnreferencedFileRemovalSettingsTypeDef](./type_defs.md#icebergunreferencedfileremovalsettingstypedef) 
## ListNamespacesRequestPaginateTypeDef

```python
# ListNamespacesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import ListNamespacesRequestPaginateTypeDef


def get_value() -> ListNamespacesRequestPaginateTypeDef:
    return {
        "tableBucketARN": ...,
    }


# ListNamespacesRequestPaginateTypeDef definition

class ListNamespacesRequestPaginateTypeDef(TypedDict):
    tableBucketARN: str,
    prefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTableBucketsRequestPaginateTypeDef

```python
# ListTableBucketsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import ListTableBucketsRequestPaginateTypeDef


def get_value() -> ListTableBucketsRequestPaginateTypeDef:
    return {
        "prefix": ...,
    }


# ListTableBucketsRequestPaginateTypeDef definition

class ListTableBucketsRequestPaginateTypeDef(TypedDict):
    prefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesRequestPaginateTypeDef

```python
# ListTablesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import ListTablesRequestPaginateTypeDef


def get_value() -> ListTablesRequestPaginateTypeDef:
    return {
        "tableBucketARN": ...,
    }


# ListTablesRequestPaginateTypeDef definition

class ListTablesRequestPaginateTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: NotRequired[str],
    prefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNamespacesResponseTypeDef

```python
# ListNamespacesResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import ListNamespacesResponseTypeDef


def get_value() -> ListNamespacesResponseTypeDef:
    return {
        "namespaces": ...,
    }


# ListNamespacesResponseTypeDef definition

class ListNamespacesResponseTypeDef(TypedDict):
    namespaces: List[NamespaceSummaryTypeDef],  # (1)
    continuationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamespaceSummaryTypeDef](./type_defs.md#namespacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTableBucketsResponseTypeDef

```python
# ListTableBucketsResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import ListTableBucketsResponseTypeDef


def get_value() -> ListTableBucketsResponseTypeDef:
    return {
        "tableBuckets": ...,
    }


# ListTableBucketsResponseTypeDef definition

class ListTableBucketsResponseTypeDef(TypedDict):
    tableBuckets: List[TableBucketSummaryTypeDef],  # (1)
    continuationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableBucketSummaryTypeDef](./type_defs.md#tablebucketsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTablesResponseTypeDef

```python
# ListTablesResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import ListTablesResponseTypeDef


def get_value() -> ListTablesResponseTypeDef:
    return {
        "tables": ...,
    }


# ListTablesResponseTypeDef definition

class ListTablesResponseTypeDef(TypedDict):
    tables: List[TableSummaryTypeDef],  # (1)
    continuationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableSummaryTypeDef](./type_defs.md#tablesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IcebergMetadataTypeDef

```python
# IcebergMetadataTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import IcebergMetadataTypeDef


def get_value() -> IcebergMetadataTypeDef:
    return {
        "schema": ...,
    }


# IcebergMetadataTypeDef definition

class IcebergMetadataTypeDef(TypedDict):
    schema: IcebergSchemaTypeDef,  # (1)
```

1. See [:material-code-braces: IcebergSchemaTypeDef](./type_defs.md#icebergschematypedef) 
## TableMaintenanceConfigurationValueTypeDef

```python
# TableMaintenanceConfigurationValueTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import TableMaintenanceConfigurationValueTypeDef


def get_value() -> TableMaintenanceConfigurationValueTypeDef:
    return {
        "status": ...,
    }


# TableMaintenanceConfigurationValueTypeDef definition

class TableMaintenanceConfigurationValueTypeDef(TypedDict):
    status: NotRequired[MaintenanceStatusType],  # (1)
    settings: NotRequired[TableMaintenanceSettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: MaintenanceStatusType](./literals.md#maintenancestatustype) 
2. See [:material-code-braces: TableMaintenanceSettingsTypeDef](./type_defs.md#tablemaintenancesettingstypedef) 
## TableBucketMaintenanceConfigurationValueTypeDef

```python
# TableBucketMaintenanceConfigurationValueTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import TableBucketMaintenanceConfigurationValueTypeDef


def get_value() -> TableBucketMaintenanceConfigurationValueTypeDef:
    return {
        "status": ...,
    }


# TableBucketMaintenanceConfigurationValueTypeDef definition

class TableBucketMaintenanceConfigurationValueTypeDef(TypedDict):
    status: NotRequired[MaintenanceStatusType],  # (1)
    settings: NotRequired[TableBucketMaintenanceSettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: MaintenanceStatusType](./literals.md#maintenancestatustype) 
2. See [:material-code-braces: TableBucketMaintenanceSettingsTypeDef](./type_defs.md#tablebucketmaintenancesettingstypedef) 
## TableMetadataTypeDef

```python
# TableMetadataTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import TableMetadataTypeDef


def get_value() -> TableMetadataTypeDef:
    return {
        "iceberg": ...,
    }


# TableMetadataTypeDef definition

class TableMetadataTypeDef(TypedDict):
    iceberg: NotRequired[IcebergMetadataTypeDef],  # (1)
```

1. See [:material-code-braces: IcebergMetadataTypeDef](./type_defs.md#icebergmetadatatypedef) 
## GetTableMaintenanceConfigurationResponseTypeDef

```python
# GetTableMaintenanceConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableMaintenanceConfigurationResponseTypeDef


def get_value() -> GetTableMaintenanceConfigurationResponseTypeDef:
    return {
        "tableARN": ...,
    }


# GetTableMaintenanceConfigurationResponseTypeDef definition

class GetTableMaintenanceConfigurationResponseTypeDef(TypedDict):
    tableARN: str,
    configuration: Dict[TableMaintenanceTypeType, TableMaintenanceConfigurationValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TableMaintenanceTypeType](./literals.md#tablemaintenancetypetype) [:material-code-braces: TableMaintenanceConfigurationValueTypeDef](./type_defs.md#tablemaintenanceconfigurationvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutTableMaintenanceConfigurationRequestTypeDef

```python
# PutTableMaintenanceConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import PutTableMaintenanceConfigurationRequestTypeDef


def get_value() -> PutTableMaintenanceConfigurationRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# PutTableMaintenanceConfigurationRequestTypeDef definition

class PutTableMaintenanceConfigurationRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
    type: TableMaintenanceTypeType,  # (1)
    value: TableMaintenanceConfigurationValueTypeDef,  # (2)
```

1. See [:material-code-brackets: TableMaintenanceTypeType](./literals.md#tablemaintenancetypetype) 
2. See [:material-code-braces: TableMaintenanceConfigurationValueTypeDef](./type_defs.md#tablemaintenanceconfigurationvaluetypedef) 
## GetTableBucketMaintenanceConfigurationResponseTypeDef

```python
# GetTableBucketMaintenanceConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import GetTableBucketMaintenanceConfigurationResponseTypeDef


def get_value() -> GetTableBucketMaintenanceConfigurationResponseTypeDef:
    return {
        "tableBucketARN": ...,
    }


# GetTableBucketMaintenanceConfigurationResponseTypeDef definition

class GetTableBucketMaintenanceConfigurationResponseTypeDef(TypedDict):
    tableBucketARN: str,
    configuration: Dict[TableBucketMaintenanceTypeType, TableBucketMaintenanceConfigurationValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TableBucketMaintenanceTypeType](./literals.md#tablebucketmaintenancetypetype) [:material-code-braces: TableBucketMaintenanceConfigurationValueTypeDef](./type_defs.md#tablebucketmaintenanceconfigurationvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutTableBucketMaintenanceConfigurationRequestTypeDef

```python
# PutTableBucketMaintenanceConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import PutTableBucketMaintenanceConfigurationRequestTypeDef


def get_value() -> PutTableBucketMaintenanceConfigurationRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# PutTableBucketMaintenanceConfigurationRequestTypeDef definition

class PutTableBucketMaintenanceConfigurationRequestTypeDef(TypedDict):
    tableBucketARN: str,
    type: TableBucketMaintenanceTypeType,  # (1)
    value: TableBucketMaintenanceConfigurationValueTypeDef,  # (2)
```

1. See [:material-code-brackets: TableBucketMaintenanceTypeType](./literals.md#tablebucketmaintenancetypetype) 
2. See [:material-code-braces: TableBucketMaintenanceConfigurationValueTypeDef](./type_defs.md#tablebucketmaintenanceconfigurationvaluetypedef) 
## CreateTableRequestTypeDef

```python
# CreateTableRequestTypeDef TypedDict usage example

from types_aiobotocore_s3tables.type_defs import CreateTableRequestTypeDef


def get_value() -> CreateTableRequestTypeDef:
    return {
        "tableBucketARN": ...,
    }


# CreateTableRequestTypeDef definition

class CreateTableRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
    format: OpenTableFormatType,  # (1)
    metadata: NotRequired[TableMetadataTypeDef],  # (2)
```

1. See [:material-code-brackets: OpenTableFormatType](./literals.md#opentableformattype) 
2. See [:material-code-braces: TableMetadataTypeDef](./type_defs.md#tablemetadatatypedef) 
