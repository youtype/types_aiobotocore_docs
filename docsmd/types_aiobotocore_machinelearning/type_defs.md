# Type definitions

> [Index](../README.md) > [MachineLearning](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MachineLearning](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
    type annotations stubs module [types-aiobotocore-machinelearning](https://pypi.org/project/types-aiobotocore-machinelearning/).



## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
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

## BatchPredictionTypeDef

```python
# BatchPredictionTypeDef definition

class BatchPredictionTypeDef(TypedDict):
    BatchPredictionId: NotRequired[str],
    MLModelId: NotRequired[str],
    BatchPredictionDataSourceId: NotRequired[str],
    InputDataLocationS3: NotRequired[str],
    CreatedByIamUser: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    Name: NotRequired[str],
    Status: NotRequired[EntityStatusType],  # (1)
    OutputUri: NotRequired[str],
    Message: NotRequired[str],
    ComputeTime: NotRequired[int],
    FinishedAt: NotRequired[datetime],
    StartedAt: NotRequired[datetime],
    TotalRecordCount: NotRequired[int],
    InvalidRecordCount: NotRequired[int],
```

1. See [:material-code-brackets: EntityStatusType](./literals.md#entitystatustype) 
## CreateBatchPredictionInputRequestTypeDef

```python
# CreateBatchPredictionInputRequestTypeDef definition

class CreateBatchPredictionInputRequestTypeDef(TypedDict):
    BatchPredictionId: str,
    MLModelId: str,
    BatchPredictionDataSourceId: str,
    OutputUri: str,
    BatchPredictionName: NotRequired[str],
```

## S3DataSpecTypeDef

```python
# S3DataSpecTypeDef definition

class S3DataSpecTypeDef(TypedDict):
    DataLocationS3: str,
    DataRearrangement: NotRequired[str],
    DataSchema: NotRequired[str],
    DataSchemaLocationS3: NotRequired[str],
```

## CreateEvaluationInputRequestTypeDef

```python
# CreateEvaluationInputRequestTypeDef definition

class CreateEvaluationInputRequestTypeDef(TypedDict):
    EvaluationId: str,
    MLModelId: str,
    EvaluationDataSourceId: str,
    EvaluationName: NotRequired[str],
```

## CreateMLModelInputRequestTypeDef

```python
# CreateMLModelInputRequestTypeDef definition

class CreateMLModelInputRequestTypeDef(TypedDict):
    MLModelId: str,
    MLModelType: MLModelTypeType,  # (1)
    TrainingDataSourceId: str,
    MLModelName: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
    Recipe: NotRequired[str],
    RecipeUri: NotRequired[str],
```

1. See [:material-code-brackets: MLModelTypeType](./literals.md#mlmodeltypetype) 
## CreateRealtimeEndpointInputRequestTypeDef

```python
# CreateRealtimeEndpointInputRequestTypeDef definition

class CreateRealtimeEndpointInputRequestTypeDef(TypedDict):
    MLModelId: str,
```

## RealtimeEndpointInfoTypeDef

```python
# RealtimeEndpointInfoTypeDef definition

class RealtimeEndpointInfoTypeDef(TypedDict):
    PeakRequestsPerSecond: NotRequired[int],
    CreatedAt: NotRequired[datetime],
    EndpointUrl: NotRequired[str],
    EndpointStatus: NotRequired[RealtimeEndpointStatusType],  # (1)
```

1. See [:material-code-brackets: RealtimeEndpointStatusType](./literals.md#realtimeendpointstatustype) 
## DeleteBatchPredictionInputRequestTypeDef

```python
# DeleteBatchPredictionInputRequestTypeDef definition

class DeleteBatchPredictionInputRequestTypeDef(TypedDict):
    BatchPredictionId: str,
```

## DeleteDataSourceInputRequestTypeDef

```python
# DeleteDataSourceInputRequestTypeDef definition

class DeleteDataSourceInputRequestTypeDef(TypedDict):
    DataSourceId: str,
```

## DeleteEvaluationInputRequestTypeDef

```python
# DeleteEvaluationInputRequestTypeDef definition

class DeleteEvaluationInputRequestTypeDef(TypedDict):
    EvaluationId: str,
```

## DeleteMLModelInputRequestTypeDef

```python
# DeleteMLModelInputRequestTypeDef definition

class DeleteMLModelInputRequestTypeDef(TypedDict):
    MLModelId: str,
```

## DeleteRealtimeEndpointInputRequestTypeDef

```python
# DeleteRealtimeEndpointInputRequestTypeDef definition

class DeleteRealtimeEndpointInputRequestTypeDef(TypedDict):
    MLModelId: str,
```

## DeleteTagsInputRequestTypeDef

```python
# DeleteTagsInputRequestTypeDef definition

class DeleteTagsInputRequestTypeDef(TypedDict):
    TagKeys: Sequence[str],
    ResourceId: str,
    ResourceType: TaggableResourceTypeType,  # (1)
```

1. See [:material-code-brackets: TaggableResourceTypeType](./literals.md#taggableresourcetypetype) 
## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeBatchPredictionsInputRequestTypeDef

```python
# DescribeBatchPredictionsInputRequestTypeDef definition

class DescribeBatchPredictionsInputRequestTypeDef(TypedDict):
    FilterVariable: NotRequired[BatchPredictionFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: BatchPredictionFilterVariableType](./literals.md#batchpredictionfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## DescribeDataSourcesInputRequestTypeDef

```python
# DescribeDataSourcesInputRequestTypeDef definition

class DescribeDataSourcesInputRequestTypeDef(TypedDict):
    FilterVariable: NotRequired[DataSourceFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: DataSourceFilterVariableType](./literals.md#datasourcefiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## DescribeEvaluationsInputRequestTypeDef

```python
# DescribeEvaluationsInputRequestTypeDef definition

class DescribeEvaluationsInputRequestTypeDef(TypedDict):
    FilterVariable: NotRequired[EvaluationFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: EvaluationFilterVariableType](./literals.md#evaluationfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## DescribeMLModelsInputRequestTypeDef

```python
# DescribeMLModelsInputRequestTypeDef definition

class DescribeMLModelsInputRequestTypeDef(TypedDict):
    FilterVariable: NotRequired[MLModelFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: MLModelFilterVariableType](./literals.md#mlmodelfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## DescribeTagsInputRequestTypeDef

```python
# DescribeTagsInputRequestTypeDef definition

class DescribeTagsInputRequestTypeDef(TypedDict):
    ResourceId: str,
    ResourceType: TaggableResourceTypeType,  # (1)
```

1. See [:material-code-brackets: TaggableResourceTypeType](./literals.md#taggableresourcetypetype) 
## PerformanceMetricsTypeDef

```python
# PerformanceMetricsTypeDef definition

class PerformanceMetricsTypeDef(TypedDict):
    Properties: NotRequired[Dict[str, str]],
```

## GetBatchPredictionInputRequestTypeDef

```python
# GetBatchPredictionInputRequestTypeDef definition

class GetBatchPredictionInputRequestTypeDef(TypedDict):
    BatchPredictionId: str,
```

## GetDataSourceInputRequestTypeDef

```python
# GetDataSourceInputRequestTypeDef definition

class GetDataSourceInputRequestTypeDef(TypedDict):
    DataSourceId: str,
    Verbose: NotRequired[bool],
```

## GetEvaluationInputRequestTypeDef

```python
# GetEvaluationInputRequestTypeDef definition

class GetEvaluationInputRequestTypeDef(TypedDict):
    EvaluationId: str,
```

## GetMLModelInputRequestTypeDef

```python
# GetMLModelInputRequestTypeDef definition

class GetMLModelInputRequestTypeDef(TypedDict):
    MLModelId: str,
    Verbose: NotRequired[bool],
```

## PredictInputRequestTypeDef

```python
# PredictInputRequestTypeDef definition

class PredictInputRequestTypeDef(TypedDict):
    MLModelId: str,
    Record: Mapping[str, str],
    PredictEndpoint: str,
```

## PredictionTypeDef

```python
# PredictionTypeDef definition

class PredictionTypeDef(TypedDict):
    predictedLabel: NotRequired[str],
    predictedValue: NotRequired[float],
    predictedScores: NotRequired[Dict[str, float]],
    details: NotRequired[Dict[DetailsAttributesType, str]],  # (1)
```

1. See [:material-code-brackets: DetailsAttributesType](./literals.md#detailsattributestype) 
## RDSDatabaseCredentialsTypeDef

```python
# RDSDatabaseCredentialsTypeDef definition

class RDSDatabaseCredentialsTypeDef(TypedDict):
    Username: str,
    Password: str,
```

## RDSDatabaseTypeDef

```python
# RDSDatabaseTypeDef definition

class RDSDatabaseTypeDef(TypedDict):
    InstanceIdentifier: str,
    DatabaseName: str,
```

## RedshiftDatabaseCredentialsTypeDef

```python
# RedshiftDatabaseCredentialsTypeDef definition

class RedshiftDatabaseCredentialsTypeDef(TypedDict):
    Username: str,
    Password: str,
```

## RedshiftDatabaseTypeDef

```python
# RedshiftDatabaseTypeDef definition

class RedshiftDatabaseTypeDef(TypedDict):
    DatabaseName: str,
    ClusterIdentifier: str,
```

## UpdateBatchPredictionInputRequestTypeDef

```python
# UpdateBatchPredictionInputRequestTypeDef definition

class UpdateBatchPredictionInputRequestTypeDef(TypedDict):
    BatchPredictionId: str,
    BatchPredictionName: str,
```

## UpdateDataSourceInputRequestTypeDef

```python
# UpdateDataSourceInputRequestTypeDef definition

class UpdateDataSourceInputRequestTypeDef(TypedDict):
    DataSourceId: str,
    DataSourceName: str,
```

## UpdateEvaluationInputRequestTypeDef

```python
# UpdateEvaluationInputRequestTypeDef definition

class UpdateEvaluationInputRequestTypeDef(TypedDict):
    EvaluationId: str,
    EvaluationName: str,
```

## UpdateMLModelInputRequestTypeDef

```python
# UpdateMLModelInputRequestTypeDef definition

class UpdateMLModelInputRequestTypeDef(TypedDict):
    MLModelId: str,
    MLModelName: NotRequired[str],
    ScoreThreshold: NotRequired[float],
```

## AddTagsInputRequestTypeDef

```python
# AddTagsInputRequestTypeDef definition

class AddTagsInputRequestTypeDef(TypedDict):
    Tags: Sequence[TagTypeDef],  # (1)
    ResourceId: str,
    ResourceType: TaggableResourceTypeType,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: TaggableResourceTypeType](./literals.md#taggableresourcetypetype) 
## AddTagsOutputTypeDef

```python
# AddTagsOutputTypeDef definition

class AddTagsOutputTypeDef(TypedDict):
    ResourceId: str,
    ResourceType: TaggableResourceTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TaggableResourceTypeType](./literals.md#taggableresourcetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBatchPredictionOutputTypeDef

```python
# CreateBatchPredictionOutputTypeDef definition

class CreateBatchPredictionOutputTypeDef(TypedDict):
    BatchPredictionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSourceFromRDSOutputTypeDef

```python
# CreateDataSourceFromRDSOutputTypeDef definition

class CreateDataSourceFromRDSOutputTypeDef(TypedDict):
    DataSourceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSourceFromRedshiftOutputTypeDef

```python
# CreateDataSourceFromRedshiftOutputTypeDef definition

class CreateDataSourceFromRedshiftOutputTypeDef(TypedDict):
    DataSourceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSourceFromS3OutputTypeDef

```python
# CreateDataSourceFromS3OutputTypeDef definition

class CreateDataSourceFromS3OutputTypeDef(TypedDict):
    DataSourceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEvaluationOutputTypeDef

```python
# CreateEvaluationOutputTypeDef definition

class CreateEvaluationOutputTypeDef(TypedDict):
    EvaluationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMLModelOutputTypeDef

```python
# CreateMLModelOutputTypeDef definition

class CreateMLModelOutputTypeDef(TypedDict):
    MLModelId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBatchPredictionOutputTypeDef

```python
# DeleteBatchPredictionOutputTypeDef definition

class DeleteBatchPredictionOutputTypeDef(TypedDict):
    BatchPredictionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataSourceOutputTypeDef

```python
# DeleteDataSourceOutputTypeDef definition

class DeleteDataSourceOutputTypeDef(TypedDict):
    DataSourceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEvaluationOutputTypeDef

```python
# DeleteEvaluationOutputTypeDef definition

class DeleteEvaluationOutputTypeDef(TypedDict):
    EvaluationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMLModelOutputTypeDef

```python
# DeleteMLModelOutputTypeDef definition

class DeleteMLModelOutputTypeDef(TypedDict):
    MLModelId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTagsOutputTypeDef

```python
# DeleteTagsOutputTypeDef definition

class DeleteTagsOutputTypeDef(TypedDict):
    ResourceId: str,
    ResourceType: TaggableResourceTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TaggableResourceTypeType](./literals.md#taggableresourcetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTagsOutputTypeDef

```python
# DescribeTagsOutputTypeDef definition

class DescribeTagsOutputTypeDef(TypedDict):
    ResourceId: str,
    ResourceType: TaggableResourceTypeType,  # (1)
    Tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TaggableResourceTypeType](./literals.md#taggableresourcetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBatchPredictionOutputTypeDef

```python
# GetBatchPredictionOutputTypeDef definition

class GetBatchPredictionOutputTypeDef(TypedDict):
    BatchPredictionId: str,
    MLModelId: str,
    BatchPredictionDataSourceId: str,
    InputDataLocationS3: str,
    CreatedByIamUser: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Name: str,
    Status: EntityStatusType,  # (1)
    OutputUri: str,
    LogUri: str,
    Message: str,
    ComputeTime: int,
    FinishedAt: datetime,
    StartedAt: datetime,
    TotalRecordCount: int,
    InvalidRecordCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EntityStatusType](./literals.md#entitystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBatchPredictionOutputTypeDef

```python
# UpdateBatchPredictionOutputTypeDef definition

class UpdateBatchPredictionOutputTypeDef(TypedDict):
    BatchPredictionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataSourceOutputTypeDef

```python
# UpdateDataSourceOutputTypeDef definition

class UpdateDataSourceOutputTypeDef(TypedDict):
    DataSourceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEvaluationOutputTypeDef

```python
# UpdateEvaluationOutputTypeDef definition

class UpdateEvaluationOutputTypeDef(TypedDict):
    EvaluationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMLModelOutputTypeDef

```python
# UpdateMLModelOutputTypeDef definition

class UpdateMLModelOutputTypeDef(TypedDict):
    MLModelId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBatchPredictionsOutputTypeDef

```python
# DescribeBatchPredictionsOutputTypeDef definition

class DescribeBatchPredictionsOutputTypeDef(TypedDict):
    Results: List[BatchPredictionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPredictionTypeDef](./type_defs.md#batchpredictiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSourceFromS3InputRequestTypeDef

```python
# CreateDataSourceFromS3InputRequestTypeDef definition

class CreateDataSourceFromS3InputRequestTypeDef(TypedDict):
    DataSourceId: str,
    DataSpec: S3DataSpecTypeDef,  # (1)
    DataSourceName: NotRequired[str],
    ComputeStatistics: NotRequired[bool],
```

1. See [:material-code-braces: S3DataSpecTypeDef](./type_defs.md#s3dataspectypedef) 
## CreateRealtimeEndpointOutputTypeDef

```python
# CreateRealtimeEndpointOutputTypeDef definition

class CreateRealtimeEndpointOutputTypeDef(TypedDict):
    MLModelId: str,
    RealtimeEndpointInfo: RealtimeEndpointInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RealtimeEndpointInfoTypeDef](./type_defs.md#realtimeendpointinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRealtimeEndpointOutputTypeDef

```python
# DeleteRealtimeEndpointOutputTypeDef definition

class DeleteRealtimeEndpointOutputTypeDef(TypedDict):
    MLModelId: str,
    RealtimeEndpointInfo: RealtimeEndpointInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RealtimeEndpointInfoTypeDef](./type_defs.md#realtimeendpointinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMLModelOutputTypeDef

```python
# GetMLModelOutputTypeDef definition

class GetMLModelOutputTypeDef(TypedDict):
    MLModelId: str,
    TrainingDataSourceId: str,
    CreatedByIamUser: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Name: str,
    Status: EntityStatusType,  # (1)
    SizeInBytes: int,
    EndpointInfo: RealtimeEndpointInfoTypeDef,  # (2)
    TrainingParameters: Dict[str, str],
    InputDataLocationS3: str,
    MLModelType: MLModelTypeType,  # (3)
    ScoreThreshold: float,
    ScoreThresholdLastUpdatedAt: datetime,
    LogUri: str,
    Message: str,
    ComputeTime: int,
    FinishedAt: datetime,
    StartedAt: datetime,
    Recipe: str,
    Schema: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: EntityStatusType](./literals.md#entitystatustype) 
2. See [:material-code-braces: RealtimeEndpointInfoTypeDef](./type_defs.md#realtimeendpointinfotypedef) 
3. See [:material-code-brackets: MLModelTypeType](./literals.md#mlmodeltypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MLModelTypeDef

```python
# MLModelTypeDef definition

class MLModelTypeDef(TypedDict):
    MLModelId: NotRequired[str],
    TrainingDataSourceId: NotRequired[str],
    CreatedByIamUser: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    Name: NotRequired[str],
    Status: NotRequired[EntityStatusType],  # (1)
    SizeInBytes: NotRequired[int],
    EndpointInfo: NotRequired[RealtimeEndpointInfoTypeDef],  # (2)
    TrainingParameters: NotRequired[Dict[str, str]],
    InputDataLocationS3: NotRequired[str],
    Algorithm: NotRequired[AlgorithmType],  # (3)
    MLModelType: NotRequired[MLModelTypeType],  # (4)
    ScoreThreshold: NotRequired[float],
    ScoreThresholdLastUpdatedAt: NotRequired[datetime],
    Message: NotRequired[str],
    ComputeTime: NotRequired[int],
    FinishedAt: NotRequired[datetime],
    StartedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: EntityStatusType](./literals.md#entitystatustype) 
2. See [:material-code-braces: RealtimeEndpointInfoTypeDef](./type_defs.md#realtimeendpointinfotypedef) 
3. See [:material-code-brackets: AlgorithmType](./literals.md#algorithmtype) 
4. See [:material-code-brackets: MLModelTypeType](./literals.md#mlmodeltypetype) 
## DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef

```python
# DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef definition

class DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef(TypedDict):
    FilterVariable: NotRequired[BatchPredictionFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: BatchPredictionFilterVariableType](./literals.md#batchpredictionfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeDataSourcesInputDataSourceAvailableWaitTypeDef

```python
# DescribeDataSourcesInputDataSourceAvailableWaitTypeDef definition

class DescribeDataSourcesInputDataSourceAvailableWaitTypeDef(TypedDict):
    FilterVariable: NotRequired[DataSourceFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: DataSourceFilterVariableType](./literals.md#datasourcefiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEvaluationsInputEvaluationAvailableWaitTypeDef

```python
# DescribeEvaluationsInputEvaluationAvailableWaitTypeDef definition

class DescribeEvaluationsInputEvaluationAvailableWaitTypeDef(TypedDict):
    FilterVariable: NotRequired[EvaluationFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EvaluationFilterVariableType](./literals.md#evaluationfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeMLModelsInputMLModelAvailableWaitTypeDef

```python
# DescribeMLModelsInputMLModelAvailableWaitTypeDef definition

class DescribeMLModelsInputMLModelAvailableWaitTypeDef(TypedDict):
    FilterVariable: NotRequired[MLModelFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: MLModelFilterVariableType](./literals.md#mlmodelfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef

```python
# DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef definition

class DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef(TypedDict):
    FilterVariable: NotRequired[BatchPredictionFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: BatchPredictionFilterVariableType](./literals.md#batchpredictionfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef

```python
# DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef definition

class DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef(TypedDict):
    FilterVariable: NotRequired[DataSourceFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: DataSourceFilterVariableType](./literals.md#datasourcefiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef

```python
# DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef definition

class DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef(TypedDict):
    FilterVariable: NotRequired[EvaluationFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EvaluationFilterVariableType](./literals.md#evaluationfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMLModelsInputDescribeMLModelsPaginateTypeDef

```python
# DescribeMLModelsInputDescribeMLModelsPaginateTypeDef definition

class DescribeMLModelsInputDescribeMLModelsPaginateTypeDef(TypedDict):
    FilterVariable: NotRequired[MLModelFilterVariableType],  # (1)
    EQ: NotRequired[str],
    GT: NotRequired[str],
    LT: NotRequired[str],
    GE: NotRequired[str],
    LE: NotRequired[str],
    NE: NotRequired[str],
    Prefix: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: MLModelFilterVariableType](./literals.md#mlmodelfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## EvaluationTypeDef

```python
# EvaluationTypeDef definition

class EvaluationTypeDef(TypedDict):
    EvaluationId: NotRequired[str],
    MLModelId: NotRequired[str],
    EvaluationDataSourceId: NotRequired[str],
    InputDataLocationS3: NotRequired[str],
    CreatedByIamUser: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    Name: NotRequired[str],
    Status: NotRequired[EntityStatusType],  # (1)
    PerformanceMetrics: NotRequired[PerformanceMetricsTypeDef],  # (2)
    Message: NotRequired[str],
    ComputeTime: NotRequired[int],
    FinishedAt: NotRequired[datetime],
    StartedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: EntityStatusType](./literals.md#entitystatustype) 
2. See [:material-code-braces: PerformanceMetricsTypeDef](./type_defs.md#performancemetricstypedef) 
## GetEvaluationOutputTypeDef

```python
# GetEvaluationOutputTypeDef definition

class GetEvaluationOutputTypeDef(TypedDict):
    EvaluationId: str,
    MLModelId: str,
    EvaluationDataSourceId: str,
    InputDataLocationS3: str,
    CreatedByIamUser: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    Name: str,
    Status: EntityStatusType,  # (1)
    PerformanceMetrics: PerformanceMetricsTypeDef,  # (2)
    LogUri: str,
    Message: str,
    ComputeTime: int,
    FinishedAt: datetime,
    StartedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EntityStatusType](./literals.md#entitystatustype) 
2. See [:material-code-braces: PerformanceMetricsTypeDef](./type_defs.md#performancemetricstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PredictOutputTypeDef

```python
# PredictOutputTypeDef definition

class PredictOutputTypeDef(TypedDict):
    Prediction: PredictionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PredictionTypeDef](./type_defs.md#predictiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RDSDataSpecTypeDef

```python
# RDSDataSpecTypeDef definition

class RDSDataSpecTypeDef(TypedDict):
    DatabaseInformation: RDSDatabaseTypeDef,  # (1)
    SelectSqlQuery: str,
    DatabaseCredentials: RDSDatabaseCredentialsTypeDef,  # (2)
    S3StagingLocation: str,
    ResourceRole: str,
    ServiceRole: str,
    SubnetId: str,
    SecurityGroupIds: Sequence[str],
    DataRearrangement: NotRequired[str],
    DataSchema: NotRequired[str],
    DataSchemaUri: NotRequired[str],
```

1. See [:material-code-braces: RDSDatabaseTypeDef](./type_defs.md#rdsdatabasetypedef) 
2. See [:material-code-braces: RDSDatabaseCredentialsTypeDef](./type_defs.md#rdsdatabasecredentialstypedef) 
## RDSMetadataTypeDef

```python
# RDSMetadataTypeDef definition

class RDSMetadataTypeDef(TypedDict):
    Database: NotRequired[RDSDatabaseTypeDef],  # (1)
    DatabaseUserName: NotRequired[str],
    SelectSqlQuery: NotRequired[str],
    ResourceRole: NotRequired[str],
    ServiceRole: NotRequired[str],
    DataPipelineId: NotRequired[str],
```

1. See [:material-code-braces: RDSDatabaseTypeDef](./type_defs.md#rdsdatabasetypedef) 
## RedshiftDataSpecTypeDef

```python
# RedshiftDataSpecTypeDef definition

class RedshiftDataSpecTypeDef(TypedDict):
    DatabaseInformation: RedshiftDatabaseTypeDef,  # (1)
    SelectSqlQuery: str,
    DatabaseCredentials: RedshiftDatabaseCredentialsTypeDef,  # (2)
    S3StagingLocation: str,
    DataRearrangement: NotRequired[str],
    DataSchema: NotRequired[str],
    DataSchemaUri: NotRequired[str],
```

1. See [:material-code-braces: RedshiftDatabaseTypeDef](./type_defs.md#redshiftdatabasetypedef) 
2. See [:material-code-braces: RedshiftDatabaseCredentialsTypeDef](./type_defs.md#redshiftdatabasecredentialstypedef) 
## RedshiftMetadataTypeDef

```python
# RedshiftMetadataTypeDef definition

class RedshiftMetadataTypeDef(TypedDict):
    RedshiftDatabase: NotRequired[RedshiftDatabaseTypeDef],  # (1)
    DatabaseUserName: NotRequired[str],
    SelectSqlQuery: NotRequired[str],
```

1. See [:material-code-braces: RedshiftDatabaseTypeDef](./type_defs.md#redshiftdatabasetypedef) 
## DescribeMLModelsOutputTypeDef

```python
# DescribeMLModelsOutputTypeDef definition

class DescribeMLModelsOutputTypeDef(TypedDict):
    Results: List[MLModelTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MLModelTypeDef](./type_defs.md#mlmodeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEvaluationsOutputTypeDef

```python
# DescribeEvaluationsOutputTypeDef definition

class DescribeEvaluationsOutputTypeDef(TypedDict):
    Results: List[EvaluationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvaluationTypeDef](./type_defs.md#evaluationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSourceFromRDSInputRequestTypeDef

```python
# CreateDataSourceFromRDSInputRequestTypeDef definition

class CreateDataSourceFromRDSInputRequestTypeDef(TypedDict):
    DataSourceId: str,
    RDSData: RDSDataSpecTypeDef,  # (1)
    RoleARN: str,
    DataSourceName: NotRequired[str],
    ComputeStatistics: NotRequired[bool],
```

1. See [:material-code-braces: RDSDataSpecTypeDef](./type_defs.md#rdsdataspectypedef) 
## CreateDataSourceFromRedshiftInputRequestTypeDef

```python
# CreateDataSourceFromRedshiftInputRequestTypeDef definition

class CreateDataSourceFromRedshiftInputRequestTypeDef(TypedDict):
    DataSourceId: str,
    DataSpec: RedshiftDataSpecTypeDef,  # (1)
    RoleARN: str,
    DataSourceName: NotRequired[str],
    ComputeStatistics: NotRequired[bool],
```

1. See [:material-code-braces: RedshiftDataSpecTypeDef](./type_defs.md#redshiftdataspectypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    DataSourceId: NotRequired[str],
    DataLocationS3: NotRequired[str],
    DataRearrangement: NotRequired[str],
    CreatedByIamUser: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    DataSizeInBytes: NotRequired[int],
    NumberOfFiles: NotRequired[int],
    Name: NotRequired[str],
    Status: NotRequired[EntityStatusType],  # (1)
    Message: NotRequired[str],
    RedshiftMetadata: NotRequired[RedshiftMetadataTypeDef],  # (2)
    RDSMetadata: NotRequired[RDSMetadataTypeDef],  # (3)
    RoleARN: NotRequired[str],
    ComputeStatistics: NotRequired[bool],
    ComputeTime: NotRequired[int],
    FinishedAt: NotRequired[datetime],
    StartedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: EntityStatusType](./literals.md#entitystatustype) 
2. See [:material-code-braces: RedshiftMetadataTypeDef](./type_defs.md#redshiftmetadatatypedef) 
3. See [:material-code-braces: RDSMetadataTypeDef](./type_defs.md#rdsmetadatatypedef) 
## GetDataSourceOutputTypeDef

```python
# GetDataSourceOutputTypeDef definition

class GetDataSourceOutputTypeDef(TypedDict):
    DataSourceId: str,
    DataLocationS3: str,
    DataRearrangement: str,
    CreatedByIamUser: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    DataSizeInBytes: int,
    NumberOfFiles: int,
    Name: str,
    Status: EntityStatusType,  # (1)
    LogUri: str,
    Message: str,
    RedshiftMetadata: RedshiftMetadataTypeDef,  # (2)
    RDSMetadata: RDSMetadataTypeDef,  # (3)
    RoleARN: str,
    ComputeStatistics: bool,
    ComputeTime: int,
    FinishedAt: datetime,
    StartedAt: datetime,
    DataSourceSchema: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: EntityStatusType](./literals.md#entitystatustype) 
2. See [:material-code-braces: RedshiftMetadataTypeDef](./type_defs.md#redshiftmetadatatypedef) 
3. See [:material-code-braces: RDSMetadataTypeDef](./type_defs.md#rdsmetadatatypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataSourcesOutputTypeDef

```python
# DescribeDataSourcesOutputTypeDef definition

class DescribeDataSourcesOutputTypeDef(TypedDict):
    Results: List[DataSourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
