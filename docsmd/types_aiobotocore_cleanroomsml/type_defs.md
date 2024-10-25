# Type definitions

> [Index](../README.md) > [CleanRoomsML](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CleanRoomsML](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
    type annotations stubs module [types-aiobotocore-cleanroomsml](https://pypi.org/project/types-aiobotocore-cleanroomsml/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ColumnSchemaUnionTypeDef

```python
# ColumnSchemaUnionTypeDef definition

ColumnSchemaUnionTypeDef = Union[
    ColumnSchemaTypeDef,  # (1)
    ColumnSchemaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ColumnSchemaTypeDef](./type_defs.md#columnschematypedef) 
2. See [:material-code-braces: ColumnSchemaOutputTypeDef](./type_defs.md#columnschemaoutputtypedef) 

## ProtectedQuerySQLParametersUnionTypeDef

```python
# ProtectedQuerySQLParametersUnionTypeDef definition

ProtectedQuerySQLParametersUnionTypeDef = Union[
    ProtectedQuerySQLParametersTypeDef,  # (1)
    ProtectedQuerySQLParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) 
2. See [:material-code-braces: ProtectedQuerySQLParametersOutputTypeDef](./type_defs.md#protectedquerysqlparametersoutputtypedef) 

## DatasetInputConfigUnionTypeDef

```python
# DatasetInputConfigUnionTypeDef definition

DatasetInputConfigUnionTypeDef = Union[
    DatasetInputConfigTypeDef,  # (1)
    DatasetInputConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DatasetInputConfigTypeDef](./type_defs.md#datasetinputconfigtypedef) 
2. See [:material-code-braces: DatasetInputConfigOutputTypeDef](./type_defs.md#datasetinputconfigoutputtypedef) 

## DatasetUnionTypeDef

```python
# DatasetUnionTypeDef definition

DatasetUnionTypeDef = Union[
    DatasetTypeDef,  # (1)
    DatasetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: DatasetOutputTypeDef](./type_defs.md#datasetoutputtypedef) 



## S3ConfigMapTypeDef

```python
# S3ConfigMapTypeDef definition

class S3ConfigMapTypeDef(TypedDict):
    s3Uri: str,
```

## AudienceSizeTypeDef

```python
# AudienceSizeTypeDef definition

class AudienceSizeTypeDef(TypedDict):
    type: AudienceSizeTypeType,  # (1)
    value: int,
```

1. See [:material-code-brackets: AudienceSizeTypeType](./literals.md#audiencesizetypetype) 
## StatusDetailsTypeDef

```python
# StatusDetailsTypeDef definition

class StatusDetailsTypeDef(TypedDict):
    statusCode: NotRequired[str],
    message: NotRequired[str],
```

## ProtectedQuerySQLParametersOutputTypeDef

```python
# ProtectedQuerySQLParametersOutputTypeDef definition

class ProtectedQuerySQLParametersOutputTypeDef(TypedDict):
    queryString: NotRequired[str],
    analysisTemplateArn: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
```

## AudienceGenerationJobSummaryTypeDef

```python
# AudienceGenerationJobSummaryTypeDef definition

class AudienceGenerationJobSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    audienceGenerationJobArn: str,
    name: str,
    status: AudienceGenerationJobStatusType,  # (1)
    configuredAudienceModelArn: str,
    description: NotRequired[str],
    collaborationId: NotRequired[str],
    startedBy: NotRequired[str],
```

1. See [:material-code-brackets: AudienceGenerationJobStatusType](./literals.md#audiencegenerationjobstatustype) 
## AudienceModelSummaryTypeDef

```python
# AudienceModelSummaryTypeDef definition

class AudienceModelSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    audienceModelArn: str,
    name: str,
    trainingDatasetArn: str,
    status: AudienceModelStatusType,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-brackets: AudienceModelStatusType](./literals.md#audiencemodelstatustype) 
## AudienceSizeConfigOutputTypeDef

```python
# AudienceSizeConfigOutputTypeDef definition

class AudienceSizeConfigOutputTypeDef(TypedDict):
    audienceSizeType: AudienceSizeTypeType,  # (1)
    audienceSizeBins: List[int],
```

1. See [:material-code-brackets: AudienceSizeTypeType](./literals.md#audiencesizetypetype) 
## AudienceSizeConfigTypeDef

```python
# AudienceSizeConfigTypeDef definition

class AudienceSizeConfigTypeDef(TypedDict):
    audienceSizeType: AudienceSizeTypeType,  # (1)
    audienceSizeBins: Sequence[int],
```

1. See [:material-code-brackets: AudienceSizeTypeType](./literals.md#audiencesizetypetype) 
## ColumnSchemaOutputTypeDef

```python
# ColumnSchemaOutputTypeDef definition

class ColumnSchemaOutputTypeDef(TypedDict):
    columnName: str,
    columnTypes: List[ColumnTypeType],  # (1)
```

1. See [:material-code-brackets: ColumnTypeType](./literals.md#columntypetype) 
## ColumnSchemaTypeDef

```python
# ColumnSchemaTypeDef definition

class ColumnSchemaTypeDef(TypedDict):
    columnName: str,
    columnTypes: Sequence[ColumnTypeType],  # (1)
```

1. See [:material-code-brackets: ColumnTypeType](./literals.md#columntypetype) 
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

## GlueDataSourceTypeDef

```python
# GlueDataSourceTypeDef definition

class GlueDataSourceTypeDef(TypedDict):
    tableName: str,
    databaseName: str,
    catalogId: NotRequired[str],
```

## DeleteAudienceGenerationJobRequestRequestTypeDef

```python
# DeleteAudienceGenerationJobRequestRequestTypeDef definition

class DeleteAudienceGenerationJobRequestRequestTypeDef(TypedDict):
    audienceGenerationJobArn: str,
```

## DeleteAudienceModelRequestRequestTypeDef

```python
# DeleteAudienceModelRequestRequestTypeDef definition

class DeleteAudienceModelRequestRequestTypeDef(TypedDict):
    audienceModelArn: str,
```

## DeleteConfiguredAudienceModelPolicyRequestRequestTypeDef

```python
# DeleteConfiguredAudienceModelPolicyRequestRequestTypeDef definition

class DeleteConfiguredAudienceModelPolicyRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## DeleteConfiguredAudienceModelRequestRequestTypeDef

```python
# DeleteConfiguredAudienceModelRequestRequestTypeDef definition

class DeleteConfiguredAudienceModelRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## DeleteTrainingDatasetRequestRequestTypeDef

```python
# DeleteTrainingDatasetRequestRequestTypeDef definition

class DeleteTrainingDatasetRequestRequestTypeDef(TypedDict):
    trainingDatasetArn: str,
```

## GetAudienceGenerationJobRequestRequestTypeDef

```python
# GetAudienceGenerationJobRequestRequestTypeDef definition

class GetAudienceGenerationJobRequestRequestTypeDef(TypedDict):
    audienceGenerationJobArn: str,
```

## GetAudienceModelRequestRequestTypeDef

```python
# GetAudienceModelRequestRequestTypeDef definition

class GetAudienceModelRequestRequestTypeDef(TypedDict):
    audienceModelArn: str,
```

## GetConfiguredAudienceModelPolicyRequestRequestTypeDef

```python
# GetConfiguredAudienceModelPolicyRequestRequestTypeDef definition

class GetConfiguredAudienceModelPolicyRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## GetConfiguredAudienceModelRequestRequestTypeDef

```python
# GetConfiguredAudienceModelRequestRequestTypeDef definition

class GetConfiguredAudienceModelRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## GetTrainingDatasetRequestRequestTypeDef

```python
# GetTrainingDatasetRequestRequestTypeDef definition

class GetTrainingDatasetRequestRequestTypeDef(TypedDict):
    trainingDatasetArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAudienceExportJobsRequestRequestTypeDef

```python
# ListAudienceExportJobsRequestRequestTypeDef definition

class ListAudienceExportJobsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    audienceGenerationJobArn: NotRequired[str],
```

## ListAudienceGenerationJobsRequestRequestTypeDef

```python
# ListAudienceGenerationJobsRequestRequestTypeDef definition

class ListAudienceGenerationJobsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    configuredAudienceModelArn: NotRequired[str],
    collaborationId: NotRequired[str],
```

## ListAudienceModelsRequestRequestTypeDef

```python
# ListAudienceModelsRequestRequestTypeDef definition

class ListAudienceModelsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListConfiguredAudienceModelsRequestRequestTypeDef

```python
# ListConfiguredAudienceModelsRequestRequestTypeDef definition

class ListConfiguredAudienceModelsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTrainingDatasetsRequestRequestTypeDef

```python
# ListTrainingDatasetsRequestRequestTypeDef definition

class ListTrainingDatasetsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TrainingDatasetSummaryTypeDef

```python
# TrainingDatasetSummaryTypeDef definition

class TrainingDatasetSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    trainingDatasetArn: str,
    name: str,
    status: TrainingDatasetStatusType,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-brackets: TrainingDatasetStatusType](./literals.md#trainingdatasetstatustype) 
## ProtectedQuerySQLParametersTypeDef

```python
# ProtectedQuerySQLParametersTypeDef definition

class ProtectedQuerySQLParametersTypeDef(TypedDict):
    queryString: NotRequired[str],
    analysisTemplateArn: NotRequired[str],
    parameters: NotRequired[Mapping[str, str]],
```

## PutConfiguredAudienceModelPolicyRequestRequestTypeDef

```python
# PutConfiguredAudienceModelPolicyRequestRequestTypeDef definition

class PutConfiguredAudienceModelPolicyRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    configuredAudienceModelPolicy: str,
    previousPolicyHash: NotRequired[str],
    policyExistenceCondition: NotRequired[PolicyExistenceConditionType],  # (1)
```

1. See [:material-code-brackets: PolicyExistenceConditionType](./literals.md#policyexistenceconditiontype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AudienceDestinationTypeDef

```python
# AudienceDestinationTypeDef definition

class AudienceDestinationTypeDef(TypedDict):
    s3Destination: S3ConfigMapTypeDef,  # (1)
```

1. See [:material-code-braces: S3ConfigMapTypeDef](./type_defs.md#s3configmaptypedef) 
## RelevanceMetricTypeDef

```python
# RelevanceMetricTypeDef definition

class RelevanceMetricTypeDef(TypedDict):
    audienceSize: AudienceSizeTypeDef,  # (1)
    score: NotRequired[float],
```

1. See [:material-code-braces: AudienceSizeTypeDef](./type_defs.md#audiencesizetypedef) 
## StartAudienceExportJobRequestRequestTypeDef

```python
# StartAudienceExportJobRequestRequestTypeDef definition

class StartAudienceExportJobRequestRequestTypeDef(TypedDict):
    name: str,
    audienceGenerationJobArn: str,
    audienceSize: AudienceSizeTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: AudienceSizeTypeDef](./type_defs.md#audiencesizetypedef) 
## AudienceExportJobSummaryTypeDef

```python
# AudienceExportJobSummaryTypeDef definition

class AudienceExportJobSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    name: str,
    audienceGenerationJobArn: str,
    audienceSize: AudienceSizeTypeDef,  # (1)
    status: AudienceExportJobStatusType,  # (2)
    description: NotRequired[str],
    statusDetails: NotRequired[StatusDetailsTypeDef],  # (3)
    outputLocation: NotRequired[str],
```

1. See [:material-code-braces: AudienceSizeTypeDef](./type_defs.md#audiencesizetypedef) 
2. See [:material-code-brackets: AudienceExportJobStatusType](./literals.md#audienceexportjobstatustype) 
3. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
## AudienceGenerationJobDataSourceOutputTypeDef

```python
# AudienceGenerationJobDataSourceOutputTypeDef definition

class AudienceGenerationJobDataSourceOutputTypeDef(TypedDict):
    roleArn: str,
    dataSource: NotRequired[S3ConfigMapTypeDef],  # (1)
    sqlParameters: NotRequired[ProtectedQuerySQLParametersOutputTypeDef],  # (2)
```

1. See [:material-code-braces: S3ConfigMapTypeDef](./type_defs.md#s3configmaptypedef) 
2. See [:material-code-braces: ProtectedQuerySQLParametersOutputTypeDef](./type_defs.md#protectedquerysqlparametersoutputtypedef) 
## CreateAudienceModelRequestRequestTypeDef

```python
# CreateAudienceModelRequestRequestTypeDef definition

class CreateAudienceModelRequestRequestTypeDef(TypedDict):
    name: str,
    trainingDatasetArn: str,
    trainingDataStartTime: NotRequired[TimestampTypeDef],
    trainingDataEndTime: NotRequired[TimestampTypeDef],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    description: NotRequired[str],
```

## CreateAudienceModelResponseTypeDef

```python
# CreateAudienceModelResponseTypeDef definition

class CreateAudienceModelResponseTypeDef(TypedDict):
    audienceModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredAudienceModelResponseTypeDef

```python
# CreateConfiguredAudienceModelResponseTypeDef definition

class CreateConfiguredAudienceModelResponseTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrainingDatasetResponseTypeDef

```python
# CreateTrainingDatasetResponseTypeDef definition

class CreateTrainingDatasetResponseTypeDef(TypedDict):
    trainingDatasetArn: str,
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
## GetAudienceModelResponseTypeDef

```python
# GetAudienceModelResponseTypeDef definition

class GetAudienceModelResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    trainingDataStartTime: datetime,
    trainingDataEndTime: datetime,
    audienceModelArn: str,
    name: str,
    trainingDatasetArn: str,
    status: AudienceModelStatusType,  # (1)
    statusDetails: StatusDetailsTypeDef,  # (2)
    kmsKeyArn: str,
    tags: Dict[str, str],
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AudienceModelStatusType](./literals.md#audiencemodelstatustype) 
2. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredAudienceModelPolicyResponseTypeDef

```python
# GetConfiguredAudienceModelPolicyResponseTypeDef definition

class GetConfiguredAudienceModelPolicyResponseTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    configuredAudienceModelPolicy: str,
    policyHash: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAudienceGenerationJobsResponseTypeDef

```python
# ListAudienceGenerationJobsResponseTypeDef definition

class ListAudienceGenerationJobsResponseTypeDef(TypedDict):
    audienceGenerationJobs: List[AudienceGenerationJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AudienceGenerationJobSummaryTypeDef](./type_defs.md#audiencegenerationjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAudienceModelsResponseTypeDef

```python
# ListAudienceModelsResponseTypeDef definition

class ListAudienceModelsResponseTypeDef(TypedDict):
    audienceModels: List[AudienceModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AudienceModelSummaryTypeDef](./type_defs.md#audiencemodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutConfiguredAudienceModelPolicyResponseTypeDef

```python
# PutConfiguredAudienceModelPolicyResponseTypeDef definition

class PutConfiguredAudienceModelPolicyResponseTypeDef(TypedDict):
    configuredAudienceModelPolicy: str,
    policyHash: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAudienceGenerationJobResponseTypeDef

```python
# StartAudienceGenerationJobResponseTypeDef definition

class StartAudienceGenerationJobResponseTypeDef(TypedDict):
    audienceGenerationJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredAudienceModelResponseTypeDef

```python
# UpdateConfiguredAudienceModelResponseTypeDef definition

class UpdateConfiguredAudienceModelResponseTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    glueDataSource: GlueDataSourceTypeDef,  # (1)
```

1. See [:material-code-braces: GlueDataSourceTypeDef](./type_defs.md#gluedatasourcetypedef) 
## ListAudienceExportJobsRequestListAudienceExportJobsPaginateTypeDef

```python
# ListAudienceExportJobsRequestListAudienceExportJobsPaginateTypeDef definition

class ListAudienceExportJobsRequestListAudienceExportJobsPaginateTypeDef(TypedDict):
    audienceGenerationJobArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAudienceGenerationJobsRequestListAudienceGenerationJobsPaginateTypeDef

```python
# ListAudienceGenerationJobsRequestListAudienceGenerationJobsPaginateTypeDef definition

class ListAudienceGenerationJobsRequestListAudienceGenerationJobsPaginateTypeDef(TypedDict):
    configuredAudienceModelArn: NotRequired[str],
    collaborationId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAudienceModelsRequestListAudienceModelsPaginateTypeDef

```python
# ListAudienceModelsRequestListAudienceModelsPaginateTypeDef definition

class ListAudienceModelsRequestListAudienceModelsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredAudienceModelsRequestListConfiguredAudienceModelsPaginateTypeDef

```python
# ListConfiguredAudienceModelsRequestListConfiguredAudienceModelsPaginateTypeDef definition

class ListConfiguredAudienceModelsRequestListConfiguredAudienceModelsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrainingDatasetsRequestListTrainingDatasetsPaginateTypeDef

```python
# ListTrainingDatasetsRequestListTrainingDatasetsPaginateTypeDef definition

class ListTrainingDatasetsRequestListTrainingDatasetsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrainingDatasetsResponseTypeDef

```python
# ListTrainingDatasetsResponseTypeDef definition

class ListTrainingDatasetsResponseTypeDef(TypedDict):
    trainingDatasets: List[TrainingDatasetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TrainingDatasetSummaryTypeDef](./type_defs.md#trainingdatasetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfiguredAudienceModelOutputConfigTypeDef

```python
# ConfiguredAudienceModelOutputConfigTypeDef definition

class ConfiguredAudienceModelOutputConfigTypeDef(TypedDict):
    destination: AudienceDestinationTypeDef,  # (1)
    roleArn: str,
```

1. See [:material-code-braces: AudienceDestinationTypeDef](./type_defs.md#audiencedestinationtypedef) 
## AudienceQualityMetricsTypeDef

```python
# AudienceQualityMetricsTypeDef definition

class AudienceQualityMetricsTypeDef(TypedDict):
    relevanceMetrics: List[RelevanceMetricTypeDef],  # (1)
    recallMetric: NotRequired[float],
```

1. See [:material-code-braces: RelevanceMetricTypeDef](./type_defs.md#relevancemetrictypedef) 
## ListAudienceExportJobsResponseTypeDef

```python
# ListAudienceExportJobsResponseTypeDef definition

class ListAudienceExportJobsResponseTypeDef(TypedDict):
    audienceExportJobs: List[AudienceExportJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AudienceExportJobSummaryTypeDef](./type_defs.md#audienceexportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetInputConfigOutputTypeDef

```python
# DatasetInputConfigOutputTypeDef definition

class DatasetInputConfigOutputTypeDef(TypedDict):
    schema: List[ColumnSchemaOutputTypeDef],  # (1)
    dataSource: DataSourceTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnSchemaOutputTypeDef](./type_defs.md#columnschemaoutputtypedef) 
2. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## DatasetInputConfigTypeDef

```python
# DatasetInputConfigTypeDef definition

class DatasetInputConfigTypeDef(TypedDict):
    schema: Sequence[ColumnSchemaUnionTypeDef],  # (1)
    dataSource: DataSourceTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnSchemaTypeDef](./type_defs.md#columnschematypedef) [:material-code-braces: ColumnSchemaOutputTypeDef](./type_defs.md#columnschemaoutputtypedef) 
2. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## AudienceGenerationJobDataSourceTypeDef

```python
# AudienceGenerationJobDataSourceTypeDef definition

class AudienceGenerationJobDataSourceTypeDef(TypedDict):
    roleArn: str,
    dataSource: NotRequired[S3ConfigMapTypeDef],  # (1)
    sqlParameters: NotRequired[ProtectedQuerySQLParametersUnionTypeDef],  # (2)
```

1. See [:material-code-braces: S3ConfigMapTypeDef](./type_defs.md#s3configmaptypedef) 
2. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) [:material-code-braces: ProtectedQuerySQLParametersOutputTypeDef](./type_defs.md#protectedquerysqlparametersoutputtypedef) 
## ConfiguredAudienceModelSummaryTypeDef

```python
# ConfiguredAudienceModelSummaryTypeDef definition

class ConfiguredAudienceModelSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    name: str,
    audienceModelArn: str,
    outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,  # (1)
    configuredAudienceModelArn: str,
    status: ConfiguredAudienceModelStatusType,  # (2)
    description: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: ConfiguredAudienceModelStatusType](./literals.md#configuredaudiencemodelstatustype) 
## CreateConfiguredAudienceModelRequestRequestTypeDef

```python
# CreateConfiguredAudienceModelRequestRequestTypeDef definition

class CreateConfiguredAudienceModelRequestRequestTypeDef(TypedDict):
    name: str,
    audienceModelArn: str,
    outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,  # (1)
    sharedAudienceMetrics: Sequence[SharedAudienceMetricsType],  # (2)
    description: NotRequired[str],
    minMatchingSeedSize: NotRequired[int],
    audienceSizeConfig: NotRequired[AudienceSizeConfigTypeDef],  # (3)
    tags: NotRequired[Mapping[str, str]],
    childResourceTagOnCreatePolicy: NotRequired[TagOnCreatePolicyType],  # (4)
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype) 
3. See [:material-code-braces: AudienceSizeConfigTypeDef](./type_defs.md#audiencesizeconfigtypedef) 
4. See [:material-code-brackets: TagOnCreatePolicyType](./literals.md#tagoncreatepolicytype) 
## GetConfiguredAudienceModelResponseTypeDef

```python
# GetConfiguredAudienceModelResponseTypeDef definition

class GetConfiguredAudienceModelResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    configuredAudienceModelArn: str,
    name: str,
    audienceModelArn: str,
    outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,  # (1)
    description: str,
    status: ConfiguredAudienceModelStatusType,  # (2)
    sharedAudienceMetrics: List[SharedAudienceMetricsType],  # (3)
    minMatchingSeedSize: int,
    audienceSizeConfig: AudienceSizeConfigOutputTypeDef,  # (4)
    tags: Dict[str, str],
    childResourceTagOnCreatePolicy: TagOnCreatePolicyType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: ConfiguredAudienceModelStatusType](./literals.md#configuredaudiencemodelstatustype) 
3. See [:material-code-brackets: SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype) 
4. See [:material-code-braces: AudienceSizeConfigOutputTypeDef](./type_defs.md#audiencesizeconfigoutputtypedef) 
5. See [:material-code-brackets: TagOnCreatePolicyType](./literals.md#tagoncreatepolicytype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredAudienceModelRequestRequestTypeDef

```python
# UpdateConfiguredAudienceModelRequestRequestTypeDef definition

class UpdateConfiguredAudienceModelRequestRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    outputConfig: NotRequired[ConfiguredAudienceModelOutputConfigTypeDef],  # (1)
    audienceModelArn: NotRequired[str],
    sharedAudienceMetrics: NotRequired[Sequence[SharedAudienceMetricsType]],  # (2)
    minMatchingSeedSize: NotRequired[int],
    audienceSizeConfig: NotRequired[AudienceSizeConfigTypeDef],  # (3)
    description: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype) 
3. See [:material-code-braces: AudienceSizeConfigTypeDef](./type_defs.md#audiencesizeconfigtypedef) 
## GetAudienceGenerationJobResponseTypeDef

```python
# GetAudienceGenerationJobResponseTypeDef definition

class GetAudienceGenerationJobResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    audienceGenerationJobArn: str,
    name: str,
    description: str,
    status: AudienceGenerationJobStatusType,  # (1)
    statusDetails: StatusDetailsTypeDef,  # (2)
    configuredAudienceModelArn: str,
    seedAudience: AudienceGenerationJobDataSourceOutputTypeDef,  # (3)
    includeSeedInOutput: bool,
    collaborationId: str,
    metrics: AudienceQualityMetricsTypeDef,  # (4)
    startedBy: str,
    tags: Dict[str, str],
    protectedQueryIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: AudienceGenerationJobStatusType](./literals.md#audiencegenerationjobstatustype) 
2. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
3. See [:material-code-braces: AudienceGenerationJobDataSourceOutputTypeDef](./type_defs.md#audiencegenerationjobdatasourceoutputtypedef) 
4. See [:material-code-braces: AudienceQualityMetricsTypeDef](./type_defs.md#audiencequalitymetricstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetOutputTypeDef

```python
# DatasetOutputTypeDef definition

class DatasetOutputTypeDef(TypedDict):
    type: DatasetTypeType,  # (1)
    inputConfig: DatasetInputConfigOutputTypeDef,  # (2)
```

1. See [:material-code-brackets: DatasetTypeType](./literals.md#datasettypetype) 
2. See [:material-code-braces: DatasetInputConfigOutputTypeDef](./type_defs.md#datasetinputconfigoutputtypedef) 
## StartAudienceGenerationJobRequestRequestTypeDef

```python
# StartAudienceGenerationJobRequestRequestTypeDef definition

class StartAudienceGenerationJobRequestRequestTypeDef(TypedDict):
    name: str,
    configuredAudienceModelArn: str,
    seedAudience: AudienceGenerationJobDataSourceTypeDef,  # (1)
    includeSeedInOutput: NotRequired[bool],
    collaborationId: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AudienceGenerationJobDataSourceTypeDef](./type_defs.md#audiencegenerationjobdatasourcetypedef) 
## ListConfiguredAudienceModelsResponseTypeDef

```python
# ListConfiguredAudienceModelsResponseTypeDef definition

class ListConfiguredAudienceModelsResponseTypeDef(TypedDict):
    configuredAudienceModels: List[ConfiguredAudienceModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredAudienceModelSummaryTypeDef](./type_defs.md#configuredaudiencemodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrainingDatasetResponseTypeDef

```python
# GetTrainingDatasetResponseTypeDef definition

class GetTrainingDatasetResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    trainingDatasetArn: str,
    name: str,
    trainingData: List[DatasetOutputTypeDef],  # (1)
    status: TrainingDatasetStatusType,  # (2)
    roleArn: str,
    tags: Dict[str, str],
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DatasetOutputTypeDef](./type_defs.md#datasetoutputtypedef) 
2. See [:material-code-brackets: TrainingDatasetStatusType](./literals.md#trainingdatasetstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetTypeDef

```python
# DatasetTypeDef definition

class DatasetTypeDef(TypedDict):
    type: DatasetTypeType,  # (1)
    inputConfig: DatasetInputConfigUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: DatasetTypeType](./literals.md#datasettypetype) 
2. See [:material-code-braces: DatasetInputConfigTypeDef](./type_defs.md#datasetinputconfigtypedef) [:material-code-braces: DatasetInputConfigOutputTypeDef](./type_defs.md#datasetinputconfigoutputtypedef) 
## CreateTrainingDatasetRequestRequestTypeDef

```python
# CreateTrainingDatasetRequestRequestTypeDef definition

class CreateTrainingDatasetRequestRequestTypeDef(TypedDict):
    name: str,
    roleArn: str,
    trainingData: Sequence[DatasetUnionTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
    description: NotRequired[str],
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) [:material-code-braces: DatasetOutputTypeDef](./type_defs.md#datasetoutputtypedef) 
