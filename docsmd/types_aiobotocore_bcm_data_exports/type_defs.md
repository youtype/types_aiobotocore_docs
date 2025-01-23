# Type definitions

> [Index](../README.md) > [BillingandCostManagementDataExports](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [BillingandCostManagementDataExports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#billingandcostmanagementdataexports)
    type annotations stubs module [types-aiobotocore-bcm-data-exports](https://pypi.org/project/types-aiobotocore-bcm-data-exports/).

## DataQueryUnionTypeDef

```python
# DataQueryUnionTypeDef definition

DataQueryUnionTypeDef = Union[
    DataQueryTypeDef,  # (1)
    DataQueryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DataQueryTypeDef](./type_defs.md#dataquerytypedef) 
2. See [:material-code-braces: DataQueryOutputTypeDef](./type_defs.md#dataqueryoutputtypedef) 



## ColumnTypeDef

```python
# ColumnTypeDef definition

class ColumnTypeDef(TypedDict):
    Description: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[str],
```

## ResourceTagTypeDef

```python
# ResourceTagTypeDef definition

class ResourceTagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## DataQueryOutputTypeDef

```python
# DataQueryOutputTypeDef definition

class DataQueryOutputTypeDef(TypedDict):
    QueryStatement: str,
    TableConfigurations: NotRequired[Dict[str, Dict[str, str]]],
```

## DataQueryTypeDef

```python
# DataQueryTypeDef definition

class DataQueryTypeDef(TypedDict):
    QueryStatement: str,
    TableConfigurations: NotRequired[Mapping[str, Mapping[str, str]]],
```

## DeleteExportRequestRequestTypeDef

```python
# DeleteExportRequestRequestTypeDef definition

class DeleteExportRequestRequestTypeDef(TypedDict):
    ExportArn: str,
```

## ExecutionStatusTypeDef

```python
# ExecutionStatusTypeDef definition

class ExecutionStatusTypeDef(TypedDict):
    CompletedAt: NotRequired[datetime],
    CreatedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    StatusCode: NotRequired[ExecutionStatusCodeType],  # (1)
    StatusReason: NotRequired[ExecutionStatusReasonType],  # (2)
```

1. See [:material-code-brackets: ExecutionStatusCodeType](./literals.md#executionstatuscodetype) 
2. See [:material-code-brackets: ExecutionStatusReasonType](./literals.md#executionstatusreasontype) 
## RefreshCadenceTypeDef

```python
# RefreshCadenceTypeDef definition

class RefreshCadenceTypeDef(TypedDict):
    Frequency: FrequencyOptionType,  # (1)
```

1. See [:material-code-brackets: FrequencyOptionType](./literals.md#frequencyoptiontype) 
## ExportStatusTypeDef

```python
# ExportStatusTypeDef definition

class ExportStatusTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    LastRefreshedAt: NotRequired[datetime],
    LastUpdatedAt: NotRequired[datetime],
    StatusCode: NotRequired[ExportStatusCodeType],  # (1)
    StatusReason: NotRequired[ExecutionStatusReasonType],  # (2)
```

1. See [:material-code-brackets: ExportStatusCodeType](./literals.md#exportstatuscodetype) 
2. See [:material-code-brackets: ExecutionStatusReasonType](./literals.md#executionstatusreasontype) 
## GetExecutionRequestRequestTypeDef

```python
# GetExecutionRequestRequestTypeDef definition

class GetExecutionRequestRequestTypeDef(TypedDict):
    ExecutionId: str,
    ExportArn: str,
```

## GetExportRequestRequestTypeDef

```python
# GetExportRequestRequestTypeDef definition

class GetExportRequestRequestTypeDef(TypedDict):
    ExportArn: str,
```

## GetTableRequestRequestTypeDef

```python
# GetTableRequestRequestTypeDef definition

class GetTableRequestRequestTypeDef(TypedDict):
    TableName: str,
    TableProperties: NotRequired[Mapping[str, str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListExecutionsRequestRequestTypeDef

```python
# ListExecutionsRequestRequestTypeDef definition

class ListExecutionsRequestRequestTypeDef(TypedDict):
    ExportArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListExportsRequestRequestTypeDef

```python
# ListExportsRequestRequestTypeDef definition

class ListExportsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTablesRequestRequestTypeDef

```python
# ListTablesRequestRequestTypeDef definition

class ListTablesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## S3OutputConfigurationsTypeDef

```python
# S3OutputConfigurationsTypeDef definition

class S3OutputConfigurationsTypeDef(TypedDict):
    Compression: CompressionOptionType,  # (1)
    Format: FormatOptionType,  # (2)
    OutputType: S3OutputTypeType,  # (3)
    Overwrite: OverwriteOptionType,  # (4)
```

1. See [:material-code-brackets: CompressionOptionType](./literals.md#compressionoptiontype) 
2. See [:material-code-brackets: FormatOptionType](./literals.md#formatoptiontype) 
3. See [:material-code-brackets: S3OutputTypeType](./literals.md#s3outputtypetype) 
4. See [:material-code-brackets: OverwriteOptionType](./literals.md#overwriteoptiontype) 
## TablePropertyDescriptionTypeDef

```python
# TablePropertyDescriptionTypeDef definition

class TablePropertyDescriptionTypeDef(TypedDict):
    DefaultValue: NotRequired[str],
    Description: NotRequired[str],
    Name: NotRequired[str],
    ValidValues: NotRequired[List[str]],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    ResourceTagKeys: Sequence[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    ResourceTags: Sequence[ResourceTagTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## CreateExportResponseTypeDef

```python
# CreateExportResponseTypeDef definition

class CreateExportResponseTypeDef(TypedDict):
    ExportArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteExportResponseTypeDef

```python
# DeleteExportResponseTypeDef definition

class DeleteExportResponseTypeDef(TypedDict):
    ExportArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableResponseTypeDef

```python
# GetTableResponseTypeDef definition

class GetTableResponseTypeDef(TypedDict):
    Description: str,
    Schema: List[ColumnTypeDef],  # (1)
    TableName: str,
    TableProperties: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    ResourceTags: List[ResourceTagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateExportResponseTypeDef

```python
# UpdateExportResponseTypeDef definition

class UpdateExportResponseTypeDef(TypedDict):
    ExportArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecutionReferenceTypeDef

```python
# ExecutionReferenceTypeDef definition

class ExecutionReferenceTypeDef(TypedDict):
    ExecutionId: str,
    ExecutionStatus: ExecutionStatusTypeDef,  # (1)
```

1. See [:material-code-braces: ExecutionStatusTypeDef](./type_defs.md#executionstatustypedef) 
## ExportReferenceTypeDef

```python
# ExportReferenceTypeDef definition

class ExportReferenceTypeDef(TypedDict):
    ExportArn: str,
    ExportName: str,
    ExportStatus: ExportStatusTypeDef,  # (1)
```

1. See [:material-code-braces: ExportStatusTypeDef](./type_defs.md#exportstatustypedef) 
## ListExecutionsRequestPaginateTypeDef

```python
# ListExecutionsRequestPaginateTypeDef definition

class ListExecutionsRequestPaginateTypeDef(TypedDict):
    ExportArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExportsRequestPaginateTypeDef

```python
# ListExportsRequestPaginateTypeDef definition

class ListExportsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesRequestPaginateTypeDef

```python
# ListTablesRequestPaginateTypeDef definition

class ListTablesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## S3DestinationTypeDef

```python
# S3DestinationTypeDef definition

class S3DestinationTypeDef(TypedDict):
    S3Bucket: str,
    S3OutputConfigurations: S3OutputConfigurationsTypeDef,  # (1)
    S3Prefix: str,
    S3Region: str,
```

1. See [:material-code-braces: S3OutputConfigurationsTypeDef](./type_defs.md#s3outputconfigurationstypedef) 
## TableTypeDef

```python
# TableTypeDef definition

class TableTypeDef(TypedDict):
    Description: NotRequired[str],
    TableName: NotRequired[str],
    TableProperties: NotRequired[List[TablePropertyDescriptionTypeDef]],  # (1)
```

1. See [:material-code-braces: TablePropertyDescriptionTypeDef](./type_defs.md#tablepropertydescriptiontypedef) 
## ListExecutionsResponseTypeDef

```python
# ListExecutionsResponseTypeDef definition

class ListExecutionsResponseTypeDef(TypedDict):
    Executions: List[ExecutionReferenceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExecutionReferenceTypeDef](./type_defs.md#executionreferencetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExportsResponseTypeDef

```python
# ListExportsResponseTypeDef definition

class ListExportsResponseTypeDef(TypedDict):
    Exports: List[ExportReferenceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportReferenceTypeDef](./type_defs.md#exportreferencetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationConfigurationsTypeDef

```python
# DestinationConfigurationsTypeDef definition

class DestinationConfigurationsTypeDef(TypedDict):
    S3Destination: S3DestinationTypeDef,  # (1)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
## ListTablesResponseTypeDef

```python
# ListTablesResponseTypeDef definition

class ListTablesResponseTypeDef(TypedDict):
    Tables: List[TableTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportOutputTypeDef

```python
# ExportOutputTypeDef definition

class ExportOutputTypeDef(TypedDict):
    DataQuery: DataQueryOutputTypeDef,  # (1)
    DestinationConfigurations: DestinationConfigurationsTypeDef,  # (2)
    Name: str,
    RefreshCadence: RefreshCadenceTypeDef,  # (3)
    Description: NotRequired[str],
    ExportArn: NotRequired[str],
```

1. See [:material-code-braces: DataQueryOutputTypeDef](./type_defs.md#dataqueryoutputtypedef) 
2. See [:material-code-braces: DestinationConfigurationsTypeDef](./type_defs.md#destinationconfigurationstypedef) 
3. See [:material-code-braces: RefreshCadenceTypeDef](./type_defs.md#refreshcadencetypedef) 
## ExportTypeDef

```python
# ExportTypeDef definition

class ExportTypeDef(TypedDict):
    DataQuery: DataQueryUnionTypeDef,  # (1)
    DestinationConfigurations: DestinationConfigurationsTypeDef,  # (2)
    Name: str,
    RefreshCadence: RefreshCadenceTypeDef,  # (3)
    Description: NotRequired[str],
    ExportArn: NotRequired[str],
```

1. See [:material-code-braces: DataQueryTypeDef](./type_defs.md#dataquerytypedef) [:material-code-braces: DataQueryOutputTypeDef](./type_defs.md#dataqueryoutputtypedef) 
2. See [:material-code-braces: DestinationConfigurationsTypeDef](./type_defs.md#destinationconfigurationstypedef) 
3. See [:material-code-braces: RefreshCadenceTypeDef](./type_defs.md#refreshcadencetypedef) 
## GetExecutionResponseTypeDef

```python
# GetExecutionResponseTypeDef definition

class GetExecutionResponseTypeDef(TypedDict):
    ExecutionId: str,
    ExecutionStatus: ExecutionStatusTypeDef,  # (1)
    Export: ExportOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ExecutionStatusTypeDef](./type_defs.md#executionstatustypedef) 
2. See [:material-code-braces: ExportOutputTypeDef](./type_defs.md#exportoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExportResponseTypeDef

```python
# GetExportResponseTypeDef definition

class GetExportResponseTypeDef(TypedDict):
    Export: ExportOutputTypeDef,  # (1)
    ExportStatus: ExportStatusTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ExportOutputTypeDef](./type_defs.md#exportoutputtypedef) 
2. See [:material-code-braces: ExportStatusTypeDef](./type_defs.md#exportstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExportRequestRequestTypeDef

```python
# CreateExportRequestRequestTypeDef definition

class CreateExportRequestRequestTypeDef(TypedDict):
    Export: ExportTypeDef,  # (1)
    ResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (2)
```

1. See [:material-code-braces: ExportTypeDef](./type_defs.md#exporttypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## UpdateExportRequestRequestTypeDef

```python
# UpdateExportRequestRequestTypeDef definition

class UpdateExportRequestRequestTypeDef(TypedDict):
    Export: ExportTypeDef,  # (1)
    ExportArn: str,
```

1. See [:material-code-braces: ExportTypeDef](./type_defs.md#exporttypedef) 
