# Type definitions

> [Index](../README.md) > [NeptuneData](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [NeptuneData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData)
    type annotations stubs module [types-aiobotocore-neptunedata](https://pypi.org/project/types-aiobotocore-neptunedata/).



## CancelGremlinQueryInputRequestTypeDef

```python
# CancelGremlinQueryInputRequestTypeDef definition

class CancelGremlinQueryInputRequestTypeDef(TypedDict):
    queryId: str,
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

## CancelLoaderJobInputRequestTypeDef

```python
# CancelLoaderJobInputRequestTypeDef definition

class CancelLoaderJobInputRequestTypeDef(TypedDict):
    loadId: str,
```

## CancelMLDataProcessingJobInputRequestTypeDef

```python
# CancelMLDataProcessingJobInputRequestTypeDef definition

class CancelMLDataProcessingJobInputRequestTypeDef(TypedDict):
    id: str,
    neptuneIamRoleArn: NotRequired[str],
    clean: NotRequired[bool],
```

## CancelMLModelTrainingJobInputRequestTypeDef

```python
# CancelMLModelTrainingJobInputRequestTypeDef definition

class CancelMLModelTrainingJobInputRequestTypeDef(TypedDict):
    id: str,
    neptuneIamRoleArn: NotRequired[str],
    clean: NotRequired[bool],
```

## CancelMLModelTransformJobInputRequestTypeDef

```python
# CancelMLModelTransformJobInputRequestTypeDef definition

class CancelMLModelTransformJobInputRequestTypeDef(TypedDict):
    id: str,
    neptuneIamRoleArn: NotRequired[str],
    clean: NotRequired[bool],
```

## CancelOpenCypherQueryInputRequestTypeDef

```python
# CancelOpenCypherQueryInputRequestTypeDef definition

class CancelOpenCypherQueryInputRequestTypeDef(TypedDict):
    queryId: str,
    silent: NotRequired[bool],
```

## CreateMLEndpointInputRequestTypeDef

```python
# CreateMLEndpointInputRequestTypeDef definition

class CreateMLEndpointInputRequestTypeDef(TypedDict):
    id: NotRequired[str],
    mlModelTrainingJobId: NotRequired[str],
    mlModelTransformJobId: NotRequired[str],
    update: NotRequired[bool],
    neptuneIamRoleArn: NotRequired[str],
    modelName: NotRequired[str],
    instanceType: NotRequired[str],
    instanceCount: NotRequired[int],
    volumeEncryptionKMSKey: NotRequired[str],
```

## CustomModelTrainingParametersTypeDef

```python
# CustomModelTrainingParametersTypeDef definition

class CustomModelTrainingParametersTypeDef(TypedDict):
    sourceS3DirectoryPath: str,
    trainingEntryPointScript: NotRequired[str],
    transformEntryPointScript: NotRequired[str],
```

## CustomModelTransformParametersTypeDef

```python
# CustomModelTransformParametersTypeDef definition

class CustomModelTransformParametersTypeDef(TypedDict):
    sourceS3DirectoryPath: str,
    transformEntryPointScript: NotRequired[str],
```

## DeleteMLEndpointInputRequestTypeDef

```python
# DeleteMLEndpointInputRequestTypeDef definition

class DeleteMLEndpointInputRequestTypeDef(TypedDict):
    id: str,
    neptuneIamRoleArn: NotRequired[str],
    clean: NotRequired[bool],
```

## DeleteStatisticsValueMapTypeDef

```python
# DeleteStatisticsValueMapTypeDef definition

class DeleteStatisticsValueMapTypeDef(TypedDict):
    active: NotRequired[bool],
    statisticsId: NotRequired[str],
```

## EdgeStructureTypeDef

```python
# EdgeStructureTypeDef definition

class EdgeStructureTypeDef(TypedDict):
    count: NotRequired[int],
    edgeProperties: NotRequired[List[str]],
```

## ExecuteFastResetInputRequestTypeDef

```python
# ExecuteFastResetInputRequestTypeDef definition

class ExecuteFastResetInputRequestTypeDef(TypedDict):
    action: ActionType,  # (1)
    token: NotRequired[str],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
## FastResetTokenTypeDef

```python
# FastResetTokenTypeDef definition

class FastResetTokenTypeDef(TypedDict):
    token: NotRequired[str],
```

## ExecuteGremlinExplainQueryInputRequestTypeDef

```python
# ExecuteGremlinExplainQueryInputRequestTypeDef definition

class ExecuteGremlinExplainQueryInputRequestTypeDef(TypedDict):
    gremlinQuery: str,
```

## ExecuteGremlinProfileQueryInputRequestTypeDef

```python
# ExecuteGremlinProfileQueryInputRequestTypeDef definition

class ExecuteGremlinProfileQueryInputRequestTypeDef(TypedDict):
    gremlinQuery: str,
    results: NotRequired[bool],
    chop: NotRequired[int],
    serializer: NotRequired[str],
    indexOps: NotRequired[bool],
```

## ExecuteGremlinQueryInputRequestTypeDef

```python
# ExecuteGremlinQueryInputRequestTypeDef definition

class ExecuteGremlinQueryInputRequestTypeDef(TypedDict):
    gremlinQuery: str,
    serializer: NotRequired[str],
```

## GremlinQueryStatusAttributesTypeDef

```python
# GremlinQueryStatusAttributesTypeDef definition

class GremlinQueryStatusAttributesTypeDef(TypedDict):
    message: NotRequired[str],
    code: NotRequired[int],
    attributes: NotRequired[Dict[str, Any]],
```

## ExecuteOpenCypherExplainQueryInputRequestTypeDef

```python
# ExecuteOpenCypherExplainQueryInputRequestTypeDef definition

class ExecuteOpenCypherExplainQueryInputRequestTypeDef(TypedDict):
    openCypherQuery: str,
    explainMode: OpenCypherExplainModeType,  # (1)
    parameters: NotRequired[str],
```

1. See [:material-code-brackets: OpenCypherExplainModeType](./literals.md#opencypherexplainmodetype) 
## ExecuteOpenCypherQueryInputRequestTypeDef

```python
# ExecuteOpenCypherQueryInputRequestTypeDef definition

class ExecuteOpenCypherQueryInputRequestTypeDef(TypedDict):
    openCypherQuery: str,
    parameters: NotRequired[str],
```

## QueryLanguageVersionTypeDef

```python
# QueryLanguageVersionTypeDef definition

class QueryLanguageVersionTypeDef(TypedDict):
    version: str,
```

## GetGremlinQueryStatusInputRequestTypeDef

```python
# GetGremlinQueryStatusInputRequestTypeDef definition

class GetGremlinQueryStatusInputRequestTypeDef(TypedDict):
    queryId: str,
```

## QueryEvalStatsTypeDef

```python
# QueryEvalStatsTypeDef definition

class QueryEvalStatsTypeDef(TypedDict):
    waited: NotRequired[int],
    elapsed: NotRequired[int],
    cancelled: NotRequired[bool],
    subqueries: NotRequired[Dict[str, Any]],
```

## GetLoaderJobStatusInputRequestTypeDef

```python
# GetLoaderJobStatusInputRequestTypeDef definition

class GetLoaderJobStatusInputRequestTypeDef(TypedDict):
    loadId: str,
    details: NotRequired[bool],
    errors: NotRequired[bool],
    page: NotRequired[int],
    errorsPerPage: NotRequired[int],
```

## GetMLDataProcessingJobInputRequestTypeDef

```python
# GetMLDataProcessingJobInputRequestTypeDef definition

class GetMLDataProcessingJobInputRequestTypeDef(TypedDict):
    id: str,
    neptuneIamRoleArn: NotRequired[str],
```

## MlResourceDefinitionTypeDef

```python
# MlResourceDefinitionTypeDef definition

class MlResourceDefinitionTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    status: NotRequired[str],
    outputLocation: NotRequired[str],
    failureReason: NotRequired[str],
    cloudwatchLogUrl: NotRequired[str],
```

## GetMLEndpointInputRequestTypeDef

```python
# GetMLEndpointInputRequestTypeDef definition

class GetMLEndpointInputRequestTypeDef(TypedDict):
    id: str,
    neptuneIamRoleArn: NotRequired[str],
```

## MlConfigDefinitionTypeDef

```python
# MlConfigDefinitionTypeDef definition

class MlConfigDefinitionTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
```

## GetMLModelTrainingJobInputRequestTypeDef

```python
# GetMLModelTrainingJobInputRequestTypeDef definition

class GetMLModelTrainingJobInputRequestTypeDef(TypedDict):
    id: str,
    neptuneIamRoleArn: NotRequired[str],
```

## GetMLModelTransformJobInputRequestTypeDef

```python
# GetMLModelTransformJobInputRequestTypeDef definition

class GetMLModelTransformJobInputRequestTypeDef(TypedDict):
    id: str,
    neptuneIamRoleArn: NotRequired[str],
```

## GetOpenCypherQueryStatusInputRequestTypeDef

```python
# GetOpenCypherQueryStatusInputRequestTypeDef definition

class GetOpenCypherQueryStatusInputRequestTypeDef(TypedDict):
    queryId: str,
```

## GetPropertygraphStreamInputRequestTypeDef

```python
# GetPropertygraphStreamInputRequestTypeDef definition

class GetPropertygraphStreamInputRequestTypeDef(TypedDict):
    limit: NotRequired[int],
    iteratorType: NotRequired[IteratorTypeType],  # (1)
    commitNum: NotRequired[int],
    opNum: NotRequired[int],
    encoding: NotRequired[EncodingType],  # (2)
```

1. See [:material-code-brackets: IteratorTypeType](./literals.md#iteratortypetype) 
2. See [:material-code-brackets: EncodingType](./literals.md#encodingtype) 
## GetPropertygraphSummaryInputRequestTypeDef

```python
# GetPropertygraphSummaryInputRequestTypeDef definition

class GetPropertygraphSummaryInputRequestTypeDef(TypedDict):
    mode: NotRequired[GraphSummaryTypeType],  # (1)
```

1. See [:material-code-brackets: GraphSummaryTypeType](./literals.md#graphsummarytypetype) 
## GetRDFGraphSummaryInputRequestTypeDef

```python
# GetRDFGraphSummaryInputRequestTypeDef definition

class GetRDFGraphSummaryInputRequestTypeDef(TypedDict):
    mode: NotRequired[GraphSummaryTypeType],  # (1)
```

1. See [:material-code-brackets: GraphSummaryTypeType](./literals.md#graphsummarytypetype) 
## GetSparqlStreamInputRequestTypeDef

```python
# GetSparqlStreamInputRequestTypeDef definition

class GetSparqlStreamInputRequestTypeDef(TypedDict):
    limit: NotRequired[int],
    iteratorType: NotRequired[IteratorTypeType],  # (1)
    commitNum: NotRequired[int],
    opNum: NotRequired[int],
    encoding: NotRequired[EncodingType],  # (2)
```

1. See [:material-code-brackets: IteratorTypeType](./literals.md#iteratortypetype) 
2. See [:material-code-brackets: EncodingType](./literals.md#encodingtype) 
## ListGremlinQueriesInputRequestTypeDef

```python
# ListGremlinQueriesInputRequestTypeDef definition

class ListGremlinQueriesInputRequestTypeDef(TypedDict):
    includeWaiting: NotRequired[bool],
```

## ListLoaderJobsInputRequestTypeDef

```python
# ListLoaderJobsInputRequestTypeDef definition

class ListLoaderJobsInputRequestTypeDef(TypedDict):
    limit: NotRequired[int],
    includeQueuedLoads: NotRequired[bool],
```

## LoaderIdResultTypeDef

```python
# LoaderIdResultTypeDef definition

class LoaderIdResultTypeDef(TypedDict):
    loadIds: NotRequired[List[str]],
```

## ListMLDataProcessingJobsInputRequestTypeDef

```python
# ListMLDataProcessingJobsInputRequestTypeDef definition

class ListMLDataProcessingJobsInputRequestTypeDef(TypedDict):
    maxItems: NotRequired[int],
    neptuneIamRoleArn: NotRequired[str],
```

## ListMLEndpointsInputRequestTypeDef

```python
# ListMLEndpointsInputRequestTypeDef definition

class ListMLEndpointsInputRequestTypeDef(TypedDict):
    maxItems: NotRequired[int],
    neptuneIamRoleArn: NotRequired[str],
```

## ListMLModelTrainingJobsInputRequestTypeDef

```python
# ListMLModelTrainingJobsInputRequestTypeDef definition

class ListMLModelTrainingJobsInputRequestTypeDef(TypedDict):
    maxItems: NotRequired[int],
    neptuneIamRoleArn: NotRequired[str],
```

## ListMLModelTransformJobsInputRequestTypeDef

```python
# ListMLModelTransformJobsInputRequestTypeDef definition

class ListMLModelTransformJobsInputRequestTypeDef(TypedDict):
    maxItems: NotRequired[int],
    neptuneIamRoleArn: NotRequired[str],
```

## ListOpenCypherQueriesInputRequestTypeDef

```python
# ListOpenCypherQueriesInputRequestTypeDef definition

class ListOpenCypherQueriesInputRequestTypeDef(TypedDict):
    includeWaiting: NotRequired[bool],
```

## ManagePropertygraphStatisticsInputRequestTypeDef

```python
# ManagePropertygraphStatisticsInputRequestTypeDef definition

class ManagePropertygraphStatisticsInputRequestTypeDef(TypedDict):
    mode: NotRequired[StatisticsAutoGenerationModeType],  # (1)
```

1. See [:material-code-brackets: StatisticsAutoGenerationModeType](./literals.md#statisticsautogenerationmodetype) 
## RefreshStatisticsIdMapTypeDef

```python
# RefreshStatisticsIdMapTypeDef definition

class RefreshStatisticsIdMapTypeDef(TypedDict):
    statisticsId: NotRequired[str],
```

## ManageSparqlStatisticsInputRequestTypeDef

```python
# ManageSparqlStatisticsInputRequestTypeDef definition

class ManageSparqlStatisticsInputRequestTypeDef(TypedDict):
    mode: NotRequired[StatisticsAutoGenerationModeType],  # (1)
```

1. See [:material-code-brackets: StatisticsAutoGenerationModeType](./literals.md#statisticsautogenerationmodetype) 
## NodeStructureTypeDef

```python
# NodeStructureTypeDef definition

class NodeStructureTypeDef(TypedDict):
    count: NotRequired[int],
    nodeProperties: NotRequired[List[str]],
    distinctOutgoingEdgeLabels: NotRequired[List[str]],
```

## PropertygraphDataTypeDef

```python
# PropertygraphDataTypeDef definition

class PropertygraphDataTypeDef(TypedDict):
    id: str,
    type: str,
    key: str,
    value: Dict[str, Any],
    from: NotRequired[str],
    to: NotRequired[str],
```

## SubjectStructureTypeDef

```python
# SubjectStructureTypeDef definition

class SubjectStructureTypeDef(TypedDict):
    count: NotRequired[int],
    predicates: NotRequired[List[str]],
```

## SparqlDataTypeDef

```python
# SparqlDataTypeDef definition

class SparqlDataTypeDef(TypedDict):
    stmt: str,
```

## StartLoaderJobInputRequestTypeDef

```python
# StartLoaderJobInputRequestTypeDef definition

class StartLoaderJobInputRequestTypeDef(TypedDict):
    source: str,
    format: FormatType,  # (1)
    s3BucketRegion: S3BucketRegionType,  # (2)
    iamRoleArn: str,
    mode: NotRequired[ModeType],  # (3)
    failOnError: NotRequired[bool],
    parallelism: NotRequired[ParallelismType],  # (4)
    parserConfiguration: NotRequired[Mapping[str, str]],
    updateSingleCardinalityProperties: NotRequired[bool],
    queueRequest: NotRequired[bool],
    dependencies: NotRequired[Sequence[str]],
    userProvidedEdgeIds: NotRequired[bool],
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
2. See [:material-code-brackets: S3BucketRegionType](./literals.md#s3bucketregiontype) 
3. See [:material-code-brackets: ModeType](./literals.md#modetype) 
4. See [:material-code-brackets: ParallelismType](./literals.md#parallelismtype) 
## StartMLDataProcessingJobInputRequestTypeDef

```python
# StartMLDataProcessingJobInputRequestTypeDef definition

class StartMLDataProcessingJobInputRequestTypeDef(TypedDict):
    inputDataS3Location: str,
    processedDataS3Location: str,
    id: NotRequired[str],
    previousDataProcessingJobId: NotRequired[str],
    sagemakerIamRoleArn: NotRequired[str],
    neptuneIamRoleArn: NotRequired[str],
    processingInstanceType: NotRequired[str],
    processingInstanceVolumeSizeInGB: NotRequired[int],
    processingTimeOutInSeconds: NotRequired[int],
    modelType: NotRequired[str],
    configFileName: NotRequired[str],
    subnets: NotRequired[Sequence[str]],
    securityGroupIds: NotRequired[Sequence[str]],
    volumeEncryptionKMSKey: NotRequired[str],
    s3OutputEncryptionKMSKey: NotRequired[str],
```

## StatisticsSummaryTypeDef

```python
# StatisticsSummaryTypeDef definition

class StatisticsSummaryTypeDef(TypedDict):
    signatureCount: NotRequired[int],
    instanceCount: NotRequired[int],
    predicateCount: NotRequired[int],
```

## CancelGremlinQueryOutputTypeDef

```python
# CancelGremlinQueryOutputTypeDef definition

class CancelGremlinQueryOutputTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelLoaderJobOutputTypeDef

```python
# CancelLoaderJobOutputTypeDef definition

class CancelLoaderJobOutputTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelMLDataProcessingJobOutputTypeDef

```python
# CancelMLDataProcessingJobOutputTypeDef definition

class CancelMLDataProcessingJobOutputTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelMLModelTrainingJobOutputTypeDef

```python
# CancelMLModelTrainingJobOutputTypeDef definition

class CancelMLModelTrainingJobOutputTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelMLModelTransformJobOutputTypeDef

```python
# CancelMLModelTransformJobOutputTypeDef definition

class CancelMLModelTransformJobOutputTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelOpenCypherQueryOutputTypeDef

```python
# CancelOpenCypherQueryOutputTypeDef definition

class CancelOpenCypherQueryOutputTypeDef(TypedDict):
    status: str,
    payload: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMLEndpointOutputTypeDef

```python
# CreateMLEndpointOutputTypeDef definition

class CreateMLEndpointOutputTypeDef(TypedDict):
    id: str,
    arn: str,
    creationTimeInMillis: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMLEndpointOutputTypeDef

```python
# DeleteMLEndpointOutputTypeDef definition

class DeleteMLEndpointOutputTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteGremlinExplainQueryOutputTypeDef

```python
# ExecuteGremlinExplainQueryOutputTypeDef definition

class ExecuteGremlinExplainQueryOutputTypeDef(TypedDict):
    output: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteGremlinProfileQueryOutputTypeDef

```python
# ExecuteGremlinProfileQueryOutputTypeDef definition

class ExecuteGremlinProfileQueryOutputTypeDef(TypedDict):
    output: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteOpenCypherExplainQueryOutputTypeDef

```python
# ExecuteOpenCypherExplainQueryOutputTypeDef definition

class ExecuteOpenCypherExplainQueryOutputTypeDef(TypedDict):
    results: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteOpenCypherQueryOutputTypeDef

```python
# ExecuteOpenCypherQueryOutputTypeDef definition

class ExecuteOpenCypherQueryOutputTypeDef(TypedDict):
    results: Dict[str, Any],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLoaderJobStatusOutputTypeDef

```python
# GetLoaderJobStatusOutputTypeDef definition

class GetLoaderJobStatusOutputTypeDef(TypedDict):
    status: str,
    payload: Dict[str, Any],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMLDataProcessingJobsOutputTypeDef

```python
# ListMLDataProcessingJobsOutputTypeDef definition

class ListMLDataProcessingJobsOutputTypeDef(TypedDict):
    ids: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMLEndpointsOutputTypeDef

```python
# ListMLEndpointsOutputTypeDef definition

class ListMLEndpointsOutputTypeDef(TypedDict):
    ids: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMLModelTrainingJobsOutputTypeDef

```python
# ListMLModelTrainingJobsOutputTypeDef definition

class ListMLModelTrainingJobsOutputTypeDef(TypedDict):
    ids: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMLModelTransformJobsOutputTypeDef

```python
# ListMLModelTransformJobsOutputTypeDef definition

class ListMLModelTransformJobsOutputTypeDef(TypedDict):
    ids: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartLoaderJobOutputTypeDef

```python
# StartLoaderJobOutputTypeDef definition

class StartLoaderJobOutputTypeDef(TypedDict):
    status: str,
    payload: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMLDataProcessingJobOutputTypeDef

```python
# StartMLDataProcessingJobOutputTypeDef definition

class StartMLDataProcessingJobOutputTypeDef(TypedDict):
    id: str,
    arn: str,
    creationTimeInMillis: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMLModelTrainingJobOutputTypeDef

```python
# StartMLModelTrainingJobOutputTypeDef definition

class StartMLModelTrainingJobOutputTypeDef(TypedDict):
    id: str,
    arn: str,
    creationTimeInMillis: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMLModelTransformJobOutputTypeDef

```python
# StartMLModelTransformJobOutputTypeDef definition

class StartMLModelTransformJobOutputTypeDef(TypedDict):
    id: str,
    arn: str,
    creationTimeInMillis: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMLModelTrainingJobInputRequestTypeDef

```python
# StartMLModelTrainingJobInputRequestTypeDef definition

class StartMLModelTrainingJobInputRequestTypeDef(TypedDict):
    dataProcessingJobId: str,
    trainModelS3Location: str,
    id: NotRequired[str],
    previousModelTrainingJobId: NotRequired[str],
    sagemakerIamRoleArn: NotRequired[str],
    neptuneIamRoleArn: NotRequired[str],
    baseProcessingInstanceType: NotRequired[str],
    trainingInstanceType: NotRequired[str],
    trainingInstanceVolumeSizeInGB: NotRequired[int],
    trainingTimeOutInSeconds: NotRequired[int],
    maxHPONumberOfTrainingJobs: NotRequired[int],
    maxHPOParallelTrainingJobs: NotRequired[int],
    subnets: NotRequired[Sequence[str]],
    securityGroupIds: NotRequired[Sequence[str]],
    volumeEncryptionKMSKey: NotRequired[str],
    s3OutputEncryptionKMSKey: NotRequired[str],
    enableManagedSpotTraining: NotRequired[bool],
    customModelTrainingParameters: NotRequired[CustomModelTrainingParametersTypeDef],  # (1)
```

1. See [:material-code-braces: CustomModelTrainingParametersTypeDef](./type_defs.md#custommodeltrainingparameterstypedef) 
## StartMLModelTransformJobInputRequestTypeDef

```python
# StartMLModelTransformJobInputRequestTypeDef definition

class StartMLModelTransformJobInputRequestTypeDef(TypedDict):
    modelTransformOutputS3Location: str,
    id: NotRequired[str],
    dataProcessingJobId: NotRequired[str],
    mlModelTrainingJobId: NotRequired[str],
    trainingJobName: NotRequired[str],
    sagemakerIamRoleArn: NotRequired[str],
    neptuneIamRoleArn: NotRequired[str],
    customModelTransformParameters: NotRequired[CustomModelTransformParametersTypeDef],  # (1)
    baseProcessingInstanceType: NotRequired[str],
    baseProcessingInstanceVolumeSizeInGB: NotRequired[int],
    subnets: NotRequired[Sequence[str]],
    securityGroupIds: NotRequired[Sequence[str]],
    volumeEncryptionKMSKey: NotRequired[str],
    s3OutputEncryptionKMSKey: NotRequired[str],
```

1. See [:material-code-braces: CustomModelTransformParametersTypeDef](./type_defs.md#custommodeltransformparameterstypedef) 
## DeletePropertygraphStatisticsOutputTypeDef

```python
# DeletePropertygraphStatisticsOutputTypeDef definition

class DeletePropertygraphStatisticsOutputTypeDef(TypedDict):
    statusCode: int,
    status: str,
    payload: DeleteStatisticsValueMapTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeleteStatisticsValueMapTypeDef](./type_defs.md#deletestatisticsvaluemaptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSparqlStatisticsOutputTypeDef

```python
# DeleteSparqlStatisticsOutputTypeDef definition

class DeleteSparqlStatisticsOutputTypeDef(TypedDict):
    statusCode: int,
    status: str,
    payload: DeleteStatisticsValueMapTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeleteStatisticsValueMapTypeDef](./type_defs.md#deletestatisticsvaluemaptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteFastResetOutputTypeDef

```python
# ExecuteFastResetOutputTypeDef definition

class ExecuteFastResetOutputTypeDef(TypedDict):
    status: str,
    payload: FastResetTokenTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FastResetTokenTypeDef](./type_defs.md#fastresettokentypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteGremlinQueryOutputTypeDef

```python
# ExecuteGremlinQueryOutputTypeDef definition

class ExecuteGremlinQueryOutputTypeDef(TypedDict):
    requestId: str,
    status: GremlinQueryStatusAttributesTypeDef,  # (1)
    result: Dict[str, Any],
    meta: Dict[str, Any],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GremlinQueryStatusAttributesTypeDef](./type_defs.md#gremlinquerystatusattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEngineStatusOutputTypeDef

```python
# GetEngineStatusOutputTypeDef definition

class GetEngineStatusOutputTypeDef(TypedDict):
    status: str,
    startTime: str,
    dbEngineVersion: str,
    role: str,
    dfeQueryEngine: str,
    gremlin: QueryLanguageVersionTypeDef,  # (1)
    sparql: QueryLanguageVersionTypeDef,  # (1)
    opencypher: QueryLanguageVersionTypeDef,  # (1)
    labMode: Dict[str, str],
    rollingBackTrxCount: int,
    rollingBackTrxEarliestStartTime: str,
    features: Dict[str, Dict[str, Any]],
    settings: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: QueryLanguageVersionTypeDef](./type_defs.md#querylanguageversiontypedef) 
2. See [:material-code-braces: QueryLanguageVersionTypeDef](./type_defs.md#querylanguageversiontypedef) 
3. See [:material-code-braces: QueryLanguageVersionTypeDef](./type_defs.md#querylanguageversiontypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGremlinQueryStatusOutputTypeDef

```python
# GetGremlinQueryStatusOutputTypeDef definition

class GetGremlinQueryStatusOutputTypeDef(TypedDict):
    queryId: str,
    queryString: str,
    queryEvalStats: QueryEvalStatsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueryEvalStatsTypeDef](./type_defs.md#queryevalstatstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOpenCypherQueryStatusOutputTypeDef

```python
# GetOpenCypherQueryStatusOutputTypeDef definition

class GetOpenCypherQueryStatusOutputTypeDef(TypedDict):
    queryId: str,
    queryString: str,
    queryEvalStats: QueryEvalStatsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueryEvalStatsTypeDef](./type_defs.md#queryevalstatstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GremlinQueryStatusTypeDef

```python
# GremlinQueryStatusTypeDef definition

class GremlinQueryStatusTypeDef(TypedDict):
    queryId: NotRequired[str],
    queryString: NotRequired[str],
    queryEvalStats: NotRequired[QueryEvalStatsTypeDef],  # (1)
```

1. See [:material-code-braces: QueryEvalStatsTypeDef](./type_defs.md#queryevalstatstypedef) 
## GetMLDataProcessingJobOutputTypeDef

```python
# GetMLDataProcessingJobOutputTypeDef definition

class GetMLDataProcessingJobOutputTypeDef(TypedDict):
    status: str,
    id: str,
    processingJob: MlResourceDefinitionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MlResourceDefinitionTypeDef](./type_defs.md#mlresourcedefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMLEndpointOutputTypeDef

```python
# GetMLEndpointOutputTypeDef definition

class GetMLEndpointOutputTypeDef(TypedDict):
    status: str,
    id: str,
    endpoint: MlResourceDefinitionTypeDef,  # (1)
    endpointConfig: MlConfigDefinitionTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MlResourceDefinitionTypeDef](./type_defs.md#mlresourcedefinitiontypedef) 
2. See [:material-code-braces: MlConfigDefinitionTypeDef](./type_defs.md#mlconfigdefinitiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMLModelTrainingJobOutputTypeDef

```python
# GetMLModelTrainingJobOutputTypeDef definition

class GetMLModelTrainingJobOutputTypeDef(TypedDict):
    status: str,
    id: str,
    processingJob: MlResourceDefinitionTypeDef,  # (1)
    hpoJob: MlResourceDefinitionTypeDef,  # (1)
    modelTransformJob: MlResourceDefinitionTypeDef,  # (1)
    mlModels: List[MlConfigDefinitionTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: MlResourceDefinitionTypeDef](./type_defs.md#mlresourcedefinitiontypedef) 
2. See [:material-code-braces: MlResourceDefinitionTypeDef](./type_defs.md#mlresourcedefinitiontypedef) 
3. See [:material-code-braces: MlResourceDefinitionTypeDef](./type_defs.md#mlresourcedefinitiontypedef) 
4. See [:material-code-braces: MlConfigDefinitionTypeDef](./type_defs.md#mlconfigdefinitiontypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMLModelTransformJobOutputTypeDef

```python
# GetMLModelTransformJobOutputTypeDef definition

class GetMLModelTransformJobOutputTypeDef(TypedDict):
    status: str,
    id: str,
    baseProcessingJob: MlResourceDefinitionTypeDef,  # (1)
    remoteModelTransformJob: MlResourceDefinitionTypeDef,  # (1)
    models: List[MlConfigDefinitionTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: MlResourceDefinitionTypeDef](./type_defs.md#mlresourcedefinitiontypedef) 
2. See [:material-code-braces: MlResourceDefinitionTypeDef](./type_defs.md#mlresourcedefinitiontypedef) 
3. See [:material-code-braces: MlConfigDefinitionTypeDef](./type_defs.md#mlconfigdefinitiontypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLoaderJobsOutputTypeDef

```python
# ListLoaderJobsOutputTypeDef definition

class ListLoaderJobsOutputTypeDef(TypedDict):
    status: str,
    payload: LoaderIdResultTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoaderIdResultTypeDef](./type_defs.md#loaderidresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ManagePropertygraphStatisticsOutputTypeDef

```python
# ManagePropertygraphStatisticsOutputTypeDef definition

class ManagePropertygraphStatisticsOutputTypeDef(TypedDict):
    status: str,
    payload: RefreshStatisticsIdMapTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RefreshStatisticsIdMapTypeDef](./type_defs.md#refreshstatisticsidmaptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ManageSparqlStatisticsOutputTypeDef

```python
# ManageSparqlStatisticsOutputTypeDef definition

class ManageSparqlStatisticsOutputTypeDef(TypedDict):
    status: str,
    payload: RefreshStatisticsIdMapTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RefreshStatisticsIdMapTypeDef](./type_defs.md#refreshstatisticsidmaptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PropertygraphSummaryTypeDef

```python
# PropertygraphSummaryTypeDef definition

class PropertygraphSummaryTypeDef(TypedDict):
    numNodes: NotRequired[int],
    numEdges: NotRequired[int],
    numNodeLabels: NotRequired[int],
    numEdgeLabels: NotRequired[int],
    nodeLabels: NotRequired[List[str]],
    edgeLabels: NotRequired[List[str]],
    numNodeProperties: NotRequired[int],
    numEdgeProperties: NotRequired[int],
    nodeProperties: NotRequired[List[Dict[str, int]]],
    edgeProperties: NotRequired[List[Dict[str, int]]],
    totalNodePropertyValues: NotRequired[int],
    totalEdgePropertyValues: NotRequired[int],
    nodeStructures: NotRequired[List[NodeStructureTypeDef]],  # (1)
    edgeStructures: NotRequired[List[EdgeStructureTypeDef]],  # (2)
```

1. See [:material-code-braces: NodeStructureTypeDef](./type_defs.md#nodestructuretypedef) 
2. See [:material-code-braces: EdgeStructureTypeDef](./type_defs.md#edgestructuretypedef) 
## PropertygraphRecordTypeDef

```python
# PropertygraphRecordTypeDef definition

class PropertygraphRecordTypeDef(TypedDict):
    commitTimestampInMillis: int,
    eventId: Dict[str, str],
    data: PropertygraphDataTypeDef,  # (1)
    op: str,
    isLastOp: NotRequired[bool],
```

1. See [:material-code-braces: PropertygraphDataTypeDef](./type_defs.md#propertygraphdatatypedef) 
## RDFGraphSummaryTypeDef

```python
# RDFGraphSummaryTypeDef definition

class RDFGraphSummaryTypeDef(TypedDict):
    numDistinctSubjects: NotRequired[int],
    numDistinctPredicates: NotRequired[int],
    numQuads: NotRequired[int],
    numClasses: NotRequired[int],
    classes: NotRequired[List[str]],
    predicates: NotRequired[List[Dict[str, int]]],
    subjectStructures: NotRequired[List[SubjectStructureTypeDef]],  # (1)
```

1. See [:material-code-braces: SubjectStructureTypeDef](./type_defs.md#subjectstructuretypedef) 
## SparqlRecordTypeDef

```python
# SparqlRecordTypeDef definition

class SparqlRecordTypeDef(TypedDict):
    commitTimestampInMillis: int,
    eventId: Dict[str, str],
    data: SparqlDataTypeDef,  # (1)
    op: str,
    isLastOp: NotRequired[bool],
```

1. See [:material-code-braces: SparqlDataTypeDef](./type_defs.md#sparqldatatypedef) 
## StatisticsTypeDef

```python
# StatisticsTypeDef definition

class StatisticsTypeDef(TypedDict):
    autoCompute: NotRequired[bool],
    active: NotRequired[bool],
    statisticsId: NotRequired[str],
    date: NotRequired[datetime],
    note: NotRequired[str],
    signatureInfo: NotRequired[StatisticsSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: StatisticsSummaryTypeDef](./type_defs.md#statisticssummarytypedef) 
## ListGremlinQueriesOutputTypeDef

```python
# ListGremlinQueriesOutputTypeDef definition

class ListGremlinQueriesOutputTypeDef(TypedDict):
    acceptedQueryCount: int,
    runningQueryCount: int,
    queries: List[GremlinQueryStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GremlinQueryStatusTypeDef](./type_defs.md#gremlinquerystatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOpenCypherQueriesOutputTypeDef

```python
# ListOpenCypherQueriesOutputTypeDef definition

class ListOpenCypherQueriesOutputTypeDef(TypedDict):
    acceptedQueryCount: int,
    runningQueryCount: int,
    queries: List[GremlinQueryStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GremlinQueryStatusTypeDef](./type_defs.md#gremlinquerystatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PropertygraphSummaryValueMapTypeDef

```python
# PropertygraphSummaryValueMapTypeDef definition

class PropertygraphSummaryValueMapTypeDef(TypedDict):
    version: NotRequired[str],
    lastStatisticsComputationTime: NotRequired[datetime],
    graphSummary: NotRequired[PropertygraphSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: PropertygraphSummaryTypeDef](./type_defs.md#propertygraphsummarytypedef) 
## GetPropertygraphStreamOutputTypeDef

```python
# GetPropertygraphStreamOutputTypeDef definition

class GetPropertygraphStreamOutputTypeDef(TypedDict):
    lastEventId: Dict[str, str],
    lastTrxTimestampInMillis: int,
    format: str,
    records: List[PropertygraphRecordTypeDef],  # (1)
    totalRecords: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PropertygraphRecordTypeDef](./type_defs.md#propertygraphrecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RDFGraphSummaryValueMapTypeDef

```python
# RDFGraphSummaryValueMapTypeDef definition

class RDFGraphSummaryValueMapTypeDef(TypedDict):
    version: NotRequired[str],
    lastStatisticsComputationTime: NotRequired[datetime],
    graphSummary: NotRequired[RDFGraphSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: RDFGraphSummaryTypeDef](./type_defs.md#rdfgraphsummarytypedef) 
## GetSparqlStreamOutputTypeDef

```python
# GetSparqlStreamOutputTypeDef definition

class GetSparqlStreamOutputTypeDef(TypedDict):
    lastEventId: Dict[str, str],
    lastTrxTimestampInMillis: int,
    format: str,
    records: List[SparqlRecordTypeDef],  # (1)
    totalRecords: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SparqlRecordTypeDef](./type_defs.md#sparqlrecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPropertygraphStatisticsOutputTypeDef

```python
# GetPropertygraphStatisticsOutputTypeDef definition

class GetPropertygraphStatisticsOutputTypeDef(TypedDict):
    status: str,
    payload: StatisticsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StatisticsTypeDef](./type_defs.md#statisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSparqlStatisticsOutputTypeDef

```python
# GetSparqlStatisticsOutputTypeDef definition

class GetSparqlStatisticsOutputTypeDef(TypedDict):
    status: str,
    payload: StatisticsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StatisticsTypeDef](./type_defs.md#statisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPropertygraphSummaryOutputTypeDef

```python
# GetPropertygraphSummaryOutputTypeDef definition

class GetPropertygraphSummaryOutputTypeDef(TypedDict):
    statusCode: int,
    payload: PropertygraphSummaryValueMapTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PropertygraphSummaryValueMapTypeDef](./type_defs.md#propertygraphsummaryvaluemaptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRDFGraphSummaryOutputTypeDef

```python
# GetRDFGraphSummaryOutputTypeDef definition

class GetRDFGraphSummaryOutputTypeDef(TypedDict):
    statusCode: int,
    payload: RDFGraphSummaryValueMapTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RDFGraphSummaryValueMapTypeDef](./type_defs.md#rdfgraphsummaryvaluemaptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
