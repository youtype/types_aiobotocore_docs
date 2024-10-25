# Type definitions

> [Index](../README.md) > [LookoutforVision](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LookoutforVision](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
    type annotations stubs module [types-aiobotocore-lookoutvision](https://pypi.org/project/types-aiobotocore-lookoutvision/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## GreengrassConfigurationUnionTypeDef

```python
# GreengrassConfigurationUnionTypeDef definition

GreengrassConfigurationUnionTypeDef = Union[
    GreengrassConfigurationTypeDef,  # (1)
    GreengrassConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GreengrassConfigurationTypeDef](./type_defs.md#greengrassconfigurationtypedef) 
2. See [:material-code-braces: GreengrassConfigurationOutputTypeDef](./type_defs.md#greengrassconfigurationoutputtypedef) 



## PixelAnomalyTypeDef

```python
# PixelAnomalyTypeDef definition

class PixelAnomalyTypeDef(TypedDict):
    TotalPercentageArea: NotRequired[float],
    Color: NotRequired[str],
```

## DatasetMetadataTypeDef

```python
# DatasetMetadataTypeDef definition

class DatasetMetadataTypeDef(TypedDict):
    DatasetType: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
    Status: NotRequired[DatasetStatusType],  # (1)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
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

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateProjectRequestRequestTypeDef

```python
# CreateProjectRequestRequestTypeDef definition

class CreateProjectRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    ClientToken: NotRequired[str],
```

## ProjectMetadataTypeDef

```python
# ProjectMetadataTypeDef definition

class ProjectMetadataTypeDef(TypedDict):
    ProjectArn: NotRequired[str],
    ProjectName: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
```

## DatasetImageStatsTypeDef

```python
# DatasetImageStatsTypeDef definition

class DatasetImageStatsTypeDef(TypedDict):
    Total: NotRequired[int],
    Labeled: NotRequired[int],
    Normal: NotRequired[int],
    Anomaly: NotRequired[int],
```

## InputS3ObjectTypeDef

```python
# InputS3ObjectTypeDef definition

class InputS3ObjectTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    VersionId: NotRequired[str],
```

## DeleteDatasetRequestRequestTypeDef

```python
# DeleteDatasetRequestRequestTypeDef definition

class DeleteDatasetRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    DatasetType: str,
    ClientToken: NotRequired[str],
```

## DeleteModelRequestRequestTypeDef

```python
# DeleteModelRequestRequestTypeDef definition

class DeleteModelRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
    ClientToken: NotRequired[str],
```

## DeleteProjectRequestRequestTypeDef

```python
# DeleteProjectRequestRequestTypeDef definition

class DeleteProjectRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    ClientToken: NotRequired[str],
```

## DescribeDatasetRequestRequestTypeDef

```python
# DescribeDatasetRequestRequestTypeDef definition

class DescribeDatasetRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    DatasetType: str,
```

## DescribeModelPackagingJobRequestRequestTypeDef

```python
# DescribeModelPackagingJobRequestRequestTypeDef definition

class DescribeModelPackagingJobRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    JobName: str,
```

## DescribeModelRequestRequestTypeDef

```python
# DescribeModelRequestRequestTypeDef definition

class DescribeModelRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
```

## DescribeProjectRequestRequestTypeDef

```python
# DescribeProjectRequestRequestTypeDef definition

class DescribeProjectRequestRequestTypeDef(TypedDict):
    ProjectName: str,
```

## ImageSourceTypeDef

```python
# ImageSourceTypeDef definition

class ImageSourceTypeDef(TypedDict):
    Type: NotRequired[str],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    Bucket: str,
    Prefix: NotRequired[str],
```

## TargetPlatformTypeDef

```python
# TargetPlatformTypeDef definition

class TargetPlatformTypeDef(TypedDict):
    Os: TargetPlatformOsType,  # (1)
    Arch: TargetPlatformArchType,  # (2)
    Accelerator: NotRequired[TargetPlatformAcceleratorType],  # (3)
```

1. See [:material-code-brackets: TargetPlatformOsType](./literals.md#targetplatformostype) 
2. See [:material-code-brackets: TargetPlatformArchType](./literals.md#targetplatformarchtype) 
3. See [:material-code-brackets: TargetPlatformAcceleratorType](./literals.md#targetplatformacceleratortype) 
## GreengrassOutputDetailsTypeDef

```python
# GreengrassOutputDetailsTypeDef definition

class GreengrassOutputDetailsTypeDef(TypedDict):
    ComponentVersionArn: NotRequired[str],
    ComponentName: NotRequired[str],
    ComponentVersion: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListModelPackagingJobsRequestRequestTypeDef

```python
# ListModelPackagingJobsRequestRequestTypeDef definition

class ListModelPackagingJobsRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ModelPackagingJobMetadataTypeDef

```python
# ModelPackagingJobMetadataTypeDef definition

class ModelPackagingJobMetadataTypeDef(TypedDict):
    JobName: NotRequired[str],
    ProjectName: NotRequired[str],
    ModelVersion: NotRequired[str],
    ModelPackagingJobDescription: NotRequired[str],
    ModelPackagingMethod: NotRequired[str],
    Status: NotRequired[ModelPackagingJobStatusType],  # (1)
    StatusMessage: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ModelPackagingJobStatusType](./literals.md#modelpackagingjobstatustype) 
## ListModelsRequestRequestTypeDef

```python
# ListModelsRequestRequestTypeDef definition

class ListModelsRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListProjectsRequestRequestTypeDef

```python
# ListProjectsRequestRequestTypeDef definition

class ListProjectsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ModelPerformanceTypeDef

```python
# ModelPerformanceTypeDef definition

class ModelPerformanceTypeDef(TypedDict):
    F1Score: NotRequired[float],
    Recall: NotRequired[float],
    Precision: NotRequired[float],
```

## OutputS3ObjectTypeDef

```python
# OutputS3ObjectTypeDef definition

class OutputS3ObjectTypeDef(TypedDict):
    Bucket: str,
    Key: str,
```

## StartModelRequestRequestTypeDef

```python
# StartModelRequestRequestTypeDef definition

class StartModelRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
    MinInferenceUnits: int,
    ClientToken: NotRequired[str],
    MaxInferenceUnits: NotRequired[int],
```

## StopModelRequestRequestTypeDef

```python
# StopModelRequestRequestTypeDef definition

class StopModelRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
    ClientToken: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## AnomalyTypeDef

```python
# AnomalyTypeDef definition

class AnomalyTypeDef(TypedDict):
    Name: NotRequired[str],
    PixelAnomaly: NotRequired[PixelAnomalyTypeDef],  # (1)
```

1. See [:material-code-braces: PixelAnomalyTypeDef](./type_defs.md#pixelanomalytypedef) 
## DetectAnomaliesRequestRequestTypeDef

```python
# DetectAnomaliesRequestRequestTypeDef definition

class DetectAnomaliesRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
    Body: BlobTypeDef,
    ContentType: str,
```

## UpdateDatasetEntriesRequestRequestTypeDef

```python
# UpdateDatasetEntriesRequestRequestTypeDef definition

class UpdateDatasetEntriesRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    DatasetType: str,
    Changes: BlobTypeDef,
    ClientToken: NotRequired[str],
```

## ProjectDescriptionTypeDef

```python
# ProjectDescriptionTypeDef definition

class ProjectDescriptionTypeDef(TypedDict):
    ProjectArn: NotRequired[str],
    ProjectName: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
    Datasets: NotRequired[List[DatasetMetadataTypeDef]],  # (1)
```

1. See [:material-code-braces: DatasetMetadataTypeDef](./type_defs.md#datasetmetadatatypedef) 
## CreateDatasetResponseTypeDef

```python
# CreateDatasetResponseTypeDef definition

class CreateDatasetResponseTypeDef(TypedDict):
    DatasetMetadata: DatasetMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetMetadataTypeDef](./type_defs.md#datasetmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteModelResponseTypeDef

```python
# DeleteModelResponseTypeDef definition

class DeleteModelResponseTypeDef(TypedDict):
    ModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProjectResponseTypeDef

```python
# DeleteProjectResponseTypeDef definition

class DeleteProjectResponseTypeDef(TypedDict):
    ProjectArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatasetEntriesResponseTypeDef

```python
# ListDatasetEntriesResponseTypeDef definition

class ListDatasetEntriesResponseTypeDef(TypedDict):
    DatasetEntries: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartModelPackagingJobResponseTypeDef

```python
# StartModelPackagingJobResponseTypeDef definition

class StartModelPackagingJobResponseTypeDef(TypedDict):
    JobName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartModelResponseTypeDef

```python
# StartModelResponseTypeDef definition

class StartModelResponseTypeDef(TypedDict):
    Status: ModelHostingStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ModelHostingStatusType](./literals.md#modelhostingstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopModelResponseTypeDef

```python
# StopModelResponseTypeDef definition

class StopModelResponseTypeDef(TypedDict):
    Status: ModelHostingStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ModelHostingStatusType](./literals.md#modelhostingstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDatasetEntriesResponseTypeDef

```python
# UpdateDatasetEntriesResponseTypeDef definition

class UpdateDatasetEntriesResponseTypeDef(TypedDict):
    Status: DatasetStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateProjectResponseTypeDef

```python
# CreateProjectResponseTypeDef definition

class CreateProjectResponseTypeDef(TypedDict):
    ProjectMetadata: ProjectMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectMetadataTypeDef](./type_defs.md#projectmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectsResponseTypeDef

```python
# ListProjectsResponseTypeDef definition

class ListProjectsResponseTypeDef(TypedDict):
    Projects: List[ProjectMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectMetadataTypeDef](./type_defs.md#projectmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetDescriptionTypeDef

```python
# DatasetDescriptionTypeDef definition

class DatasetDescriptionTypeDef(TypedDict):
    ProjectName: NotRequired[str],
    DatasetType: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
    Status: NotRequired[DatasetStatusType],  # (1)
    StatusMessage: NotRequired[str],
    ImageStats: NotRequired[DatasetImageStatsTypeDef],  # (2)
```

1. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
2. See [:material-code-braces: DatasetImageStatsTypeDef](./type_defs.md#datasetimagestatstypedef) 
## DatasetGroundTruthManifestTypeDef

```python
# DatasetGroundTruthManifestTypeDef definition

class DatasetGroundTruthManifestTypeDef(TypedDict):
    S3Object: NotRequired[InputS3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: InputS3ObjectTypeDef](./type_defs.md#inputs3objecttypedef) 
## OutputConfigTypeDef

```python
# OutputConfigTypeDef definition

class OutputConfigTypeDef(TypedDict):
    S3Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## GreengrassConfigurationOutputTypeDef

```python
# GreengrassConfigurationOutputTypeDef definition

class GreengrassConfigurationOutputTypeDef(TypedDict):
    S3OutputLocation: S3LocationTypeDef,  # (3)
    ComponentName: str,
    CompilerOptions: NotRequired[str],
    TargetDevice: NotRequired[TargetDeviceType],  # (1)
    TargetPlatform: NotRequired[TargetPlatformTypeDef],  # (2)
    ComponentVersion: NotRequired[str],
    ComponentDescription: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: TargetDeviceType](./literals.md#targetdevicetype) 
2. See [:material-code-braces: TargetPlatformTypeDef](./type_defs.md#targetplatformtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GreengrassConfigurationTypeDef

```python
# GreengrassConfigurationTypeDef definition

class GreengrassConfigurationTypeDef(TypedDict):
    S3OutputLocation: S3LocationTypeDef,  # (3)
    ComponentName: str,
    CompilerOptions: NotRequired[str],
    TargetDevice: NotRequired[TargetDeviceType],  # (1)
    TargetPlatform: NotRequired[TargetPlatformTypeDef],  # (2)
    ComponentVersion: NotRequired[str],
    ComponentDescription: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: TargetDeviceType](./literals.md#targetdevicetype) 
2. See [:material-code-braces: TargetPlatformTypeDef](./type_defs.md#targetplatformtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ModelPackagingOutputDetailsTypeDef

```python
# ModelPackagingOutputDetailsTypeDef definition

class ModelPackagingOutputDetailsTypeDef(TypedDict):
    Greengrass: NotRequired[GreengrassOutputDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: GreengrassOutputDetailsTypeDef](./type_defs.md#greengrassoutputdetailstypedef) 
## ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef

```python
# ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef definition

class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(TypedDict):
    ProjectName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelsRequestListModelsPaginateTypeDef

```python
# ListModelsRequestListModelsPaginateTypeDef definition

class ListModelsRequestListModelsPaginateTypeDef(TypedDict):
    ProjectName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestListProjectsPaginateTypeDef

```python
# ListProjectsRequestListProjectsPaginateTypeDef definition

class ListProjectsRequestListProjectsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef

```python
# ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef definition

class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(TypedDict):
    ProjectName: str,
    DatasetType: str,
    Labeled: NotRequired[bool],
    AnomalyClass: NotRequired[str],
    BeforeCreationDate: NotRequired[TimestampTypeDef],
    AfterCreationDate: NotRequired[TimestampTypeDef],
    SourceRefContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetEntriesRequestRequestTypeDef

```python
# ListDatasetEntriesRequestRequestTypeDef definition

class ListDatasetEntriesRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    DatasetType: str,
    Labeled: NotRequired[bool],
    AnomalyClass: NotRequired[str],
    BeforeCreationDate: NotRequired[TimestampTypeDef],
    AfterCreationDate: NotRequired[TimestampTypeDef],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SourceRefContains: NotRequired[str],
```

## ListModelPackagingJobsResponseTypeDef

```python
# ListModelPackagingJobsResponseTypeDef definition

class ListModelPackagingJobsResponseTypeDef(TypedDict):
    ModelPackagingJobs: List[ModelPackagingJobMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ModelPackagingJobMetadataTypeDef](./type_defs.md#modelpackagingjobmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelMetadataTypeDef

```python
# ModelMetadataTypeDef definition

class ModelMetadataTypeDef(TypedDict):
    CreationTimestamp: NotRequired[datetime],
    ModelVersion: NotRequired[str],
    ModelArn: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[ModelStatusType],  # (1)
    StatusMessage: NotRequired[str],
    Performance: NotRequired[ModelPerformanceTypeDef],  # (2)
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
2. See [:material-code-braces: ModelPerformanceTypeDef](./type_defs.md#modelperformancetypedef) 
## DetectAnomalyResultTypeDef

```python
# DetectAnomalyResultTypeDef definition

class DetectAnomalyResultTypeDef(TypedDict):
    Source: NotRequired[ImageSourceTypeDef],  # (1)
    IsAnomalous: NotRequired[bool],
    Confidence: NotRequired[float],
    Anomalies: NotRequired[List[AnomalyTypeDef]],  # (2)
    AnomalyMask: NotRequired[bytes],
```

1. See [:material-code-braces: ImageSourceTypeDef](./type_defs.md#imagesourcetypedef) 
2. See [:material-code-braces: AnomalyTypeDef](./type_defs.md#anomalytypedef) 
## DescribeProjectResponseTypeDef

```python
# DescribeProjectResponseTypeDef definition

class DescribeProjectResponseTypeDef(TypedDict):
    ProjectDescription: ProjectDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectDescriptionTypeDef](./type_defs.md#projectdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDatasetResponseTypeDef

```python
# DescribeDatasetResponseTypeDef definition

class DescribeDatasetResponseTypeDef(TypedDict):
    DatasetDescription: DatasetDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetDescriptionTypeDef](./type_defs.md#datasetdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetSourceTypeDef

```python
# DatasetSourceTypeDef definition

class DatasetSourceTypeDef(TypedDict):
    GroundTruthManifest: NotRequired[DatasetGroundTruthManifestTypeDef],  # (1)
```

1. See [:material-code-braces: DatasetGroundTruthManifestTypeDef](./type_defs.md#datasetgroundtruthmanifesttypedef) 
## CreateModelRequestRequestTypeDef

```python
# CreateModelRequestRequestTypeDef definition

class CreateModelRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    OutputConfig: OutputConfigTypeDef,  # (1)
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ModelDescriptionTypeDef

```python
# ModelDescriptionTypeDef definition

class ModelDescriptionTypeDef(TypedDict):
    ModelVersion: NotRequired[str],
    ModelArn: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
    Description: NotRequired[str],
    Status: NotRequired[ModelStatusType],  # (1)
    StatusMessage: NotRequired[str],
    Performance: NotRequired[ModelPerformanceTypeDef],  # (2)
    OutputConfig: NotRequired[OutputConfigTypeDef],  # (3)
    EvaluationManifest: NotRequired[OutputS3ObjectTypeDef],  # (4)
    EvaluationResult: NotRequired[OutputS3ObjectTypeDef],  # (4)
    EvaluationEndTimestamp: NotRequired[datetime],
    KmsKeyId: NotRequired[str],
    MinInferenceUnits: NotRequired[int],
    MaxInferenceUnits: NotRequired[int],
```

1. See [:material-code-brackets: ModelStatusType](./literals.md#modelstatustype) 
2. See [:material-code-braces: ModelPerformanceTypeDef](./type_defs.md#modelperformancetypedef) 
3. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
4. See [:material-code-braces: OutputS3ObjectTypeDef](./type_defs.md#outputs3objecttypedef) 
5. See [:material-code-braces: OutputS3ObjectTypeDef](./type_defs.md#outputs3objecttypedef) 
## ModelPackagingConfigurationOutputTypeDef

```python
# ModelPackagingConfigurationOutputTypeDef definition

class ModelPackagingConfigurationOutputTypeDef(TypedDict):
    Greengrass: GreengrassConfigurationOutputTypeDef,  # (1)
```

1. See [:material-code-braces: GreengrassConfigurationOutputTypeDef](./type_defs.md#greengrassconfigurationoutputtypedef) 
## CreateModelResponseTypeDef

```python
# CreateModelResponseTypeDef definition

class CreateModelResponseTypeDef(TypedDict):
    ModelMetadata: ModelMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelMetadataTypeDef](./type_defs.md#modelmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelsResponseTypeDef

```python
# ListModelsResponseTypeDef definition

class ListModelsResponseTypeDef(TypedDict):
    Models: List[ModelMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ModelMetadataTypeDef](./type_defs.md#modelmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DetectAnomaliesResponseTypeDef

```python
# DetectAnomaliesResponseTypeDef definition

class DetectAnomaliesResponseTypeDef(TypedDict):
    DetectAnomalyResult: DetectAnomalyResultTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectAnomalyResultTypeDef](./type_defs.md#detectanomalyresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetRequestRequestTypeDef

```python
# CreateDatasetRequestRequestTypeDef definition

class CreateDatasetRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    DatasetType: str,
    DatasetSource: NotRequired[DatasetSourceTypeDef],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef) 
## DescribeModelResponseTypeDef

```python
# DescribeModelResponseTypeDef definition

class DescribeModelResponseTypeDef(TypedDict):
    ModelDescription: ModelDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelDescriptionTypeDef](./type_defs.md#modeldescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelPackagingDescriptionTypeDef

```python
# ModelPackagingDescriptionTypeDef definition

class ModelPackagingDescriptionTypeDef(TypedDict):
    JobName: NotRequired[str],
    ProjectName: NotRequired[str],
    ModelVersion: NotRequired[str],
    ModelPackagingConfiguration: NotRequired[ModelPackagingConfigurationOutputTypeDef],  # (1)
    ModelPackagingJobDescription: NotRequired[str],
    ModelPackagingMethod: NotRequired[str],
    ModelPackagingOutputDetails: NotRequired[ModelPackagingOutputDetailsTypeDef],  # (2)
    Status: NotRequired[ModelPackagingJobStatusType],  # (3)
    StatusMessage: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
    LastUpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: ModelPackagingConfigurationOutputTypeDef](./type_defs.md#modelpackagingconfigurationoutputtypedef) 
2. See [:material-code-braces: ModelPackagingOutputDetailsTypeDef](./type_defs.md#modelpackagingoutputdetailstypedef) 
3. See [:material-code-brackets: ModelPackagingJobStatusType](./literals.md#modelpackagingjobstatustype) 
## ModelPackagingConfigurationTypeDef

```python
# ModelPackagingConfigurationTypeDef definition

class ModelPackagingConfigurationTypeDef(TypedDict):
    Greengrass: GreengrassConfigurationUnionTypeDef,  # (1)
```

1. See [:material-code-braces: GreengrassConfigurationTypeDef](./type_defs.md#greengrassconfigurationtypedef) [:material-code-braces: GreengrassConfigurationOutputTypeDef](./type_defs.md#greengrassconfigurationoutputtypedef) 
## DescribeModelPackagingJobResponseTypeDef

```python
# DescribeModelPackagingJobResponseTypeDef definition

class DescribeModelPackagingJobResponseTypeDef(TypedDict):
    ModelPackagingDescription: ModelPackagingDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelPackagingDescriptionTypeDef](./type_defs.md#modelpackagingdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartModelPackagingJobRequestRequestTypeDef

```python
# StartModelPackagingJobRequestRequestTypeDef definition

class StartModelPackagingJobRequestRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
    Configuration: ModelPackagingConfigurationTypeDef,  # (1)
    JobName: NotRequired[str],
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: ModelPackagingConfigurationTypeDef](./type_defs.md#modelpackagingconfigurationtypedef) 
