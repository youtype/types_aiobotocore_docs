# Type definitions

> [Index](../README.md) > [TimestreamQuery](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [TimestreamQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#timestreamquery)
    type annotations stubs module [types-aiobotocore-timestream-query](https://pypi.org/project/types-aiobotocore-timestream-query/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## MixedMeasureMappingUnionTypeDef

```python
# MixedMeasureMappingUnionTypeDef definition

MixedMeasureMappingUnionTypeDef = Union[
    MixedMeasureMappingTypeDef,  # (1)
    MixedMeasureMappingOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MixedMeasureMappingTypeDef](./type_defs.md#mixedmeasuremappingtypedef) 
2. See [:material-code-braces: MixedMeasureMappingOutputTypeDef](./type_defs.md#mixedmeasuremappingoutputtypedef) 

## MultiMeasureMappingsUnionTypeDef

```python
# MultiMeasureMappingsUnionTypeDef definition

MultiMeasureMappingsUnionTypeDef = Union[
    MultiMeasureMappingsTypeDef,  # (1)
    MultiMeasureMappingsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MultiMeasureMappingsTypeDef](./type_defs.md#multimeasuremappingstypedef) 
2. See [:material-code-braces: MultiMeasureMappingsOutputTypeDef](./type_defs.md#multimeasuremappingsoutputtypedef) 

## TimestreamConfigurationUnionTypeDef

```python
# TimestreamConfigurationUnionTypeDef definition

TimestreamConfigurationUnionTypeDef = Union[
    TimestreamConfigurationTypeDef,  # (1)
    TimestreamConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TimestreamConfigurationTypeDef](./type_defs.md#timestreamconfigurationtypedef) 
2. See [:material-code-braces: TimestreamConfigurationOutputTypeDef](./type_defs.md#timestreamconfigurationoutputtypedef) 



## SnsConfigurationTypeDef

```python
# SnsConfigurationTypeDef definition

class SnsConfigurationTypeDef(TypedDict):
    TopicArn: str,
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
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## TypePaginatorTypeDef

```python
# TypePaginatorTypeDef definition

class TypePaginatorTypeDef(TypedDict):
    ScalarType: NotRequired[ScalarTypeType],  # (1)
    ArrayColumnInfo: NotRequired[Dict[str, Any]],
    TimeSeriesMeasureValueColumnInfo: NotRequired[Dict[str, Any]],
    RowColumnInfo: NotRequired[List[Dict[str, Any]]],
```

1. See [:material-code-brackets: ScalarTypeType](./literals.md#scalartypetype) 
## ColumnInfoTypeDef

```python
# ColumnInfoTypeDef definition

class ColumnInfoTypeDef(TypedDict):
    Type: Dict[str, Any],
    Name: NotRequired[str],
```

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

## TimeSeriesDataPointPaginatorTypeDef

```python
# TimeSeriesDataPointPaginatorTypeDef definition

class TimeSeriesDataPointPaginatorTypeDef(TypedDict):
    Time: str,
    Value: Dict[str, Any],
```

## TimeSeriesDataPointTypeDef

```python
# TimeSeriesDataPointTypeDef definition

class TimeSeriesDataPointTypeDef(TypedDict):
    Time: str,
    Value: Dict[str, Any],
```

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

## ScheduledQueryInsightsTypeDef

```python
# ScheduledQueryInsightsTypeDef definition

class ScheduledQueryInsightsTypeDef(TypedDict):
    Mode: ScheduledQueryInsightsModeType,  # (1)
```

1. See [:material-code-brackets: ScheduledQueryInsightsModeType](./literals.md#scheduledqueryinsightsmodetype) 
## ExecutionStatsTypeDef

```python
# ExecutionStatsTypeDef definition

class ExecutionStatsTypeDef(TypedDict):
    ExecutionTimeInMillis: NotRequired[int],
    DataWrites: NotRequired[int],
    BytesMetered: NotRequired[int],
    CumulativeBytesScanned: NotRequired[int],
    RecordsIngested: NotRequired[int],
    QueryResultRows: NotRequired[int],
```

## LastUpdateTypeDef

```python
# LastUpdateTypeDef definition

class LastUpdateTypeDef(TypedDict):
    TargetQueryTCU: NotRequired[int],
    Status: NotRequired[LastUpdateStatusType],  # (1)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: LastUpdateStatusType](./literals.md#lastupdatestatustype) 
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
## PrepareQueryRequestRequestTypeDef

```python
# PrepareQueryRequestRequestTypeDef definition

class PrepareQueryRequestRequestTypeDef(TypedDict):
    QueryString: str,
    ValidateOnly: NotRequired[bool],
```

## QueryInsightsTypeDef

```python
# QueryInsightsTypeDef definition

class QueryInsightsTypeDef(TypedDict):
    Mode: QueryInsightsModeType,  # (1)
```

1. See [:material-code-brackets: QueryInsightsModeType](./literals.md#queryinsightsmodetype) 
## QueryStatusTypeDef

```python
# QueryStatusTypeDef definition

class QueryStatusTypeDef(TypedDict):
    ProgressPercentage: NotRequired[float],
    CumulativeBytesScanned: NotRequired[int],
    CumulativeBytesMetered: NotRequired[int],
```

## QuerySpatialCoverageMaxTypeDef

```python
# QuerySpatialCoverageMaxTypeDef definition

class QuerySpatialCoverageMaxTypeDef(TypedDict):
    Value: NotRequired[float],
    TableArn: NotRequired[str],
    PartitionKey: NotRequired[List[str]],
```

## QueryTemporalRangeMaxTypeDef

```python
# QueryTemporalRangeMaxTypeDef definition

class QueryTemporalRangeMaxTypeDef(TypedDict):
    Value: NotRequired[int],
    TableArn: NotRequired[str],
```

## TimestreamDestinationTypeDef

```python
# TimestreamDestinationTypeDef definition

class TimestreamDestinationTypeDef(TypedDict):
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
```

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
## AccountSettingsNotificationConfigurationTypeDef

```python
# AccountSettingsNotificationConfigurationTypeDef definition

class AccountSettingsNotificationConfigurationTypeDef(TypedDict):
    RoleArn: str,
    SnsConfiguration: NotRequired[SnsConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: SnsConfigurationTypeDef](./type_defs.md#snsconfigurationtypedef) 
## NotificationConfigurationTypeDef

```python
# NotificationConfigurationTypeDef definition

class NotificationConfigurationTypeDef(TypedDict):
    SnsConfiguration: SnsConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: SnsConfigurationTypeDef](./type_defs.md#snsconfigurationtypedef) 
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
## ColumnInfoPaginatorTypeDef

```python
# ColumnInfoPaginatorTypeDef definition

class ColumnInfoPaginatorTypeDef(TypedDict):
    Type: TypePaginatorTypeDef,  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: TypePaginatorTypeDef](./type_defs.md#typepaginatortypedef) 
## TypeTypeDef

```python
# TypeTypeDef definition

class TypeTypeDef(TypedDict):
    ScalarType: NotRequired[ScalarTypeType],  # (1)
    ArrayColumnInfo: NotRequired[Dict[str, Any]],
    TimeSeriesMeasureValueColumnInfo: NotRequired[Dict[str, Any]],
    RowColumnInfo: NotRequired[List[ColumnInfoTypeDef]],  # (2)
```

1. See [:material-code-brackets: ScalarTypeType](./literals.md#scalartypetype) 
2. See [:material-code-braces: ColumnInfoTypeDef](./type_defs.md#columninfotypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
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
## DatumPaginatorTypeDef

```python
# DatumPaginatorTypeDef definition

class DatumPaginatorTypeDef(TypedDict):
    ScalarValue: NotRequired[str],
    TimeSeriesValue: NotRequired[List[TimeSeriesDataPointPaginatorTypeDef]],  # (1)
    ArrayValue: NotRequired[List[Dict[str, Any]]],
    RowValue: NotRequired[Dict[str, Any]],
    NullValue: NotRequired[bool],
```

1. See [:material-code-braces: TimeSeriesDataPointPaginatorTypeDef](./type_defs.md#timeseriesdatapointpaginatortypedef) 
## DatumTypeDef

```python
# DatumTypeDef definition

class DatumTypeDef(TypedDict):
    ScalarValue: NotRequired[str],
    TimeSeriesValue: NotRequired[List[TimeSeriesDataPointTypeDef]],  # (1)
    ArrayValue: NotRequired[List[Dict[str, Any]]],
    RowValue: NotRequired[Dict[str, Any]],
    NullValue: NotRequired[bool],
```

1. See [:material-code-braces: TimeSeriesDataPointTypeDef](./type_defs.md#timeseriesdatapointtypedef) 
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
    InvocationTime: TimestampTypeDef,
    ClientToken: NotRequired[str],
    QueryInsights: NotRequired[ScheduledQueryInsightsTypeDef],  # (1)
```

1. See [:material-code-braces: ScheduledQueryInsightsTypeDef](./type_defs.md#scheduledqueryinsightstypedef) 
## ListScheduledQueriesRequestPaginateTypeDef

```python
# ListScheduledQueriesRequestPaginateTypeDef definition

class ListScheduledQueriesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestPaginateTypeDef

```python
# ListTagsForResourceRequestPaginateTypeDef definition

class ListTagsForResourceRequestPaginateTypeDef(TypedDict):
    ResourceARN: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## MixedMeasureMappingOutputTypeDef

```python
# MixedMeasureMappingOutputTypeDef definition

class MixedMeasureMappingOutputTypeDef(TypedDict):
    MeasureValueType: MeasureValueTypeType,  # (1)
    MeasureName: NotRequired[str],
    SourceColumn: NotRequired[str],
    TargetMeasureName: NotRequired[str],
    MultiMeasureAttributeMappings: NotRequired[List[MultiMeasureAttributeMappingTypeDef]],  # (2)
```

1. See [:material-code-brackets: MeasureValueTypeType](./literals.md#measurevaluetypetype) 
2. See [:material-code-braces: MultiMeasureAttributeMappingTypeDef](./type_defs.md#multimeasureattributemappingtypedef) 
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
## MultiMeasureMappingsOutputTypeDef

```python
# MultiMeasureMappingsOutputTypeDef definition

class MultiMeasureMappingsOutputTypeDef(TypedDict):
    MultiMeasureAttributeMappings: List[MultiMeasureAttributeMappingTypeDef],  # (1)
    TargetMultiMeasureName: NotRequired[str],
```

1. See [:material-code-braces: MultiMeasureAttributeMappingTypeDef](./type_defs.md#multimeasureattributemappingtypedef) 
## MultiMeasureMappingsTypeDef

```python
# MultiMeasureMappingsTypeDef definition

class MultiMeasureMappingsTypeDef(TypedDict):
    MultiMeasureAttributeMappings: Sequence[MultiMeasureAttributeMappingTypeDef],  # (1)
    TargetMultiMeasureName: NotRequired[str],
```

1. See [:material-code-braces: MultiMeasureAttributeMappingTypeDef](./type_defs.md#multimeasureattributemappingtypedef) 
## QueryRequestPaginateTypeDef

```python
# QueryRequestPaginateTypeDef definition

class QueryRequestPaginateTypeDef(TypedDict):
    QueryString: str,
    ClientToken: NotRequired[str],
    QueryInsights: NotRequired[QueryInsightsTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: QueryInsightsTypeDef](./type_defs.md#queryinsightstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## QueryRequestRequestTypeDef

```python
# QueryRequestRequestTypeDef definition

class QueryRequestRequestTypeDef(TypedDict):
    QueryString: str,
    ClientToken: NotRequired[str],
    NextToken: NotRequired[str],
    MaxRows: NotRequired[int],
    QueryInsights: NotRequired[QueryInsightsTypeDef],  # (1)
```

1. See [:material-code-braces: QueryInsightsTypeDef](./type_defs.md#queryinsightstypedef) 
## QuerySpatialCoverageTypeDef

```python
# QuerySpatialCoverageTypeDef definition

class QuerySpatialCoverageTypeDef(TypedDict):
    Max: NotRequired[QuerySpatialCoverageMaxTypeDef],  # (1)
```

1. See [:material-code-braces: QuerySpatialCoverageMaxTypeDef](./type_defs.md#queryspatialcoveragemaxtypedef) 
## QueryTemporalRangeTypeDef

```python
# QueryTemporalRangeTypeDef definition

class QueryTemporalRangeTypeDef(TypedDict):
    Max: NotRequired[QueryTemporalRangeMaxTypeDef],  # (1)
```

1. See [:material-code-braces: QueryTemporalRangeMaxTypeDef](./type_defs.md#querytemporalrangemaxtypedef) 
## TargetDestinationTypeDef

```python
# TargetDestinationTypeDef definition

class TargetDestinationTypeDef(TypedDict):
    TimestreamDestination: NotRequired[TimestreamDestinationTypeDef],  # (1)
```

1. See [:material-code-braces: TimestreamDestinationTypeDef](./type_defs.md#timestreamdestinationtypedef) 
## ProvisionedCapacityRequestTypeDef

```python
# ProvisionedCapacityRequestTypeDef definition

class ProvisionedCapacityRequestTypeDef(TypedDict):
    TargetQueryTCU: int,
    NotificationConfiguration: NotRequired[AccountSettingsNotificationConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AccountSettingsNotificationConfigurationTypeDef](./type_defs.md#accountsettingsnotificationconfigurationtypedef) 
## ProvisionedCapacityResponseTypeDef

```python
# ProvisionedCapacityResponseTypeDef definition

class ProvisionedCapacityResponseTypeDef(TypedDict):
    ActiveQueryTCU: NotRequired[int],
    NotificationConfiguration: NotRequired[AccountSettingsNotificationConfigurationTypeDef],  # (1)
    LastUpdate: NotRequired[LastUpdateTypeDef],  # (2)
```

1. See [:material-code-braces: AccountSettingsNotificationConfigurationTypeDef](./type_defs.md#accountsettingsnotificationconfigurationtypedef) 
2. See [:material-code-braces: LastUpdateTypeDef](./type_defs.md#lastupdatetypedef) 
## ParameterMappingTypeDef

```python
# ParameterMappingTypeDef definition

class ParameterMappingTypeDef(TypedDict):
    Name: str,
    Type: TypeTypeDef,  # (1)
```

1. See [:material-code-braces: TypeTypeDef](./type_defs.md#typetypedef) 
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
## RowPaginatorTypeDef

```python
# RowPaginatorTypeDef definition

class RowPaginatorTypeDef(TypedDict):
    Data: List[DatumPaginatorTypeDef],  # (1)
```

1. See [:material-code-braces: DatumPaginatorTypeDef](./type_defs.md#datumpaginatortypedef) 
## RowTypeDef

```python
# RowTypeDef definition

class RowTypeDef(TypedDict):
    Data: List[DatumTypeDef],  # (1)
```

1. See [:material-code-braces: DatumTypeDef](./type_defs.md#datumtypedef) 
## TimestreamConfigurationOutputTypeDef

```python
# TimestreamConfigurationOutputTypeDef definition

class TimestreamConfigurationOutputTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    TimeColumn: str,
    DimensionMappings: List[DimensionMappingTypeDef],  # (1)
    MultiMeasureMappings: NotRequired[MultiMeasureMappingsOutputTypeDef],  # (2)
    MixedMeasureMappings: NotRequired[List[MixedMeasureMappingOutputTypeDef]],  # (3)
    MeasureNameColumn: NotRequired[str],
```

1. See [:material-code-braces: DimensionMappingTypeDef](./type_defs.md#dimensionmappingtypedef) 
2. See [:material-code-braces: MultiMeasureMappingsOutputTypeDef](./type_defs.md#multimeasuremappingsoutputtypedef) 
3. See [:material-code-braces: MixedMeasureMappingOutputTypeDef](./type_defs.md#mixedmeasuremappingoutputtypedef) 
## QueryInsightsResponseTypeDef

```python
# QueryInsightsResponseTypeDef definition

class QueryInsightsResponseTypeDef(TypedDict):
    QuerySpatialCoverage: NotRequired[QuerySpatialCoverageTypeDef],  # (1)
    QueryTemporalRange: NotRequired[QueryTemporalRangeTypeDef],  # (2)
    QueryTableCount: NotRequired[int],
    OutputRows: NotRequired[int],
    OutputBytes: NotRequired[int],
    UnloadPartitionCount: NotRequired[int],
    UnloadWrittenRows: NotRequired[int],
    UnloadWrittenBytes: NotRequired[int],
```

1. See [:material-code-braces: QuerySpatialCoverageTypeDef](./type_defs.md#queryspatialcoveragetypedef) 
2. See [:material-code-braces: QueryTemporalRangeTypeDef](./type_defs.md#querytemporalrangetypedef) 
## ScheduledQueryInsightsResponseTypeDef

```python
# ScheduledQueryInsightsResponseTypeDef definition

class ScheduledQueryInsightsResponseTypeDef(TypedDict):
    QuerySpatialCoverage: NotRequired[QuerySpatialCoverageTypeDef],  # (1)
    QueryTemporalRange: NotRequired[QueryTemporalRangeTypeDef],  # (2)
    QueryTableCount: NotRequired[int],
    OutputRows: NotRequired[int],
    OutputBytes: NotRequired[int],
```

1. See [:material-code-braces: QuerySpatialCoverageTypeDef](./type_defs.md#queryspatialcoveragetypedef) 
2. See [:material-code-braces: QueryTemporalRangeTypeDef](./type_defs.md#querytemporalrangetypedef) 
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
## QueryComputeRequestTypeDef

```python
# QueryComputeRequestTypeDef definition

class QueryComputeRequestTypeDef(TypedDict):
    ComputeMode: NotRequired[ComputeModeType],  # (1)
    ProvisionedCapacity: NotRequired[ProvisionedCapacityRequestTypeDef],  # (2)
```

1. See [:material-code-brackets: ComputeModeType](./literals.md#computemodetype) 
2. See [:material-code-braces: ProvisionedCapacityRequestTypeDef](./type_defs.md#provisionedcapacityrequesttypedef) 
## QueryComputeResponseTypeDef

```python
# QueryComputeResponseTypeDef definition

class QueryComputeResponseTypeDef(TypedDict):
    ComputeMode: NotRequired[ComputeModeType],  # (1)
    ProvisionedCapacity: NotRequired[ProvisionedCapacityResponseTypeDef],  # (2)
```

1. See [:material-code-brackets: ComputeModeType](./literals.md#computemodetype) 
2. See [:material-code-braces: ProvisionedCapacityResponseTypeDef](./type_defs.md#provisionedcapacityresponsetypedef) 
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
## TargetConfigurationOutputTypeDef

```python
# TargetConfigurationOutputTypeDef definition

class TargetConfigurationOutputTypeDef(TypedDict):
    TimestreamConfiguration: TimestreamConfigurationOutputTypeDef,  # (1)
```

1. See [:material-code-braces: TimestreamConfigurationOutputTypeDef](./type_defs.md#timestreamconfigurationoutputtypedef) 
## TimestreamConfigurationTypeDef

```python
# TimestreamConfigurationTypeDef definition

class TimestreamConfigurationTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    TimeColumn: str,
    DimensionMappings: Sequence[DimensionMappingTypeDef],  # (1)
    MultiMeasureMappings: NotRequired[MultiMeasureMappingsUnionTypeDef],  # (2)
    MixedMeasureMappings: NotRequired[Sequence[MixedMeasureMappingUnionTypeDef]],  # (3)
    MeasureNameColumn: NotRequired[str],
```

1. See [:material-code-braces: DimensionMappingTypeDef](./type_defs.md#dimensionmappingtypedef) 
2. See [:material-code-braces: MultiMeasureMappingsTypeDef](./type_defs.md#multimeasuremappingstypedef) [:material-code-braces: MultiMeasureMappingsOutputTypeDef](./type_defs.md#multimeasuremappingsoutputtypedef) 
3. See [:material-code-braces: MixedMeasureMappingTypeDef](./type_defs.md#mixedmeasuremappingtypedef) [:material-code-braces: MixedMeasureMappingOutputTypeDef](./type_defs.md#mixedmeasuremappingoutputtypedef) 
## QueryResponsePaginatorTypeDef

```python
# QueryResponsePaginatorTypeDef definition

class QueryResponsePaginatorTypeDef(TypedDict):
    QueryId: str,
    Rows: List[RowPaginatorTypeDef],  # (1)
    ColumnInfo: List[ColumnInfoPaginatorTypeDef],  # (2)
    QueryStatus: QueryStatusTypeDef,  # (3)
    QueryInsightsResponse: QueryInsightsResponseTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RowPaginatorTypeDef](./type_defs.md#rowpaginatortypedef) 
2. See [:material-code-braces: ColumnInfoPaginatorTypeDef](./type_defs.md#columninfopaginatortypedef) 
3. See [:material-code-braces: QueryStatusTypeDef](./type_defs.md#querystatustypedef) 
4. See [:material-code-braces: QueryInsightsResponseTypeDef](./type_defs.md#queryinsightsresponsetypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryResponseTypeDef

```python
# QueryResponseTypeDef definition

class QueryResponseTypeDef(TypedDict):
    QueryId: str,
    Rows: List[RowTypeDef],  # (1)
    ColumnInfo: List[ColumnInfoTypeDef],  # (2)
    QueryStatus: QueryStatusTypeDef,  # (3)
    QueryInsightsResponse: QueryInsightsResponseTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RowTypeDef](./type_defs.md#rowtypedef) 
2. See [:material-code-braces: ColumnInfoTypeDef](./type_defs.md#columninfotypedef) 
3. See [:material-code-braces: QueryStatusTypeDef](./type_defs.md#querystatustypedef) 
4. See [:material-code-braces: QueryInsightsResponseTypeDef](./type_defs.md#queryinsightsresponsetypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScheduledQueryRunSummaryTypeDef

```python
# ScheduledQueryRunSummaryTypeDef definition

class ScheduledQueryRunSummaryTypeDef(TypedDict):
    InvocationTime: NotRequired[datetime],
    TriggerTime: NotRequired[datetime],
    RunStatus: NotRequired[ScheduledQueryRunStatusType],  # (1)
    ExecutionStats: NotRequired[ExecutionStatsTypeDef],  # (2)
    QueryInsightsResponse: NotRequired[ScheduledQueryInsightsResponseTypeDef],  # (3)
    ErrorReportLocation: NotRequired[ErrorReportLocationTypeDef],  # (4)
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: ScheduledQueryRunStatusType](./literals.md#scheduledqueryrunstatustype) 
2. See [:material-code-braces: ExecutionStatsTypeDef](./type_defs.md#executionstatstypedef) 
3. See [:material-code-braces: ScheduledQueryInsightsResponseTypeDef](./type_defs.md#scheduledqueryinsightsresponsetypedef) 
4. See [:material-code-braces: ErrorReportLocationTypeDef](./type_defs.md#errorreportlocationtypedef) 
## ListScheduledQueriesResponseTypeDef

```python
# ListScheduledQueriesResponseTypeDef definition

class ListScheduledQueriesResponseTypeDef(TypedDict):
    ScheduledQueries: List[ScheduledQueryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ScheduledQueryTypeDef](./type_defs.md#scheduledquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountSettingsRequestRequestTypeDef

```python
# UpdateAccountSettingsRequestRequestTypeDef definition

class UpdateAccountSettingsRequestRequestTypeDef(TypedDict):
    MaxQueryTCU: NotRequired[int],
    QueryPricingModel: NotRequired[QueryPricingModelType],  # (1)
    QueryCompute: NotRequired[QueryComputeRequestTypeDef],  # (2)
```

1. See [:material-code-brackets: QueryPricingModelType](./literals.md#querypricingmodeltype) 
2. See [:material-code-braces: QueryComputeRequestTypeDef](./type_defs.md#querycomputerequesttypedef) 
## DescribeAccountSettingsResponseTypeDef

```python
# DescribeAccountSettingsResponseTypeDef definition

class DescribeAccountSettingsResponseTypeDef(TypedDict):
    MaxQueryTCU: int,
    QueryPricingModel: QueryPricingModelType,  # (1)
    QueryCompute: QueryComputeResponseTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: QueryPricingModelType](./literals.md#querypricingmodeltype) 
2. See [:material-code-braces: QueryComputeResponseTypeDef](./type_defs.md#querycomputeresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountSettingsResponseTypeDef

```python
# UpdateAccountSettingsResponseTypeDef definition

class UpdateAccountSettingsResponseTypeDef(TypedDict):
    MaxQueryTCU: int,
    QueryPricingModel: QueryPricingModelType,  # (1)
    QueryCompute: QueryComputeResponseTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: QueryPricingModelType](./literals.md#querypricingmodeltype) 
2. See [:material-code-braces: QueryComputeResponseTypeDef](./type_defs.md#querycomputeresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    TargetConfiguration: NotRequired[TargetConfigurationOutputTypeDef],  # (4)
    ScheduledQueryExecutionRoleArn: NotRequired[str],
    KmsKeyId: NotRequired[str],
    ErrorReportConfiguration: NotRequired[ErrorReportConfigurationTypeDef],  # (5)
    LastRunSummary: NotRequired[ScheduledQueryRunSummaryTypeDef],  # (6)
    RecentlyFailedRuns: NotRequired[List[ScheduledQueryRunSummaryTypeDef]],  # (7)
```

1. See [:material-code-brackets: ScheduledQueryStateType](./literals.md#scheduledquerystatetype) 
2. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
3. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
4. See [:material-code-braces: TargetConfigurationOutputTypeDef](./type_defs.md#targetconfigurationoutputtypedef) 
5. See [:material-code-braces: ErrorReportConfigurationTypeDef](./type_defs.md#errorreportconfigurationtypedef) 
6. See [:material-code-braces: ScheduledQueryRunSummaryTypeDef](./type_defs.md#scheduledqueryrunsummarytypedef) 
7. See [:material-code-braces: ScheduledQueryRunSummaryTypeDef](./type_defs.md#scheduledqueryrunsummarytypedef) 
## TargetConfigurationTypeDef

```python
# TargetConfigurationTypeDef definition

class TargetConfigurationTypeDef(TypedDict):
    TimestreamConfiguration: TimestreamConfigurationUnionTypeDef,  # (1)
```

1. See [:material-code-braces: TimestreamConfigurationTypeDef](./type_defs.md#timestreamconfigurationtypedef) [:material-code-braces: TimestreamConfigurationOutputTypeDef](./type_defs.md#timestreamconfigurationoutputtypedef) 
## DescribeScheduledQueryResponseTypeDef

```python
# DescribeScheduledQueryResponseTypeDef definition

class DescribeScheduledQueryResponseTypeDef(TypedDict):
    ScheduledQuery: ScheduledQueryDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScheduledQueryDescriptionTypeDef](./type_defs.md#scheduledquerydescriptiontypedef) 
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
