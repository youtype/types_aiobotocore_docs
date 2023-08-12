# Type definitions

> [Index](../README.md) > [Honeycode](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Honeycode](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
    type annotations stubs module [types-aiobotocore-honeycode](https://pypi.org/project/types-aiobotocore-honeycode/).



## FailedBatchItemTypeDef

```python
# FailedBatchItemTypeDef definition

class FailedBatchItemTypeDef(TypedDict):
    id: str,
    errorMessage: str,
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

## BatchDeleteTableRowsRequestRequestTypeDef

```python
# BatchDeleteTableRowsRequestRequestTypeDef definition

class BatchDeleteTableRowsRequestRequestTypeDef(TypedDict):
    workbookId: str,
    tableId: str,
    rowIds: Sequence[str],
    clientRequestToken: NotRequired[str],
```

## UpsertRowsResultTypeDef

```python
# UpsertRowsResultTypeDef definition

class UpsertRowsResultTypeDef(TypedDict):
    rowIds: List[str],
    upsertAction: UpsertActionType,  # (1)
```

1. See [:material-code-brackets: UpsertActionType](./literals.md#upsertactiontype) 
## CellInputTypeDef

```python
# CellInputTypeDef definition

class CellInputTypeDef(TypedDict):
    fact: NotRequired[str],
    facts: NotRequired[Sequence[str]],
```

## CellTypeDef

```python
# CellTypeDef definition

class CellTypeDef(TypedDict):
    formula: NotRequired[str],
    format: NotRequired[FormatType],  # (1)
    rawValue: NotRequired[str],
    formattedValue: NotRequired[str],
    formattedValues: NotRequired[List[str]],
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
## ColumnMetadataTypeDef

```python
# ColumnMetadataTypeDef definition

class ColumnMetadataTypeDef(TypedDict):
    name: str,
    format: FormatType,  # (1)
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
## DataItemTypeDef

```python
# DataItemTypeDef definition

class DataItemTypeDef(TypedDict):
    overrideFormat: NotRequired[FormatType],  # (1)
    rawValue: NotRequired[str],
    formattedValue: NotRequired[str],
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
## DelimitedTextImportOptionsTypeDef

```python
# DelimitedTextImportOptionsTypeDef definition

class DelimitedTextImportOptionsTypeDef(TypedDict):
    delimiter: str,
    hasHeaderRow: NotRequired[bool],
    ignoreEmptyRows: NotRequired[bool],
    dataCharacterEncoding: NotRequired[ImportDataCharacterEncodingType],  # (1)
```

1. See [:material-code-brackets: ImportDataCharacterEncodingType](./literals.md#importdatacharacterencodingtype) 
## DescribeTableDataImportJobRequestRequestTypeDef

```python
# DescribeTableDataImportJobRequestRequestTypeDef definition

class DescribeTableDataImportJobRequestRequestTypeDef(TypedDict):
    workbookId: str,
    tableId: str,
    jobId: str,
```

## SourceDataColumnPropertiesTypeDef

```python
# SourceDataColumnPropertiesTypeDef definition

class SourceDataColumnPropertiesTypeDef(TypedDict):
    columnIndex: NotRequired[int],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    formula: str,
    contextRowId: NotRequired[str],
```

## VariableValueTypeDef

```python
# VariableValueTypeDef definition

class VariableValueTypeDef(TypedDict):
    rawValue: str,
```

## ImportDataSourceConfigTypeDef

```python
# ImportDataSourceConfigTypeDef definition

class ImportDataSourceConfigTypeDef(TypedDict):
    dataSourceUrl: NotRequired[str],
```

## ImportJobSubmitterTypeDef

```python
# ImportJobSubmitterTypeDef definition

class ImportJobSubmitterTypeDef(TypedDict):
    email: NotRequired[str],
    userArn: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListTableColumnsRequestRequestTypeDef

```python
# ListTableColumnsRequestRequestTypeDef definition

class ListTableColumnsRequestRequestTypeDef(TypedDict):
    workbookId: str,
    tableId: str,
    nextToken: NotRequired[str],
```

## TableColumnTypeDef

```python
# TableColumnTypeDef definition

class TableColumnTypeDef(TypedDict):
    tableColumnId: NotRequired[str],
    tableColumnName: NotRequired[str],
    format: NotRequired[FormatType],  # (1)
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
## ListTableRowsRequestRequestTypeDef

```python
# ListTableRowsRequestRequestTypeDef definition

class ListTableRowsRequestRequestTypeDef(TypedDict):
    workbookId: str,
    tableId: str,
    rowIds: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTablesRequestRequestTypeDef

```python
# ListTablesRequestRequestTypeDef definition

class ListTablesRequestRequestTypeDef(TypedDict):
    workbookId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## TableTypeDef

```python
# TableTypeDef definition

class TableTypeDef(TypedDict):
    tableId: NotRequired[str],
    tableName: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
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

## BatchCreateTableRowsResultTypeDef

```python
# BatchCreateTableRowsResultTypeDef definition

class BatchCreateTableRowsResultTypeDef(TypedDict):
    workbookCursor: int,
    createdRows: Dict[str, str],
    failedBatchItems: List[FailedBatchItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedBatchItemTypeDef](./type_defs.md#failedbatchitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteTableRowsResultTypeDef

```python
# BatchDeleteTableRowsResultTypeDef definition

class BatchDeleteTableRowsResultTypeDef(TypedDict):
    workbookCursor: int,
    failedBatchItems: List[FailedBatchItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedBatchItemTypeDef](./type_defs.md#failedbatchitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateTableRowsResultTypeDef

```python
# BatchUpdateTableRowsResultTypeDef definition

class BatchUpdateTableRowsResultTypeDef(TypedDict):
    workbookCursor: int,
    failedBatchItems: List[FailedBatchItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedBatchItemTypeDef](./type_defs.md#failedbatchitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvokeScreenAutomationResultTypeDef

```python
# InvokeScreenAutomationResultTypeDef definition

class InvokeScreenAutomationResultTypeDef(TypedDict):
    workbookCursor: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTableDataImportJobResultTypeDef

```python
# StartTableDataImportJobResultTypeDef definition

class StartTableDataImportJobResultTypeDef(TypedDict):
    jobId: str,
    jobStatus: TableDataImportJobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TableDataImportJobStatusType](./literals.md#tabledataimportjobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpsertTableRowsResultTypeDef

```python
# BatchUpsertTableRowsResultTypeDef definition

class BatchUpsertTableRowsResultTypeDef(TypedDict):
    rows: Dict[str, UpsertRowsResultTypeDef],  # (1)
    workbookCursor: int,
    failedBatchItems: List[FailedBatchItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: UpsertRowsResultTypeDef](./type_defs.md#upsertrowsresulttypedef) 
2. See [:material-code-braces: FailedBatchItemTypeDef](./type_defs.md#failedbatchitemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRowDataTypeDef

```python
# CreateRowDataTypeDef definition

class CreateRowDataTypeDef(TypedDict):
    batchItemId: str,
    cellsToCreate: Mapping[str, CellInputTypeDef],  # (1)
```

1. See [:material-code-braces: CellInputTypeDef](./type_defs.md#cellinputtypedef) 
## UpdateRowDataTypeDef

```python
# UpdateRowDataTypeDef definition

class UpdateRowDataTypeDef(TypedDict):
    rowId: str,
    cellsToUpdate: Mapping[str, CellInputTypeDef],  # (1)
```

1. See [:material-code-braces: CellInputTypeDef](./type_defs.md#cellinputtypedef) 
## TableRowTypeDef

```python
# TableRowTypeDef definition

class TableRowTypeDef(TypedDict):
    rowId: str,
    cells: List[CellTypeDef],  # (1)
```

1. See [:material-code-braces: CellTypeDef](./type_defs.md#celltypedef) 
## ResultRowTypeDef

```python
# ResultRowTypeDef definition

class ResultRowTypeDef(TypedDict):
    dataItems: List[DataItemTypeDef],  # (1)
    rowId: NotRequired[str],
```

1. See [:material-code-braces: DataItemTypeDef](./type_defs.md#dataitemtypedef) 
## DestinationOptionsTypeDef

```python
# DestinationOptionsTypeDef definition

class DestinationOptionsTypeDef(TypedDict):
    columnMap: NotRequired[Dict[str, SourceDataColumnPropertiesTypeDef]],  # (1)
```

1. See [:material-code-braces: SourceDataColumnPropertiesTypeDef](./type_defs.md#sourcedatacolumnpropertiestypedef) 
## QueryTableRowsRequestRequestTypeDef

```python
# QueryTableRowsRequestRequestTypeDef definition

class QueryTableRowsRequestRequestTypeDef(TypedDict):
    workbookId: str,
    tableId: str,
    filterFormula: FilterTypeDef,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## UpsertRowDataTypeDef

```python
# UpsertRowDataTypeDef definition

class UpsertRowDataTypeDef(TypedDict):
    batchItemId: str,
    filter: FilterTypeDef,  # (1)
    cellsToUpdate: Mapping[str, CellInputTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: CellInputTypeDef](./type_defs.md#cellinputtypedef) 
## GetScreenDataRequestRequestTypeDef

```python
# GetScreenDataRequestRequestTypeDef definition

class GetScreenDataRequestRequestTypeDef(TypedDict):
    workbookId: str,
    appId: str,
    screenId: str,
    variables: NotRequired[Mapping[str, VariableValueTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) 
## InvokeScreenAutomationRequestRequestTypeDef

```python
# InvokeScreenAutomationRequestRequestTypeDef definition

class InvokeScreenAutomationRequestRequestTypeDef(TypedDict):
    workbookId: str,
    appId: str,
    screenId: str,
    screenAutomationId: str,
    variables: NotRequired[Mapping[str, VariableValueTypeDef]],  # (1)
    rowId: NotRequired[str],
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) 
## ImportDataSourceTypeDef

```python
# ImportDataSourceTypeDef definition

class ImportDataSourceTypeDef(TypedDict):
    dataSourceConfig: ImportDataSourceConfigTypeDef,  # (1)
```

1. See [:material-code-braces: ImportDataSourceConfigTypeDef](./type_defs.md#importdatasourceconfigtypedef) 
## ListTableColumnsRequestListTableColumnsPaginateTypeDef

```python
# ListTableColumnsRequestListTableColumnsPaginateTypeDef definition

class ListTableColumnsRequestListTableColumnsPaginateTypeDef(TypedDict):
    workbookId: str,
    tableId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTableRowsRequestListTableRowsPaginateTypeDef

```python
# ListTableRowsRequestListTableRowsPaginateTypeDef definition

class ListTableRowsRequestListTableRowsPaginateTypeDef(TypedDict):
    workbookId: str,
    tableId: str,
    rowIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesRequestListTablesPaginateTypeDef

```python
# ListTablesRequestListTablesPaginateTypeDef definition

class ListTablesRequestListTablesPaginateTypeDef(TypedDict):
    workbookId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## QueryTableRowsRequestQueryTableRowsPaginateTypeDef

```python
# QueryTableRowsRequestQueryTableRowsPaginateTypeDef definition

class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(TypedDict):
    workbookId: str,
    tableId: str,
    filterFormula: FilterTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTableColumnsResultTypeDef

```python
# ListTableColumnsResultTypeDef definition

class ListTableColumnsResultTypeDef(TypedDict):
    tableColumns: List[TableColumnTypeDef],  # (1)
    nextToken: str,
    workbookCursor: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableColumnTypeDef](./type_defs.md#tablecolumntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTablesResultTypeDef

```python
# ListTablesResultTypeDef definition

class ListTablesResultTypeDef(TypedDict):
    tables: List[TableTypeDef],  # (1)
    nextToken: str,
    workbookCursor: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateTableRowsRequestRequestTypeDef

```python
# BatchCreateTableRowsRequestRequestTypeDef definition

class BatchCreateTableRowsRequestRequestTypeDef(TypedDict):
    workbookId: str,
    tableId: str,
    rowsToCreate: Sequence[CreateRowDataTypeDef],  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: CreateRowDataTypeDef](./type_defs.md#createrowdatatypedef) 
## BatchUpdateTableRowsRequestRequestTypeDef

```python
# BatchUpdateTableRowsRequestRequestTypeDef definition

class BatchUpdateTableRowsRequestRequestTypeDef(TypedDict):
    workbookId: str,
    tableId: str,
    rowsToUpdate: Sequence[UpdateRowDataTypeDef],  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: UpdateRowDataTypeDef](./type_defs.md#updaterowdatatypedef) 
## ListTableRowsResultTypeDef

```python
# ListTableRowsResultTypeDef definition

class ListTableRowsResultTypeDef(TypedDict):
    columnIds: List[str],
    rows: List[TableRowTypeDef],  # (1)
    rowIdsNotFound: List[str],
    nextToken: str,
    workbookCursor: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableRowTypeDef](./type_defs.md#tablerowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryTableRowsResultTypeDef

```python
# QueryTableRowsResultTypeDef definition

class QueryTableRowsResultTypeDef(TypedDict):
    columnIds: List[str],
    rows: List[TableRowTypeDef],  # (1)
    nextToken: str,
    workbookCursor: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableRowTypeDef](./type_defs.md#tablerowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResultSetTypeDef

```python
# ResultSetTypeDef definition

class ResultSetTypeDef(TypedDict):
    headers: List[ColumnMetadataTypeDef],  # (1)
    rows: List[ResultRowTypeDef],  # (2)
```

1. See [:material-code-braces: ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef) 
2. See [:material-code-braces: ResultRowTypeDef](./type_defs.md#resultrowtypedef) 
## ImportOptionsTypeDef

```python
# ImportOptionsTypeDef definition

class ImportOptionsTypeDef(TypedDict):
    destinationOptions: NotRequired[DestinationOptionsTypeDef],  # (1)
    delimitedTextOptions: NotRequired[DelimitedTextImportOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: DestinationOptionsTypeDef](./type_defs.md#destinationoptionstypedef) 
2. See [:material-code-braces: DelimitedTextImportOptionsTypeDef](./type_defs.md#delimitedtextimportoptionstypedef) 
## BatchUpsertTableRowsRequestRequestTypeDef

```python
# BatchUpsertTableRowsRequestRequestTypeDef definition

class BatchUpsertTableRowsRequestRequestTypeDef(TypedDict):
    workbookId: str,
    tableId: str,
    rowsToUpsert: Sequence[UpsertRowDataTypeDef],  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: UpsertRowDataTypeDef](./type_defs.md#upsertrowdatatypedef) 
## GetScreenDataResultTypeDef

```python
# GetScreenDataResultTypeDef definition

class GetScreenDataResultTypeDef(TypedDict):
    results: Dict[str, ResultSetTypeDef],  # (1)
    workbookCursor: int,
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResultSetTypeDef](./type_defs.md#resultsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTableDataImportJobRequestRequestTypeDef

```python
# StartTableDataImportJobRequestRequestTypeDef definition

class StartTableDataImportJobRequestRequestTypeDef(TypedDict):
    workbookId: str,
    dataSource: ImportDataSourceTypeDef,  # (1)
    dataFormat: ImportSourceDataFormatType,  # (2)
    destinationTableId: str,
    importOptions: ImportOptionsTypeDef,  # (3)
    clientRequestToken: str,
```

1. See [:material-code-braces: ImportDataSourceTypeDef](./type_defs.md#importdatasourcetypedef) 
2. See [:material-code-brackets: ImportSourceDataFormatType](./literals.md#importsourcedataformattype) 
3. See [:material-code-braces: ImportOptionsTypeDef](./type_defs.md#importoptionstypedef) 
## TableDataImportJobMetadataTypeDef

```python
# TableDataImportJobMetadataTypeDef definition

class TableDataImportJobMetadataTypeDef(TypedDict):
    submitter: ImportJobSubmitterTypeDef,  # (1)
    submitTime: datetime,
    importOptions: ImportOptionsTypeDef,  # (2)
    dataSource: ImportDataSourceTypeDef,  # (3)
```

1. See [:material-code-braces: ImportJobSubmitterTypeDef](./type_defs.md#importjobsubmittertypedef) 
2. See [:material-code-braces: ImportOptionsTypeDef](./type_defs.md#importoptionstypedef) 
3. See [:material-code-braces: ImportDataSourceTypeDef](./type_defs.md#importdatasourcetypedef) 
## DescribeTableDataImportJobResultTypeDef

```python
# DescribeTableDataImportJobResultTypeDef definition

class DescribeTableDataImportJobResultTypeDef(TypedDict):
    jobStatus: TableDataImportJobStatusType,  # (1)
    message: str,
    jobMetadata: TableDataImportJobMetadataTypeDef,  # (2)
    errorCode: ErrorCodeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: TableDataImportJobStatusType](./literals.md#tabledataimportjobstatustype) 
2. See [:material-code-braces: TableDataImportJobMetadataTypeDef](./type_defs.md#tabledataimportjobmetadatatypedef) 
3. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
