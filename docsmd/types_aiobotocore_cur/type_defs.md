# Type definitions

> [Index](../README.md) > [CostandUsageReportService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
    type annotations stubs module [types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).



## DeleteReportDefinitionRequestRequestTypeDef

```python
# DeleteReportDefinitionRequestRequestTypeDef definition

class DeleteReportDefinitionRequestRequestTypeDef(TypedDict):
    ReportName: NotRequired[str],
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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeReportDefinitionsRequestRequestTypeDef

```python
# DescribeReportDefinitionsRequestRequestTypeDef definition

class DescribeReportDefinitionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ReportDefinitionTypeDef

```python
# ReportDefinitionTypeDef definition

class ReportDefinitionTypeDef(TypedDict):
    ReportName: str,
    TimeUnit: TimeUnitType,  # (1)
    Format: ReportFormatType,  # (2)
    Compression: CompressionFormatType,  # (3)
    AdditionalSchemaElements: List[SchemaElementType],  # (4)
    S3Bucket: str,
    S3Prefix: str,
    S3Region: AWSRegionType,  # (5)
    AdditionalArtifacts: NotRequired[List[AdditionalArtifactType]],  # (6)
    RefreshClosedReports: NotRequired[bool],
    ReportVersioning: NotRequired[ReportVersioningType],  # (7)
    BillingViewArn: NotRequired[str],
```

1. See [:material-code-brackets: TimeUnitType](./literals.md#timeunittype) 
2. See [:material-code-brackets: ReportFormatType](./literals.md#reportformattype) 
3. See [:material-code-brackets: CompressionFormatType](./literals.md#compressionformattype) 
4. See [:material-code-brackets: SchemaElementType](./literals.md#schemaelementtype) 
5. See [:material-code-brackets: AWSRegionType](./literals.md#awsregiontype) 
6. See [:material-code-brackets: AdditionalArtifactType](./literals.md#additionalartifacttype) 
7. See [:material-code-brackets: ReportVersioningType](./literals.md#reportversioningtype) 
## DeleteReportDefinitionResponseTypeDef

```python
# DeleteReportDefinitionResponseTypeDef definition

class DeleteReportDefinitionResponseTypeDef(TypedDict):
    ResponseMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef

```python
# DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef definition

class DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeReportDefinitionsResponseTypeDef

```python
# DescribeReportDefinitionsResponseTypeDef definition

class DescribeReportDefinitionsResponseTypeDef(TypedDict):
    ReportDefinitions: List[ReportDefinitionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyReportDefinitionRequestRequestTypeDef

```python
# ModifyReportDefinitionRequestRequestTypeDef definition

class ModifyReportDefinitionRequestRequestTypeDef(TypedDict):
    ReportName: str,
    ReportDefinition: ReportDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef) 
## PutReportDefinitionRequestRequestTypeDef

```python
# PutReportDefinitionRequestRequestTypeDef definition

class PutReportDefinitionRequestRequestTypeDef(TypedDict):
    ReportDefinition: ReportDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef) 
