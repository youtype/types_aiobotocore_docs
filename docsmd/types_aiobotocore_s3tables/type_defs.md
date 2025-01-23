# Type definitions

> [Index](../README.md) > [S3Tables](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [S3Tables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables.html#s3tables)
    type annotations stubs module [types-aiobotocore-s3tables](https://pypi.org/project/types-aiobotocore-s3tables/).



## CreateNamespaceRequestRequestTypeDef

```python
# CreateNamespaceRequestRequestTypeDef definition

class CreateNamespaceRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: Sequence[str],
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

## CreateTableBucketRequestRequestTypeDef

```python
# CreateTableBucketRequestRequestTypeDef definition

class CreateTableBucketRequestRequestTypeDef(TypedDict):
    name: str,
```

## CreateTableRequestRequestTypeDef

```python
# CreateTableRequestRequestTypeDef definition

class CreateTableRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
    format: OpenTableFormatType,  # (1)
```

1. See [:material-code-brackets: OpenTableFormatType](./literals.md#opentableformattype) 
## DeleteNamespaceRequestRequestTypeDef

```python
# DeleteNamespaceRequestRequestTypeDef definition

class DeleteNamespaceRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
```

## DeleteTableBucketPolicyRequestRequestTypeDef

```python
# DeleteTableBucketPolicyRequestRequestTypeDef definition

class DeleteTableBucketPolicyRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
```

## DeleteTableBucketRequestRequestTypeDef

```python
# DeleteTableBucketRequestRequestTypeDef definition

class DeleteTableBucketRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
```

## DeleteTablePolicyRequestRequestTypeDef

```python
# DeleteTablePolicyRequestRequestTypeDef definition

class DeleteTablePolicyRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## DeleteTableRequestRequestTypeDef

```python
# DeleteTableRequestRequestTypeDef definition

class DeleteTableRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
    versionToken: NotRequired[str],
```

## GetNamespaceRequestRequestTypeDef

```python
# GetNamespaceRequestRequestTypeDef definition

class GetNamespaceRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
```

## GetTableBucketMaintenanceConfigurationRequestRequestTypeDef

```python
# GetTableBucketMaintenanceConfigurationRequestRequestTypeDef definition

class GetTableBucketMaintenanceConfigurationRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
```

## GetTableBucketPolicyRequestRequestTypeDef

```python
# GetTableBucketPolicyRequestRequestTypeDef definition

class GetTableBucketPolicyRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
```

## GetTableBucketRequestRequestTypeDef

```python
# GetTableBucketRequestRequestTypeDef definition

class GetTableBucketRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
```

## GetTableMaintenanceConfigurationRequestRequestTypeDef

```python
# GetTableMaintenanceConfigurationRequestRequestTypeDef definition

class GetTableMaintenanceConfigurationRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## GetTableMaintenanceJobStatusRequestRequestTypeDef

```python
# GetTableMaintenanceJobStatusRequestRequestTypeDef definition

class GetTableMaintenanceJobStatusRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## TableMaintenanceJobStatusValueTypeDef

```python
# TableMaintenanceJobStatusValueTypeDef definition

class TableMaintenanceJobStatusValueTypeDef(TypedDict):
    status: JobStatusType,  # (1)
    lastRunTimestamp: NotRequired[datetime],
    failureMessage: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## GetTableMetadataLocationRequestRequestTypeDef

```python
# GetTableMetadataLocationRequestRequestTypeDef definition

class GetTableMetadataLocationRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## GetTablePolicyRequestRequestTypeDef

```python
# GetTablePolicyRequestRequestTypeDef definition

class GetTablePolicyRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## GetTableRequestRequestTypeDef

```python
# GetTableRequestRequestTypeDef definition

class GetTableRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
```

## IcebergCompactionSettingsTypeDef

```python
# IcebergCompactionSettingsTypeDef definition

class IcebergCompactionSettingsTypeDef(TypedDict):
    targetFileSizeMB: NotRequired[int],
```

## IcebergSnapshotManagementSettingsTypeDef

```python
# IcebergSnapshotManagementSettingsTypeDef definition

class IcebergSnapshotManagementSettingsTypeDef(TypedDict):
    minSnapshotsToKeep: NotRequired[int],
    maxSnapshotAgeHours: NotRequired[int],
```

## IcebergUnreferencedFileRemovalSettingsTypeDef

```python
# IcebergUnreferencedFileRemovalSettingsTypeDef definition

class IcebergUnreferencedFileRemovalSettingsTypeDef(TypedDict):
    unreferencedDays: NotRequired[int],
    nonCurrentDays: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListNamespacesRequestRequestTypeDef

```python
# ListNamespacesRequestRequestTypeDef definition

class ListNamespacesRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    prefix: NotRequired[str],
    continuationToken: NotRequired[str],
    maxNamespaces: NotRequired[int],
```

## NamespaceSummaryTypeDef

```python
# NamespaceSummaryTypeDef definition

class NamespaceSummaryTypeDef(TypedDict):
    namespace: List[str],
    createdAt: datetime,
    createdBy: str,
    ownerAccountId: str,
```

## ListTableBucketsRequestRequestTypeDef

```python
# ListTableBucketsRequestRequestTypeDef definition

class ListTableBucketsRequestRequestTypeDef(TypedDict):
    prefix: NotRequired[str],
    continuationToken: NotRequired[str],
    maxBuckets: NotRequired[int],
```

## TableBucketSummaryTypeDef

```python
# TableBucketSummaryTypeDef definition

class TableBucketSummaryTypeDef(TypedDict):
    arn: str,
    name: str,
    ownerAccountId: str,
    createdAt: datetime,
```

## ListTablesRequestRequestTypeDef

```python
# ListTablesRequestRequestTypeDef definition

class ListTablesRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: NotRequired[str],
    prefix: NotRequired[str],
    continuationToken: NotRequired[str],
    maxTables: NotRequired[int],
```

## TableSummaryTypeDef

```python
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
## PutTableBucketPolicyRequestRequestTypeDef

```python
# PutTableBucketPolicyRequestRequestTypeDef definition

class PutTableBucketPolicyRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    resourcePolicy: str,
```

## PutTablePolicyRequestRequestTypeDef

```python
# PutTablePolicyRequestRequestTypeDef definition

class PutTablePolicyRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
    resourcePolicy: str,
```

## RenameTableRequestRequestTypeDef

```python
# RenameTableRequestRequestTypeDef definition

class RenameTableRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
    newNamespaceName: NotRequired[str],
    newName: NotRequired[str],
    versionToken: NotRequired[str],
```

## UpdateTableMetadataLocationRequestRequestTypeDef

```python
# UpdateTableMetadataLocationRequestRequestTypeDef definition

class UpdateTableMetadataLocationRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: str,
    name: str,
    versionToken: str,
    metadataLocation: str,
```

## CreateNamespaceResponseTypeDef

```python
# CreateNamespaceResponseTypeDef definition

class CreateNamespaceResponseTypeDef(TypedDict):
    tableBucketARN: str,
    namespace: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTableBucketResponseTypeDef

```python
# CreateTableBucketResponseTypeDef definition

class CreateTableBucketResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTableResponseTypeDef

```python
# CreateTableResponseTypeDef definition

class CreateTableResponseTypeDef(TypedDict):
    tableARN: str,
    versionToken: str,
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
## GetNamespaceResponseTypeDef

```python
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
# GetTableBucketPolicyResponseTypeDef definition

class GetTableBucketPolicyResponseTypeDef(TypedDict):
    resourcePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableBucketResponseTypeDef

```python
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
# GetTablePolicyResponseTypeDef definition

class GetTablePolicyResponseTypeDef(TypedDict):
    resourcePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableResponseTypeDef

```python
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
# GetTableMaintenanceJobStatusResponseTypeDef definition

class GetTableMaintenanceJobStatusResponseTypeDef(TypedDict):
    tableARN: str,
    status: Dict[TableMaintenanceJobTypeType, TableMaintenanceJobStatusValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TableMaintenanceJobTypeType](./literals.md#tablemaintenancejobtypetype) [:material-code-braces: TableMaintenanceJobStatusValueTypeDef](./type_defs.md#tablemaintenancejobstatusvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableMaintenanceSettingsTypeDef

```python
# TableMaintenanceSettingsTypeDef definition

class TableMaintenanceSettingsTypeDef(TypedDict):
    icebergCompaction: NotRequired[IcebergCompactionSettingsTypeDef],  # (1)
    icebergSnapshotManagement: NotRequired[IcebergSnapshotManagementSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: IcebergCompactionSettingsTypeDef](./type_defs.md#icebergcompactionsettingstypedef) 
2. See [:material-code-braces: IcebergSnapshotManagementSettingsTypeDef](./type_defs.md#icebergsnapshotmanagementsettingstypedef) 
## TableBucketMaintenanceSettingsTypeDef

```python
# TableBucketMaintenanceSettingsTypeDef definition

class TableBucketMaintenanceSettingsTypeDef(TypedDict):
    icebergUnreferencedFileRemoval: NotRequired[IcebergUnreferencedFileRemovalSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: IcebergUnreferencedFileRemovalSettingsTypeDef](./type_defs.md#icebergunreferencedfileremovalsettingstypedef) 
## ListNamespacesRequestPaginateTypeDef

```python
# ListNamespacesRequestPaginateTypeDef definition

class ListNamespacesRequestPaginateTypeDef(TypedDict):
    tableBucketARN: str,
    prefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTableBucketsRequestPaginateTypeDef

```python
# ListTableBucketsRequestPaginateTypeDef definition

class ListTableBucketsRequestPaginateTypeDef(TypedDict):
    prefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesRequestPaginateTypeDef

```python
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
# ListTablesResponseTypeDef definition

class ListTablesResponseTypeDef(TypedDict):
    tables: List[TableSummaryTypeDef],  # (1)
    continuationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableSummaryTypeDef](./type_defs.md#tablesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableMaintenanceConfigurationValueTypeDef

```python
# TableMaintenanceConfigurationValueTypeDef definition

class TableMaintenanceConfigurationValueTypeDef(TypedDict):
    status: NotRequired[MaintenanceStatusType],  # (1)
    settings: NotRequired[TableMaintenanceSettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: MaintenanceStatusType](./literals.md#maintenancestatustype) 
2. See [:material-code-braces: TableMaintenanceSettingsTypeDef](./type_defs.md#tablemaintenancesettingstypedef) 
## TableBucketMaintenanceConfigurationValueTypeDef

```python
# TableBucketMaintenanceConfigurationValueTypeDef definition

class TableBucketMaintenanceConfigurationValueTypeDef(TypedDict):
    status: NotRequired[MaintenanceStatusType],  # (1)
    settings: NotRequired[TableBucketMaintenanceSettingsTypeDef],  # (2)
```

1. See [:material-code-brackets: MaintenanceStatusType](./literals.md#maintenancestatustype) 
2. See [:material-code-braces: TableBucketMaintenanceSettingsTypeDef](./type_defs.md#tablebucketmaintenancesettingstypedef) 
## GetTableMaintenanceConfigurationResponseTypeDef

```python
# GetTableMaintenanceConfigurationResponseTypeDef definition

class GetTableMaintenanceConfigurationResponseTypeDef(TypedDict):
    tableARN: str,
    configuration: Dict[TableMaintenanceTypeType, TableMaintenanceConfigurationValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TableMaintenanceTypeType](./literals.md#tablemaintenancetypetype) [:material-code-braces: TableMaintenanceConfigurationValueTypeDef](./type_defs.md#tablemaintenanceconfigurationvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutTableMaintenanceConfigurationRequestRequestTypeDef

```python
# PutTableMaintenanceConfigurationRequestRequestTypeDef definition

class PutTableMaintenanceConfigurationRequestRequestTypeDef(TypedDict):
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
# GetTableBucketMaintenanceConfigurationResponseTypeDef definition

class GetTableBucketMaintenanceConfigurationResponseTypeDef(TypedDict):
    tableBucketARN: str,
    configuration: Dict[TableBucketMaintenanceTypeType, TableBucketMaintenanceConfigurationValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TableBucketMaintenanceTypeType](./literals.md#tablebucketmaintenancetypetype) [:material-code-braces: TableBucketMaintenanceConfigurationValueTypeDef](./type_defs.md#tablebucketmaintenanceconfigurationvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutTableBucketMaintenanceConfigurationRequestRequestTypeDef

```python
# PutTableBucketMaintenanceConfigurationRequestRequestTypeDef definition

class PutTableBucketMaintenanceConfigurationRequestRequestTypeDef(TypedDict):
    tableBucketARN: str,
    type: TableBucketMaintenanceTypeType,  # (1)
    value: TableBucketMaintenanceConfigurationValueTypeDef,  # (2)
```

1. See [:material-code-brackets: TableBucketMaintenanceTypeType](./literals.md#tablebucketmaintenancetypetype) 
2. See [:material-code-braces: TableBucketMaintenanceConfigurationValueTypeDef](./type_defs.md#tablebucketmaintenanceconfigurationvaluetypedef) 
