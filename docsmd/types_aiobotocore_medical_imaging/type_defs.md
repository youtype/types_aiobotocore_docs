# Type definitions

> [Index](../README.md) > [HealthImaging](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [HealthImaging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
    type annotations stubs module [types-aiobotocore-medical-imaging](https://pypi.org/project/types-aiobotocore-medical-imaging/).

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




## CopyDestinationImageSetPropertiesTypeDef

```python
# CopyDestinationImageSetPropertiesTypeDef definition

class CopyDestinationImageSetPropertiesTypeDef(TypedDict):
    imageSetId: str,
    latestVersionId: str,
    imageSetState: NotRequired[ImageSetStateType],  # (1)
    imageSetWorkflowStatus: NotRequired[ImageSetWorkflowStatusType],  # (2)
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    imageSetArn: NotRequired[str],
```

1. See [:material-code-brackets: ImageSetStateType](./literals.md#imagesetstatetype) 
2. See [:material-code-brackets: ImageSetWorkflowStatusType](./literals.md#imagesetworkflowstatustype) 
## CopyDestinationImageSetTypeDef

```python
# CopyDestinationImageSetTypeDef definition

class CopyDestinationImageSetTypeDef(TypedDict):
    imageSetId: str,
    latestVersionId: str,
```

## CopySourceImageSetPropertiesTypeDef

```python
# CopySourceImageSetPropertiesTypeDef definition

class CopySourceImageSetPropertiesTypeDef(TypedDict):
    imageSetId: str,
    latestVersionId: str,
    imageSetState: NotRequired[ImageSetStateType],  # (1)
    imageSetWorkflowStatus: NotRequired[ImageSetWorkflowStatusType],  # (2)
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    imageSetArn: NotRequired[str],
```

1. See [:material-code-brackets: ImageSetStateType](./literals.md#imagesetstatetype) 
2. See [:material-code-brackets: ImageSetWorkflowStatusType](./literals.md#imagesetworkflowstatustype) 
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

## MetadataCopiesTypeDef

```python
# MetadataCopiesTypeDef definition

class MetadataCopiesTypeDef(TypedDict):
    copiableAttributes: str,
```

## CreateDatastoreRequestRequestTypeDef

```python
# CreateDatastoreRequestRequestTypeDef definition

class CreateDatastoreRequestRequestTypeDef(TypedDict):
    clientToken: str,
    datastoreName: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    kmsKeyArn: NotRequired[str],
```

## DICOMImportJobPropertiesTypeDef

```python
# DICOMImportJobPropertiesTypeDef definition

class DICOMImportJobPropertiesTypeDef(TypedDict):
    jobId: str,
    jobName: str,
    jobStatus: JobStatusType,  # (1)
    datastoreId: str,
    dataAccessRoleArn: str,
    inputS3Uri: str,
    outputS3Uri: str,
    endedAt: NotRequired[datetime],
    submittedAt: NotRequired[datetime],
    message: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## DICOMImportJobSummaryTypeDef

```python
# DICOMImportJobSummaryTypeDef definition

class DICOMImportJobSummaryTypeDef(TypedDict):
    jobId: str,
    jobName: str,
    jobStatus: JobStatusType,  # (1)
    datastoreId: str,
    dataAccessRoleArn: NotRequired[str],
    endedAt: NotRequired[datetime],
    submittedAt: NotRequired[datetime],
    message: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## DICOMStudyDateAndTimeTypeDef

```python
# DICOMStudyDateAndTimeTypeDef definition

class DICOMStudyDateAndTimeTypeDef(TypedDict):
    DICOMStudyDate: str,
    DICOMStudyTime: NotRequired[str],
```

## DICOMTagsTypeDef

```python
# DICOMTagsTypeDef definition

class DICOMTagsTypeDef(TypedDict):
    DICOMPatientId: NotRequired[str],
    DICOMPatientName: NotRequired[str],
    DICOMPatientBirthDate: NotRequired[str],
    DICOMPatientSex: NotRequired[str],
    DICOMStudyInstanceUID: NotRequired[str],
    DICOMStudyId: NotRequired[str],
    DICOMStudyDescription: NotRequired[str],
    DICOMNumberOfStudyRelatedSeries: NotRequired[int],
    DICOMNumberOfStudyRelatedInstances: NotRequired[int],
    DICOMAccessionNumber: NotRequired[str],
    DICOMSeriesInstanceUID: NotRequired[str],
    DICOMSeriesModality: NotRequired[str],
    DICOMSeriesBodyPart: NotRequired[str],
    DICOMSeriesNumber: NotRequired[int],
    DICOMStudyDate: NotRequired[str],
    DICOMStudyTime: NotRequired[str],
```

## DatastorePropertiesTypeDef

```python
# DatastorePropertiesTypeDef definition

class DatastorePropertiesTypeDef(TypedDict):
    datastoreId: str,
    datastoreName: str,
    datastoreStatus: DatastoreStatusType,  # (1)
    kmsKeyArn: NotRequired[str],
    datastoreArn: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: DatastoreStatusType](./literals.md#datastorestatustype) 
## DatastoreSummaryTypeDef

```python
# DatastoreSummaryTypeDef definition

class DatastoreSummaryTypeDef(TypedDict):
    datastoreId: str,
    datastoreName: str,
    datastoreStatus: DatastoreStatusType,  # (1)
    datastoreArn: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: DatastoreStatusType](./literals.md#datastorestatustype) 
## DeleteDatastoreRequestRequestTypeDef

```python
# DeleteDatastoreRequestRequestTypeDef definition

class DeleteDatastoreRequestRequestTypeDef(TypedDict):
    datastoreId: str,
```

## DeleteImageSetRequestRequestTypeDef

```python
# DeleteImageSetRequestRequestTypeDef definition

class DeleteImageSetRequestRequestTypeDef(TypedDict):
    datastoreId: str,
    imageSetId: str,
```

## GetDICOMImportJobRequestRequestTypeDef

```python
# GetDICOMImportJobRequestRequestTypeDef definition

class GetDICOMImportJobRequestRequestTypeDef(TypedDict):
    datastoreId: str,
    jobId: str,
```

## GetDatastoreRequestRequestTypeDef

```python
# GetDatastoreRequestRequestTypeDef definition

class GetDatastoreRequestRequestTypeDef(TypedDict):
    datastoreId: str,
```

## ImageFrameInformationTypeDef

```python
# ImageFrameInformationTypeDef definition

class ImageFrameInformationTypeDef(TypedDict):
    imageFrameId: str,
```

## GetImageSetMetadataRequestRequestTypeDef

```python
# GetImageSetMetadataRequestRequestTypeDef definition

class GetImageSetMetadataRequestRequestTypeDef(TypedDict):
    datastoreId: str,
    imageSetId: str,
    versionId: NotRequired[str],
```

## GetImageSetRequestRequestTypeDef

```python
# GetImageSetRequestRequestTypeDef definition

class GetImageSetRequestRequestTypeDef(TypedDict):
    datastoreId: str,
    imageSetId: str,
    versionId: NotRequired[str],
```

## OverridesTypeDef

```python
# OverridesTypeDef definition

class OverridesTypeDef(TypedDict):
    forced: NotRequired[bool],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDICOMImportJobsRequestRequestTypeDef

```python
# ListDICOMImportJobsRequestRequestTypeDef definition

class ListDICOMImportJobsRequestRequestTypeDef(TypedDict):
    datastoreId: str,
    jobStatus: NotRequired[JobStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## ListDatastoresRequestRequestTypeDef

```python
# ListDatastoresRequestRequestTypeDef definition

class ListDatastoresRequestRequestTypeDef(TypedDict):
    datastoreStatus: NotRequired[DatastoreStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: DatastoreStatusType](./literals.md#datastorestatustype) 
## ListImageSetVersionsRequestRequestTypeDef

```python
# ListImageSetVersionsRequestRequestTypeDef definition

class ListImageSetVersionsRequestRequestTypeDef(TypedDict):
    datastoreId: str,
    imageSetId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## SortTypeDef

```python
# SortTypeDef definition

class SortTypeDef(TypedDict):
    sortOrder: SortOrderType,  # (1)
    sortField: SortFieldType,  # (2)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: SortFieldType](./literals.md#sortfieldtype) 
## StartDICOMImportJobRequestRequestTypeDef

```python
# StartDICOMImportJobRequestRequestTypeDef definition

class StartDICOMImportJobRequestRequestTypeDef(TypedDict):
    dataAccessRoleArn: str,
    clientToken: str,
    datastoreId: str,
    inputS3Uri: str,
    outputS3Uri: str,
    jobName: NotRequired[str],
    inputOwnerAccountId: NotRequired[str],
```

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

## DICOMUpdatesTypeDef

```python
# DICOMUpdatesTypeDef definition

class DICOMUpdatesTypeDef(TypedDict):
    removableAttributes: NotRequired[BlobTypeDef],
    updatableAttributes: NotRequired[BlobTypeDef],
```

## CopyImageSetResponseTypeDef

```python
# CopyImageSetResponseTypeDef definition

class CopyImageSetResponseTypeDef(TypedDict):
    datastoreId: str,
    sourceImageSetProperties: CopySourceImageSetPropertiesTypeDef,  # (1)
    destinationImageSetProperties: CopyDestinationImageSetPropertiesTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CopySourceImageSetPropertiesTypeDef](./type_defs.md#copysourceimagesetpropertiestypedef) 
2. See [:material-code-braces: CopyDestinationImageSetPropertiesTypeDef](./type_defs.md#copydestinationimagesetpropertiestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatastoreResponseTypeDef

```python
# CreateDatastoreResponseTypeDef definition

class CreateDatastoreResponseTypeDef(TypedDict):
    datastoreId: str,
    datastoreStatus: DatastoreStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DatastoreStatusType](./literals.md#datastorestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDatastoreResponseTypeDef

```python
# DeleteDatastoreResponseTypeDef definition

class DeleteDatastoreResponseTypeDef(TypedDict):
    datastoreId: str,
    datastoreStatus: DatastoreStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DatastoreStatusType](./literals.md#datastorestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteImageSetResponseTypeDef

```python
# DeleteImageSetResponseTypeDef definition

class DeleteImageSetResponseTypeDef(TypedDict):
    datastoreId: str,
    imageSetId: str,
    imageSetState: ImageSetStateType,  # (1)
    imageSetWorkflowStatus: ImageSetWorkflowStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ImageSetStateType](./literals.md#imagesetstatetype) 
2. See [:material-code-brackets: ImageSetWorkflowStatusType](./literals.md#imagesetworkflowstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetImageFrameResponseTypeDef

```python
# GetImageFrameResponseTypeDef definition

class GetImageFrameResponseTypeDef(TypedDict):
    imageFrameBlob: StreamingBody,
    contentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetImageSetMetadataResponseTypeDef

```python
# GetImageSetMetadataResponseTypeDef definition

class GetImageSetMetadataResponseTypeDef(TypedDict):
    imageSetMetadataBlob: StreamingBody,
    contentType: str,
    contentEncoding: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDICOMImportJobResponseTypeDef

```python
# StartDICOMImportJobResponseTypeDef definition

class StartDICOMImportJobResponseTypeDef(TypedDict):
    datastoreId: str,
    jobId: str,
    jobStatus: JobStatusType,  # (1)
    submittedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateImageSetMetadataResponseTypeDef

```python
# UpdateImageSetMetadataResponseTypeDef definition

class UpdateImageSetMetadataResponseTypeDef(TypedDict):
    datastoreId: str,
    imageSetId: str,
    latestVersionId: str,
    imageSetState: ImageSetStateType,  # (1)
    imageSetWorkflowStatus: ImageSetWorkflowStatusType,  # (2)
    createdAt: datetime,
    updatedAt: datetime,
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ImageSetStateType](./literals.md#imagesetstatetype) 
2. See [:material-code-brackets: ImageSetWorkflowStatusType](./literals.md#imagesetworkflowstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopySourceImageSetInformationTypeDef

```python
# CopySourceImageSetInformationTypeDef definition

class CopySourceImageSetInformationTypeDef(TypedDict):
    latestVersionId: str,
    DICOMCopies: NotRequired[MetadataCopiesTypeDef],  # (1)
```

1. See [:material-code-braces: MetadataCopiesTypeDef](./type_defs.md#metadatacopiestypedef) 
## GetDICOMImportJobResponseTypeDef

```python
# GetDICOMImportJobResponseTypeDef definition

class GetDICOMImportJobResponseTypeDef(TypedDict):
    jobProperties: DICOMImportJobPropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DICOMImportJobPropertiesTypeDef](./type_defs.md#dicomimportjobpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDICOMImportJobsResponseTypeDef

```python
# ListDICOMImportJobsResponseTypeDef definition

class ListDICOMImportJobsResponseTypeDef(TypedDict):
    jobSummaries: List[DICOMImportJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DICOMImportJobSummaryTypeDef](./type_defs.md#dicomimportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImageSetsMetadataSummaryTypeDef

```python
# ImageSetsMetadataSummaryTypeDef definition

class ImageSetsMetadataSummaryTypeDef(TypedDict):
    imageSetId: str,
    version: NotRequired[int],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    DICOMTags: NotRequired[DICOMTagsTypeDef],  # (1)
```

1. See [:material-code-braces: DICOMTagsTypeDef](./type_defs.md#dicomtagstypedef) 
## GetDatastoreResponseTypeDef

```python
# GetDatastoreResponseTypeDef definition

class GetDatastoreResponseTypeDef(TypedDict):
    datastoreProperties: DatastorePropertiesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatastorePropertiesTypeDef](./type_defs.md#datastorepropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatastoresResponseTypeDef

```python
# ListDatastoresResponseTypeDef definition

class ListDatastoresResponseTypeDef(TypedDict):
    datastoreSummaries: List[DatastoreSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DatastoreSummaryTypeDef](./type_defs.md#datastoresummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetImageFrameRequestRequestTypeDef

```python
# GetImageFrameRequestRequestTypeDef definition

class GetImageFrameRequestRequestTypeDef(TypedDict):
    datastoreId: str,
    imageSetId: str,
    imageFrameInformation: ImageFrameInformationTypeDef,  # (1)
```

1. See [:material-code-braces: ImageFrameInformationTypeDef](./type_defs.md#imageframeinformationtypedef) 
## GetImageSetResponseTypeDef

```python
# GetImageSetResponseTypeDef definition

class GetImageSetResponseTypeDef(TypedDict):
    datastoreId: str,
    imageSetId: str,
    versionId: str,
    imageSetState: ImageSetStateType,  # (1)
    imageSetWorkflowStatus: ImageSetWorkflowStatusType,  # (2)
    createdAt: datetime,
    updatedAt: datetime,
    deletedAt: datetime,
    message: str,
    imageSetArn: str,
    overrides: OverridesTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ImageSetStateType](./literals.md#imagesetstatetype) 
2. See [:material-code-brackets: ImageSetWorkflowStatusType](./literals.md#imagesetworkflowstatustype) 
3. See [:material-code-braces: OverridesTypeDef](./type_defs.md#overridestypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImageSetPropertiesTypeDef

```python
# ImageSetPropertiesTypeDef definition

class ImageSetPropertiesTypeDef(TypedDict):
    imageSetId: str,
    versionId: str,
    imageSetState: ImageSetStateType,  # (1)
    ImageSetWorkflowStatus: NotRequired[ImageSetWorkflowStatusType],  # (2)
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    deletedAt: NotRequired[datetime],
    message: NotRequired[str],
    overrides: NotRequired[OverridesTypeDef],  # (3)
```

1. See [:material-code-brackets: ImageSetStateType](./literals.md#imagesetstatetype) 
2. See [:material-code-brackets: ImageSetWorkflowStatusType](./literals.md#imagesetworkflowstatustype) 
3. See [:material-code-braces: OverridesTypeDef](./type_defs.md#overridestypedef) 
## ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef

```python
# ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef definition

class ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef(TypedDict):
    datastoreId: str,
    jobStatus: NotRequired[JobStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatastoresRequestListDatastoresPaginateTypeDef

```python
# ListDatastoresRequestListDatastoresPaginateTypeDef definition

class ListDatastoresRequestListDatastoresPaginateTypeDef(TypedDict):
    datastoreStatus: NotRequired[DatastoreStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DatastoreStatusType](./literals.md#datastorestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef

```python
# ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef definition

class ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef(TypedDict):
    datastoreId: str,
    imageSetId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchByAttributeValueTypeDef

```python
# SearchByAttributeValueTypeDef definition

class SearchByAttributeValueTypeDef(TypedDict):
    DICOMPatientId: NotRequired[str],
    DICOMAccessionNumber: NotRequired[str],
    DICOMStudyId: NotRequired[str],
    DICOMStudyInstanceUID: NotRequired[str],
    DICOMSeriesInstanceUID: NotRequired[str],
    createdAt: NotRequired[TimestampTypeDef],
    updatedAt: NotRequired[TimestampTypeDef],
    DICOMStudyDateAndTime: NotRequired[DICOMStudyDateAndTimeTypeDef],  # (1)
```

1. See [:material-code-braces: DICOMStudyDateAndTimeTypeDef](./type_defs.md#dicomstudydateandtimetypedef) 
## MetadataUpdatesTypeDef

```python
# MetadataUpdatesTypeDef definition

class MetadataUpdatesTypeDef(TypedDict):
    DICOMUpdates: NotRequired[DICOMUpdatesTypeDef],  # (1)
    revertToVersionId: NotRequired[str],
```

1. See [:material-code-braces: DICOMUpdatesTypeDef](./type_defs.md#dicomupdatestypedef) 
## CopyImageSetInformationTypeDef

```python
# CopyImageSetInformationTypeDef definition

class CopyImageSetInformationTypeDef(TypedDict):
    sourceImageSet: CopySourceImageSetInformationTypeDef,  # (1)
    destinationImageSet: NotRequired[CopyDestinationImageSetTypeDef],  # (2)
```

1. See [:material-code-braces: CopySourceImageSetInformationTypeDef](./type_defs.md#copysourceimagesetinformationtypedef) 
2. See [:material-code-braces: CopyDestinationImageSetTypeDef](./type_defs.md#copydestinationimagesettypedef) 
## SearchImageSetsResponseTypeDef

```python
# SearchImageSetsResponseTypeDef definition

class SearchImageSetsResponseTypeDef(TypedDict):
    imageSetsMetadataSummaries: List[ImageSetsMetadataSummaryTypeDef],  # (1)
    sort: SortTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImageSetsMetadataSummaryTypeDef](./type_defs.md#imagesetsmetadatasummarytypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImageSetVersionsResponseTypeDef

```python
# ListImageSetVersionsResponseTypeDef definition

class ListImageSetVersionsResponseTypeDef(TypedDict):
    imageSetPropertiesList: List[ImageSetPropertiesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImageSetPropertiesTypeDef](./type_defs.md#imagesetpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchFilterTypeDef

```python
# SearchFilterTypeDef definition

class SearchFilterTypeDef(TypedDict):
    values: Sequence[SearchByAttributeValueTypeDef],  # (1)
    operator: OperatorType,  # (2)
```

1. See [:material-code-braces: SearchByAttributeValueTypeDef](./type_defs.md#searchbyattributevaluetypedef) 
2. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## UpdateImageSetMetadataRequestRequestTypeDef

```python
# UpdateImageSetMetadataRequestRequestTypeDef definition

class UpdateImageSetMetadataRequestRequestTypeDef(TypedDict):
    datastoreId: str,
    imageSetId: str,
    latestVersionId: str,
    updateImageSetMetadataUpdates: MetadataUpdatesTypeDef,  # (1)
    force: NotRequired[bool],
```

1. See [:material-code-braces: MetadataUpdatesTypeDef](./type_defs.md#metadataupdatestypedef) 
## CopyImageSetRequestRequestTypeDef

```python
# CopyImageSetRequestRequestTypeDef definition

class CopyImageSetRequestRequestTypeDef(TypedDict):
    datastoreId: str,
    sourceImageSetId: str,
    copyImageSetInformation: CopyImageSetInformationTypeDef,  # (1)
    force: NotRequired[bool],
```

1. See [:material-code-braces: CopyImageSetInformationTypeDef](./type_defs.md#copyimagesetinformationtypedef) 
## SearchCriteriaTypeDef

```python
# SearchCriteriaTypeDef definition

class SearchCriteriaTypeDef(TypedDict):
    filters: NotRequired[Sequence[SearchFilterTypeDef]],  # (1)
    sort: NotRequired[SortTypeDef],  # (2)
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## SearchImageSetsRequestRequestTypeDef

```python
# SearchImageSetsRequestRequestTypeDef definition

class SearchImageSetsRequestRequestTypeDef(TypedDict):
    datastoreId: str,
    searchCriteria: NotRequired[SearchCriteriaTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef) 
## SearchImageSetsRequestSearchImageSetsPaginateTypeDef

```python
# SearchImageSetsRequestSearchImageSetsPaginateTypeDef definition

class SearchImageSetsRequestSearchImageSetsPaginateTypeDef(TypedDict):
    datastoreId: str,
    searchCriteria: NotRequired[SearchCriteriaTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
