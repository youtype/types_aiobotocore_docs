# Type definitions

> [Index](../README.md) > [LookoutforVision](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LookoutforVision](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#lookoutforvision)
    type annotations stubs module [types-aiobotocore-lookoutvision](https://pypi.org/project/types-aiobotocore-lookoutvision/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_lookoutvision.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


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
# TimestampTypeDef Union usage example

from types_aiobotocore_lookoutvision.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ModelPackagingConfigurationUnionTypeDef

```python
# ModelPackagingConfigurationUnionTypeDef Union usage example

from types_aiobotocore_lookoutvision.type_defs import ModelPackagingConfigurationUnionTypeDef


def get_value() -> ModelPackagingConfigurationUnionTypeDef:
    return ...


# ModelPackagingConfigurationUnionTypeDef definition

ModelPackagingConfigurationUnionTypeDef = Union[
    ModelPackagingConfigurationTypeDef,  # (1)
    ModelPackagingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ModelPackagingConfigurationTypeDef](./type_defs.md#modelpackagingconfigurationtypedef) 
2. See [:material-code-braces: ModelPackagingConfigurationOutputTypeDef](./type_defs.md#modelpackagingconfigurationoutputtypedef) 



## PixelAnomalyTypeDef

```python
# PixelAnomalyTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import PixelAnomalyTypeDef


def get_value() -> PixelAnomalyTypeDef:
    return {
        "TotalPercentageArea": ...,
    }


# PixelAnomalyTypeDef definition

class PixelAnomalyTypeDef(TypedDict):
    TotalPercentageArea: NotRequired[float],
    Color: NotRequired[str],
```

## DatasetMetadataTypeDef

```python
# DatasetMetadataTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DatasetMetadataTypeDef


def get_value() -> DatasetMetadataTypeDef:
    return {
        "DatasetType": ...,
    }


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
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


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
# TagTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateProjectRequestTypeDef

```python
# CreateProjectRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import CreateProjectRequestTypeDef


def get_value() -> CreateProjectRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# CreateProjectRequestTypeDef definition

class CreateProjectRequestTypeDef(TypedDict):
    ProjectName: str,
    ClientToken: NotRequired[str],
```

## ProjectMetadataTypeDef

```python
# ProjectMetadataTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ProjectMetadataTypeDef


def get_value() -> ProjectMetadataTypeDef:
    return {
        "ProjectArn": ...,
    }


# ProjectMetadataTypeDef definition

class ProjectMetadataTypeDef(TypedDict):
    ProjectArn: NotRequired[str],
    ProjectName: NotRequired[str],
    CreationTimestamp: NotRequired[datetime],
```

## DatasetImageStatsTypeDef

```python
# DatasetImageStatsTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DatasetImageStatsTypeDef


def get_value() -> DatasetImageStatsTypeDef:
    return {
        "Total": ...,
    }


# DatasetImageStatsTypeDef definition

class DatasetImageStatsTypeDef(TypedDict):
    Total: NotRequired[int],
    Labeled: NotRequired[int],
    Normal: NotRequired[int],
    Anomaly: NotRequired[int],
```

## InputS3ObjectTypeDef

```python
# InputS3ObjectTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import InputS3ObjectTypeDef


def get_value() -> InputS3ObjectTypeDef:
    return {
        "Bucket": ...,
    }


# InputS3ObjectTypeDef definition

class InputS3ObjectTypeDef(TypedDict):
    Bucket: str,
    Key: str,
    VersionId: NotRequired[str],
```

## DeleteDatasetRequestTypeDef

```python
# DeleteDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DeleteDatasetRequestTypeDef


def get_value() -> DeleteDatasetRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# DeleteDatasetRequestTypeDef definition

class DeleteDatasetRequestTypeDef(TypedDict):
    ProjectName: str,
    DatasetType: str,
    ClientToken: NotRequired[str],
```

## DeleteModelRequestTypeDef

```python
# DeleteModelRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DeleteModelRequestTypeDef


def get_value() -> DeleteModelRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# DeleteModelRequestTypeDef definition

class DeleteModelRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
    ClientToken: NotRequired[str],
```

## DeleteProjectRequestTypeDef

```python
# DeleteProjectRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DeleteProjectRequestTypeDef


def get_value() -> DeleteProjectRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# DeleteProjectRequestTypeDef definition

class DeleteProjectRequestTypeDef(TypedDict):
    ProjectName: str,
    ClientToken: NotRequired[str],
```

## DescribeDatasetRequestTypeDef

```python
# DescribeDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DescribeDatasetRequestTypeDef


def get_value() -> DescribeDatasetRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# DescribeDatasetRequestTypeDef definition

class DescribeDatasetRequestTypeDef(TypedDict):
    ProjectName: str,
    DatasetType: str,
```

## DescribeModelPackagingJobRequestTypeDef

```python
# DescribeModelPackagingJobRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DescribeModelPackagingJobRequestTypeDef


def get_value() -> DescribeModelPackagingJobRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# DescribeModelPackagingJobRequestTypeDef definition

class DescribeModelPackagingJobRequestTypeDef(TypedDict):
    ProjectName: str,
    JobName: str,
```

## DescribeModelRequestTypeDef

```python
# DescribeModelRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DescribeModelRequestTypeDef


def get_value() -> DescribeModelRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# DescribeModelRequestTypeDef definition

class DescribeModelRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
```

## DescribeProjectRequestTypeDef

```python
# DescribeProjectRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DescribeProjectRequestTypeDef


def get_value() -> DescribeProjectRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# DescribeProjectRequestTypeDef definition

class DescribeProjectRequestTypeDef(TypedDict):
    ProjectName: str,
```

## ImageSourceTypeDef

```python
# ImageSourceTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ImageSourceTypeDef


def get_value() -> ImageSourceTypeDef:
    return {
        "Type": ...,
    }


# ImageSourceTypeDef definition

class ImageSourceTypeDef(TypedDict):
    Type: NotRequired[str],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import S3LocationTypeDef


def get_value() -> S3LocationTypeDef:
    return {
        "Bucket": ...,
    }


# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    Bucket: str,
    Prefix: NotRequired[str],
```

## TargetPlatformTypeDef

```python
# TargetPlatformTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import TargetPlatformTypeDef


def get_value() -> TargetPlatformTypeDef:
    return {
        "Os": ...,
    }


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
# GreengrassOutputDetailsTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import GreengrassOutputDetailsTypeDef


def get_value() -> GreengrassOutputDetailsTypeDef:
    return {
        "ComponentVersionArn": ...,
    }


# GreengrassOutputDetailsTypeDef definition

class GreengrassOutputDetailsTypeDef(TypedDict):
    ComponentVersionArn: NotRequired[str],
    ComponentName: NotRequired[str],
    ComponentVersion: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListModelPackagingJobsRequestTypeDef

```python
# ListModelPackagingJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListModelPackagingJobsRequestTypeDef


def get_value() -> ListModelPackagingJobsRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# ListModelPackagingJobsRequestTypeDef definition

class ListModelPackagingJobsRequestTypeDef(TypedDict):
    ProjectName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ModelPackagingJobMetadataTypeDef

```python
# ModelPackagingJobMetadataTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ModelPackagingJobMetadataTypeDef


def get_value() -> ModelPackagingJobMetadataTypeDef:
    return {
        "JobName": ...,
    }


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
## ListModelsRequestTypeDef

```python
# ListModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListModelsRequestTypeDef


def get_value() -> ListModelsRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# ListModelsRequestTypeDef definition

class ListModelsRequestTypeDef(TypedDict):
    ProjectName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListProjectsRequestTypeDef

```python
# ListProjectsRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListProjectsRequestTypeDef


def get_value() -> ListProjectsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListProjectsRequestTypeDef definition

class ListProjectsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ModelPerformanceTypeDef

```python
# ModelPerformanceTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ModelPerformanceTypeDef


def get_value() -> ModelPerformanceTypeDef:
    return {
        "F1Score": ...,
    }


# ModelPerformanceTypeDef definition

class ModelPerformanceTypeDef(TypedDict):
    F1Score: NotRequired[float],
    Recall: NotRequired[float],
    Precision: NotRequired[float],
```

## OutputS3ObjectTypeDef

```python
# OutputS3ObjectTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import OutputS3ObjectTypeDef


def get_value() -> OutputS3ObjectTypeDef:
    return {
        "Bucket": ...,
    }


# OutputS3ObjectTypeDef definition

class OutputS3ObjectTypeDef(TypedDict):
    Bucket: str,
    Key: str,
```

## StartModelRequestTypeDef

```python
# StartModelRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import StartModelRequestTypeDef


def get_value() -> StartModelRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# StartModelRequestTypeDef definition

class StartModelRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
    MinInferenceUnits: int,
    ClientToken: NotRequired[str],
    MaxInferenceUnits: NotRequired[int],
```

## StopModelRequestTypeDef

```python
# StopModelRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import StopModelRequestTypeDef


def get_value() -> StopModelRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# StopModelRequestTypeDef definition

class StopModelRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
    ClientToken: NotRequired[str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## AnomalyTypeDef

```python
# AnomalyTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import AnomalyTypeDef


def get_value() -> AnomalyTypeDef:
    return {
        "Name": ...,
    }


# AnomalyTypeDef definition

class AnomalyTypeDef(TypedDict):
    Name: NotRequired[str],
    PixelAnomaly: NotRequired[PixelAnomalyTypeDef],  # (1)
```

1. See [:material-code-braces: PixelAnomalyTypeDef](./type_defs.md#pixelanomalytypedef) 
## DetectAnomaliesRequestTypeDef

```python
# DetectAnomaliesRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DetectAnomaliesRequestTypeDef


def get_value() -> DetectAnomaliesRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# DetectAnomaliesRequestTypeDef definition

class DetectAnomaliesRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
    Body: BlobTypeDef,
    ContentType: str,
```

## UpdateDatasetEntriesRequestTypeDef

```python
# UpdateDatasetEntriesRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import UpdateDatasetEntriesRequestTypeDef


def get_value() -> UpdateDatasetEntriesRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# UpdateDatasetEntriesRequestTypeDef definition

class UpdateDatasetEntriesRequestTypeDef(TypedDict):
    ProjectName: str,
    DatasetType: str,
    Changes: BlobTypeDef,
    ClientToken: NotRequired[str],
```

## ProjectDescriptionTypeDef

```python
# ProjectDescriptionTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ProjectDescriptionTypeDef


def get_value() -> ProjectDescriptionTypeDef:
    return {
        "ProjectArn": ...,
    }


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
# CreateDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import CreateDatasetResponseTypeDef


def get_value() -> CreateDatasetResponseTypeDef:
    return {
        "DatasetMetadata": ...,
    }


# CreateDatasetResponseTypeDef definition

class CreateDatasetResponseTypeDef(TypedDict):
    DatasetMetadata: DatasetMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetMetadataTypeDef](./type_defs.md#datasetmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteModelResponseTypeDef

```python
# DeleteModelResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DeleteModelResponseTypeDef


def get_value() -> DeleteModelResponseTypeDef:
    return {
        "ModelArn": ...,
    }


# DeleteModelResponseTypeDef definition

class DeleteModelResponseTypeDef(TypedDict):
    ModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProjectResponseTypeDef

```python
# DeleteProjectResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DeleteProjectResponseTypeDef


def get_value() -> DeleteProjectResponseTypeDef:
    return {
        "ProjectArn": ...,
    }


# DeleteProjectResponseTypeDef definition

class DeleteProjectResponseTypeDef(TypedDict):
    ProjectArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatasetEntriesResponseTypeDef

```python
# ListDatasetEntriesResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListDatasetEntriesResponseTypeDef


def get_value() -> ListDatasetEntriesResponseTypeDef:
    return {
        "DatasetEntries": ...,
    }


# ListDatasetEntriesResponseTypeDef definition

class ListDatasetEntriesResponseTypeDef(TypedDict):
    DatasetEntries: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartModelPackagingJobResponseTypeDef

```python
# StartModelPackagingJobResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import StartModelPackagingJobResponseTypeDef


def get_value() -> StartModelPackagingJobResponseTypeDef:
    return {
        "JobName": ...,
    }


# StartModelPackagingJobResponseTypeDef definition

class StartModelPackagingJobResponseTypeDef(TypedDict):
    JobName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartModelResponseTypeDef

```python
# StartModelResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import StartModelResponseTypeDef


def get_value() -> StartModelResponseTypeDef:
    return {
        "Status": ...,
    }


# StartModelResponseTypeDef definition

class StartModelResponseTypeDef(TypedDict):
    Status: ModelHostingStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ModelHostingStatusType](./literals.md#modelhostingstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopModelResponseTypeDef

```python
# StopModelResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import StopModelResponseTypeDef


def get_value() -> StopModelResponseTypeDef:
    return {
        "Status": ...,
    }


# StopModelResponseTypeDef definition

class StopModelResponseTypeDef(TypedDict):
    Status: ModelHostingStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ModelHostingStatusType](./literals.md#modelhostingstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDatasetEntriesResponseTypeDef

```python
# UpdateDatasetEntriesResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import UpdateDatasetEntriesResponseTypeDef


def get_value() -> UpdateDatasetEntriesResponseTypeDef:
    return {
        "Status": ...,
    }


# UpdateDatasetEntriesResponseTypeDef definition

class UpdateDatasetEntriesResponseTypeDef(TypedDict):
    Status: DatasetStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateProjectResponseTypeDef

```python
# CreateProjectResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import CreateProjectResponseTypeDef


def get_value() -> CreateProjectResponseTypeDef:
    return {
        "ProjectMetadata": ...,
    }


# CreateProjectResponseTypeDef definition

class CreateProjectResponseTypeDef(TypedDict):
    ProjectMetadata: ProjectMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectMetadataTypeDef](./type_defs.md#projectmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectsResponseTypeDef

```python
# ListProjectsResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListProjectsResponseTypeDef


def get_value() -> ListProjectsResponseTypeDef:
    return {
        "Projects": ...,
    }


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
# DatasetDescriptionTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DatasetDescriptionTypeDef


def get_value() -> DatasetDescriptionTypeDef:
    return {
        "ProjectName": ...,
    }


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
# DatasetGroundTruthManifestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DatasetGroundTruthManifestTypeDef


def get_value() -> DatasetGroundTruthManifestTypeDef:
    return {
        "S3Object": ...,
    }


# DatasetGroundTruthManifestTypeDef definition

class DatasetGroundTruthManifestTypeDef(TypedDict):
    S3Object: NotRequired[InputS3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: InputS3ObjectTypeDef](./type_defs.md#inputs3objecttypedef) 
## OutputConfigTypeDef

```python
# OutputConfigTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import OutputConfigTypeDef


def get_value() -> OutputConfigTypeDef:
    return {
        "S3Location": ...,
    }


# OutputConfigTypeDef definition

class OutputConfigTypeDef(TypedDict):
    S3Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## GreengrassConfigurationOutputTypeDef

```python
# GreengrassConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import GreengrassConfigurationOutputTypeDef


def get_value() -> GreengrassConfigurationOutputTypeDef:
    return {
        "CompilerOptions": ...,
    }


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
# GreengrassConfigurationTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import GreengrassConfigurationTypeDef


def get_value() -> GreengrassConfigurationTypeDef:
    return {
        "CompilerOptions": ...,
    }


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
# ModelPackagingOutputDetailsTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ModelPackagingOutputDetailsTypeDef


def get_value() -> ModelPackagingOutputDetailsTypeDef:
    return {
        "Greengrass": ...,
    }


# ModelPackagingOutputDetailsTypeDef definition

class ModelPackagingOutputDetailsTypeDef(TypedDict):
    Greengrass: NotRequired[GreengrassOutputDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: GreengrassOutputDetailsTypeDef](./type_defs.md#greengrassoutputdetailstypedef) 
## ListModelPackagingJobsRequestPaginateTypeDef

```python
# ListModelPackagingJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListModelPackagingJobsRequestPaginateTypeDef


def get_value() -> ListModelPackagingJobsRequestPaginateTypeDef:
    return {
        "ProjectName": ...,
    }


# ListModelPackagingJobsRequestPaginateTypeDef definition

class ListModelPackagingJobsRequestPaginateTypeDef(TypedDict):
    ProjectName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelsRequestPaginateTypeDef

```python
# ListModelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListModelsRequestPaginateTypeDef


def get_value() -> ListModelsRequestPaginateTypeDef:
    return {
        "ProjectName": ...,
    }


# ListModelsRequestPaginateTypeDef definition

class ListModelsRequestPaginateTypeDef(TypedDict):
    ProjectName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestPaginateTypeDef

```python
# ListProjectsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListProjectsRequestPaginateTypeDef


def get_value() -> ListProjectsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListProjectsRequestPaginateTypeDef definition

class ListProjectsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetEntriesRequestPaginateTypeDef

```python
# ListDatasetEntriesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListDatasetEntriesRequestPaginateTypeDef


def get_value() -> ListDatasetEntriesRequestPaginateTypeDef:
    return {
        "ProjectName": ...,
    }


# ListDatasetEntriesRequestPaginateTypeDef definition

class ListDatasetEntriesRequestPaginateTypeDef(TypedDict):
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
## ListDatasetEntriesRequestTypeDef

```python
# ListDatasetEntriesRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListDatasetEntriesRequestTypeDef


def get_value() -> ListDatasetEntriesRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# ListDatasetEntriesRequestTypeDef definition

class ListDatasetEntriesRequestTypeDef(TypedDict):
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
# ListModelPackagingJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListModelPackagingJobsResponseTypeDef


def get_value() -> ListModelPackagingJobsResponseTypeDef:
    return {
        "ModelPackagingJobs": ...,
    }


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
# ModelMetadataTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ModelMetadataTypeDef


def get_value() -> ModelMetadataTypeDef:
    return {
        "CreationTimestamp": ...,
    }


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
# DetectAnomalyResultTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DetectAnomalyResultTypeDef


def get_value() -> DetectAnomalyResultTypeDef:
    return {
        "Source": ...,
    }


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
# DescribeProjectResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DescribeProjectResponseTypeDef


def get_value() -> DescribeProjectResponseTypeDef:
    return {
        "ProjectDescription": ...,
    }


# DescribeProjectResponseTypeDef definition

class DescribeProjectResponseTypeDef(TypedDict):
    ProjectDescription: ProjectDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectDescriptionTypeDef](./type_defs.md#projectdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDatasetResponseTypeDef

```python
# DescribeDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DescribeDatasetResponseTypeDef


def get_value() -> DescribeDatasetResponseTypeDef:
    return {
        "DatasetDescription": ...,
    }


# DescribeDatasetResponseTypeDef definition

class DescribeDatasetResponseTypeDef(TypedDict):
    DatasetDescription: DatasetDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetDescriptionTypeDef](./type_defs.md#datasetdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetSourceTypeDef

```python
# DatasetSourceTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DatasetSourceTypeDef


def get_value() -> DatasetSourceTypeDef:
    return {
        "GroundTruthManifest": ...,
    }


# DatasetSourceTypeDef definition

class DatasetSourceTypeDef(TypedDict):
    GroundTruthManifest: NotRequired[DatasetGroundTruthManifestTypeDef],  # (1)
```

1. See [:material-code-braces: DatasetGroundTruthManifestTypeDef](./type_defs.md#datasetgroundtruthmanifesttypedef) 
## CreateModelRequestTypeDef

```python
# CreateModelRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import CreateModelRequestTypeDef


def get_value() -> CreateModelRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# CreateModelRequestTypeDef definition

class CreateModelRequestTypeDef(TypedDict):
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
# ModelDescriptionTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ModelDescriptionTypeDef


def get_value() -> ModelDescriptionTypeDef:
    return {
        "ModelVersion": ...,
    }


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
# ModelPackagingConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ModelPackagingConfigurationOutputTypeDef


def get_value() -> ModelPackagingConfigurationOutputTypeDef:
    return {
        "Greengrass": ...,
    }


# ModelPackagingConfigurationOutputTypeDef definition

class ModelPackagingConfigurationOutputTypeDef(TypedDict):
    Greengrass: GreengrassConfigurationOutputTypeDef,  # (1)
```

1. See [:material-code-braces: GreengrassConfigurationOutputTypeDef](./type_defs.md#greengrassconfigurationoutputtypedef) 
## ModelPackagingConfigurationTypeDef

```python
# ModelPackagingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ModelPackagingConfigurationTypeDef


def get_value() -> ModelPackagingConfigurationTypeDef:
    return {
        "Greengrass": ...,
    }


# ModelPackagingConfigurationTypeDef definition

class ModelPackagingConfigurationTypeDef(TypedDict):
    Greengrass: GreengrassConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: GreengrassConfigurationTypeDef](./type_defs.md#greengrassconfigurationtypedef) 
## CreateModelResponseTypeDef

```python
# CreateModelResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import CreateModelResponseTypeDef


def get_value() -> CreateModelResponseTypeDef:
    return {
        "ModelMetadata": ...,
    }


# CreateModelResponseTypeDef definition

class CreateModelResponseTypeDef(TypedDict):
    ModelMetadata: ModelMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelMetadataTypeDef](./type_defs.md#modelmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelsResponseTypeDef

```python
# ListModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ListModelsResponseTypeDef


def get_value() -> ListModelsResponseTypeDef:
    return {
        "Models": ...,
    }


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
# DetectAnomaliesResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DetectAnomaliesResponseTypeDef


def get_value() -> DetectAnomaliesResponseTypeDef:
    return {
        "DetectAnomalyResult": ...,
    }


# DetectAnomaliesResponseTypeDef definition

class DetectAnomaliesResponseTypeDef(TypedDict):
    DetectAnomalyResult: DetectAnomalyResultTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectAnomalyResultTypeDef](./type_defs.md#detectanomalyresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetRequestTypeDef

```python
# CreateDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import CreateDatasetRequestTypeDef


def get_value() -> CreateDatasetRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# CreateDatasetRequestTypeDef definition

class CreateDatasetRequestTypeDef(TypedDict):
    ProjectName: str,
    DatasetType: str,
    DatasetSource: NotRequired[DatasetSourceTypeDef],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef) 
## DescribeModelResponseTypeDef

```python
# DescribeModelResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DescribeModelResponseTypeDef


def get_value() -> DescribeModelResponseTypeDef:
    return {
        "ModelDescription": ...,
    }


# DescribeModelResponseTypeDef definition

class DescribeModelResponseTypeDef(TypedDict):
    ModelDescription: ModelDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelDescriptionTypeDef](./type_defs.md#modeldescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelPackagingDescriptionTypeDef

```python
# ModelPackagingDescriptionTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import ModelPackagingDescriptionTypeDef


def get_value() -> ModelPackagingDescriptionTypeDef:
    return {
        "JobName": ...,
    }


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
## DescribeModelPackagingJobResponseTypeDef

```python
# DescribeModelPackagingJobResponseTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import DescribeModelPackagingJobResponseTypeDef


def get_value() -> DescribeModelPackagingJobResponseTypeDef:
    return {
        "ModelPackagingDescription": ...,
    }


# DescribeModelPackagingJobResponseTypeDef definition

class DescribeModelPackagingJobResponseTypeDef(TypedDict):
    ModelPackagingDescription: ModelPackagingDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelPackagingDescriptionTypeDef](./type_defs.md#modelpackagingdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartModelPackagingJobRequestTypeDef

```python
# StartModelPackagingJobRequestTypeDef TypedDict usage example

from types_aiobotocore_lookoutvision.type_defs import StartModelPackagingJobRequestTypeDef


def get_value() -> StartModelPackagingJobRequestTypeDef:
    return {
        "ProjectName": ...,
    }


# StartModelPackagingJobRequestTypeDef definition

class StartModelPackagingJobRequestTypeDef(TypedDict):
    ProjectName: str,
    ModelVersion: str,
    Configuration: ModelPackagingConfigurationUnionTypeDef,  # (1)
    JobName: NotRequired[str],
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: ModelPackagingConfigurationTypeDef](./type_defs.md#modelpackagingconfigurationtypedef) [:material-code-braces: ModelPackagingConfigurationOutputTypeDef](./type_defs.md#modelpackagingconfigurationoutputtypedef) 
