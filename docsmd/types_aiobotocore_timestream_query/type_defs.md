# Type definitions

> [Index](../README.md) > [TimestreamQuery](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [TimestreamQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
    type annotations stubs module [types-aiobotocore-timestream-query](https://pypi.org/project/types-aiobotocore-timestream-query/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## CancelQueryRequestRequestTypeDef

```python
# CancelQueryRequestRequestTypeDef definition

class CancelQueryRequestRequestTypeDef(TypedDict):
    QueryId: str,
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

## ColumnInfoTypeDef

```python
# ColumnInfoTypeDef definition

class ColumnInfoTypeDef(TypedDict):
    Type: TypeTypeDef,  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: TypeTypeDef](./type_defs.md#typetypedef) 
## ScheduleConfigurationTypeDef

```python
# ScheduleConfigurationTypeDef definition

class ScheduleConfigurationTypeDef(TypedDict):
    ScheduleExpression: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## RowTypeDef

```python
# RowTypeDef definition

class RowTypeDef(TypedDict):
    Data: List[DatumTypeDef],  # (1)
```

1. See [:material-code-braces: DatumTypeDef](./type_defs.md#datumtypedef) 
## TimeSeriesDataPointTypeDef

```python
# TimeSeriesDataPointTypeDef definition

class TimeSeriesDataPointTypeDef(TypedDict):
    Time: str,
    Value: DatumTypeDef,  # (1)
```

1. See [:material-code-braces: DatumTypeDef](./type_defs.md#datumtypedef) 
## DeleteScheduledQueryRequestRequestTypeDef

```python
# DeleteScheduledQueryRequestRequestTypeDef definition

class DeleteScheduledQueryRequestRequestTypeDef(TypedDict):
    ScheduledQueryArn: str,
```

## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Address: str,
    CachePeriodInMinutes: int,
```

## DescribeScheduledQueryRequestRequestTypeDef

```python
# DescribeScheduledQueryRequestRequestTypeDef definition

class DescribeScheduledQueryRequestRequestTypeDef(TypedDict):
    ScheduledQueryArn: str,
```

## DimensionMappingTypeDef

```python
# DimensionMappingTypeDef definition

class DimensionMappingTypeDef(TypedDict):
    Name: str,
    DimensionValueType: DimensionValueTypeType,  # (1)
```

1. See [:material-code-brackets: DimensionValueTypeType](./literals.md#dimensionvaluetypetype) 
## S3ConfigurationTypeDef

```python
# S3ConfigurationTypeDef definition

class S3ConfigurationTypeDef(TypedDict):
    BucketName: str,
    ObjectKeyPrefix: NotRequired[str],
    EncryptionOption: NotRequired[S3EncryptionOptionType],  # (1)
```

1. See [:material-code-brackets: S3EncryptionOptionType](./literals.md#s3encryptionoptiontype) 
## S3ReportLocationTypeDef

```python
# S3ReportLocationTypeDef definition

class S3ReportLocationTypeDef(TypedDict):
    BucketName: NotRequired[str],
    ObjectKey: NotRequired[str],
```

## ExecutionStatsTypeDef

```python
# ExecutionStatsTypeDef definition

class ExecutionStatsTypeDef(TypedDict):
    ExecutionTimeInMillis: NotRequired[int],
    DataWrites: NotRequired[int],
    BytesMetered: NotRequired[int],
    RecordsIngested: NotRequired[int],
    QueryResultRows: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListScheduledQueriesRequestRequestTypeDef

```python
# ListScheduledQueriesRequestRequestTypeDef definition

class ListScheduledQueriesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## MultiMeasureAttributeMappingTypeDef

```python
# MultiMeasureAttributeMappingTypeDef definition

class MultiMeasureAttributeMappingTypeDef(TypedDict):
    SourceColumn: str,
    MeasureValueType: ScalarMeasureValueTypeType,  # (1)
    TargetMultiMeasureAttributeName: NotRequired[str],
```

1. See [:material-code-brackets: ScalarMeasureValueTypeType](./literals.md#scalarmeasurevaluetypetype) 
## SnsConfigurationTypeDef

```python
# SnsConfigurationTypeDef definition

class SnsConfigurationTypeDef(TypedDict):
    TopicArn: str,
```

## ParameterMappingTypeDef

```python
# ParameterMappingTypeDef definition

class ParameterMappingTypeDef(TypedDict):
    Name: str,
    Type: TypeTypeDef,  # (1)
```

1. See [:material-code-braces: TypeTypeDef](./type_defs.md#typetypedef) 
## PrepareQueryRequestRequestTypeDef

```python
# PrepareQueryRequestRequestTypeDef definition

class PrepareQueryRequestRequestTypeDef(TypedDict):
    QueryString: str,
    ValidateOnly: NotRequired[bool],
```

## SelectColumnTypeDef

```python
# SelectColumnTypeDef definition

class SelectColumnTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[TypeTypeDef],  # (1)
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    Aliased: NotRequired[bool],
```

1. See [:material-code-braces: TypeTypeDef](./type_defs.md#typetypedef) 
## QueryRequestRequestTypeDef

```python
# QueryRequestRequestTypeDef definition

class QueryRequestRequestTypeDef(TypedDict):
    QueryString: str,
    ClientToken: NotRequired[str],
    NextToken: NotRequired[str],
    MaxRows: NotRequired[int],
```

## QueryStatusTypeDef

```python
# QueryStatusTypeDef definition

class QueryStatusTypeDef(TypedDict):
    ProgressPercentage: NotRequired[float],
    CumulativeBytesScanned: NotRequired[int],
    CumulativeBytesMetered: NotRequired[int],
```

## TimestreamDestinationTypeDef

```python
# TimestreamDestinationTypeDef definition

class TimestreamDestinationTypeDef(TypedDict):
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
```

## TypeTypeDef

```python
# TypeTypeDef definition

class TypeTypeDef(TypedDict):
    ScalarType: NotRequired[ScalarTypeType],  # (1)
    ArrayColumnInfo: NotRequired[ColumnInfoTypeDef],  # (2)
    TimeSeriesMeasureValueColumnInfo: NotRequired[ColumnInfoTypeDef],  # (2)
    RowColumnInfo: NotRequired[List[ColumnInfoTypeDef]],  # (4)
```

1. See [:material-code-brackets: ScalarTypeType](./literals.md#scalartypetype) 
2. See [:material-code-braces: ColumnInfoTypeDef](./type_defs.md#columninfotypedef) 
3. See [:material-code-braces: ColumnInfoTypeDef](./type_defs.md#columninfotypedef) 
4. See [:material-code-braces: ColumnInfoTypeDef](./type_defs.md#columninfotypedef) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateScheduledQueryRequestRequestTypeDef

```python
# UpdateScheduledQueryRequestRequestTypeDef definition

class UpdateScheduledQueryRequestRequestTypeDef(TypedDict):
    ScheduledQueryArn: str,
    State: ScheduledQueryStateType,  # (1)
```

1. See [:material-code-brackets: ScheduledQueryStateType](./literals.md#scheduledquerystatetype) 
## CancelQueryResponseTypeDef

```python
# CancelQueryResponseTypeDef definition

class CancelQueryResponseTypeDef(TypedDict):
    CancellationMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScheduledQueryResponseTypeDef

```python
# CreateScheduledQueryResponseTypeDef definition

class CreateScheduledQueryResponseTypeDef(TypedDict):
    Arn: str,
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
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    NextToken: str,
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
## DatumTypeDef

```python
# DatumTypeDef definition

class DatumTypeDef(TypedDict):
    ScalarValue: NotRequired[str],
    TimeSeriesValue: NotRequired[List[TimeSeriesDataPointTypeDef]],  # (1)
    ArrayValue: NotRequired[List[DatumTypeDef]],  # (2)
    RowValue: NotRequired[RowTypeDef],  # (3)
    NullValue: NotRequired[bool],
```

1. See [:material-code-braces: TimeSeriesDataPointTypeDef](./type_defs.md#timeseriesdatapointtypedef) 
2. See [:material-code-braces: DatumTypeDef](./type_defs.md#datumtypedef) 
3. See [:material-code-braces: RowTypeDef](./type_defs.md#rowtypedef) 
## DescribeEndpointsResponseTypeDef

```python
# DescribeEndpointsResponseTypeDef definition

class DescribeEndpointsResponseTypeDef(TypedDict):
    Endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ErrorReportConfigurationTypeDef

```python
# ErrorReportConfigurationTypeDef definition

class ErrorReportConfigurationTypeDef(TypedDict):
    S3Configuration: S3ConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: S3ConfigurationTypeDef](./type_defs.md#s3configurationtypedef) 
## ErrorReportLocationTypeDef

```python
# ErrorReportLocationTypeDef definition

class ErrorReportLocationTypeDef(TypedDict):
    S3ReportLocation: NotRequired[S3ReportLocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3ReportLocationTypeDef](./type_defs.md#s3reportlocationtypedef) 
## ExecuteScheduledQueryRequestRequestTypeDef

```python
# ExecuteScheduledQueryRequestRequestTypeDef definition

class ExecuteScheduledQueryRequestRequestTypeDef(TypedDict):
    ScheduledQueryArn: str,
    InvocationTime: Union[datetime, str],
    ClientToken: NotRequired[str],
```

## ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef

```python
# ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef definition

class ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestListTagsForResourcePaginateTypeDef

```python
# ListTagsForResourceRequestListTagsForResourcePaginateTypeDef definition

class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(TypedDict):
    ResourceARN: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## QueryRequestQueryPaginateTypeDef

```python
# QueryRequestQueryPaginateTypeDef definition

class QueryRequestQueryPaginateTypeDef(TypedDict):
    QueryString: str,
    ClientToken: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
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
## NotificationConfigurationTypeDef

```python
# NotificationConfigurationTypeDef definition

class NotificationConfigurationTypeDef(TypedDict):
    SnsConfiguration: SnsConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: SnsConfigurationTypeDef](./type_defs.md#snsconfigurationtypedef) 
## PrepareQueryResponseTypeDef

```python
# PrepareQueryResponseTypeDef definition

class PrepareQueryResponseTypeDef(TypedDict):
    QueryString: str,
    Columns: List[SelectColumnTypeDef],  # (1)
    Parameters: List[ParameterMappingTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SelectColumnTypeDef](./type_defs.md#selectcolumntypedef) 
2. See [:material-code-braces: ParameterMappingTypeDef](./type_defs.md#parametermappingtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryResponseTypeDef

```python
# QueryResponseTypeDef definition

class QueryResponseTypeDef(TypedDict):
    QueryId: str,
    NextToken: str,
    Rows: List[RowTypeDef],  # (1)
    ColumnInfo: List[ColumnInfoTypeDef],  # (2)
    QueryStatus: QueryStatusTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: RowTypeDef](./type_defs.md#rowtypedef) 
2. See [:material-code-braces: ColumnInfoTypeDef](./type_defs.md#columninfotypedef) 
3. See [:material-code-braces: QueryStatusTypeDef](./type_defs.md#querystatustypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TargetDestinationTypeDef

```python
# TargetDestinationTypeDef definition

class TargetDestinationTypeDef(TypedDict):
    TimestreamDestination: NotRequired[TimestreamDestinationTypeDef],  # (1)
```

1. See [:material-code-braces: TimestreamDestinationTypeDef](./type_defs.md#timestreamdestinationtypedef) 
## ScheduledQueryRunSummaryTypeDef

```python
# ScheduledQueryRunSummaryTypeDef definition

class ScheduledQueryRunSummaryTypeDef(TypedDict):
    InvocationTime: NotRequired[datetime],
    TriggerTime: NotRequired[datetime],
    RunStatus: NotRequired[ScheduledQueryRunStatusType],  # (1)
    ExecutionStats: NotRequired[ExecutionStatsTypeDef],  # (2)
    ErrorReportLocation: NotRequired[ErrorReportLocationTypeDef],  # (3)
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: ScheduledQueryRunStatusType](./literals.md#scheduledqueryrunstatustype) 
2. See [:material-code-braces: ExecutionStatsTypeDef](./type_defs.md#executionstatstypedef) 
3. See [:material-code-braces: ErrorReportLocationTypeDef](./type_defs.md#errorreportlocationtypedef) 
## TimestreamConfigurationTypeDef

```python
# TimestreamConfigurationTypeDef definition

class TimestreamConfigurationTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    TimeColumn: str,
    DimensionMappings: Sequence[DimensionMappingTypeDef],  # (1)
    MultiMeasureMappings: NotRequired[MultiMeasureMappingsTypeDef],  # (2)
    MixedMeasureMappings: NotRequired[Sequence[MixedMeasureMappingTypeDef]],  # (3)
    MeasureNameColumn: NotRequired[str],
```

1. See [:material-code-braces: DimensionMappingTypeDef](./type_defs.md#dimensionmappingtypedef) 
2. See [:material-code-braces: MultiMeasureMappingsTypeDef](./type_defs.md#multimeasuremappingstypedef) 
3. See [:material-code-braces: MixedMeasureMappingTypeDef](./type_defs.md#mixedmeasuremappingtypedef) 
## ScheduledQueryTypeDef

```python
# ScheduledQueryTypeDef definition

class ScheduledQueryTypeDef(TypedDict):
    Arn: str,
    Name: str,
    State: ScheduledQueryStateType,  # (1)
    CreationTime: NotRequired[datetime],
    PreviousInvocationTime: NotRequired[datetime],
    NextInvocationTime: NotRequired[datetime],
    ErrorReportConfiguration: NotRequired[ErrorReportConfigurationTypeDef],  # (2)
    TargetDestination: NotRequired[TargetDestinationTypeDef],  # (3)
    LastRunStatus: NotRequired[ScheduledQueryRunStatusType],  # (4)
```

1. See [:material-code-brackets: ScheduledQueryStateType](./literals.md#scheduledquerystatetype) 
2. See [:material-code-braces: ErrorReportConfigurationTypeDef](./type_defs.md#errorreportconfigurationtypedef) 
3. See [:material-code-braces: TargetDestinationTypeDef](./type_defs.md#targetdestinationtypedef) 
4. See [:material-code-brackets: ScheduledQueryRunStatusType](./literals.md#scheduledqueryrunstatustype) 
## TargetConfigurationTypeDef

```python
# TargetConfigurationTypeDef definition

class TargetConfigurationTypeDef(TypedDict):
    TimestreamConfiguration: TimestreamConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: TimestreamConfigurationTypeDef](./type_defs.md#timestreamconfigurationtypedef) 
## ListScheduledQueriesResponseTypeDef

```python
# ListScheduledQueriesResponseTypeDef definition

class ListScheduledQueriesResponseTypeDef(TypedDict):
    ScheduledQueries: List[ScheduledQueryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduledQueryTypeDef](./type_defs.md#scheduledquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScheduledQueryRequestRequestTypeDef

```python
# CreateScheduledQueryRequestRequestTypeDef definition

class CreateScheduledQueryRequestRequestTypeDef(TypedDict):
    Name: str,
    QueryString: str,
    ScheduleConfiguration: ScheduleConfigurationTypeDef,  # (1)
    NotificationConfiguration: NotificationConfigurationTypeDef,  # (2)
    ScheduledQueryExecutionRoleArn: str,
    ErrorReportConfiguration: ErrorReportConfigurationTypeDef,  # (3)
    TargetConfiguration: NotRequired[TargetConfigurationTypeDef],  # (4)
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
2. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
3. See [:material-code-braces: ErrorReportConfigurationTypeDef](./type_defs.md#errorreportconfigurationtypedef) 
4. See [:material-code-braces: TargetConfigurationTypeDef](./type_defs.md#targetconfigurationtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ScheduledQueryDescriptionTypeDef

```python
# ScheduledQueryDescriptionTypeDef definition

class ScheduledQueryDescriptionTypeDef(TypedDict):
    Arn: str,
    Name: str,
    QueryString: str,
    State: ScheduledQueryStateType,  # (1)
    ScheduleConfiguration: ScheduleConfigurationTypeDef,  # (2)
    NotificationConfiguration: NotificationConfigurationTypeDef,  # (3)
    CreationTime: NotRequired[datetime],
    PreviousInvocationTime: NotRequired[datetime],
    NextInvocationTime: NotRequired[datetime],
    TargetConfiguration: NotRequired[TargetConfigurationTypeDef],  # (4)
    ScheduledQueryExecutionRoleArn: NotRequired[str],
    KmsKeyId: NotRequired[str],
    ErrorReportConfiguration: NotRequired[ErrorReportConfigurationTypeDef],  # (5)
    LastRunSummary: NotRequired[ScheduledQueryRunSummaryTypeDef],  # (6)
    RecentlyFailedRuns: NotRequired[List[ScheduledQueryRunSummaryTypeDef]],  # (7)
```

1. See [:material-code-brackets: ScheduledQueryStateType](./literals.md#scheduledquerystatetype) 
2. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
3. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
4. See [:material-code-braces: TargetConfigurationTypeDef](./type_defs.md#targetconfigurationtypedef) 
5. See [:material-code-braces: ErrorReportConfigurationTypeDef](./type_defs.md#errorreportconfigurationtypedef) 
6. See [:material-code-braces: ScheduledQueryRunSummaryTypeDef](./type_defs.md#scheduledqueryrunsummarytypedef) 
7. See [:material-code-braces: ScheduledQueryRunSummaryTypeDef](./type_defs.md#scheduledqueryrunsummarytypedef) 
## DescribeScheduledQueryResponseTypeDef

```python
# DescribeScheduledQueryResponseTypeDef definition

class DescribeScheduledQueryResponseTypeDef(TypedDict):
    ScheduledQuery: ScheduledQueryDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduledQueryDescriptionTypeDef](./type_defs.md#scheduledquerydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
