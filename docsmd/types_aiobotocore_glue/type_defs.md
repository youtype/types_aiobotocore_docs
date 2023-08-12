# Type definitions

> [Index](../README.md) > [Glue](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Glue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
    type annotations stubs module [types-aiobotocore-glue](https://pypi.org/project/types-aiobotocore-glue/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## NotificationPropertyTypeDef

```python
# NotificationPropertyTypeDef definition

class NotificationPropertyTypeDef(TypedDict):
    NotifyDelayAfter: NotRequired[int],
```

## AggregateOperationTypeDef

```python
# AggregateOperationTypeDef definition

class AggregateOperationTypeDef(TypedDict):
    Column: List[str],
    AggFunc: AggFunctionType,  # (1)
```

1. See [:material-code-brackets: AggFunctionType](./literals.md#aggfunctiontype) 
## AmazonRedshiftAdvancedOptionTypeDef

```python
# AmazonRedshiftAdvancedOptionTypeDef definition

class AmazonRedshiftAdvancedOptionTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## OptionTypeDef

```python
# OptionTypeDef definition

class OptionTypeDef(TypedDict):
    Value: NotRequired[str],
    Label: NotRequired[str],
    Description: NotRequired[str],
```

## ApplyMappingTypeDef

```python
# ApplyMappingTypeDef definition

class ApplyMappingTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Mapping: List[MappingTypeDef],  # (1)
```

1. See [:material-code-braces: MappingTypeDef](./type_defs.md#mappingtypedef) 
## AuditContextTypeDef

```python
# AuditContextTypeDef definition

class AuditContextTypeDef(TypedDict):
    AdditionalAuditContext: NotRequired[str],
    RequestedColumns: NotRequired[Sequence[str]],
    AllColumnsRequested: NotRequired[bool],
```

## PartitionValueListTypeDef

```python
# PartitionValueListTypeDef definition

class PartitionValueListTypeDef(TypedDict):
    Values: Sequence[str],
```

## BasicCatalogTargetTypeDef

```python
# BasicCatalogTargetTypeDef definition

class BasicCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
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

## BatchDeleteConnectionRequestRequestTypeDef

```python
# BatchDeleteConnectionRequestRequestTypeDef definition

class BatchDeleteConnectionRequestRequestTypeDef(TypedDict):
    ConnectionNameList: Sequence[str],
    CatalogId: NotRequired[str],
```

## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## BatchDeleteTableRequestRequestTypeDef

```python
# BatchDeleteTableRequestRequestTypeDef definition

class BatchDeleteTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TablesToDelete: Sequence[str],
    CatalogId: NotRequired[str],
    TransactionId: NotRequired[str],
```

## BatchDeleteTableVersionRequestRequestTypeDef

```python
# BatchDeleteTableVersionRequestRequestTypeDef definition

class BatchDeleteTableVersionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    VersionIds: Sequence[str],
    CatalogId: NotRequired[str],
```

## BatchGetBlueprintsRequestRequestTypeDef

```python
# BatchGetBlueprintsRequestRequestTypeDef definition

class BatchGetBlueprintsRequestRequestTypeDef(TypedDict):
    Names: Sequence[str],
    IncludeBlueprint: NotRequired[bool],
    IncludeParameterSpec: NotRequired[bool],
```

## BatchGetCrawlersRequestRequestTypeDef

```python
# BatchGetCrawlersRequestRequestTypeDef definition

class BatchGetCrawlersRequestRequestTypeDef(TypedDict):
    CrawlerNames: Sequence[str],
```

## BatchGetCustomEntityTypesRequestRequestTypeDef

```python
# BatchGetCustomEntityTypesRequestRequestTypeDef definition

class BatchGetCustomEntityTypesRequestRequestTypeDef(TypedDict):
    Names: Sequence[str],
```

## CustomEntityTypeTypeDef

```python
# CustomEntityTypeTypeDef definition

class CustomEntityTypeTypeDef(TypedDict):
    Name: str,
    RegexString: str,
    ContextWords: NotRequired[List[str]],
```

## BatchGetDataQualityResultRequestRequestTypeDef

```python
# BatchGetDataQualityResultRequestRequestTypeDef definition

class BatchGetDataQualityResultRequestRequestTypeDef(TypedDict):
    ResultIds: Sequence[str],
```

## BatchGetDevEndpointsRequestRequestTypeDef

```python
# BatchGetDevEndpointsRequestRequestTypeDef definition

class BatchGetDevEndpointsRequestRequestTypeDef(TypedDict):
    DevEndpointNames: Sequence[str],
```

## DevEndpointTypeDef

```python
# DevEndpointTypeDef definition

class DevEndpointTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    RoleArn: NotRequired[str],
    SecurityGroupIds: NotRequired[List[str]],
    SubnetId: NotRequired[str],
    YarnEndpointAddress: NotRequired[str],
    PrivateAddress: NotRequired[str],
    ZeppelinRemoteSparkInterpreterPort: NotRequired[int],
    PublicAddress: NotRequired[str],
    Status: NotRequired[str],
    WorkerType: NotRequired[WorkerTypeType],  # (1)
    GlueVersion: NotRequired[str],
    NumberOfWorkers: NotRequired[int],
    NumberOfNodes: NotRequired[int],
    AvailabilityZone: NotRequired[str],
    VpcId: NotRequired[str],
    ExtraPythonLibsS3Path: NotRequired[str],
    ExtraJarsS3Path: NotRequired[str],
    FailureReason: NotRequired[str],
    LastUpdateStatus: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    LastModifiedTimestamp: NotRequired[datetime],
    PublicKey: NotRequired[str],
    PublicKeys: NotRequired[List[str]],
    SecurityConfiguration: NotRequired[str],
    Arguments: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
## BatchGetJobsRequestRequestTypeDef

```python
# BatchGetJobsRequestRequestTypeDef definition

class BatchGetJobsRequestRequestTypeDef(TypedDict):
    JobNames: Sequence[str],
```

## BatchGetTriggersRequestRequestTypeDef

```python
# BatchGetTriggersRequestRequestTypeDef definition

class BatchGetTriggersRequestRequestTypeDef(TypedDict):
    TriggerNames: Sequence[str],
```

## BatchGetWorkflowsRequestRequestTypeDef

```python
# BatchGetWorkflowsRequestRequestTypeDef definition

class BatchGetWorkflowsRequestRequestTypeDef(TypedDict):
    Names: Sequence[str],
    IncludeGraph: NotRequired[bool],
```

## BatchStopJobRunRequestRequestTypeDef

```python
# BatchStopJobRunRequestRequestTypeDef definition

class BatchStopJobRunRequestRequestTypeDef(TypedDict):
    JobName: str,
    JobRunIds: Sequence[str],
```

## BatchStopJobRunSuccessfulSubmissionTypeDef

```python
# BatchStopJobRunSuccessfulSubmissionTypeDef definition

class BatchStopJobRunSuccessfulSubmissionTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
```

## BinaryColumnStatisticsDataTypeDef

```python
# BinaryColumnStatisticsDataTypeDef definition

class BinaryColumnStatisticsDataTypeDef(TypedDict):
    MaximumLength: int,
    AverageLength: float,
    NumberOfNulls: int,
```

## BlueprintDetailsTypeDef

```python
# BlueprintDetailsTypeDef definition

class BlueprintDetailsTypeDef(TypedDict):
    BlueprintName: NotRequired[str],
    RunId: NotRequired[str],
```

## BlueprintRunTypeDef

```python
# BlueprintRunTypeDef definition

class BlueprintRunTypeDef(TypedDict):
    BlueprintName: NotRequired[str],
    RunId: NotRequired[str],
    WorkflowName: NotRequired[str],
    State: NotRequired[BlueprintRunStateType],  # (1)
    StartedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    ErrorMessage: NotRequired[str],
    RollbackErrorMessage: NotRequired[str],
    Parameters: NotRequired[str],
    RoleArn: NotRequired[str],
```

1. See [:material-code-brackets: BlueprintRunStateType](./literals.md#blueprintrunstatetype) 
## LastActiveDefinitionTypeDef

```python
# LastActiveDefinitionTypeDef definition

class LastActiveDefinitionTypeDef(TypedDict):
    Description: NotRequired[str],
    LastModifiedOn: NotRequired[datetime],
    ParameterSpec: NotRequired[str],
    BlueprintLocation: NotRequired[str],
    BlueprintServiceLocation: NotRequired[str],
```

## BooleanColumnStatisticsDataTypeDef

```python
# BooleanColumnStatisticsDataTypeDef definition

class BooleanColumnStatisticsDataTypeDef(TypedDict):
    NumberOfTrues: int,
    NumberOfFalses: int,
    NumberOfNulls: int,
```

## CancelDataQualityRuleRecommendationRunRequestRequestTypeDef

```python
# CancelDataQualityRuleRecommendationRunRequestRequestTypeDef definition

class CancelDataQualityRuleRecommendationRunRequestRequestTypeDef(TypedDict):
    RunId: str,
```

## CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef

```python
# CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef definition

class CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef(TypedDict):
    RunId: str,
```

## CancelMLTaskRunRequestRequestTypeDef

```python
# CancelMLTaskRunRequestRequestTypeDef definition

class CancelMLTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
    TaskRunId: str,
```

## CancelStatementRequestRequestTypeDef

```python
# CancelStatementRequestRequestTypeDef definition

class CancelStatementRequestRequestTypeDef(TypedDict):
    SessionId: str,
    Id: int,
    RequestOrigin: NotRequired[str],
```

## CatalogEntryTypeDef

```python
# CatalogEntryTypeDef definition

class CatalogEntryTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
```

## CatalogImportStatusTypeDef

```python
# CatalogImportStatusTypeDef definition

class CatalogImportStatusTypeDef(TypedDict):
    ImportCompleted: NotRequired[bool],
    ImportTime: NotRequired[datetime],
    ImportedBy: NotRequired[str],
```

## KafkaStreamingSourceOptionsTypeDef

```python
# KafkaStreamingSourceOptionsTypeDef definition

class KafkaStreamingSourceOptionsTypeDef(TypedDict):
    BootstrapServers: NotRequired[str],
    SecurityProtocol: NotRequired[str],
    ConnectionName: NotRequired[str],
    TopicName: NotRequired[str],
    Assign: NotRequired[str],
    SubscribePattern: NotRequired[str],
    Classification: NotRequired[str],
    Delimiter: NotRequired[str],
    StartingOffsets: NotRequired[str],
    EndingOffsets: NotRequired[str],
    PollTimeoutMs: NotRequired[int],
    NumRetries: NotRequired[int],
    RetryIntervalMs: NotRequired[int],
    MaxOffsetsPerTrigger: NotRequired[int],
    MinPartitions: NotRequired[int],
    IncludeHeaders: NotRequired[bool],
    AddRecordTimestamp: NotRequired[str],
    EmitConsumerLagMetrics: NotRequired[str],
    StartingTimestamp: NotRequired[datetime],
```

## StreamingDataPreviewOptionsTypeDef

```python
# StreamingDataPreviewOptionsTypeDef definition

class StreamingDataPreviewOptionsTypeDef(TypedDict):
    PollingTime: NotRequired[int],
    RecordPollingLimit: NotRequired[int],
```

## KinesisStreamingSourceOptionsTypeDef

```python
# KinesisStreamingSourceOptionsTypeDef definition

class KinesisStreamingSourceOptionsTypeDef(TypedDict):
    EndpointUrl: NotRequired[str],
    StreamName: NotRequired[str],
    Classification: NotRequired[str],
    Delimiter: NotRequired[str],
    StartingPosition: NotRequired[StartingPositionType],  # (1)
    MaxFetchTimeInMs: NotRequired[int],
    MaxFetchRecordsPerShard: NotRequired[int],
    MaxRecordPerRead: NotRequired[int],
    AddIdleTimeBetweenReads: NotRequired[bool],
    IdleTimeBetweenReadsInMs: NotRequired[int],
    DescribeShardInterval: NotRequired[int],
    NumRetries: NotRequired[int],
    RetryIntervalMs: NotRequired[int],
    MaxRetryIntervalMs: NotRequired[int],
    AvoidEmptyBatches: NotRequired[bool],
    StreamArn: NotRequired[str],
    RoleArn: NotRequired[str],
    RoleSessionName: NotRequired[str],
    AddRecordTimestamp: NotRequired[str],
    EmitConsumerLagMetrics: NotRequired[str],
    StartingTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: StartingPositionType](./literals.md#startingpositiontype) 
## CatalogSchemaChangePolicyTypeDef

```python
# CatalogSchemaChangePolicyTypeDef definition

class CatalogSchemaChangePolicyTypeDef(TypedDict):
    EnableUpdateCatalog: NotRequired[bool],
    UpdateBehavior: NotRequired[UpdateCatalogBehaviorType],  # (1)
```

1. See [:material-code-brackets: UpdateCatalogBehaviorType](./literals.md#updatecatalogbehaviortype) 
## CatalogSourceTypeDef

```python
# CatalogSourceTypeDef definition

class CatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## CatalogTargetTypeDef

```python
# CatalogTargetTypeDef definition

class CatalogTargetTypeDef(TypedDict):
    DatabaseName: str,
    Tables: List[str],
    ConnectionName: NotRequired[str],
    EventQueueArn: NotRequired[str],
    DlqEventQueueArn: NotRequired[str],
```

## CheckSchemaVersionValidityInputRequestTypeDef

```python
# CheckSchemaVersionValidityInputRequestTypeDef definition

class CheckSchemaVersionValidityInputRequestTypeDef(TypedDict):
    DataFormat: DataFormatType,  # (1)
    SchemaDefinition: str,
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
## CsvClassifierTypeDef

```python
# CsvClassifierTypeDef definition

class CsvClassifierTypeDef(TypedDict):
    Name: str,
    CreationTime: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    Version: NotRequired[int],
    Delimiter: NotRequired[str],
    QuoteSymbol: NotRequired[str],
    ContainsHeader: NotRequired[CsvHeaderOptionType],  # (1)
    Header: NotRequired[List[str]],
    DisableValueTrimming: NotRequired[bool],
    AllowSingleColumn: NotRequired[bool],
    CustomDatatypeConfigured: NotRequired[bool],
    CustomDatatypes: NotRequired[List[str]],
```

1. See [:material-code-brackets: CsvHeaderOptionType](./literals.md#csvheaderoptiontype) 
## GrokClassifierTypeDef

```python
# GrokClassifierTypeDef definition

class GrokClassifierTypeDef(TypedDict):
    Name: str,
    Classification: str,
    GrokPattern: str,
    CreationTime: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    Version: NotRequired[int],
    CustomPatterns: NotRequired[str],
```

## JsonClassifierTypeDef

```python
# JsonClassifierTypeDef definition

class JsonClassifierTypeDef(TypedDict):
    Name: str,
    JsonPath: str,
    CreationTime: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    Version: NotRequired[int],
```

## XMLClassifierTypeDef

```python
# XMLClassifierTypeDef definition

class XMLClassifierTypeDef(TypedDict):
    Name: str,
    Classification: str,
    CreationTime: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    Version: NotRequired[int],
    RowTag: NotRequired[str],
```

## CloudWatchEncryptionTypeDef

```python
# CloudWatchEncryptionTypeDef definition

class CloudWatchEncryptionTypeDef(TypedDict):
    CloudWatchEncryptionMode: NotRequired[CloudWatchEncryptionModeType],  # (1)
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: CloudWatchEncryptionModeType](./literals.md#cloudwatchencryptionmodetype) 
## DirectJDBCSourceTypeDef

```python
# DirectJDBCSourceTypeDef definition

class DirectJDBCSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    ConnectionName: str,
    ConnectionType: JDBCConnectionTypeType,  # (1)
    RedshiftTmpDir: NotRequired[str],
```

1. See [:material-code-brackets: JDBCConnectionTypeType](./literals.md#jdbcconnectiontypetype) 
## DropDuplicatesTypeDef

```python
# DropDuplicatesTypeDef definition

class DropDuplicatesTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Columns: NotRequired[List[List[str]]],
```

## DropFieldsTypeDef

```python
# DropFieldsTypeDef definition

class DropFieldsTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Paths: List[List[str]],
```

## DynamoDBCatalogSourceTypeDef

```python
# DynamoDBCatalogSourceTypeDef definition

class DynamoDBCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## FillMissingValuesTypeDef

```python
# FillMissingValuesTypeDef definition

class FillMissingValuesTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    ImputedPath: str,
    FilledPath: NotRequired[str],
```

## MergeTypeDef

```python
# MergeTypeDef definition

class MergeTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Source: str,
    PrimaryKeys: List[List[str]],
```

## MicrosoftSQLServerCatalogSourceTypeDef

```python
# MicrosoftSQLServerCatalogSourceTypeDef definition

class MicrosoftSQLServerCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## MicrosoftSQLServerCatalogTargetTypeDef

```python
# MicrosoftSQLServerCatalogTargetTypeDef definition

class MicrosoftSQLServerCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
```

## MySQLCatalogSourceTypeDef

```python
# MySQLCatalogSourceTypeDef definition

class MySQLCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## MySQLCatalogTargetTypeDef

```python
# MySQLCatalogTargetTypeDef definition

class MySQLCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
```

## OracleSQLCatalogSourceTypeDef

```python
# OracleSQLCatalogSourceTypeDef definition

class OracleSQLCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## OracleSQLCatalogTargetTypeDef

```python
# OracleSQLCatalogTargetTypeDef definition

class OracleSQLCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
```

## PIIDetectionTypeDef

```python
# PIIDetectionTypeDef definition

class PIIDetectionTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    PiiType: PiiTypeType,  # (1)
    EntityTypesToDetect: List[str],
    OutputColumnName: NotRequired[str],
    SampleFraction: NotRequired[float],
    ThresholdFraction: NotRequired[float],
    MaskValue: NotRequired[str],
```

1. See [:material-code-brackets: PiiTypeType](./literals.md#piitypetype) 
## PostgreSQLCatalogSourceTypeDef

```python
# PostgreSQLCatalogSourceTypeDef definition

class PostgreSQLCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## PostgreSQLCatalogTargetTypeDef

```python
# PostgreSQLCatalogTargetTypeDef definition

class PostgreSQLCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
```

## RedshiftSourceTypeDef

```python
# RedshiftSourceTypeDef definition

class RedshiftSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    RedshiftTmpDir: NotRequired[str],
    TmpDirIAMRole: NotRequired[str],
```

## RelationalCatalogSourceTypeDef

```python
# RelationalCatalogSourceTypeDef definition

class RelationalCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## RenameFieldTypeDef

```python
# RenameFieldTypeDef definition

class RenameFieldTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    SourcePath: List[str],
    TargetPath: List[str],
```

## SelectFieldsTypeDef

```python
# SelectFieldsTypeDef definition

class SelectFieldsTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Paths: List[List[str]],
```

## SelectFromCollectionTypeDef

```python
# SelectFromCollectionTypeDef definition

class SelectFromCollectionTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Index: int,
```

## SpigotTypeDef

```python
# SpigotTypeDef definition

class SpigotTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Path: str,
    Topk: NotRequired[int],
    Prob: NotRequired[float],
```

## SplitFieldsTypeDef

```python
# SplitFieldsTypeDef definition

class SplitFieldsTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Paths: List[List[str]],
```

## UnionTypeDef

```python
# UnionTypeDef definition

class UnionTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    UnionType: UnionTypeType,  # (1)
```

1. See [:material-code-brackets: UnionTypeType](./literals.md#uniontypetype) 
## CodeGenEdgeTypeDef

```python
# CodeGenEdgeTypeDef definition

class CodeGenEdgeTypeDef(TypedDict):
    Source: str,
    Target: str,
    TargetParameter: NotRequired[str],
```

## CodeGenNodeArgTypeDef

```python
# CodeGenNodeArgTypeDef definition

class CodeGenNodeArgTypeDef(TypedDict):
    Name: str,
    Value: str,
    Param: NotRequired[bool],
```

## ColumnImportanceTypeDef

```python
# ColumnImportanceTypeDef definition

class ColumnImportanceTypeDef(TypedDict):
    ColumnName: NotRequired[str],
    Importance: NotRequired[float],
```

## ColumnRowFilterTypeDef

```python
# ColumnRowFilterTypeDef definition

class ColumnRowFilterTypeDef(TypedDict):
    ColumnName: NotRequired[str],
    RowFilterExpression: NotRequired[str],
```

## DateColumnStatisticsDataTypeDef

```python
# DateColumnStatisticsDataTypeDef definition

class DateColumnStatisticsDataTypeDef(TypedDict):
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
    MinimumValue: NotRequired[datetime],
    MaximumValue: NotRequired[datetime],
```

## DoubleColumnStatisticsDataTypeDef

```python
# DoubleColumnStatisticsDataTypeDef definition

class DoubleColumnStatisticsDataTypeDef(TypedDict):
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
    MinimumValue: NotRequired[float],
    MaximumValue: NotRequired[float],
```

## LongColumnStatisticsDataTypeDef

```python
# LongColumnStatisticsDataTypeDef definition

class LongColumnStatisticsDataTypeDef(TypedDict):
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
    MinimumValue: NotRequired[int],
    MaximumValue: NotRequired[int],
```

## StringColumnStatisticsDataTypeDef

```python
# StringColumnStatisticsDataTypeDef definition

class StringColumnStatisticsDataTypeDef(TypedDict):
    MaximumLength: int,
    AverageLength: float,
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
```

## ColumnTypeDef

```python
# ColumnTypeDef definition

class ColumnTypeDef(TypedDict):
    Name: str,
    Type: NotRequired[str],
    Comment: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
```

## ConditionTypeDef

```python
# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    LogicalOperator: NotRequired[LogicalOperatorType],  # (1)
    JobName: NotRequired[str],
    State: NotRequired[JobRunStateType],  # (2)
    CrawlerName: NotRequired[str],
    CrawlState: NotRequired[CrawlStateType],  # (3)
```

1. See [:material-code-brackets: LogicalOperatorType](./literals.md#logicaloperatortype) 
2. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
3. See [:material-code-brackets: CrawlStateType](./literals.md#crawlstatetype) 
## ConfusionMatrixTypeDef

```python
# ConfusionMatrixTypeDef definition

class ConfusionMatrixTypeDef(TypedDict):
    NumTruePositives: NotRequired[int],
    NumFalsePositives: NotRequired[int],
    NumTrueNegatives: NotRequired[int],
    NumFalseNegatives: NotRequired[int],
```

## PhysicalConnectionRequirementsTypeDef

```python
# PhysicalConnectionRequirementsTypeDef definition

class PhysicalConnectionRequirementsTypeDef(TypedDict):
    SubnetId: NotRequired[str],
    SecurityGroupIdList: NotRequired[Sequence[str]],
    AvailabilityZone: NotRequired[str],
```

## ConnectionPasswordEncryptionTypeDef

```python
# ConnectionPasswordEncryptionTypeDef definition

class ConnectionPasswordEncryptionTypeDef(TypedDict):
    ReturnConnectionPasswordEncrypted: bool,
    AwsKmsKeyId: NotRequired[str],
```

## ConnectionsListTypeDef

```python
# ConnectionsListTypeDef definition

class ConnectionsListTypeDef(TypedDict):
    Connections: NotRequired[List[str]],
```

## CrawlTypeDef

```python
# CrawlTypeDef definition

class CrawlTypeDef(TypedDict):
    State: NotRequired[CrawlStateType],  # (1)
    StartedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    ErrorMessage: NotRequired[str],
    LogGroup: NotRequired[str],
    LogStream: NotRequired[str],
```

1. See [:material-code-brackets: CrawlStateType](./literals.md#crawlstatetype) 
## CrawlerHistoryTypeDef

```python
# CrawlerHistoryTypeDef definition

class CrawlerHistoryTypeDef(TypedDict):
    CrawlId: NotRequired[str],
    State: NotRequired[CrawlerHistoryStateType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Summary: NotRequired[str],
    ErrorMessage: NotRequired[str],
    LogGroup: NotRequired[str],
    LogStream: NotRequired[str],
    MessagePrefix: NotRequired[str],
    DPUHour: NotRequired[float],
```

1. See [:material-code-brackets: CrawlerHistoryStateType](./literals.md#crawlerhistorystatetype) 
## CrawlerMetricsTypeDef

```python
# CrawlerMetricsTypeDef definition

class CrawlerMetricsTypeDef(TypedDict):
    CrawlerName: NotRequired[str],
    TimeLeftSeconds: NotRequired[float],
    StillEstimating: NotRequired[bool],
    LastRuntimeSeconds: NotRequired[float],
    MedianRuntimeSeconds: NotRequired[float],
    TablesCreated: NotRequired[int],
    TablesUpdated: NotRequired[int],
    TablesDeleted: NotRequired[int],
```

## DeltaTargetTypeDef

```python
# DeltaTargetTypeDef definition

class DeltaTargetTypeDef(TypedDict):
    DeltaTables: NotRequired[List[str]],
    ConnectionName: NotRequired[str],
    WriteManifest: NotRequired[bool],
    CreateNativeDeltaTable: NotRequired[bool],
```

## DynamoDBTargetTypeDef

```python
# DynamoDBTargetTypeDef definition

class DynamoDBTargetTypeDef(TypedDict):
    Path: NotRequired[str],
    scanAll: NotRequired[bool],
    scanRate: NotRequired[float],
```

## HudiTargetTypeDef

```python
# HudiTargetTypeDef definition

class HudiTargetTypeDef(TypedDict):
    Paths: NotRequired[List[str]],
    ConnectionName: NotRequired[str],
    Exclusions: NotRequired[List[str]],
    MaximumTraversalDepth: NotRequired[int],
```

## IcebergTargetTypeDef

```python
# IcebergTargetTypeDef definition

class IcebergTargetTypeDef(TypedDict):
    Paths: NotRequired[List[str]],
    ConnectionName: NotRequired[str],
    Exclusions: NotRequired[List[str]],
    MaximumTraversalDepth: NotRequired[int],
```

## JdbcTargetTypeDef

```python
# JdbcTargetTypeDef definition

class JdbcTargetTypeDef(TypedDict):
    ConnectionName: NotRequired[str],
    Path: NotRequired[str],
    Exclusions: NotRequired[List[str]],
    EnableAdditionalMetadata: NotRequired[List[JdbcMetadataEntryType]],  # (1)
```

1. See [:material-code-brackets: JdbcMetadataEntryType](./literals.md#jdbcmetadataentrytype) 
## MongoDBTargetTypeDef

```python
# MongoDBTargetTypeDef definition

class MongoDBTargetTypeDef(TypedDict):
    ConnectionName: NotRequired[str],
    Path: NotRequired[str],
    ScanAll: NotRequired[bool],
```

## S3TargetTypeDef

```python
# S3TargetTypeDef definition

class S3TargetTypeDef(TypedDict):
    Path: NotRequired[str],
    Exclusions: NotRequired[List[str]],
    ConnectionName: NotRequired[str],
    SampleSize: NotRequired[int],
    EventQueueArn: NotRequired[str],
    DlqEventQueueArn: NotRequired[str],
```

## LakeFormationConfigurationTypeDef

```python
# LakeFormationConfigurationTypeDef definition

class LakeFormationConfigurationTypeDef(TypedDict):
    UseLakeFormationCredentials: NotRequired[bool],
    AccountId: NotRequired[str],
```

## LastCrawlInfoTypeDef

```python
# LastCrawlInfoTypeDef definition

class LastCrawlInfoTypeDef(TypedDict):
    Status: NotRequired[LastCrawlStatusType],  # (1)
    ErrorMessage: NotRequired[str],
    LogGroup: NotRequired[str],
    LogStream: NotRequired[str],
    MessagePrefix: NotRequired[str],
    StartTime: NotRequired[datetime],
```

1. See [:material-code-brackets: LastCrawlStatusType](./literals.md#lastcrawlstatustype) 
## LineageConfigurationTypeDef

```python
# LineageConfigurationTypeDef definition

class LineageConfigurationTypeDef(TypedDict):
    CrawlerLineageSettings: NotRequired[CrawlerLineageSettingsType],  # (1)
```

1. See [:material-code-brackets: CrawlerLineageSettingsType](./literals.md#crawlerlineagesettingstype) 
## RecrawlPolicyTypeDef

```python
# RecrawlPolicyTypeDef definition

class RecrawlPolicyTypeDef(TypedDict):
    RecrawlBehavior: NotRequired[RecrawlBehaviorType],  # (1)
```

1. See [:material-code-brackets: RecrawlBehaviorType](./literals.md#recrawlbehaviortype) 
## ScheduleTypeDef

```python
# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    ScheduleExpression: NotRequired[str],
    State: NotRequired[ScheduleStateType],  # (1)
```

1. See [:material-code-brackets: ScheduleStateType](./literals.md#schedulestatetype) 
## SchemaChangePolicyTypeDef

```python
# SchemaChangePolicyTypeDef definition

class SchemaChangePolicyTypeDef(TypedDict):
    UpdateBehavior: NotRequired[UpdateBehaviorType],  # (1)
    DeleteBehavior: NotRequired[DeleteBehaviorType],  # (2)
```

1. See [:material-code-brackets: UpdateBehaviorType](./literals.md#updatebehaviortype) 
2. See [:material-code-brackets: DeleteBehaviorType](./literals.md#deletebehaviortype) 
## CrawlsFilterTypeDef

```python
# CrawlsFilterTypeDef definition

class CrawlsFilterTypeDef(TypedDict):
    FieldName: NotRequired[FieldNameType],  # (1)
    FilterOperator: NotRequired[FilterOperatorType],  # (2)
    FieldValue: NotRequired[str],
```

1. See [:material-code-brackets: FieldNameType](./literals.md#fieldnametype) 
2. See [:material-code-brackets: FilterOperatorType](./literals.md#filteroperatortype) 
## CreateBlueprintRequestRequestTypeDef

```python
# CreateBlueprintRequestRequestTypeDef definition

class CreateBlueprintRequestRequestTypeDef(TypedDict):
    Name: str,
    BlueprintLocation: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## CreateCsvClassifierRequestTypeDef

```python
# CreateCsvClassifierRequestTypeDef definition

class CreateCsvClassifierRequestTypeDef(TypedDict):
    Name: str,
    Delimiter: NotRequired[str],
    QuoteSymbol: NotRequired[str],
    ContainsHeader: NotRequired[CsvHeaderOptionType],  # (1)
    Header: NotRequired[Sequence[str]],
    DisableValueTrimming: NotRequired[bool],
    AllowSingleColumn: NotRequired[bool],
    CustomDatatypeConfigured: NotRequired[bool],
    CustomDatatypes: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: CsvHeaderOptionType](./literals.md#csvheaderoptiontype) 
## CreateGrokClassifierRequestTypeDef

```python
# CreateGrokClassifierRequestTypeDef definition

class CreateGrokClassifierRequestTypeDef(TypedDict):
    Classification: str,
    Name: str,
    GrokPattern: str,
    CustomPatterns: NotRequired[str],
```

## CreateJsonClassifierRequestTypeDef

```python
# CreateJsonClassifierRequestTypeDef definition

class CreateJsonClassifierRequestTypeDef(TypedDict):
    Name: str,
    JsonPath: str,
```

## CreateXMLClassifierRequestTypeDef

```python
# CreateXMLClassifierRequestTypeDef definition

class CreateXMLClassifierRequestTypeDef(TypedDict):
    Classification: str,
    Name: str,
    RowTag: NotRequired[str],
```

## CreateCustomEntityTypeRequestRequestTypeDef

```python
# CreateCustomEntityTypeRequestRequestTypeDef definition

class CreateCustomEntityTypeRequestRequestTypeDef(TypedDict):
    Name: str,
    RegexString: str,
    ContextWords: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

## DataQualityTargetTableTypeDef

```python
# DataQualityTargetTableTypeDef definition

class DataQualityTargetTableTypeDef(TypedDict):
    TableName: str,
    DatabaseName: str,
    CatalogId: NotRequired[str],
```

## CreateDevEndpointRequestRequestTypeDef

```python
# CreateDevEndpointRequestRequestTypeDef definition

class CreateDevEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
    RoleArn: str,
    SecurityGroupIds: NotRequired[Sequence[str]],
    SubnetId: NotRequired[str],
    PublicKey: NotRequired[str],
    PublicKeys: NotRequired[Sequence[str]],
    NumberOfNodes: NotRequired[int],
    WorkerType: NotRequired[WorkerTypeType],  # (1)
    GlueVersion: NotRequired[str],
    NumberOfWorkers: NotRequired[int],
    ExtraPythonLibsS3Path: NotRequired[str],
    ExtraJarsS3Path: NotRequired[str],
    SecurityConfiguration: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    Arguments: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
## ExecutionPropertyTypeDef

```python
# ExecutionPropertyTypeDef definition

class ExecutionPropertyTypeDef(TypedDict):
    MaxConcurrentRuns: NotRequired[int],
```

## JobCommandTypeDef

```python
# JobCommandTypeDef definition

class JobCommandTypeDef(TypedDict):
    Name: NotRequired[str],
    ScriptLocation: NotRequired[str],
    PythonVersion: NotRequired[str],
    Runtime: NotRequired[str],
```

## SourceControlDetailsTypeDef

```python
# SourceControlDetailsTypeDef definition

class SourceControlDetailsTypeDef(TypedDict):
    Provider: NotRequired[SourceControlProviderType],  # (1)
    Repository: NotRequired[str],
    Owner: NotRequired[str],
    Branch: NotRequired[str],
    Folder: NotRequired[str],
    LastCommitId: NotRequired[str],
    AuthStrategy: NotRequired[SourceControlAuthStrategyType],  # (2)
    AuthToken: NotRequired[str],
```

1. See [:material-code-brackets: SourceControlProviderType](./literals.md#sourcecontrolprovidertype) 
2. See [:material-code-brackets: SourceControlAuthStrategyType](./literals.md#sourcecontrolauthstrategytype) 
## GlueTableTypeDef

```python
# GlueTableTypeDef definition

class GlueTableTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    ConnectionName: NotRequired[str],
    AdditionalOptions: NotRequired[Dict[str, str]],
```

## PartitionIndexTypeDef

```python
# PartitionIndexTypeDef definition

class PartitionIndexTypeDef(TypedDict):
    Keys: Sequence[str],
    IndexName: str,
```

## CreateRegistryInputRequestTypeDef

```python
# CreateRegistryInputRequestTypeDef definition

class CreateRegistryInputRequestTypeDef(TypedDict):
    RegistryName: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## RegistryIdTypeDef

```python
# RegistryIdTypeDef definition

class RegistryIdTypeDef(TypedDict):
    RegistryName: NotRequired[str],
    RegistryArn: NotRequired[str],
```

## SessionCommandTypeDef

```python
# SessionCommandTypeDef definition

class SessionCommandTypeDef(TypedDict):
    Name: NotRequired[str],
    PythonVersion: NotRequired[str],
```

## EventBatchingConditionTypeDef

```python
# EventBatchingConditionTypeDef definition

class EventBatchingConditionTypeDef(TypedDict):
    BatchSize: int,
    BatchWindow: NotRequired[int],
```

## CreateWorkflowRequestRequestTypeDef

```python
# CreateWorkflowRequestRequestTypeDef definition

class CreateWorkflowRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    DefaultRunProperties: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Mapping[str, str]],
    MaxConcurrentRuns: NotRequired[int],
```

## DQResultsPublishingOptionsTypeDef

```python
# DQResultsPublishingOptionsTypeDef definition

class DQResultsPublishingOptionsTypeDef(TypedDict):
    EvaluationContext: NotRequired[str],
    ResultsS3Prefix: NotRequired[str],
    CloudWatchMetricsEnabled: NotRequired[bool],
    ResultsPublishingEnabled: NotRequired[bool],
```

## DQStopJobOnFailureOptionsTypeDef

```python
# DQStopJobOnFailureOptionsTypeDef definition

class DQStopJobOnFailureOptionsTypeDef(TypedDict):
    StopJobOnFailureTiming: NotRequired[DQStopJobOnFailureTimingType],  # (1)
```

1. See [:material-code-brackets: DQStopJobOnFailureTimingType](./literals.md#dqstopjobonfailuretimingtype) 
## EncryptionAtRestTypeDef

```python
# EncryptionAtRestTypeDef definition

class EncryptionAtRestTypeDef(TypedDict):
    CatalogEncryptionMode: CatalogEncryptionModeType,  # (1)
    SseAwsKmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: CatalogEncryptionModeType](./literals.md#catalogencryptionmodetype) 
## DataLakePrincipalTypeDef

```python
# DataLakePrincipalTypeDef definition

class DataLakePrincipalTypeDef(TypedDict):
    DataLakePrincipalIdentifier: NotRequired[str],
```

## DataQualityEvaluationRunAdditionalRunOptionsTypeDef

```python
# DataQualityEvaluationRunAdditionalRunOptionsTypeDef definition

class DataQualityEvaluationRunAdditionalRunOptionsTypeDef(TypedDict):
    CloudWatchMetricsEnabled: NotRequired[bool],
    ResultsS3Prefix: NotRequired[str],
```

## DataQualityRuleResultTypeDef

```python
# DataQualityRuleResultTypeDef definition

class DataQualityRuleResultTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    EvaluationMessage: NotRequired[str],
    Result: NotRequired[DataQualityRuleResultStatusType],  # (1)
    EvaluatedMetrics: NotRequired[Dict[str, float]],
```

1. See [:material-code-brackets: DataQualityRuleResultStatusType](./literals.md#dataqualityruleresultstatustype) 
## DatabaseIdentifierTypeDef

```python
# DatabaseIdentifierTypeDef definition

class DatabaseIdentifierTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    DatabaseName: NotRequired[str],
    Region: NotRequired[str],
```

## FederatedDatabaseTypeDef

```python
# FederatedDatabaseTypeDef definition

class FederatedDatabaseTypeDef(TypedDict):
    Identifier: NotRequired[str],
    ConnectionName: NotRequired[str],
```

## DatatypeTypeDef

```python
# DatatypeTypeDef definition

class DatatypeTypeDef(TypedDict):
    Id: str,
    Label: str,
```

## DecimalNumberTypeDef

```python
# DecimalNumberTypeDef definition

class DecimalNumberTypeDef(TypedDict):
    UnscaledValue: bytes,
    Scale: int,
```

## DeleteBlueprintRequestRequestTypeDef

```python
# DeleteBlueprintRequestRequestTypeDef definition

class DeleteBlueprintRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteClassifierRequestRequestTypeDef

```python
# DeleteClassifierRequestRequestTypeDef definition

class DeleteClassifierRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteColumnStatisticsForPartitionRequestRequestTypeDef

```python
# DeleteColumnStatisticsForPartitionRequestRequestTypeDef definition

class DeleteColumnStatisticsForPartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    ColumnName: str,
    CatalogId: NotRequired[str],
```

## DeleteColumnStatisticsForTableRequestRequestTypeDef

```python
# DeleteColumnStatisticsForTableRequestRequestTypeDef definition

class DeleteColumnStatisticsForTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    ColumnName: str,
    CatalogId: NotRequired[str],
```

## DeleteConnectionRequestRequestTypeDef

```python
# DeleteConnectionRequestRequestTypeDef definition

class DeleteConnectionRequestRequestTypeDef(TypedDict):
    ConnectionName: str,
    CatalogId: NotRequired[str],
```

## DeleteCrawlerRequestRequestTypeDef

```python
# DeleteCrawlerRequestRequestTypeDef definition

class DeleteCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteCustomEntityTypeRequestRequestTypeDef

```python
# DeleteCustomEntityTypeRequestRequestTypeDef definition

class DeleteCustomEntityTypeRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteDataQualityRulesetRequestRequestTypeDef

```python
# DeleteDataQualityRulesetRequestRequestTypeDef definition

class DeleteDataQualityRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteDatabaseRequestRequestTypeDef

```python
# DeleteDatabaseRequestRequestTypeDef definition

class DeleteDatabaseRequestRequestTypeDef(TypedDict):
    Name: str,
    CatalogId: NotRequired[str],
```

## DeleteDevEndpointRequestRequestTypeDef

```python
# DeleteDevEndpointRequestRequestTypeDef definition

class DeleteDevEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
```

## DeleteJobRequestRequestTypeDef

```python
# DeleteJobRequestRequestTypeDef definition

class DeleteJobRequestRequestTypeDef(TypedDict):
    JobName: str,
```

## DeleteMLTransformRequestRequestTypeDef

```python
# DeleteMLTransformRequestRequestTypeDef definition

class DeleteMLTransformRequestRequestTypeDef(TypedDict):
    TransformId: str,
```

## DeletePartitionIndexRequestRequestTypeDef

```python
# DeletePartitionIndexRequestRequestTypeDef definition

class DeletePartitionIndexRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    IndexName: str,
    CatalogId: NotRequired[str],
```

## DeletePartitionRequestRequestTypeDef

```python
# DeletePartitionRequestRequestTypeDef definition

class DeletePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    CatalogId: NotRequired[str],
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    PolicyHashCondition: NotRequired[str],
    ResourceArn: NotRequired[str],
```

## SchemaIdTypeDef

```python
# SchemaIdTypeDef definition

class SchemaIdTypeDef(TypedDict):
    SchemaArn: NotRequired[str],
    SchemaName: NotRequired[str],
    RegistryName: NotRequired[str],
```

## DeleteSecurityConfigurationRequestRequestTypeDef

```python
# DeleteSecurityConfigurationRequestRequestTypeDef definition

class DeleteSecurityConfigurationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteSessionRequestRequestTypeDef

```python
# DeleteSessionRequestRequestTypeDef definition

class DeleteSessionRequestRequestTypeDef(TypedDict):
    Id: str,
    RequestOrigin: NotRequired[str],
```

## DeleteTableRequestRequestTypeDef

```python
# DeleteTableRequestRequestTypeDef definition

class DeleteTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    Name: str,
    CatalogId: NotRequired[str],
    TransactionId: NotRequired[str],
```

## DeleteTableVersionRequestRequestTypeDef

```python
# DeleteTableVersionRequestRequestTypeDef definition

class DeleteTableVersionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    VersionId: str,
    CatalogId: NotRequired[str],
```

## DeleteTriggerRequestRequestTypeDef

```python
# DeleteTriggerRequestRequestTypeDef definition

class DeleteTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteUserDefinedFunctionRequestRequestTypeDef

```python
# DeleteUserDefinedFunctionRequestRequestTypeDef definition

class DeleteUserDefinedFunctionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    FunctionName: str,
    CatalogId: NotRequired[str],
```

## DeleteWorkflowRequestRequestTypeDef

```python
# DeleteWorkflowRequestRequestTypeDef definition

class DeleteWorkflowRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DevEndpointCustomLibrariesTypeDef

```python
# DevEndpointCustomLibrariesTypeDef definition

class DevEndpointCustomLibrariesTypeDef(TypedDict):
    ExtraPythonLibsS3Path: NotRequired[str],
    ExtraJarsS3Path: NotRequired[str],
```

## DirectSchemaChangePolicyTypeDef

```python
# DirectSchemaChangePolicyTypeDef definition

class DirectSchemaChangePolicyTypeDef(TypedDict):
    EnableUpdateCatalog: NotRequired[bool],
    UpdateBehavior: NotRequired[UpdateCatalogBehaviorType],  # (1)
    Table: NotRequired[str],
    Database: NotRequired[str],
```

1. See [:material-code-brackets: UpdateCatalogBehaviorType](./literals.md#updatecatalogbehaviortype) 
## NullCheckBoxListTypeDef

```python
# NullCheckBoxListTypeDef definition

class NullCheckBoxListTypeDef(TypedDict):
    IsEmpty: NotRequired[bool],
    IsNullString: NotRequired[bool],
    IsNegOne: NotRequired[bool],
```

## TransformConfigParameterTypeDef

```python
# TransformConfigParameterTypeDef definition

class TransformConfigParameterTypeDef(TypedDict):
    Name: str,
    Type: ParamTypeType,  # (1)
    ValidationRule: NotRequired[str],
    ValidationMessage: NotRequired[str],
    Value: NotRequired[List[str]],
    ListType: NotRequired[ParamTypeType],  # (1)
    IsOptional: NotRequired[bool],
```

1. See [:material-code-brackets: ParamTypeType](./literals.md#paramtypetype) 
2. See [:material-code-brackets: ParamTypeType](./literals.md#paramtypetype) 
## EdgeTypeDef

```python
# EdgeTypeDef definition

class EdgeTypeDef(TypedDict):
    SourceId: NotRequired[str],
    DestinationId: NotRequired[str],
```

## JobBookmarksEncryptionTypeDef

```python
# JobBookmarksEncryptionTypeDef definition

class JobBookmarksEncryptionTypeDef(TypedDict):
    JobBookmarksEncryptionMode: NotRequired[JobBookmarksEncryptionModeType],  # (1)
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: JobBookmarksEncryptionModeType](./literals.md#jobbookmarksencryptionmodetype) 
## S3EncryptionTypeDef

```python
# S3EncryptionTypeDef definition

class S3EncryptionTypeDef(TypedDict):
    S3EncryptionMode: NotRequired[S3EncryptionModeType],  # (1)
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: S3EncryptionModeType](./literals.md#s3encryptionmodetype) 
## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## ExportLabelsTaskRunPropertiesTypeDef

```python
# ExportLabelsTaskRunPropertiesTypeDef definition

class ExportLabelsTaskRunPropertiesTypeDef(TypedDict):
    OutputS3Path: NotRequired[str],
```

## FederatedTableTypeDef

```python
# FederatedTableTypeDef definition

class FederatedTableTypeDef(TypedDict):
    Identifier: NotRequired[str],
    DatabaseIdentifier: NotRequired[str],
    ConnectionName: NotRequired[str],
```

## FilterValueTypeDef

```python
# FilterValueTypeDef definition

class FilterValueTypeDef(TypedDict):
    Type: FilterValueTypeType,  # (1)
    Value: List[str],
```

1. See [:material-code-brackets: FilterValueTypeType](./literals.md#filtervaluetypetype) 
## FindMatchesParametersTypeDef

```python
# FindMatchesParametersTypeDef definition

class FindMatchesParametersTypeDef(TypedDict):
    PrimaryKeyColumnName: NotRequired[str],
    PrecisionRecallTradeoff: NotRequired[float],
    AccuracyCostTradeoff: NotRequired[float],
    EnforceProvidedLabels: NotRequired[bool],
```

## FindMatchesTaskRunPropertiesTypeDef

```python
# FindMatchesTaskRunPropertiesTypeDef definition

class FindMatchesTaskRunPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
```

## GetBlueprintRequestRequestTypeDef

```python
# GetBlueprintRequestRequestTypeDef definition

class GetBlueprintRequestRequestTypeDef(TypedDict):
    Name: str,
    IncludeBlueprint: NotRequired[bool],
    IncludeParameterSpec: NotRequired[bool],
```

## GetBlueprintRunRequestRequestTypeDef

```python
# GetBlueprintRunRequestRequestTypeDef definition

class GetBlueprintRunRequestRequestTypeDef(TypedDict):
    BlueprintName: str,
    RunId: str,
```

## GetBlueprintRunsRequestRequestTypeDef

```python
# GetBlueprintRunsRequestRequestTypeDef definition

class GetBlueprintRunsRequestRequestTypeDef(TypedDict):
    BlueprintName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetCatalogImportStatusRequestRequestTypeDef

```python
# GetCatalogImportStatusRequestRequestTypeDef definition

class GetCatalogImportStatusRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
```

## GetClassifierRequestRequestTypeDef

```python
# GetClassifierRequestRequestTypeDef definition

class GetClassifierRequestRequestTypeDef(TypedDict):
    Name: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetClassifiersRequestRequestTypeDef

```python
# GetClassifiersRequestRequestTypeDef definition

class GetClassifiersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetColumnStatisticsForPartitionRequestRequestTypeDef

```python
# GetColumnStatisticsForPartitionRequestRequestTypeDef definition

class GetColumnStatisticsForPartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    ColumnNames: Sequence[str],
    CatalogId: NotRequired[str],
```

## GetColumnStatisticsForTableRequestRequestTypeDef

```python
# GetColumnStatisticsForTableRequestRequestTypeDef definition

class GetColumnStatisticsForTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    ColumnNames: Sequence[str],
    CatalogId: NotRequired[str],
```

## GetConnectionRequestRequestTypeDef

```python
# GetConnectionRequestRequestTypeDef definition

class GetConnectionRequestRequestTypeDef(TypedDict):
    Name: str,
    CatalogId: NotRequired[str],
    HidePassword: NotRequired[bool],
```

## GetConnectionsFilterTypeDef

```python
# GetConnectionsFilterTypeDef definition

class GetConnectionsFilterTypeDef(TypedDict):
    MatchCriteria: NotRequired[Sequence[str]],
    ConnectionType: NotRequired[ConnectionTypeType],  # (1)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
## GetCrawlerMetricsRequestRequestTypeDef

```python
# GetCrawlerMetricsRequestRequestTypeDef definition

class GetCrawlerMetricsRequestRequestTypeDef(TypedDict):
    CrawlerNameList: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetCrawlerRequestRequestTypeDef

```python
# GetCrawlerRequestRequestTypeDef definition

class GetCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetCrawlersRequestRequestTypeDef

```python
# GetCrawlersRequestRequestTypeDef definition

class GetCrawlersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetCustomEntityTypeRequestRequestTypeDef

```python
# GetCustomEntityTypeRequestRequestTypeDef definition

class GetCustomEntityTypeRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetDataCatalogEncryptionSettingsRequestRequestTypeDef

```python
# GetDataCatalogEncryptionSettingsRequestRequestTypeDef definition

class GetDataCatalogEncryptionSettingsRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
```

## GetDataQualityResultRequestRequestTypeDef

```python
# GetDataQualityResultRequestRequestTypeDef definition

class GetDataQualityResultRequestRequestTypeDef(TypedDict):
    ResultId: str,
```

## GetDataQualityRuleRecommendationRunRequestRequestTypeDef

```python
# GetDataQualityRuleRecommendationRunRequestRequestTypeDef definition

class GetDataQualityRuleRecommendationRunRequestRequestTypeDef(TypedDict):
    RunId: str,
```

## GetDataQualityRulesetEvaluationRunRequestRequestTypeDef

```python
# GetDataQualityRulesetEvaluationRunRequestRequestTypeDef definition

class GetDataQualityRulesetEvaluationRunRequestRequestTypeDef(TypedDict):
    RunId: str,
```

## GetDataQualityRulesetRequestRequestTypeDef

```python
# GetDataQualityRulesetRequestRequestTypeDef definition

class GetDataQualityRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetDatabaseRequestRequestTypeDef

```python
# GetDatabaseRequestRequestTypeDef definition

class GetDatabaseRequestRequestTypeDef(TypedDict):
    Name: str,
    CatalogId: NotRequired[str],
```

## GetDatabasesRequestRequestTypeDef

```python
# GetDatabasesRequestRequestTypeDef definition

class GetDatabasesRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ResourceShareType: NotRequired[ResourceShareTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
## GetDataflowGraphRequestRequestTypeDef

```python
# GetDataflowGraphRequestRequestTypeDef definition

class GetDataflowGraphRequestRequestTypeDef(TypedDict):
    PythonScript: NotRequired[str],
```

## GetDevEndpointRequestRequestTypeDef

```python
# GetDevEndpointRequestRequestTypeDef definition

class GetDevEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
```

## GetDevEndpointsRequestRequestTypeDef

```python
# GetDevEndpointsRequestRequestTypeDef definition

class GetDevEndpointsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetJobBookmarkRequestRequestTypeDef

```python
# GetJobBookmarkRequestRequestTypeDef definition

class GetJobBookmarkRequestRequestTypeDef(TypedDict):
    JobName: str,
    RunId: NotRequired[str],
```

## JobBookmarkEntryTypeDef

```python
# JobBookmarkEntryTypeDef definition

class JobBookmarkEntryTypeDef(TypedDict):
    JobName: NotRequired[str],
    Version: NotRequired[int],
    Run: NotRequired[int],
    Attempt: NotRequired[int],
    PreviousRunId: NotRequired[str],
    RunId: NotRequired[str],
    JobBookmark: NotRequired[str],
```

## GetJobRequestRequestTypeDef

```python
# GetJobRequestRequestTypeDef definition

class GetJobRequestRequestTypeDef(TypedDict):
    JobName: str,
```

## GetJobRunRequestRequestTypeDef

```python
# GetJobRunRequestRequestTypeDef definition

class GetJobRunRequestRequestTypeDef(TypedDict):
    JobName: str,
    RunId: str,
    PredecessorsIncluded: NotRequired[bool],
```

## GetJobRunsRequestRequestTypeDef

```python
# GetJobRunsRequestRequestTypeDef definition

class GetJobRunsRequestRequestTypeDef(TypedDict):
    JobName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetJobsRequestRequestTypeDef

```python
# GetJobsRequestRequestTypeDef definition

class GetJobsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetMLTaskRunRequestRequestTypeDef

```python
# GetMLTaskRunRequestRequestTypeDef definition

class GetMLTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
    TaskRunId: str,
```

## TaskRunSortCriteriaTypeDef

```python
# TaskRunSortCriteriaTypeDef definition

class TaskRunSortCriteriaTypeDef(TypedDict):
    Column: TaskRunSortColumnTypeType,  # (1)
    SortDirection: SortDirectionTypeType,  # (2)
```

1. See [:material-code-brackets: TaskRunSortColumnTypeType](./literals.md#taskrunsortcolumntypetype) 
2. See [:material-code-brackets: SortDirectionTypeType](./literals.md#sortdirectiontypetype) 
## GetMLTransformRequestRequestTypeDef

```python
# GetMLTransformRequestRequestTypeDef definition

class GetMLTransformRequestRequestTypeDef(TypedDict):
    TransformId: str,
```

## SchemaColumnTypeDef

```python
# SchemaColumnTypeDef definition

class SchemaColumnTypeDef(TypedDict):
    Name: NotRequired[str],
    DataType: NotRequired[str],
```

## TransformSortCriteriaTypeDef

```python
# TransformSortCriteriaTypeDef definition

class TransformSortCriteriaTypeDef(TypedDict):
    Column: TransformSortColumnTypeType,  # (1)
    SortDirection: SortDirectionTypeType,  # (2)
```

1. See [:material-code-brackets: TransformSortColumnTypeType](./literals.md#transformsortcolumntypetype) 
2. See [:material-code-brackets: SortDirectionTypeType](./literals.md#sortdirectiontypetype) 
## MappingEntryTypeDef

```python
# MappingEntryTypeDef definition

class MappingEntryTypeDef(TypedDict):
    SourceTable: NotRequired[str],
    SourcePath: NotRequired[str],
    SourceType: NotRequired[str],
    TargetTable: NotRequired[str],
    TargetPath: NotRequired[str],
    TargetType: NotRequired[str],
```

## GetPartitionIndexesRequestRequestTypeDef

```python
# GetPartitionIndexesRequestRequestTypeDef definition

class GetPartitionIndexesRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetPartitionRequestRequestTypeDef

```python
# GetPartitionRequestRequestTypeDef definition

class GetPartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    CatalogId: NotRequired[str],
```

## SegmentTypeDef

```python
# SegmentTypeDef definition

class SegmentTypeDef(TypedDict):
    SegmentNumber: int,
    TotalSegments: int,
```

## GetResourcePoliciesRequestRequestTypeDef

```python
# GetResourcePoliciesRequestRequestTypeDef definition

class GetResourcePoliciesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GluePolicyTypeDef

```python
# GluePolicyTypeDef definition

class GluePolicyTypeDef(TypedDict):
    PolicyInJson: NotRequired[str],
    PolicyHash: NotRequired[str],
    CreateTime: NotRequired[datetime],
    UpdateTime: NotRequired[datetime],
```

## GetResourcePolicyRequestRequestTypeDef

```python
# GetResourcePolicyRequestRequestTypeDef definition

class GetResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
```

## SchemaVersionNumberTypeDef

```python
# SchemaVersionNumberTypeDef definition

class SchemaVersionNumberTypeDef(TypedDict):
    LatestVersion: NotRequired[bool],
    VersionNumber: NotRequired[int],
```

## GetSecurityConfigurationRequestRequestTypeDef

```python
# GetSecurityConfigurationRequestRequestTypeDef definition

class GetSecurityConfigurationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetSecurityConfigurationsRequestRequestTypeDef

```python
# GetSecurityConfigurationsRequestRequestTypeDef definition

class GetSecurityConfigurationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetSessionRequestRequestTypeDef

```python
# GetSessionRequestRequestTypeDef definition

class GetSessionRequestRequestTypeDef(TypedDict):
    Id: str,
    RequestOrigin: NotRequired[str],
```

## GetStatementRequestRequestTypeDef

```python
# GetStatementRequestRequestTypeDef definition

class GetStatementRequestRequestTypeDef(TypedDict):
    SessionId: str,
    Id: int,
    RequestOrigin: NotRequired[str],
```

## GetTableVersionRequestRequestTypeDef

```python
# GetTableVersionRequestRequestTypeDef definition

class GetTableVersionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    VersionId: NotRequired[str],
```

## GetTableVersionsRequestRequestTypeDef

```python
# GetTableVersionsRequestRequestTypeDef definition

class GetTableVersionsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetTagsRequestRequestTypeDef

```python
# GetTagsRequestRequestTypeDef definition

class GetTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetTriggerRequestRequestTypeDef

```python
# GetTriggerRequestRequestTypeDef definition

class GetTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetTriggersRequestRequestTypeDef

```python
# GetTriggersRequestRequestTypeDef definition

class GetTriggersRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    DependentJobName: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetUserDefinedFunctionRequestRequestTypeDef

```python
# GetUserDefinedFunctionRequestRequestTypeDef definition

class GetUserDefinedFunctionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    FunctionName: str,
    CatalogId: NotRequired[str],
```

## GetUserDefinedFunctionsRequestRequestTypeDef

```python
# GetUserDefinedFunctionsRequestRequestTypeDef definition

class GetUserDefinedFunctionsRequestRequestTypeDef(TypedDict):
    Pattern: str,
    CatalogId: NotRequired[str],
    DatabaseName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetWorkflowRequestRequestTypeDef

```python
# GetWorkflowRequestRequestTypeDef definition

class GetWorkflowRequestRequestTypeDef(TypedDict):
    Name: str,
    IncludeGraph: NotRequired[bool],
```

## GetWorkflowRunPropertiesRequestRequestTypeDef

```python
# GetWorkflowRunPropertiesRequestRequestTypeDef definition

class GetWorkflowRunPropertiesRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
```

## GetWorkflowRunRequestRequestTypeDef

```python
# GetWorkflowRunRequestRequestTypeDef definition

class GetWorkflowRunRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
    IncludeGraph: NotRequired[bool],
```

## GetWorkflowRunsRequestRequestTypeDef

```python
# GetWorkflowRunsRequestRequestTypeDef definition

class GetWorkflowRunsRequestRequestTypeDef(TypedDict):
    Name: str,
    IncludeGraph: NotRequired[bool],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GlueStudioSchemaColumnTypeDef

```python
# GlueStudioSchemaColumnTypeDef definition

class GlueStudioSchemaColumnTypeDef(TypedDict):
    Name: str,
    Type: NotRequired[str],
```

## S3SourceAdditionalOptionsTypeDef

```python
# S3SourceAdditionalOptionsTypeDef definition

class S3SourceAdditionalOptionsTypeDef(TypedDict):
    BoundedSize: NotRequired[int],
    BoundedFiles: NotRequired[int],
```

## IcebergInputTypeDef

```python
# IcebergInputTypeDef definition

class IcebergInputTypeDef(TypedDict):
    MetadataOperation: MetadataOperationType,  # (1)
    Version: NotRequired[str],
```

1. See [:material-code-brackets: MetadataOperationType](./literals.md#metadataoperationtype) 
## ImportCatalogToGlueRequestRequestTypeDef

```python
# ImportCatalogToGlueRequestRequestTypeDef definition

class ImportCatalogToGlueRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
```

## ImportLabelsTaskRunPropertiesTypeDef

```python
# ImportLabelsTaskRunPropertiesTypeDef definition

class ImportLabelsTaskRunPropertiesTypeDef(TypedDict):
    InputS3Path: NotRequired[str],
    Replace: NotRequired[bool],
```

## JDBCConnectorOptionsTypeDef

```python
# JDBCConnectorOptionsTypeDef definition

class JDBCConnectorOptionsTypeDef(TypedDict):
    FilterPredicate: NotRequired[str],
    PartitionColumn: NotRequired[str],
    LowerBound: NotRequired[int],
    UpperBound: NotRequired[int],
    NumPartitions: NotRequired[int],
    JobBookmarkKeys: NotRequired[List[str]],
    JobBookmarkKeysSortOrder: NotRequired[str],
    DataTypeMapping: NotRequired[Dict[JDBCDataTypeType, GlueRecordTypeType]],  # (1)
```

1. See [:material-code-brackets: JDBCDataTypeType](./literals.md#jdbcdatatypetype) [:material-code-brackets: GlueRecordTypeType](./literals.md#gluerecordtypetype) 
## PredecessorTypeDef

```python
# PredecessorTypeDef definition

class PredecessorTypeDef(TypedDict):
    JobName: NotRequired[str],
    RunId: NotRequired[str],
```

## JoinColumnTypeDef

```python
# JoinColumnTypeDef definition

class JoinColumnTypeDef(TypedDict):
    From: str,
    Keys: List[List[str]],
```

## KeySchemaElementTypeDef

```python
# KeySchemaElementTypeDef definition

class KeySchemaElementTypeDef(TypedDict):
    Name: str,
    Type: str,
```

## LabelingSetGenerationTaskRunPropertiesTypeDef

```python
# LabelingSetGenerationTaskRunPropertiesTypeDef definition

class LabelingSetGenerationTaskRunPropertiesTypeDef(TypedDict):
    OutputS3Path: NotRequired[str],
```

## ListBlueprintsRequestRequestTypeDef

```python
# ListBlueprintsRequestRequestTypeDef definition

class ListBlueprintsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

## ListCrawlersRequestRequestTypeDef

```python
# ListCrawlersRequestRequestTypeDef definition

class ListCrawlersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## ListCustomEntityTypesRequestRequestTypeDef

```python
# ListCustomEntityTypesRequestRequestTypeDef definition

class ListCustomEntityTypesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

## ListDevEndpointsRequestRequestTypeDef

```python
# ListDevEndpointsRequestRequestTypeDef definition

class ListDevEndpointsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

## ListJobsRequestRequestTypeDef

```python
# ListJobsRequestRequestTypeDef definition

class ListJobsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

## ListRegistriesInputRequestTypeDef

```python
# ListRegistriesInputRequestTypeDef definition

class ListRegistriesInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## RegistryListItemTypeDef

```python
# RegistryListItemTypeDef definition

class RegistryListItemTypeDef(TypedDict):
    RegistryName: NotRequired[str],
    RegistryArn: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[RegistryStatusType],  # (1)
    CreatedTime: NotRequired[str],
    UpdatedTime: NotRequired[str],
```

1. See [:material-code-brackets: RegistryStatusType](./literals.md#registrystatustype) 
## SchemaVersionListItemTypeDef

```python
# SchemaVersionListItemTypeDef definition

class SchemaVersionListItemTypeDef(TypedDict):
    SchemaArn: NotRequired[str],
    SchemaVersionId: NotRequired[str],
    VersionNumber: NotRequired[int],
    Status: NotRequired[SchemaVersionStatusType],  # (1)
    CreatedTime: NotRequired[str],
```

1. See [:material-code-brackets: SchemaVersionStatusType](./literals.md#schemaversionstatustype) 
## SchemaListItemTypeDef

```python
# SchemaListItemTypeDef definition

class SchemaListItemTypeDef(TypedDict):
    RegistryName: NotRequired[str],
    SchemaName: NotRequired[str],
    SchemaArn: NotRequired[str],
    Description: NotRequired[str],
    SchemaStatus: NotRequired[SchemaStatusType],  # (1)
    CreatedTime: NotRequired[str],
    UpdatedTime: NotRequired[str],
```

1. See [:material-code-brackets: SchemaStatusType](./literals.md#schemastatustype) 
## ListSessionsRequestRequestTypeDef

```python
# ListSessionsRequestRequestTypeDef definition

class ListSessionsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
    RequestOrigin: NotRequired[str],
```

## ListStatementsRequestRequestTypeDef

```python
# ListStatementsRequestRequestTypeDef definition

class ListStatementsRequestRequestTypeDef(TypedDict):
    SessionId: str,
    RequestOrigin: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListTriggersRequestRequestTypeDef

```python
# ListTriggersRequestRequestTypeDef definition

class ListTriggersRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    DependentJobName: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

## ListWorkflowsRequestRequestTypeDef

```python
# ListWorkflowsRequestRequestTypeDef definition

class ListWorkflowsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MLUserDataEncryptionTypeDef

```python
# MLUserDataEncryptionTypeDef definition

class MLUserDataEncryptionTypeDef(TypedDict):
    MlUserDataEncryptionMode: MLUserDataEncryptionModeStringType,  # (1)
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: MLUserDataEncryptionModeStringType](./literals.md#mluserdataencryptionmodestringtype) 
## MappingTypeDef

```python
# MappingTypeDef definition

class MappingTypeDef(TypedDict):
    ToKey: NotRequired[str],
    FromPath: NotRequired[List[str]],
    FromType: NotRequired[str],
    ToType: NotRequired[str],
    Dropped: NotRequired[bool],
    Children: NotRequired[List[MappingTypeDef]],  # (1)
```

1. See [:material-code-braces: MappingTypeDef](./type_defs.md#mappingtypedef) 
## OtherMetadataValueListItemTypeDef

```python
# OtherMetadataValueListItemTypeDef definition

class OtherMetadataValueListItemTypeDef(TypedDict):
    MetadataValue: NotRequired[str],
    CreatedTime: NotRequired[str],
```

## MetadataKeyValuePairTypeDef

```python
# MetadataKeyValuePairTypeDef definition

class MetadataKeyValuePairTypeDef(TypedDict):
    MetadataKey: NotRequired[str],
    MetadataValue: NotRequired[str],
```

## OrderTypeDef

```python
# OrderTypeDef definition

class OrderTypeDef(TypedDict):
    Column: str,
    SortOrder: int,
```

## PropertyPredicateTypeDef

```python
# PropertyPredicateTypeDef definition

class PropertyPredicateTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    Comparator: NotRequired[ComparatorType],  # (1)
```

1. See [:material-code-brackets: ComparatorType](./literals.md#comparatortype) 
## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    PolicyInJson: str,
    ResourceArn: NotRequired[str],
    PolicyHashCondition: NotRequired[str],
    PolicyExistsCondition: NotRequired[ExistConditionType],  # (1)
    EnableHybrid: NotRequired[EnableHybridValuesType],  # (2)
```

1. See [:material-code-brackets: ExistConditionType](./literals.md#existconditiontype) 
2. See [:material-code-brackets: EnableHybridValuesType](./literals.md#enablehybridvaluestype) 
## PutWorkflowRunPropertiesRequestRequestTypeDef

```python
# PutWorkflowRunPropertiesRequestRequestTypeDef definition

class PutWorkflowRunPropertiesRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
    RunProperties: Mapping[str, str],
```

## RecipeReferenceTypeDef

```python
# RecipeReferenceTypeDef definition

class RecipeReferenceTypeDef(TypedDict):
    RecipeArn: str,
    RecipeVersion: str,
```

## UpsertRedshiftTargetOptionsTypeDef

```python
# UpsertRedshiftTargetOptionsTypeDef definition

class UpsertRedshiftTargetOptionsTypeDef(TypedDict):
    TableLocation: NotRequired[str],
    ConnectionName: NotRequired[str],
    UpsertKeys: NotRequired[List[str]],
```

## ResetJobBookmarkRequestRequestTypeDef

```python
# ResetJobBookmarkRequestRequestTypeDef definition

class ResetJobBookmarkRequestRequestTypeDef(TypedDict):
    JobName: str,
    RunId: NotRequired[str],
```

## ResourceUriTypeDef

```python
# ResourceUriTypeDef definition

class ResourceUriTypeDef(TypedDict):
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    Uri: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ResumeWorkflowRunRequestRequestTypeDef

```python
# ResumeWorkflowRunRequestRequestTypeDef definition

class ResumeWorkflowRunRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
    NodeIds: Sequence[str],
```

## RunStatementRequestRequestTypeDef

```python
# RunStatementRequestRequestTypeDef definition

class RunStatementRequestRequestTypeDef(TypedDict):
    SessionId: str,
    Code: str,
    RequestOrigin: NotRequired[str],
```

## S3DirectSourceAdditionalOptionsTypeDef

```python
# S3DirectSourceAdditionalOptionsTypeDef definition

class S3DirectSourceAdditionalOptionsTypeDef(TypedDict):
    BoundedSize: NotRequired[int],
    BoundedFiles: NotRequired[int],
    EnableSamplePath: NotRequired[bool],
    SamplePath: NotRequired[str],
```

## SortCriterionTypeDef

```python
# SortCriterionTypeDef definition

class SortCriterionTypeDef(TypedDict):
    FieldName: NotRequired[str],
    Sort: NotRequired[SortType],  # (1)
```

1. See [:material-code-brackets: SortType](./literals.md#sorttype) 
## SerDeInfoTypeDef

```python
# SerDeInfoTypeDef definition

class SerDeInfoTypeDef(TypedDict):
    Name: NotRequired[str],
    SerializationLibrary: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
```

## SkewedInfoTypeDef

```python
# SkewedInfoTypeDef definition

class SkewedInfoTypeDef(TypedDict):
    SkewedColumnNames: NotRequired[Sequence[str]],
    SkewedColumnValues: NotRequired[Sequence[str]],
    SkewedColumnValueLocationMaps: NotRequired[Mapping[str, str]],
```

## SqlAliasTypeDef

```python
# SqlAliasTypeDef definition

class SqlAliasTypeDef(TypedDict):
    From: str,
    Alias: str,
```

## StartBlueprintRunRequestRequestTypeDef

```python
# StartBlueprintRunRequestRequestTypeDef definition

class StartBlueprintRunRequestRequestTypeDef(TypedDict):
    BlueprintName: str,
    RoleArn: str,
    Parameters: NotRequired[str],
```

## StartCrawlerRequestRequestTypeDef

```python
# StartCrawlerRequestRequestTypeDef definition

class StartCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StartCrawlerScheduleRequestRequestTypeDef

```python
# StartCrawlerScheduleRequestRequestTypeDef definition

class StartCrawlerScheduleRequestRequestTypeDef(TypedDict):
    CrawlerName: str,
```

## StartExportLabelsTaskRunRequestRequestTypeDef

```python
# StartExportLabelsTaskRunRequestRequestTypeDef definition

class StartExportLabelsTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
    OutputS3Path: str,
```

## StartImportLabelsTaskRunRequestRequestTypeDef

```python
# StartImportLabelsTaskRunRequestRequestTypeDef definition

class StartImportLabelsTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
    InputS3Path: str,
    ReplaceAllLabels: NotRequired[bool],
```

## StartMLEvaluationTaskRunRequestRequestTypeDef

```python
# StartMLEvaluationTaskRunRequestRequestTypeDef definition

class StartMLEvaluationTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
```

## StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef

```python
# StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef definition

class StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
    OutputS3Path: str,
```

## StartTriggerRequestRequestTypeDef

```python
# StartTriggerRequestRequestTypeDef definition

class StartTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StartWorkflowRunRequestRequestTypeDef

```python
# StartWorkflowRunRequestRequestTypeDef definition

class StartWorkflowRunRequestRequestTypeDef(TypedDict):
    Name: str,
    RunProperties: NotRequired[Mapping[str, str]],
```

## StartingEventBatchConditionTypeDef

```python
# StartingEventBatchConditionTypeDef definition

class StartingEventBatchConditionTypeDef(TypedDict):
    BatchSize: NotRequired[int],
    BatchWindow: NotRequired[int],
```

## StatementOutputDataTypeDef

```python
# StatementOutputDataTypeDef definition

class StatementOutputDataTypeDef(TypedDict):
    TextPlain: NotRequired[str],
```

## StopCrawlerRequestRequestTypeDef

```python
# StopCrawlerRequestRequestTypeDef definition

class StopCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StopCrawlerScheduleRequestRequestTypeDef

```python
# StopCrawlerScheduleRequestRequestTypeDef definition

class StopCrawlerScheduleRequestRequestTypeDef(TypedDict):
    CrawlerName: str,
```

## StopSessionRequestRequestTypeDef

```python
# StopSessionRequestRequestTypeDef definition

class StopSessionRequestRequestTypeDef(TypedDict):
    Id: str,
    RequestOrigin: NotRequired[str],
```

## StopTriggerRequestRequestTypeDef

```python
# StopTriggerRequestRequestTypeDef definition

class StopTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StopWorkflowRunRequestRequestTypeDef

```python
# StopWorkflowRunRequestRequestTypeDef definition

class StopWorkflowRunRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
```

## TableIdentifierTypeDef

```python
# TableIdentifierTypeDef definition

class TableIdentifierTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    DatabaseName: NotRequired[str],
    Name: NotRequired[str],
    Region: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagsToAdd: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagsToRemove: Sequence[str],
```

## UpdateBlueprintRequestRequestTypeDef

```python
# UpdateBlueprintRequestRequestTypeDef definition

class UpdateBlueprintRequestRequestTypeDef(TypedDict):
    Name: str,
    BlueprintLocation: str,
    Description: NotRequired[str],
```

## UpdateCsvClassifierRequestTypeDef

```python
# UpdateCsvClassifierRequestTypeDef definition

class UpdateCsvClassifierRequestTypeDef(TypedDict):
    Name: str,
    Delimiter: NotRequired[str],
    QuoteSymbol: NotRequired[str],
    ContainsHeader: NotRequired[CsvHeaderOptionType],  # (1)
    Header: NotRequired[Sequence[str]],
    DisableValueTrimming: NotRequired[bool],
    AllowSingleColumn: NotRequired[bool],
    CustomDatatypeConfigured: NotRequired[bool],
    CustomDatatypes: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: CsvHeaderOptionType](./literals.md#csvheaderoptiontype) 
## UpdateGrokClassifierRequestTypeDef

```python
# UpdateGrokClassifierRequestTypeDef definition

class UpdateGrokClassifierRequestTypeDef(TypedDict):
    Name: str,
    Classification: NotRequired[str],
    GrokPattern: NotRequired[str],
    CustomPatterns: NotRequired[str],
```

## UpdateJsonClassifierRequestTypeDef

```python
# UpdateJsonClassifierRequestTypeDef definition

class UpdateJsonClassifierRequestTypeDef(TypedDict):
    Name: str,
    JsonPath: NotRequired[str],
```

## UpdateXMLClassifierRequestTypeDef

```python
# UpdateXMLClassifierRequestTypeDef definition

class UpdateXMLClassifierRequestTypeDef(TypedDict):
    Name: str,
    Classification: NotRequired[str],
    RowTag: NotRequired[str],
```

## UpdateCrawlerScheduleRequestRequestTypeDef

```python
# UpdateCrawlerScheduleRequestRequestTypeDef definition

class UpdateCrawlerScheduleRequestRequestTypeDef(TypedDict):
    CrawlerName: str,
    Schedule: NotRequired[str],
```

## UpdateDataQualityRulesetRequestRequestTypeDef

```python
# UpdateDataQualityRulesetRequestRequestTypeDef definition

class UpdateDataQualityRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    Ruleset: NotRequired[str],
```

## UpdateJobFromSourceControlRequestRequestTypeDef

```python
# UpdateJobFromSourceControlRequestRequestTypeDef definition

class UpdateJobFromSourceControlRequestRequestTypeDef(TypedDict):
    JobName: NotRequired[str],
    Provider: NotRequired[SourceControlProviderType],  # (1)
    RepositoryName: NotRequired[str],
    RepositoryOwner: NotRequired[str],
    BranchName: NotRequired[str],
    Folder: NotRequired[str],
    CommitId: NotRequired[str],
    AuthStrategy: NotRequired[SourceControlAuthStrategyType],  # (2)
    AuthToken: NotRequired[str],
```

1. See [:material-code-brackets: SourceControlProviderType](./literals.md#sourcecontrolprovidertype) 
2. See [:material-code-brackets: SourceControlAuthStrategyType](./literals.md#sourcecontrolauthstrategytype) 
## UpdateSourceControlFromJobRequestRequestTypeDef

```python
# UpdateSourceControlFromJobRequestRequestTypeDef definition

class UpdateSourceControlFromJobRequestRequestTypeDef(TypedDict):
    JobName: NotRequired[str],
    Provider: NotRequired[SourceControlProviderType],  # (1)
    RepositoryName: NotRequired[str],
    RepositoryOwner: NotRequired[str],
    BranchName: NotRequired[str],
    Folder: NotRequired[str],
    CommitId: NotRequired[str],
    AuthStrategy: NotRequired[SourceControlAuthStrategyType],  # (2)
    AuthToken: NotRequired[str],
```

1. See [:material-code-brackets: SourceControlProviderType](./literals.md#sourcecontrolprovidertype) 
2. See [:material-code-brackets: SourceControlAuthStrategyType](./literals.md#sourcecontrolauthstrategytype) 
## UpdateWorkflowRequestRequestTypeDef

```python
# UpdateWorkflowRequestRequestTypeDef definition

class UpdateWorkflowRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    DefaultRunProperties: NotRequired[Mapping[str, str]],
    MaxConcurrentRuns: NotRequired[int],
```

## WorkflowRunStatisticsTypeDef

```python
# WorkflowRunStatisticsTypeDef definition

class WorkflowRunStatisticsTypeDef(TypedDict):
    TotalActions: NotRequired[int],
    TimeoutActions: NotRequired[int],
    FailedActions: NotRequired[int],
    StoppedActions: NotRequired[int],
    SucceededActions: NotRequired[int],
    RunningActions: NotRequired[int],
    ErroredActions: NotRequired[int],
    WaitingActions: NotRequired[int],
```

## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    JobName: NotRequired[str],
    Arguments: NotRequired[Dict[str, str]],
    Timeout: NotRequired[int],
    SecurityConfiguration: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (1)
    CrawlerName: NotRequired[str],
```

1. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
## StartJobRunRequestRequestTypeDef

```python
# StartJobRunRequestRequestTypeDef definition

class StartJobRunRequestRequestTypeDef(TypedDict):
    JobName: str,
    JobRunId: NotRequired[str],
    Arguments: NotRequired[Mapping[str, str]],
    AllocatedCapacity: NotRequired[int],
    Timeout: NotRequired[int],
    MaxCapacity: NotRequired[float],
    SecurityConfiguration: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (1)
    WorkerType: NotRequired[WorkerTypeType],  # (2)
    NumberOfWorkers: NotRequired[int],
    ExecutionClass: NotRequired[ExecutionClassType],  # (3)
```

1. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
2. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
3. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
## AggregateTypeDef

```python
# AggregateTypeDef definition

class AggregateTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Groups: List[List[str]],
    Aggs: List[AggregateOperationTypeDef],  # (1)
```

1. See [:material-code-braces: AggregateOperationTypeDef](./type_defs.md#aggregateoperationtypedef) 
## AmazonRedshiftNodeDataTypeDef

```python
# AmazonRedshiftNodeDataTypeDef definition

class AmazonRedshiftNodeDataTypeDef(TypedDict):
    AccessType: NotRequired[str],
    SourceType: NotRequired[str],
    Connection: NotRequired[OptionTypeDef],  # (1)
    Schema: NotRequired[OptionTypeDef],  # (1)
    Table: NotRequired[OptionTypeDef],  # (1)
    CatalogDatabase: NotRequired[OptionTypeDef],  # (1)
    CatalogTable: NotRequired[OptionTypeDef],  # (1)
    CatalogRedshiftSchema: NotRequired[str],
    CatalogRedshiftTable: NotRequired[str],
    TempDir: NotRequired[str],
    IamRole: NotRequired[OptionTypeDef],  # (1)
    AdvancedOptions: NotRequired[List[AmazonRedshiftAdvancedOptionTypeDef]],  # (7)
    SampleQuery: NotRequired[str],
    PreAction: NotRequired[str],
    PostAction: NotRequired[str],
    Action: NotRequired[str],
    TablePrefix: NotRequired[str],
    Upsert: NotRequired[bool],
    MergeAction: NotRequired[str],
    MergeWhenMatched: NotRequired[str],
    MergeWhenNotMatched: NotRequired[str],
    MergeClause: NotRequired[str],
    CrawlerConnection: NotRequired[str],
    TableSchema: NotRequired[List[OptionTypeDef]],  # (8)
    StagingTable: NotRequired[str],
    SelectedColumns: NotRequired[List[OptionTypeDef]],  # (8)
```

1. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
2. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
3. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
4. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
5. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
6. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
7. See [:material-code-braces: AmazonRedshiftAdvancedOptionTypeDef](./type_defs.md#amazonredshiftadvancedoptiontypedef) 
8. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
9. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
## SnowflakeNodeDataTypeDef

```python
# SnowflakeNodeDataTypeDef definition

class SnowflakeNodeDataTypeDef(TypedDict):
    SourceType: NotRequired[str],
    Connection: NotRequired[OptionTypeDef],  # (1)
    Schema: NotRequired[str],
    Table: NotRequired[str],
    Database: NotRequired[str],
    TempDir: NotRequired[str],
    IamRole: NotRequired[OptionTypeDef],  # (1)
    AdditionalOptions: NotRequired[Dict[str, str]],
    SampleQuery: NotRequired[str],
    PreAction: NotRequired[str],
    PostAction: NotRequired[str],
    Action: NotRequired[str],
    Upsert: NotRequired[bool],
    MergeAction: NotRequired[str],
    MergeWhenMatched: NotRequired[str],
    MergeWhenNotMatched: NotRequired[str],
    MergeClause: NotRequired[str],
    StagingTable: NotRequired[str],
    SelectedColumns: NotRequired[List[OptionTypeDef]],  # (3)
    AutoPushdown: NotRequired[bool],
    TableSchema: NotRequired[List[OptionTypeDef]],  # (3)
```

1. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
2. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
3. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
4. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
## GetUnfilteredPartitionMetadataRequestRequestTypeDef

```python
# GetUnfilteredPartitionMetadataRequestRequestTypeDef definition

class GetUnfilteredPartitionMetadataRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    SupportedPermissionTypes: Sequence[PermissionTypeType],  # (1)
    AuditContext: NotRequired[AuditContextTypeDef],  # (2)
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
## GetUnfilteredTableMetadataRequestRequestTypeDef

```python
# GetUnfilteredTableMetadataRequestRequestTypeDef definition

class GetUnfilteredTableMetadataRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    Name: str,
    SupportedPermissionTypes: Sequence[PermissionTypeType],  # (1)
    AuditContext: NotRequired[AuditContextTypeDef],  # (2)
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
## BackfillErrorTypeDef

```python
# BackfillErrorTypeDef definition

class BackfillErrorTypeDef(TypedDict):
    Code: NotRequired[BackfillErrorCodeType],  # (1)
    Partitions: NotRequired[List[PartitionValueListTypeDef]],  # (2)
```

1. See [:material-code-brackets: BackfillErrorCodeType](./literals.md#backfillerrorcodetype) 
2. See [:material-code-braces: PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef) 
## BatchDeletePartitionRequestRequestTypeDef

```python
# BatchDeletePartitionRequestRequestTypeDef definition

class BatchDeletePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionsToDelete: Sequence[PartitionValueListTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef) 
## BatchGetPartitionRequestRequestTypeDef

```python
# BatchGetPartitionRequestRequestTypeDef definition

class BatchGetPartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionsToGet: Sequence[PartitionValueListTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef) 
## CancelMLTaskRunResponseTypeDef

```python
# CancelMLTaskRunResponseTypeDef definition

class CancelMLTaskRunResponseTypeDef(TypedDict):
    TransformId: str,
    TaskRunId: str,
    Status: TaskStatusTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CheckSchemaVersionValidityResponseTypeDef

```python
# CheckSchemaVersionValidityResponseTypeDef definition

class CheckSchemaVersionValidityResponseTypeDef(TypedDict):
    Valid: bool,
    Error: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBlueprintResponseTypeDef

```python
# CreateBlueprintResponseTypeDef definition

class CreateBlueprintResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomEntityTypeResponseTypeDef

```python
# CreateCustomEntityTypeResponseTypeDef definition

class CreateCustomEntityTypeResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataQualityRulesetResponseTypeDef

```python
# CreateDataQualityRulesetResponseTypeDef definition

class CreateDataQualityRulesetResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDevEndpointResponseTypeDef

```python
# CreateDevEndpointResponseTypeDef definition

class CreateDevEndpointResponseTypeDef(TypedDict):
    EndpointName: str,
    Status: str,
    SecurityGroupIds: List[str],
    SubnetId: str,
    RoleArn: str,
    YarnEndpointAddress: str,
    ZeppelinRemoteSparkInterpreterPort: int,
    NumberOfNodes: int,
    WorkerType: WorkerTypeType,  # (1)
    GlueVersion: str,
    NumberOfWorkers: int,
    AvailabilityZone: str,
    VpcId: str,
    ExtraPythonLibsS3Path: str,
    ExtraJarsS3Path: str,
    FailureReason: str,
    SecurityConfiguration: str,
    CreatedTimestamp: datetime,
    Arguments: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobResponseTypeDef

```python
# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMLTransformResponseTypeDef

```python
# CreateMLTransformResponseTypeDef definition

class CreateMLTransformResponseTypeDef(TypedDict):
    TransformId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRegistryResponseTypeDef

```python
# CreateRegistryResponseTypeDef definition

class CreateRegistryResponseTypeDef(TypedDict):
    RegistryArn: str,
    RegistryName: str,
    Description: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSchemaResponseTypeDef

```python
# CreateSchemaResponseTypeDef definition

class CreateSchemaResponseTypeDef(TypedDict):
    RegistryName: str,
    RegistryArn: str,
    SchemaName: str,
    SchemaArn: str,
    Description: str,
    DataFormat: DataFormatType,  # (1)
    Compatibility: CompatibilityType,  # (2)
    SchemaCheckpoint: int,
    LatestSchemaVersion: int,
    NextSchemaVersion: int,
    SchemaStatus: SchemaStatusType,  # (3)
    Tags: Dict[str, str],
    SchemaVersionId: str,
    SchemaVersionStatus: SchemaVersionStatusType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
3. See [:material-code-brackets: SchemaStatusType](./literals.md#schemastatustype) 
4. See [:material-code-brackets: SchemaVersionStatusType](./literals.md#schemaversionstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScriptResponseTypeDef

```python
# CreateScriptResponseTypeDef definition

class CreateScriptResponseTypeDef(TypedDict):
    PythonScript: str,
    ScalaCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSecurityConfigurationResponseTypeDef

```python
# CreateSecurityConfigurationResponseTypeDef definition

class CreateSecurityConfigurationResponseTypeDef(TypedDict):
    Name: str,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTriggerResponseTypeDef

```python
# CreateTriggerResponseTypeDef definition

class CreateTriggerResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkflowResponseTypeDef

```python
# CreateWorkflowResponseTypeDef definition

class CreateWorkflowResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBlueprintResponseTypeDef

```python
# DeleteBlueprintResponseTypeDef definition

class DeleteBlueprintResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCustomEntityTypeResponseTypeDef

```python
# DeleteCustomEntityTypeResponseTypeDef definition

class DeleteCustomEntityTypeResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteJobResponseTypeDef

```python
# DeleteJobResponseTypeDef definition

class DeleteJobResponseTypeDef(TypedDict):
    JobName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMLTransformResponseTypeDef

```python
# DeleteMLTransformResponseTypeDef definition

class DeleteMLTransformResponseTypeDef(TypedDict):
    TransformId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRegistryResponseTypeDef

```python
# DeleteRegistryResponseTypeDef definition

class DeleteRegistryResponseTypeDef(TypedDict):
    RegistryName: str,
    RegistryArn: str,
    Status: RegistryStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RegistryStatusType](./literals.md#registrystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSchemaResponseTypeDef

```python
# DeleteSchemaResponseTypeDef definition

class DeleteSchemaResponseTypeDef(TypedDict):
    SchemaArn: str,
    SchemaName: str,
    Status: SchemaStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SchemaStatusType](./literals.md#schemastatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSessionResponseTypeDef

```python
# DeleteSessionResponseTypeDef definition

class DeleteSessionResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTriggerResponseTypeDef

```python
# DeleteTriggerResponseTypeDef definition

class DeleteTriggerResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkflowResponseTypeDef

```python
# DeleteWorkflowResponseTypeDef definition

class DeleteWorkflowResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCustomEntityTypeResponseTypeDef

```python
# GetCustomEntityTypeResponseTypeDef definition

class GetCustomEntityTypeResponseTypeDef(TypedDict):
    Name: str,
    RegexString: str,
    ContextWords: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPlanResponseTypeDef

```python
# GetPlanResponseTypeDef definition

class GetPlanResponseTypeDef(TypedDict):
    PythonScript: str,
    ScalaCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRegistryResponseTypeDef

```python
# GetRegistryResponseTypeDef definition

class GetRegistryResponseTypeDef(TypedDict):
    RegistryName: str,
    RegistryArn: str,
    Description: str,
    Status: RegistryStatusType,  # (1)
    CreatedTime: str,
    UpdatedTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RegistryStatusType](./literals.md#registrystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    PolicyInJson: str,
    PolicyHash: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaByDefinitionResponseTypeDef

```python
# GetSchemaByDefinitionResponseTypeDef definition

class GetSchemaByDefinitionResponseTypeDef(TypedDict):
    SchemaVersionId: str,
    SchemaArn: str,
    DataFormat: DataFormatType,  # (1)
    Status: SchemaVersionStatusType,  # (2)
    CreatedTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-brackets: SchemaVersionStatusType](./literals.md#schemaversionstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaResponseTypeDef

```python
# GetSchemaResponseTypeDef definition

class GetSchemaResponseTypeDef(TypedDict):
    RegistryName: str,
    RegistryArn: str,
    SchemaName: str,
    SchemaArn: str,
    Description: str,
    DataFormat: DataFormatType,  # (1)
    Compatibility: CompatibilityType,  # (2)
    SchemaCheckpoint: int,
    LatestSchemaVersion: int,
    NextSchemaVersion: int,
    SchemaStatus: SchemaStatusType,  # (3)
    CreatedTime: str,
    UpdatedTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
3. See [:material-code-brackets: SchemaStatusType](./literals.md#schemastatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaVersionResponseTypeDef

```python
# GetSchemaVersionResponseTypeDef definition

class GetSchemaVersionResponseTypeDef(TypedDict):
    SchemaVersionId: str,
    SchemaDefinition: str,
    DataFormat: DataFormatType,  # (1)
    SchemaArn: str,
    VersionNumber: int,
    Status: SchemaVersionStatusType,  # (2)
    CreatedTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-brackets: SchemaVersionStatusType](./literals.md#schemaversionstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaVersionsDiffResponseTypeDef

```python
# GetSchemaVersionsDiffResponseTypeDef definition

class GetSchemaVersionsDiffResponseTypeDef(TypedDict):
    Diff: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTagsResponseTypeDef

```python
# GetTagsResponseTypeDef definition

class GetTagsResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkflowRunPropertiesResponseTypeDef

```python
# GetWorkflowRunPropertiesResponseTypeDef definition

class GetWorkflowRunPropertiesResponseTypeDef(TypedDict):
    RunProperties: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBlueprintsResponseTypeDef

```python
# ListBlueprintsResponseTypeDef definition

class ListBlueprintsResponseTypeDef(TypedDict):
    Blueprints: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCrawlersResponseTypeDef

```python
# ListCrawlersResponseTypeDef definition

class ListCrawlersResponseTypeDef(TypedDict):
    CrawlerNames: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDevEndpointsResponseTypeDef

```python
# ListDevEndpointsResponseTypeDef definition

class ListDevEndpointsResponseTypeDef(TypedDict):
    DevEndpointNames: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsResponseTypeDef

```python
# ListJobsResponseTypeDef definition

class ListJobsResponseTypeDef(TypedDict):
    JobNames: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMLTransformsResponseTypeDef

```python
# ListMLTransformsResponseTypeDef definition

class ListMLTransformsResponseTypeDef(TypedDict):
    TransformIds: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTriggersResponseTypeDef

```python
# ListTriggersResponseTypeDef definition

class ListTriggersResponseTypeDef(TypedDict):
    TriggerNames: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkflowsResponseTypeDef

```python
# ListWorkflowsResponseTypeDef definition

class ListWorkflowsResponseTypeDef(TypedDict):
    Workflows: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResponseTypeDef

```python
# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    PolicyHash: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSchemaVersionMetadataResponseTypeDef

```python
# PutSchemaVersionMetadataResponseTypeDef definition

class PutSchemaVersionMetadataResponseTypeDef(TypedDict):
    SchemaArn: str,
    SchemaName: str,
    RegistryName: str,
    LatestVersion: bool,
    VersionNumber: int,
    SchemaVersionId: str,
    MetadataKey: str,
    MetadataValue: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterSchemaVersionResponseTypeDef

```python
# RegisterSchemaVersionResponseTypeDef definition

class RegisterSchemaVersionResponseTypeDef(TypedDict):
    SchemaVersionId: str,
    VersionNumber: int,
    Status: SchemaVersionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SchemaVersionStatusType](./literals.md#schemaversionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveSchemaVersionMetadataResponseTypeDef

```python
# RemoveSchemaVersionMetadataResponseTypeDef definition

class RemoveSchemaVersionMetadataResponseTypeDef(TypedDict):
    SchemaArn: str,
    SchemaName: str,
    RegistryName: str,
    LatestVersion: bool,
    VersionNumber: int,
    SchemaVersionId: str,
    MetadataKey: str,
    MetadataValue: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResumeWorkflowRunResponseTypeDef

```python
# ResumeWorkflowRunResponseTypeDef definition

class ResumeWorkflowRunResponseTypeDef(TypedDict):
    RunId: str,
    NodeIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunStatementResponseTypeDef

```python
# RunStatementResponseTypeDef definition

class RunStatementResponseTypeDef(TypedDict):
    Id: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartBlueprintRunResponseTypeDef

```python
# StartBlueprintRunResponseTypeDef definition

class StartBlueprintRunResponseTypeDef(TypedDict):
    RunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataQualityRuleRecommendationRunResponseTypeDef

```python
# StartDataQualityRuleRecommendationRunResponseTypeDef definition

class StartDataQualityRuleRecommendationRunResponseTypeDef(TypedDict):
    RunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataQualityRulesetEvaluationRunResponseTypeDef

```python
# StartDataQualityRulesetEvaluationRunResponseTypeDef definition

class StartDataQualityRulesetEvaluationRunResponseTypeDef(TypedDict):
    RunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExportLabelsTaskRunResponseTypeDef

```python
# StartExportLabelsTaskRunResponseTypeDef definition

class StartExportLabelsTaskRunResponseTypeDef(TypedDict):
    TaskRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImportLabelsTaskRunResponseTypeDef

```python
# StartImportLabelsTaskRunResponseTypeDef definition

class StartImportLabelsTaskRunResponseTypeDef(TypedDict):
    TaskRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartJobRunResponseTypeDef

```python
# StartJobRunResponseTypeDef definition

class StartJobRunResponseTypeDef(TypedDict):
    JobRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMLEvaluationTaskRunResponseTypeDef

```python
# StartMLEvaluationTaskRunResponseTypeDef definition

class StartMLEvaluationTaskRunResponseTypeDef(TypedDict):
    TaskRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMLLabelingSetGenerationTaskRunResponseTypeDef

```python
# StartMLLabelingSetGenerationTaskRunResponseTypeDef definition

class StartMLLabelingSetGenerationTaskRunResponseTypeDef(TypedDict):
    TaskRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTriggerResponseTypeDef

```python
# StartTriggerResponseTypeDef definition

class StartTriggerResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartWorkflowRunResponseTypeDef

```python
# StartWorkflowRunResponseTypeDef definition

class StartWorkflowRunResponseTypeDef(TypedDict):
    RunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopSessionResponseTypeDef

```python
# StopSessionResponseTypeDef definition

class StopSessionResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopTriggerResponseTypeDef

```python
# StopTriggerResponseTypeDef definition

class StopTriggerResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBlueprintResponseTypeDef

```python
# UpdateBlueprintResponseTypeDef definition

class UpdateBlueprintResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataQualityRulesetResponseTypeDef

```python
# UpdateDataQualityRulesetResponseTypeDef definition

class UpdateDataQualityRulesetResponseTypeDef(TypedDict):
    Name: str,
    Description: str,
    Ruleset: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateJobFromSourceControlResponseTypeDef

```python
# UpdateJobFromSourceControlResponseTypeDef definition

class UpdateJobFromSourceControlResponseTypeDef(TypedDict):
    JobName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateJobResponseTypeDef

```python
# UpdateJobResponseTypeDef definition

class UpdateJobResponseTypeDef(TypedDict):
    JobName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMLTransformResponseTypeDef

```python
# UpdateMLTransformResponseTypeDef definition

class UpdateMLTransformResponseTypeDef(TypedDict):
    TransformId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRegistryResponseTypeDef

```python
# UpdateRegistryResponseTypeDef definition

class UpdateRegistryResponseTypeDef(TypedDict):
    RegistryName: str,
    RegistryArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSchemaResponseTypeDef

```python
# UpdateSchemaResponseTypeDef definition

class UpdateSchemaResponseTypeDef(TypedDict):
    SchemaArn: str,
    SchemaName: str,
    RegistryName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSourceControlFromJobResponseTypeDef

```python
# UpdateSourceControlFromJobResponseTypeDef definition

class UpdateSourceControlFromJobResponseTypeDef(TypedDict):
    JobName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkflowResponseTypeDef

```python
# UpdateWorkflowResponseTypeDef definition

class UpdateWorkflowResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteConnectionResponseTypeDef

```python
# BatchDeleteConnectionResponseTypeDef definition

class BatchDeleteConnectionResponseTypeDef(TypedDict):
    Succeeded: List[str],
    Errors: Dict[str, ErrorDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchStopJobRunErrorTypeDef

```python
# BatchStopJobRunErrorTypeDef definition

class BatchStopJobRunErrorTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
    ErrorDetail: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## BatchUpdatePartitionFailureEntryTypeDef

```python
# BatchUpdatePartitionFailureEntryTypeDef definition

class BatchUpdatePartitionFailureEntryTypeDef(TypedDict):
    PartitionValueList: NotRequired[List[str]],
    ErrorDetail: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## ColumnErrorTypeDef

```python
# ColumnErrorTypeDef definition

class ColumnErrorTypeDef(TypedDict):
    ColumnName: NotRequired[str],
    Error: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## PartitionErrorTypeDef

```python
# PartitionErrorTypeDef definition

class PartitionErrorTypeDef(TypedDict):
    PartitionValues: NotRequired[List[str]],
    ErrorDetail: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## TableErrorTypeDef

```python
# TableErrorTypeDef definition

class TableErrorTypeDef(TypedDict):
    TableName: NotRequired[str],
    ErrorDetail: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## TableVersionErrorTypeDef

```python
# TableVersionErrorTypeDef definition

class TableVersionErrorTypeDef(TypedDict):
    TableName: NotRequired[str],
    VersionId: NotRequired[str],
    ErrorDetail: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## BatchGetCustomEntityTypesResponseTypeDef

```python
# BatchGetCustomEntityTypesResponseTypeDef definition

class BatchGetCustomEntityTypesResponseTypeDef(TypedDict):
    CustomEntityTypes: List[CustomEntityTypeTypeDef],  # (1)
    CustomEntityTypesNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomEntityTypeTypeDef](./type_defs.md#customentitytypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomEntityTypesResponseTypeDef

```python
# ListCustomEntityTypesResponseTypeDef definition

class ListCustomEntityTypesResponseTypeDef(TypedDict):
    CustomEntityTypes: List[CustomEntityTypeTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomEntityTypeTypeDef](./type_defs.md#customentitytypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetDevEndpointsResponseTypeDef

```python
# BatchGetDevEndpointsResponseTypeDef definition

class BatchGetDevEndpointsResponseTypeDef(TypedDict):
    DevEndpoints: List[DevEndpointTypeDef],  # (1)
    DevEndpointsNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DevEndpointTypeDef](./type_defs.md#devendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDevEndpointResponseTypeDef

```python
# GetDevEndpointResponseTypeDef definition

class GetDevEndpointResponseTypeDef(TypedDict):
    DevEndpoint: DevEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DevEndpointTypeDef](./type_defs.md#devendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDevEndpointsResponseTypeDef

```python
# GetDevEndpointsResponseTypeDef definition

class GetDevEndpointsResponseTypeDef(TypedDict):
    DevEndpoints: List[DevEndpointTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DevEndpointTypeDef](./type_defs.md#devendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlueprintRunResponseTypeDef

```python
# GetBlueprintRunResponseTypeDef definition

class GetBlueprintRunResponseTypeDef(TypedDict):
    BlueprintRun: BlueprintRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueprintRunTypeDef](./type_defs.md#blueprintruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlueprintRunsResponseTypeDef

```python
# GetBlueprintRunsResponseTypeDef definition

class GetBlueprintRunsResponseTypeDef(TypedDict):
    BlueprintRuns: List[BlueprintRunTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueprintRunTypeDef](./type_defs.md#blueprintruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BlueprintTypeDef

```python
# BlueprintTypeDef definition

class BlueprintTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    ParameterSpec: NotRequired[str],
    BlueprintLocation: NotRequired[str],
    BlueprintServiceLocation: NotRequired[str],
    Status: NotRequired[BlueprintStatusType],  # (1)
    ErrorMessage: NotRequired[str],
    LastActiveDefinition: NotRequired[LastActiveDefinitionTypeDef],  # (2)
```

1. See [:material-code-brackets: BlueprintStatusType](./literals.md#blueprintstatustype) 
2. See [:material-code-braces: LastActiveDefinitionTypeDef](./type_defs.md#lastactivedefinitiontypedef) 
## GetCatalogImportStatusResponseTypeDef

```python
# GetCatalogImportStatusResponseTypeDef definition

class GetCatalogImportStatusResponseTypeDef(TypedDict):
    ImportStatus: CatalogImportStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CatalogImportStatusTypeDef](./type_defs.md#catalogimportstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CatalogKafkaSourceTypeDef

```python
# CatalogKafkaSourceTypeDef definition

class CatalogKafkaSourceTypeDef(TypedDict):
    Name: str,
    Table: str,
    Database: str,
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    StreamingOptions: NotRequired[KafkaStreamingSourceOptionsTypeDef],  # (1)
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KafkaStreamingSourceOptionsTypeDef](./type_defs.md#kafkastreamingsourceoptionstypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## DirectKafkaSourceTypeDef

```python
# DirectKafkaSourceTypeDef definition

class DirectKafkaSourceTypeDef(TypedDict):
    Name: str,
    StreamingOptions: NotRequired[KafkaStreamingSourceOptionsTypeDef],  # (1)
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KafkaStreamingSourceOptionsTypeDef](./type_defs.md#kafkastreamingsourceoptionstypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## CatalogKinesisSourceTypeDef

```python
# CatalogKinesisSourceTypeDef definition

class CatalogKinesisSourceTypeDef(TypedDict):
    Name: str,
    Table: str,
    Database: str,
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    StreamingOptions: NotRequired[KinesisStreamingSourceOptionsTypeDef],  # (1)
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KinesisStreamingSourceOptionsTypeDef](./type_defs.md#kinesisstreamingsourceoptionstypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## DirectKinesisSourceTypeDef

```python
# DirectKinesisSourceTypeDef definition

class DirectKinesisSourceTypeDef(TypedDict):
    Name: str,
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    StreamingOptions: NotRequired[KinesisStreamingSourceOptionsTypeDef],  # (1)
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KinesisStreamingSourceOptionsTypeDef](./type_defs.md#kinesisstreamingsourceoptionstypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## GovernedCatalogTargetTypeDef

```python
# GovernedCatalogTargetTypeDef definition

class GovernedCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Table: str,
    Database: str,
    PartitionKeys: NotRequired[List[List[str]]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## S3CatalogTargetTypeDef

```python
# S3CatalogTargetTypeDef definition

class S3CatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Table: str,
    Database: str,
    PartitionKeys: NotRequired[List[List[str]]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## S3DeltaCatalogTargetTypeDef

```python
# S3DeltaCatalogTargetTypeDef definition

class S3DeltaCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Table: str,
    Database: str,
    PartitionKeys: NotRequired[List[List[str]]],
    AdditionalOptions: NotRequired[Dict[str, str]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## S3HudiCatalogTargetTypeDef

```python
# S3HudiCatalogTargetTypeDef definition

class S3HudiCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Table: str,
    Database: str,
    AdditionalOptions: Dict[str, str],
    PartitionKeys: NotRequired[List[List[str]]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## ClassifierTypeDef

```python
# ClassifierTypeDef definition

class ClassifierTypeDef(TypedDict):
    GrokClassifier: NotRequired[GrokClassifierTypeDef],  # (1)
    XMLClassifier: NotRequired[XMLClassifierTypeDef],  # (2)
    JsonClassifier: NotRequired[JsonClassifierTypeDef],  # (3)
    CsvClassifier: NotRequired[CsvClassifierTypeDef],  # (4)
```

1. See [:material-code-braces: GrokClassifierTypeDef](./type_defs.md#grokclassifiertypedef) 
2. See [:material-code-braces: XMLClassifierTypeDef](./type_defs.md#xmlclassifiertypedef) 
3. See [:material-code-braces: JsonClassifierTypeDef](./type_defs.md#jsonclassifiertypedef) 
4. See [:material-code-braces: CsvClassifierTypeDef](./type_defs.md#csvclassifiertypedef) 
## CodeGenNodeTypeDef

```python
# CodeGenNodeTypeDef definition

class CodeGenNodeTypeDef(TypedDict):
    Id: str,
    NodeType: str,
    Args: Sequence[CodeGenNodeArgTypeDef],  # (1)
    LineNumber: NotRequired[int],
```

1. See [:material-code-braces: CodeGenNodeArgTypeDef](./type_defs.md#codegennodeargtypedef) 
## LocationTypeDef

```python
# LocationTypeDef definition

class LocationTypeDef(TypedDict):
    Jdbc: NotRequired[Sequence[CodeGenNodeArgTypeDef]],  # (1)
    S3: NotRequired[Sequence[CodeGenNodeArgTypeDef]],  # (1)
    DynamoDB: NotRequired[Sequence[CodeGenNodeArgTypeDef]],  # (1)
```

1. See [:material-code-braces: CodeGenNodeArgTypeDef](./type_defs.md#codegennodeargtypedef) 
2. See [:material-code-braces: CodeGenNodeArgTypeDef](./type_defs.md#codegennodeargtypedef) 
3. See [:material-code-braces: CodeGenNodeArgTypeDef](./type_defs.md#codegennodeargtypedef) 
## PredicateTypeDef

```python
# PredicateTypeDef definition

class PredicateTypeDef(TypedDict):
    Logical: NotRequired[LogicalType],  # (1)
    Conditions: NotRequired[List[ConditionTypeDef]],  # (2)
```

1. See [:material-code-brackets: LogicalType](./literals.md#logicaltype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
## FindMatchesMetricsTypeDef

```python
# FindMatchesMetricsTypeDef definition

class FindMatchesMetricsTypeDef(TypedDict):
    AreaUnderPRCurve: NotRequired[float],
    Precision: NotRequired[float],
    Recall: NotRequired[float],
    F1: NotRequired[float],
    ConfusionMatrix: NotRequired[ConfusionMatrixTypeDef],  # (1)
    ColumnImportances: NotRequired[List[ColumnImportanceTypeDef]],  # (2)
```

1. See [:material-code-braces: ConfusionMatrixTypeDef](./type_defs.md#confusionmatrixtypedef) 
2. See [:material-code-braces: ColumnImportanceTypeDef](./type_defs.md#columnimportancetypedef) 
## ConnectionInputTypeDef

```python
# ConnectionInputTypeDef definition

class ConnectionInputTypeDef(TypedDict):
    Name: str,
    ConnectionType: ConnectionTypeType,  # (1)
    ConnectionProperties: Mapping[ConnectionPropertyKeyType, str],  # (2)
    Description: NotRequired[str],
    MatchCriteria: NotRequired[Sequence[str]],
    PhysicalConnectionRequirements: NotRequired[PhysicalConnectionRequirementsTypeDef],  # (3)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-brackets: ConnectionPropertyKeyType](./literals.md#connectionpropertykeytype) 
3. See [:material-code-braces: PhysicalConnectionRequirementsTypeDef](./type_defs.md#physicalconnectionrequirementstypedef) 
## ConnectionTypeDef

```python
# ConnectionTypeDef definition

class ConnectionTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    ConnectionType: NotRequired[ConnectionTypeType],  # (1)
    MatchCriteria: NotRequired[List[str]],
    ConnectionProperties: NotRequired[Dict[ConnectionPropertyKeyType, str]],  # (2)
    PhysicalConnectionRequirements: NotRequired[PhysicalConnectionRequirementsTypeDef],  # (3)
    CreationTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    LastUpdatedBy: NotRequired[str],
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-brackets: ConnectionPropertyKeyType](./literals.md#connectionpropertykeytype) 
3. See [:material-code-braces: PhysicalConnectionRequirementsTypeDef](./type_defs.md#physicalconnectionrequirementstypedef) 
## CrawlerNodeDetailsTypeDef

```python
# CrawlerNodeDetailsTypeDef definition

class CrawlerNodeDetailsTypeDef(TypedDict):
    Crawls: NotRequired[List[CrawlTypeDef]],  # (1)
```

1. See [:material-code-braces: CrawlTypeDef](./type_defs.md#crawltypedef) 
## ListCrawlsResponseTypeDef

```python
# ListCrawlsResponseTypeDef definition

class ListCrawlsResponseTypeDef(TypedDict):
    Crawls: List[CrawlerHistoryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CrawlerHistoryTypeDef](./type_defs.md#crawlerhistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCrawlerMetricsResponseTypeDef

```python
# GetCrawlerMetricsResponseTypeDef definition

class GetCrawlerMetricsResponseTypeDef(TypedDict):
    CrawlerMetricsList: List[CrawlerMetricsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CrawlerMetricsTypeDef](./type_defs.md#crawlermetricstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CrawlerTargetsTypeDef

```python
# CrawlerTargetsTypeDef definition

class CrawlerTargetsTypeDef(TypedDict):
    S3Targets: NotRequired[List[S3TargetTypeDef]],  # (1)
    JdbcTargets: NotRequired[List[JdbcTargetTypeDef]],  # (2)
    MongoDBTargets: NotRequired[List[MongoDBTargetTypeDef]],  # (3)
    DynamoDBTargets: NotRequired[List[DynamoDBTargetTypeDef]],  # (4)
    CatalogTargets: NotRequired[List[CatalogTargetTypeDef]],  # (5)
    DeltaTargets: NotRequired[List[DeltaTargetTypeDef]],  # (6)
    IcebergTargets: NotRequired[List[IcebergTargetTypeDef]],  # (7)
    HudiTargets: NotRequired[List[HudiTargetTypeDef]],  # (8)
```

1. See [:material-code-braces: S3TargetTypeDef](./type_defs.md#s3targettypedef) 
2. See [:material-code-braces: JdbcTargetTypeDef](./type_defs.md#jdbctargettypedef) 
3. See [:material-code-braces: MongoDBTargetTypeDef](./type_defs.md#mongodbtargettypedef) 
4. See [:material-code-braces: DynamoDBTargetTypeDef](./type_defs.md#dynamodbtargettypedef) 
5. See [:material-code-braces: CatalogTargetTypeDef](./type_defs.md#catalogtargettypedef) 
6. See [:material-code-braces: DeltaTargetTypeDef](./type_defs.md#deltatargettypedef) 
7. See [:material-code-braces: IcebergTargetTypeDef](./type_defs.md#icebergtargettypedef) 
8. See [:material-code-braces: HudiTargetTypeDef](./type_defs.md#huditargettypedef) 
## ListCrawlsRequestRequestTypeDef

```python
# ListCrawlsRequestRequestTypeDef definition

class ListCrawlsRequestRequestTypeDef(TypedDict):
    CrawlerName: str,
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[CrawlsFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CrawlsFilterTypeDef](./type_defs.md#crawlsfiltertypedef) 
## CreateClassifierRequestRequestTypeDef

```python
# CreateClassifierRequestRequestTypeDef definition

class CreateClassifierRequestRequestTypeDef(TypedDict):
    GrokClassifier: NotRequired[CreateGrokClassifierRequestTypeDef],  # (1)
    XMLClassifier: NotRequired[CreateXMLClassifierRequestTypeDef],  # (2)
    JsonClassifier: NotRequired[CreateJsonClassifierRequestTypeDef],  # (3)
    CsvClassifier: NotRequired[CreateCsvClassifierRequestTypeDef],  # (4)
```

1. See [:material-code-braces: CreateGrokClassifierRequestTypeDef](./type_defs.md#creategrokclassifierrequesttypedef) 
2. See [:material-code-braces: CreateXMLClassifierRequestTypeDef](./type_defs.md#createxmlclassifierrequesttypedef) 
3. See [:material-code-braces: CreateJsonClassifierRequestTypeDef](./type_defs.md#createjsonclassifierrequesttypedef) 
4. See [:material-code-braces: CreateCsvClassifierRequestTypeDef](./type_defs.md#createcsvclassifierrequesttypedef) 
## CreateDataQualityRulesetRequestRequestTypeDef

```python
# CreateDataQualityRulesetRequestRequestTypeDef definition

class CreateDataQualityRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
    Ruleset: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    TargetTable: NotRequired[DataQualityTargetTableTypeDef],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: DataQualityTargetTableTypeDef](./type_defs.md#dataqualitytargettabletypedef) 
## DataQualityRulesetListDetailsTypeDef

```python
# DataQualityRulesetListDetailsTypeDef definition

class DataQualityRulesetListDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    TargetTable: NotRequired[DataQualityTargetTableTypeDef],  # (1)
    RecommendationRunId: NotRequired[str],
    RuleCount: NotRequired[int],
```

1. See [:material-code-braces: DataQualityTargetTableTypeDef](./type_defs.md#dataqualitytargettabletypedef) 
## GetDataQualityRulesetResponseTypeDef

```python
# GetDataQualityRulesetResponseTypeDef definition

class GetDataQualityRulesetResponseTypeDef(TypedDict):
    Name: str,
    Description: str,
    Ruleset: str,
    TargetTable: DataQualityTargetTableTypeDef,  # (1)
    CreatedOn: datetime,
    LastModifiedOn: datetime,
    RecommendationRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataQualityTargetTableTypeDef](./type_defs.md#dataqualitytargettabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    GlueTable: GlueTableTypeDef,  # (1)
```

1. See [:material-code-braces: GlueTableTypeDef](./type_defs.md#gluetabletypedef) 
## CreatePartitionIndexRequestRequestTypeDef

```python
# CreatePartitionIndexRequestRequestTypeDef definition

class CreatePartitionIndexRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionIndex: PartitionIndexTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionIndexTypeDef](./type_defs.md#partitionindextypedef) 
## CreateSchemaInputRequestTypeDef

```python
# CreateSchemaInputRequestTypeDef definition

class CreateSchemaInputRequestTypeDef(TypedDict):
    SchemaName: str,
    DataFormat: DataFormatType,  # (1)
    RegistryId: NotRequired[RegistryIdTypeDef],  # (2)
    Compatibility: NotRequired[CompatibilityType],  # (3)
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    SchemaDefinition: NotRequired[str],
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
3. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
## DeleteRegistryInputRequestTypeDef

```python
# DeleteRegistryInputRequestTypeDef definition

class DeleteRegistryInputRequestTypeDef(TypedDict):
    RegistryId: RegistryIdTypeDef,  # (1)
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
## GetRegistryInputRequestTypeDef

```python
# GetRegistryInputRequestTypeDef definition

class GetRegistryInputRequestTypeDef(TypedDict):
    RegistryId: RegistryIdTypeDef,  # (1)
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
## ListSchemasInputRequestTypeDef

```python
# ListSchemasInputRequestTypeDef definition

class ListSchemasInputRequestTypeDef(TypedDict):
    RegistryId: NotRequired[RegistryIdTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
## UpdateRegistryInputRequestTypeDef

```python
# UpdateRegistryInputRequestTypeDef definition

class UpdateRegistryInputRequestTypeDef(TypedDict):
    RegistryId: RegistryIdTypeDef,  # (1)
    Description: str,
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
## CreateSessionRequestRequestTypeDef

```python
# CreateSessionRequestRequestTypeDef definition

class CreateSessionRequestRequestTypeDef(TypedDict):
    Id: str,
    Role: str,
    Command: SessionCommandTypeDef,  # (1)
    Description: NotRequired[str],
    Timeout: NotRequired[int],
    IdleTimeout: NotRequired[int],
    DefaultArguments: NotRequired[Mapping[str, str]],
    Connections: NotRequired[ConnectionsListTypeDef],  # (2)
    MaxCapacity: NotRequired[float],
    NumberOfWorkers: NotRequired[int],
    WorkerType: NotRequired[WorkerTypeType],  # (3)
    SecurityConfiguration: NotRequired[str],
    GlueVersion: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    RequestOrigin: NotRequired[str],
```

1. See [:material-code-braces: SessionCommandTypeDef](./type_defs.md#sessioncommandtypedef) 
2. See [:material-code-braces: ConnectionsListTypeDef](./type_defs.md#connectionslisttypedef) 
3. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
## SessionTypeDef

```python
# SessionTypeDef definition

class SessionTypeDef(TypedDict):
    Id: NotRequired[str],
    CreatedOn: NotRequired[datetime],
    Status: NotRequired[SessionStatusType],  # (1)
    ErrorMessage: NotRequired[str],
    Description: NotRequired[str],
    Role: NotRequired[str],
    Command: NotRequired[SessionCommandTypeDef],  # (2)
    DefaultArguments: NotRequired[Dict[str, str]],
    Connections: NotRequired[ConnectionsListTypeDef],  # (3)
    Progress: NotRequired[float],
    MaxCapacity: NotRequired[float],
    SecurityConfiguration: NotRequired[str],
    GlueVersion: NotRequired[str],
```

1. See [:material-code-brackets: SessionStatusType](./literals.md#sessionstatustype) 
2. See [:material-code-braces: SessionCommandTypeDef](./type_defs.md#sessioncommandtypedef) 
3. See [:material-code-braces: ConnectionsListTypeDef](./type_defs.md#connectionslisttypedef) 
## EvaluateDataQualityMultiFrameTypeDef

```python
# EvaluateDataQualityMultiFrameTypeDef definition

class EvaluateDataQualityMultiFrameTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Ruleset: str,
    AdditionalDataSources: NotRequired[Dict[str, str]],
    PublishingOptions: NotRequired[DQResultsPublishingOptionsTypeDef],  # (1)
    AdditionalOptions: NotRequired[Dict[AdditionalOptionKeysType, str]],  # (2)
    StopJobOnFailureOptions: NotRequired[DQStopJobOnFailureOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: DQResultsPublishingOptionsTypeDef](./type_defs.md#dqresultspublishingoptionstypedef) 
2. See [:material-code-brackets: AdditionalOptionKeysType](./literals.md#additionaloptionkeystype) 
3. See [:material-code-braces: DQStopJobOnFailureOptionsTypeDef](./type_defs.md#dqstopjobonfailureoptionstypedef) 
## EvaluateDataQualityTypeDef

```python
# EvaluateDataQualityTypeDef definition

class EvaluateDataQualityTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Ruleset: str,
    Output: NotRequired[DQTransformOutputType],  # (1)
    PublishingOptions: NotRequired[DQResultsPublishingOptionsTypeDef],  # (2)
    StopJobOnFailureOptions: NotRequired[DQStopJobOnFailureOptionsTypeDef],  # (3)
```

1. See [:material-code-brackets: DQTransformOutputType](./literals.md#dqtransformoutputtype) 
2. See [:material-code-braces: DQResultsPublishingOptionsTypeDef](./type_defs.md#dqresultspublishingoptionstypedef) 
3. See [:material-code-braces: DQStopJobOnFailureOptionsTypeDef](./type_defs.md#dqstopjobonfailureoptionstypedef) 
## DataCatalogEncryptionSettingsTypeDef

```python
# DataCatalogEncryptionSettingsTypeDef definition

class DataCatalogEncryptionSettingsTypeDef(TypedDict):
    EncryptionAtRest: NotRequired[EncryptionAtRestTypeDef],  # (1)
    ConnectionPasswordEncryption: NotRequired[ConnectionPasswordEncryptionTypeDef],  # (2)
```

1. See [:material-code-braces: EncryptionAtRestTypeDef](./type_defs.md#encryptionatresttypedef) 
2. See [:material-code-braces: ConnectionPasswordEncryptionTypeDef](./type_defs.md#connectionpasswordencryptiontypedef) 
## PrincipalPermissionsTypeDef

```python
# PrincipalPermissionsTypeDef definition

class PrincipalPermissionsTypeDef(TypedDict):
    Principal: NotRequired[DataLakePrincipalTypeDef],  # (1)
    Permissions: NotRequired[Sequence[PermissionType]],  # (2)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## DataQualityRulesetFilterCriteriaTypeDef

```python
# DataQualityRulesetFilterCriteriaTypeDef definition

class DataQualityRulesetFilterCriteriaTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    CreatedBefore: NotRequired[Union[datetime, str]],
    CreatedAfter: NotRequired[Union[datetime, str]],
    LastModifiedBefore: NotRequired[Union[datetime, str]],
    LastModifiedAfter: NotRequired[Union[datetime, str]],
    TargetTable: NotRequired[DataQualityTargetTableTypeDef],  # (1)
```

1. See [:material-code-braces: DataQualityTargetTableTypeDef](./type_defs.md#dataqualitytargettabletypedef) 
## GetTableRequestRequestTypeDef

```python
# GetTableRequestRequestTypeDef definition

class GetTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    Name: str,
    CatalogId: NotRequired[str],
    TransactionId: NotRequired[str],
    QueryAsOfTime: NotRequired[Union[datetime, str]],
```

## GetTablesRequestRequestTypeDef

```python
# GetTablesRequestRequestTypeDef definition

class GetTablesRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    CatalogId: NotRequired[str],
    Expression: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    TransactionId: NotRequired[str],
    QueryAsOfTime: NotRequired[Union[datetime, str]],
```

## TaskRunFilterCriteriaTypeDef

```python
# TaskRunFilterCriteriaTypeDef definition

class TaskRunFilterCriteriaTypeDef(TypedDict):
    TaskRunType: NotRequired[TaskTypeType],  # (1)
    Status: NotRequired[TaskStatusTypeType],  # (2)
    StartedBefore: NotRequired[Union[datetime, str]],
    StartedAfter: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: TaskTypeType](./literals.md#tasktypetype) 
2. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
## NullValueFieldTypeDef

```python
# NullValueFieldTypeDef definition

class NullValueFieldTypeDef(TypedDict):
    Value: str,
    Datatype: DatatypeTypeDef,  # (1)
```

1. See [:material-code-braces: DatatypeTypeDef](./type_defs.md#datatypetypedef) 
## DecimalColumnStatisticsDataTypeDef

```python
# DecimalColumnStatisticsDataTypeDef definition

class DecimalColumnStatisticsDataTypeDef(TypedDict):
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
    MinimumValue: NotRequired[DecimalNumberTypeDef],  # (1)
    MaximumValue: NotRequired[DecimalNumberTypeDef],  # (1)
```

1. See [:material-code-braces: DecimalNumberTypeDef](./type_defs.md#decimalnumbertypedef) 
2. See [:material-code-braces: DecimalNumberTypeDef](./type_defs.md#decimalnumbertypedef) 
## DeleteSchemaInputRequestTypeDef

```python
# DeleteSchemaInputRequestTypeDef definition

class DeleteSchemaInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## DeleteSchemaVersionsInputRequestTypeDef

```python
# DeleteSchemaVersionsInputRequestTypeDef definition

class DeleteSchemaVersionsInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    Versions: str,
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## GetSchemaByDefinitionInputRequestTypeDef

```python
# GetSchemaByDefinitionInputRequestTypeDef definition

class GetSchemaByDefinitionInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    SchemaDefinition: str,
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## GetSchemaInputRequestTypeDef

```python
# GetSchemaInputRequestTypeDef definition

class GetSchemaInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## ListSchemaVersionsInputRequestTypeDef

```python
# ListSchemaVersionsInputRequestTypeDef definition

class ListSchemaVersionsInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## RegisterSchemaVersionInputRequestTypeDef

```python
# RegisterSchemaVersionInputRequestTypeDef definition

class RegisterSchemaVersionInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    SchemaDefinition: str,
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## SchemaReferenceTypeDef

```python
# SchemaReferenceTypeDef definition

class SchemaReferenceTypeDef(TypedDict):
    SchemaId: NotRequired[SchemaIdTypeDef],  # (1)
    SchemaVersionId: NotRequired[str],
    SchemaVersionNumber: NotRequired[int],
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## UpdateDevEndpointRequestRequestTypeDef

```python
# UpdateDevEndpointRequestRequestTypeDef definition

class UpdateDevEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
    PublicKey: NotRequired[str],
    AddPublicKeys: NotRequired[Sequence[str]],
    DeletePublicKeys: NotRequired[Sequence[str]],
    CustomLibraries: NotRequired[DevEndpointCustomLibrariesTypeDef],  # (1)
    UpdateEtlLibraries: NotRequired[bool],
    DeleteArguments: NotRequired[Sequence[str]],
    AddArguments: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DevEndpointCustomLibrariesTypeDef](./type_defs.md#devendpointcustomlibrariestypedef) 
## S3DeltaDirectTargetTypeDef

```python
# S3DeltaDirectTargetTypeDef definition

class S3DeltaDirectTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Path: str,
    Compression: DeltaTargetCompressionTypeType,  # (1)
    Format: TargetFormatType,  # (2)
    PartitionKeys: NotRequired[List[List[str]]],
    AdditionalOptions: NotRequired[Dict[str, str]],
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (3)
```

1. See [:material-code-brackets: DeltaTargetCompressionTypeType](./literals.md#deltatargetcompressiontypetype) 
2. See [:material-code-brackets: TargetFormatType](./literals.md#targetformattype) 
3. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## S3DirectTargetTypeDef

```python
# S3DirectTargetTypeDef definition

class S3DirectTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Path: str,
    Format: TargetFormatType,  # (1)
    PartitionKeys: NotRequired[List[List[str]]],
    Compression: NotRequired[str],
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (2)
```

1. See [:material-code-brackets: TargetFormatType](./literals.md#targetformattype) 
2. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## S3GlueParquetTargetTypeDef

```python
# S3GlueParquetTargetTypeDef definition

class S3GlueParquetTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Path: str,
    PartitionKeys: NotRequired[List[List[str]]],
    Compression: NotRequired[ParquetCompressionTypeType],  # (1)
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (2)
```

1. See [:material-code-brackets: ParquetCompressionTypeType](./literals.md#parquetcompressiontypetype) 
2. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## S3HudiDirectTargetTypeDef

```python
# S3HudiDirectTargetTypeDef definition

class S3HudiDirectTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Path: str,
    Compression: HudiTargetCompressionTypeType,  # (1)
    Format: TargetFormatType,  # (2)
    AdditionalOptions: Dict[str, str],
    PartitionKeys: NotRequired[List[List[str]]],
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (3)
```

1. See [:material-code-brackets: HudiTargetCompressionTypeType](./literals.md#huditargetcompressiontypetype) 
2. See [:material-code-brackets: TargetFormatType](./literals.md#targetformattype) 
3. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    S3Encryption: NotRequired[Sequence[S3EncryptionTypeDef]],  # (1)
    CloudWatchEncryption: NotRequired[CloudWatchEncryptionTypeDef],  # (2)
    JobBookmarksEncryption: NotRequired[JobBookmarksEncryptionTypeDef],  # (3)
```

1. See [:material-code-braces: S3EncryptionTypeDef](./type_defs.md#s3encryptiontypedef) 
2. See [:material-code-braces: CloudWatchEncryptionTypeDef](./type_defs.md#cloudwatchencryptiontypedef) 
3. See [:material-code-braces: JobBookmarksEncryptionTypeDef](./type_defs.md#jobbookmarksencryptiontypedef) 
## SchemaVersionErrorItemTypeDef

```python
# SchemaVersionErrorItemTypeDef definition

class SchemaVersionErrorItemTypeDef(TypedDict):
    VersionNumber: NotRequired[int],
    ErrorDetails: NotRequired[ErrorDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## FilterExpressionTypeDef

```python
# FilterExpressionTypeDef definition

class FilterExpressionTypeDef(TypedDict):
    Operation: FilterOperationType,  # (1)
    Values: List[FilterValueTypeDef],  # (2)
    Negated: NotRequired[bool],
```

1. See [:material-code-brackets: FilterOperationType](./literals.md#filteroperationtype) 
2. See [:material-code-braces: FilterValueTypeDef](./type_defs.md#filtervaluetypedef) 
## TransformParametersTypeDef

```python
# TransformParametersTypeDef definition

class TransformParametersTypeDef(TypedDict):
    TransformType: TransformTypeType,  # (1)
    FindMatchesParameters: NotRequired[FindMatchesParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: TransformTypeType](./literals.md#transformtypetype) 
2. See [:material-code-braces: FindMatchesParametersTypeDef](./type_defs.md#findmatchesparameterstypedef) 
## GetClassifiersRequestGetClassifiersPaginateTypeDef

```python
# GetClassifiersRequestGetClassifiersPaginateTypeDef definition

class GetClassifiersRequestGetClassifiersPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef

```python
# GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef definition

class GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef(TypedDict):
    CrawlerNameList: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetCrawlersRequestGetCrawlersPaginateTypeDef

```python
# GetCrawlersRequestGetCrawlersPaginateTypeDef definition

class GetCrawlersRequestGetCrawlersPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDatabasesRequestGetDatabasesPaginateTypeDef

```python
# GetDatabasesRequestGetDatabasesPaginateTypeDef definition

class GetDatabasesRequestGetDatabasesPaginateTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    ResourceShareType: NotRequired[ResourceShareTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef

```python
# GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef definition

class GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetJobRunsRequestGetJobRunsPaginateTypeDef

```python
# GetJobRunsRequestGetJobRunsPaginateTypeDef definition

class GetJobRunsRequestGetJobRunsPaginateTypeDef(TypedDict):
    JobName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetJobsRequestGetJobsPaginateTypeDef

```python
# GetJobsRequestGetJobsPaginateTypeDef definition

class GetJobsRequestGetJobsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef

```python
# GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef definition

class GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef

```python
# GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef definition

class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef

```python
# GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef definition

class GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTableVersionsRequestGetTableVersionsPaginateTypeDef

```python
# GetTableVersionsRequestGetTableVersionsPaginateTypeDef definition

class GetTableVersionsRequestGetTableVersionsPaginateTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTablesRequestGetTablesPaginateTypeDef

```python
# GetTablesRequestGetTablesPaginateTypeDef definition

class GetTablesRequestGetTablesPaginateTypeDef(TypedDict):
    DatabaseName: str,
    CatalogId: NotRequired[str],
    Expression: NotRequired[str],
    TransactionId: NotRequired[str],
    QueryAsOfTime: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTriggersRequestGetTriggersPaginateTypeDef

```python
# GetTriggersRequestGetTriggersPaginateTypeDef definition

class GetTriggersRequestGetTriggersPaginateTypeDef(TypedDict):
    DependentJobName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef

```python
# GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef definition

class GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef(TypedDict):
    Pattern: str,
    CatalogId: NotRequired[str],
    DatabaseName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRegistriesInputListRegistriesPaginateTypeDef

```python
# ListRegistriesInputListRegistriesPaginateTypeDef definition

class ListRegistriesInputListRegistriesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef

```python
# ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef definition

class ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchemasInputListSchemasPaginateTypeDef

```python
# ListSchemasInputListSchemasPaginateTypeDef definition

class ListSchemasInputListSchemasPaginateTypeDef(TypedDict):
    RegistryId: NotRequired[RegistryIdTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetConnectionsRequestGetConnectionsPaginateTypeDef

```python
# GetConnectionsRequestGetConnectionsPaginateTypeDef definition

class GetConnectionsRequestGetConnectionsPaginateTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    Filter: NotRequired[GetConnectionsFilterTypeDef],  # (1)
    HidePassword: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: GetConnectionsFilterTypeDef](./type_defs.md#getconnectionsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetConnectionsRequestRequestTypeDef

```python
# GetConnectionsRequestRequestTypeDef definition

class GetConnectionsRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    Filter: NotRequired[GetConnectionsFilterTypeDef],  # (1)
    HidePassword: NotRequired[bool],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: GetConnectionsFilterTypeDef](./type_defs.md#getconnectionsfiltertypedef) 
## GetJobBookmarkResponseTypeDef

```python
# GetJobBookmarkResponseTypeDef definition

class GetJobBookmarkResponseTypeDef(TypedDict):
    JobBookmarkEntry: JobBookmarkEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobBookmarkEntryTypeDef](./type_defs.md#jobbookmarkentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetJobBookmarkResponseTypeDef

```python
# ResetJobBookmarkResponseTypeDef definition

class ResetJobBookmarkResponseTypeDef(TypedDict):
    JobBookmarkEntry: JobBookmarkEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobBookmarkEntryTypeDef](./type_defs.md#jobbookmarkentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransformFilterCriteriaTypeDef

```python
# TransformFilterCriteriaTypeDef definition

class TransformFilterCriteriaTypeDef(TypedDict):
    Name: NotRequired[str],
    TransformType: NotRequired[TransformTypeType],  # (1)
    Status: NotRequired[TransformStatusTypeType],  # (2)
    GlueVersion: NotRequired[str],
    CreatedBefore: NotRequired[Union[datetime, str]],
    CreatedAfter: NotRequired[Union[datetime, str]],
    LastModifiedBefore: NotRequired[Union[datetime, str]],
    LastModifiedAfter: NotRequired[Union[datetime, str]],
    Schema: NotRequired[Sequence[SchemaColumnTypeDef]],  # (3)
```

1. See [:material-code-brackets: TransformTypeType](./literals.md#transformtypetype) 
2. See [:material-code-brackets: TransformStatusTypeType](./literals.md#transformstatustypetype) 
3. See [:material-code-braces: SchemaColumnTypeDef](./type_defs.md#schemacolumntypedef) 
## GetMappingResponseTypeDef

```python
# GetMappingResponseTypeDef definition

class GetMappingResponseTypeDef(TypedDict):
    Mapping: List[MappingEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MappingEntryTypeDef](./type_defs.md#mappingentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPartitionsRequestGetPartitionsPaginateTypeDef

```python
# GetPartitionsRequestGetPartitionsPaginateTypeDef definition

class GetPartitionsRequestGetPartitionsPaginateTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    Expression: NotRequired[str],
    Segment: NotRequired[SegmentTypeDef],  # (1)
    ExcludeColumnSchema: NotRequired[bool],
    TransactionId: NotRequired[str],
    QueryAsOfTime: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetPartitionsRequestRequestTypeDef

```python
# GetPartitionsRequestRequestTypeDef definition

class GetPartitionsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    Expression: NotRequired[str],
    NextToken: NotRequired[str],
    Segment: NotRequired[SegmentTypeDef],  # (1)
    MaxResults: NotRequired[int],
    ExcludeColumnSchema: NotRequired[bool],
    TransactionId: NotRequired[str],
    QueryAsOfTime: NotRequired[Union[datetime, str]],
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
## GetUnfilteredPartitionsMetadataRequestRequestTypeDef

```python
# GetUnfilteredPartitionsMetadataRequestRequestTypeDef definition

class GetUnfilteredPartitionsMetadataRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    SupportedPermissionTypes: Sequence[PermissionTypeType],  # (1)
    Expression: NotRequired[str],
    AuditContext: NotRequired[AuditContextTypeDef],  # (2)
    NextToken: NotRequired[str],
    Segment: NotRequired[SegmentTypeDef],  # (3)
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
3. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
## GetResourcePoliciesResponseTypeDef

```python
# GetResourcePoliciesResponseTypeDef definition

class GetResourcePoliciesResponseTypeDef(TypedDict):
    GetResourcePoliciesResponseList: List[GluePolicyTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GluePolicyTypeDef](./type_defs.md#gluepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaVersionInputRequestTypeDef

```python
# GetSchemaVersionInputRequestTypeDef definition

class GetSchemaVersionInputRequestTypeDef(TypedDict):
    SchemaId: NotRequired[SchemaIdTypeDef],  # (1)
    SchemaVersionId: NotRequired[str],
    SchemaVersionNumber: NotRequired[SchemaVersionNumberTypeDef],  # (2)
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
## GetSchemaVersionsDiffInputRequestTypeDef

```python
# GetSchemaVersionsDiffInputRequestTypeDef definition

class GetSchemaVersionsDiffInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    FirstSchemaVersionNumber: SchemaVersionNumberTypeDef,  # (2)
    SecondSchemaVersionNumber: SchemaVersionNumberTypeDef,  # (2)
    SchemaDiffType: SchemaDiffTypeType,  # (4)
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
3. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
4. See [:material-code-brackets: SchemaDiffTypeType](./literals.md#schemadifftypetype) 
## UpdateSchemaInputRequestTypeDef

```python
# UpdateSchemaInputRequestTypeDef definition

class UpdateSchemaInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    SchemaVersionNumber: NotRequired[SchemaVersionNumberTypeDef],  # (2)
    Compatibility: NotRequired[CompatibilityType],  # (3)
    Description: NotRequired[str],
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
3. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
## GlueSchemaTypeDef

```python
# GlueSchemaTypeDef definition

class GlueSchemaTypeDef(TypedDict):
    Columns: NotRequired[List[GlueStudioSchemaColumnTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueStudioSchemaColumnTypeDef](./type_defs.md#gluestudioschemacolumntypedef) 
## GovernedCatalogSourceTypeDef

```python
# GovernedCatalogSourceTypeDef definition

class GovernedCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    PartitionPredicate: NotRequired[str],
    AdditionalOptions: NotRequired[S3SourceAdditionalOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: S3SourceAdditionalOptionsTypeDef](./type_defs.md#s3sourceadditionaloptionstypedef) 
## S3CatalogSourceTypeDef

```python
# S3CatalogSourceTypeDef definition

class S3CatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    PartitionPredicate: NotRequired[str],
    AdditionalOptions: NotRequired[S3SourceAdditionalOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: S3SourceAdditionalOptionsTypeDef](./type_defs.md#s3sourceadditionaloptionstypedef) 
## OpenTableFormatInputTypeDef

```python
# OpenTableFormatInputTypeDef definition

class OpenTableFormatInputTypeDef(TypedDict):
    IcebergInput: NotRequired[IcebergInputTypeDef],  # (1)
```

1. See [:material-code-braces: IcebergInputTypeDef](./type_defs.md#iceberginputtypedef) 
## JobRunTypeDef

```python
# JobRunTypeDef definition

class JobRunTypeDef(TypedDict):
    Id: NotRequired[str],
    Attempt: NotRequired[int],
    PreviousRunId: NotRequired[str],
    TriggerName: NotRequired[str],
    JobName: NotRequired[str],
    StartedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    JobRunState: NotRequired[JobRunStateType],  # (1)
    Arguments: NotRequired[Dict[str, str]],
    ErrorMessage: NotRequired[str],
    PredecessorRuns: NotRequired[List[PredecessorTypeDef]],  # (2)
    AllocatedCapacity: NotRequired[int],
    ExecutionTime: NotRequired[int],
    Timeout: NotRequired[int],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (3)
    NumberOfWorkers: NotRequired[int],
    SecurityConfiguration: NotRequired[str],
    LogGroupName: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (4)
    GlueVersion: NotRequired[str],
    DPUSeconds: NotRequired[float],
    ExecutionClass: NotRequired[ExecutionClassType],  # (5)
```

1. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
2. See [:material-code-braces: PredecessorTypeDef](./type_defs.md#predecessortypedef) 
3. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
4. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
5. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
## JoinTypeDef

```python
# JoinTypeDef definition

class JoinTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    JoinType: JoinTypeType,  # (1)
    Columns: List[JoinColumnTypeDef],  # (2)
```

1. See [:material-code-brackets: JoinTypeType](./literals.md#jointypetype) 
2. See [:material-code-braces: JoinColumnTypeDef](./type_defs.md#joincolumntypedef) 
## TaskRunPropertiesTypeDef

```python
# TaskRunPropertiesTypeDef definition

class TaskRunPropertiesTypeDef(TypedDict):
    TaskType: NotRequired[TaskTypeType],  # (1)
    ImportLabelsTaskRunProperties: NotRequired[ImportLabelsTaskRunPropertiesTypeDef],  # (2)
    ExportLabelsTaskRunProperties: NotRequired[ExportLabelsTaskRunPropertiesTypeDef],  # (3)
    LabelingSetGenerationTaskRunProperties: NotRequired[LabelingSetGenerationTaskRunPropertiesTypeDef],  # (4)
    FindMatchesTaskRunProperties: NotRequired[FindMatchesTaskRunPropertiesTypeDef],  # (5)
```

1. See [:material-code-brackets: TaskTypeType](./literals.md#tasktypetype) 
2. See [:material-code-braces: ImportLabelsTaskRunPropertiesTypeDef](./type_defs.md#importlabelstaskrunpropertiestypedef) 
3. See [:material-code-braces: ExportLabelsTaskRunPropertiesTypeDef](./type_defs.md#exportlabelstaskrunpropertiestypedef) 
4. See [:material-code-braces: LabelingSetGenerationTaskRunPropertiesTypeDef](./type_defs.md#labelingsetgenerationtaskrunpropertiestypedef) 
5. See [:material-code-braces: FindMatchesTaskRunPropertiesTypeDef](./type_defs.md#findmatchestaskrunpropertiestypedef) 
## ListRegistriesResponseTypeDef

```python
# ListRegistriesResponseTypeDef definition

class ListRegistriesResponseTypeDef(TypedDict):
    Registries: List[RegistryListItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegistryListItemTypeDef](./type_defs.md#registrylistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemaVersionsResponseTypeDef

```python
# ListSchemaVersionsResponseTypeDef definition

class ListSchemaVersionsResponseTypeDef(TypedDict):
    Schemas: List[SchemaVersionListItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaVersionListItemTypeDef](./type_defs.md#schemaversionlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemasResponseTypeDef

```python
# ListSchemasResponseTypeDef definition

class ListSchemasResponseTypeDef(TypedDict):
    Schemas: List[SchemaListItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaListItemTypeDef](./type_defs.md#schemalistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransformEncryptionTypeDef

```python
# TransformEncryptionTypeDef definition

class TransformEncryptionTypeDef(TypedDict):
    MlUserDataEncryption: NotRequired[MLUserDataEncryptionTypeDef],  # (1)
    TaskRunSecurityConfigurationName: NotRequired[str],
```

1. See [:material-code-braces: MLUserDataEncryptionTypeDef](./type_defs.md#mluserdataencryptiontypedef) 
## MetadataInfoTypeDef

```python
# MetadataInfoTypeDef definition

class MetadataInfoTypeDef(TypedDict):
    MetadataValue: NotRequired[str],
    CreatedTime: NotRequired[str],
    OtherMetadataValueList: NotRequired[List[OtherMetadataValueListItemTypeDef]],  # (1)
```

1. See [:material-code-braces: OtherMetadataValueListItemTypeDef](./type_defs.md#othermetadatavaluelistitemtypedef) 
## PutSchemaVersionMetadataInputRequestTypeDef

```python
# PutSchemaVersionMetadataInputRequestTypeDef definition

class PutSchemaVersionMetadataInputRequestTypeDef(TypedDict):
    MetadataKeyValue: MetadataKeyValuePairTypeDef,  # (1)
    SchemaId: NotRequired[SchemaIdTypeDef],  # (2)
    SchemaVersionNumber: NotRequired[SchemaVersionNumberTypeDef],  # (3)
    SchemaVersionId: NotRequired[str],
```

1. See [:material-code-braces: MetadataKeyValuePairTypeDef](./type_defs.md#metadatakeyvaluepairtypedef) 
2. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
3. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
## QuerySchemaVersionMetadataInputRequestTypeDef

```python
# QuerySchemaVersionMetadataInputRequestTypeDef definition

class QuerySchemaVersionMetadataInputRequestTypeDef(TypedDict):
    SchemaId: NotRequired[SchemaIdTypeDef],  # (1)
    SchemaVersionNumber: NotRequired[SchemaVersionNumberTypeDef],  # (2)
    SchemaVersionId: NotRequired[str],
    MetadataList: NotRequired[Sequence[MetadataKeyValuePairTypeDef]],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
3. See [:material-code-braces: MetadataKeyValuePairTypeDef](./type_defs.md#metadatakeyvaluepairtypedef) 
## RemoveSchemaVersionMetadataInputRequestTypeDef

```python
# RemoveSchemaVersionMetadataInputRequestTypeDef definition

class RemoveSchemaVersionMetadataInputRequestTypeDef(TypedDict):
    MetadataKeyValue: MetadataKeyValuePairTypeDef,  # (1)
    SchemaId: NotRequired[SchemaIdTypeDef],  # (2)
    SchemaVersionNumber: NotRequired[SchemaVersionNumberTypeDef],  # (3)
    SchemaVersionId: NotRequired[str],
```

1. See [:material-code-braces: MetadataKeyValuePairTypeDef](./type_defs.md#metadatakeyvaluepairtypedef) 
2. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
3. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
## RecipeTypeDef

```python
# RecipeTypeDef definition

class RecipeTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    RecipeReference: RecipeReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: RecipeReferenceTypeDef](./type_defs.md#recipereferencetypedef) 
## RedshiftTargetTypeDef

```python
# RedshiftTargetTypeDef definition

class RedshiftTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
    RedshiftTmpDir: NotRequired[str],
    TmpDirIAMRole: NotRequired[str],
    UpsertRedshiftOptions: NotRequired[UpsertRedshiftTargetOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: UpsertRedshiftTargetOptionsTypeDef](./type_defs.md#upsertredshifttargetoptionstypedef) 
## UserDefinedFunctionInputTypeDef

```python
# UserDefinedFunctionInputTypeDef definition

class UserDefinedFunctionInputTypeDef(TypedDict):
    FunctionName: NotRequired[str],
    ClassName: NotRequired[str],
    OwnerName: NotRequired[str],
    OwnerType: NotRequired[PrincipalTypeType],  # (1)
    ResourceUris: NotRequired[Sequence[ResourceUriTypeDef]],  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ResourceUriTypeDef](./type_defs.md#resourceuritypedef) 
## UserDefinedFunctionTypeDef

```python
# UserDefinedFunctionTypeDef definition

class UserDefinedFunctionTypeDef(TypedDict):
    FunctionName: NotRequired[str],
    DatabaseName: NotRequired[str],
    ClassName: NotRequired[str],
    OwnerName: NotRequired[str],
    OwnerType: NotRequired[PrincipalTypeType],  # (1)
    CreateTime: NotRequired[datetime],
    ResourceUris: NotRequired[List[ResourceUriTypeDef]],  # (2)
    CatalogId: NotRequired[str],
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ResourceUriTypeDef](./type_defs.md#resourceuritypedef) 
## SearchTablesRequestRequestTypeDef

```python
# SearchTablesRequestRequestTypeDef definition

class SearchTablesRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[PropertyPredicateTypeDef]],  # (1)
    SearchText: NotRequired[str],
    SortCriteria: NotRequired[Sequence[SortCriterionTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    ResourceShareType: NotRequired[ResourceShareTypeType],  # (3)
```

1. See [:material-code-braces: PropertyPredicateTypeDef](./type_defs.md#propertypredicatetypedef) 
2. See [:material-code-braces: SortCriterionTypeDef](./type_defs.md#sortcriteriontypedef) 
3. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
## StatementOutputTypeDef

```python
# StatementOutputTypeDef definition

class StatementOutputTypeDef(TypedDict):
    Data: NotRequired[StatementOutputDataTypeDef],  # (1)
    ExecutionCount: NotRequired[int],
    Status: NotRequired[StatementStateType],  # (2)
    ErrorName: NotRequired[str],
    ErrorValue: NotRequired[str],
    Traceback: NotRequired[List[str]],
```

1. See [:material-code-braces: StatementOutputDataTypeDef](./type_defs.md#statementoutputdatatypedef) 
2. See [:material-code-brackets: StatementStateType](./literals.md#statementstatetype) 
## UpdateClassifierRequestRequestTypeDef

```python
# UpdateClassifierRequestRequestTypeDef definition

class UpdateClassifierRequestRequestTypeDef(TypedDict):
    GrokClassifier: NotRequired[UpdateGrokClassifierRequestTypeDef],  # (1)
    XMLClassifier: NotRequired[UpdateXMLClassifierRequestTypeDef],  # (2)
    JsonClassifier: NotRequired[UpdateJsonClassifierRequestTypeDef],  # (3)
    CsvClassifier: NotRequired[UpdateCsvClassifierRequestTypeDef],  # (4)
```

1. See [:material-code-braces: UpdateGrokClassifierRequestTypeDef](./type_defs.md#updategrokclassifierrequesttypedef) 
2. See [:material-code-braces: UpdateXMLClassifierRequestTypeDef](./type_defs.md#updatexmlclassifierrequesttypedef) 
3. See [:material-code-braces: UpdateJsonClassifierRequestTypeDef](./type_defs.md#updatejsonclassifierrequesttypedef) 
4. See [:material-code-braces: UpdateCsvClassifierRequestTypeDef](./type_defs.md#updatecsvclassifierrequesttypedef) 
## AmazonRedshiftSourceTypeDef

```python
# AmazonRedshiftSourceTypeDef definition

class AmazonRedshiftSourceTypeDef(TypedDict):
    Name: NotRequired[str],
    Data: NotRequired[AmazonRedshiftNodeDataTypeDef],  # (1)
```

1. See [:material-code-braces: AmazonRedshiftNodeDataTypeDef](./type_defs.md#amazonredshiftnodedatatypedef) 
## AmazonRedshiftTargetTypeDef

```python
# AmazonRedshiftTargetTypeDef definition

class AmazonRedshiftTargetTypeDef(TypedDict):
    Name: NotRequired[str],
    Data: NotRequired[AmazonRedshiftNodeDataTypeDef],  # (1)
    Inputs: NotRequired[List[str]],
```

1. See [:material-code-braces: AmazonRedshiftNodeDataTypeDef](./type_defs.md#amazonredshiftnodedatatypedef) 
## SnowflakeTargetTypeDef

```python
# SnowflakeTargetTypeDef definition

class SnowflakeTargetTypeDef(TypedDict):
    Name: str,
    Data: SnowflakeNodeDataTypeDef,  # (1)
    Inputs: NotRequired[List[str]],
```

1. See [:material-code-braces: SnowflakeNodeDataTypeDef](./type_defs.md#snowflakenodedatatypedef) 
## PartitionIndexDescriptorTypeDef

```python
# PartitionIndexDescriptorTypeDef definition

class PartitionIndexDescriptorTypeDef(TypedDict):
    IndexName: str,
    Keys: List[KeySchemaElementTypeDef],  # (1)
    IndexStatus: PartitionIndexStatusType,  # (2)
    BackfillErrors: NotRequired[List[BackfillErrorTypeDef]],  # (3)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-brackets: PartitionIndexStatusType](./literals.md#partitionindexstatustype) 
3. See [:material-code-braces: BackfillErrorTypeDef](./type_defs.md#backfillerrortypedef) 
## BatchStopJobRunResponseTypeDef

```python
# BatchStopJobRunResponseTypeDef definition

class BatchStopJobRunResponseTypeDef(TypedDict):
    SuccessfulSubmissions: List[BatchStopJobRunSuccessfulSubmissionTypeDef],  # (1)
    Errors: List[BatchStopJobRunErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchStopJobRunSuccessfulSubmissionTypeDef](./type_defs.md#batchstopjobrunsuccessfulsubmissiontypedef) 
2. See [:material-code-braces: BatchStopJobRunErrorTypeDef](./type_defs.md#batchstopjobrunerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdatePartitionResponseTypeDef

```python
# BatchUpdatePartitionResponseTypeDef definition

class BatchUpdatePartitionResponseTypeDef(TypedDict):
    Errors: List[BatchUpdatePartitionFailureEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchUpdatePartitionFailureEntryTypeDef](./type_defs.md#batchupdatepartitionfailureentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreatePartitionResponseTypeDef

```python
# BatchCreatePartitionResponseTypeDef definition

class BatchCreatePartitionResponseTypeDef(TypedDict):
    Errors: List[PartitionErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartitionErrorTypeDef](./type_defs.md#partitionerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeletePartitionResponseTypeDef

```python
# BatchDeletePartitionResponseTypeDef definition

class BatchDeletePartitionResponseTypeDef(TypedDict):
    Errors: List[PartitionErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartitionErrorTypeDef](./type_defs.md#partitionerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteTableResponseTypeDef

```python
# BatchDeleteTableResponseTypeDef definition

class BatchDeleteTableResponseTypeDef(TypedDict):
    Errors: List[TableErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableErrorTypeDef](./type_defs.md#tableerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteTableVersionResponseTypeDef

```python
# BatchDeleteTableVersionResponseTypeDef definition

class BatchDeleteTableVersionResponseTypeDef(TypedDict):
    Errors: List[TableVersionErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableVersionErrorTypeDef](./type_defs.md#tableversionerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetBlueprintsResponseTypeDef

```python
# BatchGetBlueprintsResponseTypeDef definition

class BatchGetBlueprintsResponseTypeDef(TypedDict):
    Blueprints: List[BlueprintTypeDef],  # (1)
    MissingBlueprints: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueprintTypeDef](./type_defs.md#blueprinttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlueprintResponseTypeDef

```python
# GetBlueprintResponseTypeDef definition

class GetBlueprintResponseTypeDef(TypedDict):
    Blueprint: BlueprintTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueprintTypeDef](./type_defs.md#blueprinttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetClassifierResponseTypeDef

```python
# GetClassifierResponseTypeDef definition

class GetClassifierResponseTypeDef(TypedDict):
    Classifier: ClassifierTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClassifierTypeDef](./type_defs.md#classifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetClassifiersResponseTypeDef

```python
# GetClassifiersResponseTypeDef definition

class GetClassifiersResponseTypeDef(TypedDict):
    Classifiers: List[ClassifierTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClassifierTypeDef](./type_defs.md#classifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScriptRequestRequestTypeDef

```python
# CreateScriptRequestRequestTypeDef definition

class CreateScriptRequestRequestTypeDef(TypedDict):
    DagNodes: NotRequired[Sequence[CodeGenNodeTypeDef]],  # (1)
    DagEdges: NotRequired[Sequence[CodeGenEdgeTypeDef]],  # (2)
    Language: NotRequired[LanguageType],  # (3)
```

1. See [:material-code-braces: CodeGenNodeTypeDef](./type_defs.md#codegennodetypedef) 
2. See [:material-code-braces: CodeGenEdgeTypeDef](./type_defs.md#codegenedgetypedef) 
3. See [:material-code-brackets: LanguageType](./literals.md#languagetype) 
## GetDataflowGraphResponseTypeDef

```python
# GetDataflowGraphResponseTypeDef definition

class GetDataflowGraphResponseTypeDef(TypedDict):
    DagNodes: List[CodeGenNodeTypeDef],  # (1)
    DagEdges: List[CodeGenEdgeTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CodeGenNodeTypeDef](./type_defs.md#codegennodetypedef) 
2. See [:material-code-braces: CodeGenEdgeTypeDef](./type_defs.md#codegenedgetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMappingRequestRequestTypeDef

```python
# GetMappingRequestRequestTypeDef definition

class GetMappingRequestRequestTypeDef(TypedDict):
    Source: CatalogEntryTypeDef,  # (1)
    Sinks: NotRequired[Sequence[CatalogEntryTypeDef]],  # (2)
    Location: NotRequired[LocationTypeDef],  # (3)
```

1. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
2. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
3. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
## GetPlanRequestRequestTypeDef

```python
# GetPlanRequestRequestTypeDef definition

class GetPlanRequestRequestTypeDef(TypedDict):
    Mapping: Sequence[MappingEntryTypeDef],  # (1)
    Source: CatalogEntryTypeDef,  # (2)
    Sinks: NotRequired[Sequence[CatalogEntryTypeDef]],  # (3)
    Location: NotRequired[LocationTypeDef],  # (4)
    Language: NotRequired[LanguageType],  # (5)
    AdditionalPlanOptionsMap: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MappingEntryTypeDef](./type_defs.md#mappingentrytypedef) 
2. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
3. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
4. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
5. See [:material-code-brackets: LanguageType](./literals.md#languagetype) 
## CreateTriggerRequestRequestTypeDef

```python
# CreateTriggerRequestRequestTypeDef definition

class CreateTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
    Type: TriggerTypeType,  # (1)
    Actions: Sequence[ActionTypeDef],  # (2)
    WorkflowName: NotRequired[str],
    Schedule: NotRequired[str],
    Predicate: NotRequired[PredicateTypeDef],  # (3)
    Description: NotRequired[str],
    StartOnCreation: NotRequired[bool],
    Tags: NotRequired[Mapping[str, str]],
    EventBatchingCondition: NotRequired[EventBatchingConditionTypeDef],  # (4)
```

1. See [:material-code-brackets: TriggerTypeType](./literals.md#triggertypetype) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
3. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
4. See [:material-code-braces: EventBatchingConditionTypeDef](./type_defs.md#eventbatchingconditiontypedef) 
## TriggerTypeDef

```python
# TriggerTypeDef definition

class TriggerTypeDef(TypedDict):
    Name: NotRequired[str],
    WorkflowName: NotRequired[str],
    Id: NotRequired[str],
    Type: NotRequired[TriggerTypeType],  # (1)
    State: NotRequired[TriggerStateType],  # (2)
    Description: NotRequired[str],
    Schedule: NotRequired[str],
    Actions: NotRequired[List[ActionTypeDef]],  # (3)
    Predicate: NotRequired[PredicateTypeDef],  # (4)
    EventBatchingCondition: NotRequired[EventBatchingConditionTypeDef],  # (5)
```

1. See [:material-code-brackets: TriggerTypeType](./literals.md#triggertypetype) 
2. See [:material-code-brackets: TriggerStateType](./literals.md#triggerstatetype) 
3. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
4. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
5. See [:material-code-braces: EventBatchingConditionTypeDef](./type_defs.md#eventbatchingconditiontypedef) 
## TriggerUpdateTypeDef

```python
# TriggerUpdateTypeDef definition

class TriggerUpdateTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    Schedule: NotRequired[str],
    Actions: NotRequired[Sequence[ActionTypeDef]],  # (1)
    Predicate: NotRequired[PredicateTypeDef],  # (2)
    EventBatchingCondition: NotRequired[EventBatchingConditionTypeDef],  # (3)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
3. See [:material-code-braces: EventBatchingConditionTypeDef](./type_defs.md#eventbatchingconditiontypedef) 
## EvaluationMetricsTypeDef

```python
# EvaluationMetricsTypeDef definition

class EvaluationMetricsTypeDef(TypedDict):
    TransformType: TransformTypeType,  # (1)
    FindMatchesMetrics: NotRequired[FindMatchesMetricsTypeDef],  # (2)
```

1. See [:material-code-brackets: TransformTypeType](./literals.md#transformtypetype) 
2. See [:material-code-braces: FindMatchesMetricsTypeDef](./type_defs.md#findmatchesmetricstypedef) 
## CreateConnectionRequestRequestTypeDef

```python
# CreateConnectionRequestRequestTypeDef definition

class CreateConnectionRequestRequestTypeDef(TypedDict):
    ConnectionInput: ConnectionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConnectionInputTypeDef](./type_defs.md#connectioninputtypedef) 
## UpdateConnectionRequestRequestTypeDef

```python
# UpdateConnectionRequestRequestTypeDef definition

class UpdateConnectionRequestRequestTypeDef(TypedDict):
    Name: str,
    ConnectionInput: ConnectionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: ConnectionInputTypeDef](./type_defs.md#connectioninputtypedef) 
## GetConnectionResponseTypeDef

```python
# GetConnectionResponseTypeDef definition

class GetConnectionResponseTypeDef(TypedDict):
    Connection: ConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectionsResponseTypeDef

```python
# GetConnectionsResponseTypeDef definition

class GetConnectionsResponseTypeDef(TypedDict):
    ConnectionList: List[ConnectionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CrawlerTypeDef

```python
# CrawlerTypeDef definition

class CrawlerTypeDef(TypedDict):
    Name: NotRequired[str],
    Role: NotRequired[str],
    Targets: NotRequired[CrawlerTargetsTypeDef],  # (1)
    DatabaseName: NotRequired[str],
    Description: NotRequired[str],
    Classifiers: NotRequired[List[str]],
    RecrawlPolicy: NotRequired[RecrawlPolicyTypeDef],  # (2)
    SchemaChangePolicy: NotRequired[SchemaChangePolicyTypeDef],  # (3)
    LineageConfiguration: NotRequired[LineageConfigurationTypeDef],  # (4)
    State: NotRequired[CrawlerStateType],  # (5)
    TablePrefix: NotRequired[str],
    Schedule: NotRequired[ScheduleTypeDef],  # (6)
    CrawlElapsedTime: NotRequired[int],
    CreationTime: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    LastCrawl: NotRequired[LastCrawlInfoTypeDef],  # (7)
    Version: NotRequired[int],
    Configuration: NotRequired[str],
    CrawlerSecurityConfiguration: NotRequired[str],
    LakeFormationConfiguration: NotRequired[LakeFormationConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: CrawlerTargetsTypeDef](./type_defs.md#crawlertargetstypedef) 
2. See [:material-code-braces: RecrawlPolicyTypeDef](./type_defs.md#recrawlpolicytypedef) 
3. See [:material-code-braces: SchemaChangePolicyTypeDef](./type_defs.md#schemachangepolicytypedef) 
4. See [:material-code-braces: LineageConfigurationTypeDef](./type_defs.md#lineageconfigurationtypedef) 
5. See [:material-code-brackets: CrawlerStateType](./literals.md#crawlerstatetype) 
6. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
7. See [:material-code-braces: LastCrawlInfoTypeDef](./type_defs.md#lastcrawlinfotypedef) 
8. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) 
## CreateCrawlerRequestRequestTypeDef

```python
# CreateCrawlerRequestRequestTypeDef definition

class CreateCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
    Role: str,
    Targets: CrawlerTargetsTypeDef,  # (1)
    DatabaseName: NotRequired[str],
    Description: NotRequired[str],
    Schedule: NotRequired[str],
    Classifiers: NotRequired[Sequence[str]],
    TablePrefix: NotRequired[str],
    SchemaChangePolicy: NotRequired[SchemaChangePolicyTypeDef],  # (2)
    RecrawlPolicy: NotRequired[RecrawlPolicyTypeDef],  # (3)
    LineageConfiguration: NotRequired[LineageConfigurationTypeDef],  # (4)
    LakeFormationConfiguration: NotRequired[LakeFormationConfigurationTypeDef],  # (5)
    Configuration: NotRequired[str],
    CrawlerSecurityConfiguration: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CrawlerTargetsTypeDef](./type_defs.md#crawlertargetstypedef) 
2. See [:material-code-braces: SchemaChangePolicyTypeDef](./type_defs.md#schemachangepolicytypedef) 
3. See [:material-code-braces: RecrawlPolicyTypeDef](./type_defs.md#recrawlpolicytypedef) 
4. See [:material-code-braces: LineageConfigurationTypeDef](./type_defs.md#lineageconfigurationtypedef) 
5. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) 
## UpdateCrawlerRequestRequestTypeDef

```python
# UpdateCrawlerRequestRequestTypeDef definition

class UpdateCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
    Role: NotRequired[str],
    DatabaseName: NotRequired[str],
    Description: NotRequired[str],
    Targets: NotRequired[CrawlerTargetsTypeDef],  # (1)
    Schedule: NotRequired[str],
    Classifiers: NotRequired[Sequence[str]],
    TablePrefix: NotRequired[str],
    SchemaChangePolicy: NotRequired[SchemaChangePolicyTypeDef],  # (2)
    RecrawlPolicy: NotRequired[RecrawlPolicyTypeDef],  # (3)
    LineageConfiguration: NotRequired[LineageConfigurationTypeDef],  # (4)
    LakeFormationConfiguration: NotRequired[LakeFormationConfigurationTypeDef],  # (5)
    Configuration: NotRequired[str],
    CrawlerSecurityConfiguration: NotRequired[str],
```

1. See [:material-code-braces: CrawlerTargetsTypeDef](./type_defs.md#crawlertargetstypedef) 
2. See [:material-code-braces: SchemaChangePolicyTypeDef](./type_defs.md#schemachangepolicytypedef) 
3. See [:material-code-braces: RecrawlPolicyTypeDef](./type_defs.md#recrawlpolicytypedef) 
4. See [:material-code-braces: LineageConfigurationTypeDef](./type_defs.md#lineageconfigurationtypedef) 
5. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) 
## ListDataQualityRulesetsResponseTypeDef

```python
# ListDataQualityRulesetsResponseTypeDef definition

class ListDataQualityRulesetsResponseTypeDef(TypedDict):
    Rulesets: List[DataQualityRulesetListDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataQualityRulesetListDetailsTypeDef](./type_defs.md#dataqualityrulesetlistdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataQualityResultDescriptionTypeDef

```python
# DataQualityResultDescriptionTypeDef definition

class DataQualityResultDescriptionTypeDef(TypedDict):
    ResultId: NotRequired[str],
    DataSource: NotRequired[DataSourceTypeDef],  # (1)
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
    StartedOn: NotRequired[datetime],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## DataQualityResultFilterCriteriaTypeDef

```python
# DataQualityResultFilterCriteriaTypeDef definition

class DataQualityResultFilterCriteriaTypeDef(TypedDict):
    DataSource: NotRequired[DataSourceTypeDef],  # (1)
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
    StartedAfter: NotRequired[Union[datetime, str]],
    StartedBefore: NotRequired[Union[datetime, str]],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## DataQualityResultTypeDef

```python
# DataQualityResultTypeDef definition

class DataQualityResultTypeDef(TypedDict):
    ResultId: NotRequired[str],
    Score: NotRequired[float],
    DataSource: NotRequired[DataSourceTypeDef],  # (1)
    RulesetName: NotRequired[str],
    EvaluationContext: NotRequired[str],
    StartedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
    RulesetEvaluationRunId: NotRequired[str],
    RuleResults: NotRequired[List[DataQualityRuleResultTypeDef]],  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: DataQualityRuleResultTypeDef](./type_defs.md#dataqualityruleresulttypedef) 
## DataQualityRuleRecommendationRunDescriptionTypeDef

```python
# DataQualityRuleRecommendationRunDescriptionTypeDef definition

class DataQualityRuleRecommendationRunDescriptionTypeDef(TypedDict):
    RunId: NotRequired[str],
    Status: NotRequired[TaskStatusTypeType],  # (1)
    StartedOn: NotRequired[datetime],
    DataSource: NotRequired[DataSourceTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
2. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## DataQualityRuleRecommendationRunFilterTypeDef

```python
# DataQualityRuleRecommendationRunFilterTypeDef definition

class DataQualityRuleRecommendationRunFilterTypeDef(TypedDict):
    DataSource: DataSourceTypeDef,  # (1)
    StartedBefore: NotRequired[Union[datetime, str]],
    StartedAfter: NotRequired[Union[datetime, str]],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## DataQualityRulesetEvaluationRunDescriptionTypeDef

```python
# DataQualityRulesetEvaluationRunDescriptionTypeDef definition

class DataQualityRulesetEvaluationRunDescriptionTypeDef(TypedDict):
    RunId: NotRequired[str],
    Status: NotRequired[TaskStatusTypeType],  # (1)
    StartedOn: NotRequired[datetime],
    DataSource: NotRequired[DataSourceTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
2. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## DataQualityRulesetEvaluationRunFilterTypeDef

```python
# DataQualityRulesetEvaluationRunFilterTypeDef definition

class DataQualityRulesetEvaluationRunFilterTypeDef(TypedDict):
    DataSource: DataSourceTypeDef,  # (1)
    StartedBefore: NotRequired[Union[datetime, str]],
    StartedAfter: NotRequired[Union[datetime, str]],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## GetDataQualityResultResponseTypeDef

```python
# GetDataQualityResultResponseTypeDef definition

class GetDataQualityResultResponseTypeDef(TypedDict):
    ResultId: str,
    Score: float,
    DataSource: DataSourceTypeDef,  # (1)
    RulesetName: str,
    EvaluationContext: str,
    StartedOn: datetime,
    CompletedOn: datetime,
    JobName: str,
    JobRunId: str,
    RulesetEvaluationRunId: str,
    RuleResults: List[DataQualityRuleResultTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: DataQualityRuleResultTypeDef](./type_defs.md#dataqualityruleresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataQualityRuleRecommendationRunResponseTypeDef

```python
# GetDataQualityRuleRecommendationRunResponseTypeDef definition

class GetDataQualityRuleRecommendationRunResponseTypeDef(TypedDict):
    RunId: str,
    DataSource: DataSourceTypeDef,  # (1)
    Role: str,
    NumberOfWorkers: int,
    Timeout: int,
    Status: TaskStatusTypeType,  # (2)
    ErrorString: str,
    StartedOn: datetime,
    LastModifiedOn: datetime,
    CompletedOn: datetime,
    ExecutionTime: int,
    RecommendedRuleset: str,
    CreatedRulesetName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataQualityRulesetEvaluationRunResponseTypeDef

```python
# GetDataQualityRulesetEvaluationRunResponseTypeDef definition

class GetDataQualityRulesetEvaluationRunResponseTypeDef(TypedDict):
    RunId: str,
    DataSource: DataSourceTypeDef,  # (1)
    Role: str,
    NumberOfWorkers: int,
    Timeout: int,
    AdditionalRunOptions: DataQualityEvaluationRunAdditionalRunOptionsTypeDef,  # (2)
    Status: TaskStatusTypeType,  # (3)
    ErrorString: str,
    StartedOn: datetime,
    LastModifiedOn: datetime,
    CompletedOn: datetime,
    ExecutionTime: int,
    RulesetNames: List[str],
    ResultIds: List[str],
    AdditionalDataSources: Dict[str, DataSourceTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: DataQualityEvaluationRunAdditionalRunOptionsTypeDef](./type_defs.md#dataqualityevaluationrunadditionalrunoptionstypedef) 
3. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
4. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataQualityRuleRecommendationRunRequestRequestTypeDef

```python
# StartDataQualityRuleRecommendationRunRequestRequestTypeDef definition

class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(TypedDict):
    DataSource: DataSourceTypeDef,  # (1)
    Role: str,
    NumberOfWorkers: NotRequired[int],
    Timeout: NotRequired[int],
    CreatedRulesetName: NotRequired[str],
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## StartDataQualityRulesetEvaluationRunRequestRequestTypeDef

```python
# StartDataQualityRulesetEvaluationRunRequestRequestTypeDef definition

class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(TypedDict):
    DataSource: DataSourceTypeDef,  # (1)
    Role: str,
    RulesetNames: Sequence[str],
    NumberOfWorkers: NotRequired[int],
    Timeout: NotRequired[int],
    ClientToken: NotRequired[str],
    AdditionalRunOptions: NotRequired[DataQualityEvaluationRunAdditionalRunOptionsTypeDef],  # (2)
    AdditionalDataSources: NotRequired[Mapping[str, DataSourceTypeDef]],  # (3)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: DataQualityEvaluationRunAdditionalRunOptionsTypeDef](./type_defs.md#dataqualityevaluationrunadditionalrunoptionstypedef) 
3. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## CreateSessionResponseTypeDef

```python
# CreateSessionResponseTypeDef definition

class CreateSessionResponseTypeDef(TypedDict):
    Session: SessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSessionResponseTypeDef

```python
# GetSessionResponseTypeDef definition

class GetSessionResponseTypeDef(TypedDict):
    Session: SessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSessionsResponseTypeDef

```python
# ListSessionsResponseTypeDef definition

class ListSessionsResponseTypeDef(TypedDict):
    Ids: List[str],
    Sessions: List[SessionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataCatalogEncryptionSettingsResponseTypeDef

```python
# GetDataCatalogEncryptionSettingsResponseTypeDef definition

class GetDataCatalogEncryptionSettingsResponseTypeDef(TypedDict):
    DataCatalogEncryptionSettings: DataCatalogEncryptionSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataCatalogEncryptionSettingsTypeDef](./type_defs.md#datacatalogencryptionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDataCatalogEncryptionSettingsRequestRequestTypeDef

```python
# PutDataCatalogEncryptionSettingsRequestRequestTypeDef definition

class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(TypedDict):
    DataCatalogEncryptionSettings: DataCatalogEncryptionSettingsTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: DataCatalogEncryptionSettingsTypeDef](./type_defs.md#datacatalogencryptionsettingstypedef) 
## DatabaseInputTypeDef

```python
# DatabaseInputTypeDef definition

class DatabaseInputTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    LocationUri: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
    CreateTableDefaultPermissions: NotRequired[Sequence[PrincipalPermissionsTypeDef]],  # (1)
    TargetDatabase: NotRequired[DatabaseIdentifierTypeDef],  # (2)
    FederatedDatabase: NotRequired[FederatedDatabaseTypeDef],  # (3)
```

1. See [:material-code-braces: PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef) 
2. See [:material-code-braces: DatabaseIdentifierTypeDef](./type_defs.md#databaseidentifiertypedef) 
3. See [:material-code-braces: FederatedDatabaseTypeDef](./type_defs.md#federateddatabasetypedef) 
## DatabaseTypeDef

```python
# DatabaseTypeDef definition

class DatabaseTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    LocationUri: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
    CreateTime: NotRequired[datetime],
    CreateTableDefaultPermissions: NotRequired[List[PrincipalPermissionsTypeDef]],  # (1)
    TargetDatabase: NotRequired[DatabaseIdentifierTypeDef],  # (2)
    CatalogId: NotRequired[str],
    FederatedDatabase: NotRequired[FederatedDatabaseTypeDef],  # (3)
```

1. See [:material-code-braces: PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef) 
2. See [:material-code-braces: DatabaseIdentifierTypeDef](./type_defs.md#databaseidentifiertypedef) 
3. See [:material-code-braces: FederatedDatabaseTypeDef](./type_defs.md#federateddatabasetypedef) 
## ListDataQualityRulesetsRequestRequestTypeDef

```python
# ListDataQualityRulesetsRequestRequestTypeDef definition

class ListDataQualityRulesetsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filter: NotRequired[DataQualityRulesetFilterCriteriaTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DataQualityRulesetFilterCriteriaTypeDef](./type_defs.md#dataqualityrulesetfiltercriteriatypedef) 
## GetMLTaskRunsRequestRequestTypeDef

```python
# GetMLTaskRunsRequestRequestTypeDef definition

class GetMLTaskRunsRequestRequestTypeDef(TypedDict):
    TransformId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filter: NotRequired[TaskRunFilterCriteriaTypeDef],  # (1)
    Sort: NotRequired[TaskRunSortCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: TaskRunFilterCriteriaTypeDef](./type_defs.md#taskrunfiltercriteriatypedef) 
2. See [:material-code-braces: TaskRunSortCriteriaTypeDef](./type_defs.md#taskrunsortcriteriatypedef) 
## DropNullFieldsTypeDef

```python
# DropNullFieldsTypeDef definition

class DropNullFieldsTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    NullCheckBoxList: NotRequired[NullCheckBoxListTypeDef],  # (1)
    NullTextList: NotRequired[List[NullValueFieldTypeDef]],  # (2)
```

1. See [:material-code-braces: NullCheckBoxListTypeDef](./type_defs.md#nullcheckboxlisttypedef) 
2. See [:material-code-braces: NullValueFieldTypeDef](./type_defs.md#nullvaluefieldtypedef) 
## ColumnStatisticsDataTypeDef

```python
# ColumnStatisticsDataTypeDef definition

class ColumnStatisticsDataTypeDef(TypedDict):
    Type: ColumnStatisticsTypeType,  # (1)
    BooleanColumnStatisticsData: NotRequired[BooleanColumnStatisticsDataTypeDef],  # (2)
    DateColumnStatisticsData: NotRequired[DateColumnStatisticsDataTypeDef],  # (3)
    DecimalColumnStatisticsData: NotRequired[DecimalColumnStatisticsDataTypeDef],  # (4)
    DoubleColumnStatisticsData: NotRequired[DoubleColumnStatisticsDataTypeDef],  # (5)
    LongColumnStatisticsData: NotRequired[LongColumnStatisticsDataTypeDef],  # (6)
    StringColumnStatisticsData: NotRequired[StringColumnStatisticsDataTypeDef],  # (7)
    BinaryColumnStatisticsData: NotRequired[BinaryColumnStatisticsDataTypeDef],  # (8)
```

1. See [:material-code-brackets: ColumnStatisticsTypeType](./literals.md#columnstatisticstypetype) 
2. See [:material-code-braces: BooleanColumnStatisticsDataTypeDef](./type_defs.md#booleancolumnstatisticsdatatypedef) 
3. See [:material-code-braces: DateColumnStatisticsDataTypeDef](./type_defs.md#datecolumnstatisticsdatatypedef) 
4. See [:material-code-braces: DecimalColumnStatisticsDataTypeDef](./type_defs.md#decimalcolumnstatisticsdatatypedef) 
5. See [:material-code-braces: DoubleColumnStatisticsDataTypeDef](./type_defs.md#doublecolumnstatisticsdatatypedef) 
6. See [:material-code-braces: LongColumnStatisticsDataTypeDef](./type_defs.md#longcolumnstatisticsdatatypedef) 
7. See [:material-code-braces: StringColumnStatisticsDataTypeDef](./type_defs.md#stringcolumnstatisticsdatatypedef) 
8. See [:material-code-braces: BinaryColumnStatisticsDataTypeDef](./type_defs.md#binarycolumnstatisticsdatatypedef) 
## StorageDescriptorTypeDef

```python
# StorageDescriptorTypeDef definition

class StorageDescriptorTypeDef(TypedDict):
    Columns: NotRequired[Sequence[ColumnTypeDef]],  # (1)
    Location: NotRequired[str],
    AdditionalLocations: NotRequired[Sequence[str]],
    InputFormat: NotRequired[str],
    OutputFormat: NotRequired[str],
    Compressed: NotRequired[bool],
    NumberOfBuckets: NotRequired[int],
    SerdeInfo: NotRequired[SerDeInfoTypeDef],  # (2)
    BucketColumns: NotRequired[Sequence[str]],
    SortColumns: NotRequired[Sequence[OrderTypeDef]],  # (3)
    Parameters: NotRequired[Mapping[str, str]],
    SkewedInfo: NotRequired[SkewedInfoTypeDef],  # (4)
    StoredAsSubDirectories: NotRequired[bool],
    SchemaReference: NotRequired[SchemaReferenceTypeDef],  # (5)
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
2. See [:material-code-braces: SerDeInfoTypeDef](./type_defs.md#serdeinfotypedef) 
3. See [:material-code-braces: OrderTypeDef](./type_defs.md#ordertypedef) 
4. See [:material-code-braces: SkewedInfoTypeDef](./type_defs.md#skewedinfotypedef) 
5. See [:material-code-braces: SchemaReferenceTypeDef](./type_defs.md#schemareferencetypedef) 
## CreateSecurityConfigurationRequestRequestTypeDef

```python
# CreateSecurityConfigurationRequestRequestTypeDef definition

class CreateSecurityConfigurationRequestRequestTypeDef(TypedDict):
    Name: str,
    EncryptionConfiguration: EncryptionConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## SecurityConfigurationTypeDef

```python
# SecurityConfigurationTypeDef definition

class SecurityConfigurationTypeDef(TypedDict):
    Name: NotRequired[str],
    CreatedTimeStamp: NotRequired[datetime],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## DeleteSchemaVersionsResponseTypeDef

```python
# DeleteSchemaVersionsResponseTypeDef definition

class DeleteSchemaVersionsResponseTypeDef(TypedDict):
    SchemaVersionErrors: List[SchemaVersionErrorItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaVersionErrorItemTypeDef](./type_defs.md#schemaversionerroritemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    LogicalOperator: FilterLogicalOperatorType,  # (1)
    Filters: List[FilterExpressionTypeDef],  # (2)
```

1. See [:material-code-brackets: FilterLogicalOperatorType](./literals.md#filterlogicaloperatortype) 
2. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef) 
## UpdateMLTransformRequestRequestTypeDef

```python
# UpdateMLTransformRequestRequestTypeDef definition

class UpdateMLTransformRequestRequestTypeDef(TypedDict):
    TransformId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    Parameters: NotRequired[TransformParametersTypeDef],  # (1)
    Role: NotRequired[str],
    GlueVersion: NotRequired[str],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (2)
    NumberOfWorkers: NotRequired[int],
    Timeout: NotRequired[int],
    MaxRetries: NotRequired[int],
```

1. See [:material-code-braces: TransformParametersTypeDef](./type_defs.md#transformparameterstypedef) 
2. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
## GetMLTransformsRequestRequestTypeDef

```python
# GetMLTransformsRequestRequestTypeDef definition

class GetMLTransformsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filter: NotRequired[TransformFilterCriteriaTypeDef],  # (1)
    Sort: NotRequired[TransformSortCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: TransformFilterCriteriaTypeDef](./type_defs.md#transformfiltercriteriatypedef) 
2. See [:material-code-braces: TransformSortCriteriaTypeDef](./type_defs.md#transformsortcriteriatypedef) 
## ListMLTransformsRequestRequestTypeDef

```python
# ListMLTransformsRequestRequestTypeDef definition

class ListMLTransformsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filter: NotRequired[TransformFilterCriteriaTypeDef],  # (1)
    Sort: NotRequired[TransformSortCriteriaTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TransformFilterCriteriaTypeDef](./type_defs.md#transformfiltercriteriatypedef) 
2. See [:material-code-braces: TransformSortCriteriaTypeDef](./type_defs.md#transformsortcriteriatypedef) 
## AthenaConnectorSourceTypeDef

```python
# AthenaConnectorSourceTypeDef definition

class AthenaConnectorSourceTypeDef(TypedDict):
    Name: str,
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    SchemaName: str,
    ConnectionTable: NotRequired[str],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## CatalogDeltaSourceTypeDef

```python
# CatalogDeltaSourceTypeDef definition

class CatalogDeltaSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalDeltaOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## CatalogHudiSourceTypeDef

```python
# CatalogHudiSourceTypeDef definition

class CatalogHudiSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalHudiOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## CustomCodeTypeDef

```python
# CustomCodeTypeDef definition

class CustomCodeTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Code: str,
    ClassName: str,
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## DynamicTransformTypeDef

```python
# DynamicTransformTypeDef definition

class DynamicTransformTypeDef(TypedDict):
    Name: str,
    TransformName: str,
    Inputs: List[str],
    FunctionName: str,
    Path: str,
    Parameters: NotRequired[List[TransformConfigParameterTypeDef]],  # (1)
    Version: NotRequired[str],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: TransformConfigParameterTypeDef](./type_defs.md#transformconfigparametertypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## JDBCConnectorSourceTypeDef

```python
# JDBCConnectorSourceTypeDef definition

class JDBCConnectorSourceTypeDef(TypedDict):
    Name: str,
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[JDBCConnectorOptionsTypeDef],  # (1)
    ConnectionTable: NotRequired[str],
    Query: NotRequired[str],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: JDBCConnectorOptionsTypeDef](./type_defs.md#jdbcconnectoroptionstypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## JDBCConnectorTargetTypeDef

```python
# JDBCConnectorTargetTypeDef definition

class JDBCConnectorTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    ConnectionName: str,
    ConnectionTable: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3CatalogDeltaSourceTypeDef

```python
# S3CatalogDeltaSourceTypeDef definition

class S3CatalogDeltaSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalDeltaOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3CatalogHudiSourceTypeDef

```python
# S3CatalogHudiSourceTypeDef definition

class S3CatalogHudiSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalHudiOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3CsvSourceTypeDef

```python
# S3CsvSourceTypeDef definition

class S3CsvSourceTypeDef(TypedDict):
    Name: str,
    Paths: List[str],
    Separator: SeparatorType,  # (3)
    QuoteChar: QuoteCharType,  # (4)
    CompressionType: NotRequired[CompressionTypeType],  # (1)
    Exclusions: NotRequired[List[str]],
    GroupSize: NotRequired[str],
    GroupFiles: NotRequired[str],
    Recurse: NotRequired[bool],
    MaxBand: NotRequired[int],
    MaxFilesInBand: NotRequired[int],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (2)
    Escaper: NotRequired[str],
    Multiline: NotRequired[bool],
    WithHeader: NotRequired[bool],
    WriteHeader: NotRequired[bool],
    SkipFirst: NotRequired[bool],
    OptimizePerformance: NotRequired[bool],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (5)
```

1. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
2. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
3. See [:material-code-brackets: SeparatorType](./literals.md#separatortype) 
4. See [:material-code-brackets: QuoteCharType](./literals.md#quotechartype) 
5. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3DeltaSourceTypeDef

```python
# S3DeltaSourceTypeDef definition

class S3DeltaSourceTypeDef(TypedDict):
    Name: str,
    Paths: List[str],
    AdditionalDeltaOptions: NotRequired[Dict[str, str]],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (1)
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3HudiSourceTypeDef

```python
# S3HudiSourceTypeDef definition

class S3HudiSourceTypeDef(TypedDict):
    Name: str,
    Paths: List[str],
    AdditionalHudiOptions: NotRequired[Dict[str, str]],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (1)
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3JsonSourceTypeDef

```python
# S3JsonSourceTypeDef definition

class S3JsonSourceTypeDef(TypedDict):
    Name: str,
    Paths: List[str],
    CompressionType: NotRequired[CompressionTypeType],  # (1)
    Exclusions: NotRequired[List[str]],
    GroupSize: NotRequired[str],
    GroupFiles: NotRequired[str],
    Recurse: NotRequired[bool],
    MaxBand: NotRequired[int],
    MaxFilesInBand: NotRequired[int],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (2)
    JsonPath: NotRequired[str],
    Multiline: NotRequired[bool],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (3)
```

1. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
2. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
3. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3ParquetSourceTypeDef

```python
# S3ParquetSourceTypeDef definition

class S3ParquetSourceTypeDef(TypedDict):
    Name: str,
    Paths: List[str],
    CompressionType: NotRequired[ParquetCompressionTypeType],  # (1)
    Exclusions: NotRequired[List[str]],
    GroupSize: NotRequired[str],
    GroupFiles: NotRequired[str],
    Recurse: NotRequired[bool],
    MaxBand: NotRequired[int],
    MaxFilesInBand: NotRequired[int],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (2)
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (3)
```

1. See [:material-code-brackets: ParquetCompressionTypeType](./literals.md#parquetcompressiontypetype) 
2. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
3. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## SnowflakeSourceTypeDef

```python
# SnowflakeSourceTypeDef definition

class SnowflakeSourceTypeDef(TypedDict):
    Name: str,
    Data: SnowflakeNodeDataTypeDef,  # (1)
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: SnowflakeNodeDataTypeDef](./type_defs.md#snowflakenodedatatypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## SparkConnectorSourceTypeDef

```python
# SparkConnectorSourceTypeDef definition

class SparkConnectorSourceTypeDef(TypedDict):
    Name: str,
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## SparkConnectorTargetTypeDef

```python
# SparkConnectorTargetTypeDef definition

class SparkConnectorTargetTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## SparkSQLTypeDef

```python
# SparkSQLTypeDef definition

class SparkSQLTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    SqlQuery: str,
    SqlAliases: List[SqlAliasTypeDef],  # (1)
    OutputSchemas: NotRequired[List[GlueSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: SqlAliasTypeDef](./type_defs.md#sqlaliastypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## GetJobRunResponseTypeDef

```python
# GetJobRunResponseTypeDef definition

class GetJobRunResponseTypeDef(TypedDict):
    JobRun: JobRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobRunTypeDef](./type_defs.md#jobruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobRunsResponseTypeDef

```python
# GetJobRunsResponseTypeDef definition

class GetJobRunsResponseTypeDef(TypedDict):
    JobRuns: List[JobRunTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobRunTypeDef](./type_defs.md#jobruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobNodeDetailsTypeDef

```python
# JobNodeDetailsTypeDef definition

class JobNodeDetailsTypeDef(TypedDict):
    JobRuns: NotRequired[List[JobRunTypeDef]],  # (1)
```

1. See [:material-code-braces: JobRunTypeDef](./type_defs.md#jobruntypedef) 
## GetMLTaskRunResponseTypeDef

```python
# GetMLTaskRunResponseTypeDef definition

class GetMLTaskRunResponseTypeDef(TypedDict):
    TransformId: str,
    TaskRunId: str,
    Status: TaskStatusTypeType,  # (1)
    LogGroupName: str,
    Properties: TaskRunPropertiesTypeDef,  # (2)
    ErrorString: str,
    StartedOn: datetime,
    LastModifiedOn: datetime,
    CompletedOn: datetime,
    ExecutionTime: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
2. See [:material-code-braces: TaskRunPropertiesTypeDef](./type_defs.md#taskrunpropertiestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TaskRunTypeDef

```python
# TaskRunTypeDef definition

class TaskRunTypeDef(TypedDict):
    TransformId: NotRequired[str],
    TaskRunId: NotRequired[str],
    Status: NotRequired[TaskStatusTypeType],  # (1)
    LogGroupName: NotRequired[str],
    Properties: NotRequired[TaskRunPropertiesTypeDef],  # (2)
    ErrorString: NotRequired[str],
    StartedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    ExecutionTime: NotRequired[int],
```

1. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
2. See [:material-code-braces: TaskRunPropertiesTypeDef](./type_defs.md#taskrunpropertiestypedef) 
## CreateMLTransformRequestRequestTypeDef

```python
# CreateMLTransformRequestRequestTypeDef definition

class CreateMLTransformRequestRequestTypeDef(TypedDict):
    Name: str,
    InputRecordTables: Sequence[GlueTableTypeDef],  # (1)
    Parameters: TransformParametersTypeDef,  # (2)
    Role: str,
    Description: NotRequired[str],
    GlueVersion: NotRequired[str],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (3)
    NumberOfWorkers: NotRequired[int],
    Timeout: NotRequired[int],
    MaxRetries: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
    TransformEncryption: NotRequired[TransformEncryptionTypeDef],  # (4)
```

1. See [:material-code-braces: GlueTableTypeDef](./type_defs.md#gluetabletypedef) 
2. See [:material-code-braces: TransformParametersTypeDef](./type_defs.md#transformparameterstypedef) 
3. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
4. See [:material-code-braces: TransformEncryptionTypeDef](./type_defs.md#transformencryptiontypedef) 
## QuerySchemaVersionMetadataResponseTypeDef

```python
# QuerySchemaVersionMetadataResponseTypeDef definition

class QuerySchemaVersionMetadataResponseTypeDef(TypedDict):
    MetadataInfoMap: Dict[str, MetadataInfoTypeDef],  # (1)
    SchemaVersionId: str,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetadataInfoTypeDef](./type_defs.md#metadatainfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserDefinedFunctionRequestRequestTypeDef

```python
# CreateUserDefinedFunctionRequestRequestTypeDef definition

class CreateUserDefinedFunctionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    FunctionInput: UserDefinedFunctionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: UserDefinedFunctionInputTypeDef](./type_defs.md#userdefinedfunctioninputtypedef) 
## UpdateUserDefinedFunctionRequestRequestTypeDef

```python
# UpdateUserDefinedFunctionRequestRequestTypeDef definition

class UpdateUserDefinedFunctionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    FunctionName: str,
    FunctionInput: UserDefinedFunctionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: UserDefinedFunctionInputTypeDef](./type_defs.md#userdefinedfunctioninputtypedef) 
## GetUserDefinedFunctionResponseTypeDef

```python
# GetUserDefinedFunctionResponseTypeDef definition

class GetUserDefinedFunctionResponseTypeDef(TypedDict):
    UserDefinedFunction: UserDefinedFunctionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserDefinedFunctionTypeDef](./type_defs.md#userdefinedfunctiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserDefinedFunctionsResponseTypeDef

```python
# GetUserDefinedFunctionsResponseTypeDef definition

class GetUserDefinedFunctionsResponseTypeDef(TypedDict):
    UserDefinedFunctions: List[UserDefinedFunctionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserDefinedFunctionTypeDef](./type_defs.md#userdefinedfunctiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StatementTypeDef

```python
# StatementTypeDef definition

class StatementTypeDef(TypedDict):
    Id: NotRequired[int],
    Code: NotRequired[str],
    State: NotRequired[StatementStateType],  # (1)
    Output: NotRequired[StatementOutputTypeDef],  # (2)
    Progress: NotRequired[float],
    StartedOn: NotRequired[int],
    CompletedOn: NotRequired[int],
```

1. See [:material-code-brackets: StatementStateType](./literals.md#statementstatetype) 
2. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
## GetPartitionIndexesResponseTypeDef

```python
# GetPartitionIndexesResponseTypeDef definition

class GetPartitionIndexesResponseTypeDef(TypedDict):
    PartitionIndexDescriptorList: List[PartitionIndexDescriptorTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartitionIndexDescriptorTypeDef](./type_defs.md#partitionindexdescriptortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetTriggersResponseTypeDef

```python
# BatchGetTriggersResponseTypeDef definition

class BatchGetTriggersResponseTypeDef(TypedDict):
    Triggers: List[TriggerTypeDef],  # (1)
    TriggersNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TriggerTypeDef](./type_defs.md#triggertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTriggerResponseTypeDef

```python
# GetTriggerResponseTypeDef definition

class GetTriggerResponseTypeDef(TypedDict):
    Trigger: TriggerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TriggerTypeDef](./type_defs.md#triggertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTriggersResponseTypeDef

```python
# GetTriggersResponseTypeDef definition

class GetTriggersResponseTypeDef(TypedDict):
    Triggers: List[TriggerTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TriggerTypeDef](./type_defs.md#triggertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TriggerNodeDetailsTypeDef

```python
# TriggerNodeDetailsTypeDef definition

class TriggerNodeDetailsTypeDef(TypedDict):
    Trigger: NotRequired[TriggerTypeDef],  # (1)
```

1. See [:material-code-braces: TriggerTypeDef](./type_defs.md#triggertypedef) 
## UpdateTriggerResponseTypeDef

```python
# UpdateTriggerResponseTypeDef definition

class UpdateTriggerResponseTypeDef(TypedDict):
    Trigger: TriggerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TriggerTypeDef](./type_defs.md#triggertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTriggerRequestRequestTypeDef

```python
# UpdateTriggerRequestRequestTypeDef definition

class UpdateTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
    TriggerUpdate: TriggerUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: TriggerUpdateTypeDef](./type_defs.md#triggerupdatetypedef) 
## GetMLTransformResponseTypeDef

```python
# GetMLTransformResponseTypeDef definition

class GetMLTransformResponseTypeDef(TypedDict):
    TransformId: str,
    Name: str,
    Description: str,
    Status: TransformStatusTypeType,  # (1)
    CreatedOn: datetime,
    LastModifiedOn: datetime,
    InputRecordTables: List[GlueTableTypeDef],  # (2)
    Parameters: TransformParametersTypeDef,  # (3)
    EvaluationMetrics: EvaluationMetricsTypeDef,  # (4)
    LabelCount: int,
    Schema: List[SchemaColumnTypeDef],  # (5)
    Role: str,
    GlueVersion: str,
    MaxCapacity: float,
    WorkerType: WorkerTypeType,  # (6)
    NumberOfWorkers: int,
    Timeout: int,
    MaxRetries: int,
    TransformEncryption: TransformEncryptionTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: TransformStatusTypeType](./literals.md#transformstatustypetype) 
2. See [:material-code-braces: GlueTableTypeDef](./type_defs.md#gluetabletypedef) 
3. See [:material-code-braces: TransformParametersTypeDef](./type_defs.md#transformparameterstypedef) 
4. See [:material-code-braces: EvaluationMetricsTypeDef](./type_defs.md#evaluationmetricstypedef) 
5. See [:material-code-braces: SchemaColumnTypeDef](./type_defs.md#schemacolumntypedef) 
6. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
7. See [:material-code-braces: TransformEncryptionTypeDef](./type_defs.md#transformencryptiontypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MLTransformTypeDef

```python
# MLTransformTypeDef definition

class MLTransformTypeDef(TypedDict):
    TransformId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[TransformStatusTypeType],  # (1)
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    InputRecordTables: NotRequired[List[GlueTableTypeDef]],  # (2)
    Parameters: NotRequired[TransformParametersTypeDef],  # (3)
    EvaluationMetrics: NotRequired[EvaluationMetricsTypeDef],  # (4)
    LabelCount: NotRequired[int],
    Schema: NotRequired[List[SchemaColumnTypeDef]],  # (5)
    Role: NotRequired[str],
    GlueVersion: NotRequired[str],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (6)
    NumberOfWorkers: NotRequired[int],
    Timeout: NotRequired[int],
    MaxRetries: NotRequired[int],
    TransformEncryption: NotRequired[TransformEncryptionTypeDef],  # (7)
```

1. See [:material-code-brackets: TransformStatusTypeType](./literals.md#transformstatustypetype) 
2. See [:material-code-braces: GlueTableTypeDef](./type_defs.md#gluetabletypedef) 
3. See [:material-code-braces: TransformParametersTypeDef](./type_defs.md#transformparameterstypedef) 
4. See [:material-code-braces: EvaluationMetricsTypeDef](./type_defs.md#evaluationmetricstypedef) 
5. See [:material-code-braces: SchemaColumnTypeDef](./type_defs.md#schemacolumntypedef) 
6. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
7. See [:material-code-braces: TransformEncryptionTypeDef](./type_defs.md#transformencryptiontypedef) 
## BatchGetCrawlersResponseTypeDef

```python
# BatchGetCrawlersResponseTypeDef definition

class BatchGetCrawlersResponseTypeDef(TypedDict):
    Crawlers: List[CrawlerTypeDef],  # (1)
    CrawlersNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CrawlerTypeDef](./type_defs.md#crawlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCrawlerResponseTypeDef

```python
# GetCrawlerResponseTypeDef definition

class GetCrawlerResponseTypeDef(TypedDict):
    Crawler: CrawlerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CrawlerTypeDef](./type_defs.md#crawlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCrawlersResponseTypeDef

```python
# GetCrawlersResponseTypeDef definition

class GetCrawlersResponseTypeDef(TypedDict):
    Crawlers: List[CrawlerTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CrawlerTypeDef](./type_defs.md#crawlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataQualityResultsResponseTypeDef

```python
# ListDataQualityResultsResponseTypeDef definition

class ListDataQualityResultsResponseTypeDef(TypedDict):
    Results: List[DataQualityResultDescriptionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataQualityResultDescriptionTypeDef](./type_defs.md#dataqualityresultdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataQualityResultsRequestRequestTypeDef

```python
# ListDataQualityResultsRequestRequestTypeDef definition

class ListDataQualityResultsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[DataQualityResultFilterCriteriaTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DataQualityResultFilterCriteriaTypeDef](./type_defs.md#dataqualityresultfiltercriteriatypedef) 
## BatchGetDataQualityResultResponseTypeDef

```python
# BatchGetDataQualityResultResponseTypeDef definition

class BatchGetDataQualityResultResponseTypeDef(TypedDict):
    Results: List[DataQualityResultTypeDef],  # (1)
    ResultsNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataQualityResultTypeDef](./type_defs.md#dataqualityresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataQualityRuleRecommendationRunsResponseTypeDef

```python
# ListDataQualityRuleRecommendationRunsResponseTypeDef definition

class ListDataQualityRuleRecommendationRunsResponseTypeDef(TypedDict):
    Runs: List[DataQualityRuleRecommendationRunDescriptionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataQualityRuleRecommendationRunDescriptionTypeDef](./type_defs.md#dataqualityrulerecommendationrundescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataQualityRuleRecommendationRunsRequestRequestTypeDef

```python
# ListDataQualityRuleRecommendationRunsRequestRequestTypeDef definition

class ListDataQualityRuleRecommendationRunsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[DataQualityRuleRecommendationRunFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DataQualityRuleRecommendationRunFilterTypeDef](./type_defs.md#dataqualityrulerecommendationrunfiltertypedef) 
## ListDataQualityRulesetEvaluationRunsResponseTypeDef

```python
# ListDataQualityRulesetEvaluationRunsResponseTypeDef definition

class ListDataQualityRulesetEvaluationRunsResponseTypeDef(TypedDict):
    Runs: List[DataQualityRulesetEvaluationRunDescriptionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataQualityRulesetEvaluationRunDescriptionTypeDef](./type_defs.md#dataqualityrulesetevaluationrundescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef

```python
# ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef definition

class ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[DataQualityRulesetEvaluationRunFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DataQualityRulesetEvaluationRunFilterTypeDef](./type_defs.md#dataqualityrulesetevaluationrunfiltertypedef) 
## CreateDatabaseRequestRequestTypeDef

```python
# CreateDatabaseRequestRequestTypeDef definition

class CreateDatabaseRequestRequestTypeDef(TypedDict):
    DatabaseInput: DatabaseInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DatabaseInputTypeDef](./type_defs.md#databaseinputtypedef) 
## UpdateDatabaseRequestRequestTypeDef

```python
# UpdateDatabaseRequestRequestTypeDef definition

class UpdateDatabaseRequestRequestTypeDef(TypedDict):
    Name: str,
    DatabaseInput: DatabaseInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: DatabaseInputTypeDef](./type_defs.md#databaseinputtypedef) 
## GetDatabaseResponseTypeDef

```python
# GetDatabaseResponseTypeDef definition

class GetDatabaseResponseTypeDef(TypedDict):
    Database: DatabaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDatabasesResponseTypeDef

```python
# GetDatabasesResponseTypeDef definition

class GetDatabasesResponseTypeDef(TypedDict):
    DatabaseList: List[DatabaseTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ColumnStatisticsTypeDef

```python
# ColumnStatisticsTypeDef definition

class ColumnStatisticsTypeDef(TypedDict):
    ColumnName: str,
    ColumnType: str,
    AnalyzedTime: datetime,
    StatisticsData: ColumnStatisticsDataTypeDef,  # (1)
```

1. See [:material-code-braces: ColumnStatisticsDataTypeDef](./type_defs.md#columnstatisticsdatatypedef) 
## PartitionInputTypeDef

```python
# PartitionInputTypeDef definition

class PartitionInputTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
    LastAccessTime: NotRequired[Union[datetime, str]],
    StorageDescriptor: NotRequired[StorageDescriptorTypeDef],  # (1)
    Parameters: NotRequired[Mapping[str, str]],
    LastAnalyzedTime: NotRequired[Union[datetime, str]],
```

1. See [:material-code-braces: StorageDescriptorTypeDef](./type_defs.md#storagedescriptortypedef) 
## PartitionTypeDef

```python
# PartitionTypeDef definition

class PartitionTypeDef(TypedDict):
    Values: NotRequired[List[str]],
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastAccessTime: NotRequired[datetime],
    StorageDescriptor: NotRequired[StorageDescriptorTypeDef],  # (1)
    Parameters: NotRequired[Dict[str, str]],
    LastAnalyzedTime: NotRequired[datetime],
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: StorageDescriptorTypeDef](./type_defs.md#storagedescriptortypedef) 
## TableInputTypeDef

```python
# TableInputTypeDef definition

class TableInputTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    Owner: NotRequired[str],
    LastAccessTime: NotRequired[Union[datetime, str]],
    LastAnalyzedTime: NotRequired[Union[datetime, str]],
    Retention: NotRequired[int],
    StorageDescriptor: NotRequired[StorageDescriptorTypeDef],  # (1)
    PartitionKeys: NotRequired[Sequence[ColumnTypeDef]],  # (2)
    ViewOriginalText: NotRequired[str],
    ViewExpandedText: NotRequired[str],
    TableType: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
    TargetTable: NotRequired[TableIdentifierTypeDef],  # (3)
```

1. See [:material-code-braces: StorageDescriptorTypeDef](./type_defs.md#storagedescriptortypedef) 
2. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
3. See [:material-code-braces: TableIdentifierTypeDef](./type_defs.md#tableidentifiertypedef) 
## TableTypeDef

```python
# TableTypeDef definition

class TableTypeDef(TypedDict):
    Name: str,
    DatabaseName: NotRequired[str],
    Description: NotRequired[str],
    Owner: NotRequired[str],
    CreateTime: NotRequired[datetime],
    UpdateTime: NotRequired[datetime],
    LastAccessTime: NotRequired[datetime],
    LastAnalyzedTime: NotRequired[datetime],
    Retention: NotRequired[int],
    StorageDescriptor: NotRequired[StorageDescriptorTypeDef],  # (1)
    PartitionKeys: NotRequired[List[ColumnTypeDef]],  # (2)
    ViewOriginalText: NotRequired[str],
    ViewExpandedText: NotRequired[str],
    TableType: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
    CreatedBy: NotRequired[str],
    IsRegisteredWithLakeFormation: NotRequired[bool],
    TargetTable: NotRequired[TableIdentifierTypeDef],  # (3)
    CatalogId: NotRequired[str],
    VersionId: NotRequired[str],
    FederatedTable: NotRequired[FederatedTableTypeDef],  # (4)
```

1. See [:material-code-braces: StorageDescriptorTypeDef](./type_defs.md#storagedescriptortypedef) 
2. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
3. See [:material-code-braces: TableIdentifierTypeDef](./type_defs.md#tableidentifiertypedef) 
4. See [:material-code-braces: FederatedTableTypeDef](./type_defs.md#federatedtabletypedef) 
## GetSecurityConfigurationResponseTypeDef

```python
# GetSecurityConfigurationResponseTypeDef definition

class GetSecurityConfigurationResponseTypeDef(TypedDict):
    SecurityConfiguration: SecurityConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityConfigurationTypeDef](./type_defs.md#securityconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSecurityConfigurationsResponseTypeDef

```python
# GetSecurityConfigurationsResponseTypeDef definition

class GetSecurityConfigurationsResponseTypeDef(TypedDict):
    SecurityConfigurations: List[SecurityConfigurationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityConfigurationTypeDef](./type_defs.md#securityconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CodeGenConfigurationNodeTypeDef

```python
# CodeGenConfigurationNodeTypeDef definition

class CodeGenConfigurationNodeTypeDef(TypedDict):
    AthenaConnectorSource: NotRequired[AthenaConnectorSourceTypeDef],  # (1)
    JDBCConnectorSource: NotRequired[JDBCConnectorSourceTypeDef],  # (2)
    SparkConnectorSource: NotRequired[SparkConnectorSourceTypeDef],  # (3)
    CatalogSource: NotRequired[CatalogSourceTypeDef],  # (4)
    RedshiftSource: NotRequired[RedshiftSourceTypeDef],  # (5)
    S3CatalogSource: NotRequired[S3CatalogSourceTypeDef],  # (6)
    S3CsvSource: NotRequired[S3CsvSourceTypeDef],  # (7)
    S3JsonSource: NotRequired[S3JsonSourceTypeDef],  # (8)
    S3ParquetSource: NotRequired[S3ParquetSourceTypeDef],  # (9)
    RelationalCatalogSource: NotRequired[RelationalCatalogSourceTypeDef],  # (10)
    DynamoDBCatalogSource: NotRequired[DynamoDBCatalogSourceTypeDef],  # (11)
    JDBCConnectorTarget: NotRequired[JDBCConnectorTargetTypeDef],  # (12)
    SparkConnectorTarget: NotRequired[SparkConnectorTargetTypeDef],  # (13)
    CatalogTarget: NotRequired[BasicCatalogTargetTypeDef],  # (14)
    RedshiftTarget: NotRequired[RedshiftTargetTypeDef],  # (15)
    S3CatalogTarget: NotRequired[S3CatalogTargetTypeDef],  # (16)
    S3GlueParquetTarget: NotRequired[S3GlueParquetTargetTypeDef],  # (17)
    S3DirectTarget: NotRequired[S3DirectTargetTypeDef],  # (18)
    ApplyMapping: NotRequired[ApplyMappingTypeDef],  # (19)
    SelectFields: NotRequired[SelectFieldsTypeDef],  # (20)
    DropFields: NotRequired[DropFieldsTypeDef],  # (21)
    RenameField: NotRequired[RenameFieldTypeDef],  # (22)
    Spigot: NotRequired[SpigotTypeDef],  # (23)
    Join: NotRequired[JoinTypeDef],  # (24)
    SplitFields: NotRequired[SplitFieldsTypeDef],  # (25)
    SelectFromCollection: NotRequired[SelectFromCollectionTypeDef],  # (26)
    FillMissingValues: NotRequired[FillMissingValuesTypeDef],  # (27)
    Filter: NotRequired[FilterTypeDef],  # (28)
    CustomCode: NotRequired[CustomCodeTypeDef],  # (29)
    SparkSQL: NotRequired[SparkSQLTypeDef],  # (30)
    DirectKinesisSource: NotRequired[DirectKinesisSourceTypeDef],  # (31)
    DirectKafkaSource: NotRequired[DirectKafkaSourceTypeDef],  # (32)
    CatalogKinesisSource: NotRequired[CatalogKinesisSourceTypeDef],  # (33)
    CatalogKafkaSource: NotRequired[CatalogKafkaSourceTypeDef],  # (34)
    DropNullFields: NotRequired[DropNullFieldsTypeDef],  # (35)
    Merge: NotRequired[MergeTypeDef],  # (36)
    Union: NotRequired[UnionTypeDef],  # (37)
    PIIDetection: NotRequired[PIIDetectionTypeDef],  # (38)
    Aggregate: NotRequired[AggregateTypeDef],  # (39)
    DropDuplicates: NotRequired[DropDuplicatesTypeDef],  # (40)
    GovernedCatalogTarget: NotRequired[GovernedCatalogTargetTypeDef],  # (41)
    GovernedCatalogSource: NotRequired[GovernedCatalogSourceTypeDef],  # (42)
    MicrosoftSQLServerCatalogSource: NotRequired[MicrosoftSQLServerCatalogSourceTypeDef],  # (43)
    MySQLCatalogSource: NotRequired[MySQLCatalogSourceTypeDef],  # (44)
    OracleSQLCatalogSource: NotRequired[OracleSQLCatalogSourceTypeDef],  # (45)
    PostgreSQLCatalogSource: NotRequired[PostgreSQLCatalogSourceTypeDef],  # (46)
    MicrosoftSQLServerCatalogTarget: NotRequired[MicrosoftSQLServerCatalogTargetTypeDef],  # (47)
    MySQLCatalogTarget: NotRequired[MySQLCatalogTargetTypeDef],  # (48)
    OracleSQLCatalogTarget: NotRequired[OracleSQLCatalogTargetTypeDef],  # (49)
    PostgreSQLCatalogTarget: NotRequired[PostgreSQLCatalogTargetTypeDef],  # (50)
    DynamicTransform: NotRequired[DynamicTransformTypeDef],  # (51)
    EvaluateDataQuality: NotRequired[EvaluateDataQualityTypeDef],  # (52)
    S3CatalogHudiSource: NotRequired[S3CatalogHudiSourceTypeDef],  # (53)
    CatalogHudiSource: NotRequired[CatalogHudiSourceTypeDef],  # (54)
    S3HudiSource: NotRequired[S3HudiSourceTypeDef],  # (55)
    S3HudiCatalogTarget: NotRequired[S3HudiCatalogTargetTypeDef],  # (56)
    S3HudiDirectTarget: NotRequired[S3HudiDirectTargetTypeDef],  # (57)
    DirectJDBCSource: NotRequired[DirectJDBCSourceTypeDef],  # (58)
    S3CatalogDeltaSource: NotRequired[S3CatalogDeltaSourceTypeDef],  # (59)
    CatalogDeltaSource: NotRequired[CatalogDeltaSourceTypeDef],  # (60)
    S3DeltaSource: NotRequired[S3DeltaSourceTypeDef],  # (61)
    S3DeltaCatalogTarget: NotRequired[S3DeltaCatalogTargetTypeDef],  # (62)
    S3DeltaDirectTarget: NotRequired[S3DeltaDirectTargetTypeDef],  # (63)
    AmazonRedshiftSource: NotRequired[AmazonRedshiftSourceTypeDef],  # (64)
    AmazonRedshiftTarget: NotRequired[AmazonRedshiftTargetTypeDef],  # (65)
    EvaluateDataQualityMultiFrame: NotRequired[EvaluateDataQualityMultiFrameTypeDef],  # (66)
    Recipe: NotRequired[RecipeTypeDef],  # (67)
    SnowflakeSource: NotRequired[SnowflakeSourceTypeDef],  # (68)
    SnowflakeTarget: NotRequired[SnowflakeTargetTypeDef],  # (69)
```

1. See [:material-code-braces: AthenaConnectorSourceTypeDef](./type_defs.md#athenaconnectorsourcetypedef) 
2. See [:material-code-braces: JDBCConnectorSourceTypeDef](./type_defs.md#jdbcconnectorsourcetypedef) 
3. See [:material-code-braces: SparkConnectorSourceTypeDef](./type_defs.md#sparkconnectorsourcetypedef) 
4. See [:material-code-braces: CatalogSourceTypeDef](./type_defs.md#catalogsourcetypedef) 
5. See [:material-code-braces: RedshiftSourceTypeDef](./type_defs.md#redshiftsourcetypedef) 
6. See [:material-code-braces: S3CatalogSourceTypeDef](./type_defs.md#s3catalogsourcetypedef) 
7. See [:material-code-braces: S3CsvSourceTypeDef](./type_defs.md#s3csvsourcetypedef) 
8. See [:material-code-braces: S3JsonSourceTypeDef](./type_defs.md#s3jsonsourcetypedef) 
9. See [:material-code-braces: S3ParquetSourceTypeDef](./type_defs.md#s3parquetsourcetypedef) 
10. See [:material-code-braces: RelationalCatalogSourceTypeDef](./type_defs.md#relationalcatalogsourcetypedef) 
11. See [:material-code-braces: DynamoDBCatalogSourceTypeDef](./type_defs.md#dynamodbcatalogsourcetypedef) 
12. See [:material-code-braces: JDBCConnectorTargetTypeDef](./type_defs.md#jdbcconnectortargettypedef) 
13. See [:material-code-braces: SparkConnectorTargetTypeDef](./type_defs.md#sparkconnectortargettypedef) 
14. See [:material-code-braces: BasicCatalogTargetTypeDef](./type_defs.md#basiccatalogtargettypedef) 
15. See [:material-code-braces: RedshiftTargetTypeDef](./type_defs.md#redshifttargettypedef) 
16. See [:material-code-braces: S3CatalogTargetTypeDef](./type_defs.md#s3catalogtargettypedef) 
17. See [:material-code-braces: S3GlueParquetTargetTypeDef](./type_defs.md#s3glueparquettargettypedef) 
18. See [:material-code-braces: S3DirectTargetTypeDef](./type_defs.md#s3directtargettypedef) 
19. See [:material-code-braces: ApplyMappingTypeDef](./type_defs.md#applymappingtypedef) 
20. See [:material-code-braces: SelectFieldsTypeDef](./type_defs.md#selectfieldstypedef) 
21. See [:material-code-braces: DropFieldsTypeDef](./type_defs.md#dropfieldstypedef) 
22. See [:material-code-braces: RenameFieldTypeDef](./type_defs.md#renamefieldtypedef) 
23. See [:material-code-braces: SpigotTypeDef](./type_defs.md#spigottypedef) 
24. See [:material-code-braces: JoinTypeDef](./type_defs.md#jointypedef) 
25. See [:material-code-braces: SplitFieldsTypeDef](./type_defs.md#splitfieldstypedef) 
26. See [:material-code-braces: SelectFromCollectionTypeDef](./type_defs.md#selectfromcollectiontypedef) 
27. See [:material-code-braces: FillMissingValuesTypeDef](./type_defs.md#fillmissingvaluestypedef) 
28. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
29. See [:material-code-braces: CustomCodeTypeDef](./type_defs.md#customcodetypedef) 
30. See [:material-code-braces: SparkSQLTypeDef](./type_defs.md#sparksqltypedef) 
31. See [:material-code-braces: DirectKinesisSourceTypeDef](./type_defs.md#directkinesissourcetypedef) 
32. See [:material-code-braces: DirectKafkaSourceTypeDef](./type_defs.md#directkafkasourcetypedef) 
33. See [:material-code-braces: CatalogKinesisSourceTypeDef](./type_defs.md#catalogkinesissourcetypedef) 
34. See [:material-code-braces: CatalogKafkaSourceTypeDef](./type_defs.md#catalogkafkasourcetypedef) 
35. See [:material-code-braces: DropNullFieldsTypeDef](./type_defs.md#dropnullfieldstypedef) 
36. See [:material-code-braces: MergeTypeDef](./type_defs.md#mergetypedef) 
37. See [:material-code-braces: UnionTypeDef](./type_defs.md#uniontypedef) 
38. See [:material-code-braces: PIIDetectionTypeDef](./type_defs.md#piidetectiontypedef) 
39. See [:material-code-braces: AggregateTypeDef](./type_defs.md#aggregatetypedef) 
40. See [:material-code-braces: DropDuplicatesTypeDef](./type_defs.md#dropduplicatestypedef) 
41. See [:material-code-braces: GovernedCatalogTargetTypeDef](./type_defs.md#governedcatalogtargettypedef) 
42. See [:material-code-braces: GovernedCatalogSourceTypeDef](./type_defs.md#governedcatalogsourcetypedef) 
43. See [:material-code-braces: MicrosoftSQLServerCatalogSourceTypeDef](./type_defs.md#microsoftsqlservercatalogsourcetypedef) 
44. See [:material-code-braces: MySQLCatalogSourceTypeDef](./type_defs.md#mysqlcatalogsourcetypedef) 
45. See [:material-code-braces: OracleSQLCatalogSourceTypeDef](./type_defs.md#oraclesqlcatalogsourcetypedef) 
46. See [:material-code-braces: PostgreSQLCatalogSourceTypeDef](./type_defs.md#postgresqlcatalogsourcetypedef) 
47. See [:material-code-braces: MicrosoftSQLServerCatalogTargetTypeDef](./type_defs.md#microsoftsqlservercatalogtargettypedef) 
48. See [:material-code-braces: MySQLCatalogTargetTypeDef](./type_defs.md#mysqlcatalogtargettypedef) 
49. See [:material-code-braces: OracleSQLCatalogTargetTypeDef](./type_defs.md#oraclesqlcatalogtargettypedef) 
50. See [:material-code-braces: PostgreSQLCatalogTargetTypeDef](./type_defs.md#postgresqlcatalogtargettypedef) 
51. See [:material-code-braces: DynamicTransformTypeDef](./type_defs.md#dynamictransformtypedef) 
52. See [:material-code-braces: EvaluateDataQualityTypeDef](./type_defs.md#evaluatedataqualitytypedef) 
53. See [:material-code-braces: S3CatalogHudiSourceTypeDef](./type_defs.md#s3cataloghudisourcetypedef) 
54. See [:material-code-braces: CatalogHudiSourceTypeDef](./type_defs.md#cataloghudisourcetypedef) 
55. See [:material-code-braces: S3HudiSourceTypeDef](./type_defs.md#s3hudisourcetypedef) 
56. See [:material-code-braces: S3HudiCatalogTargetTypeDef](./type_defs.md#s3hudicatalogtargettypedef) 
57. See [:material-code-braces: S3HudiDirectTargetTypeDef](./type_defs.md#s3hudidirecttargettypedef) 
58. See [:material-code-braces: DirectJDBCSourceTypeDef](./type_defs.md#directjdbcsourcetypedef) 
59. See [:material-code-braces: S3CatalogDeltaSourceTypeDef](./type_defs.md#s3catalogdeltasourcetypedef) 
60. See [:material-code-braces: CatalogDeltaSourceTypeDef](./type_defs.md#catalogdeltasourcetypedef) 
61. See [:material-code-braces: S3DeltaSourceTypeDef](./type_defs.md#s3deltasourcetypedef) 
62. See [:material-code-braces: S3DeltaCatalogTargetTypeDef](./type_defs.md#s3deltacatalogtargettypedef) 
63. See [:material-code-braces: S3DeltaDirectTargetTypeDef](./type_defs.md#s3deltadirecttargettypedef) 
64. See [:material-code-braces: AmazonRedshiftSourceTypeDef](./type_defs.md#amazonredshiftsourcetypedef) 
65. See [:material-code-braces: AmazonRedshiftTargetTypeDef](./type_defs.md#amazonredshifttargettypedef) 
66. See [:material-code-braces: EvaluateDataQualityMultiFrameTypeDef](./type_defs.md#evaluatedataqualitymultiframetypedef) 
67. See [:material-code-braces: RecipeTypeDef](./type_defs.md#recipetypedef) 
68. See [:material-code-braces: SnowflakeSourceTypeDef](./type_defs.md#snowflakesourcetypedef) 
69. See [:material-code-braces: SnowflakeTargetTypeDef](./type_defs.md#snowflaketargettypedef) 
## GetMLTaskRunsResponseTypeDef

```python
# GetMLTaskRunsResponseTypeDef definition

class GetMLTaskRunsResponseTypeDef(TypedDict):
    TaskRuns: List[TaskRunTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TaskRunTypeDef](./type_defs.md#taskruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStatementResponseTypeDef

```python
# GetStatementResponseTypeDef definition

class GetStatementResponseTypeDef(TypedDict):
    Statement: StatementTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStatementsResponseTypeDef

```python
# ListStatementsResponseTypeDef definition

class ListStatementsResponseTypeDef(TypedDict):
    Statements: List[StatementTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NodeTypeDef

```python
# NodeTypeDef definition

class NodeTypeDef(TypedDict):
    Type: NotRequired[NodeTypeType],  # (1)
    Name: NotRequired[str],
    UniqueId: NotRequired[str],
    TriggerDetails: NotRequired[TriggerNodeDetailsTypeDef],  # (2)
    JobDetails: NotRequired[JobNodeDetailsTypeDef],  # (3)
    CrawlerDetails: NotRequired[CrawlerNodeDetailsTypeDef],  # (4)
```

1. See [:material-code-brackets: NodeTypeType](./literals.md#nodetypetype) 
2. See [:material-code-braces: TriggerNodeDetailsTypeDef](./type_defs.md#triggernodedetailstypedef) 
3. See [:material-code-braces: JobNodeDetailsTypeDef](./type_defs.md#jobnodedetailstypedef) 
4. See [:material-code-braces: CrawlerNodeDetailsTypeDef](./type_defs.md#crawlernodedetailstypedef) 
## GetMLTransformsResponseTypeDef

```python
# GetMLTransformsResponseTypeDef definition

class GetMLTransformsResponseTypeDef(TypedDict):
    Transforms: List[MLTransformTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MLTransformTypeDef](./type_defs.md#mltransformtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ColumnStatisticsErrorTypeDef

```python
# ColumnStatisticsErrorTypeDef definition

class ColumnStatisticsErrorTypeDef(TypedDict):
    ColumnStatistics: NotRequired[ColumnStatisticsTypeDef],  # (1)
    Error: NotRequired[ErrorDetailTypeDef],  # (2)
```

1. See [:material-code-braces: ColumnStatisticsTypeDef](./type_defs.md#columnstatisticstypedef) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## GetColumnStatisticsForPartitionResponseTypeDef

```python
# GetColumnStatisticsForPartitionResponseTypeDef definition

class GetColumnStatisticsForPartitionResponseTypeDef(TypedDict):
    ColumnStatisticsList: List[ColumnStatisticsTypeDef],  # (1)
    Errors: List[ColumnErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ColumnStatisticsTypeDef](./type_defs.md#columnstatisticstypedef) 
2. See [:material-code-braces: ColumnErrorTypeDef](./type_defs.md#columnerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetColumnStatisticsForTableResponseTypeDef

```python
# GetColumnStatisticsForTableResponseTypeDef definition

class GetColumnStatisticsForTableResponseTypeDef(TypedDict):
    ColumnStatisticsList: List[ColumnStatisticsTypeDef],  # (1)
    Errors: List[ColumnErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ColumnStatisticsTypeDef](./type_defs.md#columnstatisticstypedef) 
2. See [:material-code-braces: ColumnErrorTypeDef](./type_defs.md#columnerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateColumnStatisticsForPartitionRequestRequestTypeDef

```python
# UpdateColumnStatisticsForPartitionRequestRequestTypeDef definition

class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: ColumnStatisticsTypeDef](./type_defs.md#columnstatisticstypedef) 
## UpdateColumnStatisticsForTableRequestRequestTypeDef

```python
# UpdateColumnStatisticsForTableRequestRequestTypeDef definition

class UpdateColumnStatisticsForTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: ColumnStatisticsTypeDef](./type_defs.md#columnstatisticstypedef) 
## BatchCreatePartitionRequestRequestTypeDef

```python
# BatchCreatePartitionRequestRequestTypeDef definition

class BatchCreatePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionInputList: Sequence[PartitionInputTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionInputTypeDef](./type_defs.md#partitioninputtypedef) 
## BatchUpdatePartitionRequestEntryTypeDef

```python
# BatchUpdatePartitionRequestEntryTypeDef definition

class BatchUpdatePartitionRequestEntryTypeDef(TypedDict):
    PartitionValueList: Sequence[str],
    PartitionInput: PartitionInputTypeDef,  # (1)
```

1. See [:material-code-braces: PartitionInputTypeDef](./type_defs.md#partitioninputtypedef) 
## CreatePartitionRequestRequestTypeDef

```python
# CreatePartitionRequestRequestTypeDef definition

class CreatePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionInput: PartitionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionInputTypeDef](./type_defs.md#partitioninputtypedef) 
## UpdatePartitionRequestRequestTypeDef

```python
# UpdatePartitionRequestRequestTypeDef definition

class UpdatePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValueList: Sequence[str],
    PartitionInput: PartitionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionInputTypeDef](./type_defs.md#partitioninputtypedef) 
## BatchGetPartitionResponseTypeDef

```python
# BatchGetPartitionResponseTypeDef definition

class BatchGetPartitionResponseTypeDef(TypedDict):
    Partitions: List[PartitionTypeDef],  # (1)
    UnprocessedKeys: List[PartitionValueListTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
2. See [:material-code-braces: PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPartitionResponseTypeDef

```python
# GetPartitionResponseTypeDef definition

class GetPartitionResponseTypeDef(TypedDict):
    Partition: PartitionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPartitionsResponseTypeDef

```python
# GetPartitionsResponseTypeDef definition

class GetPartitionsResponseTypeDef(TypedDict):
    Partitions: List[PartitionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUnfilteredPartitionMetadataResponseTypeDef

```python
# GetUnfilteredPartitionMetadataResponseTypeDef definition

class GetUnfilteredPartitionMetadataResponseTypeDef(TypedDict):
    Partition: PartitionTypeDef,  # (1)
    AuthorizedColumns: List[str],
    IsRegisteredWithLakeFormation: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UnfilteredPartitionTypeDef

```python
# UnfilteredPartitionTypeDef definition

class UnfilteredPartitionTypeDef(TypedDict):
    Partition: NotRequired[PartitionTypeDef],  # (1)
    AuthorizedColumns: NotRequired[List[str]],
    IsRegisteredWithLakeFormation: NotRequired[bool],
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
## CreateTableRequestRequestTypeDef

```python
# CreateTableRequestRequestTypeDef definition

class CreateTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableInput: TableInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
    PartitionIndexes: NotRequired[Sequence[PartitionIndexTypeDef]],  # (2)
    TransactionId: NotRequired[str],
    OpenTableFormatInput: NotRequired[OpenTableFormatInputTypeDef],  # (3)
```

1. See [:material-code-braces: TableInputTypeDef](./type_defs.md#tableinputtypedef) 
2. See [:material-code-braces: PartitionIndexTypeDef](./type_defs.md#partitionindextypedef) 
3. See [:material-code-braces: OpenTableFormatInputTypeDef](./type_defs.md#opentableformatinputtypedef) 
## UpdateTableRequestRequestTypeDef

```python
# UpdateTableRequestRequestTypeDef definition

class UpdateTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableInput: TableInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
    SkipArchive: NotRequired[bool],
    TransactionId: NotRequired[str],
    VersionId: NotRequired[str],
```

1. See [:material-code-braces: TableInputTypeDef](./type_defs.md#tableinputtypedef) 
## GetTableResponseTypeDef

```python
# GetTableResponseTypeDef definition

class GetTableResponseTypeDef(TypedDict):
    Table: TableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTablesResponseTypeDef

```python
# GetTablesResponseTypeDef definition

class GetTablesResponseTypeDef(TypedDict):
    TableList: List[TableTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUnfilteredTableMetadataResponseTypeDef

```python
# GetUnfilteredTableMetadataResponseTypeDef definition

class GetUnfilteredTableMetadataResponseTypeDef(TypedDict):
    Table: TableTypeDef,  # (1)
    AuthorizedColumns: List[str],
    IsRegisteredWithLakeFormation: bool,
    CellFilters: List[ColumnRowFilterTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ColumnRowFilterTypeDef](./type_defs.md#columnrowfiltertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchTablesResponseTypeDef

```python
# SearchTablesResponseTypeDef definition

class SearchTablesResponseTypeDef(TypedDict):
    NextToken: str,
    TableList: List[TableTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableVersionTypeDef

```python
# TableVersionTypeDef definition

class TableVersionTypeDef(TypedDict):
    Table: NotRequired[TableTypeDef],  # (1)
    VersionId: NotRequired[str],
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
## CreateJobRequestRequestTypeDef

```python
# CreateJobRequestRequestTypeDef definition

class CreateJobRequestRequestTypeDef(TypedDict):
    Name: str,
    Role: str,
    Command: JobCommandTypeDef,  # (1)
    Description: NotRequired[str],
    LogUri: NotRequired[str],
    ExecutionProperty: NotRequired[ExecutionPropertyTypeDef],  # (2)
    DefaultArguments: NotRequired[Mapping[str, str]],
    NonOverridableArguments: NotRequired[Mapping[str, str]],
    Connections: NotRequired[ConnectionsListTypeDef],  # (3)
    MaxRetries: NotRequired[int],
    AllocatedCapacity: NotRequired[int],
    Timeout: NotRequired[int],
    MaxCapacity: NotRequired[float],
    SecurityConfiguration: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (4)
    GlueVersion: NotRequired[str],
    NumberOfWorkers: NotRequired[int],
    WorkerType: NotRequired[WorkerTypeType],  # (5)
    CodeGenConfigurationNodes: NotRequired[Mapping[str, CodeGenConfigurationNodeTypeDef]],  # (6)
    ExecutionClass: NotRequired[ExecutionClassType],  # (7)
    SourceControlDetails: NotRequired[SourceControlDetailsTypeDef],  # (8)
```

1. See [:material-code-braces: JobCommandTypeDef](./type_defs.md#jobcommandtypedef) 
2. See [:material-code-braces: ExecutionPropertyTypeDef](./type_defs.md#executionpropertytypedef) 
3. See [:material-code-braces: ConnectionsListTypeDef](./type_defs.md#connectionslisttypedef) 
4. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
5. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
6. See [:material-code-braces: CodeGenConfigurationNodeTypeDef](./type_defs.md#codegenconfigurationnodetypedef) 
7. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
8. See [:material-code-braces: SourceControlDetailsTypeDef](./type_defs.md#sourcecontroldetailstypedef) 
## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    LogUri: NotRequired[str],
    Role: NotRequired[str],
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    ExecutionProperty: NotRequired[ExecutionPropertyTypeDef],  # (1)
    Command: NotRequired[JobCommandTypeDef],  # (2)
    DefaultArguments: NotRequired[Dict[str, str]],
    NonOverridableArguments: NotRequired[Dict[str, str]],
    Connections: NotRequired[ConnectionsListTypeDef],  # (3)
    MaxRetries: NotRequired[int],
    AllocatedCapacity: NotRequired[int],
    Timeout: NotRequired[int],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (4)
    NumberOfWorkers: NotRequired[int],
    SecurityConfiguration: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (5)
    GlueVersion: NotRequired[str],
    CodeGenConfigurationNodes: NotRequired[Dict[str, CodeGenConfigurationNodeTypeDef]],  # (6)
    ExecutionClass: NotRequired[ExecutionClassType],  # (7)
    SourceControlDetails: NotRequired[SourceControlDetailsTypeDef],  # (8)
```

1. See [:material-code-braces: ExecutionPropertyTypeDef](./type_defs.md#executionpropertytypedef) 
2. See [:material-code-braces: JobCommandTypeDef](./type_defs.md#jobcommandtypedef) 
3. See [:material-code-braces: ConnectionsListTypeDef](./type_defs.md#connectionslisttypedef) 
4. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
5. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
6. See [:material-code-braces: CodeGenConfigurationNodeTypeDef](./type_defs.md#codegenconfigurationnodetypedef) 
7. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
8. See [:material-code-braces: SourceControlDetailsTypeDef](./type_defs.md#sourcecontroldetailstypedef) 
## JobUpdateTypeDef

```python
# JobUpdateTypeDef definition

class JobUpdateTypeDef(TypedDict):
    Description: NotRequired[str],
    LogUri: NotRequired[str],
    Role: NotRequired[str],
    ExecutionProperty: NotRequired[ExecutionPropertyTypeDef],  # (1)
    Command: NotRequired[JobCommandTypeDef],  # (2)
    DefaultArguments: NotRequired[Mapping[str, str]],
    NonOverridableArguments: NotRequired[Mapping[str, str]],
    Connections: NotRequired[ConnectionsListTypeDef],  # (3)
    MaxRetries: NotRequired[int],
    AllocatedCapacity: NotRequired[int],
    Timeout: NotRequired[int],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (4)
    NumberOfWorkers: NotRequired[int],
    SecurityConfiguration: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (5)
    GlueVersion: NotRequired[str],
    CodeGenConfigurationNodes: NotRequired[Mapping[str, CodeGenConfigurationNodeTypeDef]],  # (6)
    ExecutionClass: NotRequired[ExecutionClassType],  # (7)
    SourceControlDetails: NotRequired[SourceControlDetailsTypeDef],  # (8)
```

1. See [:material-code-braces: ExecutionPropertyTypeDef](./type_defs.md#executionpropertytypedef) 
2. See [:material-code-braces: JobCommandTypeDef](./type_defs.md#jobcommandtypedef) 
3. See [:material-code-braces: ConnectionsListTypeDef](./type_defs.md#connectionslisttypedef) 
4. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
5. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
6. See [:material-code-braces: CodeGenConfigurationNodeTypeDef](./type_defs.md#codegenconfigurationnodetypedef) 
7. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
8. See [:material-code-braces: SourceControlDetailsTypeDef](./type_defs.md#sourcecontroldetailstypedef) 
## WorkflowGraphTypeDef

```python
# WorkflowGraphTypeDef definition

class WorkflowGraphTypeDef(TypedDict):
    Nodes: NotRequired[List[NodeTypeDef]],  # (1)
    Edges: NotRequired[List[EdgeTypeDef]],  # (2)
```

1. See [:material-code-braces: NodeTypeDef](./type_defs.md#nodetypedef) 
2. See [:material-code-braces: EdgeTypeDef](./type_defs.md#edgetypedef) 
## UpdateColumnStatisticsForPartitionResponseTypeDef

```python
# UpdateColumnStatisticsForPartitionResponseTypeDef definition

class UpdateColumnStatisticsForPartitionResponseTypeDef(TypedDict):
    Errors: List[ColumnStatisticsErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnStatisticsErrorTypeDef](./type_defs.md#columnstatisticserrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateColumnStatisticsForTableResponseTypeDef

```python
# UpdateColumnStatisticsForTableResponseTypeDef definition

class UpdateColumnStatisticsForTableResponseTypeDef(TypedDict):
    Errors: List[ColumnStatisticsErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnStatisticsErrorTypeDef](./type_defs.md#columnstatisticserrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdatePartitionRequestRequestTypeDef

```python
# BatchUpdatePartitionRequestRequestTypeDef definition

class BatchUpdatePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    Entries: Sequence[BatchUpdatePartitionRequestEntryTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: BatchUpdatePartitionRequestEntryTypeDef](./type_defs.md#batchupdatepartitionrequestentrytypedef) 
## GetUnfilteredPartitionsMetadataResponseTypeDef

```python
# GetUnfilteredPartitionsMetadataResponseTypeDef definition

class GetUnfilteredPartitionsMetadataResponseTypeDef(TypedDict):
    UnfilteredPartitions: List[UnfilteredPartitionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnfilteredPartitionTypeDef](./type_defs.md#unfilteredpartitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableVersionResponseTypeDef

```python
# GetTableVersionResponseTypeDef definition

class GetTableVersionResponseTypeDef(TypedDict):
    TableVersion: TableVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableVersionTypeDef](./type_defs.md#tableversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableVersionsResponseTypeDef

```python
# GetTableVersionsResponseTypeDef definition

class GetTableVersionsResponseTypeDef(TypedDict):
    TableVersions: List[TableVersionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableVersionTypeDef](./type_defs.md#tableversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetJobsResponseTypeDef

```python
# BatchGetJobsResponseTypeDef definition

class BatchGetJobsResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    JobsNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobResponseTypeDef

```python
# GetJobResponseTypeDef definition

class GetJobResponseTypeDef(TypedDict):
    Job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobsResponseTypeDef

```python
# GetJobsResponseTypeDef definition

class GetJobsResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateJobRequestRequestTypeDef

```python
# UpdateJobRequestRequestTypeDef definition

class UpdateJobRequestRequestTypeDef(TypedDict):
    JobName: str,
    JobUpdate: JobUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: JobUpdateTypeDef](./type_defs.md#jobupdatetypedef) 
## WorkflowRunTypeDef

```python
# WorkflowRunTypeDef definition

class WorkflowRunTypeDef(TypedDict):
    Name: NotRequired[str],
    WorkflowRunId: NotRequired[str],
    PreviousRunId: NotRequired[str],
    WorkflowRunProperties: NotRequired[Dict[str, str]],
    StartedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    Status: NotRequired[WorkflowRunStatusType],  # (1)
    ErrorMessage: NotRequired[str],
    Statistics: NotRequired[WorkflowRunStatisticsTypeDef],  # (2)
    Graph: NotRequired[WorkflowGraphTypeDef],  # (3)
    StartingEventBatchCondition: NotRequired[StartingEventBatchConditionTypeDef],  # (4)
```

1. See [:material-code-brackets: WorkflowRunStatusType](./literals.md#workflowrunstatustype) 
2. See [:material-code-braces: WorkflowRunStatisticsTypeDef](./type_defs.md#workflowrunstatisticstypedef) 
3. See [:material-code-braces: WorkflowGraphTypeDef](./type_defs.md#workflowgraphtypedef) 
4. See [:material-code-braces: StartingEventBatchConditionTypeDef](./type_defs.md#startingeventbatchconditiontypedef) 
## GetWorkflowRunResponseTypeDef

```python
# GetWorkflowRunResponseTypeDef definition

class GetWorkflowRunResponseTypeDef(TypedDict):
    Run: WorkflowRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkflowRunTypeDef](./type_defs.md#workflowruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkflowRunsResponseTypeDef

```python
# GetWorkflowRunsResponseTypeDef definition

class GetWorkflowRunsResponseTypeDef(TypedDict):
    Runs: List[WorkflowRunTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkflowRunTypeDef](./type_defs.md#workflowruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkflowTypeDef

```python
# WorkflowTypeDef definition

class WorkflowTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    DefaultRunProperties: NotRequired[Dict[str, str]],
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    LastRun: NotRequired[WorkflowRunTypeDef],  # (1)
    Graph: NotRequired[WorkflowGraphTypeDef],  # (2)
    MaxConcurrentRuns: NotRequired[int],
    BlueprintDetails: NotRequired[BlueprintDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: WorkflowRunTypeDef](./type_defs.md#workflowruntypedef) 
2. See [:material-code-braces: WorkflowGraphTypeDef](./type_defs.md#workflowgraphtypedef) 
3. See [:material-code-braces: BlueprintDetailsTypeDef](./type_defs.md#blueprintdetailstypedef) 
## BatchGetWorkflowsResponseTypeDef

```python
# BatchGetWorkflowsResponseTypeDef definition

class BatchGetWorkflowsResponseTypeDef(TypedDict):
    Workflows: List[WorkflowTypeDef],  # (1)
    MissingWorkflows: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkflowTypeDef](./type_defs.md#workflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkflowResponseTypeDef

```python
# GetWorkflowResponseTypeDef definition

class GetWorkflowResponseTypeDef(TypedDict):
    Workflow: WorkflowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkflowTypeDef](./type_defs.md#workflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
