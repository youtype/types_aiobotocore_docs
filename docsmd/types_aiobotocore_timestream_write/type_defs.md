# Type definitions

> [Index](../README.md) > [TimestreamWrite](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [TimestreamWrite](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
    type annotations stubs module [types-aiobotocore-timestream-write](https://pypi.org/project/types-aiobotocore-timestream-write/).



## BatchLoadProgressReportTypeDef

```python
# BatchLoadProgressReportTypeDef definition

class BatchLoadProgressReportTypeDef(TypedDict):
    RecordsProcessed: NotRequired[int],
    RecordsIngested: NotRequired[int],
    ParseFailures: NotRequired[int],
    RecordIngestionFailures: NotRequired[int],
    FileFailures: NotRequired[int],
    BytesMetered: NotRequired[int],
```

## BatchLoadTaskTypeDef

```python
# BatchLoadTaskTypeDef definition

class BatchLoadTaskTypeDef(TypedDict):
    TaskId: NotRequired[str],
    TaskStatus: NotRequired[BatchLoadStatusType],  # (1)
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    ResumableUntil: NotRequired[datetime],
```

1. See [:material-code-brackets: BatchLoadStatusType](./literals.md#batchloadstatustype) 
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

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DatabaseTypeDef

```python
# DatabaseTypeDef definition

class DatabaseTypeDef(TypedDict):
    Arn: NotRequired[str],
    DatabaseName: NotRequired[str],
    TableCount: NotRequired[int],
    KmsKeyId: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

## RetentionPropertiesTypeDef

```python
# RetentionPropertiesTypeDef definition

class RetentionPropertiesTypeDef(TypedDict):
    MemoryStoreRetentionPeriodInHours: int,
    MagneticStoreRetentionPeriodInDays: int,
```

## CsvConfigurationTypeDef

```python
# CsvConfigurationTypeDef definition

class CsvConfigurationTypeDef(TypedDict):
    ColumnSeparator: NotRequired[str],
    EscapeChar: NotRequired[str],
    QuoteChar: NotRequired[str],
    NullValue: NotRequired[str],
    TrimWhiteSpace: NotRequired[bool],
```

## DataModelS3ConfigurationTypeDef

```python
# DataModelS3ConfigurationTypeDef definition

class DataModelS3ConfigurationTypeDef(TypedDict):
    BucketName: NotRequired[str],
    ObjectKey: NotRequired[str],
```

## DimensionMappingTypeDef

```python
# DimensionMappingTypeDef definition

class DimensionMappingTypeDef(TypedDict):
    SourceColumn: NotRequired[str],
    DestinationColumn: NotRequired[str],
```

## DataSourceS3ConfigurationTypeDef

```python
# DataSourceS3ConfigurationTypeDef definition

class DataSourceS3ConfigurationTypeDef(TypedDict):
    BucketName: str,
    ObjectKeyPrefix: NotRequired[str],
```

## DeleteDatabaseRequestRequestTypeDef

```python
# DeleteDatabaseRequestRequestTypeDef definition

class DeleteDatabaseRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
```

## DeleteTableRequestRequestTypeDef

```python
# DeleteTableRequestRequestTypeDef definition

class DeleteTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
```

## DescribeBatchLoadTaskRequestRequestTypeDef

```python
# DescribeBatchLoadTaskRequestRequestTypeDef definition

class DescribeBatchLoadTaskRequestRequestTypeDef(TypedDict):
    TaskId: str,
```

## DescribeDatabaseRequestRequestTypeDef

```python
# DescribeDatabaseRequestRequestTypeDef definition

class DescribeDatabaseRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
```

## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Address: str,
    CachePeriodInMinutes: int,
```

## DescribeTableRequestRequestTypeDef

```python
# DescribeTableRequestRequestTypeDef definition

class DescribeTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
```

## DimensionTypeDef

```python
# DimensionTypeDef definition

class DimensionTypeDef(TypedDict):
    Name: str,
    Value: str,
    DimensionValueType: NotRequired[DimensionValueTypeType],  # (1)
```

1. See [:material-code-brackets: DimensionValueTypeType](./literals.md#dimensionvaluetypetype) 
## ListBatchLoadTasksRequestRequestTypeDef

```python
# ListBatchLoadTasksRequestRequestTypeDef definition

class ListBatchLoadTasksRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    TaskStatus: NotRequired[BatchLoadStatusType],  # (1)
```

1. See [:material-code-brackets: BatchLoadStatusType](./literals.md#batchloadstatustype) 
## ListDatabasesRequestRequestTypeDef

```python
# ListDatabasesRequestRequestTypeDef definition

class ListDatabasesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTablesRequestRequestTypeDef

```python
# ListTablesRequestRequestTypeDef definition

class ListTablesRequestRequestTypeDef(TypedDict):
    DatabaseName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## S3ConfigurationTypeDef

```python
# S3ConfigurationTypeDef definition

class S3ConfigurationTypeDef(TypedDict):
    BucketName: NotRequired[str],
    ObjectKeyPrefix: NotRequired[str],
    EncryptionOption: NotRequired[S3EncryptionOptionType],  # (1)
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: S3EncryptionOptionType](./literals.md#s3encryptionoptiontype) 
## MeasureValueTypeDef

```python
# MeasureValueTypeDef definition

class MeasureValueTypeDef(TypedDict):
    Name: str,
    Value: str,
    Type: MeasureValueTypeType,  # (1)
```

1. See [:material-code-brackets: MeasureValueTypeType](./literals.md#measurevaluetypetype) 
## MultiMeasureAttributeMappingTypeDef

```python
# MultiMeasureAttributeMappingTypeDef definition

class MultiMeasureAttributeMappingTypeDef(TypedDict):
    SourceColumn: str,
    TargetMultiMeasureAttributeName: NotRequired[str],
    MeasureValueType: NotRequired[ScalarMeasureValueTypeType],  # (1)
```

1. See [:material-code-brackets: ScalarMeasureValueTypeType](./literals.md#scalarmeasurevaluetypetype) 
## PartitionKeyTypeDef

```python
# PartitionKeyTypeDef definition

class PartitionKeyTypeDef(TypedDict):
    Type: PartitionKeyTypeType,  # (1)
    Name: NotRequired[str],
    EnforcementInRecord: NotRequired[PartitionKeyEnforcementLevelType],  # (2)
```

1. See [:material-code-brackets: PartitionKeyTypeType](./literals.md#partitionkeytypetype) 
2. See [:material-code-brackets: PartitionKeyEnforcementLevelType](./literals.md#partitionkeyenforcementleveltype) 
## RecordsIngestedTypeDef

```python
# RecordsIngestedTypeDef definition

class RecordsIngestedTypeDef(TypedDict):
    Total: NotRequired[int],
    MemoryStore: NotRequired[int],
    MagneticStore: NotRequired[int],
```

## ReportS3ConfigurationTypeDef

```python
# ReportS3ConfigurationTypeDef definition

class ReportS3ConfigurationTypeDef(TypedDict):
    BucketName: str,
    ObjectKeyPrefix: NotRequired[str],
    EncryptionOption: NotRequired[S3EncryptionOptionType],  # (1)
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: S3EncryptionOptionType](./literals.md#s3encryptionoptiontype) 
## ResumeBatchLoadTaskRequestRequestTypeDef

```python
# ResumeBatchLoadTaskRequestRequestTypeDef definition

class ResumeBatchLoadTaskRequestRequestTypeDef(TypedDict):
    TaskId: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateDatabaseRequestRequestTypeDef

```python
# UpdateDatabaseRequestRequestTypeDef definition

class UpdateDatabaseRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    KmsKeyId: str,
```

## CreateBatchLoadTaskResponseTypeDef

```python
# CreateBatchLoadTaskResponseTypeDef definition

class CreateBatchLoadTaskResponseTypeDef(TypedDict):
    TaskId: str,
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
## ListBatchLoadTasksResponseTypeDef

```python
# ListBatchLoadTasksResponseTypeDef definition

class ListBatchLoadTasksResponseTypeDef(TypedDict):
    NextToken: str,
    BatchLoadTasks: List[BatchLoadTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchLoadTaskTypeDef](./type_defs.md#batchloadtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatabaseRequestRequestTypeDef

```python
# CreateDatabaseRequestRequestTypeDef definition

class CreateDatabaseRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDatabaseResponseTypeDef

```python
# CreateDatabaseResponseTypeDef definition

class CreateDatabaseResponseTypeDef(TypedDict):
    Database: DatabaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDatabaseResponseTypeDef

```python
# DescribeDatabaseResponseTypeDef definition

class DescribeDatabaseResponseTypeDef(TypedDict):
    Database: DatabaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatabasesResponseTypeDef

```python
# ListDatabasesResponseTypeDef definition

class ListDatabasesResponseTypeDef(TypedDict):
    Databases: List[DatabaseTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDatabaseResponseTypeDef

```python
# UpdateDatabaseResponseTypeDef definition

class UpdateDatabaseResponseTypeDef(TypedDict):
    Database: DatabaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceConfigurationTypeDef

```python
# DataSourceConfigurationTypeDef definition

class DataSourceConfigurationTypeDef(TypedDict):
    DataSourceS3Configuration: DataSourceS3ConfigurationTypeDef,  # (1)
    DataFormat: BatchLoadDataFormatType,  # (3)
    CsvConfiguration: NotRequired[CsvConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DataSourceS3ConfigurationTypeDef](./type_defs.md#datasources3configurationtypedef) 
2. See [:material-code-braces: CsvConfigurationTypeDef](./type_defs.md#csvconfigurationtypedef) 
3. See [:material-code-brackets: BatchLoadDataFormatType](./literals.md#batchloaddataformattype) 
## DescribeEndpointsResponseTypeDef

```python
# DescribeEndpointsResponseTypeDef definition

class DescribeEndpointsResponseTypeDef(TypedDict):
    Endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MagneticStoreRejectedDataLocationTypeDef

```python
# MagneticStoreRejectedDataLocationTypeDef definition

class MagneticStoreRejectedDataLocationTypeDef(TypedDict):
    S3Configuration: NotRequired[S3ConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: S3ConfigurationTypeDef](./type_defs.md#s3configurationtypedef) 
## RecordTypeDef

```python
# RecordTypeDef definition

class RecordTypeDef(TypedDict):
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
    MeasureName: NotRequired[str],
    MeasureValue: NotRequired[str],
    MeasureValueType: NotRequired[MeasureValueTypeType],  # (2)
    Time: NotRequired[str],
    TimeUnit: NotRequired[TimeUnitType],  # (3)
    Version: NotRequired[int],
    MeasureValues: NotRequired[Sequence[MeasureValueTypeDef]],  # (4)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-brackets: MeasureValueTypeType](./literals.md#measurevaluetypetype) 
3. See [:material-code-brackets: TimeUnitType](./literals.md#timeunittype) 
4. See [:material-code-braces: MeasureValueTypeDef](./type_defs.md#measurevaluetypedef) 
## MixedMeasureMappingTypeDef

```python
# MixedMeasureMappingTypeDef definition

class MixedMeasureMappingTypeDef(TypedDict):
    MeasureValueType: MeasureValueTypeType,  # (1)
    MeasureName: NotRequired[str],
    SourceColumn: NotRequired[str],
    TargetMeasureName: NotRequired[str],
    MultiMeasureAttributeMappings: NotRequired[Sequence[MultiMeasureAttributeMappingTypeDef]],  # (2)
```

1. See [:material-code-brackets: MeasureValueTypeType](./literals.md#measurevaluetypetype) 
2. See [:material-code-braces: MultiMeasureAttributeMappingTypeDef](./type_defs.md#multimeasureattributemappingtypedef) 
## MultiMeasureMappingsTypeDef

```python
# MultiMeasureMappingsTypeDef definition

class MultiMeasureMappingsTypeDef(TypedDict):
    MultiMeasureAttributeMappings: Sequence[MultiMeasureAttributeMappingTypeDef],  # (1)
    TargetMultiMeasureName: NotRequired[str],
```

1. See [:material-code-braces: MultiMeasureAttributeMappingTypeDef](./type_defs.md#multimeasureattributemappingtypedef) 
## SchemaTypeDef

```python
# SchemaTypeDef definition

class SchemaTypeDef(TypedDict):
    CompositePartitionKey: NotRequired[Sequence[PartitionKeyTypeDef]],  # (1)
```

1. See [:material-code-braces: PartitionKeyTypeDef](./type_defs.md#partitionkeytypedef) 
## WriteRecordsResponseTypeDef

```python
# WriteRecordsResponseTypeDef definition

class WriteRecordsResponseTypeDef(TypedDict):
    RecordsIngested: RecordsIngestedTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordsIngestedTypeDef](./type_defs.md#recordsingestedtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReportConfigurationTypeDef

```python
# ReportConfigurationTypeDef definition

class ReportConfigurationTypeDef(TypedDict):
    ReportS3Configuration: NotRequired[ReportS3ConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ReportS3ConfigurationTypeDef](./type_defs.md#reports3configurationtypedef) 
## MagneticStoreWritePropertiesTypeDef

```python
# MagneticStoreWritePropertiesTypeDef definition

class MagneticStoreWritePropertiesTypeDef(TypedDict):
    EnableMagneticStoreWrites: bool,
    MagneticStoreRejectedDataLocation: NotRequired[MagneticStoreRejectedDataLocationTypeDef],  # (1)
```

1. See [:material-code-braces: MagneticStoreRejectedDataLocationTypeDef](./type_defs.md#magneticstorerejecteddatalocationtypedef) 
## WriteRecordsRequestRequestTypeDef

```python
# WriteRecordsRequestRequestTypeDef definition

class WriteRecordsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    Records: Sequence[RecordTypeDef],  # (1)
    CommonAttributes: NotRequired[RecordTypeDef],  # (2)
```

1. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
2. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
## DataModelTypeDef

```python
# DataModelTypeDef definition

class DataModelTypeDef(TypedDict):
    DimensionMappings: Sequence[DimensionMappingTypeDef],  # (2)
    TimeColumn: NotRequired[str],
    TimeUnit: NotRequired[TimeUnitType],  # (1)
    MultiMeasureMappings: NotRequired[MultiMeasureMappingsTypeDef],  # (3)
    MixedMeasureMappings: NotRequired[Sequence[MixedMeasureMappingTypeDef]],  # (4)
    MeasureNameColumn: NotRequired[str],
```

1. See [:material-code-brackets: TimeUnitType](./literals.md#timeunittype) 
2. See [:material-code-braces: DimensionMappingTypeDef](./type_defs.md#dimensionmappingtypedef) 
3. See [:material-code-braces: MultiMeasureMappingsTypeDef](./type_defs.md#multimeasuremappingstypedef) 
4. See [:material-code-braces: MixedMeasureMappingTypeDef](./type_defs.md#mixedmeasuremappingtypedef) 
## CreateTableRequestRequestTypeDef

```python
# CreateTableRequestRequestTypeDef definition

class CreateTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    RetentionProperties: NotRequired[RetentionPropertiesTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    MagneticStoreWriteProperties: NotRequired[MagneticStoreWritePropertiesTypeDef],  # (3)
    Schema: NotRequired[SchemaTypeDef],  # (4)
```

1. See [:material-code-braces: RetentionPropertiesTypeDef](./type_defs.md#retentionpropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: MagneticStoreWritePropertiesTypeDef](./type_defs.md#magneticstorewritepropertiestypedef) 
4. See [:material-code-braces: SchemaTypeDef](./type_defs.md#schematypedef) 
## TableTypeDef

```python
# TableTypeDef definition

class TableTypeDef(TypedDict):
    Arn: NotRequired[str],
    TableName: NotRequired[str],
    DatabaseName: NotRequired[str],
    TableStatus: NotRequired[TableStatusType],  # (1)
    RetentionProperties: NotRequired[RetentionPropertiesTypeDef],  # (2)
    CreationTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    MagneticStoreWriteProperties: NotRequired[MagneticStoreWritePropertiesTypeDef],  # (3)
    Schema: NotRequired[SchemaTypeDef],  # (4)
```

1. See [:material-code-brackets: TableStatusType](./literals.md#tablestatustype) 
2. See [:material-code-braces: RetentionPropertiesTypeDef](./type_defs.md#retentionpropertiestypedef) 
3. See [:material-code-braces: MagneticStoreWritePropertiesTypeDef](./type_defs.md#magneticstorewritepropertiestypedef) 
4. See [:material-code-braces: SchemaTypeDef](./type_defs.md#schematypedef) 
## UpdateTableRequestRequestTypeDef

```python
# UpdateTableRequestRequestTypeDef definition

class UpdateTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    RetentionProperties: NotRequired[RetentionPropertiesTypeDef],  # (1)
    MagneticStoreWriteProperties: NotRequired[MagneticStoreWritePropertiesTypeDef],  # (2)
    Schema: NotRequired[SchemaTypeDef],  # (3)
```

1. See [:material-code-braces: RetentionPropertiesTypeDef](./type_defs.md#retentionpropertiestypedef) 
2. See [:material-code-braces: MagneticStoreWritePropertiesTypeDef](./type_defs.md#magneticstorewritepropertiestypedef) 
3. See [:material-code-braces: SchemaTypeDef](./type_defs.md#schematypedef) 
## DataModelConfigurationTypeDef

```python
# DataModelConfigurationTypeDef definition

class DataModelConfigurationTypeDef(TypedDict):
    DataModel: NotRequired[DataModelTypeDef],  # (1)
    DataModelS3Configuration: NotRequired[DataModelS3ConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DataModelTypeDef](./type_defs.md#datamodeltypedef) 
2. See [:material-code-braces: DataModelS3ConfigurationTypeDef](./type_defs.md#datamodels3configurationtypedef) 
## CreateTableResponseTypeDef

```python
# CreateTableResponseTypeDef definition

class CreateTableResponseTypeDef(TypedDict):
    Table: TableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTableResponseTypeDef

```python
# DescribeTableResponseTypeDef definition

class DescribeTableResponseTypeDef(TypedDict):
    Table: TableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTablesResponseTypeDef

```python
# ListTablesResponseTypeDef definition

class ListTablesResponseTypeDef(TypedDict):
    Tables: List[TableTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableResponseTypeDef

```python
# UpdateTableResponseTypeDef definition

class UpdateTableResponseTypeDef(TypedDict):
    Table: TableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchLoadTaskDescriptionTypeDef

```python
# BatchLoadTaskDescriptionTypeDef definition

class BatchLoadTaskDescriptionTypeDef(TypedDict):
    TaskId: NotRequired[str],
    ErrorMessage: NotRequired[str],
    DataSourceConfiguration: NotRequired[DataSourceConfigurationTypeDef],  # (1)
    ProgressReport: NotRequired[BatchLoadProgressReportTypeDef],  # (2)
    ReportConfiguration: NotRequired[ReportConfigurationTypeDef],  # (3)
    DataModelConfiguration: NotRequired[DataModelConfigurationTypeDef],  # (4)
    TargetDatabaseName: NotRequired[str],
    TargetTableName: NotRequired[str],
    TaskStatus: NotRequired[BatchLoadStatusType],  # (5)
    RecordVersion: NotRequired[int],
    CreationTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    ResumableUntil: NotRequired[datetime],
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-braces: BatchLoadProgressReportTypeDef](./type_defs.md#batchloadprogressreporttypedef) 
3. See [:material-code-braces: ReportConfigurationTypeDef](./type_defs.md#reportconfigurationtypedef) 
4. See [:material-code-braces: DataModelConfigurationTypeDef](./type_defs.md#datamodelconfigurationtypedef) 
5. See [:material-code-brackets: BatchLoadStatusType](./literals.md#batchloadstatustype) 
## CreateBatchLoadTaskRequestRequestTypeDef

```python
# CreateBatchLoadTaskRequestRequestTypeDef definition

class CreateBatchLoadTaskRequestRequestTypeDef(TypedDict):
    DataSourceConfiguration: DataSourceConfigurationTypeDef,  # (1)
    ReportConfiguration: ReportConfigurationTypeDef,  # (2)
    TargetDatabaseName: str,
    TargetTableName: str,
    ClientToken: NotRequired[str],
    DataModelConfiguration: NotRequired[DataModelConfigurationTypeDef],  # (3)
    RecordVersion: NotRequired[int],
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-braces: ReportConfigurationTypeDef](./type_defs.md#reportconfigurationtypedef) 
3. See [:material-code-braces: DataModelConfigurationTypeDef](./type_defs.md#datamodelconfigurationtypedef) 
## DescribeBatchLoadTaskResponseTypeDef

```python
# DescribeBatchLoadTaskResponseTypeDef definition

class DescribeBatchLoadTaskResponseTypeDef(TypedDict):
    BatchLoadTaskDescription: BatchLoadTaskDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchLoadTaskDescriptionTypeDef](./type_defs.md#batchloadtaskdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
