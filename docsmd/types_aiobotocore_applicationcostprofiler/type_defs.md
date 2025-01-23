# Type definitions

> [Index](../README.md) > [ApplicationCostProfiler](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ApplicationCostProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#applicationcostprofiler)
    type annotations stubs module [types-aiobotocore-applicationcostprofiler](https://pypi.org/project/types-aiobotocore-applicationcostprofiler/).



## DeleteReportDefinitionRequestRequestTypeDef

```python
# DeleteReportDefinitionRequestRequestTypeDef definition

class DeleteReportDefinitionRequestRequestTypeDef(TypedDict):
    reportId: str,
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

## GetReportDefinitionRequestRequestTypeDef

```python
# GetReportDefinitionRequestRequestTypeDef definition

class GetReportDefinitionRequestRequestTypeDef(TypedDict):
    reportId: str,
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucket: str,
    prefix: str,
```

## SourceS3LocationTypeDef

```python
# SourceS3LocationTypeDef definition

class SourceS3LocationTypeDef(TypedDict):
    bucket: str,
    key: str,
    region: NotRequired[S3BucketRegionType],  # (1)
```

1. See [:material-code-brackets: S3BucketRegionType](./literals.md#s3bucketregiontype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListReportDefinitionsRequestRequestTypeDef

```python
# ListReportDefinitionsRequestRequestTypeDef definition

class ListReportDefinitionsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## DeleteReportDefinitionResultTypeDef

```python
# DeleteReportDefinitionResultTypeDef definition

class DeleteReportDefinitionResultTypeDef(TypedDict):
    reportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportApplicationUsageResultTypeDef

```python
# ImportApplicationUsageResultTypeDef definition

class ImportApplicationUsageResultTypeDef(TypedDict):
    importId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutReportDefinitionResultTypeDef

```python
# PutReportDefinitionResultTypeDef definition

class PutReportDefinitionResultTypeDef(TypedDict):
    reportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReportDefinitionResultTypeDef

```python
# UpdateReportDefinitionResultTypeDef definition

class UpdateReportDefinitionResultTypeDef(TypedDict):
    reportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReportDefinitionResultTypeDef

```python
# GetReportDefinitionResultTypeDef definition

class GetReportDefinitionResultTypeDef(TypedDict):
    reportId: str,
    reportDescription: str,
    reportFrequency: ReportFrequencyType,  # (1)
    format: FormatType,  # (2)
    destinationS3Location: S3LocationTypeDef,  # (3)
    createdAt: datetime,
    lastUpdated: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ReportFrequencyType](./literals.md#reportfrequencytype) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutReportDefinitionRequestRequestTypeDef

```python
# PutReportDefinitionRequestRequestTypeDef definition

class PutReportDefinitionRequestRequestTypeDef(TypedDict):
    reportId: str,
    reportDescription: str,
    reportFrequency: ReportFrequencyType,  # (1)
    format: FormatType,  # (2)
    destinationS3Location: S3LocationTypeDef,  # (3)
```

1. See [:material-code-brackets: ReportFrequencyType](./literals.md#reportfrequencytype) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## ReportDefinitionTypeDef

```python
# ReportDefinitionTypeDef definition

class ReportDefinitionTypeDef(TypedDict):
    reportId: NotRequired[str],
    reportDescription: NotRequired[str],
    reportFrequency: NotRequired[ReportFrequencyType],  # (1)
    format: NotRequired[FormatType],  # (2)
    destinationS3Location: NotRequired[S3LocationTypeDef],  # (3)
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ReportFrequencyType](./literals.md#reportfrequencytype) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## UpdateReportDefinitionRequestRequestTypeDef

```python
# UpdateReportDefinitionRequestRequestTypeDef definition

class UpdateReportDefinitionRequestRequestTypeDef(TypedDict):
    reportId: str,
    reportDescription: str,
    reportFrequency: ReportFrequencyType,  # (1)
    format: FormatType,  # (2)
    destinationS3Location: S3LocationTypeDef,  # (3)
```

1. See [:material-code-brackets: ReportFrequencyType](./literals.md#reportfrequencytype) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## ImportApplicationUsageRequestRequestTypeDef

```python
# ImportApplicationUsageRequestRequestTypeDef definition

class ImportApplicationUsageRequestRequestTypeDef(TypedDict):
    sourceS3Location: SourceS3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: SourceS3LocationTypeDef](./type_defs.md#sources3locationtypedef) 
## ListReportDefinitionsRequestPaginateTypeDef

```python
# ListReportDefinitionsRequestPaginateTypeDef definition

class ListReportDefinitionsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReportDefinitionsResultTypeDef

```python
# ListReportDefinitionsResultTypeDef definition

class ListReportDefinitionsResultTypeDef(TypedDict):
    reportDefinitions: List[ReportDefinitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
