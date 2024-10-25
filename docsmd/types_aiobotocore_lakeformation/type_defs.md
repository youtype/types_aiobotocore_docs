# Type definitions

> [Index](../README.md) > [LakeFormation](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LakeFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
    type annotations stubs module [types-aiobotocore-lakeformation](https://pypi.org/project/types-aiobotocore-lakeformation/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ColumnWildcardUnionTypeDef

```python
# ColumnWildcardUnionTypeDef definition

ColumnWildcardUnionTypeDef = Union[
    ColumnWildcardTypeDef,  # (1)
    ColumnWildcardOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ColumnWildcardTypeDef](./type_defs.md#columnwildcardtypedef) 
2. See [:material-code-braces: ColumnWildcardOutputTypeDef](./type_defs.md#columnwildcardoutputtypedef) 

## LFTagKeyResourceUnionTypeDef

```python
# LFTagKeyResourceUnionTypeDef definition

LFTagKeyResourceUnionTypeDef = Union[
    LFTagKeyResourceTypeDef,  # (1)
    LFTagKeyResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LFTagKeyResourceTypeDef](./type_defs.md#lftagkeyresourcetypedef) 
2. See [:material-code-braces: LFTagKeyResourceOutputTypeDef](./type_defs.md#lftagkeyresourceoutputtypedef) 

## LFTagPairUnionTypeDef

```python
# LFTagPairUnionTypeDef definition

LFTagPairUnionTypeDef = Union[
    LFTagPairTypeDef,  # (1)
    LFTagPairOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LFTagPairTypeDef](./type_defs.md#lftagpairtypedef) 
2. See [:material-code-braces: LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef) 

## LFTagUnionTypeDef

```python
# LFTagUnionTypeDef definition

LFTagUnionTypeDef = Union[
    LFTagTypeDef,  # (1)
    LFTagOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
2. See [:material-code-braces: LFTagOutputTypeDef](./type_defs.md#lftagoutputtypedef) 

## TableResourceUnionTypeDef

```python
# TableResourceUnionTypeDef definition

TableResourceUnionTypeDef = Union[
    TableResourceTypeDef,  # (1)
    TableResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TableResourceTypeDef](./type_defs.md#tableresourcetypedef) 
2. See [:material-code-braces: TableResourceOutputTypeDef](./type_defs.md#tableresourceoutputtypedef) 

## RowFilterUnionTypeDef

```python
# RowFilterUnionTypeDef definition

RowFilterUnionTypeDef = Union[
    RowFilterTypeDef,  # (1)
    RowFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RowFilterTypeDef](./type_defs.md#rowfiltertypedef) 
2. See [:material-code-braces: RowFilterOutputTypeDef](./type_defs.md#rowfilteroutputtypedef) 

## PrincipalPermissionsUnionTypeDef

```python
# PrincipalPermissionsUnionTypeDef definition

PrincipalPermissionsUnionTypeDef = Union[
    PrincipalPermissionsTypeDef,  # (1)
    PrincipalPermissionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef) 
2. See [:material-code-braces: PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef) 

## TableWithColumnsResourceUnionTypeDef

```python
# TableWithColumnsResourceUnionTypeDef definition

TableWithColumnsResourceUnionTypeDef = Union[
    TableWithColumnsResourceTypeDef,  # (1)
    TableWithColumnsResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TableWithColumnsResourceTypeDef](./type_defs.md#tablewithcolumnsresourcetypedef) 
2. See [:material-code-braces: TableWithColumnsResourceOutputTypeDef](./type_defs.md#tablewithcolumnsresourceoutputtypedef) 

## LFTagPolicyResourceUnionTypeDef

```python
# LFTagPolicyResourceUnionTypeDef definition

LFTagPolicyResourceUnionTypeDef = Union[
    LFTagPolicyResourceTypeDef,  # (1)
    LFTagPolicyResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LFTagPolicyResourceTypeDef](./type_defs.md#lftagpolicyresourcetypedef) 
2. See [:material-code-braces: LFTagPolicyResourceOutputTypeDef](./type_defs.md#lftagpolicyresourceoutputtypedef) 

## ResourceUnionTypeDef

```python
# ResourceUnionTypeDef definition

ResourceUnionTypeDef = Union[
    ResourceTypeDef,  # (1)
    ResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 

## BatchPermissionsRequestEntryUnionTypeDef

```python
# BatchPermissionsRequestEntryUnionTypeDef definition

BatchPermissionsRequestEntryUnionTypeDef = Union[
    BatchPermissionsRequestEntryTypeDef,  # (1)
    BatchPermissionsRequestEntryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BatchPermissionsRequestEntryTypeDef](./type_defs.md#batchpermissionsrequestentrytypedef) 
2. See [:material-code-braces: BatchPermissionsRequestEntryOutputTypeDef](./type_defs.md#batchpermissionsrequestentryoutputtypedef) 



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

## AddObjectInputTypeDef

```python
# AddObjectInputTypeDef definition

class AddObjectInputTypeDef(TypedDict):
    Uri: str,
    ETag: str,
    Size: int,
    PartitionValues: NotRequired[Sequence[str]],
```

## AssumeDecoratedRoleWithSAMLRequestRequestTypeDef

```python
# AssumeDecoratedRoleWithSAMLRequestRequestTypeDef definition

class AssumeDecoratedRoleWithSAMLRequestRequestTypeDef(TypedDict):
    SAMLAssertion: str,
    RoleArn: str,
    PrincipalArn: str,
    DurationSeconds: NotRequired[int],
```

## AuditContextTypeDef

```python
# AuditContextTypeDef definition

class AuditContextTypeDef(TypedDict):
    AdditionalAuditContext: NotRequired[str],
```

## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## DataLakePrincipalTypeDef

```python
# DataLakePrincipalTypeDef definition

class DataLakePrincipalTypeDef(TypedDict):
    DataLakePrincipalIdentifier: NotRequired[str],
```

## CancelTransactionRequestRequestTypeDef

```python
# CancelTransactionRequestRequestTypeDef definition

class CancelTransactionRequestRequestTypeDef(TypedDict):
    TransactionId: str,
```

## LFTagPairOutputTypeDef

```python
# LFTagPairOutputTypeDef definition

class LFTagPairOutputTypeDef(TypedDict):
    TagKey: str,
    TagValues: List[str],
    CatalogId: NotRequired[str],
```

## ColumnWildcardOutputTypeDef

```python
# ColumnWildcardOutputTypeDef definition

class ColumnWildcardOutputTypeDef(TypedDict):
    ExcludedColumnNames: NotRequired[List[str]],
```

## ColumnWildcardTypeDef

```python
# ColumnWildcardTypeDef definition

class ColumnWildcardTypeDef(TypedDict):
    ExcludedColumnNames: NotRequired[Sequence[str]],
```

## CommitTransactionRequestRequestTypeDef

```python
# CommitTransactionRequestRequestTypeDef definition

class CommitTransactionRequestRequestTypeDef(TypedDict):
    TransactionId: str,
```

## CreateLFTagRequestRequestTypeDef

```python
# CreateLFTagRequestRequestTypeDef definition

class CreateLFTagRequestRequestTypeDef(TypedDict):
    TagKey: str,
    TagValues: Sequence[str],
    CatalogId: NotRequired[str],
```

## ExternalFilteringConfigurationTypeDef

```python
# ExternalFilteringConfigurationTypeDef definition

class ExternalFilteringConfigurationTypeDef(TypedDict):
    Status: EnableStatusType,  # (1)
    AuthorizedTargets: Sequence[str],
```

1. See [:material-code-brackets: EnableStatusType](./literals.md#enablestatustype) 
## RowFilterOutputTypeDef

```python
# RowFilterOutputTypeDef definition

class RowFilterOutputTypeDef(TypedDict):
    FilterExpression: NotRequired[str],
    AllRowsWildcard: NotRequired[Dict[str, Any]],
```

## DataCellsFilterResourceTypeDef

```python
# DataCellsFilterResourceTypeDef definition

class DataCellsFilterResourceTypeDef(TypedDict):
    TableCatalogId: NotRequired[str],
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    Name: NotRequired[str],
```

## DataLocationResourceTypeDef

```python
# DataLocationResourceTypeDef definition

class DataLocationResourceTypeDef(TypedDict):
    ResourceArn: str,
    CatalogId: NotRequired[str],
```

## DatabaseResourceTypeDef

```python
# DatabaseResourceTypeDef definition

class DatabaseResourceTypeDef(TypedDict):
    Name: str,
    CatalogId: NotRequired[str],
```

## DeleteDataCellsFilterRequestRequestTypeDef

```python
# DeleteDataCellsFilterRequestRequestTypeDef definition

class DeleteDataCellsFilterRequestRequestTypeDef(TypedDict):
    TableCatalogId: NotRequired[str],
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    Name: NotRequired[str],
```

## DeleteLFTagRequestRequestTypeDef

```python
# DeleteLFTagRequestRequestTypeDef definition

class DeleteLFTagRequestRequestTypeDef(TypedDict):
    TagKey: str,
    CatalogId: NotRequired[str],
```

## DeleteLakeFormationIdentityCenterConfigurationRequestRequestTypeDef

```python
# DeleteLakeFormationIdentityCenterConfigurationRequestRequestTypeDef definition

class DeleteLakeFormationIdentityCenterConfigurationRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
```

## DeleteObjectInputTypeDef

```python
# DeleteObjectInputTypeDef definition

class DeleteObjectInputTypeDef(TypedDict):
    Uri: str,
    ETag: NotRequired[str],
    PartitionValues: NotRequired[Sequence[str]],
```

## VirtualObjectTypeDef

```python
# VirtualObjectTypeDef definition

class VirtualObjectTypeDef(TypedDict):
    Uri: str,
    ETag: NotRequired[str],
```

## DeregisterResourceRequestRequestTypeDef

```python
# DeregisterResourceRequestRequestTypeDef definition

class DeregisterResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DescribeLakeFormationIdentityCenterConfigurationRequestRequestTypeDef

```python
# DescribeLakeFormationIdentityCenterConfigurationRequestRequestTypeDef definition

class DescribeLakeFormationIdentityCenterConfigurationRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
```

## ExternalFilteringConfigurationOutputTypeDef

```python
# ExternalFilteringConfigurationOutputTypeDef definition

class ExternalFilteringConfigurationOutputTypeDef(TypedDict):
    Status: EnableStatusType,  # (1)
    AuthorizedTargets: List[str],
```

1. See [:material-code-brackets: EnableStatusType](./literals.md#enablestatustype) 
## DescribeResourceRequestRequestTypeDef

```python
# DescribeResourceRequestRequestTypeDef definition

class DescribeResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ResourceInfoTypeDef

```python
# ResourceInfoTypeDef definition

class ResourceInfoTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    RoleArn: NotRequired[str],
    LastModified: NotRequired[datetime],
    WithFederation: NotRequired[bool],
    HybridAccessEnabled: NotRequired[bool],
```

## DescribeTransactionRequestRequestTypeDef

```python
# DescribeTransactionRequestRequestTypeDef definition

class DescribeTransactionRequestRequestTypeDef(TypedDict):
    TransactionId: str,
```

## TransactionDescriptionTypeDef

```python
# TransactionDescriptionTypeDef definition

class TransactionDescriptionTypeDef(TypedDict):
    TransactionId: NotRequired[str],
    TransactionStatus: NotRequired[TransactionStatusType],  # (1)
    TransactionStartTime: NotRequired[datetime],
    TransactionEndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: TransactionStatusType](./literals.md#transactionstatustype) 
## DetailsMapTypeDef

```python
# DetailsMapTypeDef definition

class DetailsMapTypeDef(TypedDict):
    ResourceShare: NotRequired[List[str]],
```

## ExecutionStatisticsTypeDef

```python
# ExecutionStatisticsTypeDef definition

class ExecutionStatisticsTypeDef(TypedDict):
    AverageExecutionTimeMillis: NotRequired[int],
    DataScannedBytes: NotRequired[int],
    WorkUnitsExecutedCount: NotRequired[int],
```

## ExtendTransactionRequestRequestTypeDef

```python
# ExtendTransactionRequestRequestTypeDef definition

class ExtendTransactionRequestRequestTypeDef(TypedDict):
    TransactionId: NotRequired[str],
```

## FilterConditionTypeDef

```python
# FilterConditionTypeDef definition

class FilterConditionTypeDef(TypedDict):
    Field: NotRequired[FieldNameStringType],  # (1)
    ComparisonOperator: NotRequired[ComparisonOperatorType],  # (2)
    StringValueList: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: FieldNameStringType](./literals.md#fieldnamestringtype) 
2. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## GetDataCellsFilterRequestRequestTypeDef

```python
# GetDataCellsFilterRequestRequestTypeDef definition

class GetDataCellsFilterRequestRequestTypeDef(TypedDict):
    TableCatalogId: str,
    DatabaseName: str,
    TableName: str,
    Name: str,
```

## GetDataLakeSettingsRequestRequestTypeDef

```python
# GetDataLakeSettingsRequestRequestTypeDef definition

class GetDataLakeSettingsRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
```

## GetEffectivePermissionsForPathRequestRequestTypeDef

```python
# GetEffectivePermissionsForPathRequestRequestTypeDef definition

class GetEffectivePermissionsForPathRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    CatalogId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetLFTagRequestRequestTypeDef

```python
# GetLFTagRequestRequestTypeDef definition

class GetLFTagRequestRequestTypeDef(TypedDict):
    TagKey: str,
    CatalogId: NotRequired[str],
```

## GetQueryStateRequestRequestTypeDef

```python
# GetQueryStateRequestRequestTypeDef definition

class GetQueryStateRequestRequestTypeDef(TypedDict):
    QueryId: str,
```

## GetQueryStatisticsRequestRequestTypeDef

```python
# GetQueryStatisticsRequestRequestTypeDef definition

class GetQueryStatisticsRequestRequestTypeDef(TypedDict):
    QueryId: str,
```

## PlanningStatisticsTypeDef

```python
# PlanningStatisticsTypeDef definition

class PlanningStatisticsTypeDef(TypedDict):
    EstimatedDataToScanBytes: NotRequired[int],
    PlanningTimeMillis: NotRequired[int],
    QueueTimeMillis: NotRequired[int],
    WorkUnitsGeneratedCount: NotRequired[int],
```

## PartitionValueListTypeDef

```python
# PartitionValueListTypeDef definition

class PartitionValueListTypeDef(TypedDict):
    Values: Sequence[str],
```

## GetWorkUnitResultsRequestRequestTypeDef

```python
# GetWorkUnitResultsRequestRequestTypeDef definition

class GetWorkUnitResultsRequestRequestTypeDef(TypedDict):
    QueryId: str,
    WorkUnitId: int,
    WorkUnitToken: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetWorkUnitsRequestRequestTypeDef

```python
# GetWorkUnitsRequestRequestTypeDef definition

class GetWorkUnitsRequestRequestTypeDef(TypedDict):
    QueryId: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## WorkUnitRangeTypeDef

```python
# WorkUnitRangeTypeDef definition

class WorkUnitRangeTypeDef(TypedDict):
    WorkUnitIdMax: int,
    WorkUnitIdMin: int,
    WorkUnitToken: str,
```

## LFTagKeyResourceOutputTypeDef

```python
# LFTagKeyResourceOutputTypeDef definition

class LFTagKeyResourceOutputTypeDef(TypedDict):
    TagKey: str,
    TagValues: List[str],
    CatalogId: NotRequired[str],
```

## LFTagKeyResourceTypeDef

```python
# LFTagKeyResourceTypeDef definition

class LFTagKeyResourceTypeDef(TypedDict):
    TagKey: str,
    TagValues: Sequence[str],
    CatalogId: NotRequired[str],
```

## LFTagOutputTypeDef

```python
# LFTagOutputTypeDef definition

class LFTagOutputTypeDef(TypedDict):
    TagKey: str,
    TagValues: List[str],
```

## LFTagPairTypeDef

```python
# LFTagPairTypeDef definition

class LFTagPairTypeDef(TypedDict):
    TagKey: str,
    TagValues: Sequence[str],
    CatalogId: NotRequired[str],
```

## LFTagTypeDef

```python
# LFTagTypeDef definition

class LFTagTypeDef(TypedDict):
    TagKey: str,
    TagValues: Sequence[str],
```

## TableResourceTypeDef

```python
# TableResourceTypeDef definition

class TableResourceTypeDef(TypedDict):
    DatabaseName: str,
    CatalogId: NotRequired[str],
    Name: NotRequired[str],
    TableWildcard: NotRequired[Mapping[str, Any]],
```

## ListLFTagsRequestRequestTypeDef

```python
# ListLFTagsRequestRequestTypeDef definition

class ListLFTagsRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    ResourceShareType: NotRequired[ResourceShareTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
## ListTableStorageOptimizersRequestRequestTypeDef

```python
# ListTableStorageOptimizersRequestRequestTypeDef definition

class ListTableStorageOptimizersRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    StorageOptimizerType: NotRequired[OptimizerTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: OptimizerTypeType](./literals.md#optimizertypetype) 
## StorageOptimizerTypeDef

```python
# StorageOptimizerTypeDef definition

class StorageOptimizerTypeDef(TypedDict):
    StorageOptimizerType: NotRequired[OptimizerTypeType],  # (1)
    Config: NotRequired[Dict[str, str]],
    ErrorMessage: NotRequired[str],
    Warnings: NotRequired[str],
    LastRunDetails: NotRequired[str],
```

1. See [:material-code-brackets: OptimizerTypeType](./literals.md#optimizertypetype) 
## ListTransactionsRequestRequestTypeDef

```python
# ListTransactionsRequestRequestTypeDef definition

class ListTransactionsRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    StatusFilter: NotRequired[TransactionStatusFilterType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: TransactionStatusFilterType](./literals.md#transactionstatusfiltertype) 
## TableObjectTypeDef

```python
# TableObjectTypeDef definition

class TableObjectTypeDef(TypedDict):
    Uri: NotRequired[str],
    ETag: NotRequired[str],
    Size: NotRequired[int],
```

## RegisterResourceRequestRequestTypeDef

```python
# RegisterResourceRequestRequestTypeDef definition

class RegisterResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    UseServiceLinkedRole: NotRequired[bool],
    RoleArn: NotRequired[str],
    WithFederation: NotRequired[bool],
    HybridAccessEnabled: NotRequired[bool],
```

## TableResourceOutputTypeDef

```python
# TableResourceOutputTypeDef definition

class TableResourceOutputTypeDef(TypedDict):
    DatabaseName: str,
    CatalogId: NotRequired[str],
    Name: NotRequired[str],
    TableWildcard: NotRequired[Dict[str, Any]],
```

## RowFilterTypeDef

```python
# RowFilterTypeDef definition

class RowFilterTypeDef(TypedDict):
    FilterExpression: NotRequired[str],
    AllRowsWildcard: NotRequired[Mapping[str, Any]],
```

## StartTransactionRequestRequestTypeDef

```python
# StartTransactionRequestRequestTypeDef definition

class StartTransactionRequestRequestTypeDef(TypedDict):
    TransactionType: NotRequired[TransactionTypeType],  # (1)
```

1. See [:material-code-brackets: TransactionTypeType](./literals.md#transactiontypetype) 
## UpdateLFTagRequestRequestTypeDef

```python
# UpdateLFTagRequestRequestTypeDef definition

class UpdateLFTagRequestRequestTypeDef(TypedDict):
    TagKey: str,
    CatalogId: NotRequired[str],
    TagValuesToDelete: NotRequired[Sequence[str]],
    TagValuesToAdd: NotRequired[Sequence[str]],
```

## UpdateResourceRequestRequestTypeDef

```python
# UpdateResourceRequestRequestTypeDef definition

class UpdateResourceRequestRequestTypeDef(TypedDict):
    RoleArn: str,
    ResourceArn: str,
    WithFederation: NotRequired[bool],
    HybridAccessEnabled: NotRequired[bool],
```

## UpdateTableStorageOptimizerRequestRequestTypeDef

```python
# UpdateTableStorageOptimizerRequestRequestTypeDef definition

class UpdateTableStorageOptimizerRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    StorageOptimizerConfig: Mapping[OptimizerTypeType, Mapping[str, str]],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-brackets: OptimizerTypeType](./literals.md#optimizertypetype) 
## AssumeDecoratedRoleWithSAMLResponseTypeDef

```python
# AssumeDecoratedRoleWithSAMLResponseTypeDef definition

class AssumeDecoratedRoleWithSAMLResponseTypeDef(TypedDict):
    AccessKeyId: str,
    SecretAccessKey: str,
    SessionToken: str,
    Expiration: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CommitTransactionResponseTypeDef

```python
# CommitTransactionResponseTypeDef definition

class CommitTransactionResponseTypeDef(TypedDict):
    TransactionStatus: TransactionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TransactionStatusType](./literals.md#transactionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLakeFormationIdentityCenterConfigurationResponseTypeDef

```python
# CreateLakeFormationIdentityCenterConfigurationResponseTypeDef definition

class CreateLakeFormationIdentityCenterConfigurationResponseTypeDef(TypedDict):
    ApplicationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataLakePrincipalResponseTypeDef

```python
# GetDataLakePrincipalResponseTypeDef definition

class GetDataLakePrincipalResponseTypeDef(TypedDict):
    Identity: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLFTagResponseTypeDef

```python
# GetLFTagResponseTypeDef definition

class GetLFTagResponseTypeDef(TypedDict):
    CatalogId: str,
    TagKey: str,
    TagValues: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueryStateResponseTypeDef

```python
# GetQueryStateResponseTypeDef definition

class GetQueryStateResponseTypeDef(TypedDict):
    Error: str,
    State: QueryStateStringType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: QueryStateStringType](./literals.md#querystatestringtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTemporaryGluePartitionCredentialsResponseTypeDef

```python
# GetTemporaryGluePartitionCredentialsResponseTypeDef definition

class GetTemporaryGluePartitionCredentialsResponseTypeDef(TypedDict):
    AccessKeyId: str,
    SecretAccessKey: str,
    SessionToken: str,
    Expiration: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTemporaryGlueTableCredentialsResponseTypeDef

```python
# GetTemporaryGlueTableCredentialsResponseTypeDef definition

class GetTemporaryGlueTableCredentialsResponseTypeDef(TypedDict):
    AccessKeyId: str,
    SecretAccessKey: str,
    SessionToken: str,
    Expiration: datetime,
    VendedS3Path: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkUnitResultsResponseTypeDef

```python
# GetWorkUnitResultsResponseTypeDef definition

class GetWorkUnitResultsResponseTypeDef(TypedDict):
    ResultStream: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartQueryPlanningResponseTypeDef

```python
# StartQueryPlanningResponseTypeDef definition

class StartQueryPlanningResponseTypeDef(TypedDict):
    QueryId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTransactionResponseTypeDef

```python
# StartTransactionResponseTypeDef definition

class StartTransactionResponseTypeDef(TypedDict):
    TransactionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableStorageOptimizerResponseTypeDef

```python
# UpdateTableStorageOptimizerResponseTypeDef definition

class UpdateTableStorageOptimizerResponseTypeDef(TypedDict):
    Result: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PrincipalPermissionsOutputTypeDef

```python
# PrincipalPermissionsOutputTypeDef definition

class PrincipalPermissionsOutputTypeDef(TypedDict):
    Principal: NotRequired[DataLakePrincipalTypeDef],  # (1)
    Permissions: NotRequired[List[PermissionType]],  # (2)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## PrincipalPermissionsTypeDef

```python
# PrincipalPermissionsTypeDef definition

class PrincipalPermissionsTypeDef(TypedDict):
    Principal: NotRequired[DataLakePrincipalTypeDef],  # (1)
    Permissions: NotRequired[Sequence[PermissionType]],  # (2)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## ColumnLFTagTypeDef

```python
# ColumnLFTagTypeDef definition

class ColumnLFTagTypeDef(TypedDict):
    Name: NotRequired[str],
    LFTags: NotRequired[List[LFTagPairOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef) 
## LFTagErrorTypeDef

```python
# LFTagErrorTypeDef definition

class LFTagErrorTypeDef(TypedDict):
    LFTag: NotRequired[LFTagPairOutputTypeDef],  # (1)
    Error: NotRequired[ErrorDetailTypeDef],  # (2)
```

1. See [:material-code-braces: LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## ListLFTagsResponseTypeDef

```python
# ListLFTagsResponseTypeDef definition

class ListLFTagsResponseTypeDef(TypedDict):
    LFTags: List[LFTagPairOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableWithColumnsResourceOutputTypeDef

```python
# TableWithColumnsResourceOutputTypeDef definition

class TableWithColumnsResourceOutputTypeDef(TypedDict):
    DatabaseName: str,
    Name: str,
    CatalogId: NotRequired[str],
    ColumnNames: NotRequired[List[str]],
    ColumnWildcard: NotRequired[ColumnWildcardOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ColumnWildcardOutputTypeDef](./type_defs.md#columnwildcardoutputtypedef) 
## CreateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef

```python
# CreateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef definition

class CreateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    InstanceArn: NotRequired[str],
    ExternalFiltering: NotRequired[ExternalFilteringConfigurationTypeDef],  # (1)
    ShareRecipients: NotRequired[Sequence[DataLakePrincipalTypeDef]],  # (2)
```

1. See [:material-code-braces: ExternalFilteringConfigurationTypeDef](./type_defs.md#externalfilteringconfigurationtypedef) 
2. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
## UpdateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef

```python
# UpdateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef definition

class UpdateLakeFormationIdentityCenterConfigurationRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    ShareRecipients: NotRequired[Sequence[DataLakePrincipalTypeDef]],  # (1)
    ApplicationStatus: NotRequired[ApplicationStatusType],  # (2)
    ExternalFiltering: NotRequired[ExternalFilteringConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
3. See [:material-code-braces: ExternalFilteringConfigurationTypeDef](./type_defs.md#externalfilteringconfigurationtypedef) 
## DataCellsFilterOutputTypeDef

```python
# DataCellsFilterOutputTypeDef definition

class DataCellsFilterOutputTypeDef(TypedDict):
    TableCatalogId: str,
    DatabaseName: str,
    TableName: str,
    Name: str,
    RowFilter: NotRequired[RowFilterOutputTypeDef],  # (1)
    ColumnNames: NotRequired[List[str]],
    ColumnWildcard: NotRequired[ColumnWildcardOutputTypeDef],  # (2)
    VersionId: NotRequired[str],
```

1. See [:material-code-braces: RowFilterOutputTypeDef](./type_defs.md#rowfilteroutputtypedef) 
2. See [:material-code-braces: ColumnWildcardOutputTypeDef](./type_defs.md#columnwildcardoutputtypedef) 
## TaggedDatabaseTypeDef

```python
# TaggedDatabaseTypeDef definition

class TaggedDatabaseTypeDef(TypedDict):
    Database: NotRequired[DatabaseResourceTypeDef],  # (1)
    LFTags: NotRequired[List[LFTagPairOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: DatabaseResourceTypeDef](./type_defs.md#databaseresourcetypedef) 
2. See [:material-code-braces: LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef) 
## WriteOperationTypeDef

```python
# WriteOperationTypeDef definition

class WriteOperationTypeDef(TypedDict):
    AddObject: NotRequired[AddObjectInputTypeDef],  # (1)
    DeleteObject: NotRequired[DeleteObjectInputTypeDef],  # (2)
```

1. See [:material-code-braces: AddObjectInputTypeDef](./type_defs.md#addobjectinputtypedef) 
2. See [:material-code-braces: DeleteObjectInputTypeDef](./type_defs.md#deleteobjectinputtypedef) 
## DeleteObjectsOnCancelRequestRequestTypeDef

```python
# DeleteObjectsOnCancelRequestRequestTypeDef definition

class DeleteObjectsOnCancelRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    TransactionId: str,
    Objects: Sequence[VirtualObjectTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: VirtualObjectTypeDef](./type_defs.md#virtualobjecttypedef) 
## DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef

```python
# DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef definition

class DescribeLakeFormationIdentityCenterConfigurationResponseTypeDef(TypedDict):
    CatalogId: str,
    InstanceArn: str,
    ApplicationArn: str,
    ExternalFiltering: ExternalFilteringConfigurationOutputTypeDef,  # (1)
    ShareRecipients: List[DataLakePrincipalTypeDef],  # (2)
    ResourceShare: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ExternalFilteringConfigurationOutputTypeDef](./type_defs.md#externalfilteringconfigurationoutputtypedef) 
2. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResourceResponseTypeDef

```python
# DescribeResourceResponseTypeDef definition

class DescribeResourceResponseTypeDef(TypedDict):
    ResourceInfo: ResourceInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceInfoTypeDef](./type_defs.md#resourceinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesResponseTypeDef

```python
# ListResourcesResponseTypeDef definition

class ListResourcesResponseTypeDef(TypedDict):
    ResourceInfoList: List[ResourceInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceInfoTypeDef](./type_defs.md#resourceinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTransactionResponseTypeDef

```python
# DescribeTransactionResponseTypeDef definition

class DescribeTransactionResponseTypeDef(TypedDict):
    TransactionDescription: TransactionDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TransactionDescriptionTypeDef](./type_defs.md#transactiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTransactionsResponseTypeDef

```python
# ListTransactionsResponseTypeDef definition

class ListTransactionsResponseTypeDef(TypedDict):
    Transactions: List[TransactionDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TransactionDescriptionTypeDef](./type_defs.md#transactiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesRequestRequestTypeDef

```python
# ListResourcesRequestRequestTypeDef definition

class ListResourcesRequestRequestTypeDef(TypedDict):
    FilterConditionList: NotRequired[Sequence[FilterConditionTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterConditionTypeDef](./type_defs.md#filterconditiontypedef) 
## GetQueryStatisticsResponseTypeDef

```python
# GetQueryStatisticsResponseTypeDef definition

class GetQueryStatisticsResponseTypeDef(TypedDict):
    ExecutionStatistics: ExecutionStatisticsTypeDef,  # (1)
    PlanningStatistics: PlanningStatisticsTypeDef,  # (2)
    QuerySubmissionTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ExecutionStatisticsTypeDef](./type_defs.md#executionstatisticstypedef) 
2. See [:material-code-braces: PlanningStatisticsTypeDef](./type_defs.md#planningstatisticstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableObjectsRequestRequestTypeDef

```python
# GetTableObjectsRequestRequestTypeDef definition

class GetTableObjectsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    TransactionId: NotRequired[str],
    QueryAsOfTime: NotRequired[TimestampTypeDef],
    PartitionPredicate: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## QueryPlanningContextTypeDef

```python
# QueryPlanningContextTypeDef definition

class QueryPlanningContextTypeDef(TypedDict):
    DatabaseName: str,
    CatalogId: NotRequired[str],
    QueryAsOfTime: NotRequired[TimestampTypeDef],
    QueryParameters: NotRequired[Mapping[str, str]],
    TransactionId: NotRequired[str],
```

## QuerySessionContextTypeDef

```python
# QuerySessionContextTypeDef definition

class QuerySessionContextTypeDef(TypedDict):
    QueryId: NotRequired[str],
    QueryStartTime: NotRequired[TimestampTypeDef],
    ClusterId: NotRequired[str],
    QueryAuthorizationId: NotRequired[str],
    AdditionalContext: NotRequired[Mapping[str, str]],
```

## GetTemporaryGluePartitionCredentialsRequestRequestTypeDef

```python
# GetTemporaryGluePartitionCredentialsRequestRequestTypeDef definition

class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(TypedDict):
    TableArn: str,
    Partition: PartitionValueListTypeDef,  # (1)
    Permissions: NotRequired[Sequence[PermissionType]],  # (2)
    DurationSeconds: NotRequired[int],
    AuditContext: NotRequired[AuditContextTypeDef],  # (3)
    SupportedPermissionTypes: NotRequired[Sequence[PermissionTypeType]],  # (4)
```

1. See [:material-code-braces: PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
3. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
4. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
## GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef

```python
# GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef definition

class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(TypedDict):
    QueryId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLFTagsRequestListLFTagsPaginateTypeDef

```python
# ListLFTagsRequestListLFTagsPaginateTypeDef definition

class ListLFTagsRequestListLFTagsPaginateTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    ResourceShareType: NotRequired[ResourceShareTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetWorkUnitsResponseTypeDef

```python
# GetWorkUnitsResponseTypeDef definition

class GetWorkUnitsResponseTypeDef(TypedDict):
    QueryId: str,
    WorkUnitRanges: List[WorkUnitRangeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkUnitRangeTypeDef](./type_defs.md#workunitrangetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LFTagPolicyResourceOutputTypeDef

```python
# LFTagPolicyResourceOutputTypeDef definition

class LFTagPolicyResourceOutputTypeDef(TypedDict):
    ResourceType: ResourceTypeType,  # (1)
    Expression: List[LFTagOutputTypeDef],  # (2)
    CatalogId: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: LFTagOutputTypeDef](./type_defs.md#lftagoutputtypedef) 
## SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef

```python
# SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef definition

class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(TypedDict):
    Expression: Sequence[LFTagTypeDef],  # (1)
    CatalogId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchTablesByLFTagsRequestRequestTypeDef

```python
# SearchTablesByLFTagsRequestRequestTypeDef definition

class SearchTablesByLFTagsRequestRequestTypeDef(TypedDict):
    Expression: Sequence[LFTagTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
## SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef

```python
# SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef definition

class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(TypedDict):
    Expression: Sequence[LFTagTypeDef],  # (1)
    CatalogId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef

```python
# ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef definition

class ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef(TypedDict):
    Table: NotRequired[TableResourceTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TableResourceTypeDef](./type_defs.md#tableresourcetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataCellsFilterRequestRequestTypeDef

```python
# ListDataCellsFilterRequestRequestTypeDef definition

class ListDataCellsFilterRequestRequestTypeDef(TypedDict):
    Table: NotRequired[TableResourceTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: TableResourceTypeDef](./type_defs.md#tableresourcetypedef) 
## ListTableStorageOptimizersResponseTypeDef

```python
# ListTableStorageOptimizersResponseTypeDef definition

class ListTableStorageOptimizersResponseTypeDef(TypedDict):
    StorageOptimizerList: List[StorageOptimizerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StorageOptimizerTypeDef](./type_defs.md#storageoptimizertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PartitionObjectsTypeDef

```python
# PartitionObjectsTypeDef definition

class PartitionObjectsTypeDef(TypedDict):
    PartitionValues: NotRequired[List[str]],
    Objects: NotRequired[List[TableObjectTypeDef]],  # (1)
```

1. See [:material-code-braces: TableObjectTypeDef](./type_defs.md#tableobjecttypedef) 
## DataLakeSettingsOutputTypeDef

```python
# DataLakeSettingsOutputTypeDef definition

class DataLakeSettingsOutputTypeDef(TypedDict):
    DataLakeAdmins: NotRequired[List[DataLakePrincipalTypeDef]],  # (1)
    ReadOnlyAdmins: NotRequired[List[DataLakePrincipalTypeDef]],  # (1)
    CreateDatabaseDefaultPermissions: NotRequired[List[PrincipalPermissionsOutputTypeDef]],  # (3)
    CreateTableDefaultPermissions: NotRequired[List[PrincipalPermissionsOutputTypeDef]],  # (3)
    Parameters: NotRequired[Dict[str, str]],
    TrustedResourceOwners: NotRequired[List[str]],
    AllowExternalDataFiltering: NotRequired[bool],
    AllowFullTableExternalDataAccess: NotRequired[bool],
    ExternalDataFilteringAllowList: NotRequired[List[DataLakePrincipalTypeDef]],  # (1)
    AuthorizedSessionTagValueList: NotRequired[List[str]],
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
3. See [:material-code-braces: PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef) 
4. See [:material-code-braces: PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef) 
5. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
## GetResourceLFTagsResponseTypeDef

```python
# GetResourceLFTagsResponseTypeDef definition

class GetResourceLFTagsResponseTypeDef(TypedDict):
    LFTagOnDatabase: List[LFTagPairOutputTypeDef],  # (1)
    LFTagsOnTable: List[LFTagPairOutputTypeDef],  # (1)
    LFTagsOnColumns: List[ColumnLFTagTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef) 
2. See [:material-code-braces: LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef) 
3. See [:material-code-braces: ColumnLFTagTypeDef](./type_defs.md#columnlftagtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TaggedTableTypeDef

```python
# TaggedTableTypeDef definition

class TaggedTableTypeDef(TypedDict):
    Table: NotRequired[TableResourceOutputTypeDef],  # (1)
    LFTagOnDatabase: NotRequired[List[LFTagPairOutputTypeDef]],  # (2)
    LFTagsOnTable: NotRequired[List[LFTagPairOutputTypeDef]],  # (2)
    LFTagsOnColumns: NotRequired[List[ColumnLFTagTypeDef]],  # (4)
```

1. See [:material-code-braces: TableResourceOutputTypeDef](./type_defs.md#tableresourceoutputtypedef) 
2. See [:material-code-braces: LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef) 
3. See [:material-code-braces: LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef) 
4. See [:material-code-braces: ColumnLFTagTypeDef](./type_defs.md#columnlftagtypedef) 
## AddLFTagsToResourceResponseTypeDef

```python
# AddLFTagsToResourceResponseTypeDef definition

class AddLFTagsToResourceResponseTypeDef(TypedDict):
    Failures: List[LFTagErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LFTagErrorTypeDef](./type_defs.md#lftagerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveLFTagsFromResourceResponseTypeDef

```python
# RemoveLFTagsFromResourceResponseTypeDef definition

class RemoveLFTagsFromResourceResponseTypeDef(TypedDict):
    Failures: List[LFTagErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LFTagErrorTypeDef](./type_defs.md#lftagerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableWithColumnsResourceTypeDef

```python
# TableWithColumnsResourceTypeDef definition

class TableWithColumnsResourceTypeDef(TypedDict):
    DatabaseName: str,
    Name: str,
    CatalogId: NotRequired[str],
    ColumnNames: NotRequired[Sequence[str]],
    ColumnWildcard: NotRequired[ColumnWildcardUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ColumnWildcardTypeDef](./type_defs.md#columnwildcardtypedef) [:material-code-braces: ColumnWildcardOutputTypeDef](./type_defs.md#columnwildcardoutputtypedef) 
## GetDataCellsFilterResponseTypeDef

```python
# GetDataCellsFilterResponseTypeDef definition

class GetDataCellsFilterResponseTypeDef(TypedDict):
    DataCellsFilter: DataCellsFilterOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataCellsFilterOutputTypeDef](./type_defs.md#datacellsfilteroutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataCellsFilterResponseTypeDef

```python
# ListDataCellsFilterResponseTypeDef definition

class ListDataCellsFilterResponseTypeDef(TypedDict):
    DataCellsFilters: List[DataCellsFilterOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataCellsFilterOutputTypeDef](./type_defs.md#datacellsfilteroutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchDatabasesByLFTagsResponseTypeDef

```python
# SearchDatabasesByLFTagsResponseTypeDef definition

class SearchDatabasesByLFTagsResponseTypeDef(TypedDict):
    DatabaseList: List[TaggedDatabaseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TaggedDatabaseTypeDef](./type_defs.md#taggeddatabasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableObjectsRequestRequestTypeDef

```python
# UpdateTableObjectsRequestRequestTypeDef definition

class UpdateTableObjectsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    WriteOperations: Sequence[WriteOperationTypeDef],  # (1)
    CatalogId: NotRequired[str],
    TransactionId: NotRequired[str],
```

1. See [:material-code-braces: WriteOperationTypeDef](./type_defs.md#writeoperationtypedef) 
## StartQueryPlanningRequestRequestTypeDef

```python
# StartQueryPlanningRequestRequestTypeDef definition

class StartQueryPlanningRequestRequestTypeDef(TypedDict):
    QueryPlanningContext: QueryPlanningContextTypeDef,  # (1)
    QueryString: str,
```

1. See [:material-code-braces: QueryPlanningContextTypeDef](./type_defs.md#queryplanningcontexttypedef) 
## GetTemporaryGlueTableCredentialsRequestRequestTypeDef

```python
# GetTemporaryGlueTableCredentialsRequestRequestTypeDef definition

class GetTemporaryGlueTableCredentialsRequestRequestTypeDef(TypedDict):
    TableArn: str,
    Permissions: NotRequired[Sequence[PermissionType]],  # (1)
    DurationSeconds: NotRequired[int],
    AuditContext: NotRequired[AuditContextTypeDef],  # (2)
    SupportedPermissionTypes: NotRequired[Sequence[PermissionTypeType]],  # (3)
    S3Path: NotRequired[str],
    QuerySessionContext: NotRequired[QuerySessionContextTypeDef],  # (4)
```

1. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
2. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
3. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
4. See [:material-code-braces: QuerySessionContextTypeDef](./type_defs.md#querysessioncontexttypedef) 
## ResourceOutputTypeDef

```python
# ResourceOutputTypeDef definition

class ResourceOutputTypeDef(TypedDict):
    Catalog: NotRequired[Dict[str, Any]],
    Database: NotRequired[DatabaseResourceTypeDef],  # (1)
    Table: NotRequired[TableResourceOutputTypeDef],  # (2)
    TableWithColumns: NotRequired[TableWithColumnsResourceOutputTypeDef],  # (3)
    DataLocation: NotRequired[DataLocationResourceTypeDef],  # (4)
    DataCellsFilter: NotRequired[DataCellsFilterResourceTypeDef],  # (5)
    LFTag: NotRequired[LFTagKeyResourceOutputTypeDef],  # (6)
    LFTagPolicy: NotRequired[LFTagPolicyResourceOutputTypeDef],  # (7)
```

1. See [:material-code-braces: DatabaseResourceTypeDef](./type_defs.md#databaseresourcetypedef) 
2. See [:material-code-braces: TableResourceOutputTypeDef](./type_defs.md#tableresourceoutputtypedef) 
3. See [:material-code-braces: TableWithColumnsResourceOutputTypeDef](./type_defs.md#tablewithcolumnsresourceoutputtypedef) 
4. See [:material-code-braces: DataLocationResourceTypeDef](./type_defs.md#datalocationresourcetypedef) 
5. See [:material-code-braces: DataCellsFilterResourceTypeDef](./type_defs.md#datacellsfilterresourcetypedef) 
6. See [:material-code-braces: LFTagKeyResourceOutputTypeDef](./type_defs.md#lftagkeyresourceoutputtypedef) 
7. See [:material-code-braces: LFTagPolicyResourceOutputTypeDef](./type_defs.md#lftagpolicyresourceoutputtypedef) 
## LFTagPolicyResourceTypeDef

```python
# LFTagPolicyResourceTypeDef definition

class LFTagPolicyResourceTypeDef(TypedDict):
    ResourceType: ResourceTypeType,  # (1)
    Expression: Sequence[LFTagUnionTypeDef],  # (2)
    CatalogId: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) [:material-code-braces: LFTagOutputTypeDef](./type_defs.md#lftagoutputtypedef) 
## SearchDatabasesByLFTagsRequestRequestTypeDef

```python
# SearchDatabasesByLFTagsRequestRequestTypeDef definition

class SearchDatabasesByLFTagsRequestRequestTypeDef(TypedDict):
    Expression: Sequence[LFTagUnionTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) [:material-code-braces: LFTagOutputTypeDef](./type_defs.md#lftagoutputtypedef) 
## GetTableObjectsResponseTypeDef

```python
# GetTableObjectsResponseTypeDef definition

class GetTableObjectsResponseTypeDef(TypedDict):
    Objects: List[PartitionObjectsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PartitionObjectsTypeDef](./type_defs.md#partitionobjectstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataCellsFilterTypeDef

```python
# DataCellsFilterTypeDef definition

class DataCellsFilterTypeDef(TypedDict):
    TableCatalogId: str,
    DatabaseName: str,
    TableName: str,
    Name: str,
    RowFilter: NotRequired[RowFilterUnionTypeDef],  # (1)
    ColumnNames: NotRequired[Sequence[str]],
    ColumnWildcard: NotRequired[ColumnWildcardUnionTypeDef],  # (2)
    VersionId: NotRequired[str],
```

1. See [:material-code-braces: RowFilterTypeDef](./type_defs.md#rowfiltertypedef) [:material-code-braces: RowFilterOutputTypeDef](./type_defs.md#rowfilteroutputtypedef) 
2. See [:material-code-braces: ColumnWildcardTypeDef](./type_defs.md#columnwildcardtypedef) [:material-code-braces: ColumnWildcardOutputTypeDef](./type_defs.md#columnwildcardoutputtypedef) 
## GetDataLakeSettingsResponseTypeDef

```python
# GetDataLakeSettingsResponseTypeDef definition

class GetDataLakeSettingsResponseTypeDef(TypedDict):
    DataLakeSettings: DataLakeSettingsOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeSettingsOutputTypeDef](./type_defs.md#datalakesettingsoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataLakeSettingsTypeDef

```python
# DataLakeSettingsTypeDef definition

class DataLakeSettingsTypeDef(TypedDict):
    DataLakeAdmins: NotRequired[Sequence[DataLakePrincipalTypeDef]],  # (1)
    ReadOnlyAdmins: NotRequired[Sequence[DataLakePrincipalTypeDef]],  # (1)
    CreateDatabaseDefaultPermissions: NotRequired[Sequence[PrincipalPermissionsUnionTypeDef]],  # (3)
    CreateTableDefaultPermissions: NotRequired[Sequence[PrincipalPermissionsTypeDef]],  # (4)
    Parameters: NotRequired[Mapping[str, str]],
    TrustedResourceOwners: NotRequired[Sequence[str]],
    AllowExternalDataFiltering: NotRequired[bool],
    AllowFullTableExternalDataAccess: NotRequired[bool],
    ExternalDataFilteringAllowList: NotRequired[Sequence[DataLakePrincipalTypeDef]],  # (1)
    AuthorizedSessionTagValueList: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
3. See [:material-code-braces: PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef) [:material-code-braces: PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef) 
4. See [:material-code-braces: PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef) 
5. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
## SearchTablesByLFTagsResponseTypeDef

```python
# SearchTablesByLFTagsResponseTypeDef definition

class SearchTablesByLFTagsResponseTypeDef(TypedDict):
    TableList: List[TaggedTableTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TaggedTableTypeDef](./type_defs.md#taggedtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPermissionsRequestEntryOutputTypeDef

```python
# BatchPermissionsRequestEntryOutputTypeDef definition

class BatchPermissionsRequestEntryOutputTypeDef(TypedDict):
    Id: str,
    Principal: NotRequired[DataLakePrincipalTypeDef],  # (1)
    Resource: NotRequired[ResourceOutputTypeDef],  # (2)
    Permissions: NotRequired[List[PermissionType]],  # (3)
    PermissionsWithGrantOption: NotRequired[List[PermissionType]],  # (3)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
4. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## LakeFormationOptInsInfoTypeDef

```python
# LakeFormationOptInsInfoTypeDef definition

class LakeFormationOptInsInfoTypeDef(TypedDict):
    Resource: NotRequired[ResourceOutputTypeDef],  # (1)
    Principal: NotRequired[DataLakePrincipalTypeDef],  # (2)
    LastModified: NotRequired[datetime],
    LastUpdatedBy: NotRequired[str],
```

1. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
2. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
## PrincipalResourcePermissionsTypeDef

```python
# PrincipalResourcePermissionsTypeDef definition

class PrincipalResourcePermissionsTypeDef(TypedDict):
    Principal: NotRequired[DataLakePrincipalTypeDef],  # (1)
    Resource: NotRequired[ResourceOutputTypeDef],  # (2)
    Permissions: NotRequired[List[PermissionType]],  # (3)
    PermissionsWithGrantOption: NotRequired[List[PermissionType]],  # (3)
    AdditionalDetails: NotRequired[DetailsMapTypeDef],  # (5)
    LastUpdated: NotRequired[datetime],
    LastUpdatedBy: NotRequired[str],
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
4. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
5. See [:material-code-braces: DetailsMapTypeDef](./type_defs.md#detailsmaptypedef) 
## CreateDataCellsFilterRequestRequestTypeDef

```python
# CreateDataCellsFilterRequestRequestTypeDef definition

class CreateDataCellsFilterRequestRequestTypeDef(TypedDict):
    TableData: DataCellsFilterTypeDef,  # (1)
```

1. See [:material-code-braces: DataCellsFilterTypeDef](./type_defs.md#datacellsfiltertypedef) 
## UpdateDataCellsFilterRequestRequestTypeDef

```python
# UpdateDataCellsFilterRequestRequestTypeDef definition

class UpdateDataCellsFilterRequestRequestTypeDef(TypedDict):
    TableData: DataCellsFilterTypeDef,  # (1)
```

1. See [:material-code-braces: DataCellsFilterTypeDef](./type_defs.md#datacellsfiltertypedef) 
## PutDataLakeSettingsRequestRequestTypeDef

```python
# PutDataLakeSettingsRequestRequestTypeDef definition

class PutDataLakeSettingsRequestRequestTypeDef(TypedDict):
    DataLakeSettings: DataLakeSettingsTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: DataLakeSettingsTypeDef](./type_defs.md#datalakesettingstypedef) 
## BatchPermissionsFailureEntryTypeDef

```python
# BatchPermissionsFailureEntryTypeDef definition

class BatchPermissionsFailureEntryTypeDef(TypedDict):
    RequestEntry: NotRequired[BatchPermissionsRequestEntryOutputTypeDef],  # (1)
    Error: NotRequired[ErrorDetailTypeDef],  # (2)
```

1. See [:material-code-braces: BatchPermissionsRequestEntryOutputTypeDef](./type_defs.md#batchpermissionsrequestentryoutputtypedef) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## ListLakeFormationOptInsResponseTypeDef

```python
# ListLakeFormationOptInsResponseTypeDef definition

class ListLakeFormationOptInsResponseTypeDef(TypedDict):
    LakeFormationOptInsInfoList: List[LakeFormationOptInsInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LakeFormationOptInsInfoTypeDef](./type_defs.md#lakeformationoptinsinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEffectivePermissionsForPathResponseTypeDef

```python
# GetEffectivePermissionsForPathResponseTypeDef definition

class GetEffectivePermissionsForPathResponseTypeDef(TypedDict):
    Permissions: List[PrincipalResourcePermissionsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PrincipalResourcePermissionsTypeDef](./type_defs.md#principalresourcepermissionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionsResponseTypeDef

```python
# ListPermissionsResponseTypeDef definition

class ListPermissionsResponseTypeDef(TypedDict):
    PrincipalResourcePermissions: List[PrincipalResourcePermissionsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PrincipalResourcePermissionsTypeDef](./type_defs.md#principalresourcepermissionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    Catalog: NotRequired[Mapping[str, Any]],
    Database: NotRequired[DatabaseResourceTypeDef],  # (1)
    Table: NotRequired[TableResourceUnionTypeDef],  # (2)
    TableWithColumns: NotRequired[TableWithColumnsResourceUnionTypeDef],  # (3)
    DataLocation: NotRequired[DataLocationResourceTypeDef],  # (4)
    DataCellsFilter: NotRequired[DataCellsFilterResourceTypeDef],  # (5)
    LFTag: NotRequired[LFTagKeyResourceUnionTypeDef],  # (6)
    LFTagPolicy: NotRequired[LFTagPolicyResourceUnionTypeDef],  # (7)
```

1. See [:material-code-braces: DatabaseResourceTypeDef](./type_defs.md#databaseresourcetypedef) 
2. See [:material-code-braces: TableResourceTypeDef](./type_defs.md#tableresourcetypedef) [:material-code-braces: TableResourceOutputTypeDef](./type_defs.md#tableresourceoutputtypedef) 
3. See [:material-code-braces: TableWithColumnsResourceTypeDef](./type_defs.md#tablewithcolumnsresourcetypedef) [:material-code-braces: TableWithColumnsResourceOutputTypeDef](./type_defs.md#tablewithcolumnsresourceoutputtypedef) 
4. See [:material-code-braces: DataLocationResourceTypeDef](./type_defs.md#datalocationresourcetypedef) 
5. See [:material-code-braces: DataCellsFilterResourceTypeDef](./type_defs.md#datacellsfilterresourcetypedef) 
6. See [:material-code-braces: LFTagKeyResourceTypeDef](./type_defs.md#lftagkeyresourcetypedef) [:material-code-braces: LFTagKeyResourceOutputTypeDef](./type_defs.md#lftagkeyresourceoutputtypedef) 
7. See [:material-code-braces: LFTagPolicyResourceTypeDef](./type_defs.md#lftagpolicyresourcetypedef) [:material-code-braces: LFTagPolicyResourceOutputTypeDef](./type_defs.md#lftagpolicyresourceoutputtypedef) 
## BatchGrantPermissionsResponseTypeDef

```python
# BatchGrantPermissionsResponseTypeDef definition

class BatchGrantPermissionsResponseTypeDef(TypedDict):
    Failures: List[BatchPermissionsFailureEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPermissionsFailureEntryTypeDef](./type_defs.md#batchpermissionsfailureentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchRevokePermissionsResponseTypeDef

```python
# BatchRevokePermissionsResponseTypeDef definition

class BatchRevokePermissionsResponseTypeDef(TypedDict):
    Failures: List[BatchPermissionsFailureEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPermissionsFailureEntryTypeDef](./type_defs.md#batchpermissionsfailureentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddLFTagsToResourceRequestRequestTypeDef

```python
# AddLFTagsToResourceRequestRequestTypeDef definition

class AddLFTagsToResourceRequestRequestTypeDef(TypedDict):
    Resource: ResourceTypeDef,  # (1)
    LFTags: Sequence[LFTagPairUnionTypeDef],  # (2)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: LFTagPairTypeDef](./type_defs.md#lftagpairtypedef) [:material-code-braces: LFTagPairOutputTypeDef](./type_defs.md#lftagpairoutputtypedef) 
## CreateLakeFormationOptInRequestRequestTypeDef

```python
# CreateLakeFormationOptInRequestRequestTypeDef definition

class CreateLakeFormationOptInRequestRequestTypeDef(TypedDict):
    Principal: DataLakePrincipalTypeDef,  # (1)
    Resource: ResourceTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## DeleteLakeFormationOptInRequestRequestTypeDef

```python
# DeleteLakeFormationOptInRequestRequestTypeDef definition

class DeleteLakeFormationOptInRequestRequestTypeDef(TypedDict):
    Principal: DataLakePrincipalTypeDef,  # (1)
    Resource: ResourceTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## GetResourceLFTagsRequestRequestTypeDef

```python
# GetResourceLFTagsRequestRequestTypeDef definition

class GetResourceLFTagsRequestRequestTypeDef(TypedDict):
    Resource: ResourceTypeDef,  # (1)
    CatalogId: NotRequired[str],
    ShowAssignedLFTags: NotRequired[bool],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## GrantPermissionsRequestRequestTypeDef

```python
# GrantPermissionsRequestRequestTypeDef definition

class GrantPermissionsRequestRequestTypeDef(TypedDict):
    Principal: DataLakePrincipalTypeDef,  # (1)
    Resource: ResourceTypeDef,  # (2)
    Permissions: Sequence[PermissionType],  # (3)
    CatalogId: NotRequired[str],
    PermissionsWithGrantOption: NotRequired[Sequence[PermissionType]],  # (3)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
4. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## ListLakeFormationOptInsRequestRequestTypeDef

```python
# ListLakeFormationOptInsRequestRequestTypeDef definition

class ListLakeFormationOptInsRequestRequestTypeDef(TypedDict):
    Principal: NotRequired[DataLakePrincipalTypeDef],  # (1)
    Resource: NotRequired[ResourceTypeDef],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## ListPermissionsRequestRequestTypeDef

```python
# ListPermissionsRequestRequestTypeDef definition

class ListPermissionsRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    Principal: NotRequired[DataLakePrincipalTypeDef],  # (1)
    ResourceType: NotRequired[DataLakeResourceTypeType],  # (2)
    Resource: NotRequired[ResourceTypeDef],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    IncludeRelated: NotRequired[str],
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-brackets: DataLakeResourceTypeType](./literals.md#datalakeresourcetypetype) 
3. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## RemoveLFTagsFromResourceRequestRequestTypeDef

```python
# RemoveLFTagsFromResourceRequestRequestTypeDef definition

class RemoveLFTagsFromResourceRequestRequestTypeDef(TypedDict):
    Resource: ResourceTypeDef,  # (1)
    LFTags: Sequence[LFTagPairTypeDef],  # (2)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: LFTagPairTypeDef](./type_defs.md#lftagpairtypedef) 
## RevokePermissionsRequestRequestTypeDef

```python
# RevokePermissionsRequestRequestTypeDef definition

class RevokePermissionsRequestRequestTypeDef(TypedDict):
    Principal: DataLakePrincipalTypeDef,  # (1)
    Resource: ResourceTypeDef,  # (2)
    Permissions: Sequence[PermissionType],  # (3)
    CatalogId: NotRequired[str],
    PermissionsWithGrantOption: NotRequired[Sequence[PermissionType]],  # (3)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
4. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## BatchPermissionsRequestEntryTypeDef

```python
# BatchPermissionsRequestEntryTypeDef definition

class BatchPermissionsRequestEntryTypeDef(TypedDict):
    Id: str,
    Principal: NotRequired[DataLakePrincipalTypeDef],  # (1)
    Resource: NotRequired[ResourceUnionTypeDef],  # (2)
    Permissions: NotRequired[Sequence[PermissionType]],  # (3)
    PermissionsWithGrantOption: NotRequired[Sequence[PermissionType]],  # (3)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
4. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## BatchRevokePermissionsRequestRequestTypeDef

```python
# BatchRevokePermissionsRequestRequestTypeDef definition

class BatchRevokePermissionsRequestRequestTypeDef(TypedDict):
    Entries: Sequence[BatchPermissionsRequestEntryTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: BatchPermissionsRequestEntryTypeDef](./type_defs.md#batchpermissionsrequestentrytypedef) 
## BatchGrantPermissionsRequestRequestTypeDef

```python
# BatchGrantPermissionsRequestRequestTypeDef definition

class BatchGrantPermissionsRequestRequestTypeDef(TypedDict):
    Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: BatchPermissionsRequestEntryTypeDef](./type_defs.md#batchpermissionsrequestentrytypedef) [:material-code-braces: BatchPermissionsRequestEntryOutputTypeDef](./type_defs.md#batchpermissionsrequestentryoutputtypedef) 
